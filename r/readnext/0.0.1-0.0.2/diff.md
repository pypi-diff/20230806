# Comparing `tmp/readnext-0.0.1.tar.gz` & `tmp/readnext-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readnext-0.0.1.tar", last modified: Thu Jul 27 14:19:50 2023, max compression
+gzip compressed data, was "readnext-0.0.2.tar", last modified: Sun Aug  6 15:24:40 2023, max compression
```

## Comparing `readnext-0.0.1.tar` & `readnext-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 frederickgiasson   (501) staff       (20)        0 2023-07-27 14:19:50.823467 readnext-0.0.1/
--rw-r--r--   0 frederickgiasson   (501) staff       (20)    35134 2023-07-26 20:49:25.000000 readnext-0.0.1/LICENSE
--rw-r--r--   0 frederickgiasson   (501) staff       (20)    13859 2023-07-27 14:19:50.823109 readnext-0.0.1/PKG-INFO
--rw-r--r--   0 frederickgiasson   (501) staff       (20)    13345 2023-07-27 13:27:44.000000 readnext-0.0.1/README.md
--rw-r--r--   0 frederickgiasson   (501) staff       (20)     1092 2023-07-26 19:12:32.000000 readnext-0.0.1/pyproject.toml
-drwxr-xr-x   0 frederickgiasson   (501) staff       (20)        0 2023-07-27 14:19:50.818760 readnext-0.0.1/readnext/
--rw-r--r--   0 frederickgiasson   (501) staff       (20)      731 2023-07-26 19:48:24.000000 readnext-0.0.1/readnext/__init__.py
--rw-r--r--   0 frederickgiasson   (501) staff       (20)     8052 2023-07-26 20:51:51.000000 readnext-0.0.1/readnext/arxiv_categories.py
--rw-r--r--   0 frederickgiasson   (501) staff       (20)     3684 2023-07-26 19:11:32.000000 readnext-0.0.1/readnext/arxiv_sync.py
--rw-r--r--   0 frederickgiasson   (501) staff       (20)     3819 2023-07-26 19:10:39.000000 readnext-0.0.1/readnext/embedding.py
--rw-r--r--   0 frederickgiasson   (501) staff       (20)     3280 2023-07-26 20:47:56.000000 readnext-0.0.1/readnext/main.py
--rw-r--r--   0 frederickgiasson   (501) staff       (20)     6680 2023-07-27 14:07:35.000000 readnext-0.0.1/readnext/personalize.py
-drwxr-xr-x   0 frederickgiasson   (501) staff       (20)        0 2023-07-27 14:19:50.821039 readnext-0.0.1/readnext.egg-info/
--rw-r--r--   0 frederickgiasson   (501) staff       (20)    13859 2023-07-27 14:19:50.000000 readnext-0.0.1/readnext.egg-info/PKG-INFO
--rw-r--r--   0 frederickgiasson   (501) staff       (20)      468 2023-07-27 14:19:50.000000 readnext-0.0.1/readnext.egg-info/SOURCES.txt
--rw-r--r--   0 frederickgiasson   (501) staff       (20)        1 2023-07-27 14:19:50.000000 readnext-0.0.1/readnext.egg-info/dependency_links.txt
--rw-r--r--   0 frederickgiasson   (501) staff       (20)       47 2023-07-27 14:19:50.000000 readnext-0.0.1/readnext.egg-info/entry_points.txt
--rw-r--r--   0 frederickgiasson   (501) staff       (20)       80 2023-07-27 14:19:50.000000 readnext-0.0.1/readnext.egg-info/requires.txt
--rw-r--r--   0 frederickgiasson   (501) staff       (20)       27 2023-07-27 14:19:50.000000 readnext-0.0.1/readnext.egg-info/top_level.txt
--rw-r--r--   0 frederickgiasson   (501) staff       (20)       38 2023-07-27 14:19:50.823539 readnext-0.0.1/setup.cfg
-drwxr-xr-x   0 frederickgiasson   (501) staff       (20)        0 2023-07-27 14:19:50.822682 readnext-0.0.1/tests/
--rw-r--r--   0 frederickgiasson   (501) staff       (20)      204 2023-07-25 20:35:05.000000 readnext-0.0.1/tests/test_arxiv_categories.py
--rw-r--r--   0 frederickgiasson   (501) staff       (20)     1359 2023-07-25 20:35:08.000000 readnext-0.0.1/tests/test_arxiv_sync.py
--rw-r--r--   0 frederickgiasson   (501) staff       (20)      450 2023-07-25 20:35:03.000000 readnext-0.0.1/tests/test_embedding.py
--rw-r--r--   0 frederickgiasson   (501) staff       (20)      702 2023-07-25 20:35:01.000000 readnext-0.0.1/tests/test_personalize.py
+drwxr-xr-x   0 frederickgiasson   (501) staff       (20)        0 2023-08-06 15:24:40.804982 readnext-0.0.2/
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)    35134 2023-07-26 20:49:25.000000 readnext-0.0.2/LICENSE
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)    13996 2023-08-06 15:24:40.803854 readnext-0.0.2/PKG-INFO
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)    13482 2023-07-31 17:49:50.000000 readnext-0.0.2/README.md
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)     1092 2023-08-06 15:10:40.000000 readnext-0.0.2/pyproject.toml
+drwxr-xr-x   0 frederickgiasson   (501) staff       (20)        0 2023-08-06 15:24:40.799951 readnext-0.0.2/readnext/
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)      677 2023-08-01 12:43:56.000000 readnext-0.0.2/readnext/__init__.py
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)     8052 2023-07-26 20:51:51.000000 readnext-0.0.2/readnext/arxiv_categories.py
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)     3684 2023-07-26 19:11:32.000000 readnext-0.0.2/readnext/arxiv_sync.py
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)     3831 2023-08-01 12:49:23.000000 readnext-0.0.2/readnext/embedding.py
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)     3203 2023-07-31 17:38:54.000000 readnext-0.0.2/readnext/main.py
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)     6740 2023-08-01 15:20:16.000000 readnext-0.0.2/readnext/personalize.py
+drwxr-xr-x   0 frederickgiasson   (501) staff       (20)        0 2023-08-06 15:24:40.801708 readnext-0.0.2/readnext.egg-info/
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)    13996 2023-08-06 15:24:40.000000 readnext-0.0.2/readnext.egg-info/PKG-INFO
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)      468 2023-08-06 15:24:40.000000 readnext-0.0.2/readnext.egg-info/SOURCES.txt
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)        1 2023-08-06 15:24:40.000000 readnext-0.0.2/readnext.egg-info/dependency_links.txt
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)       47 2023-08-06 15:24:40.000000 readnext-0.0.2/readnext.egg-info/entry_points.txt
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)       80 2023-08-06 15:24:40.000000 readnext-0.0.2/readnext.egg-info/requires.txt
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)       21 2023-08-06 15:24:40.000000 readnext-0.0.2/readnext.egg-info/top_level.txt
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)       38 2023-08-06 15:24:40.805131 readnext-0.0.2/setup.cfg
+drwxr-xr-x   0 frederickgiasson   (501) staff       (20)        0 2023-08-06 15:24:40.803259 readnext-0.0.2/tests/
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)      204 2023-07-25 20:35:05.000000 readnext-0.0.2/tests/test_arxiv_categories.py
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)     1359 2023-07-25 20:35:08.000000 readnext-0.0.2/tests/test_arxiv_sync.py
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)      450 2023-07-25 20:35:03.000000 readnext-0.0.2/tests/test_embedding.py
+-rw-r--r--   0 frederickgiasson   (501) staff       (20)      702 2023-07-25 20:35:01.000000 readnext-0.0.2/tests/test_personalize.py
```

### Comparing `readnext-0.0.1/LICENSE` & `readnext-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `readnext-0.0.1/PKG-INFO` & `readnext-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: readnext
-Version: 0.0.1
-Summary: ReadNext suggests the best papers for you to read next from the ArXiv.
-Author-email: Frederick Giasson <fred@fgiasson.com>
-License: GNU GPLv3
-Project-URL: Homepage, https://github.com/fgiasson/readnext
-Project-URL: Bug Tracker, https://github.com/fgiasson/readnext/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Read Next
 ## ReadNext: A Personal Papers Recommender
 
 Every day, approximately 500 new papers are published in the `cs` category on arXiv, with tens more in `cs.AI` alone. Amidst the recent craze around Generative AI, I found it increasingly challenging to keep up with the rapid influx of papers. Distilling the ones that were most relevant to my work and my employer's interests became a daunting task.
 
 ReadNext was born out of these pressing needs:
 
@@ -61,15 +47,14 @@
 
 |Option|Description|
 |------|-----------|
 |COHERE_API_KEY| Cohere API Key as [created in their Dashboard here](https://dashboard.cohere.ai/api-keys) |
 |ZOTERO_LIBRARY_ID| Your personal library ID as defined in Zotero's backend. This [ID will appears here](https://www.zotero.org/settings/keys) as `Your userID for use in API calls is 750`|
 |ZOTERO_LIBRARY_TYPE| Type of library: `user` or `group`|
 |ZOTERO_API_KEY| You Zotero API Key, [it needs to be created and managed here](https://www.zotero.org/settings/keys).|
-|ZOTERO_INTERESTING_PAPERS_COLLECTION| This is the name/title of the Zotero Collection where you want the ReadNext papers proposals to be saved within Zotero|
 |CHROMA_DB_PATH| This is the local path where you want the embedding database management system to save its indexes (ex: `/Users/me/.readnext/chroma_db/`)|
 |DOCS_PATH| This is the local path where you want the PDF files of the papers from arXiv to be saved locally (ex: `/Users/me/.readnext/docs/`)|
 |RECOMMENDATIONS_PATH| This is the local path where you want the recommended papers to be saved locally (ex: `/Users/me/.readnext/recommendations/`)|
 
 ### Setup Environment Variables
 
 #### For Windows
@@ -109,15 +94,14 @@
 Here is what the full export looks like:
 
 ```sh
 export COHERE_API_KEY=""
 export ZOTERO_LIBRARY_ID=""
 export ZOTERO_API_KEY=""
 export ZOTERO_LIBRARY_TYPE="user"
