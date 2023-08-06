# Comparing `tmp/widelearning-0.8.4.tar.gz` & `tmp/widelearning-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widelearning-0.8.4.tar", max compression
+gzip compressed data, was "widelearning-0.8.5.tar", max compression
```

## Comparing `widelearning-0.8.4.tar` & `widelearning-0.8.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    27130 2023-07-05 13:06:43.883385 widelearning-0.8.4/README.md
--rw-r--r--   0        0        0      398 2023-07-05 13:09:25.196001 widelearning-0.8.4/pyproject.toml
--rw-r--r--   0        0        0   101725 2023-06-28 17:09:06.514723 widelearning-0.8.4/widelearning.py
--rw-r--r--   0        0        0    28114 2023-07-05 13:09:44.120926 widelearning-0.8.4/setup.py
--rw-r--r--   0        0        0    27769 2023-07-05 13:09:44.122250 widelearning-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0    28498 2023-08-06 15:25:51.733322 widelearning-0.8.5/README.md
+-rw-r--r--   0        0        0      398 2023-08-06 15:30:34.538654 widelearning-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0   117926 2023-08-06 15:26:43.219052 widelearning-0.8.5/widelearning.py
+-rw-r--r--   0        0        0    29504 2023-08-06 15:31:21.706527 widelearning-0.8.5/setup.py
+-rw-r--r--   0        0        0    29137 2023-08-06 15:31:21.707715 widelearning-0.8.5/PKG-INFO
```

### Comparing `widelearning-0.8.4/README.md` & `widelearning-0.8.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,36 @@
         номер слоя, для которого необходимо вывести значения весовых коэффициентов
     name : object
         объект модели нейронной сети
         название переменной, которой присвоена структура модели
 
     Пример использования:
     wdl.show_kernel(0, model)
+    
+### auto_select(neuron, path, label, target)
+
+    Функция для расчета первоначального приближения с автоматическим выбором целевого класса.
+
+    Параметры
+    ----------
+    neuron : int
+        номер нейрона, для которого производится расчет
+    path : str
+        путь к целочисленной обучающей выборке в формате csv 
+    label : str
+        название столбца с метками классов
+    target : str, list
+        параметр, на основании которого выбирается целевой класс
+        1. 'up' - максимальное количество отсеченных экземпляров сверху
+        2. 'mx_ratio' - максимальная доля отсеченных экземпляров к неотсеченным сверху
+        3. [class] - собственный выбор целевого класса, вместо class необходимо добавить название класса в виде строки или числа 
+
+    Пример использования:
+    wdl.auto_select(1, 'KH_train.csv', 'UNS', ['very_low']) 
+    wdl.auto_select(1, 'KH_train.csv', 'UNS', 'mx_ratio')
 
 ### select_top(path, label)
     
     Функция позволяет получить грубое первоначальное приближение вектора весов
 
     Параметры
     ----------
```

### Comparing `widelearning-0.8.4/widelearning.py` & `widelearning-0.8.5/widelearning.py`

 * *Files 4% similar despite different names*

```diff
@@ -2729,12 +2729,439 @@
     output_width = int((width - kernel_size) / stride) + 1
     num_operations = (output_height * output_width * kernel_size * kernel_size * num_kernels * 2)*color_channels
     
     no_bias = (num_operations - ((kernel_size**2)*num_kernels))*color_channels
     print('Кол-во вычислительных операций = ', num_operations)  
     print('Кол-во вычислительных операций (no_bias) = ', no_bias)
 
