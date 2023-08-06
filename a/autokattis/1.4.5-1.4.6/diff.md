# Comparing `tmp/autokattis-1.4.5.tar.gz` & `tmp/autokattis-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autokattis-1.4.5.tar", last modified: Sun Jul  9 08:57:56 2023, max compression
+gzip compressed data, was "autokattis-1.4.6.tar", last modified: Sun Aug  6 10:29:16 2023, max compression
```

## Comparing `autokattis-1.4.5.tar` & `autokattis-1.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.573488 autokattis-1.4.5/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    35148 2023-05-04 07:45:56.000000 autokattis-1.4.5/LICENSE
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2639 2023-07-09 08:57:56.572488 autokattis-1.4.5/PKG-INFO
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2285 2023-06-20 09:03:54.000000 autokattis-1.4.5/README.md
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.547473 autokattis-1.4.5/autokattis/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       24 2023-05-11 09:21:05.000000 autokattis-1.4.5/autokattis/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.560763 autokattis-1.4.5/autokattis/api/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    22404 2023-07-09 08:54:22.000000 autokattis-1.4.5/autokattis/api/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.561762 autokattis-1.4.5/autokattis/database/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)   133880 2023-05-08 08:31:18.000000 autokattis-1.4.5/autokattis/database/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.569491 autokattis-1.4.5/autokattis/scraper/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       37 2023-05-11 07:47:42.000000 autokattis-1.4.5/autokattis/scraper/__init__.py
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     3031 2023-05-11 07:45:04.000000 autokattis-1.4.5/autokattis/scraper/country.py
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      977 2023-05-11 07:45:16.000000 autokattis-1.4.5/autokattis/scraper/university.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.571489 autokattis-1.4.5/autokattis/utils/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      518 2023-05-11 07:23:19.000000 autokattis-1.4.5/autokattis/utils/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.558747 autokattis-1.4.5/autokattis.egg-info/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2639 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/PKG-INFO
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      400 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/SOURCES.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)        1 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/dependency_links.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       80 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/requires.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       11 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/top_level.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       38 2023-07-09 08:57:56.574489 autokattis-1.4.5/setup.cfg
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      878 2023-07-09 08:54:41.000000 autokattis-1.4.5/setup.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-08-06 10:29:16.352418 autokattis-1.4.6/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    35148 2023-05-04 07:45:56.000000 autokattis-1.4.6/LICENSE
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2640 2023-08-06 10:29:16.351418 autokattis-1.4.6/PKG-INFO
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2286 2023-08-06 10:23:49.000000 autokattis-1.4.6/README.md
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-08-06 10:29:16.305082 autokattis-1.4.6/autokattis/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       24 2023-05-11 09:21:05.000000 autokattis-1.4.6/autokattis/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-08-06 10:29:16.337271 autokattis-1.4.6/autokattis/api/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    22905 2023-08-06 10:28:03.000000 autokattis-1.4.6/autokattis/api/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-08-06 10:29:16.339437 autokattis-1.4.6/autokattis/database/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)   133880 2023-05-08 08:31:18.000000 autokattis-1.4.6/autokattis/database/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-08-06 10:29:16.348412 autokattis-1.4.6/autokattis/scraper/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       37 2023-05-11 07:47:42.000000 autokattis-1.4.6/autokattis/scraper/__init__.py
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     3031 2023-05-11 07:45:04.000000 autokattis-1.4.6/autokattis/scraper/country.py
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      977 2023-05-11 07:45:16.000000 autokattis-1.4.6/autokattis/scraper/university.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-08-06 10:29:16.350419 autokattis-1.4.6/autokattis/utils/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      518 2023-05-11 07:23:19.000000 autokattis-1.4.6/autokattis/utils/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-08-06 10:29:16.335176 autokattis-1.4.6/autokattis.egg-info/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2640 2023-08-06 10:29:15.000000 autokattis-1.4.6/autokattis.egg-info/PKG-INFO
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      400 2023-08-06 10:29:15.000000 autokattis-1.4.6/autokattis.egg-info/SOURCES.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)        1 2023-08-06 10:29:15.000000 autokattis-1.4.6/autokattis.egg-info/dependency_links.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       80 2023-08-06 10:29:15.000000 autokattis-1.4.6/autokattis.egg-info/requires.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       11 2023-08-06 10:29:15.000000 autokattis-1.4.6/autokattis.egg-info/top_level.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       38 2023-08-06 10:29:16.352418 autokattis-1.4.6/setup.cfg
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      878 2023-08-06 09:39:30.000000 autokattis-1.4.6/setup.py
```

### Comparing `autokattis-1.4.5/LICENSE` & `autokattis-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.5/PKG-INFO` & `autokattis-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokattis
-Version: 1.4.5
+Version: 1.4.6
 Summary: Updated Kattis API wrapper
 Home-page: https://github.com/RussellDash332/autokattis
 Download-URL: https://pypi.org/project/autokattis/
 Author: Russell Saerang
 Author-email: russellsaerang@gmail.com
 License: MIT
 Keywords: Kattis