-export ZOTERO_INTERESTING_PAPERS_COLLECTION="Propositions"
 export CHROMA_DB_PATH="/Users/[MY-USER/.readnext/chroma_db/"
 export DOCS_PATH="/Users/[MY-USER]/.readnext/docs/"
 export RECOMMENDATIONS_PATH="/Users/[MY-USER]/.readnext/recommendations/"
 ```
 
 ## How it works?
 
@@ -178,23 +162,25 @@
 To get new papers proposals, you have to run the `personalized-papers` command. That command requires two arguments:
 
  - `category`: the arXiv top, or sub, category from which you want to get new papers proposals
  - `zotero_collection`: the name of the Zotero collection where your papers of interest are stored in Zotero. This is what we refer to as the "Focus" collection above. The name of the collection is case sensitive and should be exactly as written in Zotero.
 
 Then you also have three options available:
 
- - `--save-in-zotero` / `-s`: which tells ReadNext that you want to save the proposed papers in Zotero. If you don't use this option, ReadNext will only print the proposed papers in the terminal, but will not save them in Zotero. The default behaviour is that you don't save them in Zotero.
+ - `--proposals-collection`: which tells ReadNext that you want to save the proposed papers in Zotero, in the Zotero Collection specified by the argument. If you don't use this option, ReadNext will only print the proposed papers in the terminal, but will not save them in Zotero. The default behaviour is that you don't save them in Zotero.
  - `--with-artifacts` / `-a`: which tells ReadNext that you want to save the artifacts (PDF file of the papers and their summarization) into Zotero. This is the recommended workflow, but it requires a lot more space in your Zotero account. If you want to do this, you will most likely need to subscribe to one of their paid option.
  - `--nb-proposals`: which tells ReadNext how many papers you want to be proposed. The default value is 10.
 
-The following command will propose 3 papers from the `cs.AI` caterory, based on the `Focus` collection in my Zotero library, save them in Zotero with all related artifacts:
+The following command will propose 3 papers from the `cs.AI` caterory, based on the `Readnext-Focus-LLM` collection in my Zotero library, save them in Zotero in the `Readnext-Propositions-LLM` with all related artifacts:
 
 ```sh
