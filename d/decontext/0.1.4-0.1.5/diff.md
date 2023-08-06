# Comparing `tmp/decontext-0.1.4.tar.gz` & `tmp/decontext-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decontext-0.1.4.tar", last modified: Thu Aug  3 22:05:12 2023, max compression
+gzip compressed data, was "decontext-0.1.5.tar", last modified: Sun Aug  6 08:33:49 2023, max compression
```

## Comparing `decontext-0.1.4.tar` & `decontext-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-03 22:05:12.159716 decontext-0.1.4/
--rw-r--r--   0 benjaminn   (502) staff       (20)    13886 2023-08-03 22:05:12.159440 decontext-0.1.4/PKG-INFO
--rw-r--r--   0 benjaminn   (502) staff       (20)    12767 2023-08-02 22:45:19.000000 decontext-0.1.4/README.md
--rw-r--r--   0 benjaminn   (502) staff       (20)     3301 2023-08-03 22:04:56.000000 decontext-0.1.4/pyproject.toml
--rw-r--r--   0 benjaminn   (502) staff       (20)       38 2023-08-03 22:05:12.159769 decontext-0.1.4/setup.cfg
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-03 22:05:12.152057 decontext-0.1.4/src/
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-03 22:05:12.155266 decontext-0.1.4/src/decontext/
--rw-r--r--   0 benjaminn   (502) staff       (20)      120 2023-08-02 21:27:06.000000 decontext-0.1.4/src/decontext/__init__.py
--rw-r--r--   0 benjaminn   (502) staff       (20)     6676 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/cache.py
--rw-r--r--   0 benjaminn   (502) staff       (20)     6503 2023-08-02 22:45:19.000000 decontext-0.1.4/src/decontext/data_types.py
--rw-r--r--   0 benjaminn   (502) staff       (20)      115 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/logging.py
--rw-r--r--   0 benjaminn   (502) staff       (20)    13550 2023-08-03 21:51:35.000000 decontext-0.1.4/src/decontext/model.py
--rw-r--r--   0 benjaminn   (502) staff       (20)     2782 2023-08-02 22:45:19.000000 decontext-0.1.4/src/decontext/pipeline.py
--rw-r--r--   0 benjaminn   (502) staff       (20)        0 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/py.typed
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-03 22:05:12.157167 decontext-0.1.4/src/decontext/step/
--rw-r--r--   0 benjaminn   (502) staff       (20)     6148 2023-08-02 22:45:19.000000 decontext-0.1.4/src/decontext/step/qa.py
--rw-r--r--   0 benjaminn   (502) staff       (20)      767 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/step/qgen.py
--rw-r--r--   0 benjaminn   (502) staff       (20)     1033 2023-08-02 21:29:03.000000 decontext-0.1.4/src/decontext/step/step.py
--rw-r--r--   0 benjaminn   (502) staff       (20)      788 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/step/synth.py
--rw-r--r--   0 benjaminn   (502) staff       (20)     4115 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/template.py
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-03 22:05:12.158125 decontext-0.1.4/src/decontext/templates/
--rw-r--r--   0 benjaminn   (502) staff       (20)        0 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/templates/__init__.py
--rw-r--r--   0 benjaminn   (502) staff       (20)      624 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/templates/qa_fulltext.yaml
--rw-r--r--   0 benjaminn   (502) staff       (20)      957 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/templates/qa_retrieval.yaml
--rw-r--r--   0 benjaminn   (502) staff       (20)     1045 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/templates/qgen.yaml
--rw-r--r--   0 benjaminn   (502) staff       (20)     1456 2023-08-01 22:11:18.000000 decontext-0.1.4/src/decontext/templates/synth.yaml
--rw-r--r--   0 benjaminn   (502) staff       (20)     1124 2023-08-02 22:45:19.000000 decontext-0.1.4/src/decontext/utils.py
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-03 22:05:12.156195 decontext-0.1.4/src/decontext.egg-info/
--rw-r--r--   0 benjaminn   (502) staff       (20)    13886 2023-08-03 22:05:12.000000 decontext-0.1.4/src/decontext.egg-info/PKG-INFO
--rw-r--r--   0 benjaminn   (502) staff       (20)      834 2023-08-03 22:05:12.000000 decontext-0.1.4/src/decontext.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminn   (502) staff       (20)        1 2023-08-03 22:05:12.000000 decontext-0.1.4/src/decontext.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminn   (502) staff       (20)      509 2023-08-03 22:05:12.000000 decontext-0.1.4/src/decontext.egg-info/requires.txt
--rw-r--r--   0 benjaminn   (502) staff       (20)       10 2023-08-03 22:05:12.000000 decontext-0.1.4/src/decontext.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-03 22:05:12.159165 decontext-0.1.4/tests/
--rw-r--r--   0 benjaminn   (502) staff       (20)     2158 2023-08-03 21:51:35.000000 decontext-0.1.4/tests/test_cache.py
--rw-r--r--   0 benjaminn   (502) staff       (20)     1052 2023-08-01 22:11:18.000000 decontext-0.1.4/tests/test_data_types.py
--rw-r--r--   0 benjaminn   (502) staff       (20)      653 2023-08-02 22:45:19.000000 decontext-0.1.4/tests/test_model.py
--rw-r--r--   0 benjaminn   (502) staff       (20)     9068 2023-08-03 21:51:35.000000 decontext-0.1.4/tests/test_pipeline.py
--rw-r--r--   0 benjaminn   (502) staff       (20)      493 2023-08-02 22:45:19.000000 decontext-0.1.4/tests/test_utils.py
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-06 08:33:49.731232 decontext-0.1.5/
+-rw-r--r--   0 benjaminn   (502) staff       (20)    13886 2023-08-06 08:33:49.730952 decontext-0.1.5/PKG-INFO
+-rw-r--r--   0 benjaminn   (502) staff       (20)    12767 2023-08-02 22:45:19.000000 decontext-0.1.5/README.md
+-rw-r--r--   0 benjaminn   (502) staff       (20)     3301 2023-08-06 08:33:24.000000 decontext-0.1.5/pyproject.toml
+-rw-r--r--   0 benjaminn   (502) staff       (20)       38 2023-08-06 08:33:49.731298 decontext-0.1.5/setup.cfg
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-06 08:33:49.723390 decontext-0.1.5/src/
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-06 08:33:49.726449 decontext-0.1.5/src/decontext/
+-rw-r--r--   0 benjaminn   (502) staff       (20)      120 2023-08-02 21:27:06.000000 decontext-0.1.5/src/decontext/__init__.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     6676 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/cache.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     6778 2023-08-06 08:33:24.000000 decontext-0.1.5/src/decontext/data_types.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      115 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/logging.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)    13550 2023-08-03 21:51:35.000000 decontext-0.1.5/src/decontext/model.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     2782 2023-08-02 22:45:19.000000 decontext-0.1.5/src/decontext/pipeline.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)        0 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/py.typed
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-06 08:33:49.728293 decontext-0.1.5/src/decontext/step/
+-rw-r--r--   0 benjaminn   (502) staff       (20)     6544 2023-08-06 08:33:24.000000 decontext-0.1.5/src/decontext/step/qa.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      767 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/step/qgen.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1033 2023-08-02 21:29:03.000000 decontext-0.1.5/src/decontext/step/step.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      788 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/step/synth.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     4115 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/template.py
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-06 08:33:49.729498 decontext-0.1.5/src/decontext/templates/
+-rw-r--r--   0 benjaminn   (502) staff       (20)        0 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/templates/__init__.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      624 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/templates/qa_fulltext.yaml
+-rw-r--r--   0 benjaminn   (502) staff       (20)      957 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/templates/qa_retrieval.yaml
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1045 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/templates/qgen.yaml
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1456 2023-08-01 22:11:18.000000 decontext-0.1.5/src/decontext/templates/synth.yaml
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1124 2023-08-02 22:45:19.000000 decontext-0.1.5/src/decontext/utils.py
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-06 08:33:49.727321 decontext-0.1.5/src/decontext.egg-info/
+-rw-r--r--   0 benjaminn   (502) staff       (20)    13886 2023-08-06 08:33:49.000000 decontext-0.1.5/src/decontext.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminn   (502) staff       (20)      834 2023-08-06 08:33:49.000000 decontext-0.1.5/src/decontext.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminn   (502) staff       (20)        1 2023-08-06 08:33:49.000000 decontext-0.1.5/src/decontext.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminn   (502) staff       (20)      509 2023-08-06 08:33:49.000000 decontext-0.1.5/src/decontext.egg-info/requires.txt
+-rw-r--r--   0 benjaminn   (502) staff       (20)       10 2023-08-06 08:33:49.000000 decontext-0.1.5/src/decontext.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-06 08:33:49.730624 decontext-0.1.5/tests/
+-rw-r--r--   0 benjaminn   (502) staff       (20)     2158 2023-08-03 21:51:35.000000 decontext-0.1.5/tests/test_cache.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1137 2023-08-06 08:33:24.000000 decontext-0.1.5/tests/test_data_types.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      653 2023-08-02 22:45:19.000000 decontext-0.1.5/tests/test_model.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     9080 2023-08-06 08:33:24.000000 decontext-0.1.5/tests/test_pipeline.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      493 2023-08-02 22:45:19.000000 decontext-0.1.5/tests/test_utils.py
```

### Comparing `decontext-0.1.4/PKG-INFO` & `decontext-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decontext
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pipeline for decontextualization of scientific snippets.
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Benjamin Newman <bnewmancommercial@gmail.com>, Luca Soldaini <luca@soldaini.net>, Kyle Lo <kylel@allenai.org>
 Maintainer-email: Benjamin Newman <bnewmancommercial@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Repository, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Bug Tracker, https://github.com/bnewm0609/qa-decontextualization/issues
