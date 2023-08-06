# Comparing `tmp/fastapi_gen-0.3.0.tar.gz` & `tmp/fastapi_gen-0.4.0.tar.gz`

## Comparing `fastapi_gen-0.3.0.tar` & `fastapi_gen-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,46 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/cli/__init__.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/cli/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/__init__.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/.gitignore
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/main.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/requirements.txt
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/hello_world/test_main.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/.env_dev
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/.gitignore
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/__init__.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/main.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/requirements.txt
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/langchain/test_main.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/.env_dev
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/.gitignore
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/main.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/requirements.txt
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/src/templates/nlp/test_main.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/LICENSE
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/README.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 fastapi_gen-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/cli/__init__.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/cli/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/__init__.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/.gitignore
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/main.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/tests/__init__.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/tests/test_main.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/.env_dev
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/__init__.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/main.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/tests/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/tests/test_main.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/.env_dev
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/main.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/models/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/tests/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/tests/test_main.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/.env_dev
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/main.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/tests/__init__.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/tests/test_main.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/README.md
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/PKG-INFO
```

### Comparing `fastapi_gen-0.3.0/src/cli/__main__.py` & `fastapi_gen-0.4.0/src/cli/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,34 @@
 
     modified_content = content.replace(old_string, new_string)
 
     with open(file_path, "w") as file:
         file.write(modified_content)
 
 
-_choices = ["hello_world", "nlp", "langchain"]
+_choices = ["hello_world", "nlp", "langchain", "llama"]
 
+def _create_dir(path: str):
+    try:
+        os.makedirs(path)
+        click.echo(f"Folder '{path}' created successfully.")
+    except OSError as e:
+        click.echo(f"Error creating folder: {e}")
+
+def _walk_resources(package: str, path: str = ""):
+    for file in resources.files(package).iterdir():
+        if file.name in ["__pycache__", ".pytest_cache", "venv"]:
+            continue
+
+        if file.is_dir():
+            _create_dir(os.path.join(path, file.name))
+            _walk_resources(f"{package}.{file.name}", os.path.join(path, file.name))
+        else:
+            with open(os.path.join(path, file.name), "w") as f:
+                f.write(resources.read_text(package, file.name))
 
 @click.command()
 @click.option("-t", "--template", default="hello_world", type=click.Choice(_choices), help="template")
 @click.argument("name")
 @click.version_option(version=__version__, prog_name="create-fast-api")
 def fastapi_create(name: str, template: str):
     """This script creates new FastAPI project with NAME using TEMPLATE."""
@@ -42,31 +60,20 @@
     new_project_path = os.path.join(current_folder, name)
     os.path.join(current_folder, "src", "templates", template)
 
     if os.path.exists(new_project_path):
         click.echo(f"Error. Folder {new_project_path} already exists.")
         sys.exit(1)
 
-    try:
-        os.makedirs(new_project_path)
-        click.echo(f"Folder '{new_project_path}' created successfully.")
-    except OSError as e:
-        click.echo(f"Error creating folder: {e}")
-
-    package = f"templates.{template}"
-    for file in resources.files(package).iterdir():
-        if file.name in ["__pycache__", ".pytest_cache", "venv"]:
-            continue
-
-        with open(os.path.join(new_project_path, file.name), "w") as f:
-            f.write(resources.read_text(package, file.name))
+    _create_dir(new_project_path)
+    _walk_resources(f"templates.{template}", new_project_path)
 
     os.chdir(new_project_path)
 
-    replace_string_in_file(os.path.join(new_project_path, "test_main.py"), f"src.templates.{template}", name)
+    replace_string_in_file(os.path.join(new_project_path, "tests", "test_main.py"), f"src.templates.{template}", name)
 
     try:
         subprocess.run(["make", "init"], check=True)
     except subprocess.CalledProcessError as e:
         click.echo(f"An error occurred while executing the Makefile: {e}")
         sys.exit(1)