-readnext personalized-papers cs.AI Focus --save-in-zotero --with-artifacts --nb-proposals=3
+readnext personalized-papers cs.AI Readnext-Focus-LLM --proposals-collection=Readnext-Propositions-LLM --with-artifacts --nb-proposals=3
 ```
+As you can see, you can easily create a series of topics you want papers proposals around, where each of the topic is defined by a series of specific papers that you read and found important for your research.
+
 
 Here is what it looks like in the terminal:
 
 ![Personalized papers in CLI](images/personalized-papers-in-cli.jpg)
 
 Here is what it looks like in Zotero:
```

### Comparing `readnext-0.0.1/README.md` & `readnext-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: readnext
+Version: 0.0.2
+Summary: ReadNext suggests the best papers for you to read next from the ArXiv.
+Author-email: Frederick Giasson <fred@fgiasson.com>
+License: GNU GPLv3
+Project-URL: Homepage, https://github.com/fgiasson/readnext
+Project-URL: Bug Tracker, https://github.com/fgiasson/readnext/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Read Next
 ## ReadNext: A Personal Papers Recommender
 
 Every day, approximately 500 new papers are published in the `cs` category on arXiv, with tens more in `cs.AI` alone. Amidst the recent craze around Generative AI, I found it increasingly challenging to keep up with the rapid influx of papers. Distilling the ones that were most relevant to my work and my employer's interests became a daunting task.
 
 ReadNext was born out of these pressing needs:
 
