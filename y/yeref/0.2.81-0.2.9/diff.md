# Comparing `tmp/yeref-0.2.81.tar.gz` & `tmp/yeref-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.81.tar", last modified: Sun Aug  6 18:11:31 2023, max compression
+gzip compressed data, was "yeref-0.2.9.tar", last modified: Sun Jun 25 10:28:31 2023, max compression
```

## Comparing `yeref-0.2.81.tar` & `yeref-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 18:11:31.319625 yeref-0.2.81/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-06 18:11:31.319840 yeref-0.2.81/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-06 18:11:31.320675 yeref-0.2.81/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1470 2023-08-06 18:11:19.000000 yeref-0.2.81/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 18:11:31.312970 yeref-0.2.81/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.81/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.81/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   230821 2023-08-06 18:06:56.000000 yeref-0.2.81/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 18:11:31.319119 yeref-0.2.81/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-06 18:11:31.000000 yeref-0.2.81/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-06 18:11:31.000000 yeref-0.2.81/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-06 18:11:31.000000 yeref-0.2.81/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-06 18:11:31.000000 yeref-0.2.81/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:28:31.658668 yeref-0.2.9/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:28:31.658912 yeref-0.2.9/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-25 10:28:31.659829 yeref-0.2.9/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-25 10:28:13.000000 yeref-0.2.9/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:28:31.652441 yeref-0.2.9/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.9/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   558205 2023-06-25 10:27:43.000000 yeref-0.2.9/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   211219 2023-06-23 18:30:42.000000 yeref-0.2.9/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 10:28:31.657998 yeref-0.2.9/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-25 10:28:31.000000 yeref-0.2.9/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-25 10:28:31.000000 yeref-0.2.9/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-25 10:28:31.000000 yeref-0.2.9/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-25 10:28:31.000000 yeref-0.2.9/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.81/setup.py` & `yeref-0.2.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.81',
+      version='0.2.09',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -35,15 +35,15 @@
 # python setup.py sdist
 # python setup.py install
 # python setup.py develop
 #
 # python setup.py bdist_wheel
 # endregion
 
-# python -m build; twine upload --username freey.sitner.ya --password cejwez-nosgin-vaVfe7 dist/*
+# python -m build
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
 # python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.99-py3-none-any.whl
```

### Comparing `yeref-0.2.81/yeref/l_.py` & `yeref-0.2.9/yeref/l_.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,16 +110,16 @@
     'en': "🚫 Delete",
     'es': "🚫 Eliminar",
     'fr': "🚫 Supprimer",
     'zh': "🚫 删除",
     'ar': "🚫 حذف",
 }
 l_try_again = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> или попробуйте позже",
-    'en': "👩🏽‍💻 Invalid or try again later",
+    'ru': "👩🏽‍💻 <b>Попробуйте</b> позже",
+    'en': "👩🏽‍💻 Try again later",
     'es': "🚫 Eliminar",
     'fr': "🚫 Supprimer",
     'zh': "🚫 删除",
     'ar': "🚫 حذف",
 }
 l_please_subscribe = {
     'ru': "👩🏽‍💻 Оформи ежемесячную подписку",
@@ -149,49 +149,25 @@
     'ru': "👩🏽‍💻 <b>Подпишись</b> на @{0}, чтобы снять ограничения",
     'en': "🔔 You need to ⚙️Customize at least one post",
     'es': "🔔 Necesitas ⚙️Personalizar al menos una publicación",
     'fr': "🔔 Vous devez ⚙️Personnaliser au moins une publication",
     'zh': "🔔 你需要⚙️自定义至少一个帖子",
     'ar': "🔔 أنت بحاجة إلى تخصيص منشور واحد على الأقل",
 }
-l_sound = {
-    'ru': "Звук",
-    'en': "Sound",
-    'es': "🚫 Eliminar",
-    'fr': "🚫 Supprimer",
-    'zh': "🚫 删除",
-    'ar': "🚫 حذف",
-}
-l_date = {
-    'ru': "Дата",
-    'en': "Date",
-    'es': "🚫 Eliminar",
-    'fr': "🚫 Supprimer",
-    'zh': "🚫 删除",
-    'ar': "🚫 حذف",
-}
-l_media = {
-    'ru': "Медиа",
-    'en': "Media",
-    'es': "🚫 Eliminar",
-    'fr': "🚫 Supprimer",
-    'zh': "🚫 删除",
-    'ar': "🚫 حذف",
-}
 
 l_choose_direction = {
     'ru': "👇🏽 <b>Выбери</b> направление",
     'en': "👇🏽 <b>Choose</b> a direction",
     'es': "👇🏽 <b>Elige</b> una dirección",
     'fr': "👇🏽 <b>Choisissez</b> une direction",
     'zh': "👇🏽<b>选择</b>方向",
     'ar': "👇🏽 <b>اختر</b> الاتجاه",
 }
 l_about = {
-    'ru': "<b>👩🏽‍💻 Ferey проекты</b>:\n\n▪️проекты: @FereyDemoBot\n▪️конструктор: <a href='https://t.me/FereyBotBot?start=isfree'>@FereyBotBot</a>\n▪️приватные посты: @FereyPostBot\n▪️публичные медиа: @FereyMediaBot\n▪️администрирование: <a href='https://t.me/FereyChannelBot?start=isfree'>@FereyChannelBot</a>\n▪️модерация: <a href='https://t.me/FereyGroupBot?start=isfree'>@FereyGroupBot</a>\n▪️поиск: @FereyFindBot\n▪️таргет: @FereyTargetBot\n▪️инструменты: @FereyToolsBot\n▪️vpn: @FereyVPNBot\n▪️ai: @FereyAIBot\n▪️автоматизация: <a href='https://t.me/FereyUserBot?start=isfree'>@FereyUserBot</a>\n▪️вакансии: @FereyWorkBot\n▪️реклама: @FereyAdsBot",
+    'ru': "<b>👩🏽‍💻 Ferey проекты</b>:\n\n▪️проекты: @FereyDemoBot\n▪️конструктор: @FereyBotBot\n▪️приватные посты: @FereyPostBot\n▪️публичные медиа: @FereyMediaBot\n▪️администрирование: @FereyChannelBot\n▪️модерация: @FereyGroupBot\n▪️поиск: @FereyFindBot\n▪️таргет: @FereyTargetBot\n▪️инструменты: @FereyToolsBot\n▪️vpn: @FereyVPNBot\n▪️ai: @FereyAIBot\n▪️автоматизация: @FereyUserBot\n▪️вакансии: @FereyWorkBot\n▪️реклама: @FereyAdsBot",
     'en': "<b>👩🏽‍💻 Ferey projects</b>:\n\n▪️projects: @FereyDemoBot\n▪️constructor: @FereyBotBot\n▪️private_posts: @FereyPostBot\n▪️public_media: @FereyMediaBot\n▪️administration: @FereyChannelBot\n▪️moderation: @FereyGroupBot\n▪️search: @FereyFindBot\n▪️target: @FereyTargetBot\n▪️tools: @FereyToolsBot\n▪️vpn: @FereyVPNBot\n▪️ai: @FereyAIBot\n▪️automation: @FereyUserBot\n▪️vacancies: @FereyWorkBot\n▪️advert: @FereyAdsBot",
     'es': "<b>👩🏽‍💻 Proyectos de Ferey</b> :\n\n▪️proyectos: @FereyDemoBot\n▪️constructor: @FereyBotBot\n▪️publicaciones_privadas: @FereyPostBot\n▪️medios_públicos: @FereyMediaBot\n▪️administración: @FereyChannelBot\n▪️moderación: @FereyGroupBot\nƒ️búsqueda: @FereyFindBot\nƒ️objetivo: @FereyTargetBot\nƒ️herramientas: @FereyToolsBot\nƒ️vpn: @FereyVPNBot\nƒ️ai: @FereyAIBot\nƒ️automatización: @FereyUserBot\nƒ️vacantes: @FereyWorkBot\n▪️anuncio: @FereyAdsBot",
     'fr': "<b>👩🏽‍💻 Projets Ferey</b> :\n\n▪️projets : @FereyDemoBot\n▪️constructeur : @FereyBotBot\n▪️public_medias : @FereyPostBot\n▪️public_media : @FereyMediaBot\n▪️administration : @FereyChannelBot\n▪️modération : @FereyGroupBot\n▪️recherche : @FereyFindBot\n▪️cible : @FereyTargetBot\n▪️outils : @FereyToolsBot\n▪️vpn : @FereyVPNBot\n▪️ai : @FereyAIBot\n▪️automatisation : @FereyUserBot\n▪️postes vacants : @FereyWorkBot\n▪️annonce : @FereyAdsBot",
     'zh': "<b>👩🏽‍💻 Ferey 项目</b>：\n\n▪️projects： @FereyDemoBot\n▪️constructor： @FereyBotBot\n▪️private_posts： @FereyPostBot\n▪️public_media： @FereyMediaBot\n▪️administration： @FereyChannelBot\n▪️moderation： @FereyGroupBot\n▪️搜索： @FereyFindBot\n▪️目标： @FereyTargetBot\n▪️工具： @FereyToolsBot\n▪️vpn： @FereyVPNBot\n▪️ai： @FereyAIBot\n▪️自动化： @FereyUserBot\n▪️空缺： @FereyWorkBot\n▪️广告： @FereyAdsBot",
     'ar': "<b>👩🏽‍💻 المشاريع السريعة</b> :\n\n▪️ المشاريع: @FereyDemoBot\n▪️ المُنشئ: @FereyBotBot\n▪️private_posts: @FereyPostBot\n▪️public_media: @FereyMediaBot\n▪️administration: @FereyChannelBot : @ @FereyGroupBot\n▪️search: @FereyFindBot\n▪️ الهدف: @FereyTargetBot\n▪️ الأدوات: @FereyToolsBot\n▪️vpn: @FereyVPNBot\n▪️ai: @FereyAIBot\n▪️automation: @FereyUserBot @FereyWorkBot\nإعلان: @FereyAdsBot",
 }
 l_subscribe_btn = {
@@ -275,48 +251,24 @@
     'zh': "💔 喜欢",
     'ar': "💔 مثل",
 }
 # endregion
 
 
 # region post