@@ -38,14 +38,15 @@
 
 ### Problem-specific
 
 ```py
 kt.problems()                               # problems you have solved so far
 kt.problems(show_partial=False)             # exclude partial submissions
 kt.problems(*[True]*4)                      # literally all problems on Kattis
+
 kt.list_unsolved()                          # let's grind!
 
 kt.plot_problems()                          # plot the points distribution
 kt.plot_problems(filepath='plot.png')       # save to a filepath
 kt.plot_problems(show_partial=False)        # plot fully solved submissions
 
 kt.problem('2048')                          # fetch info about a problem
```

### Comparing `autokattis-1.4.5/README.md` & `autokattis-1.4.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 ### Problem-specific
 
 ```py
 kt.problems()                               # problems you have solved so far
 kt.problems(show_partial=False)             # exclude partial submissions
 kt.problems(*[True]*4)                      # literally all problems on Kattis
+
 kt.list_unsolved()                          # let's grind!
 
 kt.plot_problems()                          # plot the points distribution
 kt.plot_problems(filepath='plot.png')       # save to a filepath
 kt.plot_problems(show_partial=False)        # plot fully solved submissions
 
 kt.problem('2048')                          # fetch info about a problem
```

### Comparing `autokattis-1.4.5/autokattis/api/__init__.py` & `autokattis-1.4.6/autokattis/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,16 @@
                             total = int(columns[4].text)
                             acc = int(columns[5].text)
                             difficulty = float(re.findall('[\d\.]+', columns[7].text)[-1])
                                 # [0] instead of [-1] if we want to take min instead of max
                                 # for example:
                                 # - difficulty 9.1-9.6 -> [9.1, 9.6]
                                 # - difficulty 5.0 -> [5.0]
-                            category = re.findall('[A-Za-z]+', columns[7].text)[0]
+                            try: category = re.findall('[A-Za-z]+', columns[7].text)[0]
+                            except: category = 'N/A'
                             data.append({
                                 'name': name,
                                 'fastest': fastest,
                                 'shortest': shortest,
                                 'total': total,
                                 'acc': acc,
                                 'difficulty': difficulty,
@@ -123,16 +124,22 @@
         '''
         Plots the histogram of Kattis problems to a specified filepath.
 
         Default: plots all solved and partially solved problems without saving it to any file.
         '''
 
         df = pd.DataFrame(self.problems(show_solved, show_partial, show_tried, show_untried))
-        hist = sns.histplot(data=df, x='difficulty', hue='category', multiple='stack', binwidth=0.1)
-        hist.set(title=f'Solved Kattis Problems ({df.shape[0]})', xlabel='Difficulty')
+        categories = set(df.category)
+        hue_order = [c for c in ['Easy', 'Medium', 'Hard', 'N/A'][::-1] if c in categories]
+        palette = {'Easy': '#39a137', 'Medium': '#ffbe00', 'Hard': '#ff411a', 'N/A': 'gray'}
+        for c in [*palette]:
+            if c not in categories: del palette[c]
+        hist = sns.histplot(data=df, x='difficulty', hue='category', multiple='stack', binwidth=0.1, hue_order=hue_order, palette=palette)
+        hist.set(title=f'Solved Kattis Problems by {self.user} ({df.shape[0]})', xlabel='Difficulty')
+        plt.legend(title='Category', loc='upper right', labels=hue_order[::-1])
         plt.xticks([*range(math.floor(min(df.difficulty)), math.ceil(max(df.difficulty))+1)])
         if filepath != None:
             plt.savefig(filepath)
             print(f'Saved to {filepath}')
         plt.show()
 
     def list_unsolved(self, show_partial=True):
```

### Comparing `autokattis-1.4.5/autokattis/database/__init__.py` & `autokattis-1.4.6/autokattis/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.5/autokattis/scraper/country.py` & `autokattis-1.4.6/autokattis/scraper/country.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.5/autokattis/scraper/university.py` & `autokattis-1.4.6/autokattis/scraper/university.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.5/autokattis/utils/__init__.py` & `autokattis-1.4.6/autokattis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.5/autokattis.egg-info/PKG-INFO` & `autokattis-1.4.6/autokattis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokattis
-Version: 1.4.5
+Version: 1.4.6
 Summary: Updated Kattis API wrapper
 Home-page: https://github.com/RussellDash332/autokattis
 Download-URL: https://pypi.org/project/autokattis/
 Author: Russell Saerang
 Author-email: russellsaerang@gmail.com
 License: MIT
 Keywords: Kattis
@@ -38,14 +38,15 @@
 
 ### Problem-specific
 
 ```py
 kt.problems()                               # problems you have solved so far
 kt.problems(show_partial=False)             # exclude partial submissions
 kt.problems(*[True]*4)                      # literally all problems on Kattis
+
 kt.list_unsolved()                          # let's grind!
 
 kt.plot_problems()                          # plot the points distribution
 kt.plot_problems(filepath='plot.png')       # save to a filepath
 kt.plot_problems(show_partial=False)        # plot fully solved submissions
 
 kt.problem('2048')                          # fetch info about a problem
```

### Comparing `autokattis-1.4.5/setup.py` & `autokattis-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='autokattis',
-    version='1.4.5',
+    version='1.4.6',
     description='Updated Kattis API wrapper',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Russell Saerang',
     author_email='russellsaerang@gmail.com',
```