@@ -47,15 +61,14 @@
 
 |Option|Description|
 |------|-----------|
 |COHERE_API_KEY| Cohere API Key as [created in their Dashboard here](https://dashboard.cohere.ai/api-keys) |
 |ZOTERO_LIBRARY_ID| Your personal library ID as defined in Zotero's backend. This [ID will appears here](https://www.zotero.org/settings/keys) as `Your userID for use in API calls is 750`|
 |ZOTERO_LIBRARY_TYPE| Type of library: `user` or `group`|
 |ZOTERO_API_KEY| You Zotero API Key, [it needs to be created and managed here](https://www.zotero.org/settings/keys).|
-|ZOTERO_INTERESTING_PAPERS_COLLECTION| This is the name/title of the Zotero Collection where you want the ReadNext papers proposals to be saved within Zotero|
 |CHROMA_DB_PATH| This is the local path where you want the embedding database management system to save its indexes (ex: `/Users/me/.readnext/chroma_db/`)|
 |DOCS_PATH| This is the local path where you want the PDF files of the papers from arXiv to be saved locally (ex: `/Users/me/.readnext/docs/`)|
 |RECOMMENDATIONS_PATH| This is the local path where you want the recommended papers to be saved locally (ex: `/Users/me/.readnext/recommendations/`)|
 
 ### Setup Environment Variables
 
 #### For Windows
@@ -95,15 +108,14 @@
 Here is what the full export looks like:
 
 ```sh
 export COHERE_API_KEY=""
 export ZOTERO_LIBRARY_ID=""
 export ZOTERO_API_KEY=""
 export ZOTERO_LIBRARY_TYPE="user"
-export ZOTERO_INTERESTING_PAPERS_COLLECTION="Propositions"
 export CHROMA_DB_PATH="/Users/[MY-USER/.readnext/chroma_db/"
 export DOCS_PATH="/Users/[MY-USER]/.readnext/docs/"
 export RECOMMENDATIONS_PATH="/Users/[MY-USER]/.readnext/recommendations/"
 ```
 
 ## How it works?
 
@@ -164,23 +176,25 @@
 To get new papers proposals, you have to run the `personalized-papers` command. That command requires two arguments:
 
  - `category`: the arXiv top, or sub, category from which you want to get new papers proposals
  - `zotero_collection`: the name of the Zotero collection where your papers of interest are stored in Zotero. This is what we refer to as the "Focus" collection above. The name of the collection is case sensitive and should be exactly as written in Zotero.
 
 Then you also have three options available:
 
- - `--save-in-zotero` / `-s`: which tells ReadNext that you want to save the proposed papers in Zotero. If you don't use this option, ReadNext will only print the proposed papers in the terminal, but will not save them in Zotero. The default behaviour is that you don't save them in Zotero.
+ - `--proposals-collection`: which tells ReadNext that you want to save the proposed papers in Zotero, in the Zotero Collection specified by the argument. If you don't use this option, ReadNext will only print the proposed papers in the terminal, but will not save them in Zotero. The default behaviour is that you don't save them in Zotero.
  - `--with-artifacts` / `-a`: which tells ReadNext that you want to save the artifacts (PDF file of the papers and their summarization) into Zotero. This is the recommended workflow, but it requires a lot more space in your Zotero account. If you want to do this, you will most likely need to subscribe to one of their paid option.
  - `--nb-proposals`: which tells ReadNext how many papers you want to be proposed. The default value is 10.
 
-The following command will propose 3 papers from the `cs.AI` caterory, based on the `Focus` collection in my Zotero library, save them in Zotero with all related artifacts:
+The following command will propose 3 papers from the `cs.AI` caterory, based on the `Readnext-Focus-LLM` collection in my Zotero library, save them in Zotero in the `Readnext-Propositions-LLM` with all related artifacts:
 
 ```sh
-readnext personalized-papers cs.AI Focus --save-in-zotero --with-artifacts --nb-proposals=3
+readnext personalized-papers cs.AI Readnext-Focus-LLM --proposals-collection=Readnext-Propositions-LLM --with-artifacts --nb-proposals=3
 ```
+As you can see, you can easily create a series of topics you want papers proposals around, where each of the topic is defined by a series of specific papers that you read and found important for your research.
+
 
 Here is what it looks like in the terminal:
 
 ![Personalized papers in CLI](images/personalized-papers-in-cli.jpg)
 
 Here is what it looks like in Zotero:
```

### Comparing `readnext-0.0.1/pyproject.toml` & `readnext-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
            "recommendations*",
            "scripts*",
            ".env",
            "tests*"] # excluded as package discovery, not as a package, this is why it still appears when building the readnext package
 
 [project]
 name = "readnext"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Frederick Giasson", email="fred@fgiasson.com" },
 ]
 description = "ReadNext suggests the best papers for you to read next from the ArXiv."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GNU GPLv3"}