```

### Comparing `decontext-0.1.4/README.md` & `decontext-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/pyproject.toml` & `decontext-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "decontext"
-version = "0.1.4"
+version = "0.1.5"
 description = """\
 Pipeline for decontextualization of scientific snippets.
 """
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `decontext-0.1.4/src/decontext/cache.py` & `decontext-0.1.5/src/decontext/cache.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/data_types.py` & `decontext-0.1.5/src/decontext/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from decontext.utils import hash_strs
 
 
 # Representing Paper Snippets
 class EvidenceParagraph(BaseModel):
     section: Optional[str]
     paragraph: str
+    index: int  # index of the paragraph in the paper (NOT the section)
     paper_id: Optional[str]
 
 
 class QuestionAnswerEvidence(BaseModel):
     """Representation of the questions, answers, and evidence."""
 
     qid: str
@@ -97,22 +98,24 @@
     @validator("paragraph_with_snippet", pre=True, always=True)
     def extract_paragraph_with_snippet(cls, v, values):
         # if there's a value for paragraph_with_snippet, return it
         if v:
             return v
 
         # extract the paragraph that the snippet is in from the paper
+        paragraph_idx = 0
         paragraph_with_snippet = None
         for section in values["context"].full_text:
             for paragraph in section.paragraphs:
                 if values["snippet"] in paragraph:
                     paragraph_with_snippet = EvidenceParagraph(
-                        section=section.section_name, paragraph=paragraph
+                        section=section.section_name, paragraph=paragraph, index=paragraph_idx
                     )
                     break
+                paragraph_idx += 1
             if paragraph_with_snippet is not None:
                 break
 
         if paragraph_with_snippet is None:
             raise ValueError(
                 "Could not find snippet in the full text! Please make sure the snippet is there."
             )
@@ -129,31 +132,33 @@
             )
         )
 
     def add_evidence_paragraphs(
         self,
         qid: str,
         additional_paragraphs: List[str],
+        paragraph_indexes: List[int],
         sections: Optional[List[str]] = None,
         paper_id: Optional[str] = None,
     ):
         if sections is None:
             sections = [""] * len(additional_paragraphs)
 
         for qae in self.qae:
             if qae.qid == qid:
                 if qae.evidence is None:
                     qae.evidence = []
-                for section, additional_paragraph in zip(
-                    sections, additional_paragraphs
+                for section, paragraph_idx, additional_paragraph in zip(
+                    sections, paragraph_indexes, additional_paragraphs
                 ):
                     qae.evidence.append(
                         EvidenceParagraph(
                             section=section,
                             paragraph=additional_paragraph,
+                            index=paragraph_idx,
                             paper_id=paper_id,
                         )
                     )
 
     def add_answer(self, qid: str, answer: str):
         for qae in self.qae:
             if qae.qid == qid:
```