+def auto_select(neuron, path, label, target):
+    '''
+    Функция для расчета первоначального приближения с автоматическим выбором целевого класса.
 
+    Параметры
+    ----------
+    neuron : int
+        номер нейрона, для которого производится расчет
+    path : str
+        путь к целочисленной обучающей выборке в формате csv 
+    label : str
+        название столбца с метками классов
+    target : str, list
+        параметр, на основании которого выбирается целевой класс
+        1. 'up' - максимальное количество отсеченных экземпляров сверху
+        2. 'mx_ratio' - максимальная доля отсеченных экземпляров к неотсеченным сверху
+        3. [class] - собственный выбор целевого класса, вместо class необходимо добавить название класса в виде строки или числа 
+
+    Пример использования:
+    wdl.auto_select(1, 'KH_train.csv', 'UNS', ['very_low']) 
+    wdl.auto_select(1, 'KH_train.csv', 'UNS', 'mx_ratio') 
+
+    '''
+
+    if(os.path.exists('data') == True):
+        pass
+    else:
+        os.mkdir('data')
+        
+        
+    if(os.path.exists('weights') == True):
+        pass
+    else:
+        os.mkdir('weights')
+    
+    all_classes = pd.read_csv(path)
+    all_classes.drop(all_classes.columns[0], axis=1, inplace=True)
+    
+    uniq = pd.unique(all_classes[[label]].values.ravel('K'))
+    uniq = list(uniq)
+    
+    up_max = 0
+    max_ratio = 0
+    
+    if((target == 'mx_ratio') or (target == 'up')):
+        for o in range(len(uniq)):
+            uniq1 = uniq.copy()
+            z = o
+            top = uniq1[z:z+1]
+            uniq1.remove(top[0])
+            other = uniq1.copy()
+        
+            class_top = all_classes[all_classes[label].isin(top)] 
+            other_classes = all_classes[all_classes[label].isin(other)] 
+        
+        
+            class_top['Scalar_calc'] = ""
+            other_classes['Scalar_calc'] = ""
+        
+            class_top.to_csv('class_top.csv')
+            other_classes.to_csv('other_classes.csv')
+        
+            class_top = pd.read_csv('class_top.csv')
+            other_classes = pd.read_csv('other_classes.csv')
+        
+            class_top.drop(class_top.columns[0], axis=1, inplace=True)
+            other_classes.drop(other_classes.columns[0], axis=1, inplace=True)
+        
+            cl = other_classes.columns
+        
+            columns = []
+            for j in range(1, len(cl)):
+                if(cl[j]=='N'):
+                    break
+                else:
+                    columns.append(cl[j])
+        
+            d = []
+            for c1 in range(len(columns)):
+                z = f'd{c1}'
+                d.append(z)
+        
+            class_top_exp = 1
+            other_classes_exp = -(len(class_top)/len(other_classes))
+        
+            for c2 in range(len(d)):
+                class_top[d[c2]] = ''
+                other_classes[d[c2]] = ''
+        
+            for i1 in range(len(d)):
+                class_top[d[i1]] = class_top[columns[i1]]*class_top_exp
+        
+            for i2 in range(len(d)):
+                other_classes[d[i2]] = other_classes[columns[i2]]*other_classes_exp
+        
+            sm1 = class_top.sum()
+            sm2 = other_classes.sum()
+        
+            weights1 = []
+            for u in range(len(d)):
+                weights1.append(sm1[d[u]])
+        
+            weights2 = []
+            for uu in range(len(d)):
+                weights2.append(sm2[d[uu]]) 
+           
+            weights = [x+y for x, y in zip(weights1, weights2)]
+         
+            for i in range(len(class_top)):
+                xx = class_top.iloc[i]
+                x = []
+                for u in range(len(columns)):
+                    x.append(xx[columns[u]])
+            
+                f = np.array(weights)
+                g = np.array(x)
+                scalar = np.dot(f, g)
+        
+                class_top['Scalar_calc'][i]=scalar
+        
+            class_top = class_top.sort_values(by='Scalar_calc', ascending=False)
+        
+            for j in range(len(other_classes)):
+                xx_other = other_classes.iloc[j]
+                x_other = []
+                for uu in range(len(columns)):
+                    x_other.append(xx_other[columns[uu]])
+            
+                f1 = np.array(weights)
+                g1 = np.array(x_other)
+                scalar1 = np.dot(f1, g1)
+                other_classes['Scalar_calc'][j]=scalar1
+        
+            other_classes = other_classes.sort_values(by='Scalar_calc', ascending=False)
+        
+            up = 0
+            for i in class_top['Scalar_calc']:
+                if(i > other_classes['Scalar_calc'].max()):
+                    up+=1
+                else:
+                    break
+           
+            other_classes.to_csv('other_classes.csv')
+            other_classes = pd.read_csv('other_classes.csv')
+        
+            li = len(other_classes[label]) - 1
+            
+            lastindex_class_other_classes = other_classes[label][li]
+        
+            if((len(other_classes[label]))==1):
+              down = 1
+            else:
+              down = 0
+              for i in range(len(other_classes)-1, 0, -1):
+                if(other_classes[label][i]==lastindex_class_other_classes):
+                    down+=1
+                else:
+                    break
+        
+            other_classes.drop(other_classes.columns[0], axis=1, inplace=True)
+        
+            sum_up_down = up + down
+        
+            class_top_cut = class_top.iloc[up:]
+            other_classes_cut = other_classes.iloc[:-down]
+            
+            del class_top_cut['Scalar_calc']
+            del other_classes_cut['Scalar_calc']
+            
+            for i1 in range(len(d)):
+                del class_top_cut[d[i1]] 
+            
+            for i2 in range(len(d)):
+                del other_classes_cut[d[i2]]
+                
+            print('Количество отсеченных сверху = ', up)
+            print("Количество НЕотсеченных сверху = ", len(class_top_cut))
+            print('Количество отсеченных снизу = ', down)
+            print("Количество НЕотсеченных снизу = ", len(other_classes_cut))
+            print('===Нижняя категория: ', lastindex_class_other_classes)
+            print('СУММА отсеченных сверху и снизу = ', sum_up_down)
+            print('TOP - ', top)
+            print('OTHERS - ', other)    
+            print('+++++++++++++++++++++++++')
+            
+            if(target == 'up'):
+                if(up_max < up):
+                    up_max = up
+                    top_max = top
+                    other_max = other
+                    
+                    if(os.path.exists('tmp') == False):
+                        os.mkdir('tmp')
+                    os.mkdir(f'tmp/train_{top_max}{other_max}')
+        
+                    class_top_cut.to_csv(f'tmp/train_{top_max}{other_max}/class_top_{top_max}{other_max}.csv')
+                    other_classes_cut.to_csv(f'tmp/train_{top_max}{other_max}/other_classes_{top_max}{other_max}.csv')
+            
+                    with open(f'weights/w_{neuron}.txt', 'w') as file:
+                        file.write(str(weights))
+        
+                    folder_path = f'tmp/train_{top_max}{other_max}'
+                    file_list = [file for file in os.listdir(folder_path) if file.endswith('.csv')]
+            
+            if(target == 'mx_ratio'):
+                ratio = up / len(class_top_cut)
+                if(max_ratio < ratio):
+                    max_ratio = ratio
+                    top_max = top
+                    other_max = other
+                
+                    if(os.path.exists('tmp') == False):
+                        os.mkdir('tmp')
+                    os.mkdir(f'tmp/train_{top_max}{other_max}')
+        
+                    class_top_cut.to_csv(f'tmp/train_{top_max}{other_max}/class_top_{top_max}{other_max}.csv')
+                    other_classes_cut.to_csv(f'tmp/train_{top_max}{other_max}/other_classes_{top_max}{other_max}.csv')
+            
+                    with open(f'weights/w_{neuron}.txt', 'w') as file:
+                        file.write(str(weights))
+        
+                    folder_path = f'tmp/train_{top_max}{other_max}'
+                    file_list = [file for file in os.listdir(folder_path) if file.endswith('.csv')]
+        
+        if len(file_list) < 2:
+            print("Должно быть как минимум два CSV файла в папке для объединения.")
+            exit()
+        
+        dfs = [pd.read_csv(os.path.join(folder_path, file)) for file in file_list]
+        merged_df = pd.concat(dfs)
+        merged_df.drop(merged_df.columns[0], axis=1, inplace=True)
+        
+        nn = neuron + 1
+        fldr = 'data'
+        output_path = os.path.join(fldr, f'train_{nn}.csv')
+        
+        merged_df.to_csv(output_path)
+        
+        dr = 'tmp'
+        shutil.rmtree(dr)
+        
+        os.remove('class_top.csv')
+        os.remove('other_classes.csv')
+        
+        if(neuron == 1):
+            train1 = pd.read_csv(path) 
+            train1.drop(train1.columns[0], axis=1, inplace=True)
+            train1.to_csv('data/train_1.csv')
+    
+        print('В качестве целевого выбран класс:', top_max)
+    
+    else:
+        uniq1 = uniq.copy()
+        top = target
+        uniq1.remove(top[0])
+        other = uniq1.copy()
+        
+        class_top = all_classes[all_classes[label].isin(top)] 
+        other_classes = all_classes[all_classes[label].isin(other)] 
+    
+    
+        class_top['Scalar_calc'] = ""
+        other_classes['Scalar_calc'] = ""
+    
+        class_top.to_csv('class_top.csv')
+        other_classes.to_csv('other_classes.csv')
+    
+        class_top = pd.read_csv('class_top.csv')
+        other_classes = pd.read_csv('other_classes.csv')
+    
+        class_top.drop(class_top.columns[0], axis=1, inplace=True)
+        other_classes.drop(other_classes.columns[0], axis=1, inplace=True)
+    
+        cl = other_classes.columns
+    
+        columns = []
+        for j in range(1, len(cl)):
+            if(cl[j]=='N'):
+                break
+            else:
+                columns.append(cl[j])
+    
+        d = []
+        for c1 in range(len(columns)):
+            z = f'd{c1}'
+            d.append(z)
+    
+        class_top_exp = 1
+        other_classes_exp = -(len(class_top)/len(other_classes))
+    
+        for c2 in range(len(d)):
+            class_top[d[c2]] = ''
+            other_classes[d[c2]] = ''
+    
+        for i1 in range(len(d)):
+            class_top[d[i1]] = class_top[columns[i1]]*class_top_exp
+    
+        for i2 in range(len(d)):
+            other_classes[d[i2]] = other_classes[columns[i2]]*other_classes_exp
+    
+        sm1 = class_top.sum()
+        sm2 = other_classes.sum()
+    
+        weights1 = []
+        for u in range(len(d)):
+            weights1.append(sm1[d[u]])
+    
+        weights2 = []
+        for uu in range(len(d)):
+            weights2.append(sm2[d[uu]]) 
+       
+        weights = [x+y for x, y in zip(weights1, weights2)]
+     
+        for i in range(len(class_top)):
+            xx = class_top.iloc[i]
+            x = []
+            for u in range(len(columns)):
+                x.append(xx[columns[u]])
+        
+            f = np.array(weights)
+            g = np.array(x)
+            scalar = np.dot(f, g)
+    
+            class_top['Scalar_calc'][i]=scalar
+    
+        class_top = class_top.sort_values(by='Scalar_calc', ascending=False)
+    
+        for j in range(len(other_classes)):
+            xx_other = other_classes.iloc[j]
+            x_other = []
+            for uu in range(len(columns)):
+                x_other.append(xx_other[columns[uu]])
+        
+            f1 = np.array(weights)
+            g1 = np.array(x_other)
+            scalar1 = np.dot(f1, g1)
+            other_classes['Scalar_calc'][j]=scalar1
+    
+        other_classes = other_classes.sort_values(by='Scalar_calc', ascending=False)
+    
+        up = 0
+        for i in class_top['Scalar_calc']:
+            if(i > other_classes['Scalar_calc'].max()):
+                up+=1
+            else:
+                break
+       
+        other_classes.to_csv('other_classes.csv')
+        other_classes = pd.read_csv('other_classes.csv')
+    
+        li = len(other_classes[label]) - 1
+        
+        lastindex_class_other_classes = other_classes[label][li]
+    
+        if((len(other_classes[label]))==1):
+          down = 1
+        else:
+          down = 0
+          for i in range(len(other_classes)-1, 0, -1):
+            if(other_classes[label][i]==lastindex_class_other_classes):
+                down+=1
+            else:
+                break
+    
+        other_classes.drop(other_classes.columns[0], axis=1, inplace=True)
+    
+        sum_up_down = up + down
+    
+        class_top_cut = class_top.iloc[up:]
+        other_classes_cut = other_classes.iloc[:-down]
+        
+        del class_top_cut['Scalar_calc']
+        del other_classes_cut['Scalar_calc']
+        
+        for i1 in range(len(d)):
+            del class_top_cut[d[i1]] 
+        
+        for i2 in range(len(d)):
+            del other_classes_cut[d[i2]]
+            
+        print('Количество отсеченных сверху = ', up)
+        print("Количество НЕотсеченных сверху = ", len(class_top_cut))
+        print('Количество отсеченных снизу = ', down)
+        print("Количество НЕотсеченных снизу = ", len(other_classes_cut))
+        print('===Нижняя категория: ', lastindex_class_other_classes)
+        print('СУММА отсеченных сверху и снизу = ', sum_up_down)
+        print('TOP - ', top)
+        print('OTHERS - ', other)    
+        print('+++++++++++++++++++++++++')
+    
+            
+        if(os.path.exists('tmp') == False):
+            os.mkdir('tmp')
+        os.mkdir(f'tmp/train_{top}{other}')
+    
+        class_top_cut.to_csv(f'tmp/train_{top}{other}/class_top_{top}{other}.csv')
+        other_classes_cut.to_csv(f'tmp/train_{top}{other}/other_classes_{top}{other}.csv')
+        
+        with open(f'weights/w_{neuron}.txt', 'w') as file:
+            file.write(str(weights))
+    
+        folder_path = f'tmp/train_{top}{other}'
+        file_list = [file for file in os.listdir(folder_path) if file.endswith('.csv')]
+    
+        if len(file_list) < 2:
+            print("Должно быть как минимум два CSV файла в папке для объединения.")
+            exit()
+    
+        dfs = [pd.read_csv(os.path.join(folder_path, file)) for file in file_list]
+        merged_df = pd.concat(dfs)
+        merged_df.drop(merged_df.columns[0], axis=1, inplace=True)
+    
+        nn = neuron + 1
+        fldr = 'data'
+        output_path = os.path.join(fldr, f'train_{nn}.csv')
+    
+        merged_df.to_csv(output_path)
+    
+        dr = 'tmp'
+        shutil.rmtree(dr)
+    
+        os.remove('class_top.csv')
+        os.remove('other_classes.csv')
+    
+        if(neuron == 1):
+            train1 = pd.read_csv(path) 
+            train1.drop(train1.columns[0], axis=1, inplace=True)
+            train1.to_csv('data/train_1.csv')
```

### Comparing `widelearning-0.8.4/setup.py` & `widelearning-0.8.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['widelearning']
 setup_kwargs = {
     'name': 'widelearning',
-    'version': '0.8.4',
+    'version': '0.8.5',
     'description': 'Library for searching the optimal neural network architecture',
-    'long_description': "# wideLearning\n\n[**`Инструкция`**](https://github.com/brinkinvision/wideLearning/tree/main/Туториал) | [**`Github`**](https://github.com/brinkinvision/wideLearning) | [**`GitFlic`**](https://gitflic.ru/project/brinkinvision/wide-learning) | [**`Пример новых вариантов использования`**](https://github.com/brinkinvision/wideLearning/tree/main/Обучение_на_ошибках)\n\n# Минимальные требования к аппаратной части:\n* Операционная система: Windows 7 или выше (64-bit), Linux (64-bit)\n* Оперативная память: не менее 2 GB\n* Процессор: двухъядерный с частотой 1.6 GHz или выше\n* Свободное место на жестком диске: не менее 2 GB\n\n# Направления прикладного использования:\n1. Компьютерное зрение. Упрощение архитектур сверточных нейронных сетей для задач классификации и распознавания изображений, сегментации и детектирования объектов.\n2. Медицинская диагностика. Оптимизация нейронных сетей, используемых при анализе изображений и сигналов, полученных от медицинских приборов. Может использоваться для обнаружения и классификации заболеваний.\n3. Рекомендательные системы. Может использоваться для классификации на основе некоторых признаков контента и выдачи персонализированных рекомендаций.\n4. Развертывание моделей нейронных сетей на устройствах малой вычислительной мощности, например, мобильные гаджеты (смартфоны/планшеты), встраиваемые устройства (промышленные контроллеры/смарт-устройства) и т.п.\n\n# Установка\n```\npip install widelearning\n```\n\n# Импорт библиотеки\n```\nimport widelearning as wdl \n```\n\n# Описание функций\n\n### txt_kernel(file_path)\t\n    \n    Функция преобразования сгенерированного ядра для вставки в структуру TensorFlow \n    (для черно-белых, одноканальных изображений)\n\n    Параметры\n    ----------\n    file_path : str\n        путь к текстовому файлу, содержащему сверточное ядро, записанное в следующем виде \n        (с запятыми в конце каждой строки)\n        1,2,3,\n        4,5,6,\n        7,8,9,\n\n    Пример использования:\n    wdl.txt_kernel('horizontal.txt')\n\n### txt_kernel_rgb(k1, k2, k3) \n    \n    Функция преобразования сгенерированного ядра для вставки в структуру TensorFlow \n    (для цветных, трехканальных изображений)\n    \n    Параметры\n    ----------\n    k1 : str\n        путь к текстовому файлу, содержащему сверточное ядро первого цветового канала R, записанное в следующем виде \n        (с запятыми в конце каждой строки)\n        1,2,3,\n        4,5,6,\n        7,8,9,\n    k2 : str\n        путь к текстовому файлу, содержащему сверточное ядро второго цветового канала G\n    k3 : str\n        путь к текстовому файлу, содержащему сверточное ядро третьего цветового канала B\n\n    Пример использования:\n    wdl.txt_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt')\n\n### add_kernel(path, init_kernel)\n    \n    Функция позволяет устанавливать дополнительные ядра сверточного слоя к уже установленным исходным\n    (для черно-белых, одноканальных изображений)\n\n    Параметры\n    ----------\n    path : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра, \n        добавляемого к исходным\n    init_kernel : list\n        значения исходного/ых ядер, к которым происходит добавление. \n        Это может быть либо переменная, которой присвоено значение исходных ядер, \n        либо сами значения, полученные после преобразования с помощью функции txt_kernel:\n        [[[[1]], [[2]], [[3]]], [[[4]], [[5]], [[6]]], [[[7]], [[8]], [[9]]]].\n\n    Пример использования:\n    wdl.add_kernel('vertical.txt', w1)\n    \n### add_kernel_rgb(k1, k2, k3, w)\n    \n    Функция позволяет устанавливать дополнительные ядра сверточного слоя к уже установленным исходным\n    (для цветных, трехканальных изображений)\n\n    Параметры\n    ----------\n    path : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра, \n        добавляемого к исходным\n    init_kernel : list\n        значения исходного/ых ядер, к которым происходит добавление. \n        Это может быть либо переменная, которой присвоено значение исходных ядер, \n        либо сами значения, полученные после преобразования с помощью функции txt_kernel_rgb\n\n    Параметры\n    ----------\n    k1 : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра первого цветового канала R, \n        добавляемого к исходным в данном цветовом канале\n    k2 : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра второго цветового канала G, \n        добавляемого к исходным в данном цветовом канале\n    k3 : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра первого цветового канала B, \n        добавляемого к исходным в данном цветовом канале\n    w : list\n        значения исходного/ых ядер, к которым происходит добавление. \n        Это может быть либо переменная, которой присвоено значение исходных ядер, \n        либо сами значения, полученные после преобразования с помощью функции txt_kernel_rgb\n\n    Пример использования:\n    wdl.add_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt', w1)\n\n### horizontal(dim, values)\n    \n    Функция для генерации линейного сверточного ядра горизонтального типа\n\n    Параметры\n    ----------\n    dim : int\n        размерность генерируемой матрицы \n    values : list\n        список значений, которые будут использоваться для заполнения матрицы.\n\n    Пример использования:\n    wdl.horizontal(32, [-7,-5,-3,-1,1,3,5,7])\n\t\n### vertical(dim, values)\n    \n    Функция для генерации линейного сверточного ядра вертикального типа\n\n    Параметры\n    ----------\n    dim : int\n        размерность генерируемой матрицы \n    values : list\n        список значений, которые будут использоваться для заполнения матрицы.\n\n    Пример использования:\n    wdl.vertical(32, [-7,-5,-3,-1,1,3,5,7])\n\n### diagonal(up, down, d, dimension)\n    \n    Функция для генерации линейного сверточного ядра диагонального типа\n\n    Parameters\n    ----------\n    up : list\n        список значений, которые будут размещены над диагональю выходной матрицы\n    down : list\n        список значений, которые будут размещены ниже диагонали\n    d : int\n        значение, из которого состоит диагональ.\n    dimension : int\n        размерность генерируемого ядра\n\n    Пример использования:\n    wdl.diagonal([-7, -5, -3, -1], [1, 3, 5, 7], 1, 32)\t\n\t\n### show_kernel(N, name)\n    \n    Функция вывода коэффициентов сверточного ядра на экран пользователя\n\n    Параметры\n    ----------\n    N : int\n        номер слоя, для которого необходимо вывести значения весовых коэффициентов\n    name : object\n        объект модели нейронной сети\n        название переменной, которой присвоена структура модели\n\n    Пример использования:\n    wdl.show_kernel(0, model)\n\n### select_top(path, label)\n    \n    Функция позволяет получить грубое первоначальное приближение вектора весов\n\n    Параметры\n    ----------\n    path : str\n        путь к целочисленной обучающей выборке в формате csv\n    label : str\n        название столбца с метками классов\n\n    Пример использования:\n    wdl.select_top('KAHRAMAN_train.csv', 'UNS')\n\n### select_top_binary(path, label)\n    \n    Функция позволяет получить грубое первоначальное приближение вектора весов для бинарной обучающей выборки\n\n    Параметры\n    ----------\n    path : str\n        путь к целочисленной бинарной обучающей выборке в формате csv\n    label : str\n        название столбца с метками классов\n\n    Пример использования:\n    wdl.select_top_binary('train_6.csv', 'UNS')\n\n### grad_boost(path, t, oth, l, s, from_initial, weights_main)\n    \n    Вспомогательная функция для корректировки весовых коэффициентов с помощью градиентного уточнения, одиночный проход по вектору\n\n    Параметры\n    ----------\n    path : str\n        путь к обучающей выборке, подаваемой на вход функции select_top\n    t : list\n        метка выбранного на этапе первоначального приближения целевого класса\n    oth : list\n        список, содержащий метки оставшихся классов, которые не относятся к целевому\n    l : str\n        название столбца с метками классов\n    s : int\n        шаг изменения значений элементов вектора весов, шаг градиентного уточнения;\n    from_initial : int\n        1, если вектор берется из select_top (грубое приближение), \n        0 - если вектор снова корректируется (после grad_boost)\n    weights_main : list\n        вектор весов для корректировки\n\n### grad_boost_save_files(path, t, oth, l, s, from_initial, weights_main)\n    \n    Вспомогательная функция для сохранения усеченных обучающих выборок и скорректированных векторов весов после градиентного уточнения\n\n    Параметры\n    ----------\n    path : str\n        путь к обучающей выборке, подаваемой на вход функции select_top\n    t : list\n        метка выбранного на этапе первоначального приближения целевого класса\n    oth : list\n        список, содержащий метки оставшихся классов, которые не относятся к целевому\n    l : str\n        название столбца с метками классов\n    s : int\n        шаг изменения значений элементов вектора весов, шаг градиентного уточнения;\n    from_initial : int\n        1, если вектор берется из select_top (грубое приближение), \n        0 - если вектор снова корректируется (после grad_boost)\n    weights_main : list\n        вектор весов для корректировки\n\n### grad(path, t, oth, l, s, weights)\n    \n    Функция осуществляет градиентное уточнение полученного после первоначального приближения вектора весов \n\n    Параметры\n    ----------\n    path : str\n        путь к обучающей выборке, подаваемой на вход функции select_top\n    t : list\n        метка выбранного на этапе первоначального приближения целевого класса\n    oth : list\n        список, содержащий метки оставшихся классов, которые не относятся к целевому\n    l : str\n        название столбца с метками классов\n    s : int\n        шаг изменения значений элементов вектора весов, шаг градиентного уточнения\n    weights_main : list\n        вектор весов, значения которого необходимо изменить с целью получения большего количества \n        отсеченных экземпляров обучающей выборки\n\n    Пример использования:\n    wdl.grad('KAHRAMAN_train.csv', ['High'], ['very_low', 'Low', 'Middle'], 'UNS', 1, [455.02247191011236, 552.8764044943821, 273.38202247191015, 518.2921348314607, 2276.179775280899])\n\t\n### grad_binary(path, t, oth, l, s, weights_main)\n    \n    Функция осуществляет градиентное уточнение полученного после первоначального приближения вектора весов \n    для бинарной обучающей выборки\n\n    Параметры\n    ----------\n    path : str\n        путь к бинарной обучающей выборке, подаваемой на вход функции select_top\n    t : list\n        метка выбранного на этапе первоначального приближения целевого класса\n    oth : list\n        список, содержащий метки оставшихся классов, которые не относятся к целевому\n    l : str\n        название столбца с метками классов\n    s : int\n        шаг изменения значений элементов вектора весов, шаг градиентного уточнения\n    weights_main : list\n        вектор весов, значения которого необходимо изменить с целью получения большего количества \n        отсеченных экземпляров обучающей выборки\n\n    Пример использования:\n    wdl.grad_binary('train_6.csv', ['Low'], ['Middle'], 'UNS', 1, [1009.0, 48.0, -929.0, -1056.0, -13.0])\n\n### data_int(path, decimal, name)\n    \n    Функция преобразует набор данных, представленный в вещественнозначном виде в целочисленный вид\n\n    Параметры\n    ----------\n    path : str\n        путь к обучающей выборке в формате csv\n    decimal : str\n        путь к текстовому файлу, содержащему в каждой строке число, обозначающее количество десятичных знаков после \n        запятой в соответствующем столбце выборки\n    name : str\n        аргумент функции, обозначающий желаемое название выходных генерируемых файлов\n\n    Пример использования:\n    wdl.data_int('kahraman.csv', 'dec.txt', 'KAHRAMAN') \n\n### scale_weights(label, data_folder, weights_folder)\n    \n    Функция для масштабирования полученных векторов весов в диапазон от -1 до +1\n\n    Параметры\n    ----------\n    label : str\n        название столбца с метками классов\n    data_folder : str\n        путь к папке, содержащей обучающие выборки каждого нейрона\n    weights_folder : str\n        путь к папке, содержащей веса каждого нейрона\n\n    Пример использования:\n    wdl.scale_weights('UNS', 'data/', 'weights/')\n\n### generate_fa(label, data_folder, weights_folder)\n    \n    Функция, которая на основании проведенного обучения модифицированного полносвязного слоя, генерирует вложенную \n    логическую функцию активации для проверки весовых коэффициентов на тестовых данных\n\n    Параметры\n    ----------\n    label : str\n        название столбца обучающих выборок, в котором содержатся наименования (метки) классов\n    data_folder : str\n        путь к папке result, сгенерированной в результате выполнения функции scale_weights\n    weights_folder : str\n        путь к каталогу scale, который сгенерирован после применения функции scale_weights\n\n    Пример использования:\n    wdl.generate_fa('UNS', 'result', 'scale')\n\n### check_test(train, weights, test, label)\n    \n    Функция осуществляет проверку обучения с помощью правил логического вывода\n\n    Параметры\n    ----------\n    train : str\n        путь к полной целочисленной обучающей выборке\n    weights : str\n        путь к текстовому файлу weights.txt из сгенерированного каталога all_weights после функции scale_weights\n    test : str\n        путь к целочисленной тестовой выборке (в случае проверки обучающей выборки передается путь к полной обучающей выборке, \n        аналогичный параметру train)\n    label : str\n        название столбца с метками классов\n\n    Пример использования:\n    wdl.check_test('train_1.csv', 'weights.txt', 'KAHRAMAN_test.csv', 'UNS')\n\n### getNameColumn(nameFileTrain)\n    \n    Вспомогательная функция для определения названий всех столбцов, кроме столбца с метками классов\n\n    Параметры\n    ----------\n    nameFileTrain : str\n        путь к обучающей выборке \n\n### getCountNeuronSizeVector(nameFileTrain)\n    \n    Вспомогательная функция для определения необходимого количества нейронов в слое\n\n    Параметры\n    ----------\n    nameFileTrain : str\n        путь к обучающей выборке \n\n### initializingDictionaryKeys()\n    \n    Вспомогательная функция для инициализации ключей для правила логического вывода\n\n### initializationDictionaryValues(nameFileTrain)\n    \n    Вспомогательная функция для создания словаря логического вывода\n\n    Параметры\n    ----------\n    nameFileTrain : str\n        путь к обучающей выборке \n\n### count_conv_operations(height, width, color_channels, kernel_size, stride, num_kernels)\n    \n    Функция для подсчета количества вычислительных операций в сверточном слое \n\n    Параметры\n    ----------\n    height : int\n        высота исходного изображения выборки данных\n    width : int\n        ширина исходного изображения\n    color_channels : int\n        количество цветовых каналов изображения \n        (1 – если изображение представлено в черно-белом одноканальном виде, 3 – если изображение является цветным)\n    kernel_size : int\n        размерность сверточного ядра квадратной формы\n    stride : int\n        шаг прохода сверточного ядра по изображению\n    num_kernels : int\n        количество сверточных ядер в слое\n\n    Пример использования:\n    wdl.count_conv_operations(28, 28, 1, 14, 7, 4)\n\n# Шаблоны вызова функций сверточного слоя\n```\nwdl.txt_kernel('путь_к_сгенерированному_ядру.txt')\n```\n```\nwdl.txt_kernel_rgb('путь_к_сгенерированному_ядру_ПЕРВОГО_цветового_канала.txt', 'путь_к_сгенерированному_ядру_ВТОРОГО_цветового_канала.txt', 'путь_к_сгенерированному_ядру_ТРЕТЬЕГО_цветового_канала.txt')\n```\n```\nwdl.add_kernel('путь_к_добавляемому_ядру.txt', переменная_уже_установленных_ядер)\n```\n```\nwdl.add_kernel_rgb('путь_к_добавляемому_ядру_ПЕРВОГО_цветового_канала.txt', 'путь_к_добавляемому_ядру_ВТОРОГО_цветового_канала.txt', 'путь_к_добавляемому_ядру_ТРЕТЬЕГО_цветового_канала.txt', переменная_уже_установленных_ядер)\n```\n```\nwdl.horizontal(размерность_ядра, [список_значений_ядра])\n```\n```\nwdl.vertical(размерность_ядра, [список_значений_ядра])\n```\n```\nwdl.diagonal([список_значений_выше_диагонали], [список_значений_ниже_диагонали], значение_диагонали, размерность_ядра)\n```\n```\nwdl.show_kernel(номер_сверточного_слоя, объект_модели)\n```\n```\nwdl.count_conv_operations(высота_изображения, ширина_изображения, количество_цветовых_каналов, размерность_квадратного_ядра, шаг_ядра, количество_ядер)\n```\n\n# Шаблоны вызова функций полносвязного слоя\n```\nwdl.data_int('путь_к_обучающей_выборке.csv', 'путь_к_файлу_со_значениями_кол-ва_знаков_после_запятой.txt', 'название_выходных_файлов')\n```\n```\nwdl.select_top('путь_к_целочисленной_обучающей_выборке.csv', 'название_столбца_с_метками_классов')\n```\n```\nwdl.select_top_binary('путь_к_целочисленной_обучающей_выборке.csv', 'название_столбца_с_метками_классов')\n```\n```\nwdl.grad('путь_к_целочисленной_обучающей_выборке.csv', [целевой_класс], [список_остальных_классов], 'название_столбца_с_метками_классов', шаг, [вектор_весов])\n```\n```\nwdl.grad_binary('путь_к_целочисленной_обучающей_выборке.csv', [целевой_класс], [список_остальных_классов], 'название_столбца_с_метками_классов', шаг, [вектор_весов])\n```\n```\nwdl.scale_weights('название_столбца_с_метками_классов', 'путь_к_папке_с_обучающими_выборками', 'путь_к_папке_с_весами')\n```\n```\nwdl.generate_fa('название_столбца_с_метками_классов', 'путь_к_папке_result', 'путь_к_папке_scale')\n```\n```\nwdl.check_test('путь_к_полной_обучающей_выборке.csv', 'путь_к_файлу_со_всеми_весами.txt', 'путь_к_тестовой_выборке.csv', 'название_столбца_с_метками_классов')\n```\n",
+    'long_description': "# wideLearning\n\n[**`Инструкция`**](https://github.com/brinkinvision/wideLearning/tree/main/Туториал) | [**`Github`**](https://github.com/brinkinvision/wideLearning) | [**`GitFlic`**](https://gitflic.ru/project/brinkinvision/wide-learning) | [**`Пример новых вариантов использования`**](https://github.com/brinkinvision/wideLearning/tree/main/Обучение_на_ошибках)\n\n# Минимальные требования к аппаратной части:\n* Операционная система: Windows 7 или выше (64-bit), Linux (64-bit)\n* Оперативная память: не менее 2 GB\n* Процессор: двухъядерный с частотой 1.6 GHz или выше\n* Свободное место на жестком диске: не менее 2 GB\n\n# Направления прикладного использования:\n1. Компьютерное зрение. Упрощение архитектур сверточных нейронных сетей для задач классификации и распознавания изображений, сегментации и детектирования объектов.\n2. Медицинская диагностика. Оптимизация нейронных сетей, используемых при анализе изображений и сигналов, полученных от медицинских приборов. Может использоваться для обнаружения и классификации заболеваний.\n3. Рекомендательные системы. Может использоваться для классификации на основе некоторых признаков контента и выдачи персонализированных рекомендаций.\n4. Развертывание моделей нейронных сетей на устройствах малой вычислительной мощности, например, мобильные гаджеты (смартфоны/планшеты), встраиваемые устройства (промышленные контроллеры/смарт-устройства) и т.п.\n\n# Установка\n```\npip install widelearning\n```\n\n# Импорт библиотеки\n```\nimport widelearning as wdl \n```\n\n# Описание функций\n\n### txt_kernel(file_path)\t\n    \n    Функция преобразования сгенерированного ядра для вставки в структуру TensorFlow \n    (для черно-белых, одноканальных изображений)\n\n    Параметры\n    ----------\n    file_path : str\n        путь к текстовому файлу, содержащему сверточное ядро, записанное в следующем виде \n        (с запятыми в конце каждой строки)\n        1,2,3,\n        4,5,6,\n        7,8,9,\n\n    Пример использования:\n    wdl.txt_kernel('horizontal.txt')\n\n### txt_kernel_rgb(k1, k2, k3) \n    \n    Функция преобразования сгенерированного ядра для вставки в структуру TensorFlow \n    (для цветных, трехканальных изображений)\n    \n    Параметры\n    ----------\n    k1 : str\n        путь к текстовому файлу, содержащему сверточное ядро первого цветового канала R, записанное в следующем виде \n        (с запятыми в конце каждой строки)\n        1,2,3,\n        4,5,6,\n        7,8,9,\n    k2 : str\n        путь к текстовому файлу, содержащему сверточное ядро второго цветового канала G\n    k3 : str\n        путь к текстовому файлу, содержащему сверточное ядро третьего цветового канала B\n\n    Пример использования:\n    wdl.txt_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt')\n\n### add_kernel(path, init_kernel)\n    \n    Функция позволяет устанавливать дополнительные ядра сверточного слоя к уже установленным исходным\n    (для черно-белых, одноканальных изображений)\n\n    Параметры\n    ----------\n    path : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра, \n        добавляемого к исходным\n    init_kernel : list\n        значения исходного/ых ядер, к которым происходит добавление. \n        Это может быть либо переменная, которой присвоено значение исходных ядер, \n        либо сами значения, полученные после преобразования с помощью функции txt_kernel:\n        [[[[1]], [[2]], [[3]]], [[[4]], [[5]], [[6]]], [[[7]], [[8]], [[9]]]].\n\n    Пример использования:\n    wdl.add_kernel('vertical.txt', w1)\n    \n### add_kernel_rgb(k1, k2, k3, w)\n    \n    Функция позволяет устанавливать дополнительные ядра сверточного слоя к уже установленным исходным\n    (для цветных, трехканальных изображений)\n\n    Параметры\n    ----------\n    path : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра, \n        добавляемого к исходным\n    init_kernel : list\n        значения исходного/ых ядер, к которым происходит добавление. \n        Это может быть либо переменная, которой присвоено значение исходных ядер, \n        либо сами значения, полученные после преобразования с помощью функции txt_kernel_rgb\n\n    Параметры\n    ----------\n    k1 : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра первого цветового канала R, \n        добавляемого к исходным в данном цветовом канале\n    k2 : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра второго цветового канала G, \n        добавляемого к исходным в данном цветовом канале\n    k3 : str\n        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра первого цветового канала B, \n        добавляемого к исходным в данном цветовом канале\n    w : list\n        значения исходного/ых ядер, к которым происходит добавление. \n        Это может быть либо переменная, которой присвоено значение исходных ядер, \n        либо сами значения, полученные после преобразования с помощью функции txt_kernel_rgb\n\n    Пример использования:\n    wdl.add_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt', w1)\n\n### horizontal(dim, values)\n    \n    Функция для генерации линейного сверточного ядра горизонтального типа\n\n    Параметры\n    ----------\n    dim : int\n        размерность генерируемой матрицы \n    values : list\n        список значений, которые будут использоваться для заполнения матрицы.\n\n    Пример использования:\n    wdl.horizontal(32, [-7,-5,-3,-1,1,3,5,7])\n\t\n### vertical(dim, values)\n    \n    Функция для генерации линейного сверточного ядра вертикального типа\n\n    Параметры\n    ----------\n    dim : int\n        размерность генерируемой матрицы \n    values : list\n        список значений, которые будут использоваться для заполнения матрицы.\n\n    Пример использования:\n    wdl.vertical(32, [-7,-5,-3,-1,1,3,5,7])\n\n### diagonal(up, down, d, dimension)\n    \n    Функция для генерации линейного сверточного ядра диагонального типа\n\n    Parameters\n    ----------\n    up : list\n        список значений, которые будут размещены над диагональю выходной матрицы\n    down : list\n        список значений, которые будут размещены ниже диагонали\n    d : int\n        значение, из которого состоит диагональ.\n    dimension : int\n        размерность генерируемого ядра\n\n    Пример использования:\n    wdl.diagonal([-7, -5, -3, -1], [1, 3, 5, 7], 1, 32)\t\n\t\n### show_kernel(N, name)\n    \n    Функция вывода коэффициентов сверточного ядра на экран пользователя\n\n    Параметры\n    ----------\n    N : int\n        номер слоя, для которого необходимо вывести значения весовых коэффициентов\n    name : object\n        объект модели нейронной сети\n        название переменной, которой присвоена структура модели\n\n    Пример использования:\n    wdl.show_kernel(0, model)\n    \n### auto_select(neuron, path, label, target)\n\n    Функция для расчета первоначального приближения с автоматическим выбором целевого класса.\n\n    Параметры\n    ----------\n    neuron : int\n        номер нейрона, для которого производится расчет\n    path : str\n        путь к целочисленной обучающей выборке в формате csv \n    label : str\n        название столбца с метками классов\n    target : str, list\n        параметр, на основании которого выбирается целевой класс\n        1. 'up' - максимальное количество отсеченных экземпляров сверху\n        2. 'mx_ratio' - максимальная доля отсеченных экземпляров к неотсеченным сверху\n        3. [class] - собственный выбор целевого класса, вместо class необходимо добавить название класса в виде строки или числа \n\n    Пример использования:\n    wdl.auto_select(1, 'KH_train.csv', 'UNS', ['very_low']) \n    wdl.auto_select(1, 'KH_train.csv', 'UNS', 'mx_ratio')\n\n### select_top(path, label)\n    \n    Функция позволяет получить грубое первоначальное приближение вектора весов\n\n    Параметры\n    ----------\n    path : str\n        путь к целочисленной обучающей выборке в формате csv\n    label : str\n        название столбца с метками классов\n\n    Пример использования:\n    wdl.select_top('KAHRAMAN_train.csv', 'UNS')\n\n### select_top_binary(path, label)\n    \n    Функция позволяет получить грубое первоначальное приближение вектора весов для бинарной обучающей выборки\n\n    Параметры\n    ----------\n    path : str\n        путь к целочисленной бинарной обучающей выборке в формате csv\n    label : str\n        название столбца с метками классов\n\n    Пример использования:\n    wdl.select_top_binary('train_6.csv', 'UNS')\n\n### grad_boost(path, t, oth, l, s, from_initial, weights_main)\n    \n    Вспомогательная функция для корректировки весовых коэффициентов с помощью градиентного уточнения, одиночный проход по вектору\n\n    Параметры\n    ----------\n    path : str\n        путь к обучающей выборке, подаваемой на вход функции select_top\n    t : list\n        метка выбранного на этапе первоначального приближения целевого класса\n    oth : list\n        список, содержащий метки оставшихся классов, которые не относятся к целевому\n    l : str\n        название столбца с метками классов\n    s : int\n        шаг изменения значений элементов вектора весов, шаг градиентного уточнения;\n    from_initial : int\n        1, если вектор берется из select_top (грубое приближение), \n        0 - если вектор снова корректируется (после grad_boost)\n    weights_main : list\n        вектор весов для корректировки\n\n### grad_boost_save_files(path, t, oth, l, s, from_initial, weights_main)\n    \n    Вспомогательная функция для сохранения усеченных обучающих выборок и скорректированных векторов весов после градиентного уточнения\n\n    Параметры\n    ----------\n    path : str\n        путь к обучающей выборке, подаваемой на вход функции select_top\n    t : list\n        метка выбранного на этапе первоначального приближения целевого класса\n    oth : list\n        список, содержащий метки оставшихся классов, которые не относятся к целевому\n    l : str\n        название столбца с метками классов\n    s : int\n        шаг изменения значений элементов вектора весов, шаг градиентного уточнения;\n    from_initial : int\n        1, если вектор берется из select_top (грубое приближение), \n        0 - если вектор снова корректируется (после grad_boost)\n    weights_main : list\n        вектор весов для корректировки\n\n### grad(path, t, oth, l, s, weights)\n    \n    Функция осуществляет градиентное уточнение полученного после первоначального приближения вектора весов \n\n    Параметры\n    ----------\n    path : str\n        путь к обучающей выборке, подаваемой на вход функции select_top\n    t : list\n        метка выбранного на этапе первоначального приближения целевого класса\n    oth : list\n        список, содержащий метки оставшихся классов, которые не относятся к целевому\n    l : str\n        название столбца с метками классов\n    s : int\n        шаг изменения значений элементов вектора весов, шаг градиентного уточнения\n    weights_main : list\n        вектор весов, значения которого необходимо изменить с целью получения большего количества \n        отсеченных экземпляров обучающей выборки\n\n    Пример использования:\n    wdl.grad('KAHRAMAN_train.csv', ['High'], ['very_low', 'Low', 'Middle'], 'UNS', 1, [455.02247191011236, 552.8764044943821, 273.38202247191015, 518.2921348314607, 2276.179775280899])\n\t\n### grad_binary(path, t, oth, l, s, weights_main)\n    \n    Функция осуществляет градиентное уточнение полученного после первоначального приближения вектора весов \n    для бинарной обучающей выборки\n\n    Параметры\n    ----------\n    path : str\n        путь к бинарной обучающей выборке, подаваемой на вход функции select_top\n    t : list\n        метка выбранного на этапе первоначального приближения целевого класса\n    oth : list\n        список, содержащий метки оставшихся классов, которые не относятся к целевому\n    l : str\n        название столбца с метками классов\n    s : int\n        шаг изменения значений элементов вектора весов, шаг градиентного уточнения\n    weights_main : list\n        вектор весов, значения которого необходимо изменить с целью получения большего количества \n        отсеченных экземпляров обучающей выборки\n\n    Пример использования:\n    wdl.grad_binary('train_6.csv', ['Low'], ['Middle'], 'UNS', 1, [1009.0, 48.0, -929.0, -1056.0, -13.0])\n\n### data_int(path, decimal, name)\n    \n    Функция преобразует набор данных, представленный в вещественнозначном виде в целочисленный вид\n\n    Параметры\n    ----------\n    path : str\n        путь к обучающей выборке в формате csv\n    decimal : str\n        путь к текстовому файлу, содержащему в каждой строке число, обозначающее количество десятичных знаков после \n        запятой в соответствующем столбце выборки\n    name : str\n        аргумент функции, обозначающий желаемое название выходных генерируемых файлов\n\n    Пример использования:\n    wdl.data_int('kahraman.csv', 'dec.txt', 'KAHRAMAN') \n\n### scale_weights(label, data_folder, weights_folder)\n    \n    Функция для масштабирования полученных векторов весов в диапазон от -1 до +1\n\n    Параметры\n    ----------\n    label : str\n        название столбца с метками классов\n    data_folder : str\n        путь к папке, содержащей обучающие выборки каждого нейрона\n    weights_folder : str\n        путь к папке, содержащей веса каждого нейрона\n\n    Пример использования:\n    wdl.scale_weights('UNS', 'data/', 'weights/')\n\n### generate_fa(label, data_folder, weights_folder)\n    \n    Функция, которая на основании проведенного обучения модифицированного полносвязного слоя, генерирует вложенную \n    логическую функцию активации для проверки весовых коэффициентов на тестовых данных\n\n    Параметры\n    ----------\n    label : str\n        название столбца обучающих выборок, в котором содержатся наименования (метки) классов\n    data_folder : str\n        путь к папке result, сгенерированной в результате выполнения функции scale_weights\n    weights_folder : str\n        путь к каталогу scale, который сгенерирован после применения функции scale_weights\n\n    Пример использования:\n    wdl.generate_fa('UNS', 'result', 'scale')\n\n### check_test(train, weights, test, label)\n    \n    Функция осуществляет проверку обучения с помощью правил логического вывода\n\n    Параметры\n    ----------\n    train : str\n        путь к полной целочисленной обучающей выборке\n    weights : str\n        путь к текстовому файлу weights.txt из сгенерированного каталога all_weights после функции scale_weights\n    test : str\n        путь к целочисленной тестовой выборке (в случае проверки обучающей выборки передается путь к полной обучающей выборке, \n        аналогичный параметру train)\n    label : str\n        название столбца с метками классов\n\n    Пример использования:\n    wdl.check_test('train_1.csv', 'weights.txt', 'KAHRAMAN_test.csv', 'UNS')\n\n### getNameColumn(nameFileTrain)\n    \n    Вспомогательная функция для определения названий всех столбцов, кроме столбца с метками классов\n\n    Параметры\n    ----------\n    nameFileTrain : str\n        путь к обучающей выборке \n\n### getCountNeuronSizeVector(nameFileTrain)\n    \n    Вспомогательная функция для определения необходимого количества нейронов в слое\n\n    Параметры\n    ----------\n    nameFileTrain : str\n        путь к обучающей выборке \n\n### initializingDictionaryKeys()\n    \n    Вспомогательная функция для инициализации ключей для правила логического вывода\n\n### initializationDictionaryValues(nameFileTrain)\n    \n    Вспомогательная функция для создания словаря логического вывода\n\n    Параметры\n    ----------\n    nameFileTrain : str\n        путь к обучающей выборке \n\n### count_conv_operations(height, width, color_channels, kernel_size, stride, num_kernels)\n    \n    Функция для подсчета количества вычислительных операций в сверточном слое \n\n    Параметры\n    ----------\n    height : int\n        высота исходного изображения выборки данных\n    width : int\n        ширина исходного изображения\n    color_channels : int\n        количество цветовых каналов изображения \n        (1 – если изображение представлено в черно-белом одноканальном виде, 3 – если изображение является цветным)\n    kernel_size : int\n        размерность сверточного ядра квадратной формы\n    stride : int\n        шаг прохода сверточного ядра по изображению\n    num_kernels : int\n        количество сверточных ядер в слое\n\n    Пример использования:\n    wdl.count_conv_operations(28, 28, 1, 14, 7, 4)\n\n# Шаблоны вызова функций сверточного слоя\n```\nwdl.txt_kernel('путь_к_сгенерированному_ядру.txt')\n```\n```\nwdl.txt_kernel_rgb('путь_к_сгенерированному_ядру_ПЕРВОГО_цветового_канала.txt', 'путь_к_сгенерированному_ядру_ВТОРОГО_цветового_канала.txt', 'путь_к_сгенерированному_ядру_ТРЕТЬЕГО_цветового_канала.txt')\n```\n```\nwdl.add_kernel('путь_к_добавляемому_ядру.txt', переменная_уже_установленных_ядер)\n```\n```\nwdl.add_kernel_rgb('путь_к_добавляемому_ядру_ПЕРВОГО_цветового_канала.txt', 'путь_к_добавляемому_ядру_ВТОРОГО_цветового_канала.txt', 'путь_к_добавляемому_ядру_ТРЕТЬЕГО_цветового_канала.txt', переменная_уже_установленных_ядер)\n```\n```\nwdl.horizontal(размерность_ядра, [список_значений_ядра])\n```\n```\nwdl.vertical(размерность_ядра, [список_значений_ядра])\n```\n```\nwdl.diagonal([список_значений_выше_диагонали], [список_значений_ниже_диагонали], значение_диагонали, размерность_ядра)\n```\n```\nwdl.show_kernel(номер_сверточного_слоя, объект_модели)\n```\n```\nwdl.count_conv_operations(высота_изображения, ширина_изображения, количество_цветовых_каналов, размерность_квадратного_ядра, шаг_ядра, количество_ядер)\n```\n\n# Шаблоны вызова функций полносвязного слоя\n```\nwdl.data_int('путь_к_обучающей_выборке.csv', 'путь_к_файлу_со_значениями_кол-ва_знаков_после_запятой.txt', 'название_выходных_файлов')\n```\n```\nwdl.select_top('путь_к_целочисленной_обучающей_выборке.csv', 'название_столбца_с_метками_классов')\n```\n```\nwdl.select_top_binary('путь_к_целочисленной_обучающей_выборке.csv', 'название_столбца_с_метками_классов')\n```\n```\nwdl.grad('путь_к_целочисленной_обучающей_выборке.csv', [целевой_класс], [список_остальных_классов], 'название_столбца_с_метками_классов', шаг, [вектор_весов])\n```\n```\nwdl.grad_binary('путь_к_целочисленной_обучающей_выборке.csv', [целевой_класс], [список_остальных_классов], 'название_столбца_с_метками_классов', шаг, [вектор_весов])\n```\n```\nwdl.scale_weights('название_столбца_с_метками_классов', 'путь_к_папке_с_обучающими_выборками', 'путь_к_папке_с_весами')\n```\n```\nwdl.generate_fa('название_столбца_с_метками_классов', 'путь_к_папке_result', 'путь_к_папке_scale')\n```\n```\nwdl.check_test('путь_к_полной_обучающей_выборке.csv', 'путь_к_файлу_со_всеми_весами.txt', 'путь_к_тестовой_выборке.csv', 'название_столбца_с_метками_классов')\n```\n",
     'author': 'Brinkinvision',
     'author_email': 'brinkinvision@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'py_modules': modules,
     'python_requires': '>=3.6,<4.0',
```

### Comparing `widelearning-0.8.4/PKG-INFO` & `widelearning-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widelearning
-Version: 0.8.4
+Version: 0.8.5
 Summary: Library for searching the optimal neural network architecture
 License: Apache-2.0
 Author: Brinkinvision
 Author-email: brinkinvision@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -190,14 +190,36 @@
         номер слоя, для которого необходимо вывести значения весовых коэффициентов
     name : object
         объект модели нейронной сети
         название переменной, которой присвоена структура модели
 
     Пример использования:
     wdl.show_kernel(0, model)
+    
+### auto_select(neuron, path, label, target)
+
+    Функция для расчета первоначального приближения с автоматическим выбором целевого класса.
+
+    Параметры
+    ----------
+    neuron : int
+        номер нейрона, для которого производится расчет
+    path : str
+        путь к целочисленной обучающей выборке в формате csv 
+    label : str
+        название столбца с метками классов
+    target : str, list
+        параметр, на основании которого выбирается целевой класс
+        1. 'up' - максимальное количество отсеченных экземпляров сверху
+        2. 'mx_ratio' - максимальная доля отсеченных экземпляров к неотсеченным сверху
+        3. [class] - собственный выбор целевого класса, вместо class необходимо добавить название класса в виде строки или числа 
+
+    Пример использования:
+    wdl.auto_select(1, 'KH_train.csv', 'UNS', ['very_low']) 
+    wdl.auto_select(1, 'KH_train.csv', 'UNS', 'mx_ratio')
 
 ### select_top(path, label)
     
     Функция позволяет получить грубое первоначальное приближение вектора весов
 
     Параметры
     ----------
```