```

### Comparing `readnext-0.0.1/readnext/__init__.py` & `readnext-0.0.2/readnext/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,13 @@
 def config_exists(env_var: str):
     v = env_var.upper()
     if not os.environ.get(v) or os.environ.get(v) == '':
         print("[bold red]Error:[/bold red] [italic red]Configuration option not set.[/italic red] [yellow]Please set the [bold]" + v + "[/bold] environment variable.[/yellow]\n")
         exit()
 
 config_exists('ZOTERO_API_KEY')
-config_exists('ZOTERO_INTERESTING_PAPERS_COLLECTION')
 config_exists('ZOTERO_LIBRARY_TYPE')
 config_exists('ZOTERO_LIBRARY_ID')
 config_exists('COHERE_API_KEY')
 config_exists('CHROMA_DB_PATH')
 config_exists('DOCS_PATH')
 config_exists('RECOMMENDATIONS_PATH')
```

### Comparing `readnext-0.0.1/readnext/arxiv_categories.py` & `readnext-0.0.2/readnext/arxiv_categories.py`

 * *Files identical despite different names*

### Comparing `readnext-0.0.1/readnext/arxiv_sync.py` & `readnext-0.0.2/readnext/arxiv_sync.py`

 * *Files identical despite different names*

### Comparing `readnext-0.0.1/readnext/embedding.py` & `readnext-0.0.2/readnext/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     chroma_client = chromadb.PersistentClient(path=os.environ.get('CHROMA_DB_PATH'))
 
     if exists(category):
         # We create two Chroma collection of embeddings:
         #   1. a general one with all and every embeddings called 'all'
         #   2. one for the specific ArXiv category
         papers_all_collection = chroma_client.get_or_create_collection(name="all")
-        papers_category_collection = chroma_client.get_or_create_collection(name=category)
+        papers_category_collection = chroma_client.get_or_create_collection(name="zotero_" + category)
 
         with Progress() as progress:
             folder_path = get_docs_path(category)
             pdfs = get_pdfs_from_folder(folder_path)
 
             task = progress.add_task("[cyan]Embedding papers...", total=len(pdfs))