-l_post_media = {
-    'ru': "✏️ 1. <b>Прикрепи медиа</b> контент для поста: фото/гиф/видео/аудио/документ/стикер или запиши голосовое/видео-заметку в кружке\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 1. <b>Attach media</b> content: photo/gif/video/audio/document/sticker or write a voice/video note in a circle\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
-    'es': "✏️ 1. <b>Adjunte contenido multimedia</b> : foto/gif/video/audio/documento/pegatina o escriba una nota de voz/video en un círculo\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
-    'fr': "✏️ 1. <b>Joignez du contenu multimédia</b> : photo/gif/vidéo/audio/document/autocollant ou écrivez une note vocale/vidéo dans un cercle\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
-    'zh': "✏️ 1.<b>附上媒体</b>内容：照片/gif/视频/音频/文档/贴纸或在圈内写语音/视频备注\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
-    'ar': "✏️ 1. <b>أرفق محتوى وسائط</b> : صورة / gif / فيديو / صوت / مستند / ملصق أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
-}
-l_post_media_wait = {
-    'ru': "👩🏽‍💻 <b>Обработка</b> {0}..\n#длительность {1}мин",
-    'en': "👩🏽‍💻 <b>Processing</b> {0}..\n#duration {1}min",
-    'es': "👩🏽‍💻 <b>Procesando</b> {0}..\n#duración {1}min",
-    'fr': "👩🏽‍💻 <b>Traitement</b> {0}..\n#durée {1}min",
-    'zh': "👩🏽‍💻<b>处理</b>{0}..\n#duration {1}min",
-    'ar': "👩🏽‍💻 <b>المعالجة</b> {0} ..\n# مدة {1} دقيقة",
-}
-l_post_media_toobig = {
-    'ru': "👩🏽‍💻 Файл больше 20 Мб, загрузи меньший обьем",
-    'en': "👩🏽‍💻 The file is larger than 20 MB, please upload a smaller size",
-    'es': "👩🏽‍💻 El archivo tiene más de 20 MB, cargue un tamaño más pequeño",
-    'fr': "👩🏽‍💻 Le fichier fait plus de 20 Mo, veuillez télécharger une taille plus petite",
-    'zh': "👩🏽‍💻文件大于20MB，请上传较小的文件",
-    'ar': "👩🏽‍💻 الملف أكبر من 20 ميغا بايت ، يرجى تحميل حجم أصغر",
-}
 l_post_text = {
-    'ru': "✏️ 2. <b>Введи текст</b> (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 2. <b>Enter the text</b> for the new post (don&#x27;t forget to use <i>formatting</i> )\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
-    'es': "✏️ 2. <b>Ingresa el texto</b> de la nueva publicación (no olvides usar <i>el formato</i> )\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
-    'fr': "✏️ 2. <b>Saisissez le texte</b> du nouveau message (n&#x27;oubliez pas d&#x27;utiliser <i>le formatage</i> )\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
-    'zh': "✏️ 2.<b>输入新帖子的文本</b>（不要忘记使用<i>格式</i>）\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
-    'ar': "✏️ 2. <b>أدخل نص</b> المنشور الجديد (لا تنس استخدام <i>التنسيق</i> )\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
+    'ru': "✏️ 1. <b>Введи текст</b> для нового поста (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'en': "✏️ 1. <b>Enter the text</b> for the new post (don&#x27;t forget to use <i>formatting</i> )\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
+    'es': "✏️ 1. <b>Ingresa el texto</b> de la nueva publicación (no olvides usar <i>el formato</i> )\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
+    'fr': "✏️ 1. <b>Saisissez le texte</b> du nouveau message (n&#x27;oubliez pas d&#x27;utiliser <i>le formatage</i> )\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
+    'zh': "✏️ 1.<b>输入新帖子的文本</b>（不要忘记使用<i>格式</i>）\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
+    'ar': "✏️ 1. <b>أدخل نص</b> المنشور الجديد (لا تنس استخدام <i>التنسيق</i> )\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_text_limit = {
-    'ru': "❗️ <b>Количество символов</b> текста (<i>включая форматирование</i>): <u>{0}</u> больше 1024",
+    'ru': "❗️ <b>Количество символов</b> текста (<i>включая форматирование</i>): <u>{0}</u> больше допустимых 1024",
     'en': "❗️ <b>Number of characters</b> of text ( <i>including formatting</i> ): <u>{0}</u> more than allowed 1024",
     'es': "❗️ <b>Número de caracteres</b> de texto ( <i>incluido el formato</i> ): <u>{0}</u> más de los permitidos 1024",
     'fr': "❗️ <b>Nombre de caractères</b> de texte ( <i>y compris le formatage</i> ) : <u>{0}</u> plus que autorisé 1024",
     'zh': "❗️ 文本<b>字符数</b>（<i>包括格式</i>）： <u>{0}</u>超过允许的 1024",
     'ar': "❗️ <b>عدد أحرف</b> النص ( <i>بما في ذلك التنسيق</i> ): <u>{0}</u> أكثر من العدد المسموح به وهو 1024",
 }
 l_post_text_empty = {
@@ -324,20 +276,44 @@
     'en': "❗️ Post is empty, try again\n\n{0}",
     'es': "❗️ La publicación está vacía, inténtalo de nuevo\n\n{0}",
     'fr': "❗️ La publication est vide, réessayez\n\n{0}",
     'zh': "❗️ 帖子为空，请重试\n\n{0}",
     'ar': "❗️ النشر فارغ ، حاول مرة أخرى\n\n{0}",
 }
 l_post_edit = {
-    'ru': "✏️ 2. <b>Введи измененный текст</b> для текущего поста\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 2. <b>Enter the modified text</b> for the current post\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
-    'es': "✏️ 2. <b>Ingresa el texto modificado</b> para la publicación actual\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
-    'fr': "✏️ 2. <b>Entrez le texte modifié</b> pour le message actuel\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
-    'zh': "✏️ 2.<b>输入当前帖子的修改文本</b>\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
-    'ar': "✏️ 2. <b>أدخل النص المعدل</b> للنشر الحالي\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
+    'ru': "✏️ 1. <b>Введи измененный текст</b> для текущего поста\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'en': "✏️ 1. <b>Enter the modified text</b> for the current post\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
+    'es': "✏️ 1. <b>Ingresa el texto modificado</b> para la publicación actual\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
+    'fr': "✏️ 1. <b>Entrez le texte modifié</b> pour le message actuel\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
+    'zh': "✏️ 1.<b>输入当前帖子的修改文本</b>\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
+    'ar': "✏️ 1. <b>أدخل النص المعدل</b> للنشر الحالي\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
+}
+l_post_media = {
+    'ru': "✏️ 2. <b>Прикрепи медиа</b> контент: фото/гиф/видео/аудио/документ/стикер или запиши голосовое/видео-заметку в кружке\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'en': "✏️ 2. <b>Attach media</b> content: photo/gif/video/audio/document/sticker or write a voice/video note in a circle\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
+    'es': "✏️ 2. <b>Adjunte contenido multimedia</b> : foto/gif/video/audio/documento/pegatina o escriba una nota de voz/video en un círculo\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
+    'fr': "✏️ 2. <b>Joignez du contenu multimédia</b> : photo/gif/vidéo/audio/document/autocollant ou écrivez une note vocale/vidéo dans un cercle\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
+    'zh': "✏️ 2.<b>附上媒体</b>内容：照片/gif/视频/音频/文档/贴纸或在圈内写语音/视频备注\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
+    'ar': "✏️ 2. <b>أرفق محتوى وسائط</b> : صورة / gif / فيديو / صوت / مستند / ملصق أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
+}
+l_post_media_wait = {
+    'ru': "👩🏽‍💻 <b>Обработка</b> {0}..\n#длительность {1}мин",
+    'en': "👩🏽‍💻 <b>Processing</b> {0}..\n#duration {1}min",
+    'es': "👩🏽‍💻 <b>Procesando</b> {0}..\n#duración {1}min",
+    'fr': "👩🏽‍💻 <b>Traitement</b> {0}..\n#durée {1}min",
+    'zh': "👩🏽‍💻<b>处理</b>{0}..\n#duration {1}min",
+    'ar': "👩🏽‍💻 <b>المعالجة</b> {0} ..\n# مدة {1} دقيقة",
+}
+l_post_media_toobig = {
+    'ru': "👩🏽‍💻 Файл больше 20 Мб, загрузи меньший обьем",
+    'en': "👩🏽‍💻 The file is larger than 20 MB, please upload a smaller size",
+    'es': "👩🏽‍💻 El archivo tiene más de 20 MB, cargue un tamaño más pequeño",
+    'fr': "👩🏽‍💻 Le fichier fait plus de 20 Mo, veuillez télécharger une taille plus petite",
+    'zh': "👩🏽‍💻文件大于20MB，请上传较小的文件",
+    'ar': "👩🏽‍💻 الملف أكبر من 20 ميغا بايت ، يرجى تحميل حجم أصغر",
 }
 l_post_tgph = {
     'ru': "✏️ *2. Использовать загруженный <b>media</b>-контент в виде <u>предпросмотра</u> внизу поста (работает только с <i>jpg|png|gif|mp4</i>-файлами до 5Mb)?\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ *2. Use uploaded <b>media</b> content as <u>a preview</u> at the bottom of the post (only works with <i>jpg|png|gif|mp4</i> files up to 5Mb)?\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ *2. ¿Usar el contenido <b>multimedia</b> cargado como <u>una vista previa</u> en la parte inferior de la publicación (solo funciona con archivos <i>jpg|png|gif|mp4</i> de hasta 5 Mb)?\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ *2. Utiliser le contenu <b>multimédia</b> téléchargé comme <u>aperçu</u> au bas de la publication (fonctionne uniquement avec les fichiers <i>jpg|png|gif|mp4</i> jusqu&#x27;à 5 Mo) ?\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ *2。使用上传的<b>媒体</b>内容作为帖子底部的<u>预览</u>（仅适用于最大 5Mb 的<i>jpg|png|gif|mp4</i>文件）？\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
@@ -380,15 +356,15 @@
     'en': "✏️ 3. Pin ( <b>pin</b> ) the message on top of the screen: да | нет ?\n\n( <i>or press &quot;➡️️/Next&quot; to <u>not pin</u> the message</i> )",
     'es': "✏️ 3. Pin ( <b>pin</b> ) el mensaje en la parte superior de la pantalla: да | нет ?\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para <u>no fijar</u> el mensaje</i> )",
     'fr': "✏️ 3. Epingler ( <b>épingler</b> ) le message en haut de l&#x27;écran : да | нет ?\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour <u>ne pas épingler</u> le message</i> )",
     'zh': "✏️ 3. 将消息置顶（<b>置顶</b>）： да | нет ？\n\n（<i>或按“➡️️/下一步”<u>不固定</u>消息</i>）",
     'ar': "✏️ 3. قم بتثبيت ( <b>تثبيت</b> ) الرسالة أعلى الشاشة: да | нет ؟\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لعدم <u>تثبيت</u> الرسالة</i> )",
 }
 l_post_date = {
-    'ru': "✏️ <b>Выбери дату</b> на календаре\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 4. <b>Выбери дату</b> на календаре\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 4. <b>Select a date</b> on the calendar\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 4. <b>Selecciona una fecha</b> en el calendario\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 4. <b>Sélectionnez une date</b> sur le calendrier\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 4. 在日历上<b>选择一个日期</b>\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
     'ar': "✏️ 4. <b>حدد تاريخًا</b> في التقويم\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_window = {
@@ -404,15 +380,15 @@
     'en': "❗️ <b>Number of characters</b> of text ( <i>including formatting</i> ): <u>{0}</u> more than allowed 1024",
     'es': "❗️ <b>Número de caracteres</b> de texto ( <i>incluido el formato</i> ): <u>{0}</u> más de los permitidos 1024",
     'fr': "❗️ <b>Nombre de caractères</b> de texte ( <i>y compris le formatage</i> ) : <u>{0}</u> plus que autorisé 1024",
     'zh': "❗️ 文本<b>字符数</b>（<i>包括格式</i>）： <u>{0}</u>超过允许的 1024",
     'ar': "❗️ <b>عدد أحرف</b> النص ( <i>بما في ذلك التنسيق</i> ): <u>{0}</u> أكثر من العدد المسموح به وهو 1024",
 }
 l_post_finish = {
-    'ru': "✅ <b>Пост готов</b>\n\n<i>Нажми «➡️️/Next», чтобы подтвердить, а затем на кнопку: [🔗 Публикация]</i>",
+    'ru': "✅ <b>Пост готов</b>\n\n<i>Нажми «➡️️/Next», чтобы подтвердить, а затем на кнопку 🔗 Публикация</i>",
     'en': "✅ <b>Post is ready</b>\n\n<i>Press &quot;➡️️/Next&quot; to confirm, and then press the button 🔗 Publish</i>",
     'es': "✅ <b>La publicación está lista</b>\n\n<i>Presiona &quot;➡️️/Siguiente&quot; para confirmar y luego presiona el botón 🔗 Publicar</i>",
     'fr': "✅ <b>La publication est prête</b>\n\n<i>Appuyez sur &quot;➡️️/Suivant&quot; pour confirmer, puis appuyez sur le bouton 🔗 Publier</i>",
     'zh': "✅<b>发布准备就绪</b>\n\n<i>按“➡️️/Next”确认，然后按按钮🔗发布</i>",
     'ar': "✅ <b>النشر جاهز</b>\n\n<i>اضغط على &quot;➡️️ / التالي&quot; للتأكيد ، ثم اضغط على الزر 🔗 نشر</i>",
 }
 l_switch_pm_text = {
@@ -469,15 +445,15 @@
     'en': "👩🏽‍💻 Post published",
     'es': "👩🏽‍💻 Publicación publicada",
     'fr': "👩🏽‍💻 Article publié",
     'zh': "👩🏽‍💻 帖子已发布",
     'ar': "👩🏽‍💻 تم نشر المنشور",
 }
 l_post_btn_answer = {
-    'ru': "✅ <b>Пользователь</b> <b>{0}</b> (username={1}, id={2}) <i>нажал</i> на [<b>{3}</b>] в посте #<u>{4}</u>",
+    'ru': "✅ Пользователь <b>{0}</b> (username={1}, id={2}) <i>нажал</i> на [<b>{3}</b>] в посте #<u>{4}</u>",
     'en': "✅ User <b>{0}</b> (username={1}, id= {2} ) <i>clicked</i> on [<b>{3}</b>] in post # <u>{4}</u>",
     'es': "✅ El usuario <b>{0}</b> (username={1}, id= {2} ) <i>hizo clic</i> en [<b>{3}</b>] en la publicación n.º <u>{4}</u>",
     'fr': "✅ L'utilisateur <b>{0}</b> (username={1}, id= {2} ) <i>a cliqué</i> sur [<b>{3}</b>] dans le post # <u>{4}</u>",
     'zh': "✅ 用户<b>{0}</b> （用户名 = {1}，id = {2} ）在帖子 # <u>{4}</u>中<i>点击了</i>[<b>{3}</b>]",
     'ar': "✅ المستخدم <b>{0}</b> (اسم المستخدم = {1} ، المعرف = {2} ) <i>نقر</i> على [<b>{3}</b>] في المشاركة رقم <u>{4}</u>",
 }
 l_post_datetime = {
@@ -517,37 +493,37 @@
     'ru': "кнопки",
     'en': "buttons",
     'es': "botones",
     'fr': "boutons",
     'zh': "纽扣",
     'ar': "أزرار",
 }
-l_default = {
-    'ru': "по умолчанию",
+l_pin = {
+    'ru': "закреп",
     'en': "fixed",
     'es': "fijado",
     'fr': "fixé",
     'zh': "固定的",
     'ar': "مُثَبَّت",
 }
 l_silence = {
     'ru': "тихо",
     'en': "quiet",
     'es': "tranquilo",
     'fr': "calme",
     'zh': "安静的",
     'ar': "هادئ",
 }
-l_pin = {
-    'ru': "закреп",
-    'en': "fixed",
-    'es': "fijado",
-    'fr': "fixé",
-    'zh': "固定的",
-    'ar': "مُثَبَّت",
+l_gallery = {
+    'ru': "галерея",
+    'en': "gallery",
+    'es': "galería",
+    'fr': "galerie",
+    'zh': "画廊",
+    'ar': "صالة عرض",
 }
 l_preview = {
     'ru': "превью",
     'en': "preview",
     'es': "avance",
     'fr': "aperçu",
     'zh': "预览",
@@ -557,54 +533,14 @@
     'ru': "спойлер",
     'en': "spoiler",
     'es': "revelación",
     'fr': "divulgacher",
     'zh': "剧透",
     'ar': "المفسد",
 }
-l_album = {
-    'ru': "альбом",
-    'en': "album",
-    'es': "galería",
-    'fr': "galerie",
-    'zh': "画廊",
-    'ar': "صالة عرض",
-}
-l_gallery = {
-    'ru': "галерея",
-    'en': "gallery",
-    'es': "galería",
-    'fr': "galerie",
-    'zh': "画廊",
-    'ar': "صالة عرض",
-}
-l_format = {
-    'ru': "формат",
-    'en': "format",
-    'es': "galería",
-    'fr': "galerie",
-    'zh': "画廊",
-    'ar': "صالة عرض",
-}
-l_blog = {
-    'ru': "блог",
-    'en': "blog",
-    'es': "revelación",
-    'fr': "divulgacher",
-    'zh': "剧透",
-    'ar': "المفسد",
-}
-l_web = {
-    'ru': "веб",
-    'en': "web",
-    'es': "revelación",
-    'fr': "divulgacher",
-    'zh': "剧透",
-    'ar': "المفسد",
-}
 l_notice = {
     'ru': "нотис",
     'en': "notice",
     'es': "revelación",
     'fr': "divulgacher",
     'zh': "剧透",
     'ar': "المفسد",
@@ -615,39 +551,39 @@
     'es': "revelación",
     'fr': "divulgacher",
     'zh': "剧透",
     'ar': "المفسد",
 }
 
 l_buttons_text = {
-    'ru': "👩🏽‍💻 Режим [✅ кнопки] доступен, если создана хотя бы 1 кнопка при создании поста",
+    'ru': "👩🏽‍💻 Режим [кнопки] доступен, если создана хотя бы 1 кнопка при создании поста",
     'en': "👩🏽‍💻 [Buttons] mode is available if at least 1 button is created when creating a post",
     'es': "👩🏽‍💻 El modo [Botones] está disponible si se crea al menos 1 botón al crear una publicación",
     'fr': "👩🏽‍💻 Le mode [Boutons] est disponible si au moins 1 bouton est créé lors de la création d'une publication",
     'zh': "👩🏽‍💻 如果在创建帖子时至少创建了 1 个按钮，则可以使用 [按钮] 模式",
     'ar': "يكون وضع [الأزرار] متاحًا إذا تم إنشاء زر واحد على الأقل عند إنشاء منشور",
 }
 l_preview_text = {
-    'ru': "👩🏽‍💻 Режим [✅ превью] используется с одиночными jpg|png|gif|mp4-файлами до 5Mb",
+    'ru': "👩🏽‍💻 Режим [превью] используется с одиночными jpg|png|gif|mp4-файлами до 5Mb",
     'en': "👩🏽‍💻 The [preview] mode is used with single jpg|png|gif|mp4 files up to 5Mb",
     'es': "👩🏽‍💻 El modo [vista previa] se usa con archivos individuales jpg|png|gif|mp4 de hasta 5Mb",
     'fr': "👩🏽‍💻 Le mode [aperçu] est utilisé avec des fichiers jpg|png|gif|mp4 uniques jusqu'à 5 Mo",
     'zh': "👩🏽‍💻 [预览] 模式用于最大 5Mb 的单个 jpg|png|gif|mp4 文件",
     'ar': "👩🏽‍💻 يتم استخدام وضع [المعاينة] مع ملفات jpg واحدة | png | gif | mp4 حتى 5 ميغا بايت",
 }
 l_gallery_text = {
-    'ru': "👩🏽‍💻 Режим [✅ галерея] доступен для 2 и более медиа файлов",
+    'ru': "👩🏽‍💻 Режим [галерея] доступен для 2 и более медиа файлов",
     'en': "👩🏽‍💻 [Gallery] mode is available for 2 or more media files",
     'es': "👩🏽‍💻 El modo [Galería] está disponible para 2 o más archivos multimedia",
     'fr': "👩🏽‍💻 Le mode [Galerie] est disponible pour 2 fichiers multimédias ou plus",
     'zh': "👩🏽‍💻 [图库] 模式可用于 2 个或更多媒体文件",
     'ar': "وضع [المعرض] متاح لملفات وسائط أو أكثر",
 }
 l_spoiler_text = {
-    'ru': "👩🏽‍💻 Режим [✅ спойлер] доступен для photo/gif/video",
+    'ru': "👩🏽‍💻 Режим [спойлер] доступен для photo/gif/video",
     'en': "👩🏽‍💻 [spoiler] mode available for photo/gif/video",
     'es': "👩🏽‍💻 Modo [spoiler] disponible para foto/gif/video",
     'fr': "👩🏽‍💻 Mode [spoiler] disponible pour photo/gif/vidéo",
     'zh': "👩🏽‍💻 [剧透] 模式可用于照片/gif/视频",
     'ar': "👩🏽‍💻 وضع [المفسد] متاح للصور / gif / الفيديو",
 }
 l_window_text = {
@@ -671,15 +607,15 @@
     'en': "📍 Location <b>time zone</b> set\n\n🕐 <b>Current</b> time: <u>{0}</u> ({1}{2} GMT)",
     'es': "📍 Configuración <b>de la zona horaria</b> de la ubicación\n\n🕐 Hora <b>actual</b> : <u>{0}</u> ({1}{2} GMT)",
     'fr': "📍 <b>Fuseau horaire</b> de l&#x27;emplacement défini\n\n🕐 Heure <b>actuelle</b> : <u>{0}</u> ({1}{2} GMT)",
     'zh': "📍 位置<b>时区</b>设置\n\n🕐<b>当前</b>时间： <u>{0}</u> （{1}{2} GMT）",
     'ar': "📍 تعيين <b>المنطقة الزمنية</b> للموقع\n\n🕐 الوقت <b>الحالي</b> : <u>{0}</u> ({1} {2} GMT)",
 }
 l_post_time_future = {
-    'ru': "🕒 <b>Укажи</b> дату и время в будущем",
+    'ru': "🕒 <b>Укажи</b> время в будущем",
     'en': "🕒 Set time in the future",
     'es': "🕒 Establecer tiempo en el futuro",
     'fr': "🕒 Réglez l'heure dans le futur",
     'zh': "🕒 设定未来的时间",
     'ar': "🕒 حدد الوقت في المستقبل",
 }
 l_me = {
@@ -970,95 +906,95 @@
     'en': "bot constructor",
     'es': "constructor de bots",
     'fr': "constructeur de bot",
     'zh': "机器人构造器",
     'ar': "منشئ الروبوت",
 }
 l_inline_post = {
-    'ru': "приватные посты",
+    'ru': "конструктор офферов",
     'en': "offer constructor",
     'es': "constructor de ofertas",
     'fr': "offre constructeur",
     'zh': "提供构造函数",
     'ar': "عرض منشئ",
 }
 l_inline_media = {
-    'ru': "публичные медиа",
+    'ru': "конструктор медиа-заметок",
     'en': "media note builder",
     'es': "generador de notas de medios",
     'fr': "constructeur de note média",
     'zh': "媒体笔记生成器",
     'ar': "منشئ الملاحظات الإعلامية",
 }
 l_inline_channel = {
-    'ru': "администрирование каналов",
+    'ru': "администратор каналов",
     'en': "channel administrator",
     'es': "administrador del canal",
     'fr': "administrateur de la chaîne",
     'zh': "频道管理员",
     'ar': "مدير القناة",
 }
 l_inline_group = {
-    'ru': "модерация групп",
+    'ru': "администратор групп",
     'en': "group administrator",
     'es': "administrador de grupo",
     'fr': "administrateur de groupe",
     'zh': "群管理员",
     'ar': "مسؤول المجموعة",
 }
 l_inline_find = {
-    'ru': "премиум поиск",
+    'ru': "бот для поиска",
     'en': "search bot",
     'es': "robot de búsqueda",
     'fr': "robot de recherche",
     'zh': "搜索机器人",
     'ar': "بحث بوت",
 }
 l_inline_ai = {
-    'ru': "нейросеть",
+    'ru': "бот с нейросетью",
     'en': "bot with neural network",
     'es': "bot con red neuronal",
     'fr': "bot avec réseau de neurones",
     'zh': "具有神经网络的机器人",
     'ar': "بوت مع الشبكة العصبية",
 }
 l_inline_ads = {
-    'ru': "реклама",
+    'ru': "рекламный бот",
     'en': "advertising bot",
     'es': "robot publicitario",
     'fr': "robot publicitaire",
     'zh': "广告机器人",
     'ar': "روبوت إعلاني",
 }
 l_inline_vpn = {
-    'ru': "VPN",
+    'ru': "vpn-бот",
     'en': "vpn-bot",
     'es': "vpn-bot",
     'fr': "vpn-bot",
     'zh': "vpn机器人",
     'ar': "vpn- بوت",
 }
 l_inline_target = {
-    'ru': "таргет",
+    'ru': "таргет-бот",
     'en': "target bot",
     'es': "robot objetivo",
     'fr': "robot cible",
     'zh': "目标机器人",
     'ar': "الهدف الروبوت",
 }
 l_inline_user = {
-    'ru': "автоматизация пользователей",
+    'ru': "администратор пользователя",
     'en': "user administrator",
     'es': "administrador de usuarios",
     'fr': "administrateur d'utilisateurs",
     'zh': "用户管理员",
     'ar': "مسؤول المستخدم",
 }
 l_inline_tools = {
-    'ru': "инструменты",
+    'ru': "Telegram-инструменты",
     'en': "Telegram tools",
     'es': "Herramientas de telegramas",
     'fr': "Outils de télégramme",
     'zh': "电报工具",
     'ar': "أدوات Telegram",
 }
 l_inline_work = {
@@ -1086,31 +1022,23 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_bot_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> автоматизации <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️интеграции и <b>платежи</b>\n▪️<b>нейросети</b>: графика и текст бота\n\n❗️Регулярно-обновляемый /content",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> автоматизации <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️нейросети: графика и текст бота\n▪️интеграции и платежи\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to the <b>Telegram</b> bot автоматизации <i>landing bot</i> :\n\n▪️auto-posting and <b>auto-translation</b>\n▪️ <b>auto-replies</b> and notifications\n▪️integrations and payments\n▪️users and administrators\n\n❗️You can also order the development of a chatbot in our ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> автоматизации de bots <b>de Telegram</b> :\n\n▪️auto-publicación y <b>auto-traducción</b>\n▪️auto <b>-respuestas</b> y notificaciones\n▪️integraciones y pagos\n▪️usuarios y administradores\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro ferey studio",
     'fr': "🌱 {0}, bienvenue dans le <i>bot d&#x27;atterrissage</i> автоматизации du bot <b>Telegram</b> :\n\n▪️publication et <b>traduction automatiques</b>\n▪️ <b>réponses et notifications automatiques</b>\n▪️intégrations et paiements\n▪️utilisateurs et administrateurs\n\n❗️Vous pouvez également commander le développement d'un chatbot dans notre studio ferey",
     'zh': "🌱 {0}，欢迎使用<b>Telegram</b>机器人автоматизации<i>登陆机器人</i>：\n\n▪️自动发布和<b>自动翻译</b>\n▪️<b>自动回复</b>和通知\n▪️集成和支付\n▪️用户和管理员\n\n❗️您也可以在我们的ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> автоматизации لروبوت <b>Telegram</b> :\n\n▪️ النشر التلقائي <b>والترجمة التلقائية</b>\n▪️ <b>الردود التلقائية</b> والإشعارات\n▪️ عمليات الدمج والمدفوعات\nالمستخدمون والمسؤولون\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو ferey الخاص بنا",
 }
 l_subscribe_bot = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️авто-перевод\n(<i>в том числе, текста кнопок</i>)\n▪️авто-ответ\n(<i>chatgpt видит блоки бота</i>)\n▪️создание бота через текстовый запрос\n(<i>с помощью нейросети</i>)\n▪️клонирование ботов конкурентов\n▪️создание > 1 активного бота\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
-}
-l_subscribe_isfree = {
-    'ru': "👩🏽‍💻 <b>Расширенный</b> период использования @{0}-бота завершился\n\n👩🏽‍💻 <b>Оформи</b> подписку, чтобы продолжать использовать созданные шаблоны <a href='{1}'>@donate</a>",
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️авто-перевод\n(<i>в том числе, текста кнопок</i>)\n▪️авто-ответ\n(<i>chatgpt видит блоки бота</i>)\n▪️приоритетная поддержка\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
@@ -1127,15 +1055,15 @@
     'en': "➕ Subscribe for >1 bot or unsubscribe active bot to add a new one",
     'es': "➕ Suscríbete a >1 bot o cancela la suscripción de un bot activo para agregar uno nuevo",
     'fr': "➕ Abonnez-vous pour > 1 bot ou désabonnez-vous du bot actif pour en ajouter un nouveau",
     'zh': "➕ 订阅 >1 个机器人或取消订阅活动机器人以添加新机器人",
     'ar': "➕ اشترك في> 1 bot أو إلغاء الاشتراك في bot النشط لإضافة واحد جديد",
 }
 l_test_bot_desc = {
-    'ru': "🫥 Описание @{0}-бота:\n\n▪️телеграф-блог\n▪️авто-перевод\n(в том числе, текста кнопок)\n▪️оповещения и utm-рефералы\n▪️нейросети: графика и текст бота\n▪️интеграции и платежи",
+    'ru': "🫥 Описание @{0}-бота:\n\n▪️телеграф блог\n▪️авто-перевод\n▪️оповещения и utm-рефералы\n▪️интеграции",
     'en': "🫥 @{0}-bot description:\n\n▪️telegraph blog\n▪️auto-translation\n▪️alerts and utm referrals\n▪️integrations",
     'es': "🫥 @{0}-bot description:\n\n▪️telegraph blog\n▪️traducción automática\n▪️alertas y referencias utm\n▪️integraciones",
     'fr': "🫥 @{0}-bot description :\n\n▪️blog télégraphique\n▪️traduction automatique\n▪️alertes et références utm\n▪️intégrations",
     'zh': "🫥 @{0}-bot 描述：\n\n▪️电报博客\n▪️自动翻译\n▪️提醒和 utm 推荐\n▪️集成",
     'ar': "🫥 @ {0} وصف البرنامج الآلي:\n\n▪️ مدونة telegraph\n▪️ ترجمة تلقائية\n▪️ تنبيهات وإحالات UTM\n▪️ تكامل",
 }
 l_clone_bot_button = {
@@ -1143,15 +1071,15 @@
     'en': "©️ Clone the bot",
     'es': "©️ Clonar el bot",
     'fr': "©️ Cloner le bot",
     'zh': "©️ 克隆机器人",
     'ar': "© ️ استنساخ الروبوت",
 }
 l_clone_bot_call = {
-    'ru': "©️ Оформи подписку, чтобы склонировать бота конкурента",
+    'ru': "©️ Оформи подписку для >1 бота или открепи активного бота, чтобы склонировать бота конкурента",
     'en': "©️ Subscribe >1 bot or unpin an active bot to clone a competitor's bot",
     'es': "©️ Suscríbete >1 bot o desancla un bot activo para clonar el bot de un competidor",
     'fr': "©️ Abonnez-vous >1 bot ou désépinglez un bot actif pour cloner le bot d'un concurrent",
     'zh': "©️ 订阅 >1 个机器人或取消固定一个活跃的机器人以克隆竞争对手的机器人",
     'ar': "© ️ اشترك> 1 بوت أو قم بإلغاء تثبيت روبوت نشط لاستنساخ روبوت منافس",
 }
 l_clone_bot_text = {
@@ -1206,26 +1134,18 @@
     'ru': "👩🏽‍💻 *Промокод*: `{txt}` активирован",
     'en': "👩🏽‍💻 *Promo code*: `{txt}` activated",
     'es': "👩🏽‍💻 *Código promocional*: `{txt}` activado",
     'fr': "👩🏽‍💻 *Code promotionnel* : `{txt}` activé",
     'zh': "👩🏽‍💻 *促销代码*：`{txt}` 激活",
     'ar': "👩🏽‍💻 * الرمز الترويجي *: '{txt}` مفعل",
 }
-l_create_view_web = {
-    'ru': "👩🏽‍💻 <b>Спрятанная</b> ссылка на веб-страницу: <a href='https://t.me/{0}/web?startapp={1}_{2}'>@{3}/web</a>\n\n👩🏽‍💻 <b>Подлинная</b> телеграм-ссылка: <code>https://t.me/{0}/web?startapp={1}_{2}</code>",
-    'en': "👩🏽‍💻 *Promo code*: `{txt}` activated",
-    'es': "👩🏽‍💻 *Código promocional*: `{txt}` activado",
-    'fr': "👩🏽‍💻 *Code promotionnel* : `{txt}` activé",
-    'zh': "👩🏽‍💻 *促销代码*：`{txt}` 激活",
-    'ar': "👩🏽‍💻 * الرمز الترويجي *: '{txt}` مفعل",
-}
 
 # region commands
 l_bot_commands_handler = {
-    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/status <i>статус</i>\n/on     <i>включение</i>\n/off    <i>выключение</i>\n/restart  <i>перезагрузка</i>\n\n/parse [premium|promo|utm|old]\n/admin [id]    <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>\n/unban     <i>разбан</i>\n/transfer [id] <i>передача прав</i>",
+    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/status <i>статус</i>\n/on     <i>включение</i>\n/off    <i>выключение</i>\n/restart  <i>перезагрузка</i>\n\n/parse [premium|admin|utm|ban]\n/admin [id]    <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>\n/unban     <i>разбан</i>",
     'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>promo code</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
     'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disabled</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>administradores</i>\n/promo <i>código de promoción</i>\n/ban [id/ @username ] <i>lista</i>\n/unban <i>no baneado</i>",
     'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>recharger</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>code promo</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
     'zh': "⚙️<b>命令</b>/cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo<i>促销代码</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
     'ar': "⚙️ <b>أوامر</b> / cmd لـ <b>@ {0}</b>\n\n/ info <i>info</i>\n/ stat <i>analytics</i>\n/ status <i>status</i>\n/ on <i>تمكين</i>\n/off <i>تعطيل</i>\n/restart <i>تحميل</i>\n\n/ parse [premium | admin | utm | ban]\n/ admin [id] <i>admins</i>\n/ <i>promo code</i>\n/ ban [id / @username ] <i>list</i>\n/ <i>unsanned</i>",
 }
 l_bot_status_handler = {
@@ -1233,39 +1153,31 @@
     'en': "👩🏽‍💻 <b>Status</b> @{0}-bot: {1}",
     'es': "👩🏽‍💻 <b>Estado</b> @{0}-bot: {1}",
     'fr': "👩🏽‍💻 <b>Statut</b> @{0}-bot : {1}",
     'zh': "👩🏽‍💻<b>状态</b>@{0}-bot：{1}",
     'ar': "👩🏽‍💻 <b>الحالة</b> @ {0} -روبوت: {1}",
 }
 l_bot_on_handler = {
-    'ru': "👩🏽‍💻 <b>Запуск</b> @{0}-бота..\n#длительность 0мин",
+    'ru': "👩🏽‍💻 <b>Запуск</b> @{0}-бота..\n\n#длительность 1мин",
     'en': "👩🏽‍💻 <b>Launch</b> @{0}-bot..\n\n#duration 1 min",
     'es': "👩🏽‍💻 <b>Lanzar</b> @{0}-bot..\n\n#duración 1 min",
     'fr': "👩🏽‍💻 <b>Lancer</b> @{0}-bot..\n\n#durée 1 min",
     'zh': "👩🏽‍💻<b>启动</b>@{0}-bot..\n\n#duration 1 分钟",
     'ar': "👩🏽‍💻 <b>Launch</b> @ {0} -bot ..\n\n# المدة 1 دقيقة",
 }
-l_bot_on_handler_done = {
-    'ru': "👩🏽‍💻 <b>@{0}</b>-бот запущен",
-    'en': "👩🏽‍💻 <b>@{0}</b> - the bot is already running",
-    'es': "👩🏽‍💻 <b>@{0}</b> : el bot ya se está ejecutando",
-    'fr': "👩🏽‍💻 <b>@{0}</b> - le bot est déjà en cours d'exécution",
-    'zh': "👩🏽‍💻 <b>@{0}</b> - 机器人已经在运行",
-    'ar': "👩🏽‍💻 <b>@ {0}</b> - الروبوت قيد التشغيل بالفعل",
-}
 l_bot_on_handler_already = {
     'ru': "👩🏽‍💻 <b>@{0}</b>-бот уже запущен",
     'en': "👩🏽‍💻 <b>@{0}</b> - the bot is already running",
     'es': "👩🏽‍💻 <b>@{0}</b> : el bot ya se está ejecutando",
     'fr': "👩🏽‍💻 <b>@{0}</b> - le bot est déjà en cours d'exécution",
     'zh': "👩🏽‍💻 <b>@{0}</b> - 机器人已经在运行",
     'ar': "👩🏽‍💻 <b>@ {0}</b> - الروبوت قيد التشغيل بالفعل",
 }
 l_bot_off_handler = {
-    'ru': "👩🏽‍💻 <b>Остановка</b> @{0}-бота..\n#длительность 0мин",
+    'ru': "👩🏽‍💻 <b>Остановка</b> @{0}-бота..\n\n#длительность 1мин",
     'en': "👩🏽‍💻 @{0}-bot <b>stop</b> ..\n\n#duration 1 min",
     'es': "👩🏽‍💻 @{0}-bot <b>parada</b> ..\n\n#duración 1 min",
     'fr': "👩🏽‍💻 @{0}-bot <b>stop</b> ..\n\n#durée 1 min",
     'zh': "👩🏽‍💻 @{0}-bot<b>停止</b>..\n\n#duration 1 分钟",
     'ar': "👩🏽‍💻 @ {0} -bot <b>stop</b> ..\n\n# المدة 1 دقيقة",
 }
 l_bot_off_handler_already = {
@@ -1281,46 +1193,21 @@
     'en': "👩🏽‍💻 <b>@{0}</b> -bot is off",
     'es': "👩🏽‍💻 <b>@{0}</b> -bot está apagado",
     'fr': "👩🏽‍💻 <b>@{0}</b> -bot est désactivé",
     'zh': "👩🏽‍💻 <b>@{0}</b> -bot 已关闭",
     'ar': "👩🏽‍💻 <b>@ {0}</b> -الروبوت غير مفعّل",
 }
 l_bot_restart_handler = {
-    'ru': "👩🏽‍💻 <b>Перезапуск</b> @{0}-бота..\n#длительность 0мин",
+    'ru': "👩🏽‍💻 <b>Перезапуск</b> @{0}-бота..\n\n#длительность 1мин",
     'en': "👩🏽‍💻 @{0}-bot <b>restart</b> ..\n\n#duration 1 min",
     'es': "👩🏽‍💻 @{0}-bot <b>reinicio</b> ..\n\n#duración 1 min",
     'fr': "👩🏽‍💻 @{0}-bot <b>restart</b> ..\n\n#durée 1 min",
     'zh': "👩🏽‍💻@{0}-bot<b>重启</b>..\n\n#duration 1 分钟",
     'ar': "👩🏽‍💻 @ {0} -bot <b>إعادة التشغيل</b> ..\n\n# المدة 1 دقيقة",
 }
-l_bot_update_users = {
-    'ru': "👩🏽‍💻 <b>Загружено</b> пользователей в {0}-бота: <u>{1}</u>\n\n👩🏽‍💻 <b>Корректность</b> данных о пользователях обновляется: <i>автоматически, периодически и непрерывно</i>",
-    'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>promo code</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disabled</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>administradores</i>\n/promo <i>código de promoción</i>\n/ban [id/ @username ] <i>lista</i>\n/unban <i>no baneado</i>",
-    'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>recharger</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>code promo</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'zh': "⚙️<b>命令</b>/cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo<i>促销代码</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'ar': "⚙️ <b>أوامر</b> / cmd لـ <b>@ {0}</b>\n\n/ info <i>info</i>\n/ stat <i>analytics</i>\n/ status <i>status</i>\n/ on <i>تمكين</i>\n/off <i>تعطيل</i>\n/restart <i>تحميل</i>\n\n/ parse [premium | admin | utm | ban]\n/ admin [id] <i>admins</i>\n/ <i>promo code</i>\n/ ban [id / @username ] <i>list</i>\n/ <i>unsanned</i>",
-}
-l_bot_transfer_to = {
-    'ru': "👩🏽‍💻 @{0} - успешно передан пользователю: <code>{1}</code>",
-    'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>promo code</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disabled</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>administradores</i>\n/promo <i>código de promoción</i>\n/ban [id/ @username ] <i>lista</i>\n/unban <i>no baneado</i>",
-    'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>recharger</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>code promo</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'zh': "⚙️<b>命令</b>/cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo<i>促销代码</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'ar': "⚙️ <b>أوامر</b> / cmd لـ <b>@ {0}</b>\n\n/ info <i>info</i>\n/ stat <i>analytics</i>\n/ status <i>status</i>\n/ on <i>تمكين</i>\n/off <i>تعطيل</i>\n/restart <i>تحميل</i>\n\n/ parse [premium | admin | utm | ban]\n/ admin [id] <i>admins</i>\n/ <i>promo code</i>\n/ ban [id / @username ] <i>list</i>\n/ <i>unsanned</i>",
-}
-l_bot_transfer_from = {
-    'ru': "👩🏽‍💻 @{0} - успешно получен от пользователя: <code>{1}</code>",
-    'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>promo code</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disabled</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>administradores</i>\n/promo <i>código de promoción</i>\n/ban [id/ @username ] <i>lista</i>\n/unban <i>no baneado</i>",
-    'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>recharger</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>code promo</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'zh': "⚙️<b>命令</b>/cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo<i>促销代码</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'ar': "⚙️ <b>أوامر</b> / cmd لـ <b>@ {0}</b>\n\n/ info <i>info</i>\n/ stat <i>analytics</i>\n/ status <i>status</i>\n/ on <i>تمكين</i>\n/off <i>تعطيل</i>\n/restart <i>تحميل</i>\n\n/ parse [premium | admin | utm | ban]\n/ admin [id] <i>admins</i>\n/ <i>promo code</i>\n/ ban [id / @username ] <i>list</i>\n/ <i>unsanned</i>",
-}
-
 # endregion
 
 
 # region bot
 l_bot_config = {
     ("cctor", "👩🏽‍💻", "☑"): {
         'ru': "Конструктор ᴺᴱᵂ",
@@ -1408,49 +1295,34 @@
     'ru': "🚫Убрать бота",
     'en': "🚫Remove bot",
     'es': "🚫Eliminar bot",
     'fr': "🚫Supprimer le robot",
     'zh': "🚫删除机器人",
     'ar': "🚫 إزالة البوت",
 }
+
 l_show_bots = {
     'ru': "👩🏽‍💻 <b>Добавленные боты</b>\n\n[команды /cmd]",
     'en': "👩🏽‍💻 <b>Added bots</b>\n\n[commands /cmd]",
     'es': "👩🏽‍💻 <b>Se agregaron bots</b>\n\n[comandos /cmd]",
     'fr': "👩🏽‍💻 <b>Ajout de bots</b>\n\n[commandes /cmd]",
     'zh': "👩🏽‍💻<b>添加了机器人</b>\n\n[命令/cmd]",
     'ar': "👩🏽‍💻 <b>الروبوتات المضافة</b>\n\n[أوامر / cmd]",
 }
-l_wait_free_ip = {
-    'ru': "👩🏽‍💻 <b>Ожидание</b> свободных ресурсов для создания бота..\n#длительность 21мин",
-    'en': "🚫Remove bot",
-    'es': "🚫Eliminar bot",
-    'fr': "🚫Supprimer le robot",
-    'zh': "🚫删除机器人",
-    'ar': "🚫 إزالة البوت",
-}
-l_bot_token_taken = {
-    'ru': "👩🏽‍💻 <b>Токен</b>: {0} уже используется другим пользователем\n\n👩🏽‍💻 <b>Необходимо</b> перевыпустить/отозвать токен в @BotFather",
-    'en': "🚫Remove bot",
-    'es': "🚫Eliminar bot",
-    'fr': "🚫Supprimer le robot",
-    'zh': "🚫删除机器人",
-    'ar': "🚫 إزالة البوت",
-}
 
 l_creturntext = {
     'ru': "✖️ <b>Сбросить</b> настройки по умолчанию (до рекомендуемых) для бота [<b>{0}</b>]?",
     'en': "✖️ <b>Reset</b> default settings (recommended) for bot [<b>{0}</b>]?",
     'es': "✖️ <b>¿Restablecer</b> la configuración predeterminada (recomendado) para el bot [<b>{0}</b>]?",
     'fr': "✖️ <b>Réinitialiser</b> les paramètres par défaut (recommandé) pour le bot [<b>{0}</b>] ?",
     'zh': "✖️<b>重置</b>机器人 [<b>{0}</b>] 的默认设置（推荐）？",
     'ar': "✖️ <b>إعادة تعيين</b> الإعدادات الافتراضية (موصى به) للروبوت [<b>{0}</b>]؟",
 }
 l_creturnanswer = {
-    'ru': "✖️ <b>Настройки</b> бота [<b>{0}</b>] успешно сброшены!",
+    'ru': "✖️ Настройки бота [<b>{0}</b>] успешно сброшены!",
     'en': "✖️ Bot settings [<b>{0}</b>] successfully reset!",
     'es': "✖️ ¡La configuración del bot [<b>{0}</b>] se restableció correctamente!",
     'fr': "✖️ Les paramètres du bot [<b>{0}</b>] ont été réinitialisés avec succès !",
     'zh': "✖️ 机器人设置 [<b>{0}</b>] 成功重置！",
     'ar': "✖️ تم إعادة تعيين إعدادات البوت [<b>{0}</b>] بنجاح!",
 }
 l_cdeletetext = {
@@ -1477,57 +1349,14 @@
     'zh': "👩🏽‍💻 @{0}-bot 的<b>所有权</b>已成功转移到@{1}-帐户！\n\n👩🏽‍💻 您现在可以使用@botfather -bot 转移所有权/配置",
     'ar': "👩🏽‍💻 تم نقل <b>ملكية</b> @ {0} -bot بنجاح إلى @ {1} -account!\n\n👩🏽‍💻 يمكنك الآن استخدام @botfather -bot لنقل الملكية / التهيئة",
 }
 # endregion
 
 
 # region config
-# region cpost_
-l_pstsound = {
-    'ru': "🔈 <b>Жми</b> на ✅/🔘 чтобы <b>Вкл/Выкл</b> режим отправки со звуком <i>по умолчанию</i>/<i>тихий режим</i> без звука/<i>закреп-пин</i>\n\n📍 <b>Режим</b> [✅ Закреп] - позволяет оповестить пользователя даже при отключенных уведомлениях",
-    'en': "👋🏽 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to text messages using neural network",
-    'es': "👋🏽 <b>Presione</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática a los mensajes de texto usando la red neuronal",
-    'fr': "👋🏽 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique aux messages texte à l'aide du réseau neuronal",
-    'zh': "👋🏽<b>按</b>✅/☑️ 使用神经网络<b>打开/关闭</b>自动回复短信",
-    'ar': "👋🏽 <b>اضغط</b> <b>على ✅ / ☑️ لتشغيل / إيقاف</b> الرد التلقائي على الرسائل النصية باستخدام الشبكة العصبية",
-}
-l_pstmedia = {
-    'ru': "👩🏽‍💻 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> режим просмотра поста: <i>превью-предпросмотр</i>/<i>спойлер-скрытый</i>/<i>галерея</i>\n\n[✅ превью]-режим помещает медиа-контент <i>(jpg/gif/mp4 до 5 Мб)</i> под текстом\n[✅ формат]-режим применяет случайные стили к посту",
-    'en': "👋🏽 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to text messages using neural network",
-    'es': "👋🏽 <b>Presione</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática a los mensajes de texto usando la red neuronal",
-    'fr': "👋🏽 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique aux messages texte à l'aide du réseau neuronal",
-    'zh': "👋🏽<b>按</b>✅/☑️ 使用神经网络<b>打开/关闭</b>自动回复短信",
-    'ar': "👋🏽 <b>اضغط</b> <b>على ✅ / ☑️ لتشغيل / إيقاف</b> الرد التلقائي على الرسائل النصية باستخدام الشبكة العصبية",
-}
-l_mode_spoiler = {
-    'ru': "👩🏽‍💻 Режим [✅ спойлер] доступен для фото/гиф/видео-форматов",
-    'en': "👋🏽 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to text messages using neural network",
-    'es': "👋🏽 <b>Presione</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática a los mensajes de texto usando la red neuronal",
-    'fr': "👋🏽 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique aux messages texte à l'aide du réseau neuronal",
-    'zh': "👋🏽<b>按</b>✅/☑️ 使用神经网络<b>打开/关闭</b>自动回复短信",
-    'ar': "👋🏽 <b>اضغط</b> <b>على ✅ / ☑️ لتشغيل / إيقاف</b> الرد التلقائي على الرسائل النصية باستخدام الشبكة العصبية",
-}
-l_mode_album = {
-    'ru': "👩🏽‍💻 Режим [✅ альбом] доступен для фото/видео/аудио/документов",
-    'en': "👋🏽 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to text messages using neural network",
-    'es': "👋🏽 <b>Presione</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática a los mensajes de texto usando la red neuronal",
-    'fr': "👋🏽 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique aux messages texte à l'aide du réseau neuronal",
-    'zh': "👋🏽<b>按</b>✅/☑️ 使用神经网络<b>打开/关闭</b>自动回复短信",
-    'ar': "👋🏽 <b>اضغط</b> <b>على ✅ / ☑️ لتشغيل / إيقاف</b> الرد التلقائي على الرسائل النصية باستخدام الشبكة العصبية",
-}
-l_mode_gallery = {
-    'ru': "👩🏽‍💻 Режим [✅ галерея] доступен для фото/видео/аудио/документов",
-    'en': "👋🏽 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to text messages using neural network",
-    'es': "👋🏽 <b>Presione</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática a los mensajes de texto usando la red neuronal",
-    'fr': "👋🏽 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique aux messages texte à l'aide du réseau neuronal",
-    'zh': "👋🏽<b>按</b>✅/☑️ 使用神经网络<b>打开/关闭</b>自动回复短信",
-    'ar': "👋🏽 <b>اضغط</b> <b>على ✅ / ☑️ لتشغيل / إيقاف</b> الرد التلقائي على الرسائل النصية باستخدام الشبكة العصبية",
-}
-# endregion
-
 # region ctranslate_
 l_ctranslate_text = {
     'ru': "文 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> авто-перевод для <i>исходящих</i> сообщений бота на язык пользователя при /start-запуске бота",
     'en': "文<b>Click</b> on ✅/☑️ to <b>enable/disable</b> auto-translate for <i>outgoing</i> bot messages into the user's language when /start-starting the bot",
     'es': "文<b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> la traducción automática de los mensajes <i>salientes</i> del bot al idioma del usuario cuando/inicie el bot",
     'fr': "文<b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> la traduction automatique des messages <i>sortants</i> du bot dans la langue de l'utilisateur lors du/démarrage du bot",
     'zh': "文<b>单击</b>✅/☑️<b>启用/禁用</b>在/启动机器人时将<i>传出的</i>机器人消息自动翻译成用户的语言",
@@ -1866,23 +1695,23 @@
     'en': "👥 <b>Think of</b> a name for the /utm link (*after ?start= there can be <u>any</u> source name from numbers and/or Latin letters)\n\n👩🏽‍💻 <b>For example</b> , /utm referral links for tracking:\nhttps://t .me/{0}?start={1} - <i>referral users</i> {1} - <i>user</i>\nhttps://t.me/{0}?start=instagram - <i>users from instagram</i>",
     'es': "👥 <b>Piense en</b> un nombre para el enlace /utm (*después de ?start= puede haber <u>cualquier</u> nombre de fuente de números y/o letras latinas)\n\n👩🏽‍💻 <b>Por ejemplo</b> , enlaces de referencia /utm para el seguimiento:\nhttps ://t .me/{0}?start={1} - <i>usuarios de referencia</i> {1} - <i>usuario</i>\nhttps://t.me/{0}?start=instagram - <i>usuarios de instagram</i>",
     'fr': "👥 <b>Pensez à</b> un nom pour le lien /utm (*après ?start= il peut y avoir <u>n&#x27;importe quel</u> nom de source à partir de chiffres et/ou de lettres latines)\n\n👩🏽‍💻 <b>Par exemple</b> , les liens de référence /utm pour le suivi :\nhttps ://t .me/{0}?start={1} - <i>utilisateurs de référence</i> {1} - <i>utilisateur</i>\nhttps://t.me/{0}?start=instagram - <i>utilisateurs d&#x27;instagram</i>",
     'zh': "👥<b>为 /utm 链接想</b>一个名字（*在?start=之后可以有<u>任何</u>来自数字和/或拉丁字母的源名称）\n\n👩🏽‍💻<b>例如</b>，用于跟踪的 /utm 推荐链接：\nhttps ://t .me/{0}?start={1} -<i>推荐用户</i>{1} -<i>用户</i>\nhttps://t.me/{0}?start=instagram -<i>来自 instagram 的用户</i>",
     'ar': "👥 <b>فكر في</b> اسم ارتباط / utm (* after ?start= يمكن أن يكون هناك <u>أي</u> اسم مصدر من الأرقام و / أو الأحرف اللاتينية)\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، روابط الإحالة / utm للتتبع:\nhttps : // t .me / {0}؟ start = {1} - <i>المستخدمون المحالون</i> {1} - <i>المستخدم</i>\nhttps: //t.me/ {0}؟ start = instagram - <i>المستخدمون من instagram</i>",
 }
 l_promo_done = {
-    'ru': "👩🏽‍💻 <b>Готово!</b>\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{0}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n<code>/promo 0</code>\n\n⚙️ <b>Команды</b> /cmd",
+    'ru': "👩🏽‍💻 <b>Готово!</b>\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{0}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n/promo 0",
     'en': "👩🏽‍💻 <b>Done!</b>\n\n👩🏽‍💻 <i>Current /promo code</i> :\n{0}\n👩🏽‍💻 <i>Delete /promo code</i> :\n/promo 0",
     'es': "👩🏽‍💻 <b>Listo!</b>\n\n👩🏽‍💻 <i>Código /promocional actual</i> :\n{0}\n👩🏽‍💻 <i>Eliminar código /promocional</i> :\n/promo 0",
     'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 <i>Code /promo actuel</i> :\n{0}\n👩🏽‍💻 <i>Supprimer le code /promo</i> :\n/promo 0",
     'zh': "👩🏽‍💻<b>完成！</b>\n\n👩🏽‍💻<i>当前/促销代码</i>：\n{0}\n👩🏽‍💻<i>删除/促销代码</i>：\n/promo 0",
     'ar': "👩🏽‍💻 <b>انتهى!</b>\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n{0}\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n/promo 0",
 }
 l_promo_start = {
-    'ru': "👩🏽‍💻 <b>Введи</b> /promo-код для @{0}-бота:\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{1}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n<code>/promo 0</code>\n\n⚙️ <b>Команды</b> /cmd",
+    'ru': "👩🏽‍💻 <b>Введи</b> /promo-код для @{0}-бота:\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{1}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n/promo 0",
     'en': "👩🏽‍💻 <b>Enter</b> /promo code for @{0}-bot:\n\n👩🏽‍💻 <i>Current /promo code</i> :\n{1}\n👩🏽‍💻 <i>Delete /promo code</i> :\n/promo 0",
     'es': "👩🏽‍💻 <b>Ingresa el</b> /código de promoción para @{0}-bot:\n\n👩🏽‍💻 <i>Actual /código de promoción</i> :\n{1}\n👩🏽‍💻 <i>Eliminar /código de promoción</i> :\n/promo 0",
     'fr': "👩🏽‍💻 <b>Entrez</b> /code promo pour @{0}-bot :\n\n👩🏽‍💻 <i>Code /code promo actuel</i> :\n{1}\n👩🏽‍💻 <i>Supprimer /code promo</i> :\n/promo 0",
     'zh': "👩🏽‍💻<b>输入</b>@{0}-bot 的 /promo 代码：\n\n👩🏽‍💻<i>当前 /promo 代码</i>：\n{1}\n👩🏽‍💻<i>删除 /promo 代码</i>：\n/promo 0",
     'ar': "👩🏽‍💻 <b>أدخل</b> / الرمز الترويجي لـ @ {0} -bot:\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n{1}\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n/promo 0",
 }
 # endregion
@@ -1894,15 +1723,15 @@
     'en': "👮🏽 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>access of added administrators to functionality <b>[💬 Notifications]</b></i>\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/admin - add/remove administrator\n/parse - display all users",
     'es': "👮🏽 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i>el acceso de los administradores agregados a la funcionalidad <b>[💬 Notificaciones]</b></i>\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/admin - agregar/eliminar administrador\n/ analizar - mostrar todos los usuarios",
     'fr': "👮🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>l&#x27;accès des administrateurs ajoutés à la fonctionnalité <b>[💬 Notifications]</b></i>\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/admin - ajouter/supprimer un administrateur\n/ parse - affiche tous les utilisateurs",
     'zh': "👮🏽<b>单击</b>✅/☑️<b>启用/禁用</b><i>添加的管理员对功能的访问<b>[💬 通知]</b></i>\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/admin - 添加/删除管理员\n/ parse - 显示所有用户",
     'ar': "👮🏽 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>وصول المسؤولين المضافين إلى الوظائف <b>[💬 إعلامات]</b></i>\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - كافة الأوامر\n/ admin - إضافة / إزالة المسؤول\n/ تحليل - عرض جميع المستخدمين",
 }
 l_cadmin_done = {
-    'ru': "👮🏽 <b>Готово!</b> /admin-список @{0}-бота:\n\n{1}\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{2}/10</u>",
+    'ru': "👮🏽 <b>Готово!</b>/admin-список @{0}-бота:\n\n{1}\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{2}/10</u>",
     'en': "👮🏽 <b>Done!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/admin - add/remove administrator\n/parse - display all users\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{2}/10</u>",
     'es': "👮🏽 <b>Listo!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/admin - agregar/eliminar administrador\n/parse - mostrar todos los usuarios\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{2}/10</u>",
     'fr': "👮🏽 <b>C&#x27;est fait !</b> /admin-list @{0}-bot :\n\n{1}\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/admin - ajouter/supprimer un administrateur\n/parse - afficher tous les utilisateurs\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{2}/10</u>",
     'zh': "👮🏽<b>完成！</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/admin - 添加/删除管理员\n/parse - 显示所有用户\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{2}/10</u>",
     'ar': "👮🏽 <b>انتهى!</b> / admin-list @ {0} -bot:\n\n{1}\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ admin - إضافة / إزالة المسؤول\n/ parse - عرض جميع المستخدمين\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{2} / 10</u>",
 }
 l_cadmin_add = {
@@ -1918,15 +1747,15 @@
     'en': "👮🏽 <b>Enter</b> user id separated by spaces or separators to remove them from /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
     'es': "👮🏽 <b>Ingrese</b> id de usuario separados por espacios o separadores para eliminarlos de /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
     'fr': "👮🏽 <b>Entrez</b> id d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les supprimer de /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
     'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户id ，以将其从 /admin-list 中删除\n\n👩🏽‍💻<b>当前</b>管理员数量： <u>{0}</u>",
     'ar': "👮🏽 <b>أدخل</b> id المستخدمين مفصولة بمسافات أو فواصل لإزالتها من / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
 }
 l_parse_text = {
-    'ru': "👩🏽‍💻 <b>Готово!</b> Парсинг пользователей (<u>{0}</u>) @{1}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse     <i>все пользователи бота</i>\n<code>/parse utm</code>   <i>utm-рефералы</i>\n<code>/parse ban</code>    <i>ban-пользователи</i>\n<code>/parse old</code>    <i>старые id-пользователи</i>\n<code>/parse admin</code>    <i>admin-пользователи</i>\n<code>/parse promo</code>    <i>promo-пользователи</i>\n<code>/parse premium</code>    <i>premium-пользователи</i>",
+    'ru': "👩🏽‍💻 <b>Готово!</b> Парсинг пользователей (<u>{0}</u>) @{1}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/parse premium - вывести premium-пользователей\n/parse admin - вывести admin-пользователей\n/parse utm - вывести utm-рефералов\n",
     'en': "👩🏽‍💻 <b>Done!</b> Parsing users ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - print all users\n/parse premium - print premium users\n/parse admin - display admin users\n/parse utm - display utm referrals\n",
     'es': "👩🏽‍💻 <b>Listo!</b> Analizando usuarios ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - imprimir todos los usuarios\n/parse premium - imprimir usuarios premium\n/parse admin - mostrar usuarios administradores\n/parse utm - mostrar referencias utm\n",
     'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b> Analyse des utilisateurs ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - imprimer tous les utilisateurs\n/parse premium - imprimer les utilisateurs premium\n/parse admin - affiche les utilisateurs administrateurs\n/parse utm - affiche les références utm\n",
     'zh': "👩🏽‍💻<b>完成！</b>解析用户（ <u>{0}</u> ）@{1}-bot\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 打印所有用户\n/parse premium - 打印高级用户\n/parse admin - 显示管理员用户\n/parse utm - 显示 utm 引用\n",
     'ar': "👩🏽‍💻 <b>انتهى!</b> تحليل المستخدمين ( <u>{0}</u> ) @ {1} -bot\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ تحليل - طباعة جميع المستخدمين\n/parse premium - طباعة المستخدمين المتميزين\n/parse admin - عرض المستخدمين المسؤولين\n/parse utm - عرض إحالات UTM\n",
 }
 # endregion
@@ -1970,23 +1799,14 @@
     'ru': "👩🏽‍💻 <b>Нет прав</b> для записи в данную таблицу: {0}\n\n👩🏽‍💻 <b>Необходимо</b> заново добавить корректную ссылку на таблицу в @{1}-боте",
     'en': "Profile photo: @{1}Landing blog for promotion in <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Description{5}",
     'es': "Foto de perfil: @{1}Blog de aterrizaje para promoción en <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Descripción{5}",
     'fr': "Photo de profil : @{1}Blog d'atterrissage pour la promotion dans <i>Telegram</i> 👩🏽‍💻 <b>bot :</b> {2}[<b>id</b> = {3}] <b>Bio :</b> {4}Description{5}",
     'zh': "个人资料照片：@{1}登陆博客以在<i>Telegram</i> 👩🏽‍💻<b>机器人中进行推广：</b> {2}[<b>id</b> = {3}]<b>简介：</b> {4}说明{5}",
     'ar': "صورة الملف الشخصي: @ {1} مدونة الهبوط للترويج في <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2} [<b>id</b> = {3}] <b>السيرة الذاتية:</b> {4} الوصف {5}",
 }
-l_transfer_need_username  = {
-    'ru': "👩🏽‍💻 <b>Создай</b> @username своего аккаунта, чтобы получить права на @{0}-бота",
-    'en': "Profile photo: @{1}Landing blog for promotion in <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Description{5}",
-    'es': "Foto de perfil: @{1}Blog de aterrizaje para promoción en <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Descripción{5}",
-    'fr': "Photo de profil : @{1}Blog d'atterrissage pour la promotion dans <i>Telegram</i> 👩🏽‍💻 <b>bot :</b> {2}[<b>id</b> = {3}] <b>Bio :</b> {4}Description{5}",
-    'zh': "个人资料照片：@{1}登陆博客以在<i>Telegram</i> 👩🏽‍💻<b>机器人中进行推广：</b> {2}[<b>id</b> = {3}]<b>简介：</b> {4}说明{5}",
-    'ar': "صورة الملف الشخصي: @ {1} مدونة الهبوط للترويج في <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2} [<b>id</b> = {3}] <b>السيرة الذاتية:</b> {4} الوصف {5}",
-}
-
 # endregion
 
 
 # region extra bot
 l_show_admin_panel_md = {
     'ru': "*👩🏽‍💻 Создание и редактирование блога*\n\n👩🏽‍💻 Вы зашли как *Администратор* и можете создавать и редактировать блоги, но не удалять их\n\n¹ Авторизация (в течение 10сек) по ссылке в браузере:\n`{0}`\n\n² Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
     'en': "*👩🏽‍💻 Creating and editing a blog*\n\n👩🏽‍💻 You are logged in as *Administrator* and can create and edit blogs, but not delete them\n\n¹ Authorization via link in browser:\n`{0 }`\n\n² Go (within 10 seconds) to the desired link to edit the post (click to copy):\n\n",
@@ -2015,151 +1835,29 @@
     'ru': "👩🏽‍💻 Авторизация",
     'en': "👩🏽‍💻 Authorization",
     'es': "👩🏽‍💻 Autorización",
     'fr': "👩🏽‍💻 Autorisation",
     'zh': "👩🏽‍💻授权",
     'ar': "👩🏽‍💻 إذن",
 }
-
-l_triggers = {
-    'ru': "Триггеры",
-    'en': "Triggers",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_actions2 = {
-    'ru': "Действия",
-    'en': "Actions",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_messages = {
-    'ru': "Сообщения",
-    'en': "Messages",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_languages = {
-    'ru': "Языки",
-    'en': "Languages",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_buttons = {
-    'ru': "Кнопки",
-    'en': "Buttons",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_medias = {
-    'ru': "Медиа",
-    'en': "Medias",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-
-l_users = {
-    'ru': "Пользователи",
-    'en': "Users",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_promos = {
-    'ru': "Promo-пользователи",
-    'en': "Promos",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_utms = {
-    'ru': "UTM-пользователи",
-    'en': "Promos",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_premiums = {
-    'ru': "Premium-пользователи",
-    'en': "Promos",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_bans = {
-    'ru': "Бан-пользователи",
-    'en': "Promos",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_auto_translate = {
-    'ru': "Авто-перевод",
-    'en': "Auto-translate",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_auto_answer = {
-    'ru': "Авто-ответ",
-    'en': "Auto-answer",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
-l_auto_post = {
-    'ru': "Авто-постинг",
-    'en': "Auto-post",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
-}
 # endregion
 
 
 # region html
 l_burger_save = {
     'ru': "Сохранить",
     'en': "Save",
     'es': "Ahorrar",
     'fr': "Sauvegarder",
     'zh': "节省",
     'ar': "يحفظ",
 }
-l_burger_ai = {
-    'ru': "AI бот ᴺᴱᵂ",
-    'en': "AI bot ᴺᴱᵂ",
-    'es': "Generar bot",
-    'fr': "Générer un robot",
-    'zh': "生成机器人",
-    'ar': "توليد بوت",
-}
-l_burger_template = {
-    'ru': "Шаблон бота",
-    'en': "Template bot",
+l_burger_gen = {
+    'ru': "Сгенерировать бота",
+    'en': "Generate bot",
     'es': "Generar bot",
     'fr': "Générer un robot",
     'zh': "生成机器人",
     'ar': "توليد بوت",
 }
 l_burger_import = {
     'ru': "Импортировать .bot",
@@ -2386,15 +2084,15 @@
     'es': "+ solicitud",
     'fr': "+ demande",
     'zh': "+ 要求",
     'ar': "+ طلب",
 }
 
 l_msg_text = {
-    'ru': ": текст",
+    'ru': ": text",
     'en': ": text",
     'es': ": texto",
     'fr': ": texte",
     'zh': "： 文本",
     'ar': ": نص",
 }
 l_msg_photo = {
@@ -2473,22 +2171,14 @@
     'ru': ": игра",
     'en': ": game",
     'es': ": juego",
     'fr': ": jeu",
     'zh': "： 游戏",
     'ar': ": لعبة",
 }
-l_msg_web = {
-    'ru': ": веб",
-    'en': ": web",
-    'es': ": juego",
-    'fr': ": jeu",
-    'zh': "： 游戏",
-    'ar': ": لعبة",
-}
 
 l_btn_button_in = {
     'ru': "✅ Кнопка ↑",
     'en': "✅ Button ↑",
     'es': "✅ Botón ↑",
     'fr': "✅ Bouton ↑",
     'zh': "✅按钮↑",
@@ -2522,22 +2212,14 @@
     'ru': "❤️ Лайк",
     'en': "❤️ Like",
     'es': "❤️ Me gusta",
     'fr': "❤️ J'aime",
     'zh': "❤️喜欢",
     'ar': "❤️ مثل",
 }
-l_btn_web = {
-    'ru': "🌐 Веб",
-    'en': "❤️ Like",
-    'es': "❤️ Me gusta",
-    'fr': "❤️ J'aime",
-    'zh': "❤️喜欢",
-    'ar': "❤️ مثل",
-}
 l_btn_button_kb = {
     'ru': "✅ Кнопка ↓",
     'en': "✅ Button ↓",
     'es': "✅ Botón ↓",
     'fr': "✅ Bouton ↓",
     'zh': "✅按钮↓",
     'ar': "✅ زر ↓",
@@ -2648,39 +2330,14 @@
     'ar': "رسالة هادئة",
 }
 # endregion
 # endregion
 
 
 # region FereyUserBot
-l_user_btn1 = {
-    'ru': "⛰️ Пользователи",
-    'en': "⛰️ Channels",
-    'es': "⛰️ Canales",
-    'fr': "⛰️ Chaînes",
-    'zh': "⛰️频道",
-    'ar': "⛰️ القنوات",
-}
-l_user_btn2 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
-}
-l_user_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> автоматизации <b>Telegram</b>-аккаунтов:\n\n▪️<b>защита</b>\n▪️<b>организация</b>\n▪️<b>сбор</b>\n▪️<b>кнопочный</b>\n▪️<b>реакции</b>\n▪️<b>авто-декор</b>\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to the <b>Telegram</b> channel администрирования <i>landing bot</i> :\n\n▪️ <b>protection</b> of the channel from spyware entry\n▪️display <b>of statistics</b> and engagement (%)\n▪️restriction of rights before <b>subscribing</b> to the channel\n▪️ <b>organization</b> of a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> администрирования de canales <b>de Telegram</b> :\n\ <b>n▪️protección</b> del canal contra la entrada de software espía\n▪️visualización <b>de estadísticas</b> e interacción (%)\n▪️restricción de derechos antes de <b>suscribirse</b> al canal\n▪️ <b>organización</b> de una prohibición y anti-inundación\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> администрирования de la chaîne <b>Telegram</b> :\n\n▪️ <b>protection</b> de la chaîne contre l&#x27;entrée de logiciels espions\n▪️affichage <b>des statistiques</b> et de l&#x27;engagement (%)\n▪️restriction des droits avant de <b>s&#x27;abonner</b> à la chaîne\n<b>▪️organisation</b> d'une interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
-    'zh': "🌱 {0}，欢迎使用<b>Telegram</b>频道администрирования<i>登陆机器人</i>：\n\n▪️<b>保护</b>频道免受间谍软件入侵\n▪️ 显示<b>统计信息</b>和参与度 (%)\n▪️<b>订阅</b>频道前的权利限制\n▪️<b>组织</b>禁令和反洪水\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت</i> администрирования قناة <b>Telegram</b> :\n\n▪️ <b>حماية</b> القناة من إدخال برامج التجسس\n▪️ <b>عرض الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> حظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
-}
-
 l_subscribe_user = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️до 5 <b>рассылок</b> пользователям\n▪️<b>авто-ответ</b> с chatgpt\n▪️<b>экстра</b> бот\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
@@ -2743,15 +2400,15 @@
     'en': "➕ Add channel",
     'es': "➕ Agregar canal",
     'fr': "➕ Ajouter une chaîne",
     'zh': "➕ 添加频道",
     'ar': "➕ إضافة قناة",
 }
 l_bot_removed = {
-    'ru': "🚫 @{0}-бот удален из <b>{1}</b> [id=<code>{2}</code>]",
+    'ru': "🚫 @{0}-бот удален из <b>{1}</b> ({2})",
     'en': "🚫 @{0}-bot removed from <b>{1}</b> ( {2} )",
     'es': "🚫 @{0}-bot eliminado de <b>{1}</b> ( {2} )",
     'fr': "🚫 @{0}-bot supprimé de <b>{1}</b> ( {2} )",
     'zh': "🚫 @{0}-bot 从<b>{1}</b> ( {2} ) 中移除",
     'ar': "🚫 @ {0} -إزالة الروبوت من <b>{1}</b> ( {2} )",
 }
 
@@ -2842,20 +2499,20 @@
     'en': "⚙️ <b>Select</b> option for /cmd <i>settings</i> [<b>{0}</b>] {1}",
     'es': "⚙️ <b>Seleccione</b> la opción para <i>la configuración de</i> /cmd [<b>{0}</b>] {1}",
     'fr': "⚙️ <b>Sélectionnez</b> l&#x27;option pour <i>les paramètres</i> /cmd [<b>{0}</b>] {1}",
     'zh': "⚙️<b>选择</b>/cmd<i>设置</i>选项 [<b>{0}</b>] {1}",
     'ar': "⚙️ <b>تحديد</b> خيار <i>إعدادات</i> / cmd [<b>{0}</b>] {1}",
 }
 l_chat_join_request_handler = {
-    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в <b>{1}</b>\n\n👩🏽‍💻 <b>Выбери</b> <i>правильный вариант</i> в соответствии с заданием на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
-    'en': "👮🏽 {0}, you submitted an application to join <b>{1}</b>\n\n👩🏽‍💻 <b>Choose</b> <i>the correct option</i> according to заданием in the picture so that your <i>application</i> to join is <b>approved</b>",
-    'es': "👮🏽 {0}, envió una solicitud para unirse <b>{1}</b>\n\n👩🏽‍💻 <b>Elija</b> <i>la opción correcta</i> de acuerdo con заданием en la imagen para que se <b>apruebe</b> su <i>solicitud</i> para unirse",
-    'fr': "👮🏽 {0}, vous avez soumis une candidature pour rejoindre <b>{1}</b>\n\n👩🏽‍💻 <b>Choisissez</b> <i>la bonne option</i> en fonction de заданием dans l&#x27;image afin que votre <i>candidature</i> soit <b>approuvée</b>",
-    'zh': "👮🏽 {0}，你提交了加入<b>{1}</b>的申请\n\n👩🏽‍💻 根据图片中的заданием<b>选择</b><i>正确的选项</i>，这样你的加入<i>申请</i>就<b>通过了</b>",
-    'ar': "👮🏽 {0} ، لقد قدمت طلبًا للانضمام <b>{1}</b>\n\n👩🏽‍💻 <b>اختر</b> <i>الخيار الصحيح</i> وفقًا заданием الموجودة في الصورة حتى تتم <b>الموافقة على</b> <i>طلبك</i> للانضمام",
+    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в <b>{1}</b>\n\n👉🏼 <b>Выбери</b> <i>правильный вариант</i> в соответствии с заданием на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
+    'en': "👮🏽 {0}, you submitted an application to join <b>{1}</b>\n\n👉🏼 <b>Choose</b> <i>the correct option</i> according to заданием in the picture so that your <i>application</i> to join is <b>approved</b>",
+    'es': "👮🏽 {0}, envió una solicitud para unirse <b>{1}</b>\n\n👉🏼 <b>Elija</b> <i>la opción correcta</i> de acuerdo con заданием en la imagen para que se <b>apruebe</b> su <i>solicitud</i> para unirse",
+    'fr': "👮🏽 {0}, vous avez soumis une candidature pour rejoindre <b>{1}</b>\n\n👉🏼 <b>Choisissez</b> <i>la bonne option</i> en fonction de заданием dans l&#x27;image afin que votre <i>candidature</i> soit <b>approuvée</b>",
+    'zh': "👮🏽 {0}，你提交了加入<b>{1}</b>的申请\n\n👉🏼 根据图片中的заданием<b>选择</b><i>正确的选项</i>，这样你的加入<i>申请</i>就<b>通过了</b>",
+    'ar': "👮🏽 {0} ، لقد قدمت طلبًا للانضمام <b>{1}</b>\n\n👉🏼 <b>اختر</b> <i>الخيار الصحيح</i> وفقًا заданием الموجودة في الصورة حتى تتم <b>الموافقة على</b> <i>طلبك</i> للانضمام",
 }
 l_content_types_sub_button = {
     'ru': "👮🏽 Я подписался",
     'en': "👮🏽 I subscribed",
     'es': "👮🏽 me suscribí",
     'fr': "👮🏽 je me suis abonné",
     'zh': "👮🏽 我订阅了",
@@ -2875,15 +2532,15 @@
     'es': "🕐 Espera 1 minuto",
     'fr': "🕐 Attendez 1min",
     'zh': "🕐 等一分钟",
     'ar': "🕐 انتظر 1 دقيقة",
 }
 
 l_creturn_answer = {
-    'ru': "✖️ <b>Настройки</b> для [<b>{0}</b>] успешно сброшены!",
+    'ru': "✖️ Настройки для [<b>{0}</b>] успешно сброшены!",
     'en': "✖️ Settings for [<b>{0}</b>] reset successfully!",
     'es': "✖️ ¡La configuración de [<b>{0}</b>] se restableció correctamente!",
     'fr': "✖️ Les paramètres de [<b>{0}</b>] ont été réinitialisés avec succès !",
     'zh': "✖️ [<b>{0}</b>] 的设置重置成功！",
     'ar': "✖️ تمت إعادة تعيين إعدادات [<b>{0}</b>] بنجاح!",
 }
 l_cdelete_text = {
@@ -3081,23 +2738,23 @@
     'es': "\n<b>#хэштеги</b> <b>de grupo</b> :\n{0}\n",
     'fr': "\n<b>Groupe</b> <b>#хэштеги</b> :\n{0}\n",
     'zh': "\n<b>组#хэштеги</b> ：\n{0}\n",
     'ar': "\n<b>Group</b> <b>#хэштеги</b> :\n{0}\n",
 }
 
 l_transfer_start = {
-    'ru': "⚠️ <b>Пользователь</b> {0} должен /start-запустить @{1}",
+    'ru': "⚠️ Пользователь {0} должен /start-запустить @{1}",
     'en': "⚠️ User {0} must /start-start @{1}",
     'es': "⚠️ El usuario {0} debe /start-start @{1}",
     'fr': "⚠️ L'utilisateur {0} doit /start-start @{1}",
     'zh': "⚠️ 用户 {0} 必须 /start-start @{1}",
     'ar': "⚠️ المستخدم {0} must / start-start @ {1}",
 }
 l_transfer_admin = {
-    'ru': "⚠️ <b>Пользователь</b> {0} должен быть <b>администратором</b> в <b>{1}</b>",
+    'ru': "⚠️ Пользователь {0} должен быть <b>администратором</b> в <b>{1}</b>",
     'en': "⚠️ User {0} must be <b>an administrator</b> in <b>{1}</b>",
     'es': "⚠️ El usuario {0} debe ser <b>administrador</b> en <b>{1}</b>",
     'fr': "⚠️ L'utilisateur {0} doit être <b>administrateur</b> dans <b>{1}</b>",
     'zh': "⚠️ 用户 {0} 必须是<b>{1}</b>的<b>管理员</b>",
     'ar': "⚠️ يجب أن يكون المستخدم {0} <b>مسؤولاً</b> في <b>{1}</b>",
 }
 l_transfer_transfer = {
@@ -3185,20 +2842,20 @@
     'en': "👩🏽‍💻 <b>Cleanup</b> completed\n<b>Current</b> number of users in the database: <u>{0}</u> (-{1})",
     'es': "👩🏽‍💻 <b>Limpieza</b> completada\nNúmero <b>actual</b> de usuarios en la base de datos: <u>{0}</u> (-{1})",
     'fr': "👩🏽‍💻 <b>Nettoyage</b> terminé\nNombre <b>actuel</b> d&#x27;utilisateurs dans la base de données : <u>{0}</u> (-{1})",
     'zh': "👩🏽‍💻<b>清理</b>完成\n数据库中的<b>当前</b>用户数： <u>{0}</u> (-{1})",
     'ar': "👩🏽‍💻 اكتمل <b>التنظيف</b>\nالعدد <b>الحالي</b> للمستخدمين في قاعدة البيانات: <u>{0}</u> (- {1})",
 }
 l_chn_ccheck_handler = {
-    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> по сгенерированной ссылке: {0} (только для ЧАСТНЫХ каналов)\n\n👩🏽‍💻 Для <b>проверки подписки</b> на другой канал <i>добавь</i> @{1}-бота в канал и выполни команду: /channel {2}\n\n👩🏽‍💻 Для <i>защиты от атаки</i> на канал включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
-    'en': "👮🏽 <b>Click</b> on ✅/🔘 to <b>switch</b> user <i>verification</i> type when <u>joining</u> via generated link: {0} (only for ЧАСТНЫХ channels)\n\n👩🏽‍💻 To <b>check subscription</b> to another channel, <i>add</i> @{1}-bot to the channel and run the command: /channel {2}\n\n👩🏽‍💻 To <i>protect against an attack</i> on the channel, turn on <b>the anti-raid</b> mode (block <u>all</u> intruders)",
-    'es': "👮🏽 <b>Haz clic</b> en ✅/🔘 para <b>cambiar</b> el tipo <i>de verificación</i> de usuario al <u>unirse</u> a través del enlace generado: {0} (solo para canales ЧАСТНЫХ )\n\n👩🏽‍💻 Para <b>verificar la suscripción</b> a otro canal, <i>agrega</i> @{1}-bot al canal y ejecuta el comando: /channel {2}\n\n👩🏽‍💻 Para <i>protegerte contra un ataque</i> en el canal, activa <b>el modo anti-raid</b> (bloquea <u>a todos</u> los intrusos)",
-    'fr': "👮🏽 <b>Cliquez</b> sur ✅/🔘 pour <b>changer</b> le type <i>de vérification</i> de l&#x27;utilisateur lors <u>de la connexion</u> via un lien généré : {0} (uniquement pour les canaux ЧАСТНЫХ )\n\n👩🏽‍💻 Pour <b>vérifier l&#x27;abonnement</b> à un autre canal, <i>ajoutez</i> @{1}-bot au canal et lancez la commande : /channel {2}\n\n👩🏽‍💻 Pour <i>vous protéger contre une attaque</i> sur le channel, activez <b>le mode anti-raid</b> (bloquer <u>tous</u> les intrus)",
-    'zh': "👮🏽<b>点击</b>✅/🔘 在通过生成的链接<u>加入</u>时<b>切换</b>用户<i>验证</i>类型：{0}（仅适用于ЧАСТНЫХ频道）\n\n👩🏽‍💻 要<b>检查对另一个频道的订阅</b>，请将 @{1}-bot<i>添加</i>到频道并运行命令： /channel {2}\n\n👩🏽‍💻 为<i>防止通道受到攻击</i>，请开启<b>防突袭</b>模式（阻止<u>所有</u>入侵者）",
-    'ar': "👮🏽 <b>انقر</b> على ✅ / 🔘 <b>لتبديل</b> نوع <i>التحقق</i> من المستخدم عند <u>الانضمام</u> عبر الرابط الذي تم إنشاؤه: {0} (للقنوات ЧАСТНЫХ فقط)\n\n👩🏽‍💻 للتحقق <b>من الاشتراك</b> في قناة أخرى ، <i>أضف</i> @ {1} -bot إلى القناة وقم بتشغيل الأمر: /channel {2}\n\n👩🏽‍💻 <i>للحماية من هجوم</i> على القناة ، قم بتشغيل الوضع <b>المضاد للغارة</b> (حظر <u>جميع</u> المتسللين)",
+    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> по сгенерированной ссылке: {0} (только для ЧАСТНЫХ каналов)\n\n👉🏼 Для <b>проверки подписки</b> на другой канал <i>добавь</i> @{1}-бота в канал и выполни команду: /channel {2}\n\n👉🏼 Для <i>защиты от атаки</i> на канал включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
+    'en': "👮🏽 <b>Click</b> on ✅/🔘 to <b>switch</b> user <i>verification</i> type when <u>joining</u> via generated link: {0} (only for ЧАСТНЫХ channels)\n\n👉🏼 To <b>check subscription</b> to another channel, <i>add</i> @{1}-bot to the channel and run the command: /channel {2}\n\n👉🏼 To <i>protect against an attack</i> on the channel, turn on <b>the anti-raid</b> mode (block <u>all</u> intruders)",
+    'es': "👮🏽 <b>Haz clic</b> en ✅/🔘 para <b>cambiar</b> el tipo <i>de verificación</i> de usuario al <u>unirse</u> a través del enlace generado: {0} (solo para canales ЧАСТНЫХ )\n\n👉🏼 Para <b>verificar la suscripción</b> a otro canal, <i>agrega</i> @{1}-bot al canal y ejecuta el comando: /channel {2}\n\n👉🏼 Para <i>protegerte contra un ataque</i> en el canal, activa <b>el modo anti-raid</b> (bloquea <u>a todos</u> los intrusos)",
+    'fr': "👮🏽 <b>Cliquez</b> sur ✅/🔘 pour <b>changer</b> le type <i>de vérification</i> de l&#x27;utilisateur lors <u>de la connexion</u> via un lien généré : {0} (uniquement pour les canaux ЧАСТНЫХ )\n\n👉🏼 Pour <b>vérifier l&#x27;abonnement</b> à un autre canal, <i>ajoutez</i> @{1}-bot au canal et lancez la commande : /channel {2}\n\n👉🏼 Pour <i>vous protéger contre une attaque</i> sur le channel, activez <b>le mode anti-raid</b> (bloquer <u>tous</u> les intrus)",
+    'zh': "👮🏽<b>点击</b>✅/🔘 在通过生成的链接<u>加入</u>时<b>切换</b>用户<i>验证</i>类型：{0}（仅适用于ЧАСТНЫХ频道）\n\n👉🏼 要<b>检查对另一个频道的订阅</b>，请将 @{1}-bot<i>添加</i>到频道并运行命令： /channel {2}\n\n👉🏼 为<i>防止通道受到攻击</i>，请开启<b>防突袭</b>模式（阻止<u>所有</u>入侵者）",
+    'ar': "👮🏽 <b>انقر</b> على ✅ / 🔘 <b>لتبديل</b> نوع <i>التحقق</i> من المستخدم عند <u>الانضمام</u> عبر الرابط الذي تم إنشاؤه: {0} (للقنوات ЧАСТНЫХ فقط)\n\n👉🏼 للتحقق <b>من الاشتراك</b> في قناة أخرى ، <i>أضف</i> @ {1} -bot إلى القناة وقم بتشغيل الأمر: /channel {2}\n\n👉🏼 <i>للحماية من هجوم</i> على القناة ، قم بتشغيل الوضع <b>المضاد للغارة</b> (حظر <u>جميع</u> المتسللين)",
 }
 l_ccheck_call = {
     'ru': "👮🏽 Для проверки подписки необходимо добавить дополнительный канал командой:\n\n/channel ССЫЛКА НА КАНАЛ",
     'en': "👮🏽 To check the subscription, you need to add an additional channel with the command:\n\n/channel LINK TO THE CHANNEL",
     'es': "👮🏽 Para verificar la suscripción, debe agregar un canal adicional con el comando:\n\n/canal ENLACE AL CANAL",
     'fr': "👮🏽 Pour vérifier l'abonnement, vous devez ajouter une chaîne supplémentaire avec la commande :\n\n/channel LIEN VERS LA CHAÎNE",
     'zh': "👮🏽 要检查订阅，您需要使用以下命令添加一个额外的频道：\n\n/channel LINK TO THE CHANNEL",
@@ -3333,47 +2990,47 @@
     'ar': "🔘️☐ Off مكافحة الغارة",
 }
 # endregion
 
 
 # region cban_
 l_cban_add = {
-    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей через <i>пробельные или разделительные</i> символы, чтобы добавить их в /ban-список (*даже тех, кто еще не запускал бота)\n\n👩🏽‍💻 <code>/ban 0</code> - очистить /ban-список",
+    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей  через <i>пробельные или разделительные</i> символы, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
     'en': "🕵🏽 <b>Enter</b> user id or @username separated by spaces or separators to add them to the /ban list (*even those not in the <u>{0}</u> file)\n\n👩🏽‍💻 <b>Current</b> number of users on the /ban list : <u>{1}</u>",
     'es': "🕵🏽 <b>Ingrese</b> id de usuario o @username usuario separados por espacios o separadores para agregarlos a la lista de /ban (*incluso aquellos que no están en el archivo <u>{0}</u> )\n\n👩🏽‍💻 Número <b>actual</b> de usuarios en la lista de /ban : <u>{1}</u>",
     'fr': "🕵🏽 <b>Entrez</b> id ou @username d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les ajouter à la liste /ban (*même ceux qui ne figurent pas dans le fichier <u>{0}</u> )\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs sur la liste /ban : <u>{1}</u>",
     'zh': "🕵🏽<b>输入</b>用空格或分隔符分隔的用户id或@username ，将他们添加到 /ban 列表（*即使那些不在<u>{0}</u>文件中的）\n\n👩🏽‍💻 /ban 列表中的<b>当前</b>用户数： <u>{1}</u>",
     'ar': "🕵🏽 <b>أدخل</b> id المستخدم أو @username مفصولة بمسافات أو فواصل لإضافتهما إلى / قائمة الحظر (* حتى أولئك غير الموجودين في <u>{0}</u> الملف)\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين في / قائمة الحظر : <u>{1}</u>",
 }
 l_cban_remove = {
-    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей через <i>пробельные или разделительные</i> символы, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 <code>/ban 0</code> - очистить /ban-список",
+    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей из <u>{0}</u>-файла через <i>пробельные или разделительные</i> символы, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
     'en': "🕵🏽 <b>Enter</b> id or @username of users from <u>{0}</u> -file separated by spaces or separators to remove them from /ban-list\n\n👩🏽‍💻 <b>Current</b> number of users /ban-list: <u>{1}</u>",
     'es': "🕵🏽 <b>Ingrese</b> id o @username de los usuarios de <u>{0}</u> -archivo separado por espacios o separadores para eliminarlos de /ban-list\n\n👩🏽‍💻 Número <b>actual</b> de usuarios /ban-list: <u>{1}</u>",
     'fr': "🕵🏽 <b>Entrez</b> id ou @username utilisateur des utilisateurs de <u>{0}</u> -fichier séparés par des espaces ou des séparateurs pour les supprimer de /ban-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs /ban-list : <u>{1}</u>",
     'zh': "🕵🏽<b>输入</b><u>{0}</u>文件中用户的id或@username ，以空格或分隔符分隔，以将其从 /ban-list 中删除\n\n👩🏽‍💻<b>当前</b>用户数 /ban-list： <u>{1}</u>",
     'ar': "🕵🏽 <b>أدخل</b> id أو @username للمستخدمين من <u>{0}</u> - ملف مفصول بمسافات أو فواصل لإزالتهم من / ban-list\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين / قائمة الحظر: <u>{1}</u>",
 }
 l_cban_added = {
-    'ru': "🕵🏽 <b>Пользователь</b> {0} добавлен в /ban-список (причина: <i>{1}</i>)",
+    'ru': "🕵🏽 Пользователь {0} добавлен в /ban-список (причина: <i>{1}</i>)",
     'en': "🕵🏽 User {0} added to /ban list (reason: <i>{1}</i> )",
     'es': "🕵🏽 Usuario {0} agregado a /lista de prohibición (razón: <i>{1}</i> )",
     'fr': "🕵🏽 L'utilisateur {0} a été ajouté à la liste /ban (raison : <i>{1}</i> )",
     'zh': "🕵🏽 用户 {0} 添加到 /ban 列表（原因： <i>{1}</i> ）",
     'ar': "🕵🏽 تمت إضافة المستخدم {0} إلى / قائمة الحظر (السبب: <i>{1}</i> )",
 }
 l_cban_text = {
-    'ru': "🕵🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> бан <u>пользователей</u> бота: <i>с недавно зарегистрированными new-id/аккаунтов без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban [id|@username] - блок пользователя\n/unban [id|@username] - разблок\n/parse - вывести всех пользователей",
+    'ru': "🕵🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> бан <u>пользователей</u> бота: <i>с недавно зарегистрированными new-id/аккаунтов без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей",
     'en': "🕵🏽 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> ban of bot <u>users</u> : <i>with newly registered new-id/accounts without</i> <i>@username</i> <i>/accounts from</i> <i>Anti-Spam System</i> <i>/accounts with 文-glyph, ب-arab/</i> <i>zalgo-characters</i>\n\ n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/ban - block/unblock user\n/parse - list all users",
     'es': "🕵🏽 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> la prohibición de <u>usuarios</u> de bots: <i>con nueva identificación recién registrada/cuentas sin</i> <i>@username</i> <i>/cuentas del</i> <i>sistema antispam</i> <i>/cuentas con 文-glyph, ب-arab/</i> <i>zalgo-characters</i>\n\ n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/ban - bloquear/desbloquear usuario\n/parse - enumerar todos los usuarios",
     'fr': "🕵🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> l&#x27;interdiction des <u>utilisateurs</u> de bot : <i>avec un nouvel identifiant nouvellement enregistré/des comptes sans</i> <i>@username</i> <i>/des comptes du</i> <i>système anti-spam</i> <i>/des comptes avec</i> <i>les caractères 文-glyph, ب-arab/ zalgo-characters</i>\n\ n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/ban - bloquer/débloquer l'utilisateur\n/parse - lister tous les utilisateurs",
     'zh': "🕵🏽<b>点击</b>✅/☑️ 以<b>启用/禁用</b>机器人<u>用户</u>的禁令：<i>新注册的新 ID/帐户没有@username</i> <i>/来自反垃圾邮件系统的</i>帐户<i>/带有文字形、Ø-arab/</i> <i>zalgo-characters 的</i>帐户\n\ n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/ban - 阻止/取消阻止用户\n/parse - 列出所有用户",
     'ar': "🕵🏽 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> حظر <u>مستخدمي</u> الروبوت: <i>مع معرف / حسابات جديدة مسجلة حديثًا بدون</i> <i>@username</i> <i>/ حسابات من</i> <i>نظام مكافحة البريد العشوائي</i> <i>/ الحسابات ذات الأحرف 文 -glyph و b- arab /</i> <i>zalgo-character</i>\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - كافة الأوامر\n/ حظر - حظر / إلغاء حظر المستخدم\n/ تحليل - سرد كافة المستخدمين",
 }
 l_cban_done = {
-    'ru': "🕵🏽 <b>Готово!</b> /ban-список нежелательных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/ban [id|@username] - блок пользователя\n/unban [id|@username] - разблок\n<code>/ban 0</code> - очистить /ban-список\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Готово!</b> /ban-список нежелательных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
     'en': "🕵🏽 <b>Done!</b> /ban-list of unwanted users of @{0}-bot\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/ban - block/unblock user\n/parse - list all users\n\n👩🏽‍💻 <b>Current</b> number of users/ban-list: <u>{1}</u>",
     'es': "🕵🏽 <b>Listo!</b> /lista de prohibición de usuarios no deseados de @{0}-bot\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/prohibición - bloquear/desbloquear usuario\n/parse - enumerar todos los usuarios\n\n👩🏽‍💻 Número <b>actual</b> de usuarios/lista de prohibición: <u>{1}</u>",
     'fr': "🕵🏽 <b>C&#x27;est fait !</b> /ban-list des utilisateurs indésirables de @{0}-bot\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/ban - bloquer/débloquer l&#x27;utilisateur\n/parse - lister tous les utilisateurs\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs/ban-list : <u>{1}</u>",
     'zh': "🕵🏽<b>完成！</b> /ban-list of unblock users of @{0}-bot\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/ban - 阻止/取消阻止用户\n/parse - 列出所有用户\n\n👩🏽‍💻<b>当前</b>用户数/黑名单： <u>{1}</u>",
     'ar': "🕵🏽 <b>انتهى!</b> / ban-list of غير المرغوب فيهم لـ @ {0} -bot\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ الحظر - حظر / إلغاء حظر المستخدم\n/ parse - سرد كافة المستخدمين\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين / قائمة الحظر: <u>{1}</u>",
 }
 l_cban_correct = {
@@ -3382,20 +3039,20 @@
     'es': "🕵🏽 <b>Ingrese</b> una identificación de usuario válida o @username o prohíba a todos los usuarios: /ban",
     'fr': "🕵🏽 <b>Entrez</b> un identifiant ou @username d'utilisateur valide ou bannissez tous les utilisateurs : /ban",
     'zh': "🕵🏽<b>输入</b>有效的用户 ID 或@username或禁止所有用户：/ban",
     'ar': "🕵🏽 <b>أدخل</b> معرف مستخدم صالحًا أو @username أو احظر جميع المستخدمين: / ban",
 }
 
 l_cban_handler = {
-    'ru': "🕵🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>аккаунтов с недавно зарегистрированными new-id/без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👩🏽‍💻 Например, опция <b>new-id</b> блокирует аккаунты со <i>свежим</i> <u>id</u>",
-    'en': "🕵🏽 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <u>auto</u> -ban <i>of accounts with newly registered new-id/without</i> <i>@username</i> <i>/accounts from</i> <i>the Anti-Spam System</i> <i>/accounts with 文-glyph, ب-arab/</i> <i>zalgo-characters</i>\n\ n👩🏽‍💻 For example, the <b>new-id</b> option blocks accounts with <i>a fresh</i> <u>id</u>",
-    'es': "🕵🏽 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> la prohibición <u>automática</u> <i>de cuentas con nueva identificación recién registrada/sin</i> <i>@username</i> <i>/cuentas del</i> <i>sistema antispam</i> <i>/cuentas con 文-glyph, ب-arab/</i> <i>zalgo-characters</i>\n\ n👩🏽‍💻 Por ejemplo, la opción <b>new-id</b> bloquea cuentas con <i>una nueva</i> <u>identificación</u>",
-    'fr': "🕵🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> l&#x27;interdiction <u>automatique</u> <i>des comptes avec un nouvel identifiant nouvellement enregistré/sans</i> <i>@username</i> <i>/comptes du</i> <i>système anti-spam</i> <i>/comptes avec 文-glyphe, ب-arabe/</i> <i>zalgo-caractères</i>\n\ n👩🏽‍💻 Par exemple, l&#x27;option <b>new-id</b> bloque les comptes avec <i>un nouvel</i> <u>identifiant</u>",
-    'zh': "🕵🏽<b>单击</b>✅/☑️<b>启用/禁用</b><u>自动</u>禁止<i>具有新注册的 new-id/不带@username</i>的帐户<i>/来自反垃圾邮件系统的帐户/具有 text-glyph、ب-arab/</i> <i>zalgo-characters</i>\n的帐户\n👩🏽‍💻 例如<b>new-id</b>选项屏蔽<i>新</i><u>id</u>的账号",
-    'ar': "🕵🏽 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> الحظر <u>التلقائي</u> <i>للحسابات ذات المعرف الجديد المسجل حديثًا / بدون</i> <i>@username</i> <i>/ الحسابات من</i> <i>نظام مكافحة البريد العشوائي</i> <i>/ الحسابات ذات</i> <i>الأحرف 文 -glyph و b- arab / zalgo-character</i>\n\n👩🏽‍💻 على سبيل المثال ، يقوم خيار <b>المعرف الجديد</b> بحظر الحسابات ذات <u>المعرف</u> <i>الجديد</i>",
+    'ru': "🕵🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>аккаунтов с недавно зарегистрированными new-id/без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>new-id</b> блокирует аккаунты со <i>свежим</i> <u>id</u>",
+    'en': "🕵🏽 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <u>auto</u> -ban <i>of accounts with newly registered new-id/without</i> <i>@username</i> <i>/accounts from</i> <i>the Anti-Spam System</i> <i>/accounts with 文-glyph, ب-arab/</i> <i>zalgo-characters</i>\n\ n👉🏼 For example, the <b>new-id</b> option blocks accounts with <i>a fresh</i> <u>id</u>",
+    'es': "🕵🏽 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> la prohibición <u>automática</u> <i>de cuentas con nueva identificación recién registrada/sin</i> <i>@username</i> <i>/cuentas del</i> <i>sistema antispam</i> <i>/cuentas con 文-glyph, ب-arab/</i> <i>zalgo-characters</i>\n\ n👉🏼 Por ejemplo, la opción <b>new-id</b> bloquea cuentas con <i>una nueva</i> <u>identificación</u>",
+    'fr': "🕵🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> l&#x27;interdiction <u>automatique</u> <i>des comptes avec un nouvel identifiant nouvellement enregistré/sans</i> <i>@username</i> <i>/comptes du</i> <i>système anti-spam</i> <i>/comptes avec 文-glyphe, ب-arabe/</i> <i>zalgo-caractères</i>\n\ n👉🏼 Par exemple, l&#x27;option <b>new-id</b> bloque les comptes avec <i>un nouvel</i> <u>identifiant</u>",
+    'zh': "🕵🏽<b>单击</b>✅/☑️<b>启用/禁用</b><u>自动</u>禁止<i>具有新注册的 new-id/不带@username</i>的帐户<i>/来自反垃圾邮件系统的帐户/具有 text-glyph、ب-arab/</i> <i>zalgo-characters</i>\n的帐户\n👉🏼 例如<b>new-id</b>选项屏蔽<i>新</i><u>id</u>的账号",
+    'ar': "🕵🏽 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> الحظر <u>التلقائي</u> <i>للحسابات ذات المعرف الجديد المسجل حديثًا / بدون</i> <i>@username</i> <i>/ الحسابات من</i> <i>نظام مكافحة البريد العشوائي</i> <i>/ الحسابات ذات</i> <i>الأحرف 文 -glyph و b- arab / zalgo-character</i>\n\n👉🏼 على سبيل المثال ، يقوم خيار <b>المعرف الجديد</b> بحظر الحسابات ذات <u>المعرف</u> <i>الجديد</i>",
 }
 l_cban_new_on = {
     'ru': "✅☑Вкл new-id-бан",
     'en': "✅☑Includes new-id-ban",
     'es': "✅☑Incluye nuevo-id-ban",
     'fr': "✅☑Comprend une nouvelle interdiction d'identité",
     'zh': "✅☑包括新身份禁令",
@@ -3482,20 +3139,20 @@
     'en': "🔔 You need to ⚙️Customize at least one post",
     'es': "🔔 Necesitas ⚙️Personalizar al menos una publicación",
     'fr': "🔔 Vous devez ⚙️Personnaliser au moins une publication",
     'zh': "🔔 你需要⚙️自定义至少一个帖子",
     'ar': "🔔 أنت بحاجة إلى تخصيص منشور واحد على الأقل",
 }
 l_cpost_text = {
-    'ru': "🔔 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <b>авто</b>-постинг по дате\n\n👩🏽‍💻 <b>Текущее</b> количество постов <u>{0}</u>",
-    'en': "🔔 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> <b>auto</b> -posting by date\n\n👩🏽‍💻 <b>Current</b> number of posts <u>{0}</u>",
-    'es': "🔔 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> la publicación <b>automática</b> por fecha\n\n👩🏽‍💻 Número <b>actual</b> de publicaciones <u>{0}</u>",
-    'fr': "🔔 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> la publication <b>automatique</b> par date\n\n👩🏽‍💻 Nombre <b>actuel</b> de publications <u>{0}</u>",
+    'ru': "🔔 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <b>авто</b>-постинг по дате\n\n👉🏼 <b>Текущее</b> количество постов <u>{0}</u>",
+    'en': "🔔 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> <b>auto</b> -posting by date\n\n👉🏼 <b>Current</b> number of posts <u>{0}</u>",
+    'es': "🔔 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> la publicación <b>automática</b> por fecha\n\n👉🏼 Número <b>actual</b> de publicaciones <u>{0}</u>",
+    'fr': "🔔 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> la publication <b>automatique</b> par date\n\n👉🏼 Nombre <b>actuel</b> de publications <u>{0}</u>",
     'zh': "🔔<b>单击</b>✅/☑️ 以<b>打开/关闭</b>按日期<b>自动</b>发布\n\n👉🏼<b>当前</b>的帖子数<u>{0}</u>",
-    'ar': "🔔 <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> النشر <b>التلقائي</b> حسب التاريخ\n\n👩🏽‍💻 العدد <b>الحالي</b> من المشاركات <u>{0}</u>",
+    'ar': "🔔 <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> النشر <b>التلقائي</b> حسب التاريخ\n\n👉🏼 العدد <b>الحالي</b> من المشاركات <u>{0}</u>",
 }
 l_fsm_post_call = {
     'ru': "🔔 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Отправка сообщений]\n[✅ Редактирование постов]\n\n🕚Подожди 1min",
     'en': "🔔 In the [Administrators] settings, enable the option for @{0}-bot:\n[✅ Send messages]\n[✅ Edit posts]\n\n🕚Wait 1min",
     'es': "🔔 En la configuración de [Administradores], habilita la opción para @{0}-bot:\n[✅ Enviar mensajes]\n[✅ Editar publicaciones]\n\n🕚Espera 1 minuto",
     'fr': "🔔 Dans les paramètres [Administrateurs], activez l'option pour @{0}-bot :\n[✅ Envoyer des messages]\n[✅ Modifier les messages]\n\n🕚Attendez 1 min",
     'zh': "🔔 在 [Administrators] 设置中，启用 @{0}-bot 的选项：\n[✅ 发送消息]\n[✅ 编辑帖子]\n\n🕚等待 1 分钟",
@@ -3598,20 +3255,20 @@
     'ar': "👁️‍🗨️ / عرض-طرق العرض التلقائي معطلة",
 }
 # endregion
 
 
 # region cdecor_
 l_cdecor_text = {
-    'ru': "🪄 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-декор публикуемого поста: <i><b>пагинация</b> (порядковый номер поста)/креативный <b>формат текста</b> (<b>жирный</b>/<i>курсив</i>/<u>подчеркнутый</u>/моно/<tg-spoiler>спойлер</tg-spoiler>/#хэштег/<a href='{0}'>ссылка</a>)/<b>футер</b> (текстовое окончание поста)</i>\n\n👩🏽‍💻 Например, опция <b>[✅☑Вкл формат текста]</b> означает креативное изменение поста с использованием 7 стилей",
-    'en': "🪄 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the auto-decor of the published post: <i><b>pagination</b> (post serial number)/creative <b>text format</b> ( <b>bold</b> /italic/ <u>underlined</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/link)/ <b>footer</b> (post text ending)</i>\n\n👩🏽‍💻 For example, the option <b>[✅☑Enable Text Format]</b> means creative post editing using 7 styles",
-    'es': "🪄 <b>Haga clic</b> en ✅/☑️ para <b>activar/desactivar</b> la decoración automática de la publicación: <i><b>paginación</b> (número de serie de la publicación)/ <b>formato de texto</b> creativo ( <b>negrita</b> /cursiva/ <u>subrayado</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/enlace)/ <b>pie de página</b> (publicación final del texto)</i>\n\n👩🏽‍💻 Por ejemplo, la opción <b>[✅☑Habilitar formato de texto]</b> significa edición creativa de publicaciones usando 7 estilos",
-    'fr': "🪄 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> le décor automatique de l&#x27;article publié : <i><b>pagination</b> (numéro de série de l&#x27;article)/ <b>format du texte</b> créatif ( <b>gras</b> /italique/ <u>souligné</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/lien)/ <b>pied de page</b> (article fin du texte)</i>\n\n👩🏽‍💻 Par exemple, l&#x27;option <b>[✅☑Activer le format de texte]</b> signifie une post-édition créative utilisant 7 styles",
-    'zh': "🪄<b>点击</b>✅/☑️<b>开启/关闭</b>已发布帖子的自动装饰：<i><b>分页</b>（帖子序列号）/创意<b>文本格式</b>（<b>粗体</b>/斜体/<u>下划线</u>/</i> моно <i>/剧透/</i> <i>#хэштег</i> <i>/link）/<b>页脚</b>（帖子text ending)</i>\n\n👩🏽‍💻 例如选项<b>[✅☑Enable Text Format]</b>表示使用 7 种样式进行创意后期编辑",
-    'ar': "🪄 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف</b> الديكور التلقائي للمنشور المنشور: <i><b>ترقيم الصفحات</b> (الرقم التسلسلي للرسالة) / <b>تنسيق النص</b> الإبداعي ( <b>غامق</b> / مائل / <u>تحته خط</u> /</i> моно <i>/ سبويلر /</i> <i>#хэштег</i> <i>/ رابط) / تذييل ( <b>منشور</b> ) نهاية النص)</i>\n\n👩🏽‍💻 على سبيل المثال ، الخيار <b>[✅☑ تمكين تنسيق النص]</b> يعني تحرير المنشور الإبداعي باستخدام 7 أنماط",
+    'ru': "🪄 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-декор публикуемого поста: <i><b>пагинация</b> (порядковый номер поста)/креативный <b>формат текста</b> (<b>жирный</b>/<i>курсив</i>/<u>подчеркнутый</u>/моно/<tg-spoiler>спойлер</tg-spoiler>/#хэштег/<a href='{0}'>ссылка</a>)/<b>футер</b> (текстовое окончание поста)</i>\n\n👉🏼 Например, опция <b>[✅☑Вкл формат текста]</b> означает креативное изменение поста с использованием 7 стилей",
+    'en': "🪄 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the auto-decor of the published post: <i><b>pagination</b> (post serial number)/creative <b>text format</b> ( <b>bold</b> /italic/ <u>underlined</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/link)/ <b>footer</b> (post text ending)</i>\n\n👉🏼 For example, the option <b>[✅☑Enable Text Format]</b> means creative post editing using 7 styles",
+    'es': "🪄 <b>Haga clic</b> en ✅/☑️ para <b>activar/desactivar</b> la decoración automática de la publicación: <i><b>paginación</b> (número de serie de la publicación)/ <b>formato de texto</b> creativo ( <b>negrita</b> /cursiva/ <u>subrayado</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/enlace)/ <b>pie de página</b> (publicación final del texto)</i>\n\n👉🏼 Por ejemplo, la opción <b>[✅☑Habilitar formato de texto]</b> significa edición creativa de publicaciones usando 7 estilos",
+    'fr': "🪄 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> le décor automatique de l&#x27;article publié : <i><b>pagination</b> (numéro de série de l&#x27;article)/ <b>format du texte</b> créatif ( <b>gras</b> /italique/ <u>souligné</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/lien)/ <b>pied de page</b> (article fin du texte)</i>\n\n👉🏼 Par exemple, l&#x27;option <b>[✅☑Activer le format de texte]</b> signifie une post-édition créative utilisant 7 styles",
+    'zh': "🪄<b>点击</b>✅/☑️<b>开启/关闭</b>已发布帖子的自动装饰：<i><b>分页</b>（帖子序列号）/创意<b>文本格式</b>（<b>粗体</b>/斜体/<u>下划线</u>/</i> моно <i>/剧透/</i> <i>#хэштег</i> <i>/link）/<b>页脚</b>（帖子text ending)</i>\n\n👉🏼 例如选项<b>[✅☑Enable Text Format]</b>表示使用 7 种样式进行创意后期编辑",
+    'ar': "🪄 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف</b> الديكور التلقائي للمنشور المنشور: <i><b>ترقيم الصفحات</b> (الرقم التسلسلي للرسالة) / <b>تنسيق النص</b> الإبداعي ( <b>غامق</b> / مائل / <u>تحته خط</u> /</i> моно <i>/ سبويلر /</i> <i>#хэштег</i> <i>/ رابط) / تذييل ( <b>منشور</b> ) نهاية النص)</i>\n\n👉🏼 على سبيل المثال ، الخيار <b>[✅☑ تمكين تنسيق النص]</b> يعني تحرير المنشور الإبداعي باستخدام 7 أنماط",
 }
 l_cdecor_footer_call = {
     'ru': "🪄 Футер пустой, необходимо его ⚙️Настроить",
     'en': "🪄 The footer is empty, you need to set it up ⚙️",
     'es': "🪄 El pie de página está vacío, debes configurarlo ⚙️",
     'fr': "🪄 Le pied de page est vide, vous devez le paramétrer ⚙️",
     'zh': "🪄 footer 是空的，需要设置一下⚙️",
@@ -3751,23 +3408,23 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_group_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> модерации <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b>\n▪️<b>организация</b> бана и антифлуда\n▪️<b>авто-ответы</b> и стоп-слова\n▪️<b>кнопочный</b> счетчик\n\n❗️Регулярно-обновляемый /content",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> администрирования <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b>\n▪️<b>организация</b> бана и антифлуда\n▪️<b>авто-ответы</b> и стоп-слова\n▪️<b>кнопочный</b> счетчик\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> администрирования <b>Telegram</b> groups:\n\n▪️ <b>protecting</b> the group from spyware\n▪️displaying <b>statistics</b> and engagement (%)\n▪️restricting rights before <b>subscribing</b> to the channel\n▪️ <b>organizing</b> a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> администрирования grupos <b>de Telegram</b> :\n\ <b>n▪️proteger</b> al grupo de spyware\n▪️mostrar <b>estadísticas</b> e interacción (%)\n▪️restringir los derechos antes de <b>suscribirse</b> al canal\ <b>n▪️organizar</b> un prohibición y anti-inundación\n\n❗️también puede solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> администрирования des groupes <b>Telegram</b> :\n\n▪️ <b>protéger</b> le groupe des spywares\n▪️afficher <b>les statistiques</b> et l&#x27;engagement (%)\n▪️restreindre les droits avant de <b>s&#x27;abonner</b> à la chaîne\n▪️ <b>organiser</b> un interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
     'zh': "🌱 {0}，欢迎使用администрирования <b>Telegram</b>群组的<i>登陆机器人</i>：\n\n▪️<b>保护</b>群组免受间谍软件的侵害\n▪️ 显示<b>统计数据</b>和参与度 (%)\n▪️ 在<b>订阅</b>频道之前限制权利\n▪️<b>组织</b>一个ban 和 anti-flood\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> администрирования مجموعات <b>Telegram</b> :\n\n▪️ <b>حماية</b> المجموعة من برامج التجسس\n▪️ عرض <b>الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> الحظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_group = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️до 50 <b>стоп-слов</b>\n▪️до 10 <b>старт-слов</b>\n▪️до 5 <b>авто-приглашений</b>\n\n👩🏽‍💻 /balance",
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️до 50 <b>стоп-слов</b>\n▪️до 10 <b>старт-слова</b>\n▪️до 5 <b>авто-приглашений</b>\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
@@ -3953,15 +3610,15 @@
     'ar': "👮🏽 <i>للتحقق من الاشتراك ،</i> تحتاج إلى إضافة قناة باستخدام الأمر:\n\n/ channel LINK TO THE CHANNEL",
 }
 # endregion
 
 
 # region commands
 l_group_commands_handler = {
-    'ru': "⚙️ <b>Настройки</b> группы [<b>{0}</b>] {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/parse  <i>[all|old|premium|active|online]</i>\n/transfer [id]   <i>передача прав</i>\n\n<b>⛏ Команды администраторов</b>\n/ban 5m|1h|10d <i>удаление на время</i>\n/unban\n/mute 5m|1h|10d <i>ограничение на время</i>\n/unmute\n/warn+сообщ <i>предупреждение</i>\n/status\n/karma  [+|-]\n/tag+сообщ   <i>@tager random-аккаунтов</i>\n/stop  <i>добавить стоп-слово</i>\n/channel NAME   <i>добавить канал для проверки подписки</i>\n/button NAME    <i>добавить имя кнопки входного контроля</i>\n/delay MIN      <i>установить количество min для задержки 1го сообщ</i>\n/flood NUM      <i>установить количество сообщ для flood</i>\n\n<b>⛏ Команды пользователей</b>\n/help   <i>вывод команд</i>\n/rules  <i>правила группы</i>\n/report <i>сообщить о нарушении</i>\n/happy  <i>получить радость</i>\n/thanks <i>поблагодарить</i>",
+    'ru': "⚙️ <b>Настройка</b> группы <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/log   <i>посмотреть логи</i>\n/parse  <i>[all|old|premium|active|online]</i>\n/parse old - <i>парсинг старых id-аккаунтов</i>\n\n<b>⛏ Команды администраторов</b>\n/ban 5m|1h|10d <i>удаление из группы на время</i>\n/unban\n/mute 5m|1h|10d <i>ограничение в группе на время</i>\n/unmute\n/warn+сообщ <i>предупреждение</i>\n/status\n/karma  [+|-]\n/tag+сообщ   <i>@tager random-аккаунтов</i>\n/stop  <i>добавить стоп-слово</i>\n/channel NAME   <i>добавить канал для проверки подписки</i>\n/button NAME    <i>добавить имя кнопки входного контроля</i>\n/delay MIN      <i>установить количество min для задержки 1го сообщ</i>\n/flood NUM      <i>установить количество сообщ для flood</i>\n\n<b>⛏ Команды пользователей</b>\n/help   <i>вывод команд</i>\n/rules  <i>правила группы</i>\n/report <i>сообщить о нарушении</i>\n/happy  <i>получить радость</i>\n/thanks <i>поблагодарить</i>",
     'en': "⚙️ Group <b>setting</b> <b>{0}</b> {1}\n\n<b>⛏ Admin commands @{2}</b>\n/update <i>update parameters</i>\n/transfer <i>transfer admin rights</i>\n/info <i>information</i>\n/stat <i>statistics</i>\n/log <i>view logs</i>\n/parse <i>[all|old|premium|active|online]</i>\n/parse old - <i>parse old account ids</i>\n\n<b>⛏ Commands for administrators</b>\n/ban 5m|1h|10d <i>temporary removal from the group</i>\n/unban\n/mute 5m|1h|10d <i>group time limit</i>\n/unmute\n/warn+mess <i>warning</i>\n/status\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>random- accounts</i>\n/stop <i>add a stopword</i>\n/channel NAME <i>add a channel for checking subscription</i>\n/button NAME <i>add a name for input control button</i>\n/delay MIN <i>set the min amount to delay 1 message</i>\n/flood NUM <i>set the number of messages for flood</i>\n\n<b>⛏ User commands</b>\n/help <i>command output</i>\n/rules <i>group rules</i>\n/report report <i>abuse</i>\n/happy <i>get joy</i>\n/thanks <i>thank</i>",
     'es': "⚙️ <b>Configuración</b> de grupo <b>{0}</b> {1}\n\n<b>⛏ Comandos de administrador @{2}</b>\n/actualizar <i>actualizar parámetros</i>\n/transferir <i>transferir derechos de administrador</i>\n/ <i>información</i> de información\n/ <i>estadísticas</i>\n/registrar <i>ver registros</i> \ n/parse <i>[todos|antiguos|premium|activos|en línea]</i>\n/parse old : <i>analiza los ID de cuentas antiguos</i>\n\n<b>⛏ Comandos para administradores</b>\n/ban 5m|1h|10d <i>eliminación temporal del grupo</i>\n/unban\n/silencio 5m|1h| <i>límite de tiempo de grupo</i> 10d\n/no silenciar\n/advertencia+mensaje <i>advertencia</i>\n/estado\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>cuentas aleatorias</i>\n/ detener <i>agregar una palabra vacía</i>\n/NOMBRE del canal <i>agregar un canal para verificar la suscripción</i>\n/NOMBRE del botón <i>agregar un nombre para el botón de control de entrada</i>\n/retardo MIN <i>establecer la cantidad mínima para retrasar 1 mensaje</i>\n/inundación NUM <i>establecer el número de mensajes para inundación</i>\n\n<b>⛏ Comandos de usuario</b>\n/ <i>salida de comando</i> de ayuda\n/ <i>reglas reglas de grupo</i>\n/informar informar <i>abuso</i>\n/feliz <i>obtener alegría</i>\n/gracias <i>gracias</i>",
     'fr': "⚙️ <b>Paramètres</b> de groupe <b>{0}</b> {1}\n\n<b>⛏ Commandes d&#x27;administration @{2}</b>\n/mettre à jour <i>les paramètres de mise à jour</i>\n/transférer <i>les droits d&#x27;administrateur de transfert</i>\n/ <i>informations d&#x27;information</i>\n/ <i>statistiques</i>\n/journal <i>afficher les journaux</i> \ n/parse <i>[all|old|premium|active|online]</i>\n/parse old - <i>analyse les anciens identifiants de compte</i>\n\n<b>⛏ Commandes pour les administrateurs</b>\n/ban 5m|1h|10d <i>suppression temporaire du groupe</i>\n/unban\n/mute 5m|1h|10d <i>limite de temps de groupe</i>\n/unmute\n/warn+mess <i>warning</i>\n/status\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>random- accounts</i>\n/ stop <i>ajouter un mot vide</i>\n/channel NAME <i>ajouter un canal pour vérifier l&#x27;abonnement</i>\n/button NAME <i>ajouter un nom pour le bouton de contrôle d&#x27;entrée</i>\n/delay MIN <i>définir le montant minimum pour retarder 1 message</i>\n/flood NUM <i>définir le nombre de messages for flood</i>\n\n<b>⛏ Commandes utilisateur</b>\n/ <i>sortie de la commande d&#x27;</i> aide\n/ <i>rules règles du groupe</i>\n/signaler signaler un <i>abus</i>\n/happy <i>get joy</i>\n/merci <i>merci</i>",
     'zh': "⚙️ 群组<b>设置{0}</b> {1}\n\n<b>⛏ 管理员命令@{2}</b>\n/update<i>更新参数</i>\n/transfer<i>转移admin 权限</i>\n/info<i>信息</i>\n/stat<i>统计</i>\n/log<i>查看日志</i>\ n/parse <i>[all|old|premium|active|online]</i>\n/parse old -<i>解析旧帐户 ID</i>\n\n<b>⛏ 管理员命令</b>\n/ban 5m|1h|10d<i>临时从组中删除</i>\n/unban\n/mute 5m|1h|10d<i>群限时</i>\n/unmute\n/warn+mess<i>警告</i>\n/status\n/karma[+|-]\n/tag+mess <i>@tager</i> <i>random-accounts</i>\n/ stop<i>添加停用词</i>\n/channel NAME<i>添加检查订阅的频道</i>\n/button NAME<i>添加输入控制按钮的名称</i>\n/delay MIN<i>设置延迟 1 条消息的最小量</i>\n/flood NUM<i>设置消息数for flood</i>\n\n<b>⛏ 用户命令</b>\n/help<i>命令输出</i>\n/rules<i>组规则</i>\n/report 报告<i>滥用</i>\n/happy <i>get joy</i>\n/thanks <i>thank</i>",
     'ar': "⚙️ <b>إعداد</b> المجموعة <b>{0}</b> {1}\n\n<b>⛏ أوامر المسؤول @ {2}</b>\n/ <i>تحديث المعلمات</i>\n/ <i>نقل حقوق المسؤول</i>\n/ معلومات <i>المعلومات</i>\n/ <i>الإحصائيات</i> الإحصائية\n/ <i>سجلات عرض السجل</i>\n/ parse <i>[all | old | premium | active | online]</i>\n/parse old - <i>تحليل معرفات الحساب القديم</i>\n\n<b>⛏ أوامر للمسؤولين</b>\n/ ban 5m | 1h | 10d <i>إزالة مؤقتة من المجموعة</i>\n/ Unban\n/ mute 5m | 1h | 10d <i>وقت المجموعة</i>\n/ unmute\n/ warn + <i>تحذير</i> الفوضى\n/ status\n/ karma [+ | -]\n/ tag + <i>@tager</i> <i>random- حسابات</i>\n/ إيقاف <i>إضافة كلمة إيقاف</i>\n/ قناة NAME <i>إضافة قناة للتحقق من الاشتراك</i>\n/ زر NAME <i>إضافة اسم لزر التحكم في الإدخال</i>\n/ تأخير MIN <i>قم بتعيين الحد الأدنى للمبلغ لتأخير رسالة واحدة</i>\n/ إغراق NUM <i>قم بتعيين عدد الرسائل من أجل الفيضان</i>\n\n<b>⛏ أوامر المستخدم</b>\n/ <i>إخراج أمر</i> المساعدة\n/ <i>قواعد المجموعة</i>\n/ الإبلاغ عن <i>إساءة استخدام</i>\n/ سعيد <i>الحصول على الفرح</i>\n/ <i>شكرًا</i> جزيلاً",
 }
 l_update_handler00 = {
@@ -4267,23 +3924,23 @@
     'en': "👮🏽 <b>Done!</b> The current <b>button name</b> on <i>the input control</i> is set to: {0}",
     'es': "👮🏽 <b>Listo!</b> El <b>nombre del botón</b> actual en <i>el control de entrada</i> se establece en: {0}",
     'fr': "👮🏽 <b>C&#x27;est fait !</b> Le <b>nom actuel du bouton</b> sur <i>le contrôle d&#x27;entrée</i> est défini sur : {0}",
     'zh': "👮🏽<b>完成！</b><i>输入控件</i>上的当前<b>按钮名称</b>设置为：{0}",
     'ar': "👮🏽 <b>انتهى!</b> تم تعيين <b>اسم الزر</b> الحالي في <i>عنصر تحكم الإدخال</i> على: {0}",
 }
 l_button_correct = {
-    'ru': "👮🏽 <b>Введи</b> корректное название <i>для имени кнопки</i> Входного контроля\n\n👩🏽‍💻 Например, /button {0}",
-    'en': "👮🏽 <b>Please enter</b> a valid name <i>for the Input Control button name</i>\n\n👩🏽‍💻 For example, /button {0}",
-    'es': "👮🏽 <b>Ingrese</b> un nombre válido <i>para el nombre del botón de control de entrada</i>\n\n👩🏽‍💻 Por ejemplo, /button {0}",
-    'fr': "👮🏽 <b>Veuillez saisir</b> un nom valide <i>pour le nom du bouton de contrôle d&#x27;entrée</i>\n\n👩🏽‍💻 Par exemple, /button {0}",
-    'zh': "👮🏽 请<i>为输入控件按钮名称</i><b>输入</b>有效名称\n\n👩🏽‍💻 例如， /button {0}",
-    'ar': "👮🏽 <b>الرجاء إدخال</b> اسم صالح <i>لاسم زر التحكم في الإدخال</i>\n\n👩🏽‍💻 على سبيل المثال ، /button {0}",
+    'ru': "👮🏽 <b>Введи</b> корректное название <i>для имени кнопки</i> Входного контроля\n\n👉🏼 Например, /button {0}",
+    'en': "👮🏽 <b>Please enter</b> a valid name <i>for the Input Control button name</i>\n\n👉🏼 For example, /button {0}",
+    'es': "👮🏽 <b>Ingrese</b> un nombre válido <i>para el nombre del botón de control de entrada</i>\n\n👉🏼 Por ejemplo, /button {0}",
+    'fr': "👮🏽 <b>Veuillez saisir</b> un nom valide <i>pour le nom du bouton de contrôle d&#x27;entrée</i>\n\n👉🏼 Par exemple, /button {0}",
+    'zh': "👮🏽 请<i>为输入控件按钮名称</i><b>输入</b>有效名称\n\n👉🏼 例如， /button {0}",
+    'ar': "👮🏽 <b>الرجاء إدخال</b> اسم صالح <i>لاسم زر التحكم في الإدخال</i>\n\n👉🏼 على سبيل المثال ، /button {0}",
 }
 l_channel_check = {
-    'ru': "⚙️ <b>Добавь</b> @{0}-бота в канал для проверки подписки на него. Пришли мне корректную ссылку на канал:",
+    'ru': "⚙️ Добавь @{0}-бота в канал для проверки подписки на него. Пришли мне корректную ссылку на канал:",
     'en': "⚙️ Add @{0}-bot to the channel to check if you subscribe to it. Send me the correct link to the channel:",
     'es': "⚙️ Agrega @{0}-bot al canal para comprobar si estás suscrito. Envíame el enlace correcto al canal:",
     'fr': "⚙️ Ajoutez @{0}-bot à la chaîne pour vérifier si vous y êtes abonné. Envoyez-moi le bon lien vers la chaîne :",
     'zh': "⚙️ 将@{0}-bot 添加到频道以检查您是否订阅了它。向我发送正确的频道链接：",
     'ar': "⚙️ أضف @ {0} -bot إلى القناة للتحقق مما إذا كنت مشتركًا فيها. أرسل لي الرابط الصحيح للقناة:",
 }
 l_channel_done = {
@@ -4291,31 +3948,31 @@
     'en': "👮🏽 <b>Done!</b> Checking subscription to {0} is configured\n\nThe option can be enabled in the settings by pressing [✅☑Enable subscription]",
     'es': "👮🏽 <b>Listo!</b> Verificar que la suscripción a {0} está configurada\n\nLa opción se puede habilitar en la configuración presionando [✅☑Habilitar suscripción]",
     'fr': "👮🏽 <b>C&#x27;est fait !</b> Vérifier que l'abonnement à {0} est configuré\n\nL'option peut être activée dans les paramètres en appuyant sur [✅☑Activer l'abonnement]",
     'zh': "👮🏽<b>完成！</b>检查对 {0} 的订阅是否已配置\n\n可以通过按 [✅☑启用订阅] 在设置中启用该选项",
     'ar': "👮🏽 <b>انتهى!</b> التحقق من الاشتراك في {0} مهيأ\n\nيمكن تمكين الخيار في الإعدادات بالضغط على [✅☑ تمكين الاشتراك]",
 }
 l_channel_correct = {
-    'ru': "👮🏽 <b>Добавь</b> @{0}-бота в канал и отправь корректную <i>ссылку</i> этого канала\n\n👩🏽‍💻 Например, /channel @{1}",
-    'en': "👮🏽 Add @{0}-bot to the channel and send the correct <i>link</i> of this channel\n\n👩🏽‍💻 For example, /channel @{1}",
-    'es': "👮🏽 Agrega @{0}-bot al canal y envía el <i>enlace</i> correcto de este canal\n\n👩🏽‍💻 Por ejemplo, /channel @{1}",
-    'fr': "👮🏽 Ajoutez @{0}-bot au canal et envoyez le <i>lien</i> correct de ce canal\n\n👩🏽‍💻 Par exemple, /channel @{1}",
-    'zh': "👮🏽 将@{0}-bot 添加到频道并发送该频道的正确<i>链接</i>\n\n👩🏽‍💻 例如， /channel @{1}",
-    'ar': "👮🏽 Add @ {0} -bot إلى القناة وأرسل <i>الرابط</i> الصحيح لهذه القناة\n\n👩🏽‍💻 على سبيل المثال ، /channel @{1}",
+    'ru': "👮🏽 Добавь @{0}-бота в канал и отправь корректную <i>ссылку</i> этого канала\n\n👉🏼 Например, /channel @{1}",
+    'en': "👮🏽 Add @{0}-bot to the channel and send the correct <i>link</i> of this channel\n\n👉🏼 For example, /channel @{1}",
+    'es': "👮🏽 Agrega @{0}-bot al canal y envía el <i>enlace</i> correcto de este canal\n\n👉🏼 Por ejemplo, /channel @{1}",
+    'fr': "👮🏽 Ajoutez @{0}-bot au canal et envoyez le <i>lien</i> correct de ce canal\n\n👉🏼 Par exemple, /channel @{1}",
+    'zh': "👮🏽 将@{0}-bot 添加到频道并发送该频道的正确<i>链接</i>\n\n👉🏼 例如， /channel @{1}",
+    'ar': "👮🏽 Add @ {0} -bot إلى القناة وأرسل <i>الرابط</i> الصحيح لهذه القناة\n\n👉🏼 على سبيل المثال ، /channel @{1}",
 }
 l_delay_correct = {
-    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👩🏽‍💻 Например, /delay 1\n\nИли используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
-    'en': "👥 <b>Enter</b> the correct <i>number of</i> minutes to limit new users for the first time\n\n👩🏽‍💻 For example, /delay 1\n\nOr use <b>slow mode</b> in group settings for <u>1</u> message",
-    'es': "👥 <b>Ingrese</b> la <i>cantidad correcta de</i> minutos para limitar nuevos usuarios por primera vez\n\n👩🏽‍💻 Por ejemplo, /delay 1\n\nO use <b>el modo lento</b> en la configuración del grupo para <u>1</u> mensaje",
-    'fr': "👥 <b>Entrez</b> le <i>nombre correct de</i> minutes pour limiter les nouveaux utilisateurs pour la première fois\n\n👩🏽‍💻 Par exemple, /delay 1\n\nOu utilisez <b>le mode lent</b> dans les paramètres de groupe pour <u>1</u> message",
-    'zh': "👥 第一次<b>输入</b>正确的分钟<i>数</i>限制新用户\n\n👩🏽‍💻 例如/delay 1\n\n或者在群设置中使用<b>慢速模式</b><u>1条</u>消息",
-    'ar': "👥 <b>أدخل</b> <i>العدد</i> الصحيح للدقائق لتقييد المستخدمين الجدد لأول مرة\n\n👩🏽‍💻 على سبيل المثال ، /delay 1\n\nأو استخدم <b>الوضع البطيء</b> في إعدادات المجموعة لرسالة <u>واحدة</u>",
+    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Например, /delay 1\n\nИли используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
+    'en': "👥 <b>Enter</b> the correct <i>number of</i> minutes to limit new users for the first time\n\n👉🏼 For example, /delay 1\n\nOr use <b>slow mode</b> in group settings for <u>1</u> message",
+    'es': "👥 <b>Ingrese</b> la <i>cantidad correcta de</i> minutos para limitar nuevos usuarios por primera vez\n\n👉🏼 Por ejemplo, /delay 1\n\nO use <b>el modo lento</b> en la configuración del grupo para <u>1</u> mensaje",
+    'fr': "👥 <b>Entrez</b> le <i>nombre correct de</i> minutes pour limiter les nouveaux utilisateurs pour la première fois\n\n👉🏼 Par exemple, /delay 1\n\nOu utilisez <b>le mode lent</b> dans les paramètres de groupe pour <u>1</u> message",
+    'zh': "👥 第一次<b>输入</b>正确的分钟<i>数</i>限制新用户\n\n👉🏼 例如/delay 1\n\n或者在群设置中使用<b>慢速模式</b><u>1条</u>消息",
+    'ar': "👥 <b>أدخل</b> <i>العدد</i> الصحيح للدقائق لتقييد المستخدمين الجدد لأول مرة\n\n👉🏼 على سبيل المثال ، /delay 1\n\nأو استخدم <b>الوضع البطيء</b> في إعدادات المجموعة لرسالة <u>واحدة</u>",
 }
 l_parse_error = {
-    'ru': "📇 <b>Осуществить</b> парсинг пользователей  не удалось",
+    'ru': "📇 Осуществить парсинг пользователей  не удалось",
     'en': "📇 Failed to parse users",
     'es': "📇 No se pudieron analizar los usuarios",
     'fr': "📇 Échec de l'analyse des utilisateurs",
     'zh': "📇 解析用户失败",
     'ar': "📇 فشل تحليل المستخدمين",
 }
 l_parse_done = {
@@ -4347,63 +4004,63 @@
     'en': "📇 Let's start parsing..",
     'es': "📇 Empecemos a analizar..",
     'fr': "📇 Commençons l'analyse..",
     'zh': "📇 让我们开始解析..",
     'ar': "📇 لنبدأ في التحليل ..",
 }
 l_ban_handler = {
-    'ru': "🪦 <b>Пользователь</b> {0} в /ban-списке на {1}",
+    'ru': "🪦 Пользователь {0} в бане на {1}",
     'en': "🪦 User {0} is banned on {1}",
     'es': "🪦 El usuario {0} está prohibido en {1}",
     'fr': "🪦 L'utilisateur {0} est banni sur {1}",
     'zh': "🪦 用户 {0} 在 {1} 被封禁",
     'ar': "🪦 المستخدم {0} محظور على {1}",
 }
 l_ban_error = {
-    'ru': "🪦 <b>Формат</b> /ban-команды: /ban (1m|1h|10d)",
+    'ru': "🪦 Формат бана: /ban (1m|1h|10d)",
     'en': "🪦 Ban format: /ban (1m|1h|10d)",
     'es': "🪦 Formato de prohibición: /ban (1m|1h|10d)",
     'fr': "🪦 Format d'interdiction : /ban (1m|1h|10j)",
     'zh': "🪦 禁令格式：/ban (1m|1h|10d)",
     'ar': "🪦 تنسيق الحظر: / ban (1m | 1h | 10d)",
 }
 l_ban_unban = {
-    'ru': "🪦 <b>Пользователь</b> удален из /ban-списка",
+    'ru': "🪦 Пользователь возвращен из бана",
     'en': "🪦 User returned from ban",
     'es': "🪦 Usuario regresado de baneo",
     'fr': "🪦 L'utilisateur est revenu de l'interdiction",
     'zh': "🪦 用户从禁令中恢复",
     'ar': "🪦 عاد المستخدم من الحظر",
 }
 l_mute_handler = {
-    'ru': "💤 <b>Пользователь</b> {0} обеззвучен на {1}",
+    'ru': "💤 Пользователь {0} обеззвучен на {1}",
     'en': "💤 User {0} mute on {1}",
     'es': "💤 Usuario {0} silenciado en {1}",
     'fr': "💤 Utilisateur {0} muet sur {1}",
     'zh': "💤 用户 {0} 在 {1} 上静音",
     'ar': "💤 المستخدم {0} كتم الصوت في {1}",
 }
 l_mute_error = {
-    'ru': "💤 <b>Формат</b> /mute-команды: /mute (1m|1h|10d)",
+    'ru': "💤 Формат обеззвучивания: /mute (1m|1h|10d)",
     'en': "💤 Mute format: /mute (1m|1h|10d)",
     'es': "💤 Formato de silencio: /mute (1m|1h|10d)",
     'fr': "💤 Format muet : /muet (1m|1h|10j)",
     'zh': "💤 静音格式：/mute (1m|1h|10d)",
     'ar': "💤 تنسيق كتم الصوت: / كتم الصوت (1 م | 1 س | 10 د)",
 }
 l_mute_unmute = {
-    'ru': "💤 <b>Пользователь</b> {0} больше не обеззвучен",
+    'ru': "💤 Пользователь {0} больше не обеззвучен",
     'en': "💤 User {0} is no longer mute",
     'es': "💤 El usuario {0} ya no está silenciado",
     'fr': "💤 L'utilisateur {0} n'est plus muet",
     'zh': "💤 用户 {0} 不再是静音",
     'ar': "💤 المستخدم {0} لم يعد كتم الصوت",
 }
 l_warn_handler = {
-    'ru': "⚠️ <b>От имени</b> группы <b>{0}</b> выносится предупреждение {1}{2}",
+    'ru': "⚠️ От имени группы <b>{0}</b> выносится предупреждение {1}{2}",
     'en': "⚠️ Warning {1}{2} on behalf of group <b>{0}</b>",
     'es': "⚠️ Advertencia {1}{2} en nombre del grupo <b>{0}</b>",
     'fr': "⚠️ Avertissement {1}{2} de la part du groupe <b>{0}</b>",
     'zh': "⚠️ 代表<b>{0}</b>组警告{1}{2}",
     'ar': "⚠️ تحذير {1} {2} نيابة عن المجموعة <b>{0}</b>",
 }
 l_status_pin = {
@@ -4484,20 +4141,20 @@
     'en': "@ You must enter a message",
     'es': "@ Debes ingresar un mensaje",
     'fr': "@ Vous devez entrer un message",
     'zh': "@你必须输入信息",
     'ar': "@ يجب عليك إدخال رسالة",
 }
 l_help_handler = {
-    'ru': "👩🏽‍💻 <b>Команды</b> пользователя:\n\n/rules - правила группы\n/report - сообщить о нарушении\n/happy - получить радость\n/thanks - поблагодарить",
-    'en': "👩🏽‍💻 User <b>commands</b> :\n\n/rules - group rules\n/report - report violation\n/happy - get joy\n/thanks - give thanks",
-    'es': "👩🏽‍💻 <b>Comandos</b> de usuario:\n\n/reglas - reglas de grupo\n/reportar - reportar violación\n/feliz - alegría\n/gracias - dar gracias",
-    'fr': "👩🏽‍💻 <b>Commandes</b> utilisateur :\n\n/règles - règles de groupe\n/signaler - signaler une violation\n/heureux - obtenir de la joie\n/merci - rendre grâce",
-    'zh': "👩🏽‍💻 用户<b>命令</b>：\n\n/rules - 组规则\n/report - 报告违规\n/happy - 获得快乐\n/thanks - 给予感谢",
-    'ar': "👩🏽‍💻 <b>أوامر</b> المستخدم:\n\n/ القواعد - قواعد المجموعة\n/ الإبلاغ - الإبلاغ عن انتهاك\n/ سعيد - ابتهج\n/ شكرًا - شكر",
+    'ru': "👉🏼 <b>Команды</b> пользователя:\n\n/rules - правила группы\n/report - сообщить о нарушении\n/happy - получить радость\n/thanks - поблагодарить",
+    'en': "👉🏼 User <b>commands</b> :\n\n/rules - group rules\n/report - report violation\n/happy - get joy\n/thanks - give thanks",
+    'es': "👉🏼 <b>Comandos</b> de usuario:\n\n/reglas - reglas de grupo\n/reportar - reportar violación\n/feliz - alegría\n/gracias - dar gracias",
+    'fr': "👉🏼 <b>Commandes</b> utilisateur :\n\n/règles - règles de groupe\n/signaler - signaler une violation\n/heureux - obtenir de la joie\n/merci - rendre grâce",
+    'zh': "👉🏼 用户<b>命令</b>：\n\n/rules - 组规则\n/report - 报告违规\n/happy - 获得快乐\n/thanks - 给予感谢",
+    'ar': "👉🏼 <b>أوامر</b> المستخدم:\n\n/ القواعد - قواعد المجموعة\n/ الإبلاغ - الإبلاغ عن انتهاك\n/ سعيد - ابتهج\n/ شكرًا - شكر",
 }
 l_report_handler = {
     'ru': "❗️ Информация передана администратору. Пользователь {0} взят на карандаш",
     'en': "❗️ The information has been sent to the administrator. User {0} is penciled",
     'es': "❗️ La información ha sido enviada al administrador. El usuario {0} está escrito a lápiz",
     'fr': "❗️ L'information a été transmise à l'administrateur. L'utilisateur {0} est au crayon",
     'zh': "❗️资料已发给管理员。用户 {0} 已使用铅笔",
@@ -4556,20 +4213,20 @@
     'en': "🎥 Automatic announcement <b>of the video broadcast</b> [/videochat dh] every <u>d</u> -day (1-31) for <u>h</u> -hours (1-168). Current value: /videochat {0}\n\n👩🏽‍💻 For example\n/videochat 1 1 (daily 1 hour video announcement)\n/videochat 0 (disable option)",
     'es': "🎥 Anuncio automático <b>de la transmisión de video</b> [/videochat dh] cada <u>d</u> -día (1-31) durante <u>h</u> -horas (1-168). Valor actual: /videochat {0}\n\n👩🏽‍💻 Por ejemplo\n/videochat 1 1 (anuncio de video diario de 1 hora)\n/videochat 0 (opción deshabilitada)",
     'fr': "🎥 Annonce automatique <b>de la diffusion vidéo</b> [/videochat dh] tous <u>les j</u> -jours (1-31) pendant <u>h</u> -heures (1-168). Valeur actuelle : /videochat {0}\n\n👩🏽‍💻 Par exemple\n/videochat 1 1 (annonce vidéo quotidienne d&#x27;une heure)\n/videochat 0 (option de désactivation)",
     'zh': "🎥 每<u>d</u>天（1-31）自动播报<b>视频广播</b>[/videochat dh] ，持续<u>h</u>小时（1-168）。当前值：/videochat {0}\n\n👩🏽‍💻 例如\n/videochat 1 1 （每天1小时视频公告）\n/videochat 0 （禁用选项）",
     'ar': "🎥 الإعلان التلقائي <b>عن بث الفيديو</b> [/videochat dh] كل يوم <u>يوم</u> (1-31) لمدة <u>ساعة</u> (1-168). القيمة الحالية: / videochat {0}\n\n👩🏽‍💻 على سبيل المثال\n/videochat 1 1 (إعلان فيديو لمدة ساعة يوميًا)\n/videochat 0 (خيار تعطيل)",
 }
 l_flood_text = {
-    'ru': "💬 <b>Введи</b> корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👩🏽‍💻 <b>Текущее</b> значение /flood {0}\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
-    'en': "💬 Please <b>enter</b> a valid <i>number</i> of messages from <u>3</u> to <u>10</u>\n\n👩🏽‍💻 <b>Current</b> value /flood {0}\n\n👩🏽‍💻 For example, /flood 3 (identifies 3 messages in a row as a flood)\n/flood 0 (disables options)",
-    'es': "💬 <b>Ingrese</b> un <i>número</i> válido de mensajes de <u>3</u> a <u>10</u>\n\n👩🏽‍💻 Valor <b>actual</b> /flood {0}\n\n👩🏽‍💻 Por ejemplo, /inundación 3 (identifica 3 mensajes seguidos como una inundación)\n/inundación 0 (deshabilita opciones)",
-    'fr': "💬 Veuillez <b>entrer</b> un <i>nombre</i> valide de messages de <u>3</u> à <u>10</u>\n\n👩🏽‍💻 Valeur <b>actuelle</b> /flood {0}\n\n👩🏽‍💻 Par exemple, /flood 3 (identifie 3 messages à la suite comme une inondation)\n/flood 0 (désactive les options)",
+    'ru': "💬 <b>Введи</b> корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👉🏼 <b>Текущее</b> значение /flood {0}\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
+    'en': "💬 Please <b>enter</b> a valid <i>number</i> of messages from <u>3</u> to <u>10</u>\n\n👉🏼 <b>Current</b> value /flood {0}\n\n👩🏽‍💻 For example, /flood 3 (identifies 3 messages in a row as a flood)\n/flood 0 (disables options)",
+    'es': "💬 <b>Ingrese</b> un <i>número</i> válido de mensajes de <u>3</u> a <u>10</u>\n\n👉🏼 Valor <b>actual</b> /flood {0}\n\n👩🏽‍💻 Por ejemplo, /inundación 3 (identifica 3 mensajes seguidos como una inundación)\n/inundación 0 (deshabilita opciones)",
+    'fr': "💬 Veuillez <b>entrer</b> un <i>nombre</i> valide de messages de <u>3</u> à <u>10</u>\n\n👉🏼 Valeur <b>actuelle</b> /flood {0}\n\n👩🏽‍💻 Par exemple, /flood 3 (identifie 3 messages à la suite comme une inondation)\n/flood 0 (désactive les options)",
     'zh': "💬<b>请输入</b><u>3</u>到<u>10</u>之间的有效消息<i>数</i>\n\n👉🏼<b>当前</b>值/flood {0}\n\n👩🏽‍💻 例如 /flood 3（连续 3 条消息标识为洪水）\n/flood 0（禁用选项）",
-    'ar': "💬 الرجاء <b>إدخال</b> <i>رقم</i> صالح للرسائل من <u>3</u> إلى <u>10</u>\n\n👩🏽‍💻 القيمة <b>الحالية</b> /flood {0}\n\n👩🏽‍💻 على سبيل المثال ، / فيضان 3 (يحدد 3 رسائل في صف واحد كفيضان)\n/ فيضان 0 (تعطيل الخيارات)",
+    'ar': "💬 الرجاء <b>إدخال</b> <i>رقم</i> صالح للرسائل من <u>3</u> إلى <u>10</u>\n\n👉🏼 القيمة <b>الحالية</b> /flood {0}\n\n👩🏽‍💻 على سبيل المثال ، / فيضان 3 (يحدد 3 رسائل في صف واحد كفيضان)\n/ فيضان 0 (تعطيل الخيارات)",
 }
 l_flood_on = {
     'ru': "💬 <b>Установлен</b> flood-режим: {0} сообщения подряд",
     'en': "💬 Set flood mode: {0} messages in a row",
     'es': "💬 Establecer modo de inundación: {0} mensajes seguidos",
     'fr': "💬 Définir le mode flood : {0} messages d'affilée",
     'zh': "💬 设置泛洪模式：连续 {0} 条消息",
@@ -4580,20 +4237,20 @@
     'en': "💬 Flood mode disabled",
     'es': "💬 Modo de inundación deshabilitado",
     'fr': "💬 Mode inondation désactivé",
     'zh': "💬洪水模式禁用",
     'ar': "💬 وضع الفيضان معطل",
 }
 l_delay_text = {
-    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👩🏽‍💻 <b>Текущее</b> значение /delay {0}\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
-    'en': "👥 <b>Please enter</b> the correct <i>number</i> of minutes for the initial limit of new users\n\n👩🏽‍💻 <b>The current</b> value of /delay {0}\n\n👩🏽‍💻 For example, /delay 3 (3 min limit)\n/delay 0 (disable option )",
-    'es': "👥 <b>Ingrese</b> la <i>cantidad</i> correcta de minutos para el límite inicial de nuevos usuarios\n\n👩🏽‍💻 <b>El valor actual</b> de /delay {0}\n\n👩🏽‍💻 Por ejemplo, /delay 3 (límite de 3 min)\ n/delay 0 (opción deshabilitar)",
-    'fr': "👥 <b>Veuillez entrer</b> le <i>nombre</i> correct de minutes pour la limite initiale de nouveaux utilisateurs\n\n👩🏽‍💻 <b>La valeur actuelle</b> de /delay {0}\n\n👩🏽‍💻 Par exemple, /delay 3 (3 min limit)\ n/délai 0 (désactiver l'option )",
-    'zh': "👥<b>请输入</b>正确的新用户初始限制分钟<i>数</i>\n\n👩🏽‍💻 /delay {0}<b>当前</b>值{0}\n\n👩🏽‍💻 例如/delay 3（3分钟限制）\ n/delay 0（禁用选项）",
-    'ar': "👥 <b>الرجاء إدخال</b> <i>العدد</i> الصحيح للدقائق للحد الأولي للمستخدمين الجدد\n\n👩🏽‍💻 القيمة <b>الحالية</b> لـ /delay {0}\n\n👩🏽‍💻 على سبيل المثال ، / delay 3 (3 min limit) \ ن / تأخير 0 (تعطيل الخيار)",
+    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 <b>Текущее</b> значение /delay {0}\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
+    'en': "👥 <b>Please enter</b> the correct <i>number</i> of minutes for the initial limit of new users\n\n👉🏼 <b>The current</b> value of /delay {0}\n\n👩🏽‍💻 For example, /delay 3 (3 min limit)\n/delay 0 (disable option )",
+    'es': "👥 <b>Ingrese</b> la <i>cantidad</i> correcta de minutos para el límite inicial de nuevos usuarios\n\n👉🏼 <b>El valor actual</b> de /delay {0}\n\n👩🏽‍💻 Por ejemplo, /delay 3 (límite de 3 min)\ n/delay 0 (opción deshabilitar)",
+    'fr': "👥 <b>Veuillez entrer</b> le <i>nombre</i> correct de minutes pour la limite initiale de nouveaux utilisateurs\n\n👉🏼 <b>La valeur actuelle</b> de /delay {0}\n\n👩🏽‍💻 Par exemple, /delay 3 (3 min limit)\ n/délai 0 (désactiver l'option )",
+    'zh': "👥<b>请输入</b>正确的新用户初始限制分钟<i>数</i>\n\n👉🏼 /delay {0}<b>当前</b>值{0}\n\n👩🏽‍💻 例如/delay 3（3分钟限制）\ n/delay 0（禁用选项）",
+    'ar': "👥 <b>الرجاء إدخال</b> <i>العدد</i> الصحيح للدقائق للحد الأولي للمستخدمين الجدد\n\n👉🏼 القيمة <b>الحالية</b> لـ /delay {0}\n\n👩🏽‍💻 على سبيل المثال ، / delay 3 (3 min limit) \ ن / تأخير 0 (تعطيل الخيار)",
 }
 l_delay_on = {
     'ru': "👥 <b>Готово!</b> Текущая первичная задержка для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) установлена в значение <u>{0}</u> min",
     'en': "👥 <b>Done!</b> The current initial delay for <u>new</u> users (before writing their <u>1st</u> message) is set to <u>{0}</u> min",
     'es': "👥 <b>Listo!</b> El retraso inicial actual para <u>nuevos</u> usuarios (antes de escribir su <u>primer</u> mensaje) se establece en <u>{0}</u> min",
     'fr': "👥 <b>C&#x27;est fait !</b> Le délai initial actuel pour <u>les nouveaux</u> utilisateurs (avant d&#x27;écrire leur <u>1er</u> message) est défini sur <u>{0}</u> min",
     'zh': "👥<b>完成！</b><u>新</u>用户的当前初始延迟（在编写他们的<u>第一条</u>消息之前）设置为<u>{0}</u>分钟",
@@ -4604,48 +4261,48 @@
     'en': "👥 Delay mode disabled",
     'es': "👥 Modo de retraso deshabilitado",
     'fr': "👥 Mode délai désactivé",
     'zh': "👥 禁用延迟模式",
     'ar': "👥 وضع التأخير معطل",
 }
 l_rules_handler = {
-    'ru': "👩🏽‍💻 <b>Правила</b> группы <b>{0}</b>:\n\n{1}",
-    'en': "👩🏽‍💻 Group <b>rules</b> <b>{0}</b> :\n\n{1}",
-    'es': "👩🏽‍💻 <b>Reglas</b> de grupo <b>{0}</b> :\n\n{1}",
-    'fr': "👩🏽‍💻 <b>Règles</b> de groupe <b>{0}</b> :\n\n{1}",
-    'zh': "👩🏽‍💻 组<b>规则{0}</b> :\n\n{1}",
-    'ar': "👩🏽‍💻 <b>قواعد</b> المجموعة <b>{0}</b> :\n\n{1}",
+    'ru': "👉🏼 <b>Правила</b> группы <b>{0}</b>:\n\n{1}",
+    'en': "👉🏼 Group <b>rules</b> <b>{0}</b> :\n\n{1}",
+    'es': "👉🏼 <b>Reglas</b> de grupo <b>{0}</b> :\n\n{1}",
+    'fr': "👉🏼 <b>Règles</b> de groupe <b>{0}</b> :\n\n{1}",
+    'zh': "👉🏼 组<b>规则{0}</b> :\n\n{1}",
+    'ar': "👉🏼 <b>قواعد</b> المجموعة <b>{0}</b> :\n\n{1}",
 }
 l_rules_on = {
-    'ru': "👩🏽‍💻 <b>Установлены</b> <u>новые</u> <b>правила</b> для группы <b>{0}</b>:\n\n{1}",
-    'en': "👩🏽‍💻 <u>New</u> <b>rules</b> set for group <b>{0}</b> :\n\n{1}",
-    'es': "👩🏽‍💻 <u>Nuevas</u> <b>reglas</b> establecidas para el grupo <b>{0}</b> :\n\n{1}",
-    'fr': "👩🏽‍💻 <u>Nouvelles</u> <b>règles</b> définies pour le groupe <b>{0}</b> :\n\n{1}",
-    'zh': "👩🏽‍💻 为组<b>{0}</b>设置的<u>新</u><b>规则</b>：\n\n{1}",
-    'ar': "👩🏽‍💻 تم تعيين <b>قواعد</b> <u>جديدة</u> للمجموعة <b>{0}</b> :\n\n{1}",
+    'ru': "👉🏼 <b>Установлены</b> <u>новые</u> <b>правила</b> для группы <b>{0}</b>:\n\n{1}",
+    'en': "👉🏼 <u>New</u> <b>rules</b> set for group <b>{0}</b> :\n\n{1}",
+    'es': "👉🏼 <u>Nuevas</u> <b>reglas</b> establecidas para el grupo <b>{0}</b> :\n\n{1}",
+    'fr': "👉🏼 <u>Nouvelles</u> <b>règles</b> définies pour le groupe <b>{0}</b> :\n\n{1}",
+    'zh': "👉🏼 为组<b>{0}</b>设置的<u>新</u><b>规则</b>：\n\n{1}",
+    'ar': "👉🏼 تم تعيين <b>قواعد</b> <u>جديدة</u> للمجموعة <b>{0}</b> :\n\n{1}",
 }
 l_rules_off = {
-    'ru': "👩🏽‍💻 <b>Правила</b> в группе <b>{0}</b> не установлены. Необходимо <u>ответить на пост</u> с правилами <b>командой</b> /rules",
-    'en': "👩🏽‍💻 <b>The rules</b> in group <b>{0}</b> are not set. <u>Reply to a post</u> with rules with the /rules <b>command</b>",
-    'es': "👩🏽‍💻 <b>Las reglas</b> del grupo <b>{0}</b> no están establecidas. <u>Responda a una publicación</u> con reglas con el <b>comando</b> /rules",
-    'fr': "👩🏽‍💻 <b>Les règles</b> du groupe <b>{0}</b> ne sont pas définies. <u>Répondre à un message</u> avec des règles avec la <b>commande</b> /rules",
+    'ru': "👉🏼 <b>Правила</b> в группе <b>{0}</b> не установлены. Необходимо <u>ответить на пост</u> с правилами <b>командой</b> /rules",
+    'en': "👉🏼 <b>The rules</b> in group <b>{0}</b> are not set. <u>Reply to a post</u> with rules with the /rules <b>command</b>",
+    'es': "👉🏼 <b>Las reglas</b> del grupo <b>{0}</b> no están establecidas. <u>Responda a una publicación</u> con reglas con el <b>comando</b> /rules",
+    'fr': "👉🏼 <b>Les règles</b> du groupe <b>{0}</b> ne sont pas définies. <u>Répondre à un message</u> avec des règles avec la <b>commande</b> /rules",
     'zh': "👉🏼组<b>{0}</b>中的<b>规则</b>未设置。使用 /rules<b>命令</b><u>回复带有规则的帖子</u>",
-    'ar': "👩🏽‍💻 لم يتم تعيين <b>القواعد</b> في المجموعة <b>{0}</b> . <u>قم بالرد على منشور</u> بالقواعد باستخدام <b>الأمر</b> / rules",
+    'ar': "👉🏼 لم يتم تعيين <b>القواعد</b> في المجموعة <b>{0}</b> . <u>قم بالرد على منشور</u> بالقواعد باستخدام <b>الأمر</b> / rules",
 }
 # endregion
 
 
 # region ccheck
 l_ccheck_handler = {
-    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> в группу\n\n👩🏽‍💻 Для установки имени <b>нажимаемой кнопки</b>, выполни команду: /button {0}\n\n👩🏽‍💻 Для <b>проверки подписки</b> на канал <i>добавь</i> @{1}-бота в канал и выполни команду: /channel {2}\n\n👩🏽‍💻 Для <i>защиты от атаки</i> на группу включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
-    'en': "👮🏽 <b>Click</b> on ✅/🔘 to <b>switch</b> the type of user <i>verification</i> when <u>joining</u> a group\n\n👩🏽‍💻 To set the name <b>of the button to be pressed</b> , run the command: /button {0}\n\n👩🏽‍💻 To <b>check the subscription</b> to the channel <i>, add</i> @ {1}-bot into the channel and execute the command: /channel {2}\n\n👩🏽‍💻 To <i>protect against an attack</i> on the group, turn on the <b>anti-raid</b> mode (blocking <u>all</u> joiners)",
-    'es': "👮🏽 <b>Haz clic</b> en ✅/🔘 para <b>cambiar</b> el tipo de <i>verificación</i> de usuario al <u>unirte a</u> un grupo\n\n👩🏽‍💻 Para establecer el nombre <b>del botón que se presionará</b> , ejecuta el comando: /button {0}\n\n👩🏽‍💻 Para <b>verificar la suscripción</b> al canal <i>, agregue</i> @ {1}-bot al canal y ejecute el comando: /channel {2}\n\n👩🏽‍💻 Para <i>protegerse contra un ataque</i> al grupo, active el modo <b>anti-raid</b> (bloqueando <u>a todos</u> los carpinteros)",
-    'fr': "👮🏽 <b>Cliquez</b> sur ✅/🔘 pour <b>changer</b> le type de <i>vérification</i> de l&#x27;utilisateur lors <u>de l&#x27;adhésion à</u> un groupe\n\n👩🏽‍💻 Pour définir le nom <b>du bouton à appuyer</b> , exécutez la commande : /button {0}\n\n👩🏽‍💻 Pour <b>vérifier l&#x27;abonnement</b> au canal <i>, ajoutez</i> @{1}-bot dans le canal et exécutez la commande : /channel {2}\n\n👩🏽‍💻 Pour <i>vous protéger contre une attaque</i> sur le groupe, activez le mode <b>anti-raid</b> (bloquant <u>tous</u> les participants)",
-    'zh': "👮🏽<b>点击</b>✅/🔘<b>切换</b><u>加入</u>群组时的用户<i>验证</i>类型\n\n👩🏽‍💻 要设置<b>要按下的按钮</b>的名称，运行命令： /button {0}\n\n👉🏼<b>查看频道订阅情况</b><i>，将@{1}-bot 添加</i>到频道，执行命令： /channel {2}\n\n👩🏽‍💻 为<i>防止群内攻击</i>，开启<b>防突袭</b>模式（阻止<u>所有</u>加入者）",
-    'ar': "👮🏽 <b>انقر</b> فوق ✅ / 🔘 <b>لتبديل</b> نوع <i>التحقق</i> من المستخدم عند <u>الانضمام إلى</u> مجموعة\n\n👩🏽‍💻 لتعيين اسم <b>الزر المراد الضغط عليه</b> ، قم بتشغيل الأمر: /button {0}\n\n👩🏽‍💻 للتحقق <b>من الاشتراك</b> في القناة <i>، أضف</i> @ {1} -bot إلى القناة ونفذ الأمر: /channel {2}\n\n👩🏽‍💻 <i>للحماية من هجوم</i> على المجموعة ، شغّل وضع <b>anti-raid</b> (حظر <u>جميع</u> النجارين)",
+    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> в группу\n\n👉🏼 Для установки имени <b>нажимаемой кнопки</b>, выполни команду: /button {0}\n\n👉🏼 Для <b>проверки подписки</b> на канал <i>добавь</i> @{1}-бота в канал и выполни команду: /channel {2}\n\n👉🏼 Для <i>защиты от атаки</i> на группу включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
+    'en': "👮🏽 <b>Click</b> on ✅/🔘 to <b>switch</b> the type of user <i>verification</i> when <u>joining</u> a group\n\n👉🏼 To set the name <b>of the button to be pressed</b> , run the command: /button {0}\n\n👉🏼 To <b>check the subscription</b> to the channel <i>, add</i> @ {1}-bot into the channel and execute the command: /channel {2}\n\n👉🏼 To <i>protect against an attack</i> on the group, turn on the <b>anti-raid</b> mode (blocking <u>all</u> joiners)",
+    'es': "👮🏽 <b>Haz clic</b> en ✅/🔘 para <b>cambiar</b> el tipo de <i>verificación</i> de usuario al <u>unirte a</u> un grupo\n\n👉🏼 Para establecer el nombre <b>del botón que se presionará</b> , ejecuta el comando: /button {0}\n\n👉🏼 Para <b>verificar la suscripción</b> al canal <i>, agregue</i> @ {1}-bot al canal y ejecute el comando: /channel {2}\n\n👉🏼 Para <i>protegerse contra un ataque</i> al grupo, active el modo <b>anti-raid</b> (bloqueando <u>a todos</u> los carpinteros)",
+    'fr': "👮🏽 <b>Cliquez</b> sur ✅/🔘 pour <b>changer</b> le type de <i>vérification</i> de l&#x27;utilisateur lors <u>de l&#x27;adhésion à</u> un groupe\n\n👉🏼 Pour définir le nom <b>du bouton à appuyer</b> , exécutez la commande : /button {0}\n\n👉🏼 Pour <b>vérifier l&#x27;abonnement</b> au canal <i>, ajoutez</i> @{1}-bot dans le canal et exécutez la commande : /channel {2}\n\n👉🏼 Pour <i>vous protéger contre une attaque</i> sur le groupe, activez le mode <b>anti-raid</b> (bloquant <u>tous</u> les participants)",
+    'zh': "👮🏽<b>点击</b>✅/🔘<b>切换</b><u>加入</u>群组时的用户<i>验证</i>类型\n\n👉🏼 要设置<b>要按下的按钮</b>的名称，运行命令： /button {0}\n\n👉🏼<b>查看频道订阅情况</b><i>，将@{1}-bot 添加</i>到频道，执行命令： /channel {2}\n\n👉🏼 为<i>防止群内攻击</i>，开启<b>防突袭</b>模式（阻止<u>所有</u>加入者）",
+    'ar': "👮🏽 <b>انقر</b> فوق ✅ / 🔘 <b>لتبديل</b> نوع <i>التحقق</i> من المستخدم عند <u>الانضمام إلى</u> مجموعة\n\n👉🏼 لتعيين اسم <b>الزر المراد الضغط عليه</b> ، قم بتشغيل الأمر: /button {0}\n\n👉🏼 للتحقق <b>من الاشتراك</b> في القناة <i>، أضف</i> @ {1} -bot إلى القناة ونفذ الأمر: /channel {2}\n\n👉🏼 <i>للحماية من هجوم</i> على المجموعة ، شغّل وضع <b>anti-raid</b> (حظر <u>جميع</u> النجارين)",
 }
 l_ccheck_add = {
     'ru': "\n\nВ настройках [Администраторы] вкл для {0}-бота:\n[✅ Удаление сообщ]\n[✅ Блокировка польз]\n[✅ Добавление участ]\n\n🕚Подожди 1min",
     'en': "\n\nIn [Administrators] settings, on for {0}-bot:\n[✅ Deleting messages]\n[✅ Blocking users]\n[✅ Adding members]\n\n🕚Wait 1min",
     'es': "\n\nEn la configuración de [Administradores], activado para {0}-bot:\n[✅ Eliminación de mensajes]\n[✅ Bloqueo de usuarios]\n[✅ Adición de miembros]\n\n🕚Espera 1 minuto",
     'fr': "\n\nDans les paramètres [Administrateurs], activé pour {0}-bot :\n[✅ Suppression de messages]\n[✅ Blocage d'utilisateurs]\n[✅ Ajout de membres]\n\n🕚Attendez 1 min",
     'zh': "\n\n在 [管理员] 设置中，为 {0}-bot 打开：\n[✅ 删除消息]\n[✅ 阻止用户]\n[✅ 添加成员]\n\n🕚 等待 1 分钟",
@@ -4688,15 +4345,15 @@
     'en': "👮🏽 You didn't join {0}\n\nPlease try again later",
     'es': "👮🏽 No te uniste {0}\n\nPor favor, inténtalo de nuevo más tarde",
     'fr': "👮🏽 Vous n'avez pas rejoint {0}\n\nVeuillez réessayer plus tard",
     'zh': "👮🏽您没有加入{0}\n\n请稍后再试",
     'ar': "👮🏽 لم تنضم إلى {0}\n\nالرجاء المحاولة مرة أخرى لاحقًا",
 }
 l_ccheck_ban = {
-    'ru': "👮🏽‍ <b>Пользователь</b> {0} не прошел входной контроль и был удален из группы",
+    'ru': "👮🏽‍ Пользователь {0} не прошел входной контроль и был удален из группы",
     'en': "👮🏽‍ User {0} failed entry control and was removed from the group",
     'es': "👮🏽‍ El usuario {0} falló el control de entrada y fue eliminado del grupo",
     'fr': "👮🏽‍ L'utilisateur {0} a échoué au contrôle d'entrée et a été retiré du groupe",
     'zh': "👮🏽‍ 用户 {0} 未能通过访问控制并被移出群组",
     'ar': "👮🏽‍ المستخدم {0} فشل في التحكم في الدخول وتمت إزالته من المجموعة",
 }
 l_ccheckchannel_error = {
@@ -4740,20 +4397,20 @@
     'en': "Your greeting",
     'es': "Tu saludo",
     'fr': "Votre message d'accueil",
     'zh': "你的问候",
     'ar': "تحياتك",
 }
 l_chello_text = {
-    'ru': "👋🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👩🏽‍💻 Например, {0}{1}",
-    'en': "👋🏽 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the greeting, as well as its ⚙️Customize\n\n👩🏽‍💻 For example, {0} {1}",
-    'es': "👋🏽 <b>Haz clic</b> en ✅/☑️ para <b>activar o desactivar</b> el saludo, así como su ⚙️Personalizar\n\n👩🏽‍💻 Por ejemplo, {0} {1}",
-    'fr': "👋🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> le message d&#x27;accueil, ainsi que sa ⚙️Personnaliser\n\n👩🏽‍💻 Par exemple, {0} {1}",
-    'zh': "👋🏽<b>点击</b>✅/☑️<b>打开/关闭</b>问候语，以及它的 ⚙️自定义\n\n👩🏽‍💻 例如， {0} {1}",
-    'ar': "👋🏽 <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> الترحيب ، بالإضافة إلى تخصيص\n\n👩🏽‍💻 على سبيل المثال ، {0} {1}",
+    'ru': "👋🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👉🏼 Например, {0}{1}",
+    'en': "👋🏽 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the greeting, as well as its ⚙️Customize\n\n👉🏼 For example, {0} {1}",
+    'es': "👋🏽 <b>Haz clic</b> en ✅/☑️ para <b>activar o desactivar</b> el saludo, así como su ⚙️Personalizar\n\n👉🏼 Por ejemplo, {0} {1}",
+    'fr': "👋🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> le message d&#x27;accueil, ainsi que sa ⚙️Personnaliser\n\n👉🏼 Par exemple, {0} {1}",
+    'zh': "👋🏽<b>点击</b>✅/☑️<b>打开/关闭</b>问候语，以及它的 ⚙️自定义\n\n👉🏼 例如， {0} {1}",
+    'ar': "👋🏽 <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> الترحيب ، بالإضافة إلى تخصيص\n\n👉🏼 على سبيل المثال ، {0} {1}",
 }
 l_btn_on = {
     'ru': "✅☑Вкл",
     'en': "✅☑Incl",
     'es': "✅☑Incluye",
     'fr': "✅☑Inclus",
     'zh': "✅☑包括",
@@ -4772,20 +4429,20 @@
     'en': "⚙️Customize",
     'es': "⚙️Personalizar",
     'fr': "⚙️Personnaliser",
     'zh': "⚙️自定义",
     'ar': "⚙️ تخصيص",
 }
 l_chellochange_handler = {
-    'ru': "👋🏽 Отправь мне <b>текст</b>/<b>медиа</b> контент с текстом: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n👩🏽‍💻 Например, {0}",
-    'en': "👋🏽 Send me <b>text</b> / <b>media</b> content with text: photo / gif / video / audio / document or write a voice / video note in a circle\n\n👩🏽‍💻 For example, {0}",
-    'es': "👋🏽 Envíame <b>texto</b> /contenido <b>multimedia</b> con texto: foto/gif/video/audio/documento o escribe una nota de voz/video en un círculo\n\n👩🏽‍💻 Por ejemplo, {0}",
-    'fr': "👋🏽 Envoyez-moi <b>du texte</b> /du contenu <b>multimédia</b> avec du texte : photo/gif/vidéo/audio/document ou écrivez une note vocale/vidéo dans un cercle\n\n👩🏽‍💻 Par exemple, {0}",
-    'zh': "👋🏽 向我发送<b>文字</b>/<b>媒体</b>内容并附上文字：照片/gif/视频/音频/文档或将语音/视频笔记写成一个圆圈\n\n👩🏽‍💻 例如， {0}",
-    'ar': "👋🏽 أرسل لي محتوى <b>نصيًا</b> / <b>وسائط</b> مع نص: صورة / gif / فيديو / صوت / مستند أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n👩🏽‍💻 على سبيل المثال ، {0}",
+    'ru': "👋🏽 Отправь мне <b>текст</b>/<b>медиа</b> контент с текстом: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n👉🏼 Например, {0}",
+    'en': "👋🏽 Send me <b>text</b> / <b>media</b> content with text: photo / gif / video / audio / document or write a voice / video note in a circle\n\n👉🏼 For example, {0}",
+    'es': "👋🏽 Envíame <b>texto</b> /contenido <b>multimedia</b> con texto: foto/gif/video/audio/documento o escribe una nota de voz/video en un círculo\n\n👉🏼 Por ejemplo, {0}",
+    'fr': "👋🏽 Envoyez-moi <b>du texte</b> /du contenu <b>multimédia</b> avec du texte : photo/gif/vidéo/audio/document ou écrivez une note vocale/vidéo dans un cercle\n\n👉🏼 Par exemple, {0}",
+    'zh': "👋🏽 向我发送<b>文字</b>/<b>媒体</b>内容并附上文字：照片/gif/视频/音频/文档或将语音/视频笔记写成一个圆圈\n\n👉🏼 例如， {0}",
+    'ar': "👋🏽 أرسل لي محتوى <b>نصيًا</b> / <b>وسائط</b> مع نص: صورة / gif / فيديو / صوت / مستند أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n👉🏼 على سبيل المثال ، {0}",
 }
 l_fsm_hello_finish = {
     'ru': "👋🏽 Приветствие записано!\n\nОпцию можно включить в настройках [👋🏽Авто-приветствие], нажав [✅☑Вкл]",
     'en': "👋🏽 Greeting recorded!\n\nThe option can be enabled in the settings [👋🏽Auto-greeting] by pressing [✅☑On]",
     'es': "👋🏽 ¡Saludo grabado!\n\nLa opción se puede habilitar en la configuración [👋🏽 Saludo automático] presionando [✅☑On]",
     'fr': "👋🏽 Message d'accueil enregistré !\n\nL'option peut être activée dans les paramètres [👋🏽Salutation automatique] en appuyant sur [✅☑On]",
     'zh': "👋🏽问候语已录制！\n\n可以在设置[👋🏽自动问候语]中按[✅☑开启]启用该选项",
@@ -4800,20 +4457,20 @@
     'en': "👮🏽 In the [Permissions] settings, enable the option:\n\n[✅ Adding a part]\n\n🕚Wait 1min",
     'es': "👮🏽 En la configuración de [Permisos], habilita la opción:\n\n[✅ Agregar una parte]\n\n🕚Espera 1 minuto",
     'fr': "👮🏽 Dans les paramètres [Autorisations], activez l'option :\n\n[✅ Ajout d'une pièce]\n\n🕚Attendez 1min",
     'zh': "👮🏽 在[权限]设置中，启用选项：\n\n[✅添加零件]\n\n🕚等待1分钟",
     'ar': "👮🏽 في إعدادات [الأذونات] ، قم بتمكين الخيار:\n\n[✅ إضافة جزء]\n\n🕚 انتظر دقيقة واحدة",
 }
 l_cinvite_text_add = {
-    'ru': "\n\n👩🏽‍💻 Приглашается <u>{0}</u> пользователей в сутки из группы {1}",
-    'en': "\n\n👩🏽‍💻 <u>{0}</u> users per day from {1} group are invited",
-    'es': "\n\n👩🏽‍💻 <u>{0}</u> usuarios por día del grupo {1} están invitados",
-    'fr': "\n\n👩🏽‍💻 <u>{0}</u> utilisateurs par jour de {1} groupe sont invités",
-    'zh': "\n\n👩🏽‍💻 每天邀请来自 {1} 个组的<u>{0} 个</u>用户",
-    'ar': "\n\n👩🏽‍💻 تمت دعوة <u>{0} من</u> المستخدمين يوميًا من مجموعة {1}",
+    'ru': "\n\n👉🏼 Приглашается <u>{0}</u> пользователей в сутки из группы {1}",
+    'en': "\n\n👉🏼 <u>{0}</u> users per day from {1} group are invited",
+    'es': "\n\n👉🏼 <u>{0}</u> usuarios por día del grupo {1} están invitados",
+    'fr': "\n\n👉🏼 <u>{0}</u> utilisateurs par jour de {1} groupe sont invités",
+    'zh': "\n\n👉🏼 每天邀请来自 {1} 个组的<u>{0} 个</u>用户",
+    'ar': "\n\n👉🏼 تمت دعوة <u>{0} من</u> المستخدمين يوميًا من مجموعة {1}",
 }
 l_cinvite_text = {
     'ru': "🚶🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-инвайт пользователей в <b>{0}</b>-группу\n\n👩🏽‍💻 <b>Текущие</b> настройки авто-рассылки: {1}",
     'en': "🚶🏽 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> auto-invite users to <b>{0}</b> -group\n\n👩🏽‍💻 <b>Current</b> auto-mailing settings: {1}",
     'es': "🚶🏽 <b>Haz clic</b> en ✅/☑️ para <b>habilitar o deshabilitar</b> la invitación automática de usuarios a <b>{0}</b> -group\n\n👩🏽‍💻 Configuración <b>actual</b> de correo automático: {1}",
     'fr': "🚶🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> l&#x27;invitation automatique des utilisateurs au <b>{0}</b> -groupe\n\n👩🏽‍💻 Paramètres de messagerie automatique <b>actuels</b> : {1}",
     'zh': "🚶🏽<b>单击</b>✅/☑️<b>启用/禁用</b>自动邀请用户加入<b>{0}</b> -组\n\n👩🏽‍💻<b>当前</b>自动邮件设置：{1}",
@@ -4841,20 +4498,20 @@
     'en': "{0} source",
     'es': "{0} fuente",
     'fr': "{0} sources",
     'zh': "{0} 个来源",
     'ar': "{0} المصدر",
 }
 l_cinvitechange_handler = {
-    'ru': "🚶🏽 Пришли мне <b>ссылку</b> на группу, откуда будем брать подписчиков\n\n👩🏽‍💻 Например, <code>https://t.me/likeconcentrat</code> - <b>Жми</b> на ссылку, чтобы скопировать",
-    'en': "🚶🏽 Send me <b>a link</b> to the group from where we will take subscribers\n\n👩🏽‍💻 For example, https://t.me/likeconcentrat - <b>Click</b> on the link to copy",
-    'es': "🚶🏽 Envíame <b>un enlace</b> al grupo desde donde tomaremos suscriptores\n\n👩🏽‍💻 Por ejemplo, https://t.me/likeconcentrat - <b>Haz clic</b> en el enlace para copiar",
-    'fr': "🚶🏽 Envoyez-moi <b>un lien</b> vers le groupe d&#x27;où nous prendrons des abonnés\n\n👩🏽‍💻 Par exemple, https://t.me/likeconcentrat - <b>Cliquez</b> sur le lien pour copier",
-    'zh': "🚶🏽 向我发送指向我们将从中接收订阅者的群组<b>的链接</b>\n\n👩🏽‍💻 例如， https://t.me/likeconcentrat -<b>单击</b>链接进行复制",
-    'ar': "🚶🏽 أرسل لي <b>رابطًا</b> للمجموعة التي سنأخذ منها المشتركين\n\n👩🏽‍💻 على سبيل المثال ، https://t.me/likeconcentrat - <b>انقر</b> فوق الارتباط للنسخ",
+    'ru': "🚶🏽 Пришли мне <b>ссылку</b> на группу, откуда будем брать подписчиков\n\n👉🏼 Например, <code>https://t.me/likeconcentrat</code> - <b>Жми</b> на ссылку, чтобы скопировать",
+    'en': "🚶🏽 Send me <b>a link</b> to the group from where we will take subscribers\n\n👉🏼 For example, https://t.me/likeconcentrat - <b>Click</b> on the link to copy",
+    'es': "🚶🏽 Envíame <b>un enlace</b> al grupo desde donde tomaremos suscriptores\n\n👉🏼 Por ejemplo, https://t.me/likeconcentrat - <b>Haz clic</b> en el enlace para copiar",
+    'fr': "🚶🏽 Envoyez-moi <b>un lien</b> vers le groupe d&#x27;où nous prendrons des abonnés\n\n👉🏼 Par exemple, https://t.me/likeconcentrat - <b>Cliquez</b> sur le lien pour copier",
+    'zh': "🚶🏽 向我发送指向我们将从中接收订阅者的群组<b>的链接</b>\n\n👉🏼 例如， https://t.me/likeconcentrat -<b>单击</b>链接进行复制",
+    'ar': "🚶🏽 أرسل لي <b>رابطًا</b> للمجموعة التي سنأخذ منها المشتركين\n\n👉🏼 على سبيل المثال ، https://t.me/likeconcentrat - <b>انقر</b> فوق الارتباط للنسخ",
 }
 l_correct_link = {
     'ru': "👩🏽‍💻 <b>Вставь</b> корректные данные или повтори операцию",
     'en': "👩🏽‍💻 <b>Insert</b> correct data or try again",
     'es': "👩🏽‍💻 <b>Inserta</b> los datos correctos o vuelve a intentarlo",
     'fr': "👩🏽‍💻 <b>Insérez</b> les données correctes ou réessayez",
     'zh': "👩🏽‍💻<b>插入</b>正确的数据或重试",
@@ -5029,20 +4686,20 @@
     'ar': "يختار",
 }
 # endregion
 
 
 # region csystem_
 l_csystem_text = {
-    'ru': "👣 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>системные</i> сообщения\n\n👩🏽‍💻 Например, <i>Пользователь вступил(а) в группу</i>",
-    'en': "👣 <b>Click</b> on ✅/☑️ to turn <i>system</i> messages <b>on/off</b>\n\n👩🏽‍💻 For example, <i>User joined a group</i>",
-    'es': "👣 <b>Haz clic</b> en ✅/☑️ para activar <b>o desactivar</b> los mensajes <i>del sistema</i>\n\n👩🏽‍💻 Por ejemplo, <i>el usuario se unió a un grupo</i>",
-    'fr': "👣 <b>Cliquez</b> sur ✅/☑️ pour activer <b>/désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>l&#x27;utilisateur a rejoint un groupe</i>",
-    'zh': "👣<b>点击</b>✅/☑️ 打开<b>/关闭</b><i>系统</i>消息\n\n👩🏽‍💻 例如，<i>用户加入了一个群组</i>",
-    'ar': "👣 <b>انقر</b> فوق ✅ / ☑️ لتشغيل <b>/ إيقاف</b> تشغيل رسائل <i>النظام</i>\n\n👩🏽‍💻 على سبيل المثال ، <i>انضم المستخدم إلى مجموعة</i>",
+    'ru': "👣 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>системные</i> сообщения\n\n👉🏼 Например, <i>Пользователь вступил(а) в группу</i>",
+    'en': "👣 <b>Click</b> on ✅/☑️ to turn <i>system</i> messages <b>on/off</b>\n\n👉🏼 For example, <i>User joined a group</i>",
+    'es': "👣 <b>Haz clic</b> en ✅/☑️ para activar <b>o desactivar</b> los mensajes <i>del sistema</i>\n\n👉🏼 Por ejemplo, <i>el usuario se unió a un grupo</i>",
+    'fr': "👣 <b>Cliquez</b> sur ✅/☑️ pour activer <b>/désactiver</b> les messages <i>système</i>\n\n👉🏼 Par exemple, <i>l&#x27;utilisateur a rejoint un groupe</i>",
+    'zh': "👣<b>点击</b>✅/☑️ 打开<b>/关闭</b><i>系统</i>消息\n\n👉🏼 例如，<i>用户加入了一个群组</i>",
+    'ar': "👣 <b>انقر</b> فوق ✅ / ☑️ لتشغيل <b>/ إيقاف</b> تشغيل رسائل <i>النظام</i>\n\n👉🏼 على سبيل المثال ، <i>انضم المستخدم إلى مجموعة</i>",
 }
 # endregion
 
 
 # region cchannel_
 l_cchannel_text = {
     'ru': "🫥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>возможность</i> пользователю в группе писать <i>анонимно</i> (от имени <b>его</b> канала)",
@@ -5054,20 +4711,20 @@
 }
 
 # endregion
 
 
 # region clink_
 l_clink_text = {
-    'ru': "🔗 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>внешние <b>ссылки</b>/telegram-<b>ссылки</b>/forward</i>-<b>ссылки</b>\n\n👩🏽‍💻 Например, [✅☑Вкл forward-ссылки] означает разрешение на <b>forward-пересылку</b> сообщений из <u>других</u> Telegram-<i>каналов/групп/аккаунтов</i> в <u>нашу</u> группу",
-    'en': "🔗 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>external <b>links</b> /telegram- <b>links</b> /forward</i> - <b>links</b>\n\n👩🏽‍💻 For example, [✅☑On forward links] means permission to <b>forward</b> messages from <u>other</u> Telegram <i>channels/ groups/accounts</i> to <u>our</u> group",
-    'es': "🔗 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i><b>enlaces</b> externos/ <b>enlaces</b> de Telegram/</i> <b>enlaces</b> de reenvío\n\n👩🏽‍💻 Por ejemplo, [✅☑En enlaces de reenvío] significa permiso para <b>reenviar</b> mensajes de <u>otros</u> <i>canales/grupos/cuentas</i> de Telegram a <u>nuestro</u> grupo",
-    'fr': "🔗 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i><b>les liens</b> externes/telegram- <b>links</b> /forward</i> - <b>links</b>\n\n👩🏽‍💻 Par exemple, [✅☑On forward links] signifie l&#x27;autorisation de <b>transférer</b> des messages d&#x27; <u>autres</u> <i>chaînes/groupes/comptes</i> Telegram vers <u>notre</u> groupe",
-    'zh': "🔗<b>点击</b>✅/☑️<b>启用/禁用</b><i>外部<b>链接</b>/telegram- <b>links</b> /forward-</i> <b>links</b>\n\n👩🏽‍💻 例如，[✅☑On forward links] 表示允许将来自<u>其他</u>Telegram<i>频道/组/帐户的</i>消息<b>转发到</b><u>我们</u>组",
-    'ar': "🔗 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i><b>الروابط</b> الخارجية / <b>روابط</b> التلغرام / إعادة التوجيه</i> - <b>الروابط</b>\n\n👩🏽‍💻 على سبيل المثال ، [✅☑عند توجيه الروابط] يعني الإذن بإعادة <b>توجيه</b> الرسائل من <i>قنوات / مجموعات / حسابات</i> Telegram <u>الأخرى</u> إلى <u>مجموعتنا</u>",
+    'ru': "🔗 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>внешние <b>ссылки</b>/telegram-<b>ссылки</b>/forward</i>-<b>ссылки</b>\n\n👉🏼 Например, [✅☑Вкл forward-ссылки] означает разрешение на <b>forward-пересылку</b> сообщений из <u>других</u> Telegram-<i>каналов/групп/аккаунтов</i> в <u>нашу</u> группу",
+    'en': "🔗 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>external <b>links</b> /telegram- <b>links</b> /forward</i> - <b>links</b>\n\n👉🏼 For example, [✅☑On forward links] means permission to <b>forward</b> messages from <u>other</u> Telegram <i>channels/ groups/accounts</i> to <u>our</u> group",
+    'es': "🔗 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i><b>enlaces</b> externos/ <b>enlaces</b> de Telegram/</i> <b>enlaces</b> de reenvío\n\n👉🏼 Por ejemplo, [✅☑En enlaces de reenvío] significa permiso para <b>reenviar</b> mensajes de <u>otros</u> <i>canales/grupos/cuentas</i> de Telegram a <u>nuestro</u> grupo",
+    'fr': "🔗 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i><b>les liens</b> externes/telegram- <b>links</b> /forward</i> - <b>links</b>\n\n👉🏼 Par exemple, [✅☑On forward links] signifie l&#x27;autorisation de <b>transférer</b> des messages d&#x27; <u>autres</u> <i>chaînes/groupes/comptes</i> Telegram vers <u>notre</u> groupe",
+    'zh': "🔗<b>点击</b>✅/☑️<b>启用/禁用</b><i>外部<b>链接</b>/telegram- <b>links</b> /forward-</i> <b>links</b>\n\n👉🏼 例如，[✅☑On forward links] 表示允许将来自<u>其他</u>Telegram<i>频道/组/帐户的</i>消息<b>转发到</b><u>我们</u>组",
+    'ar': "🔗 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i><b>الروابط</b> الخارجية / <b>روابط</b> التلغرام / إعادة التوجيه</i> - <b>الروابط</b>\n\n👉🏼 على سبيل المثال ، [✅☑عند توجيه الروابط] يعني الإذن بإعادة <b>توجيه</b> الرسائل من <i>قنوات / مجموعات / حسابات</i> Telegram <u>الأخرى</u> إلى <u>مجموعتنا</u>",
 }
 l_clink_http_on = {
     'ru': "✅☑Вкл внешние-ссылки",
     'en': "✅☑Include external-links",
     'es': "✅☑Incluir enlaces externos",
     'fr': "✅☑Inclure des liens externes",
     'zh': "✅☑包括外部链接",
@@ -5114,64 +4771,64 @@
     'ar': "☑️☐ تعطيل الروابط الأمامية",
 }
 # endregion
 
 
 # region csymbol_
 l_csymbol_text = {
-    'ru': "文 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> разрешение на слова с <i>文-глиф, ب-араб/<a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👩🏽‍💻 Например, <b>zalgo</b> опция разрешает сообщения такого вида: <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
-    'en': "<b>Text</b> to ✅/☑️ to <b>enable/disable</b> <u>auto</u> -ban <i>for words with glyphs, Arabic/</i> <i>zalgo-symbols</i>\n\n👩🏽‍💻 For example, the <b>zalgo-ban</b> option removes messages like this <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
-    'es': "Envía <b>un mensaje de texto</b> a ✅/☑️ para <b>activar/desactivar</b> la prohibición <u>automática</u> <i>de palabras con glifos,</i> <i>símbolos árabes/zalgo</i>\n\n👩🏽‍💻 Por ejemplo, la opción <b>de prohibición de zalgo</b> elimina mensajes como este <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆ ̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
-    'fr': "<b>Envoyez un SMS</b> à ✅/☑️ pour <b>activer/désactiver</b> l&#x27;interdiction <u>automatique</u> <i>des mots avec des glyphes,</i> <i>des symboles arabes/zalgo</i>\n\n👩🏽‍💻 Par exemple, l&#x27;option <b>zalgo-ban</b> supprime les messages comme celui-ci <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏ ͆̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
-    'zh': "向 ✅/☑️<b>发送文本</b>以<b>启用/禁用</b><i>带有字形、阿拉伯语/</i> <i>zalgo 符号</i>的单词的<u>自动</u>禁止\n\n👩🏽‍💻 例如， <b>zalgo-ban</b>选项会删除以下类型的消息<i>：̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́ ̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̐̐͛̾́͗̈́̚͝͝͝</i>",
-    'ar': "أرسل <b>رسالة نصية</b> إلى ✅ / ☑️ <b>لتمكين / تعطيل</b> الحظر <u>التلقائي</u> <i>للكلمات ذات الحروف الرسومية والعربية /</i> <i>رموز zalgo</i>\n\n👩🏽‍💻 على سبيل المثال ، يزيل خيار <b>zalgo-ban</b> رسائل مثل هذه <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
+    'ru': "文 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>слов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>zalgo-бан</b> удаляет сообщения такого вида <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
+    'en': "<b>Text</b> to ✅/☑️ to <b>enable/disable</b> <u>auto</u> -ban <i>for words with glyphs, Arabic/</i> <i>zalgo-symbols</i>\n\n👉🏼 For example, the <b>zalgo-ban</b> option removes messages like this <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
+    'es': "Envía <b>un mensaje de texto</b> a ✅/☑️ para <b>activar/desactivar</b> la prohibición <u>automática</u> <i>de palabras con glifos,</i> <i>símbolos árabes/zalgo</i>\n\n👉🏼 Por ejemplo, la opción <b>de prohibición de zalgo</b> elimina mensajes como este <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆ ̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
+    'fr': "<b>Envoyez un SMS</b> à ✅/☑️ pour <b>activer/désactiver</b> l&#x27;interdiction <u>automatique</u> <i>des mots avec des glyphes,</i> <i>des symboles arabes/zalgo</i>\n\n👉🏼 Par exemple, l&#x27;option <b>zalgo-ban</b> supprime les messages comme celui-ci <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏ ͆̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
+    'zh': "向 ✅/☑️<b>发送文本</b>以<b>启用/禁用</b><i>带有字形、阿拉伯语/</i> <i>zalgo 符号</i>的单词的<u>自动</u>禁止\n\n👉🏼 例如， <b>zalgo-ban</b>选项会删除以下类型的消息<i>：̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́ ̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̐̐͛̾́͗̈́̚͝͝͝</i>",
+    'ar': "أرسل <b>رسالة نصية</b> إلى ✅ / ☑️ <b>لتمكين / تعطيل</b> الحظر <u>التلقائي</u> <i>للكلمات ذات الحروف الرسومية والعربية /</i> <i>رموز zalgo</i>\n\n👉🏼 على سبيل المثال ، يزيل خيار <b>zalgo-ban</b> رسائل مثل هذه <i>̢̥l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶̒͗͐͝ ͍̼͎͈̬̩̩̰̱͙̐̐͛̾́͗̈́̚͝͝</i>",
 }
 l_csymbol_symbols_on = {
-    'ru': "✅☑Вкл 文ب",
-    'en': "✅☑Incl. 文ب",
+    'ru': "✅☑Вкл 文ب-бан",
+    'en': "✅☑Incl. 文ب-ban",
     'es': "✅☑Incl. 文ب-prohibición",
     'fr': "✅☑Y compris 文ب-interdiction",
     'zh': "✅☑包括文Ho禁令",
     'ar': "✅☑Incl. 文 ب- الحظر",
 }
 l_csymbol_symbols_off = {
-    'ru': "☑️☐Выкл 文ب",
+    'ru': "☑️☐Выкл 文ب-бан",
     'en': "☑️☐Выкл 文ب-бан",
     'es': "☑️☐Выкл 文ب-бан",
     'fr': "☑️☐Выкл 文ب-бан",
     'zh': "☑️☐Выкл 文ب-бан",
     'ar': "☑️☐Выкл 文 ب- бан",
 }
 l_csymbol_zalgo_on = {
-    'ru': "✅☑Вкл zalgo",
+    'ru': "✅☑Вкл zalgo-бан",
     'en': "✅☑Incl. pledge-ban",
     'es': "✅☑Incl. prohibición de compromiso",
     'fr': "✅☑Incl.",
     'zh': "✅☑包括质押禁令",
     'ar': "✅☑Incl. تعهد الحظر",
 }
 l_csymbol_zalgo_off = {
-    'ru': "☑️☐Выкл zalgo",
+    'ru': "☑️☐Выкл zalgo-бан",
     'en': "☑️☐Vykl pledge-ban",
     'es': "☑️☐ Prohibición de compromiso de Vykl",
     'fr': "☑️☐Vykl pledge-ban",
     'zh': "☑️☐Vykl 质押禁令",
     'ar': "Vykl تعهد الحظر",
 }
 # endregion
 
 
 # region cmedia_
 l_cmedia_text = {
-    'ru': "🗣 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> разрешение на <i>media</i>-сообщения\n\n👩🏽‍💻 Например, [☑️☐Выкл видео-заметки] означает запрет на <b>видео-заметки в кружочке</b> в нашей группе\n\n👩🏽‍💻 Чтобы разрешить/запретить конкретный стикерпак, жми [⚙️Настроить]",
-    'en': "🗣 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> permission for <i>media</i> messages\n\n👩🏽‍💻 For example, [☑️☐Disable video notes] means no <b>video notes in a circle</b> in our group\n\n👩🏽‍💻 To allow/deny a specific sticker pack, press [⚙️Customize]",
-    'es': "🗣 <b>Haz clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> el permiso para mensajes <i>multimedia</i>\n\n👩🏽‍💻 Por ejemplo, [☑️☐Deshabilitar notas de video] significa que no hay <b>notas de video en un círculo</b> en nuestro grupo\n\n👩🏽‍💻 Para permitir/denegar un paquete de calcomanías específico, presiona [⚙️Personalizar]",
-    'fr': "🗣 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> l&#x27;autorisation des messages <i>multimédias</i>\n\n👩🏽‍💻 Par exemple, [☑️☐Désactiver les notes vidéo] signifie qu&#x27;il n&#x27;y a pas <b>de notes vidéo dans un cercle</b> dans notre groupe\n\n👩🏽‍💻 Autoriser/refuser un pack d'autocollants spécifique, appuyez sur [⚙️Personnaliser]",
-    'zh': "🗣<b>点击</b>✅/☑️<b>开启/关闭</b><i>媒体</i>消息权限\n\n👩🏽‍💻 例如，[☑️☐ 关闭视频笔记] 表示我们群里的<b>圈子里没有视频笔记</b>\n\n👩🏽‍💻 允许/拒绝一个特定的贴纸包，按[⚙️Customize]",
-    'ar': "🗣 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> الإذن لرسائل <i>الوسائط</i>\n\n👩🏽‍💻 على سبيل المثال ، يعني [☑️☐ تعطيل ملاحظات الفيديو] عدم وجود <b>ملاحظات فيديو في دائرة</b> في مجموعتنا\n\n👩🏽‍💻 للسماح / الرفض حزمة ملصقات محددة ، اضغط على [تخصيص]",
+    'ru': "🗣 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> разрешение на <i>media</i>-сообщения\n\n👉🏼 Например, [☑️☐Выкл видео-заметки] означает запрет на <b>видео-заметки в кружочке</b> в нашей группе\n\n👉🏼 Чтобы разрешить/запретить конкретный стикерпак, жми [⚙️Настроить]",
+    'en': "🗣 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> permission for <i>media</i> messages\n\n👉🏼 For example, [☑️☐Disable video notes] means no <b>video notes in a circle</b> in our group\n\n👉🏼 To allow/deny a specific sticker pack, press [⚙️Customize]",
+    'es': "🗣 <b>Haz clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> el permiso para mensajes <i>multimedia</i>\n\n👉🏼 Por ejemplo, [☑️☐Deshabilitar notas de video] significa que no hay <b>notas de video en un círculo</b> en nuestro grupo\n\n👉🏼 Para permitir/denegar un paquete de calcomanías específico, presiona [⚙️Personalizar]",
+    'fr': "🗣 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> l&#x27;autorisation des messages <i>multimédias</i>\n\n👉🏼 Par exemple, [☑️☐Désactiver les notes vidéo] signifie qu&#x27;il n&#x27;y a pas <b>de notes vidéo dans un cercle</b> dans notre groupe\n\n👉🏼 Autoriser/refuser un pack d'autocollants spécifique, appuyez sur [⚙️Personnaliser]",
+    'zh': "🗣<b>点击</b>✅/☑️<b>开启/关闭</b><i>媒体</i>消息权限\n\n👉🏼 例如，[☑️☐ 关闭视频笔记] 表示我们群里的<b>圈子里没有视频笔记</b>\n\n👉🏼 允许/拒绝一个特定的贴纸包，按[⚙️Customize]",
+    'ar': "🗣 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> الإذن لرسائل <i>الوسائط</i>\n\n👉🏼 على سبيل المثال ، يعني [☑️☐ تعطيل ملاحظات الفيديو] عدم وجود <b>ملاحظات فيديو في دائرة</b> في مجموعتنا\n\n👉🏼 للسماح / الرفض حزمة ملصقات محددة ، اضغط على [تخصيص]",
 }
 l_cmedia_photo_on = {
     'ru': "✅☑Вкл photo",
     'en': "✅☑Photo included",
     'es': "✅☑Foto incluida",
     'fr': "✅☑Photo incluse",
     'zh': "✅附照片",
@@ -5438,20 +5095,20 @@
     'en': "🦊 Current number of <b>banned</b> sticker packs: <u>{0}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> banned sticker packs",
     'es': "🦊 Número actual de paquetes de pegatinas <b>prohibidos</b> : <u>{0}</u>\n\n<b>Haz clic</b> en ✅/🚫 para <b>agregar o quitar</b> paquetes de pegatinas prohibidos",
     'fr': "🦊 Nombre actuel de packs d'autocollants <b>interdits</b> : <u>{0}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des packs d'autocollants interdits",
     'zh': "🦊 当前<b>禁止的</b>贴纸包数量： <u>{0}</u>\n\n<b>点击</b>✅/🚫<b>添加/删除</b>禁止的贴纸包",
     'ar': "🦊 العدد الحالي لحزم الملصقات <b>المحظورة</b> : <u>{0}</u>\n\n<b>انقر</b> فوق ✅ / 🚫 <b>لإضافة / إزالة</b> حزم الملصقات المحظورة",
 }
 l_cstickeroperation_add = {
-    'ru': "\n\n👩🏽‍💻 Например, https://t.me/addstickers/HotCherry или HotCherry",
-    'en': "\n\n👩🏽‍💻 For example, https://t.me/addstickers/HotCherry or HotCherry",
-    'es': "\n\n👩🏽‍💻 Por ejemplo, https://t.me/addstickers/HotCherry o HotCherry",
-    'fr': "\n\n👩🏽‍💻 Par exemple, https://t.me/addstickers/HotCherry ou HotCherry",
-    'zh': "\n\n👩🏽‍💻 例如， https://t.me/addstickers/HotCherry或HotCherry",
-    'ar': "\n\n👩🏽‍💻 على سبيل المثال ، https://t.me/addstickers/HotCherry أو HotCherry",
+    'ru': "\n\n👉🏼 Например, https://t.me/addstickers/HotCherry или HotCherry",
+    'en': "\n\n👉🏼 For example, https://t.me/addstickers/HotCherry or HotCherry",
+    'es': "\n\n👉🏼 Por ejemplo, https://t.me/addstickers/HotCherry o HotCherry",
+    'fr': "\n\n👉🏼 Par exemple, https://t.me/addstickers/HotCherry ou HotCherry",
+    'zh': "\n\n👉🏼 例如， https://t.me/addstickers/HotCherry或HotCherry",
+    'ar': "\n\n👉🏼 على سبيل المثال ، https://t.me/addstickers/HotCherry أو HotCherry",
 }
 l_cstickeroperation_isadd = {
     'ru': "✅ Пришли ссылку или имя <b>стикерпака</b>, чтобы <b>добавить</b> его в список разрешенных{0}",
     'en': "✅ Sent a link or <b>sticker pack</b> name to <b>add</b> it to the allowed list{0}",
     'es': "✅ Envió un enlace o nombre <b>de paquete de calcomanías</b> para <b>agregarlo</b> a la lista permitida{0}",
     'fr': "✅ Envoyé un lien ou un nom <b>de pack d&#x27;autocollants</b> pour l&#x27; <b>ajouter</b> à la liste autorisée{0}",
     'zh': "✅ 发送链接或<b>贴纸包</b>名称以将其<b>添加</b>到允许列表{0}",
@@ -5490,20 +5147,20 @@
     'ar': "🦊 <b>انتهى!</b> <b>استثناءات</b> حزمة الملصقات:\n\n+ المسموح بها: <u>{0}</u>\n- ممنوع: <u>{1}</u>\n\n[✅ Allow] يتخطى حزم الملصقات المحددة <i>كاستثناء</i> عند تحديد الخيار [☑️☐ Off sticker]\nيؤدي [🚫 Deny] إلى تعطيل حزم الملصقات المحددة <i>كاستثناء</i> عند تحديد خيار [تمكين الملصق]",
 }
 # endregion
 
 
 # region cstart_
 l_cstart_text = {
-    'ru': "🚀 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-ответ на триггер-сообщения, содержащие конкретные старт-слова\n\n👩🏽‍💻 <b>Текущее</b> количество старт-слов <u>{0}</u>",
-    'en': "🚀 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to trigger messages containing specific start words\n\n👩🏽‍💻 <b>Current</b> number of start words <u>{0}</u>",
-    'es': "🚀 <b>Presiona</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática para activar mensajes que contengan palabras de inicio específicas\n\n👩🏽‍💻 Número <b>actual</b> de palabras de inicio <u>{0}</u>",
-    'fr': "🚀 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique afin de déclencher des messages contenant des mots de départ spécifiques\n\n👩🏽‍💻 Nombre <b>actuel</b> de mots de départ <u>{0}</u>",
+    'ru': "🚀 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-ответ на триггер-сообщения, содержащие конкретные старт-слова\n\n👉🏼 <b>Текущее</b> количество старт-слов <u>{0}</u>",
+    'en': "🚀 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to trigger messages containing specific start words\n\n👉🏼 <b>Current</b> number of start words <u>{0}</u>",
+    'es': "🚀 <b>Presiona</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática para activar mensajes que contengan palabras de inicio específicas\n\n👉🏼 Número <b>actual</b> de palabras de inicio <u>{0}</u>",
+    'fr': "🚀 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique afin de déclencher des messages contenant des mots de départ spécifiques\n\n👉🏼 Nombre <b>actuel</b> de mots de départ <u>{0}</u>",
     'zh': "🚀<b>按</b>✅/☑️<b>打开/关闭</b>自动回复以触发包含特定起始词的消息\n\n👉🏼<b>当前</b>起始词数<u>{0}</u>",
-    'ar': "🚀 <b>اضغط على</b> ✅ / ☑️ <b>لتشغيل / إيقاف</b> الرد التلقائي لتشغيل الرسائل التي تحتوي على كلمات بداية محددة\n\n👩🏽‍💻 العدد <b>الحالي</b> لكلمات البداية <u>{0}</u>",
+    'ar': "🚀 <b>اضغط على</b> ✅ / ☑️ <b>لتشغيل / إيقاف</b> الرد التلقائي لتشغيل الرسائل التي تحتوي على كلمات بداية محددة\n\n👉🏼 العدد <b>الحالي</b> لكلمات البداية <u>{0}</u>",
 }
 l_cstart_call = {
     'ru': "🔔 Нужно ⚙️Настроить хотя бы одно старт-слово",
     'en': "🔔 You need to ⚙️Set up at least one start-word",
     'es': "🔔 Necesitas ⚙️Configurar al menos una palabra de inicio",
     'fr': "🔔 Vous devez ⚙️Configurer au moins un mot de départ",
     'zh': "🔔 你需要⚙️设置至少一个起始词",
@@ -5514,20 +5171,20 @@
     'en': "🚀 You need to ⚙️Set up at least one post via the 🔔Auto-posting option",
     'es': "🚀 Necesitas ⚙️Configurar al menos una publicación a través de la opción 🔔Publicación automática",
     'fr': "🚀 Vous devez ⚙️Configurer au moins une publication via l'option 🔔Publication automatique",
     'zh': "🚀 您需要⚙️通过🔔自动发布选项设置至少一个帖子",
     'ar': "🚀 تحتاج إلى إعداد منشور واحد على الأقل عبر خيار 'النشر التلقائي'",
 }
 l_cstartconfig_text = {
-    'ru': "🚀 <b>Выбери пост</b>, который будет присылаться в ответ на <b>старт</b>-слова и жми [🚀 <b>Использовать</b>] под выбранным постом\n\n👩🏽‍💻 Общее количество старт-слов: <u>{0}</u>",
-    'en': "🚀 <b>Select the post</b> that will be sent in response to <b>start</b> -words and click [🚀 <b>Use</b>] under the selected post\n\n👩🏽‍💻 Total number of start-words: <u>{0}</u>",
-    'es': "🚀 <b>Selecciona la publicación</b> que se enviará en respuesta a las palabras <b>iniciales</b> y haz clic en [🚀 <b>Usar</b>] debajo de la publicación seleccionada\n\n👩🏽‍💻 Número total de palabras iniciales: <u>{0}</u>",
-    'fr': "🚀 <b>Sélectionnez la publication</b> qui sera envoyée en réponse aux mots <b>de départ</b> et cliquez sur [🚀 <b>Utiliser</b>] sous la publication sélectionnée\n\n👩🏽‍💻 Nombre total de mots de départ : <u>{0}</u>",
-    'zh': "🚀<b>选择要发送的帖子</b>以响应<b>起始</b>词，然后单击所选帖子下的 [🚀<b>使用</b>]\n\n👩🏽‍💻 起始词总数： <u>{0}</u>",
-    'ar': "🚀 <b>حدد المنشور</b> الذي سيتم إرساله استجابةً لكلمات <b>البدء</b> وانقر فوق [🚀 <b>Use</b>] ضمن المنشور المحدد\n\n👩🏽‍💻 إجمالي عدد كلمات البداية: <u>{0}</u>",
+    'ru': "🚀 <b>Выбери пост</b>, который будет присылаться в ответ на <b>старт</b>-слова и жми [🚀 <b>Использовать</b>] под выбранным постом\n\n👉🏼 Общее количество старт-слов: <u>{0}</u>",
+    'en': "🚀 <b>Select the post</b> that will be sent in response to <b>start</b> -words and click [🚀 <b>Use</b>] under the selected post\n\n👉🏼 Total number of start-words: <u>{0}</u>",
+    'es': "🚀 <b>Selecciona la publicación</b> que se enviará en respuesta a las palabras <b>iniciales</b> y haz clic en [🚀 <b>Usar</b>] debajo de la publicación seleccionada\n\n👉🏼 Número total de palabras iniciales: <u>{0}</u>",
+    'fr': "🚀 <b>Sélectionnez la publication</b> qui sera envoyée en réponse aux mots <b>de départ</b> et cliquez sur [🚀 <b>Utiliser</b>] sous la publication sélectionnée\n\n👉🏼 Nombre total de mots de départ : <u>{0}</u>",
+    'zh': "🚀<b>选择要发送的帖子</b>以响应<b>起始</b>词，然后单击所选帖子下的 [🚀<b>使用</b>]\n\n👉🏼 起始词总数： <u>{0}</u>",
+    'ar': "🚀 <b>حدد المنشور</b> الذي سيتم إرساله استجابةً لكلمات <b>البدء</b> وانقر فوق [🚀 <b>Use</b>] ضمن المنشور المحدد\n\n👉🏼 إجمالي عدد كلمات البداية: <u>{0}</u>",
 }
 l_cstartconfig_use = {
     'ru': "🚀 Использовать",
     'en': "🚀 Use",
     'es': "🚀 Uso",
     'fr': "🚀 Utiliser",
     'zh': "🚀 使用",
@@ -5599,20 +5256,20 @@
 }
 
 # endregion
 
 
 # region cstop_
 l_cstop_text = {
-    'ru': "🧾 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-удаление сообщений, содержащие запрещенные стоп-слова\n\n👩🏽‍💻 <b>Текущее</b> количество стоп-слов <u>{0}</u>",
-    'en': "🧾 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> auto-delete messages containing banned stop words\n\n👩🏽‍💻 <b>Current</b> number of stop words <u>{0}</u>",
-    'es': "🧾 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> la eliminación automática de mensajes que contienen palabras vacías prohibidas\n\n👩🏽‍💻 Número <b>actual</b> de palabras vacías <u>{0}</u>",
-    'fr': "🧾 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> la suppression automatique des messages contenant des mots vides interdits\n\n👩🏽‍💻 Nombre <b>actuel</b> de mots vides <u>{0}</u>",
+    'ru': "🧾 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-удаление сообщений, содержащие запрещенные стоп-слова\n\n👉🏼 <b>Текущее</b> количество стоп-слов <u>{0}</u>",
+    'en': "🧾 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> auto-delete messages containing banned stop words\n\n👉🏼 <b>Current</b> number of stop words <u>{0}</u>",
+    'es': "🧾 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> la eliminación automática de mensajes que contienen palabras vacías prohibidas\n\n👉🏼 Número <b>actual</b> de palabras vacías <u>{0}</u>",
+    'fr': "🧾 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> la suppression automatique des messages contenant des mots vides interdits\n\n👉🏼 Nombre <b>actuel</b> de mots vides <u>{0}</u>",
     'zh': "🧾<b>点击</b>✅/☑️<b>打开/关闭</b>自动删除包含禁止停用词的消息\n\n👉🏼<b>当前</b>停用词数量<u>{0}</u>",
-    'ar': "🧾 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف</b> تشغيل الحذف التلقائي للرسائل التي تحتوي على كلمات إيقاف محظورة\n\n👩🏽‍💻 العدد <b>الحالي</b> لكلمات الإيقاف <u>{0}</u>",
+    'ar': "🧾 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف</b> تشغيل الحذف التلقائي للرسائل التي تحتوي على كلمات إيقاف محظورة\n\n👉🏼 العدد <b>الحالي</b> لكلمات الإيقاف <u>{0}</u>",
 }
 l_cstop_call = {
     'ru': "🔔 Нужно ⚙️Настроить хотя бы одно стоп-слово",
     'en': "🔔 You must ⚙️Set up at least one stop word",
     'es': "🔔 Debes ⚙️Configurar al menos una palabra vacía",
     'fr': "🔔 Vous devez ⚙️Configurer au moins un mot vide",
     'zh': "🔔 你必须⚙️设置至少一个停用词",
@@ -5675,20 +5332,20 @@
     'ar': "🧾 <b>انتهى!</b> العدد <b>الحالي</b> لكلمات التوقف <u>{0}</u>",
 }
 # endregion
 
 
 # region cflood_
 l_cflood_text = {
-    'ru': "💬 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>проверку</i> на частоту подряд написанных сообщ за один промежуток времени\n\n👩🏽‍💻 Например, задай количество сообщ подряд, которое будет считаться флудом командой: /flood 5\n\n👩🏽‍💻 Или используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
-    'en': "💬 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> <i>the check</i> for the frequency of consecutive messages written in one period of time\n\n👩🏽‍💻 For example, set the number of messages in a row that will be considered a flood with the command: /flood 5\n\n👩🏽‍💻 Or use <b>slow mode</b> in group settings for <u>1</u> message",
-    'es': "💬 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <i>la verificación</i> de la frecuencia de mensajes consecutivos escritos en un período de tiempo\n\n👩🏽‍💻 Por ejemplo, establece la cantidad de mensajes seguidos que se considerarán una inundación con el comando: /flood 5\n\n👩🏽‍💻 O usa <b>el modo lento</b> en la configuración del grupo para <u>1</u> mensaje",
-    'fr': "💬 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>la vérification</i> de la fréquence des messages consécutifs écrits dans une période de temps\n\n👩🏽‍💻 Par exemple, définissez le nombre de messages consécutifs qui seront considérés comme une inondation avec le commande : /flood 5\n\n👩🏽‍💻 Ou utilisez <b>le mode lent</b> dans les paramètres de groupe pour <u>1</u> message",
-    'zh': "💬<b>点击</b>✅/☑️<b>开启/关闭</b><i>检查</i>一段时间内连续写入消息的频率\n\n👩🏽‍💻 例如，设置连续消息的数量将被视为洪水命令： /flood 5\n\n👩🏽‍💻 或者在组设置中使用<b>慢速模式</b>发送<u>1 条</u>消息",
-    'ar': "💬 <b>انقر</b> فوق ✅ / ☑️ لتشغيل <b>/ إيقاف تشغيل</b> <i>التحقق</i> من تكرار الرسائل المتتالية المكتوبة في فترة زمنية واحدة\n\n👩🏽‍💻 على سبيل المثال ، قم بتعيين عدد الرسائل في الصف الذي سيتم اعتباره فيضانًا مع الأمر: /flood 5\n\n👩🏽‍💻 أو استخدم <b>الوضع البطيء</b> في إعدادات المجموعة لرسالة <u>واحدة</u>",
+    'ru': "💬 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>проверку</i> на частоту подряд написанных сообщ за один промежуток времени\n\n👉🏼 Например, задай количество сообщ подряд, которое будет считаться флудом командой: /flood 5\n\n👉🏼 Или используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
+    'en': "💬 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> <i>the check</i> for the frequency of consecutive messages written in one period of time\n\n👉🏼 For example, set the number of messages in a row that will be considered a flood with the command: /flood 5\n\n👉🏼 Or use <b>slow mode</b> in group settings for <u>1</u> message",
+    'es': "💬 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <i>la verificación</i> de la frecuencia de mensajes consecutivos escritos en un período de tiempo\n\n👉🏼 Por ejemplo, establece la cantidad de mensajes seguidos que se considerarán una inundación con el comando: /flood 5\n\n👉🏼 O usa <b>el modo lento</b> en la configuración del grupo para <u>1</u> mensaje",
+    'fr': "💬 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>la vérification</i> de la fréquence des messages consécutifs écrits dans une période de temps\n\n👉🏼 Par exemple, définissez le nombre de messages consécutifs qui seront considérés comme une inondation avec le commande : /flood 5\n\n👉🏼 Ou utilisez <b>le mode lent</b> dans les paramètres de groupe pour <u>1</u> message",
+    'zh': "💬<b>点击</b>✅/☑️<b>开启/关闭</b><i>检查</i>一段时间内连续写入消息的频率\n\n👉🏼 例如，设置连续消息的数量将被视为洪水命令： /flood 5\n\n👉🏼 或者在组设置中使用<b>慢速模式</b>发送<u>1 条</u>消息",
+    'ar': "💬 <b>انقر</b> فوق ✅ / ☑️ لتشغيل <b>/ إيقاف تشغيل</b> <i>التحقق</i> من تكرار الرسائل المتتالية المكتوبة في فترة زمنية واحدة\n\n👉🏼 على سبيل المثال ، قم بتعيين عدد الرسائل في الصف الذي سيتم اعتباره فيضانًا مع الأمر: /flood 5\n\n👉🏼 أو استخدم <b>الوضع البطيء</b> في إعدادات المجموعة لرسالة <u>واحدة</u>",
 }
 l_cflood_count_on = {
     'ru': "✅☑Вкл {0} сообщ",
     'en': "✅☑On {0} messages",
     'es': "✅☑En {0} mensajes",
     'fr': "✅☑Sur {0} messages",
     'zh': "✅☑关于 {0} 条消息",
@@ -5703,20 +5360,20 @@
     'ar': "☑️☐ إيقاف {0} الرسائل",
 }
 # endregion
 
 
 # region cuser_
 l_cuser_text = {
-    'ru': "👥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> первичную <i>задержку/свободный вход без входного контроля для premium-аккаунтов/разрешение на инвайт</i> пользователей/ботов в группу или разрешение на <i>редактирование</i> сообщений\n\n👩🏽‍💻 Например, <b>задержка</b> (<i>в мин</i>) для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) осуществляется командой: /delay  {0}",
-    'en': "👥 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> initial <i>delay/free entry without input control for premium accounts/permission to invite</i> users/bots to the group or permission to <i>edit</i> messages\n\n👩🏽‍💻 For example, <b>delay</b> ( <i>in min</i> ) for <u>new</u> users (before writing their <u>1st</u> message) is done with the command: /delay {0}",
-    'es': "👥 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <i>el retraso inicial/entrada gratuita sin control de entrada para cuentas premium/permiso para invitar</i> usuarios/bots al grupo o permiso para <i>editar</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <b>retraso</b> ( <i>en minutos</i> ) para <u>nuevos</u> usuarios (antes de escribir su <u>primer</u> mensaje) se hace con el comando: /delay {0}",
-    'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>le délai initial/entrée libre sans contrôle de saisie pour les comptes premium/autorisation d&#x27;inviter</i> des utilisateurs/bots dans le groupe ou autorisation de <i>modifier</i> des messages\n\n👩🏽‍💻 Par exemple, <b>délai</b> ( <i>en min</i> ) pour <u>les nouveaux</u> utilisateurs (avant d&#x27;écrire leur <u>1er</u> message) se fait avec la commande : /delay {0}",
-    'zh': "👥<b>点击</b>✅/☑️<b>启用/禁用</b>初始<i>延迟/免费进入高级帐户没有输入控制/允许邀请</i>用户/机器人加入组或允许<i>编辑</i>消息\n\n👩🏽‍💻 例如，<b>延迟</b>（<i>以分钟为单位</i>）对于<u>新</u>用户（在写他们的<u>第一条</u>消息之前）是用命令完成的： /delay {0}",
-    'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>التأخير الأولي / الإدخال المجاني بدون التحكم في الإدخال للحسابات المتميزة / إذن لدعوة</i> المستخدمين / الروبوتات إلى المجموعة أو الإذن <i>لتحرير</i> الرسائل\n\n👩🏽‍💻 على سبيل المثال ، <b>تأخير</b> ( <i>بالدقائق</i> ) للمستخدمين <u>الجدد</u> (قبل كتابة رسالتهم <u>الأولى</u> ) يتم باستخدام الأمر: /delay {0}",
+    'ru': "👥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> первичную <i>задержку/свободный вход без входного контроля для premium-аккаунтов/разрешение на инвайт</i> пользователей/ботов в группу или разрешение на <i>редактирование</i> сообщений\n\n👉🏼 Например, <b>задержка</b> (<i>в мин</i>) для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) осуществляется командой: /delay  {0}",
+    'en': "👥 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> initial <i>delay/free entry without input control for premium accounts/permission to invite</i> users/bots to the group or permission to <i>edit</i> messages\n\n👉🏼 For example, <b>delay</b> ( <i>in min</i> ) for <u>new</u> users (before writing their <u>1st</u> message) is done with the command: /delay {0}",
+    'es': "👥 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <i>el retraso inicial/entrada gratuita sin control de entrada para cuentas premium/permiso para invitar</i> usuarios/bots al grupo o permiso para <i>editar</i> mensajes\n\n👉🏼 Por ejemplo, <b>retraso</b> ( <i>en minutos</i> ) para <u>nuevos</u> usuarios (antes de escribir su <u>primer</u> mensaje) se hace con el comando: /delay {0}",
+    'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>le délai initial/entrée libre sans contrôle de saisie pour les comptes premium/autorisation d&#x27;inviter</i> des utilisateurs/bots dans le groupe ou autorisation de <i>modifier</i> des messages\n\n👉🏼 Par exemple, <b>délai</b> ( <i>en min</i> ) pour <u>les nouveaux</u> utilisateurs (avant d&#x27;écrire leur <u>1er</u> message) se fait avec la commande : /delay {0}",
+    'zh': "👥<b>点击</b>✅/☑️<b>启用/禁用</b>初始<i>延迟/免费进入高级帐户没有输入控制/允许邀请</i>用户/机器人加入组或允许<i>编辑</i>消息\n\n👉🏼 例如，<b>延迟</b>（<i>以分钟为单位</i>）对于<u>新</u>用户（在写他们的<u>第一条</u>消息之前）是用命令完成的： /delay {0}",
+    'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>التأخير الأولي / الإدخال المجاني بدون التحكم في الإدخال للحسابات المتميزة / إذن لدعوة</i> المستخدمين / الروبوتات إلى المجموعة أو الإذن <i>لتحرير</i> الرسائل\n\n👉🏼 على سبيل المثال ، <b>تأخير</b> ( <i>بالدقائق</i> ) للمستخدمين <u>الجدد</u> (قبل كتابة رسالتهم <u>الأولى</u> ) يتم باستخدام الأمر: /delay {0}",
 }
 l_cuser_call = {
     'ru': "👮🏽 В настройках [Разрешения] включи опцию:\n\n[✅ Добавление участ]\n\n🕚Подожди 1min",
     'en': "👮🏽 In the [Permissions] settings, enable the option:\n\n[✅ Adding a part]\n\n🕚Wait 1min",
     'es': "👮🏽 En la configuración de [Permisos], habilita la opción:\n\n[✅ Agregar una parte]\n\n🕚Espera 1 minuto",
     'fr': "👮🏽 Dans les paramètres [Autorisations], activez l'option :\n\n[✅ Ajout d'une pièce]\n\n🕚Attendez 1min",
     'zh': "👮🏽 在[权限]设置中，启用选项：\n\n[✅添加零件]\n\n🕚等待1分钟",
@@ -5804,20 +5461,20 @@
     'ar': "☑️☐ إيقاف تحرير الرسالة",
 }
 # endregion
 
 
 # region cadmin_
 l_cadmin_text = {
-    'ru': "👩🏽‍💻 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>admin-доступ</u> (только к /cmd-командам для <i>других</i> администраторов) и <u>god-режим</u> (без ограничений для администраторов)\n\n👩🏽‍💻 <b>Текущие администраторы</b>:\n{0}",
-    'en': "👩🏽‍💻 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <u>admin access</u> (only /cmd commands for <i>other</i> admins) and <u>god mode</u> (no restrictions for admins)\n\n👩🏽‍💻 <b>Current admins</b> :\n{ 0}",
-    'es': "👩🏽‍💻 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <u>el acceso de administrador</u> (solo comandos /cmd para <i>otros</i> administradores) y <u>el modo dios</u> (sin restricciones para administradores)\n\n👩🏽‍💻 <b>Administradores actuales</b> :\n{ 0}",
-    'fr': "👩🏽‍💻 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <u>l&#x27;accès administrateur</u> (uniquement les commandes /cmd pour <i>les autres</i> administrateurs) et <u>le mode Dieu</u> (aucune restriction pour les administrateurs)\n\n👩🏽‍💻 <b>Administrateurs actuels</b> :\n{ 0}",
+    'ru': "👩🏽‍💻 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>admin-доступ</u> (только к /cmd-командам для <i>других</i> администраторов) и <u>god-режим</u> (без ограничений для администраторов)\n\n👉🏼 <b>Текущие администраторы</b>:\n{0}",
+    'en': "👩🏽‍💻 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <u>admin access</u> (only /cmd commands for <i>other</i> admins) and <u>god mode</u> (no restrictions for admins)\n\n👉🏼 <b>Current admins</b> :\n{ 0}",
+    'es': "👩🏽‍💻 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <u>el acceso de administrador</u> (solo comandos /cmd para <i>otros</i> administradores) y <u>el modo dios</u> (sin restricciones para administradores)\n\n👉🏼 <b>Administradores actuales</b> :\n{ 0}",
+    'fr': "👩🏽‍💻 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <u>l&#x27;accès administrateur</u> (uniquement les commandes /cmd pour <i>les autres</i> administrateurs) et <u>le mode Dieu</u> (aucune restriction pour les administrateurs)\n\n👉🏼 <b>Administrateurs actuels</b> :\n{ 0}",
     'zh': "👩🏽‍💻<b>单击</b>✅/☑️ 以<b>启用/禁用</b><u>管理员访问权限</u>（仅对<i>其他</i>管理员执行 /cmd 命令）和<u>上帝模式</u>（对管理员无限制）\n\n👉🏼<b>当前管理员</b>：\n{ 0}",
-    'ar': "👩🏽‍💻 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <u>وصول المسؤول</u> (أوامر فقط / cmd للمسؤولين <i>الآخرين</i> ) ووضع <u>god</u> (لا توجد قيود للمسؤولين)\n\n👩🏽‍💻 <b>المشرفون الحاليون</b> :\n{0}",
+    'ar': "👩🏽‍💻 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <u>وصول المسؤول</u> (أوامر فقط / cmd للمسؤولين <i>الآخرين</i> ) ووضع <u>god</u> (لا توجد قيود للمسؤولين)\n\n👉🏼 <b>المشرفون الحاليون</b> :\n{0}",
 }
 l_cadmin_admin_on = {
     'ru': "✅☑Вкл admin-доступ",
     'en': "✅☑Enable admin access",
     'es': "✅☑Habilitar acceso de administrador",
     'fr': "✅☑Activer l'accès administrateur",
     'zh': "✅☑启用管理员访问权限",
@@ -5848,39 +5505,39 @@
     'ar': "☑️☐Vykl وضع الله",
 }
 # endregion
 
 
 # region handlers
 l_content_types_invite_user_bot = {
-    'ru': "🚶🏽 <b>Приглашение</b> @username/@name_bot не разрешено",
+    'ru': "🚶🏽 Инвайт @username/@name_bot не разрешены",
     'en': "🚶🏽 @username / @name_bot invites are not allowed",
     'es': "🚶🏽 Las invitaciones @username / @name_bot no están permitidas",
     'fr': "🚶🏽 Les invitations @username / @name_bot ne sont pas autorisées",
     'zh': "🚶🏽 @username / @name_bot邀请是不允许的",
     'ar': "🚶🏽 @username / @name_bot الدعوات غير مسموح بها",
 }
 l_content_types_invite_user = {
-    'ru': "🚶🏽 <b>Приглашение</b> @username не разрешено",
+    'ru': "🚶🏽 Инвайт @username не разрешен",
     'en': "🚶🏽 Invite @username not allowed",
     'es': "🚶🏽 Invitar @username no permitido",
     'fr': "🚶🏽 Inviter @username non autorisé",
     'zh': "🚶🏽 不允许邀请@username",
     'ar': "🚶🏽 دعوة @username غير مسموح به",
 }
 l_content_types_invite_bot = {
-    'ru': "🚶🏽 <b>Приглашение</b> @name_bot не разрешено",
+    'ru': "🚶🏽 Инвайт @name_bot не разрешен",
     'en': "🚶🏽 Invite @name_bot not allowed",
     'es': "🚶🏽 No se permite invitar a @name_bot",
     'fr': "🚶🏽 Inviter @name_bot non autorisé",
     'zh': "🚶🏽 不允许邀请@name_bot",
     'ar': "🚶🏽 دعوة @name_bot غير مسموح به",
 }
 l_content_types_button = {
-    'ru': "👮🏽 {0}, <b>жми</b> на кнопку, чтобы вс︎тупить в группу",
+    'ru': "👮🏽 {0}, на<b>Жми</b> на кнопку, чтобы вс︎тупить в группу",
     'en': "👮🏽 {0}, on <b>Press</b> the button to join the group",
     'es': "👮🏽 {0}, en <b>Presiona</b> el botón para unirte al grupo",
     'fr': "👮🏽 {0}, sur <b>Appuyez sur</b> le bouton pour rejoindre le groupe",
     'zh': "👮🏽 {0}, on<b>按下</b>按钮加入群组",
     'ar': "👮🏽 {0} ، <b>اضغط</b> على الزر للانضمام إلى المجموعة",
 }
 l_content_types_captcha = {
@@ -5888,15 +5545,15 @@
     'en': "👮🏽 {0}, choose <i>the correct</i> answer to join the group:\n\n{1}",
     'es': "👮🏽 {0}, elige <i>la respuesta correcta</i> para unirte al grupo:\n\n{1}",
     'fr': "👮🏽 {0}, choisis <i>la bonne</i> réponse pour rejoindre le groupe :\n\n{1}",
     'zh': "👮🏽 {0}，选择<i>正确</i>答案加入群组：\n\n{1}",
     'ar': "👮🏽 {0} ، اختر الإجابة <i>الصحيحة</i> للانضمام إلى المجموعة:\n\n{1}",
 }
 l_hand_msg_FLOOD_USERNAME = {
-    'ru': "💬 <b>Пользователь</b> @{0} изменил <b>name/@username</b>! Возможно, шпион!",
+    'ru': "💬 Пользователь @{0} изменил <b>name/@username</b>! Возможно, шпион!",
     'en': "💬 User @{0} changed <b>name/</b> <b>@username</b> ! Possibly a spy!",
     'es': "💬 ¡Usuario @{0} cambió <b>de nombre/</b> <b>@username</b> ! ¡Posiblemente un espía!",
     'fr': "💬 L'utilisateur @{0} a changé <b>de nom/</b> <b>@username</b> ! Peut-être un espion !",
     'zh': "💬 用户@{0} 更改了<b>名称/</b> <b>@username</b> ！可能是间谍！",
     'ar': "💬 تم تغيير <b>اسم المستخدم @ {0} /</b> <b>@username</b> ! ربما جاسوس!",
 }
 l_hand_msg_flood = {
@@ -6757,39 +6414,39 @@
     'es': "🚫 No se pudo agregar {0} a la base de datos, debe abrir el acceso gratuito para unirse",
     'fr': "🚫 Échec de l'ajout de {0} à la base de données, vous devez ouvrir un accès gratuit pour rejoindre",
     'zh': "🚫 添加{0}到数据库失败，需要开通免费权限才能加入",
     'ar': "🚫 فشل إضافة {0} إلى قاعدة البيانات ، تحتاج إلى فتح وصول مجاني للانضمام",
 }
 
 l_add_chn_fail = {
-    'ru': "🚫 <b>Канал</b> {0} не добавлен в базу\n\n{1} аватар\n{2} описание\n{3} более {4} подписчиков\n{5} последний пост менее {6} дней назад\n{7} скам",
+    'ru': "🚫 <b>Канал</b> {0} не добавлен в базу\n\n{1} аватар\n{2} описание\n{3} более {4} подписчиков\n{5} последний пост менее {6} дней назад",
     'en': "🚫 Channel {0} - not added to the database\n\n{1} avatar\n{2} >100 subscribers\n{3} last post <100 days ago",
     'es': "🚫 Canal {0} - no agregado a la base de datos\n\n{1} avatar\n{2} >100 suscriptores\n{3} última publicación <100 días atrás",
     'fr': "🚫 Chaîne {0} - non ajoutée à la base de données\n\n{1} avatar\n{2} >100 abonnés\n{3} dernier message il y a <100 jours",
     'zh': "🚫 频道 {0} - 未添加到数据库\n\n{1} 头像\n{2} >100 个订阅者\n{3} 上次发布 <100 天前",
     'ar': "🚫 القناة {0} - لم تتم إضافتها إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2}> 100 مشترك\n{3} آخر مشاركة قبل أقل من 100 يوم",
 }
 l_add_grp_fail = {
-    'ru': "🚫 <b>Группа</b> {0} не добавлена в базу\n\n{1} аватар\n{2} описание\n{3} более {4} участников\n{5} последний пост менее {6} дней назад\n{7} скам",
+    'ru': "🚫 <b>Группа</b> {0} не добавлена в базу\n\n{1} аватар\n{2} описание\n{3} более {4} участников\n{5} последний пост менее {6} дней назад",
     'en': "🚫 Group {0} - not added to the database\n\n{1} avatar\n{2} >100 members\n{3} last post <100 days ago",
     'es': "🚫 Grupo {0} - no agregado a la base de datos\n\n{1} avatar\n{2} >100 miembros\n{3} última publicación <100 días atrás",
     'fr': "🚫 Groupe {0} - non ajouté à la base de données\n\n{1} avatar\n{2} >100 membres\n{3} dernier message il y a <100 jours",
     'zh': "🚫 组 {0} - 未添加到数据库\n\n{1} 头像\n{2} >100 名成员\n{3} 上次发帖 <100 天前",
     'ar': "🚫 المجموعة {0} - لم تتم إضافتها إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2}> 100 عضو\n{3} آخر مشاركة منذ أقل من 100 يوم",
 }
 l_add_usr_fail = {
-    'ru': "🚫 <b>Пользователь</b> {0} не добавлен в базу\n\n{1} аватар\n{2} @username\n{3} био\n{4} скам",
+    'ru': "🚫 <b>Пользователь</b> {0} не добавлен в базу\n\n{1} аватар\n{2} @username\n{3} био",
     'en': "🚫 User {0} - not added to database\n\n{1} avatar\n{2} @username\n{3} bio",
     'es': "🚫 Usuario {0}: no agregado a la base de datos\n\n{1} avatar\n{2} @username\n{3} biografía",
     'fr': "🚫 Utilisateur {0} - non ajouté à la base de données\n\n{1} avatar\n{2} @username\n{3} bio",
     'zh': "🚫 用户 {0} - 未添加到数据库\n\n{1} 头像\n{2} @username\n{3} 简介",
     'ar': "🚫 المستخدم {0} - لم تتم إضافته إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2} @username\n{3} السيرة الذاتية",
 }
 l_add_bot_fail = {
-    'ru': "🚫 <b>Бот</b> {0} не добавлен в базу\n\n{1} аватар\n{2} описание\n{3} скам",
+    'ru': "🚫 <b>Бот</b> {0} не добавлен в базу\n\n{1} аватар\n{2} описание",
     'en': "🚫 Bot {0} - not added to the database\n\n{1} avatar\n{2} description",
     'es': "🚫 Bot {0} - no agregado a la base de datos\n\n{1} avatar\n{2} descripción",
     'fr': "🚫 Bot {0} - non ajouté à la base de données\n\n{1} description de l'avatar\n{2}",
     'zh': "🚫 机器人 {0} - 未添加到数据库\n\n{1} 头像\n{2} 描述",
     'ar': "🚫 بوت {0} - لم تتم إضافته إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2} الوصف",
 }
 
@@ -7141,15 +6798,15 @@
     'en': "👩🏽‍💻 <b>Enter</b> text to search media notes",
     'es': "👩🏽‍💻 <b>Ingrese</b> texto para buscar notas multimedia",
     'fr': "👩🏽‍💻 <b>Entrez</b> du texte pour rechercher des notes multimédias",
     'zh': "👩🏽‍💻<b>输入</b>文字搜索媒体笔记",
     'ar': "👩🏽‍💻 <b>أدخل</b> نصًا للبحث في ملاحظات الوسائط",
 }
 l_media_random = {
-    'ru': "🎲 Случайный выбор",
+    'ru': "🎲 <b>Случайный</b> выбор",
     'en': "🎲 <b>Random</b> selection",
     'es': "🎲 Selección <b>aleatoria</b>",
     'fr': "🎲 Sélection <b>aléatoire</b>",
     'zh': "🎲<b>随机</b>选择",
     'ar': "🎲 اختيار <b>عشوائي</b>",
 }
 l_media_none = {
```

### Comparing `yeref-0.2.81/yeref/yeref.py` & `yeref-0.2.9/yeref/yeref.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import moviepy.editor as mp
 from PIL import Image
 from aiogram import types, Bot
 from aiogram.enums import ParseMode
 from aiogram.exceptions import TelegramRetryAfter
 from aiogram.utils.keyboard import InlineKeyboardBuilder
 from aiogram.utils.text_decorations import markdown_decoration
-from bs4 import BeautifulSoup
 from exiftool import ExifToolHelper
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaFileUpload, MediaIoBaseDownload
 from loguru import logger
 from oauth2client.service_account import ServiceAccountCredentials
 from pydub import AudioSegment
 from pyrogram import enums, Client, utils
@@ -52,15 +51,14 @@
     '6236215930',
 
     '5754810063',
     '5491025132',
     '5360564451',
     '6281795468',
 ]
-GROUP_ANON_TID = 1087968824
 
 ferey_channel_europe = -1001471122743
 ferey_channel_en = -1001833151619
 ferey_channel_es = -1001988190840
 ferey_channel_fr = -1001942773697
 ferey_channel_ar = -1001913015662
 ferey_channel_zh = -1001904073819
@@ -87,17 +85,19 @@
     "https://telegra.ph/pst-FereyAdsBot-05-08": "c1024508f1a5de4f9544dd10793b1401da95de5719bdcf0b4c9f6c26a672",
 }
 
 one_minute = 60
 one_hour = 3600
 seconds_in_day = 86400
 old_tid = 5_000_000_000
-old_tid_del = 1_000_000_000
 lat_company = 59.395881
 long_company = 24.658980
+price_one = 200
+price_all = 500
+passwd = 'lost9'
 bin_empty = b'\xe2\x81\xa0\xe2\x81\xa0'  # .encode("utf-8")
 hex_empty = 'e281a0e281a0'  # .encode("utf-8").hex()  || bytes.fromhex()
 str_empty = bin_empty.decode('utf-8')
 
 
 SECTION = 'CONFIG'
 LINES_ON_PAGE = 5
@@ -150,15 +150,14 @@
 ferey_wp = 'https://t.me/bg/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 ferey_set = 'https://t.me/addstickers/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 ferey_emoji = 'https://t.me/addemoji/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 reactions_ = ['👍', '❤', '🔥', '🥰', '👏', '😁', '🤔', '🤯', '😱', '🤬', '😢', '🎉', '🤩', '🙏',
               '👌', '🕊', '🤡', '🥱', '🥴', '😍', '🐳', '❤\u200d🔥', '🌚', '🌭', '💯', '🤣', '⚡', '🍌', '🏆',
               '💔', '🤨', '😐', '🍓', '🍾', '💋', '😈', '😴', '😭', '🤓', '👻', '👨\u200d💻', '👀', '🎃',
               '🙈', '😇', '😨', '🤝', '✍', '🤗', '\U0001fae1', '😂', '🎄', '⛄', ' 🆒', '🗿']
-emojis_ = ['🙂', '😶‍🌫️', '🫥', '🎃', '😻', '🫶🏽', '🙌🏽', '👍🏽', '🤌🏾', '🫳🏽', '👉🏼', '☝🏽', '👋🏽', '✍🏽', '🙏🏼', '👣', '🫀', '👤', '👥', '👮🏽', '👩🏽‍💻', '🥷🏽', '💁🏽‍♂️', '🤷🏽‍♂️', '👕', '🧢', '🎓', '👓', '🐳', '🐋', '🌱', '🌿', '☘️', '🍀', '🍃', '🍂', '🍁', '🌚', '🌗', '🌏', '⭐️', '⚡️', '🔥', '☀️', '🌤️', '❄️', '🫧', '🌬️', '🧊', '🥏', '🎗️', '🧩', '🚀', '🗽', '🗿', '⛰️', '🏔️', '🗻', '🏠', '🏙️', '💻', '🎥', '🧭', '⏳', '🔋', '💡', '💵', '💰', '💳', '⚒️', '🛡️', '📍', '🪬', '🛋️', '🎉', '✉️', '📬', '📜', '📄', '📅', '🧾', '📇', '📋', '🗄️', '📁', '📰', '📘', '📖', '🖤', '〽️', '🔆', '✅', '🌐', '💠', '🔹', '💭', '🚩']
 themes_ = ['🐥', '⛄', '💎', '👨\u200d🏫', '🌷', '💜', '🎄', '🎮']  # все в порядке, все ставятся, если не стояли
 bot_father = "@BotFather"
 text_jpeg = 'https://telegra.ph/file/0c675e5a3724deff3b2e1.jpg'
 bot_logo_jpeg = 'https://telegra.ph/file/99d4f150a52dcf78b3e8a.jpg'
 channel_logo_jpeg = 'https://telegra.ph/file/8418e1cd70484eac89477.jpg'
 group_logo_jpeg = 'https://telegra.ph/file/807e0d4fc4f271899272a.jpg'
 payment_photo = 'https://telegra.ph/file/75747cf7bc68f45a0e8b8.jpg'
@@ -169,261 +168,28 @@
 video_note_jpg = 'https://telegra.ph/file/a0ebd72b7ab97b8d6de24.jpg'
 audio_jpg = 'https://telegra.ph/file/15da5534cb4edfbdf7601.jpg'
 voice_jpg = 'https://telegra.ph/file/10ada321eaa60d70a125d.jpg'
 document_jpg = 'https://telegra.ph/file/28b6c218157833c0f4030.jpg'
 sticker_jpg = 'https://telegra.ph/file/986323df1836577cbe55d.jpg'
 log_ = f"\033[{92}m%s\033[0m"
 
-extra_prompt = 'a candid portrait, hyper-realistic image, ultra-realistic photography, cinematic photo, uhd motion capture, high-contrast image, 8k camera, atmospheric light'
-short_description = f"""🌱 Top #10 Telegram-Marketing Bots
+short_description = f"""🌱 Top 10 Telegram-Marketing Bot
 
-Connect/Projects: t.me/FereyDemoBot
+All projects: t.me/FereyDemoBot
 🇬🇧🇨🇳🇦🇪🇪🇸🇷🇸🇫🇷
 """
 
 markupAdmin = types.ReplyKeyboardMarkup(keyboard=[
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
-BOT_VARS_ = '{"BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": "+00:00", "BOT_DT": "", "BOT_LZ": "en", "BOT_LC": "en"}'
+BOT_VARS_ = '{"BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0, "BOT_TZ": 0, "BOT_DT": "", "BOT_LZ": "en", "BOT_LC": "en"}'
 BOT_LSTS_ = '{"BOT_ADMINS": []}'
-USER_VARS_ = '{"USER_TEXT": "", "USER_PUSH": "", "USER_EMAIL": "", "USER_PROMO": "", "USER_PHONE": "", "USER_GEO": "", "USER_UTM": "", "USER_ID": 0, "USER_DT": "", "USER_TZ": "+00:00", "USER_LC": "en", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "DATE_TIME": 0}'
+USER_VARS_ = '{"USER_TEXT": "", "USER_PUSH": "", "USER_EMAIL": "", "USER_PROMO": "", "USER_PHONE": "", "USER_GEO": "", "USER_UTM": "", "USER_ID": 0, "USER_DT": "", "USER_TZ": 0, "USER_LC": "en", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "DATE_TIME": 0}'
 USER_LSTS_ = '{"USER_UTMREF": []}'
-
-
-html_404 = f"""<!DOCTYPE html>
-<html lang="en">
-<head>
-    <meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <style>
-        body {{ background-image: url('https://telegra.ph/file/4b093c7e2b68f9f2915b0.jpg'); background-size: cover; background-position: center; font-family: Arial, sans-serif; display: flex; justify-content: center; align-items: center; height: 100vh; margin: 0; }}
-        .container {{ text-align: center; padding: 30px; background-color: rgba(255, 255, 255, 0.8); border-radius: 10px; }}
-        .error-code {{ font-size: 100px; color: #2c3e50; margin: 0; }}
-        .go-back {{ margin-top: 20px; text-decoration: none; color: #3498db; }}
-    </style>
-</head>
-<body><div class="container"><h1 class="error-code">404</h1><a href="https://t.me/FereyBotBot" class="go-back">@FereyBotBot</a></div></body>
-</html>
-"""
-html_msg = f"""
-d
-"""
-html_template = """<!DOCTYPE html>
-<html lang="en">
-<head>
-    <meta charset="UTF-8">
-    <script src="https://telegram.org/js/telegram-web-app.js"></script>
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-
-    <style>
-        html {{ box-sizing: border-box; }}
-        *,*::before, *::after {{ box-sizing: inherit; font-family: Arial, sans-serif; color: rgba(40, 40, 40, 0.99);}}
-        a {{ text-decoration: none; }}
-        span {{ color: #007bff; }}
-        body {{ margin: 0; padding: 0; overflow-x: hidden; }}
-        
-        .text b, .text u, .text i, .text a, .text code, .text span {{ display: inline; }}
-        .text code {{ font-family: 'Courier New', monospace; background-color: #f5f5f5; }}
-        .text {{ width: 100%; text-align: justify; }}
-
-        .container-wrapper {{ max-width: 1270px; height: 100vh;  padding: 4px; margin: 0 auto; display: flex; flex-direction: column; justify-content: space-between; gap: 4px; }}
-        .container {{ display: flex; flex-direction: column; align-items: center; justify-content: flex-start; font-size: 14px; gap: 4px; }}
-        
-        .media-wrapper {{ -webkit-text-stroke: 0.5px rgba(50, 50, 50, 0.99); position: relative; width: 100%; min-height: 33vh; display: flex; justify-content: center; align-items: flex-start; }}
-        .media {{ width: 100%; max-height: 33vh; object-fit: cover; }}
-        .media:not(.rounded-media) {{ border-radius: 4px; }}
-        .rounded-media {{ border-radius: 50%; }}
-        
-        .buttons-wrapper {{
-            width: 100%;
-            height: 100%;
-            display: flex;
-            flex-direction: column;
-            justify-content: center;
-            gap: 4px;
-        }}
-        .buttons-row {{
-            width: 100%;
-            height: 100%;
-            display: flex;
-            flex-direction: row;
-            justify-content: center;
-            gap: 4px;
-        }}
-        .button {{
-            width: 100%;
-            height: 34px;
-
-            display: flex;
-            justify-content: center;
-            align-items: center;
-
-            background-color: #007bff;
-            color: #fff;
-            text-align: center;
-            line-height: 34px;
-            border-radius: 4px;
-            cursor: pointer;
-        }}
-        .footer {{
-            display: flex;
-            justify-content: space-between;
-            align-items: center;
-            
-            margin-bottom: 4px; 
-            color: rgba(140, 150, 160, 0.99);
-            font-size: 10px; 
-        }}
-        
-        #media-number {{
-            position: absolute;
-            top: 1%;
-            left: 1%;
-            padding: 16px;
-            padding-top: 19px;
-            font-size: 10px;
-
-            cursor: pointer;
-            color: rgba(254, 254, 254, 1.0);
-        }}
-        #media-prev {{
-            position: absolute;
-            top: 45%;
-            left: 1%;
-            padding: 16px;
-            cursor: pointer;
-            color: rgba(254, 254, 254, 1.0);
-        }}
-        #media-next {{
-            position: absolute;
-            top: 45%;
-            right: 1%;
-            padding: 16px;
-            cursor: pointer;
-            color: rgba(254, 254, 254, 1.0);
-        }}
-        .dot {{
-            cursor: pointer;
-            height: 10px;
-            width: 10px;
-            margin: 0 2px;
-
-            background-color: rgba(254, 254, 254, 1.0);
-            border-radius: 50%;
-            border: 0.5px solid rgba(50, 50, 50, 0.99);
-            display: inline-block;
-            transition: background-color 0.6s ease;
-            opacity: 0.2;
-        }}
-        
-        #media-dots {{ position: absolute; bottom: 1%;  text-align: center; padding: 16px; }}
-        .active, .dot:hover {{ opacity: 1; }}
-        #media-prev:hover {{ opacity: 0.6; }}
-        #media-next:hover {{ opacity: 0.6; }}
-    </style>
-</head>
-<body>
-    <div class="container-wrapper">
-        <div class="container">
-            {0}
-            {1}
-            {2}
-        </div>
-        <div class="footer">
-            <div style="color: rgba(140, 150, 160, 0.99);">👁 {3}</div>
-            <div><a href="https://t.me/{4}" style="color: rgba(140, 150, 160, 0.99);">@{4}</a></div>
-        </div>
-    </div>
-    <script>
-        document.addEventListener("DOMContentLoaded", async () => {{
-            const imageList = {7}
-            let currentIndex = 0
-
-            async function updateMedia() {{
-                const mediaElement = document.querySelector('.media');
-                const mediaNumber = document.getElementById('media-number');
-
-                mediaElement.src = imageList[currentIndex];
-                mediaNumber.textContent = (currentIndex + 1) + '/' + imageList.length;
-                const dots = document.getElementsByClassName('dot');
-                for (let i = 0; i < dots.length; i++) dots[i].classList.remove('active');
-                dots[currentIndex].classList.add('active');
-            }}
-
-            document.getElementById('media-prev').addEventListener('click', async () => {{
-                currentIndex = (currentIndex - 1 + imageList.length) % imageList.length;
-                await updateMedia();
-            }});
-            document.getElementById('media-next').addEventListener('click', async () => {{
-                currentIndex = (currentIndex + 1) % imageList.length;
-                await updateMedia();
-            }});
-
-            await updateMedia();
-            const roundedMedia = document.querySelectorAll('.rounded-media');
-            for (let i = 0; i < roundedMedia.length; i++) roundedMedia[i].style.width = "auto";
-        }})
-        async function fetchData(url) {{
-            try {{
-                const response = await fetch(url);
-                const data = await response.json();
-                return data;
-            }} catch (error) {{
-                console.error('Error fetching data:', error);
-                return null;
-            }}
-        }}
-
-        async function handleButtonClick(button) {{
-            const url = button.dataset.url;
-            const idArr = button.id.split("-");
-
-            let getUrl;
-            if (idArr[1] === 'payment') {{
-                tg.openInvoice(url, async (status) => {{
-                    getUrl = `/{5}?msg_id={6}&btn_id=${{idArr[2]}}&cnt_id=${{idArr[3]}}&kind=${{idArr[1]}}&status=${{status}}&${{tg.initData}}`;
-                    const response = await fetchData(getUrl);
-                    location.reload();
-                }});
-            }} else if (idArr[1] === 'like') {{
-                getUrl = `/{5}?msg_id={6}&btn_id=${{idArr[2]}}&cnt_id=${{idArr[3]}}&kind=${{idArr[1]}}&status=click&${{tg.initData}}`;
-                const response = await fetchData(getUrl);
-                location.reload();
-            }} else if (url.startsWith('https://t.me/')) {{
-                tg.openTelegramLink(url);
-                getUrl = `/{5}?msg_id={6}&btn_id=${{idArr[2]}}&cnt_id=${{idArr[3]}}&kind=${{idArr[1]}}&status=link&${{tg.initData}}`;
-                const response = await fetchData(getUrl);
-                location.reload();
-            }} else {{
-                tg.openLink(url, {{try_instant_view: true}});
-                getUrl = `/{5}?msg_id={6}&btn_id=${{idArr[2]}}&cnt_id=${{idArr[3]}}&kind=${{idArr[1]}}&status=link&${{tg.initData}}`;
-                const response = await fetchData(getUrl);
-                location.reload();
-            }}
-        }}
-
-        console.log('start');
-        let tg = window.Telegram.WebApp;
-        tg.ready();
-        console.log('script start', tg.initData);
-        if (tg.initData === '') throw new Error('404');
-        console.log(tg.initDataUnsafe);
-        console.log(tg.initData);
-        console.log(tg.initDataUnsafe['start_param']);
-        let buttonsClass = document.getElementsByClassName('button');
-
-        let startUrl = `/web?tgWebAppStartParam={5}_{6}&${{tg.initData}}`;
-        console.log('startUrl = ', startUrl);
-        fetchData(startUrl);
-
-        for (let i = 0; i < buttonsClass.length; i++)  buttonsClass[i].addEventListener('click', async () => {{ await handleButtonClick(buttonsClass[i]); }});
-    </script>
-</body>
-</html>
-"""
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
 
@@ -500,28 +266,30 @@
             TRG_VID         VARCHAR     UNIQUE NOT NULL,
             TRG_TYPE        VARCHAR,
             TRG_CONTENT     VARCHAR,
 
             TRG_RIGHTID     VARCHAR,
             TRG_RIGHTTYPE   VARCHAR,
             TRG_LEFTID      VARCHAR,
-            TRG_LEFTTYPE    VARCHAR
+            TRG_LEFTTYPE    VARCHAR,
+            TRG_USERS       VARCHAR
         )''')
 
         # ACT
         cur.execute('''CREATE TABLE IF NOT EXISTS ACT ( 
             ACT_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
                                         UNIQUE
                                         NOT NULL,
             ACT_VID         VARCHAR     UNIQUE NOT NULL,
             ACT_TYPE        VARCHAR,
             ACT_CONTENT     VARCHAR,
 
             ACT_NEXTID      VARCHAR,
-            ACT_NEXTTYPE    VARCHAR
+            ACT_NEXTTYPE    VARCHAR,
+            ACT_USERS       VARCHAR
         )''')
 
         # MSG
         cur.execute('''CREATE TABLE IF NOT EXISTS MSG ( 
             MSG_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
                                         UNIQUE
                                         NOT NULL,
@@ -534,26 +302,16 @@
             MSG_CHKBOX      VARCHAR,
             MSG_TEXTF       VARCHAR,  
             MSG_BUTTONSF    VARCHAR,
             MSG_LC          VARCHAR,
             MSG_TRANSLATED  INTEGER     DEFAULT 0,
 
             MSG_NEXTID      VARCHAR,
-            MSG_NEXTTYPE    VARCHAR
-        )''')
-
-        # VIEW
-        cur.execute('''CREATE TABLE IF NOT EXISTS VIEW ( 
-            VIEW_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
-                                        UNIQUE
-                                        NOT NULL,
-            ENT_VID         VARCHAR     UNIQUE NOT NULL,
-            ENT_TYPE        VARCHAR     NOT NULL,
-            CHAT_TID        BIGINT,
-            UNIQUE (ENT_VID, ENT_TYPE, CHAT_TID)
+            MSG_NEXTTYPE    VARCHAR,
+            MSG_USERS       VARCHAR
         )''')
 
         # LANG
         cur.execute('''CREATE TABLE IF NOT EXISTS LANG ( 
             LANG_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
                                         UNIQUE
                                         NOT NULL,
@@ -569,63 +327,36 @@
         # POST
         cur.execute('''CREATE TABLE IF NOT EXISTS POST ( 
             POST_ID            INTEGER      PRIMARY KEY AUTOINCREMENT
                                             UNIQUE
                                             NOT NULL,
             POST_CHATTID       BIGINT       NOT NULL,
             POST_USERTID       BIGINT       NOT NULL,
+            
             POST_TARGET        VARCHAR,
-            POST_TYPE          VARCHAR,
             POST_TEXT          VARCHAR,
-            POST_TEXTF         VARCHAR,
-            POST_MSGID         VARCHAR,
-            POST_TELESCOPE     VARCHAR,
-            
+            POST_MEDIATYPE     VARCHAR,
+            POST_FILEID        VARCHAR,
+            POST_FILEIDNOTE    VARCHAR,
+            POSTB_FILEID       VARCHAR,
+            POSTB_FILEIDNOTE   VARCHAR,
+            POST_FILENAME      VARCHAR,
+
+            POST_TGPHLINK      VARCHAR,
+            POST_ISTGPH        BOOLEAN     DEFAULT 0,
             POST_BUTTON        VARCHAR,
-            POST_BUTTONF       VARCHAR,
-            POST_BLOG          VARCHAR,
-            POST_WEB           VARCHAR,
-            POST_WALL          VARCHAR,
-            POST_EMOJI         VARCHAR,
-            POST_THEME         VARCHAR,
-            POST_TZ            VARCHAR,
-            POST_DT            VARCHAR,
-            POST_TR            VARCHAR,
-            POST_STATUS        BOOLEAN     DEFAULT 0,
-            
             POST_ISBUTTON      BOOLEAN     DEFAULT 0,
-            POST_ISFORMAT      BOOLEAN     DEFAULT 0,
-            POST_ISSOUND       BOOLEAN     DEFAULT 1,
-            POST_ISSILENCE     BOOLEAN     DEFAULT 0,
-            POST_ISPIN         BOOLEAN     DEFAULT 0,
-            POST_ISPREVIEW     BOOLEAN     DEFAULT 0,
             POST_ISSPOILER     BOOLEAN     DEFAULT 0,
+            POST_ISPIN         BOOLEAN     DEFAULT 0,
+            POST_ISSILENCE     BOOLEAN     DEFAULT 0,
             POST_ISGALLERY     BOOLEAN     DEFAULT 0,
-            POST_ISDESTROY     BOOLEAN     DEFAULT 0,
-            POST_ISTAG         BOOLEAN     DEFAULT 0,
-            POST_ISVIA         BOOLEAN     DEFAULT 0,
-            
-            POST_LNK           VARCHAR,
-            POST_FILENAME      VARCHAR,
-            
-            POST_FID           VARCHAR,
-            POST_FIDNOTE       VARCHAR,
-            POSTB_FID          VARCHAR,
-            POSTB_FIDNOTE      VARCHAR
-        )''')
 
-        # PUSH
-        cur.execute('''CREATE TABLE IF NOT EXISTS PUSH ( 
-            PUSH_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
-                                        UNIQUE
-                                        NOT NULL,
-            CHAT_ID         INTEGER     NOT NULL,
-            POST_ID         INTEGER     NOT NULL,
-            BUTTON_ID       INTEGER     NOT NULL,
-            UNIQUE (CHAT_ID, POST_ID, BUTTON_ID)
+            POST_STATUS        BOOLEAN     DEFAULT 0,
+            POST_TZ            VARCHAR,
+            POST_DT            VARCHAR
         )''')
 
         # USER
         cur.execute(f'''CREATE TABLE IF NOT EXISTS USER ( 
             USER_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
                                         UNIQUE
                                         NOT NULL,
@@ -736,15 +467,15 @@
 
 
 async def get_buttons_main(lz, bot_un, BASE_D):
     result = []
     try:
         result = [
             types.InlineKeyboardButton(text="👩🏽‍💼Acc", url=f"tg://user?id={my_tid}"),
-            types.InlineKeyboardButton(text="🙌🏽Tgph", web_app=types.WebAppInfo(url='https://telegra.ph/Links-07-05-462')),
+            types.InlineKeyboardButton(text="🙌🏽Tgph", web_app=types.WebAppInfo(url='https://telegra.ph')),
             types.InlineKeyboardButton(text="🔗Share",
                                        url=f'https://t.me/share/url?url=https%3A%2F%2Ft.me%2F{bot_un}&text=%40{bot_un}'),
             types.InlineKeyboardButton(text=f"{(await read_likes(BASE_D))}♥️Like", callback_data=f"like"),
             types.InlineKeyboardButton(text="🦋Chan", url=f"https://t.me/{get_tg_channel(lz)}"),
             types.InlineKeyboardButton(text="🫥Bots", switch_inline_query_current_chat=f"~"),
         ]
     except Exception as e:
@@ -787,15 +518,14 @@
                 if page_['url'] != url: continue
 
                 get_page_ = await telegraph_.get_page(path=page_['path'], return_content=True, return_html=False)
                 try:
                     content_json = json.loads(str(get_page_['content'][0]))
                     if len(content_json) > 20: raise Exception
                 except:
-                    await telegraph_.edit_page(path=page_['path'], title=page_['title'], html_content='{}')
                     content_json = {}
 
                 timestamp_ = str(utils.datetime_to_timestamp(datetime.datetime.utcnow()))
                 content_json[timestamp_] = json_
                 post_dumps = json.dumps(content_json, ensure_ascii=False)
                 await telegraph_.edit_page(path=page_['path'], title=page_['title'], html_content=post_dumps)
                 return 1
@@ -835,27 +565,23 @@
     return 0
 
 
 async def get_tgph_link(file_name):
     result = None
     try:
         if file_name and os.path.exists(file_name) and os.path.getsize(file_name) < 5242880:
-            cnt = 1
-            while cnt >= 0:
-                try:
-                    # jpg, .jpeg, .png, .gif and .mp4
-                    telegraph_ = Telegraph()
-                    res = await telegraph_.upload_file(file_name)
-                    if res:
-                        result = f"{'https://telegra.ph'}{res[0]['src']}"
-                        return
-                except Exception as e:
-                    logger.info(log_ % f"Telegraph (cnt={cnt}): {str(e)}")
-                    await asyncio.sleep(round(random.uniform(2, 3), 2))
-                    cnt -= 1
+            try:
+                # jpg, .jpeg, .png, .gif and .mp4
+                telegraph_ = Telegraph()
+                res = await telegraph_.upload_file(file_name)
+                if res:
+                    result = f"{'https://telegra.ph'}{res[0]['src']}"
+            except Exception as e:
+                logger.info(log_ % f"Telegraph: {str(e)}")
+                await asyncio.sleep(round(random.uniform(0, 1), 2))
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
 
@@ -2468,152 +2194,14 @@
         return result
 
 
 # endregion
 
 
 # region functions
-async def upper_register(txt):
-    result = str(txt).replace('0', '⁰').replace('1', '¹').replace('2', '²').replace('3', '³').replace('4', '⁴').replace('5', '⁵').replace('6', '⁶').replace('7', '⁷').replace('8', '⁸').replace('9', '⁹')
-    try:
-        if len(result) >= 3:
-            result = f"{result[0]}˙{result[1]}ᵏ"
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return result
-
-
-async def convert_tgmd_to_html(markdown_text):
-    result = markdown_text
-    try:
-        # markdown_text = "👩🏽‍💻 Lorem _начало_, ыусщте  df d d\n_Это_ *пример* [link](https://t.me) текста с *жирным* и _курсивом_\n\n[Ссылка на Google](https://www.google.com)\n\n#Хэштег #markdown #HTML\n\n$Кэштег $python $coding\n\n~Этот текст будет перечеркнут~\n\n__Этот текст будет подчеркнут__\n\n`Это кодовый фрагмент`\n\n```Это тоже кодовый фрагмент```"
-        markdown_text = markdown_text.replace('\n', '<br>')
-
-        # Заменяем * на <b> (жирный) только если он окружен пробелами или не имеет соседей с символами букв и цифр
-        html_text = re.sub(r'(?<![\w*])\*(?!\*)\s*(.*?)\s*\*(?!\*)(?![\w*])', r'<b>\1</b>', markdown_text)
-        html_text = re.sub(r'__(.*?)__', r'<u>\1</u>', html_text)
-        html_text = re.sub(r'\|\|(.*?)\|\|', r'<code>\1</code>', html_text)
-        html_text = re.sub(r'_(.*?)_', r'<i>\1</i>', html_text)
-        html_text = re.sub(r'~(.*?)~', r'<s>\1</s>', html_text)
-        html_text = re.sub(r'```(.*?)```', r'<code>\1</code>', html_text)
-        html_text = re.sub(r'`(.*?)`', r'<code>\1</code>', html_text)
-
-        html_text = re.sub(r'\[([^\]]+)\]\(([^)]+)\)', r'<a href="\2">\1</a>', html_text)
-        html_text = re.sub(r'#(\w+)', r'<span>#\1</span>', html_text)
-        html_text = re.sub(r'\$(\w+)', r'<span>$\1</span>', html_text)
-
-        # with open("index.html", "w", encoding="utf-8") as file:
-        #     file.write(f"<!DOCTYPE html>\n<html>\n<head>\n<meta charset=\"UTF-8\">\n<title>Markdown to HTML</title>\n<style>\nspan {{\n    color: #007bff;\n}}\na {{\n  text-decoration: none;\n}}\n</style>\n</head>\n<body>\n{html_text}\n</body>\n</html>")
-        result = html_text
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return result
-
-
-async def get_row_html(msg_text, msg_btns, start, finish, MSG_VID, BOT_TID, BOT_LC, BASE_BOT, BASE_D):
-    result = ''
-    try:
-        row_html = '<div class="buttons-row">'
-
-        for btn in msg_btns:
-            try:
-                print(f"int(btn['i']) = {int(btn['i'])}, start = {start}")
-                if int(btn['i']) < start: continue
-
-                if int(btn['i']) >= finish:
-                    result = f"{row_html}</div>"
-                    print(f"! res limit = {finish}, {result}")
-                    break
-
-                sql = "SELECT PUSH_ID FROM PUSH WHERE POST_ID=? AND BUTTON_ID=?"
-                data_push = await db_select(sql, (int(MSG_VID), int(btn["i"]),), BASE_BOT)
-                btn_cnt_click = str(len(data_push)).replace('0', '⁰').replace('1', '¹').replace('2', '²').replace('3', '³').replace('4', '⁴').replace('5', '⁵').replace('6', '⁶').replace('7', '⁷').replace('8', '⁸').replace('9', '⁹')
-
-                if btn['knd'] == 'payment':
-                    invoice_link = await create_invoice_link(BOT_TID, BOT_LC, msg_text, msg_btns, BASE_D)
-                    if not invoice_link: continue
-
-                    btn_html = f'<a id="btn-{btn["knd"]}-{btn["i"]}-{str(len(data_push))}" class="button" data-url="{invoice_link}">{btn_cnt_click} {btn["lbl"]}</a>'
-                    row_html = f"{row_html}{btn_html}"
-                elif btn['knd'] == 'like':
-                    btn_html = f'<a id="btn-{btn["knd"]}-{btn["i"]}-{str(len(data_push))}" class="button" data-url="lnk">{btn_cnt_click} {btn["lbl"]}</a>'
-                    row_html = f"{row_html}{btn_html}"
-                elif btn['knd'] == 'link':
-                    btn_html = f'<a id="btn-{btn["knd"]}-{btn["i"]}-{str(len(data_push))}" class="button" data-url="{btn["lnk"]}">{btn_cnt_click} {btn["lbl"]}</a>'
-                    row_html = f"{row_html}{btn_html}"
-
-                print(f"limit = {finish}, {row_html}")
-            except Exception as e:
-                logger.info(log_ % str(e))
-                await asyncio.sleep(round(random.uniform(0, 1), 2))
-
-        if len(row_html) > len('<div class="buttons-row">'):
-            result = f"{row_html}</div>"
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return result
-
-
-async def create_invoice_link(BOT_TID, BOT_LC, msg_text, msg_btns, BASE_D):
-    result = None
-    try:
-        sql = "SELECT BOT_TOKEN, BOT_TOKENPAY FROM BOT WHERE BOT_TID=?"
-        data = await db_select(sql, (BOT_TID,), BASE_D)
-        if not len(data): return
-        BOT_TOKEN, BOT_TOKENPAY = data[0]
-
-        btn_name = msg_btns[0]['lbl'].encode('utf-16', 'surrogatepass').decode('utf-16')
-        # msg_text = await replace_user_vars(chat_id, msg_text)
-        msg_text = msg_text if msg_text and msg_text != '' else btn_name
-        soup = BeautifulSoup(msg_text, 'html.parser')
-        msg_text = soup.get_text()
-
-        currency = await convert_domain_to_currency(BOT_LC)
-        price = msg_btns[0]['lnk']
-        amount = int(price.replace('.', '').replace(',', '')) if '.' in price or ',' in price else int(f"{msg_btns[0]['lnk']}00")
-        prices = [types.LabeledPrice(label=btn_name, amount=amount)]
-
-        msg_media = {
-            'title': btn_name,
-            'description': msg_text,
-            'payload': f"{BOT_TID}_{amount}",
-            'provider_token': BOT_TOKENPAY,
-            'currency': currency,
-            'prices': prices,
-            'max_tip_amount': amount,
-            'suggested_tip_amounts': [amount],
-        }
-        print(f'msg_media = {msg_media}')
-
-        extra_bot = Bot(token=BOT_TOKEN)
-        result = await extra_bot.create_invoice_link(
-            title=msg_media['title'],
-            description=msg_media['description'],
-            payload=msg_media['payload'],
-            provider_token=msg_media['provider_token'],
-            currency=msg_media['currency'],
-            prices=msg_media['prices'],
-            max_tip_amount=msg_media['max_tip_amount'],
-            suggested_tip_amounts=msg_media['suggested_tip_amounts'],
-        )
-        await extra_bot.session.close()
-        print(f'invoice_link = {result}')
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return result
-
-
 async def is_member_in_channel(bot, chat_id, lz):
     result = False
     try:
         channel_id = ferey_channel_en
         if lz == 'ru':
             channel_id = ferey_channel_europe
         elif lz == 'es':
@@ -2729,15 +2317,14 @@
     finally:
         return result
 
 
 async def auto_destroy_msg(bot, telegram_bot, chat_id, text, message_id, type_='text', sec=5):
     result = None
     try:
-        if not sec: return
         step = 1
         by = f"<a href='https://t.me/{ferey_telegram_demo_bot}'>by</a>"
         text = f"{text}\n\n{by} @{telegram_bot} <b>{sec}</b>sec"
         ix_sec = text.rfind('</b>sec')
         while text[ix_sec] != '>': ix_sec -= 1
 
         while sec > 0:
@@ -2745,22 +2332,18 @@
                 text = text.replace(f"<b>{sec}</b>sec", f"<b>{sec - 1}</b>sec")
                 sec -= step
                 if type_ == 'text':
                     await bot.edit_message_text(text, chat_id, message_id, disable_web_page_preview=True)
                 else:
                     await bot.edit_message_caption(chat_id=chat_id, message_id=message_id, caption=text)
                 await asyncio.sleep(1)
-            except TelegramRetryAfter as e:
-                logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
-                await asyncio.sleep(e.retry_after + 1)
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
                 break
-
         await bot.delete_message(chat_id, message_id)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(e)
         await asyncio.sleep(round(random.uniform(1, 2), 2))
@@ -3607,15 +3190,15 @@
                     if len(split_btn) > 1:
                         btn_name = split_btn[0].strip() if len(split_btn) > 1 else "🔗 Go"
                         btn_link = split_btn[-1].strip()
                         if not await is_url(btn_link):
                             await bot.send_message(chat_id, f"🔗 {btn_link}: invalid")
                             return
                     else:
-                        btn_name = f"⁰{split_btn[0]}" if is_counter else split_btn[0]
+                        btn_name =  f"⁰{split_btn[0]}" if is_counter else split_btn[0]
                         # btn_link = cleanhtml(split_btn[0])[:20]
                         # btn_link = f"btn_{btn_link.encode('utf-8').hex()}"
                         btn_link = f"btn_"
 
                     result[ix] = [btn_name, btn_link]
             except Exception as e:
                 logger.info(log_ % str(e))
@@ -5103,119 +4686,114 @@
 # apt install redis -y
 # nano /etc/redis/redis.conf
 # systemctl restart redis.service
 # systemctl status redis
 # redis-cli
 # netstat -lnp | grep redis
 
+# https://www.namecheap.com
+# A Record * 212.73.150.86
+# A Record @ 212.73.150.86
+
 # apt update && apt upgrade -y
 # curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash -
 # apt install -y nodejs build-essential nginx yarn
 # npm install -g npm pm2@latest -g
 # ufw allow 'Nginx Full'
 # curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | gpg --dearmor | tee /usr/share/keyrings/yarnkey.gpg >/dev/null
 # echo "deb [signed-by=/usr/share/keyrings/yarnkey.gpg] https://dl.yarnpkg.com/debian stable main" | tee /etc/apt/sources.list.d/yarn.list
 # node -v
 # nginx -v
 # yarn -v
 
+# rm /etc/nginx/sites-enabled/default
+# nano /etc/nginx/sites-enabled/tg6002
+# nano /etc/nginx/sites-available/fmessenger86.com
+# upstream tg1{
+#     server localhost:6000;
+# }
+# server{
+#     listen 80;
+#     server_name tg1.fmessenger86.com www.tg1.fmessenger86.com;
+#     charset utf-8;
+#     client_max_body_size 50M;
+#
+#     location / {
+#         proxy_redirect off;
+#         proxy_set_header   X-Real-IP $remote_addr;
+#         proxy_set_header   X-Forwarded-For $proxy_add_x_forwarded_for;
+#         proxy_set_header   X-Forwarded-Proto $scheme;
+#         proxy_set_header   Host $http_host;
+#         proxy_set_header   X-NginX-Proxy    true;
+#         proxy_set_header   Connection "";
+#         proxy_http_version 1.1;
+#         proxy_pass         http://tg1;
+#         proxy_set_header     Access-Control-Allow-Origin "*";
+#         proxy_set_header     Access-Control-Allow-Headers "Origin, X-Requested-With, Content-Type, Accept";
+#     }
+# }
+# server {
+#     server_name www.tg1.fmessenger86.com;
+#     return 301 $scheme://tg1.fmessenger86.com$request_uri;
+# }
+
 # systemctl restart nginx
 # systemctl reload nginx
 # snap install core;  snap refresh core
 # apt remove python3-certbot-nginx certbot -y
 # rm -rf /etc/letsencrypt/renewal/
 # rm -rf /etc/letsencrypt/archive/
 # rm -rf /etc/letsencrypt/live/
 # rm -rf /opt/letsencrypt
 # rm -rf /etc/letsencrypt
 # snap install --classic certbot
 # ln -s /snap/bin/certbot /usr/bin/certbot
- # POST
-# cur.execute('''CREATE TABLE IF NOT EXISTS POST (
-#     POST_ID            INTEGER      PRIMARY KEY AUTOINCREMENT
-#                                     UNIQUE
-#                                     NOT NULL,
-#     POST_CHATTID       BIGINT       NOT NULL,
-#     POST_USERTID       BIGINT       NOT NULL,
-#     POST_TARGET        VARCHAR,
-#     POST_TYPE          VARCHAR,
-#     POST_TEXT          VARCHAR,
-#
-#     POST_BUTTON        VARCHAR,
-#     POST_BLOG          VARCHAR,
-#     POST_WEB           VARCHAR,
-#     POST_EMOJI         VARCHAR,
-#     POST_THEME         VARCHAR,
-#     POST_WALL          VARCHAR,
-#     POST_TZ            VARCHAR,
-#     POST_DT            VARCHAR,
-#     POST_TR            VARCHAR,
-#     POST_STATUS        BOOLEAN     DEFAULT 0,
-#
-#     POST_ISBUTTON      BOOLEAN     DEFAULT 0,
-#     POST_ISSOUND       BOOLEAN     DEFAULT 1,
-#     POST_ISSILENCE     BOOLEAN     DEFAULT 0,
-#     POST_ISPIN         BOOLEAN     DEFAULT 0,
-#     POST_ISSPOILER     BOOLEAN     DEFAULT 0,
-#     POST_ISPREVIEW     BOOLEAN     DEFAULT 0,
-#     POST_ISALBUM       BOOLEAN     DEFAULT 0,
-#     POST_ISGALLERY     BOOLEAN     DEFAULT 0,
-#     POST_ISBLOG        BOOLEAN     DEFAULT 0,
-#     POST_ISWEB         BOOLEAN     DEFAULT 0,
-#     POST_ISDESTROY     BOOLEAN     DEFAULT 0,
-#     POST_ISTAG         BOOLEAN     DEFAULT 0,
-#     POST_ISVIA         BOOLEAN     DEFAULT 0,
+# certbot --nginx   # certbot --nginx -d tg1.fmessenger86.com -d www.tg1.fmessenger86.com
+# certbot renew --dry-run
+# systemctl reload nginx && nginx -t
 #
-#     POST_FID           VARCHAR,
-#     POST_FIDNOTE       VARCHAR,
-#     POST_FIDALB        VARCHAR,
-#     POST_FIDNOTEALB    VARCHAR,
-#     POSTB_FID          VARCHAR,
-#     POSTB_FIDNOTE      VARCHAR,
-#     POSTB_FIDALB       VARCHAR,
-#     POSTB_FIDNOTEALB   VARCHAR,
-#     POST_LNK           VARCHAR,
-#     POST_LNKALB        VARCHAR,
-#
-#     POST_FILENAME      VARCHAR
-# )''')
+# https://www.tg6002.fmessenger86.com
+# too many certificates (5) already issued for this exact set of domains in the last 168 hours
+
+# это вроде уже не нужно
+# apt install python3-certbot-nginx -y
+# certbot --nginx -d tg6001.YOURDOMAIN.com -d www.tg6001.YOURDOMAIN.com
+# carwellhobbot4@mail.ee, Agree, No, Redirect, True
+# certbot certificates
 # endregion
 
 
 # region payment
 async def update_subscribe(bot, BASE_D):
-    result = []
     try:
         dt_ = datetime.datetime.utcnow()
         if not (dt_.hour % 2 == 0 and dt_.minute % 2 == 0 and dt_.second % 2 == 0): return
         sql = "SELECT USER_TID, USER_LZ, USER_DTPAID, USER_ISPAID FROM USER"
         data = await db_select(sql, (), BASE_D)
 
         for item in data:
             try:
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
                 USER_TID, USER_LZ, USER_DTPAID, USER_ISPAID = item
                 get_ = await bot.get_chat(chat_id=USER_TID)
 
-                if USER_ISPAID == 1 and USER_DTPAID and (dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
+                if USER_ISPAID and USER_DTPAID and (dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
                     chan_private_donate = channel_library_ru if USER_LZ == 'ru' else channel_library_en
                     extra_bot = Bot(token=BOT_TOKEN_E18B)
                     get_chat_member_ = await extra_bot.get_chat_member(chat_id=chan_private_donate, user_id=USER_TID)
                     await extra_bot.session.close()
 
                     if get_chat_member_.status in ['member', 'administrator', 'creator']:
                         USER_DTPAID = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S')
                         sql = "UPDATE USER SET USER_ISPAID=1, USER_USERNAME=?, USER_FULLNAME=?, USER_DTPAID=? " \
                               "WHERE USER_TID=?"
                         await db_change(sql, (get_.username, get_.full_name, USER_DTPAID, USER_TID,), BASE_D)
                     else:
                         sql = "UPDATE USER SET USER_ISPAID=0, USER_USERNAME=?, USER_FULLNAME=? WHERE USER_TID=?"
                         await db_change(sql, (get_.username, get_.full_name, USER_TID, ), BASE_D)
-                elif USER_ISPAID == -1 and USER_DTPAID and (dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
-                    result.append(item)
                 else:
                     sql = "UPDATE USER SET USER_USERNAME=?, USER_FULLNAME=? WHERE USER_TID=?"
                     await db_change(sql, (get_.username, get_.full_name, USER_TID,), BASE_D)
             except TelegramRetryAfter as e:
                 logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
                 await asyncio.sleep(e.retry_after + 1)
             except Exception as e:
@@ -5223,17 +4801,14 @@
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return result
-
 # endregion
 
 
 def main():
     pass
```