### Comparing `decontext-0.1.4/src/decontext/model.py` & `decontext-0.1.5/src/decontext/model.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/pipeline.py` & `decontext-0.1.5/src/decontext/pipeline.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/step/qa.py` & `decontext-0.1.5/src/decontext/step/qa.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,31 +34,35 @@
                 tempfile.NamedTemporaryFile(mode="w+", delete=False)
             )
             paper_retrieval_output_file = stack.enter_context(
                 tempfile.NamedTemporaryFile(mode="w+", delete=False)
             )
 
             for context in contexts:
-                for section in [
-                    Section(
-                        section_name=context.title,
-                        paragraphs=[context.abstract],
-                    )
-                ] + (none_check(context.full_text, [])):
+
+                all_sections = [
+                    Section(section_name=context.title, paragraphs=[context.abstract])
+                ]
+                all_sections.extend(none_check(context.full_text, []))
+
+                # this is a global paragraph index. The index -1 will be the index of the abstract
+                paragraph_idx = -1
+                for section in all_sections:
                     for para_i, paragraph in enumerate(section.paragraphs):
                         doc_file.write(
                             json.dumps(
                                 {
-                                    "did": f"{context.id}.s{section.section_name}p{para_i}",
+                                    "did": f"{context.id}.s{section.section_name}p{para_i}___{paragraph_idx}",
                                     "text": paragraph,
                                     "section": section.section_name,
                                 }
                             )
                             + "\n"
                         )