```

### Comparing `readnext-0.0.1/readnext/main.py` & `readnext-0.0.2/readnext/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,49 +17,47 @@
 @app.command()
 def arxiv_sub_categories():
     "Display ArXiv sub categories. Keys are case sensitive."
     print(sub)
 
 @app.command()
 def personalized_papers(category: str, 
-                        zotero_collection: str, 
-                        save_in_zotero: Annotated[bool, 
-                                                  typer.Option("--save-in-zotero", 
-                                                               "-s",
-                                                               help="Save personalized papers in Zotero.")] = False, 
+                        focus_collection: str, 
+                        proposals_collection: Annotated[str, 
+                                                        typer.Option("--proposals-collection",
+                                                        help="Save personalized papers in Zotero in target Zotero collection.")] = "", 
                         with_artifacts: Annotated[bool, 
                                                   typer.Option("--with-artifacts", 
                                                                "-a",
                                                                help="Add paper artifacts (PDFs & summary files) to Zotero when saving.")] = False,                                                               
                         nb_proposals=10):
-    """Get personalized papers of a `zotero-collection` from an ArXiv `category`. 
+    """Get personalized papers of a `focus-collection` from an ArXiv `category`. 
     If the category is `all` then all categories that have been locally synced will be used.
-    if --in_zotero is set to True, then the papers will be uploaded to the 
-    `ZOTERO_INTERESTING_PAPERS_COLLECTION` Zotero collection, which is the default behaviour,
-    otherwise it will only be displayed to the command line.
+    if --proposals-collection is set, then the papers will be uploaded to the 
+    that Zotero collection, otherwise it will only be displayed to the command line.
     """
 
     # Step 1: Make sure the category exists
     if exists(category):
         # Step 2: get today's list of papers from arXiv
         print("[green]Syncing today's ArXiv latest papers...[/green]")
         sync_arxiv(category)
 
         # Step 3: create embeddings for each of those new papers
         print("[green]Creating embeddings for each new paper...[/green]")
         embed_category_papers(category)
 
         # Step 4: get personalized papers
         print("[green]Get personalized papers...[/green]")
-        ids = get_personalized_papers(category, zotero_collection, nb_proposals)
+        ids = get_personalized_papers(category, focus_collection, nb_proposals)
 
         # Step 5: save personalized papers in Zotero
-        if bool(save_in_zotero):
+        if proposals_collection != "":
             print("[green]Saving personalized papers in Zotero...[/green]")
-            save_personalized_papers_in_zotero(ids, with_artifacts)
+            save_personalized_papers_in_zotero(ids, proposals_collection, with_artifacts)
 
         # Step 6: display personalized papers to the command line
         search = arxiv.Search(id_list=ids.keys())
 
         for index, result in enumerate(search.results()):
             print(str(index + 1) + '. [italic yellow][' + list(ids.values())[index] + '][/italic yellow]  [blue][link=' + str(result) + ']' + result.title + '[/link][/blue]')
     else:
```

### Comparing `readnext-0.0.1/readnext/personalize.py` & `readnext-0.0.2/readnext/personalize.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,28 +39,29 @@
 
     for item in get_target_collection_items(collection_name):
         if item['data']['itemType'] != 'attachment':
             if 'title' in item['data']:
                 interests_corpus = interests_corpus + ' ' + item['data']['title']
             if 'abstractNote' in item['data']:
                 interests_corpus = interests_corpus + ' ' + item['data']['abstractNote']
+                # TODO adding authors to the embedding space
             interests_corpus = interests_corpus + ' ' + '\n'
     
     return interests_corpus
 
 def get_personalized_papers(category: str, zotero_collection: str, nb_proposals=10):
     """Given a ArXiv category and a Zotero personalization collection. 
     Returns a dictionary where the keys are the personalized ArXiv IDs, 
     and the value the distance to the personalization embedding."""
     chroma_client = chromadb.PersistentClient(path=os.environ.get('CHROMA_DB_PATH'))
     
     ids = {}
 
     if exists(category):
-        papers_category_collection = chroma_client.get_or_create_collection(name=category)
+        papers_category_collection = chroma_client.get_or_create_collection(name="zotero_" + category)
 
         co = cohere.Client(os.environ.get('COHERE_API_KEY'))
 
         interests_embedding = co.embed([create_interests_corpus(zotero_collection)])
 
         interesting_papers = papers_category_collection.query(
             query_embeddings=interests_embedding.embeddings,
@@ -76,42 +77,42 @@
 
     co = cohere.Client(os.environ.get('COHERE_API_KEY'))
 
     res = co.summarize(text[:100000], length='medium')
 
     return res.summary
 
-def check_already_in_zotero_proposals(title: str):
+def check_already_in_zotero_proposals(title: str, proposals_collection: str):
     """Check if a paper is already in the proposals collection."""
-    for item in get_target_collection_items(os.environ.get('ZOTERO_INTERESTING_PAPERS_COLLECTION')):
+    for item in get_target_collection_items(proposals_collection):
         if item['data']['itemType'] != 'attachment':
             if 'title' in item['data']:
                 if item['data']['title'] == title:
                     return True
     
     return False
 
-def save_personalized_papers_in_zotero(ids: dict, with_artifacts: bool):
+def save_personalized_papers_in_zotero(ids: dict, proposals_collection, with_artifacts: bool):
     """Get all personalized papers propositions and upload them to the 