```

### Comparing `fastapi_gen-0.3.0/src/templates/hello_world/.gitignore` & `fastapi_gen-0.4.0/src/templates/hello_world/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/hello_world/README.md` & `fastapi_gen-0.4.0/src/templates/hello_world/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/hello_world/main.py` & `fastapi_gen-0.4.0/src/templates/hello_world/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/hello_world/test_main.py` & `fastapi_gen-0.4.0/src/templates/hello_world/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/langchain/.gitignore` & `fastapi_gen-0.4.0/src/templates/langchain/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/langchain/README.md` & `fastapi_gen-0.4.0/src/templates/langchain/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/langchain/main.py` & `fastapi_gen-0.4.0/src/templates/langchain/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/langchain/test_main.py` & `fastapi_gen-0.4.0/src/templates/langchain/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/nlp/.gitignore` & `fastapi_gen-0.4.0/src/templates/nlp/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/nlp/README.md` & `fastapi_gen-0.4.0/src/templates/llama/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/nlp/main.py` & `fastapi_gen-0.4.0/src/templates/nlp/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/src/templates/nlp/test_main.py` & `fastapi_gen-0.4.0/src/templates/nlp/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/.gitignore` & `fastapi_gen-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/LICENSE` & `fastapi_gen-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/README.md` & `fastapi_gen-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # FastApi Gen
 
-Create FastAPI apps with no build configuration.
+Create LLM-enabled FastAPI applications without build configuration.
 
 <a href="https://github.com/mirpo/fastapi-gen/actions/workflows/test.yml?query=workflow%3Atest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://github.com/mirpo/fastapi-gen/actions/workflows/test.yml/badge.svg?branch=master" alt="Test">
 </a>
 <a href="https://pypi.org/project/fastapi-gen" target="_blank">
     <img src="https://img.shields.io/pypi/v/fastapi-gen?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