+                        paragraph_idx += 1
 
             # 2. create the query
             for question in paper_snippet.qae:
                 # with open(query_path, "a") as f:
                 query_file.write(
                     json.dumps(
                         {"qid": question.qid, "text": question.question}
@@ -82,20 +86,23 @@
             )
 
             # Extract the docs
             with open(retrieval_output_file_name) as retrieval_output_file:
                 docs = [
                     json.loads(line.strip()) for line in retrieval_output_file
                 ]
+
             docs_by_qid = defaultdict(list)
             for doc in docs:
-                docs_by_qid[doc["qid"]].append(doc["text"])
+                paragraph_idx = int(doc["did"].split("___")[-1])
+                docs_by_qid[doc["qid"]].append((doc["text"], paragraph_idx))
             for qid in docs_by_qid:
+                docs, paragraph_idxs = zip(*docs_by_qid[qid][:3])
                 paper_snippet.add_evidence_paragraphs(
-                    qid, docs_by_qid[qid][:3]
+                    qid=qid, additional_paragraphs=docs, paragraph_indexes=paragraph_idxs
                 )
 
         finally:
             os.remove(doc_file_name)
             os.remove(query_file_name)
             os.remove(retrieval_output_file_name)
```

### Comparing `decontext-0.1.4/src/decontext/step/qgen.py` & `decontext-0.1.5/src/decontext/step/qgen.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/step/step.py` & `decontext-0.1.5/src/decontext/step/step.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/step/synth.py` & `decontext-0.1.5/src/decontext/step/synth.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/template.py` & `decontext-0.1.5/src/decontext/template.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/templates/qa_fulltext.yaml` & `decontext-0.1.5/src/decontext/templates/qa_fulltext.yaml`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/templates/qa_retrieval.yaml` & `decontext-0.1.5/src/decontext/templates/qa_retrieval.yaml`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/templates/qgen.yaml` & `decontext-0.1.5/src/decontext/templates/qgen.yaml`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/templates/synth.yaml` & `decontext-0.1.5/src/decontext/templates/synth.yaml`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext/utils.py` & `decontext-0.1.5/src/decontext/utils.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/src/decontext.egg-info/PKG-INFO` & `decontext-0.1.5/src/decontext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decontext
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pipeline for decontextualization of scientific snippets.
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Benjamin Newman <bnewmancommercial@gmail.com>, Luca Soldaini <luca@soldaini.net>, Kyle Lo <kylel@allenai.org>
 Maintainer-email: Benjamin Newman <bnewmancommercial@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Repository, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Bug Tracker, https://github.com/bnewm0609/qa-decontextualization/issues
```

### Comparing `decontext-0.1.4/src/decontext.egg-info/SOURCES.txt` & `decontext-0.1.5/src/decontext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/tests/test_cache.py` & `decontext-0.1.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/tests/test_data_types.py` & `decontext-0.1.5/tests/test_data_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,18 @@
         abstract=snippet["abstract"],
         paragraph_with_snippet={
             "section": snippet["context_section_header"],
             "paragraph": snippet["context_paragraph"],
         },
         additional_paragraphs=[
             EvidenceParagraph(
-                section=evidence["section"], paragraph=evidence["paragraph"]
+                section=evidence["section"], paragraph=evidence["paragraph"], index=(ev_i + evs_i * len(snippet["evidence"])),
             )
-            for evidences in snippet["evidence"].values()
-            for evidence in evidences
+            for evs_i, evidences in enumerate(snippet["evidence"].values())
+            for ev_i, evidence in enumerate(evidences)
         ],
     )
 
     context_2 = PaperContext(
         title=snippet["title"],
         abstract=snippet["abstract"],
     )
```

### Comparing `decontext-0.1.4/tests/test_model.py` & `decontext-0.1.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.4/tests/test_pipeline.py` & `decontext-0.1.5/tests/test_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             ]
         )
 
         decontextualized_snippet = decontext(self.snippet, context, pipeline=pipeline)
         print(decontextualized_snippet)
 
 
-    def test_decontext_template_retrieval(self):
+    def test_decontext_template_retrieval_one_context(self):
         if self.using_github_actions:
             self.skipTest(
                 "Skipping test_decontext_template_retrieval because it requires an openai key."
             )
 
         with open("tests/fixtures/full_text.json") as f:
             full_text_json_str = f.read()
```