-    `ZOTERO_INTERESTING_PAPERS_COLLECTION` Zotero collection.
+    `proposals_collection` Zotero collection.
     
     If `with_artifacts=True`, then all documents artifacts will be
     uploaded to Zotero as well (namely PDFs and summary documents), 
     but it will take more space to the Zotero account and will be 
     slower to process."""
 
     # get information for each matched articles directly from ArXiv
     search = arxiv.Search(id_list=ids.keys())
 
     with Progress() as progress:
         task = progress.add_task("[cyan]Uploading papers to Zotero...", total=len(list(search.results())))
 
         for index, result in enumerate(search.results()):
             # skip if the paper is already in the proposals collection
-            if(check_already_in_zotero_proposals(result.title)):
+            if(check_already_in_zotero_proposals(result.title, proposals_collection)):
                 if not progress.finished:
                     progress.update(task, advance=1)
                 continue
 
             # build the template for the Zotero item
             template = zot.item_template('preprint')
 
@@ -125,15 +126,15 @@
             template['abstractNote'] = result.summary
             template['creators'] = creators
             template['url'] = result.entry_id
             template['DOI'] = result.doi
             template['repository'] = 'arXiv'
             template['archiveID'] = 'arxiv:' + result.get_short_id()
             template['libraryCatalog'] = 'arXiv.org'
-            template['collections'] = [get_collection_id_from_name(os.environ.get('ZOTERO_INTERESTING_PAPERS_COLLECTION'))]
+            template['collections'] = [get_collection_id_from_name(proposals_collection)]
 
             zot.check_items([template])
 
             resp = zot.create_items([template])
 
             if '0' in resp['success']:
                 if(with_artifacts):
```

### Comparing `readnext-0.0.1/readnext.egg-info/PKG-INFO` & `readnext-0.0.2/readnext.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readnext
-Version: 0.0.1
+Version: 0.0.2
 Summary: ReadNext suggests the best papers for you to read next from the ArXiv.
 Author-email: Frederick Giasson <fred@fgiasson.com>
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/fgiasson/readnext
 Project-URL: Bug Tracker, https://github.com/fgiasson/readnext/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -61,15 +61,14 @@
 
 |Option|Description|
 |------|-----------|
 |COHERE_API_KEY| Cohere API Key as [created in their Dashboard here](https://dashboard.cohere.ai/api-keys) |
 |ZOTERO_LIBRARY_ID| Your personal library ID as defined in Zotero's backend. This [ID will appears here](https://www.zotero.org/settings/keys) as `Your userID for use in API calls is 750`|
 |ZOTERO_LIBRARY_TYPE| Type of library: `user` or `group`|
 |ZOTERO_API_KEY| You Zotero API Key, [it needs to be created and managed here](https://www.zotero.org/settings/keys).|
-|ZOTERO_INTERESTING_PAPERS_COLLECTION| This is the name/title of the Zotero Collection where you want the ReadNext papers proposals to be saved within Zotero|
 |CHROMA_DB_PATH| This is the local path where you want the embedding database management system to save its indexes (ex: `/Users/me/.readnext/chroma_db/`)|
 |DOCS_PATH| This is the local path where you want the PDF files of the papers from arXiv to be saved locally (ex: `/Users/me/.readnext/docs/`)|
 |RECOMMENDATIONS_PATH| This is the local path where you want the recommended papers to be saved locally (ex: `/Users/me/.readnext/recommendations/`)|
 
 ### Setup Environment Variables
 
 #### For Windows
@@ -109,15 +108,14 @@
 Here is what the full export looks like:
 
 ```sh
 export COHERE_API_KEY=""
 export ZOTERO_LIBRARY_ID=""
 export ZOTERO_API_KEY=""
 export ZOTERO_LIBRARY_TYPE="user"
-export ZOTERO_INTERESTING_PAPERS_COLLECTION="Propositions"
 export CHROMA_DB_PATH="/Users/[MY-USER/.readnext/chroma_db/"
 export DOCS_PATH="/Users/[MY-USER]/.readnext/docs/"
 export RECOMMENDATIONS_PATH="/Users/[MY-USER]/.readnext/recommendations/"
 ```
 
 ## How it works?
 
@@ -178,23 +176,25 @@
 To get new papers proposals, you have to run the `personalized-papers` command. That command requires two arguments:
 
  - `category`: the arXiv top, or sub, category from which you want to get new papers proposals
  - `zotero_collection`: the name of the Zotero collection where your papers of interest are stored in Zotero. This is what we refer to as the "Focus" collection above. The name of the collection is case sensitive and should be exactly as written in Zotero.
 
 Then you also have three options available:
 
- - `--save-in-zotero` / `-s`: which tells ReadNext that you want to save the proposed papers in Zotero. If you don't use this option, ReadNext will only print the proposed papers in the terminal, but will not save them in Zotero. The default behaviour is that you don't save them in Zotero.
+ - `--proposals-collection`: which tells ReadNext that you want to save the proposed papers in Zotero, in the Zotero Collection specified by the argument. If you don't use this option, ReadNext will only print the proposed papers in the terminal, but will not save them in Zotero. The default behaviour is that you don't save them in Zotero.
  - `--with-artifacts` / `-a`: which tells ReadNext that you want to save the artifacts (PDF file of the papers and their summarization) into Zotero. This is the recommended workflow, but it requires a lot more space in your Zotero account. If you want to do this, you will most likely need to subscribe to one of their paid option.
  - `--nb-proposals`: which tells ReadNext how many papers you want to be proposed. The default value is 10.
 
-The following command will propose 3 papers from the `cs.AI` caterory, based on the `Focus` collection in my Zotero library, save them in Zotero with all related artifacts:
+The following command will propose 3 papers from the `cs.AI` caterory, based on the `Readnext-Focus-LLM` collection in my Zotero library, save them in Zotero in the `Readnext-Propositions-LLM` with all related artifacts:
 
 ```sh
-readnext personalized-papers cs.AI Focus --save-in-zotero --with-artifacts --nb-proposals=3
+readnext personalized-papers cs.AI Readnext-Focus-LLM --proposals-collection=Readnext-Propositions-LLM --with-artifacts --nb-proposals=3
 ```
+As you can see, you can easily create a series of topics you want papers proposals around, where each of the topic is defined by a series of specific papers that you read and found important for your research.
+
 
 Here is what it looks like in the terminal:
 
 ![Personalized papers in CLI](images/personalized-papers-in-cli.jpg)
 
 Here is what it looks like in Zotero:
```

### Comparing `readnext-0.0.1/tests/test_arxiv_sync.py` & `readnext-0.0.2/tests/test_arxiv_sync.py`

 * *Files identical despite different names*

### Comparing `readnext-0.0.1/tests/test_personalize.py` & `readnext-0.0.2/tests/test_personalize.py`

 * *Files identical despite different names*