@@ -13,24 +13,14 @@
 </a>
 
 ---
 
 FastApi Gen works on macOS and Linux.<br>
 If something doesn’t work, please [file an issue](https://github.com/mirpo/fastapi-gen/issues/new).
 
-Available templates:
-
-1. Default - basic template with GET/POST examples.
-2. NLP - natural language processing template with examples how to use local Hugginface models for summarization, named-entity recognition and text generation using LLM.
-3. Langchain - template with examples how to use LangChain with local Hugginface models (LLMs) for text generation and question answering.
-
-*Important note* - Langchain template requires hardware to run and will automatically download required models, be patient.
-
-More to come!
-
 ## Quick Overview
 
 ```console
 pip3 install fastapi-gen
 fastapi-gen my_app
 cd my_app
 make start-dev
@@ -44,26 +34,39 @@
 make start-dev
 ```
 
 If you've previously installed `fastapi-gen` globally via `pip3 install fastapi-gen`, we recommend you reinstall the package using `pip3 install --upgrade --force-reinstall fastapi-gen` or `pipx upgrade fastapi-gen` to ensure that you use the latest version.
 
 Then open http://localhost:8000/docs to see your app OpenAPI documentation.
 
+Available templates:
+
+1. Default - basic template with GET/POST examples.
+2. NLP - natural language processing template with examples how to use local Hugginface models for summarization, named-entity recognition and text generation using LLM.
+3. Langchain - template with examples how to use LangChain with local Hugginface models (LLMs) for text generation and question answering.
+4. Llama - template with examples how to use llama.cpp and llama-cpp-python with local Llama 2 for question asnwering.
+
+*Important notes*:
+- Langchain template requires hardware to run and will automatically download required models, be patient.
+- Llama template will download around 4GB model from Hugginface and >4GB of RAM.
+
+Each template includes not only code, but also **tests**.
+
 ### Get Started Immediately
 
 You **don’t** need to install or configure depencendeices like FastApi or Pytest.<br>
 They are preconfigured and hidden so that you can focus on the code.
 
 Create a project, and you’re good to go.
 
 ## Creating an App
 
 **You’ll need to have Python 3.7+ or later version on your local development machine**. We recommend using the latest LTS version. You can use [pyenv](https://github.com/pyenv/pyenv) (macOS/Linux) to switch Python versions between different projects.
 
-### basic template
+### Basic template
 
 ```console
 pip3 install fastapi-gen
 fastapi-gen my_app
 ```
 
 or
@@ -83,14 +86,21 @@
 ### Langchain template
 
 ```console
 pip install fastapi-gen
 fastapi-gen my_app --template Langchain
 ```
 
+### Llama template
+
+```console
+pip install fastapi-gen
+fastapi-gen my_app --template llama
+```
+
 Inside the newly created project, you can run some built-in commands:
 
 ### `make start`
 
 Runs the app in development mode.<br>
 Open [http://localhost:8000/docs](http://localhost:8000/docs) to view OpenAPI documentation in the browser.
```

#### html2text {}

```diff
@@ -1,36 +1,42 @@
-# FastApi Gen Create FastAPI apps with no build configuration. [Test] [Package
-version] [Supported_Python_versions] --- FastApi Gen works on macOS and Linux.
+# FastApi Gen Create LLM-enabled FastAPI applications without build
+configuration. [Test] [Package_version] [Supported_Python_versions] --- FastApi
+Gen works on macOS and Linux.
 If something doesnât work, please [file an issue](https://github.com/mirpo/
-fastapi-gen/issues/new). Available templates: 1. Default - basic template with
-GET/POST examples. 2. NLP - natural language processing template with examples
-how to use local Hugginface models for summarization, named-entity recognition
-and text generation using LLM. 3. Langchain - template with examples how to use
+fastapi-gen/issues/new). ## Quick Overview ```console pip3 install fastapi-gen
+fastapi-gen my_app cd my_app make start-dev ``` or ```console pipx run fastapi-
+gen my_app cd my_app make start-dev ``` If you've previously installed
+`fastapi-gen` globally via `pip3 install fastapi-gen`, we recommend you
+reinstall the package using `pip3 install --upgrade --force-reinstall fastapi-
+gen` or `pipx upgrade fastapi-gen` to ensure that you use the latest version.
+Then open http://localhost:8000/docs to see your app OpenAPI documentation.
+Available templates: 1. Default - basic template with GET/POST examples. 2. NLP
+- natural language processing template with examples how to use local
+Hugginface models for summarization, named-entity recognition and text
+generation using LLM. 3. Langchain - template with examples how to use
 LangChain with local Hugginface models (LLMs) for text generation and question
-answering. *Important note* - Langchain template requires hardware to run and
-will automatically download required models, be patient. More to come! ## Quick
-Overview ```console pip3 install fastapi-gen fastapi-gen my_app cd my_app make
-start-dev ``` or ```console pipx run fastapi-gen my_app cd my_app make start-
-dev ``` If you've previously installed `fastapi-gen` globally via `pip3 install
-fastapi-gen`, we recommend you reinstall the package using `pip3 install --
-upgrade --force-reinstall fastapi-gen` or `pipx upgrade fastapi-gen` to ensure
-that you use the latest version. Then open http://localhost:8000/docs to see
-your app OpenAPI documentation. ### Get Started Immediately You **donât**
-need to install or configure depencendeices like FastApi or Pytest.
+answering. 4. Llama - template with examples how to use llama.cpp and llama-
+cpp-python with local Llama 2 for question asnwering. *Important notes*: -
+Langchain template requires hardware to run and will automatically download
+required models, be patient. - Llama template will download around 4GB model
+from Hugginface and >4GB of RAM. Each template includes not only code, but also
+**tests**. ### Get Started Immediately You **donât** need to install or
+configure depencendeices like FastApi or Pytest.
 They are preconfigured and hidden so that you can focus on the code. Create a
 project, and youâre good to go. ## Creating an App **Youâll need to have
 Python 3.7+ or later version on your local development machine**. We recommend
 using the latest LTS version. You can use [pyenv](https://github.com/pyenv/
 pyenv) (macOS/Linux) to switch Python versions between different projects. ###
-basic template ```console pip3 install fastapi-gen fastapi-gen my_app ``` or
+Basic template ```console pip3 install fastapi-gen fastapi-gen my_app ``` or
 ```console pip3 install fastapi-gen fastapi-gen my_app --template hello_world
 ``` ### NLP template ```console pip install fastapi-gen fastapi-gen my_app --
 template nlp ``` ### Langchain template ```console pip install fastapi-gen
-fastapi-gen my_app --template Langchain ``` Inside the newly created project,
-you can run some built-in commands: ### `make start` Runs the app in
-development mode.
+fastapi-gen my_app --template Langchain ``` ### Llama template ```console pip
+install fastapi-gen fastapi-gen my_app --template llama ``` Inside the newly
+created project, you can run some built-in commands: ### `make start` Runs the
+app in development mode.
 Open [http://localhost:8000/docs](http://localhost:8000/docs) to view OpenAPI
 documentation in the browser. The page will automatically reload if you make
 changes to the code. ### `make test` Runs tests.
 By default, runs tests related to files changed since the last commit. ##
 License `fastapi-gen` is distributed under the terms of the [MIT](https://
 github.com/mirpo/fastapi-gen/blob/master/LICENSE) license.
```

### Comparing `fastapi_gen-0.3.0/pyproject.toml` & `fastapi_gen-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.3.0/PKG-INFO` & `fastapi_gen-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-gen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Set up a modern REST API by running one command.
 Project-URL: Documentation, https://github.com/mirpo/fastapi-gen#readme
 Project-URL: Issues, https://github.com/mirpo/fastapi-gen/issues
 Project-URL: Source, https://github.com/mirpo/fastapi-gen
 Author-email: Miroslav Pokrovskii <miroslavpokrovskiy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -40,15 +40,15 @@
 Requires-Dist: importlib-resources==6.0.0
 Provides-Extra: dev
 Requires-Dist: ruff==0.0.280; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # FastApi Gen
 
-Create FastAPI apps with no build configuration.
+Create LLM-enabled FastAPI applications without build configuration.
 
 <a href="https://github.com/mirpo/fastapi-gen/actions/workflows/test.yml?query=workflow%3Atest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://github.com/mirpo/fastapi-gen/actions/workflows/test.yml/badge.svg?branch=master" alt="Test">
 </a>
 <a href="https://pypi.org/project/fastapi-gen" target="_blank">
     <img src="https://img.shields.io/pypi/v/fastapi-gen?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
@@ -57,24 +57,14 @@
 </a>
 
 ---
 
 FastApi Gen works on macOS and Linux.<br>
 If something doesn’t work, please [file an issue](https://github.com/mirpo/fastapi-gen/issues/new).
 
-Available templates:
-
-1. Default - basic template with GET/POST examples.
-2. NLP - natural language processing template with examples how to use local Hugginface models for summarization, named-entity recognition and text generation using LLM.
-3. Langchain - template with examples how to use LangChain with local Hugginface models (LLMs) for text generation and question answering.
-
-*Important note* - Langchain template requires hardware to run and will automatically download required models, be patient.
-
-More to come!
-
 ## Quick Overview
 
 ```console
 pip3 install fastapi-gen
 fastapi-gen my_app
 cd my_app
 make start-dev
@@ -88,26 +78,39 @@
 make start-dev
 ```
 
 If you've previously installed `fastapi-gen` globally via `pip3 install fastapi-gen`, we recommend you reinstall the package using `pip3 install --upgrade --force-reinstall fastapi-gen` or `pipx upgrade fastapi-gen` to ensure that you use the latest version.
 
 Then open http://localhost:8000/docs to see your app OpenAPI documentation.
 
+Available templates:
+
+1. Default - basic template with GET/POST examples.
+2. NLP - natural language processing template with examples how to use local Hugginface models for summarization, named-entity recognition and text generation using LLM.
+3. Langchain - template with examples how to use LangChain with local Hugginface models (LLMs) for text generation and question answering.
+4. Llama - template with examples how to use llama.cpp and llama-cpp-python with local Llama 2 for question asnwering.
+
+*Important notes*:
+- Langchain template requires hardware to run and will automatically download required models, be patient.
+- Llama template will download around 4GB model from Hugginface and >4GB of RAM.
+
+Each template includes not only code, but also **tests**.
+
 ### Get Started Immediately
 
 You **don’t** need to install or configure depencendeices like FastApi or Pytest.<br>
 They are preconfigured and hidden so that you can focus on the code.
 
 Create a project, and you’re good to go.
 
 ## Creating an App
 
 **You’ll need to have Python 3.7+ or later version on your local development machine**. We recommend using the latest LTS version. You can use [pyenv](https://github.com/pyenv/pyenv) (macOS/Linux) to switch Python versions between different projects.
 
-### basic template
+### Basic template
 
 ```console
 pip3 install fastapi-gen
 fastapi-gen my_app
 ```
 
 or
@@ -127,14 +130,21 @@
 ### Langchain template
 
 ```console
 pip install fastapi-gen
 fastapi-gen my_app --template Langchain
 ```
 
+### Llama template
+
+```console
+pip install fastapi-gen
+fastapi-gen my_app --template llama
+```
+
 Inside the newly created project, you can run some built-in commands:
 
 ### `make start`
 
 Runs the app in development mode.<br>
 Open [http://localhost:8000/docs](http://localhost:8000/docs) to view OpenAPI documentation in the browser.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-gen Version: 0.3.0 Summary: Set up a modern
+Metadata-Version: 2.1 Name: fastapi-gen Version: 0.4.0 Summary: Set up a modern
 REST API by running one command. Project-URL: Documentation, https://
 github.com/mirpo/fastapi-gen#readme Project-URL: Issues, https://github.com/
 mirpo/fastapi-gen/issues Project-URL: Source, https://github.com/mirpo/fastapi-
 gen Author-email: Miroslav Pokrovskii
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 cli,fastapi,hello world,huggingface,langchain,llama,llama.cpp,named-entity
 recognition,ner,nlp,summarization,text generation Classifier: Development
@@ -20,44 +20,49 @@
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Typing :: Typed Requires-Python: >=3.10 Requires-Dist:
 click==8.1.6 Requires-Dist: colorama==0.4.6 Requires-Dist: importlib-
 resources==6.0.0 Provides-Extra: dev Requires-Dist: ruff==0.0.280; extra ==
-'dev' Description-Content-Type: text/markdown # FastApi Gen Create FastAPI apps
-with no build configuration. [Test] [Package_version] [Supported_Python
-versions] --- FastApi Gen works on macOS and Linux.
+'dev' Description-Content-Type: text/markdown # FastApi Gen Create LLM-enabled
+FastAPI applications without build configuration. [Test] [Package_version]
+[Supported_Python_versions] --- FastApi Gen works on macOS and Linux.
 If something doesnât work, please [file an issue](https://github.com/mirpo/
-fastapi-gen/issues/new). Available templates: 1. Default - basic template with
-GET/POST examples. 2. NLP - natural language processing template with examples
-how to use local Hugginface models for summarization, named-entity recognition
-and text generation using LLM. 3. Langchain - template with examples how to use
+fastapi-gen/issues/new). ## Quick Overview ```console pip3 install fastapi-gen
+fastapi-gen my_app cd my_app make start-dev ``` or ```console pipx run fastapi-
+gen my_app cd my_app make start-dev ``` If you've previously installed
+`fastapi-gen` globally via `pip3 install fastapi-gen`, we recommend you
+reinstall the package using `pip3 install --upgrade --force-reinstall fastapi-
+gen` or `pipx upgrade fastapi-gen` to ensure that you use the latest version.
+Then open http://localhost:8000/docs to see your app OpenAPI documentation.
+Available templates: 1. Default - basic template with GET/POST examples. 2. NLP
+- natural language processing template with examples how to use local
+Hugginface models for summarization, named-entity recognition and text
+generation using LLM. 3. Langchain - template with examples how to use
 LangChain with local Hugginface models (LLMs) for text generation and question
-answering. *Important note* - Langchain template requires hardware to run and
-will automatically download required models, be patient. More to come! ## Quick
-Overview ```console pip3 install fastapi-gen fastapi-gen my_app cd my_app make
-start-dev ``` or ```console pipx run fastapi-gen my_app cd my_app make start-
-dev ``` If you've previously installed `fastapi-gen` globally via `pip3 install
-fastapi-gen`, we recommend you reinstall the package using `pip3 install --
-upgrade --force-reinstall fastapi-gen` or `pipx upgrade fastapi-gen` to ensure
-that you use the latest version. Then open http://localhost:8000/docs to see
-your app OpenAPI documentation. ### Get Started Immediately You **donât**
-need to install or configure depencendeices like FastApi or Pytest.
+answering. 4. Llama - template with examples how to use llama.cpp and llama-
+cpp-python with local Llama 2 for question asnwering. *Important notes*: -
+Langchain template requires hardware to run and will automatically download
+required models, be patient. - Llama template will download around 4GB model
+from Hugginface and >4GB of RAM. Each template includes not only code, but also
+**tests**. ### Get Started Immediately You **donât** need to install or
+configure depencendeices like FastApi or Pytest.
 They are preconfigured and hidden so that you can focus on the code. Create a
 project, and youâre good to go. ## Creating an App **Youâll need to have
 Python 3.7+ or later version on your local development machine**. We recommend
 using the latest LTS version. You can use [pyenv](https://github.com/pyenv/
 pyenv) (macOS/Linux) to switch Python versions between different projects. ###
-basic template ```console pip3 install fastapi-gen fastapi-gen my_app ``` or
+Basic template ```console pip3 install fastapi-gen fastapi-gen my_app ``` or
 ```console pip3 install fastapi-gen fastapi-gen my_app --template hello_world
 ``` ### NLP template ```console pip install fastapi-gen fastapi-gen my_app --
 template nlp ``` ### Langchain template ```console pip install fastapi-gen
-fastapi-gen my_app --template Langchain ``` Inside the newly created project,
-you can run some built-in commands: ### `make start` Runs the app in
-development mode.
+fastapi-gen my_app --template Langchain ``` ### Llama template ```console pip
+install fastapi-gen fastapi-gen my_app --template llama ``` Inside the newly
+created project, you can run some built-in commands: ### `make start` Runs the
+app in development mode.
 Open [http://localhost:8000/docs](http://localhost:8000/docs) to view OpenAPI
 documentation in the browser. The page will automatically reload if you make
 changes to the code. ### `make test` Runs tests.
 By default, runs tests related to files changed since the last commit. ##
 License `fastapi-gen` is distributed under the terms of the [MIT](https://
 github.com/mirpo/fastapi-gen/blob/master/LICENSE) license.
```

