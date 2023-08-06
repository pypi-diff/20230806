# Comparing `tmp/sparsembed-0.0.1.tar.gz` & `tmp/sparsembed-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparsembed-0.0.1.tar", last modified: Sat Aug  5 00:16:50 2023, max compression
+gzip compressed data, was "sparsembed-0.0.2.tar", last modified: Sun Aug  6 21:04:03 2023, max compression
```

## Comparing `sparsembed-0.0.1.tar` & `sparsembed-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-05 00:16:50.716088 sparsembed-0.0.1/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1071 2023-08-04 22:25:59.000000 sparsembed-0.0.1/LICENSE
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     7008 2023-08-05 00:16:50.716168 sparsembed-0.0.1/PKG-INFO
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     6387 2023-08-05 00:03:32.000000 sparsembed-0.0.1/README.md
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       79 2023-08-05 00:16:50.716370 sparsembed-0.0.1/setup.cfg
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1118 2023-08-05 00:13:45.000000 sparsembed-0.0.1/setup.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-05 00:16:50.712499 sparsembed-0.0.1/sparsembed/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       59 2023-08-04 23:19:14.000000 sparsembed-0.0.1/sparsembed/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       63 2023-07-30 16:35:44.000000 sparsembed-0.0.1/sparsembed/__version__.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-05 00:16:50.713881 sparsembed-0.0.1/sparsembed/losses/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       83 2023-07-30 21:12:15.000000 sparsembed-0.0.1/sparsembed/losses/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2757 2023-08-04 22:59:07.000000 sparsembed-0.0.1/sparsembed/losses/cosine.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1828 2023-08-05 00:12:23.000000 sparsembed-0.0.1/sparsembed/losses/flops.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-05 00:16:50.714345 sparsembed-0.0.1/sparsembed/model/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       61 2023-08-04 22:31:40.000000 sparsembed-0.0.1/sparsembed/model/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     7671 2023-08-05 00:12:37.000000 sparsembed-0.0.1/sparsembed/model/sparsembed.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-05 00:16:50.714821 sparsembed-0.0.1/sparsembed/retrieve/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       33 2023-08-01 21:41:58.000000 sparsembed-0.0.1/sparsembed/retrieve/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)    12150 2023-08-04 23:23:32.000000 sparsembed-0.0.1/sparsembed/retrieve/retriever.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-05 00:16:50.715833 sparsembed-0.0.1/sparsembed/utils/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      123 2023-08-04 23:23:36.000000 sparsembed-0.0.1/sparsembed/utils/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      145 2023-08-05 00:11:56.000000 sparsembed-0.0.1/sparsembed/utils/evaluate.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2105 2023-08-04 23:47:55.000000 sparsembed-0.0.1/sparsembed/utils/iter.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4317 2023-08-04 22:37:00.000000 sparsembed-0.0.1/sparsembed/utils/scores.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-05 00:16:50.713225 sparsembed-0.0.1/sparsembed.egg-info/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     7008 2023-08-05 00:16:50.000000 sparsembed-0.0.1/sparsembed.egg-info/PKG-INFO
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      574 2023-08-05 00:16:50.000000 sparsembed-0.0.1/sparsembed.egg-info/SOURCES.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)        1 2023-08-05 00:16:50.000000 sparsembed-0.0.1/sparsembed.egg-info/dependency_links.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       44 2023-08-05 00:16:50.000000 sparsembed-0.0.1/sparsembed.egg-info/requires.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       11 2023-08-05 00:16:50.000000 sparsembed-0.0.1/sparsembed.egg-info/top_level.txt
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.277861 sparsembed-0.0.2/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1071 2023-08-04 22:25:59.000000 sparsembed-0.0.2/LICENSE
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     5462 2023-08-06 21:04:03.277938 sparsembed-0.0.2/PKG-INFO
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4842 2023-08-06 20:58:58.000000 sparsembed-0.0.2/README.md
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       79 2023-08-06 21:04:03.278143 sparsembed-0.0.2/setup.cfg
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1118 2023-08-06 20:57:40.000000 sparsembed-0.0.2/setup.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.273590 sparsembed-0.0.2/sparsembed/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       59 2023-08-04 23:19:14.000000 sparsembed-0.0.2/sparsembed/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       63 2023-08-06 20:52:35.000000 sparsembed-0.0.2/sparsembed/__version__.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.275091 sparsembed-0.0.2/sparsembed/losses/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       83 2023-07-30 21:12:15.000000 sparsembed-0.0.2/sparsembed/losses/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     2757 2023-08-04 22:59:07.000000 sparsembed-0.0.2/sparsembed/losses/cosine.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1828 2023-08-05 00:12:23.000000 sparsembed-0.0.2/sparsembed/losses/flops.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.275740 sparsembed-0.0.2/sparsembed/model/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       61 2023-08-04 22:31:40.000000 sparsembed-0.0.2/sparsembed/model/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     7443 2023-08-06 20:46:28.000000 sparsembed-0.0.2/sparsembed/model/sparsembed.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.276330 sparsembed-0.0.2/sparsembed/retrieve/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       58 2023-08-06 20:43:44.000000 sparsembed-0.0.2/sparsembed/retrieve/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)    11031 2023-08-06 20:57:27.000000 sparsembed-0.0.2/sparsembed/retrieve/retriever.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.277604 sparsembed-0.0.2/sparsembed/utils/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      123 2023-08-04 23:23:36.000000 sparsembed-0.0.2/sparsembed/utils/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      145 2023-08-05 00:11:56.000000 sparsembed-0.0.2/sparsembed/utils/evaluate.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     2105 2023-08-06 20:51:55.000000 sparsembed-0.0.2/sparsembed/utils/iter.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4317 2023-08-06 18:48:59.000000 sparsembed-0.0.2/sparsembed/utils/scores.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.274350 sparsembed-0.0.2/sparsembed.egg-info/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     5462 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/PKG-INFO
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      574 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)        1 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       44 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/requires.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       11 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/top_level.txt
```

### Comparing `sparsembed-0.0.1/LICENSE` & `sparsembed-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.1/README.md` & `sparsembed-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-# SparseEmbed 
+<div align="center">
+  <h1>SparsEmbed</h1>
+  <p>Neural search</p>
+</div>
 
-**Note:** This project is currently a work in progress. 🔨🧹
+This repository presents an unofficial replication of the research paper *[SparseEmbed: Learning Sparse Lexical Representations with Contextual Embeddings for Retrieval](https://research.google/pubs/pub52289/)* authored by Weize Kong, Jeffrey M. Dudek, Cheng Li, Mingyang Zhang, and Mike Bendersky, SIGIR 2023.
 
-This repository presents an unofficial replication of the research paper titled "[SparseEmbed: Learning Sparse Lexical Representations with Contextual Embeddings for Retrieval](https://research.google/pubs/pub52289/)" authored by Weize Kong, Jeffrey M. Dudek, Cheng Li, Mingyang Zhang, and Mike Bendersky. The original paper was published at SIGIR 2023.
+**Note:** This project is currently a work in progress. 🔨🧹
 
 ## Overview
 
-This repository aims to replicate the findings of the SparseEmbed paper, focusing on learning both sparse lexical representations and contextual token level embeddings for retrieval tasks. We propose to fine-tune the model and then to retrieve documents from a set of queries.
+This repository aims to replicate the SparseEmbed model, focusing on learning both sparse lexical representations and contextual token level embeddings for retrieval tasks. 
 
-The `SparsEmbed` model is compatible with any MLM based model using the class `AutoModelForMaskedLM` from HuggingFace.
+The `SparsEmbed` model available here is compatible with any model compatible with the class `AutoModelForMaskedLM` from HuggingFace.
 
-## Differences from the Original Paper
-
-During the replication process, we have encountered a few deviations from the original paper's methodology:
+### Differences with the original paper
 
 1. **Loss Function:** We did not yet implement the distillation loss used in the paper. We have initially opted for a cosine loss like the one used in SentenceTransformer library. This decision was made to fine-tune the model from scratch, avoiding the use of a cross-encoder as a teacher. The distillation loss should be available soon.
 
 2. **Multi-Head Implementation:** At this stage, the distinct MLM (Masked Language Model) head for document encoding and query encoding has not been incorporated. Our current implementation employs a shared MLM head (calculating sparse activations) for both documents and queries.
 
 ## Installation
 
 ```
-pip install
+pip install sparsembed
 ```
 
 ## Training
 
-The following PyTorch code snippet illustrates the training loop designed to fine-tune the model:
+The following PyTorch code snippet illustrates the training loop to fine-tune the model:
 
 ```python
 from sparsembed import model, utils, losses
 from transformers import AutoModelForMaskedLM, AutoTokenizer
 import torch
 
-device = "cuda"  # cpu / cuda / mps
+device = "cuda"  # cpu / cuda
 batch_size = 32
 
 model = model.SparsEmbed(
-    model=AutoModelForMaskedLM.from_pretrained("distilbert-base-uncased").to(device),
-    tokenizer=AutoTokenizer.from_pretrained("distilbert-base-uncased"),
+    model=AutoModelForMaskedLM.from_pretrained("Luyu/co-condenser-marco").to(device),
+    tokenizer=AutoTokenizer.from_pretrained("Luyu/co-condenser-marco"),
     device=device,
 )
 
 model = model.to(device)
 
 optimizer = torch.optim.AdamW(
     filter(lambda p: p.requires_grad, model.parameters()),
@@ -60,15 +61,15 @@
     ("Banana", "Apple is a popular fruit.", 0),
     ("Banana", "Banana is a yellow fruit.", 1),
 ]
 
 for queries, documents, labels in utils.iter(
     dataset,
     device=device,
-    epochs=20,
+    epochs=1,
     batch_size=batch_size,
     shuffle=True,
 ):
     queries_embeddings = model(queries, k=96)
 
     documents_embeddings = model(documents, k=256)
 
@@ -98,23 +99,22 @@
     )
 
     loss.backward()
     optimizer.step()
     optimizer.zero_grad()
 ```
 
-This code segment encapsulates the iterative process of fine-tuning the model's parameters using a combination of cosine and Flops loss functions. Queries and documents are both a list of strings. Labels is a Torch tensor containing binary values of 0 or 1. A label of 0 indicates that the query is not relevant to the document, while a label of 1 signifies that the query is indeed relevant to the document. 
-
 ## Inference
 
-Upon successfully training our model, the next step involves initializing a retriever to facilitate the retrieval of the most accurate documents based on a given set of queries. The retrieval process is conducted through two main steps: adding documents and querying.
+Once we trained the model, we can initialize a `Retriever` to retrieve relevant documents given a query.
 
-1. **Adding Documents**: By invoking the `add` method, the retriever undertakes document encoding. It performs this task by generating a sparse matrix that encapsulates the contributions of sparsely activated tokens. This matrix is constructed using the weighted values of these tokens.
-
-2. **Querying**: When the `__call__` method is invoked, the retriever proceeds to encode the query. Similar to the document encoding phase, the retriever constructs a sparse matrix that represents the query. This matrix is then used in a dot product operation against the sparse matrices of the stored documents. After this initial retrieval, a re-ranking process takes place. This re-ranking is based on the contextual representations of activated tokens derived from both the queries and the documents. This is in accordance with the established SparseEmbed scoring formula.
+- It build a sparse matrix from sparse activations of documents.
+- It build a sparse matrix from sparse activations of queries.
+- It match relevant documents using dot product of both sparse matrix.
+- It re-rank documents based on contextual embbedings similarity score.
 
 ```python
 from sparsembed import retrieve
 
 documents = [{
     "id": 0,
     "document": "Apple is a popular fruit.",
@@ -159,11 +159,7 @@
   {'id': 2, 'similarity': 194.5692901611328},
   {'id': 0, 'similarity': 192.5744171142578}]]
 ```
 
 ## Evaluations
 
 Work in progress.
-
-## Acknowledgments
-
-I would like to express my gratitude to the authors of the SparseEmbed paper for their valuable contributions, which serve as the foundation for this replication attempt.
```

### Comparing `sparsembed-0.0.1/setup.py` & `sparsembed-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.1/sparsembed/losses/cosine.py` & `sparsembed-0.0.2/sparsembed/losses/cosine.py`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.1/sparsembed/losses/flops.py` & `sparsembed-0.0.2/sparsembed/losses/flops.py`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.1/sparsembed/model/sparsembed.py` & `sparsembed-0.0.2/sparsembed/model/sparsembed.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 
     >>> print(documents_expanded)
     ['is great music was good wonderful big beautiful huge has are and of fine on '
      'a',
      'is great sports good was big has are and wonderful sport huge nice of games '
      'a']
 
+    >>> queries_embeddings["activations"].shape
+    torch.Size([2, 96])
+
     References
     ----------
     1. [SparseEmbed: Learning Sparse Lexical Representations with Contextual Embeddings for Retrieval](https://dl.acm.org/doi/pdf/10.1145/3539618.3592065)
 
     """
 
     def __init__(
@@ -170,17 +173,15 @@
             attention,
             embeddings,
         )
 
         return {
             "embeddings": self.relu(self.linear(embeddings)),
             "sparse_activations": activations["sparse_activations"],
-            "activations": self._filter_activations(
-                activations["sparse_activations"], k=k
-            ),
+            "activations": activations["activations"],
         }
 
     def _encode(self, texts: list[str], **kwargs) -> tuple[torch.Tensor, torch.Tensor]:
         """Encode sentences."""
         encoded_input = self.tokenizer.batch_encode_plus(
             texts, return_tensors="pt", **kwargs
         )
@@ -223,22 +224,13 @@
         return self.softmax(attention.transpose(1, 2))
 
     def _filter_activations(
         self, sparse_activations: torch.Tensor, k: int
     ) -> list[torch.Tensor]:
         """Among the set of activations, select the ones with a score > 0."""
         scores, activations = torch.topk(input=sparse_activations, k=k, dim=-1)
-
-        filter_activations = []
-
-        for score, activation in zip(scores, activations):
-            new_activation = torch.index_select(
+        return [
+            torch.index_select(
                 activation, dim=-1, index=torch.nonzero(score, as_tuple=True)[0]
             )
-
-            if new_activation.shape[0] == 0:
-                filter_activations.append(activation)
-
-            else:
-                filter_activations.append(new_activation)
-
-        return filter_activations
+            for score, activation in zip(scores, activations)
+        ]
```

### Comparing `sparsembed-0.0.1/sparsembed/retrieve/retriever.py` & `sparsembed-0.0.2/sparsembed/retrieve/retriever.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import os
 
-import numpy as np
 import torch
 import tqdm
-from scipy import sparse
 
 from ..model import SparsEmbed
 
 __all__ = ["Retriever"]
 
 
 class Retriever:
-    """Class dedicated to SparsEmbed model inference in order retrieve
-    documents with queries.
+    """Retriever class.
 
     Parameters
     ----------
     key
         Document unique identifier.
     on
         Document texts.
@@ -28,15 +25,15 @@
     >>> from transformers import AutoModelForMaskedLM, AutoTokenizer
     >>> from sparsembed import model, retrieve
     >>> from pprint import pprint as print
     >>> import torch
 
     >>> _ = torch.manual_seed(42)
 
-    >>> device = "mps"
+    >>> device = "cpu"
 
     >>> model = model.SparsEmbed(
     ...     model=AutoModelForMaskedLM.from_pretrained("distilbert-base-uncased").to(device),
     ...     tokenizer=AutoTokenizer.from_pretrained("distilbert-base-uncased"),
     ...     device=device,
     ...     embedding_size=3,
     ... )
@@ -59,31 +56,35 @@
     ... ]
     >>> retriever = retriever.add(
     ...     documents=documents,
     ...     k_token=256,
     ...     batch_size=24
     ... )
 
-    >>> print(retriever(["Food", "Sports", "Cinema", "Music"], k_token=96))
-    [[{'id': 0, 'similarity': 1.4686672687530518},
-      {'id': 1, 'similarity': 1.3459084033966064},
-      {'id': 3, 'similarity': 1.3040170669555664},
-      {'id': 2, 'similarity': 1.157921314239502}],
-     [{'id': 1, 'similarity': 7.03730583190918},
-      {'id': 3, 'similarity': 3.5283799171447754},
-      {'id': 2, 'similarity': 2.453505516052246},
-      {'id': 0, 'similarity': 1.789308786392212}],
-     [{'id': 2, 'similarity': 2.316730260848999},
-      {'id': 3, 'similarity': 2.2312138080596924},
-      {'id': 1, 'similarity': 2.0195863246917725},
-      {'id': 0, 'similarity': 1.289013147354126}],
-     [{'id': 3, 'similarity': 5.773364067077637},
-      {'id': 1, 'similarity': 3.6177942752838135},
-      {'id': 2, 'similarity': 3.3001816272735596},
-      {'id': 0, 'similarity': 2.591763496398926}]]
+    >>> print(retriever(["Food", "Sports", "Cinema", "Music", "Hello World"], k_token=96))
+    [[{'id': 0, 'similarity': 1.4686675071716309},
+      {'id': 1, 'similarity': 1.345913052558899},
+      {'id': 3, 'similarity': 1.304019808769226},
+      {'id': 2, 'similarity': 1.1579231023788452}],
+     [{'id': 1, 'similarity': 7.0373148918151855},
+      {'id': 3, 'similarity': 3.528376817703247},
+      {'id': 2, 'similarity': 2.4535036087036133},
+      {'id': 0, 'similarity': 1.7893059253692627}],
+     [{'id': 2, 'similarity': 2.3167333602905273},
+      {'id': 3, 'similarity': 2.2312183380126953},
+      {'id': 1, 'similarity': 2.0195937156677246},
+      {'id': 0, 'similarity': 1.2890148162841797}],
+     [{'id': 3, 'similarity': 2.4722704887390137},
+      {'id': 2, 'similarity': 1.8648046255111694},
+      {'id': 1, 'similarity': 1.732576608657837},
+      {'id': 0, 'similarity': 1.3416467905044556}],
+     [{'id': 3, 'similarity': 3.7778899669647217},
+      {'id': 2, 'similarity': 3.198120355606079},
+      {'id': 1, 'similarity': 3.1253902912139893},
+      {'id': 0, 'similarity': 2.458303451538086}]]
 
     """
 
     def __init__(
         self,
         key: str,
         on: list[str],
@@ -135,32 +136,32 @@
             batch_size=batch_size,
         )
 
         self.documents_embeddings.extend(documents_embeddings)
         self.documents_activations.extend(documents_activations)
 
         self.sparse_matrix = (
-            sparse_matrix
+            sparse_matrix.T
             if self.sparse_matrix is None
-            else sparse.vstack((self.sparse_matrix, sparse_matrix))
+            else torch.cat([self.sparse_matrix.to_sparse(), sparse_matrix.T], dim=1)
         )
 
         self.documents_keys = {
             **self.documents_keys,
             **{
                 len(self.documents_keys) + index: document[self.key]
                 for index, document in enumerate(documents)
             },
         }
 
         return self
 
     def __call__(
         self,
-        q: list[str] | str,
+        q: list[str],
         k_sparse: int = 100,
         k_token: int = 96,
         batch_size: int = 3,
     ) -> list:
         """Retrieve documents.
 
         Parameters
@@ -178,146 +179,111 @@
             sparse_matrix,
         ) = self._build_index(
             X=[q] if isinstance(q, str) else q,
             k_token=k_token,
             batch_size=batch_size,
         )
 
-        # TODO: return torch tensor
-        matchs, _ = self.top_k_by_partition(
-            similarities=(sparse_matrix @ self.sparse_matrix.T).toarray(),
-            k_sparse=k_sparse,
+        sparse_scores = (sparse_matrix @ self.sparse_matrix).to_dense()
+
+        _, sparse_matchs = torch.topk(
+            input=sparse_scores, k=min(k_sparse, len(self.documents_keys)), dim=-1
         )
 
+        sparse_matchs_idx = sparse_matchs.tolist()
+
         # Intersections between queries and documents activated tokens.
         intersections = self._get_intersection(
             queries_activations=queries_activations,
             documents_activations=[
                 [self.documents_activations[document] for document in query_matchs]
-                for query_matchs in matchs
+                for query_matchs in sparse_matchs_idx
             ],
         )
 
-        # Optimize to handle batchs
-        scores = self._get_scores(
+        dense_scores = self._get_scores(
             queries_embeddings=queries_embeddings,
             documents_embeddings=[
                 [self.documents_embeddings[document] for document in match]
-                for match in matchs
+                for match in sparse_matchs_idx
             ],
             intersections=intersections,
         )
 
-        return self._rank(scores=scores, matchs=matchs)
+        return self._rank(
+            dense_scores=dense_scores, sparse_matchs=sparse_matchs, k_sparse=k_sparse
+        )
 
-    def _rank(self, scores: torch.Tensor, matchs: torch.Tensor) -> list:
+    def _rank(
+        self, dense_scores: torch.Tensor, sparse_matchs: torch.Tensor, k_sparse: int
+    ) -> list:
         """Rank documents by scores.
 
         Parameters
         ----------
         scores
             Scores between queries and documents.
         matchs
             Documents matchs.
         """
-        ranks = torch.argsort(scores, dim=-1, descending=True, stable=False)
-
-        scores = [
-            torch.index_select(input=query_documents_score, dim=0, index=query_ranks)
-            for query_documents_score, query_ranks in zip(scores, ranks)
-        ]
+        dense_scores, dense_matchs = torch.topk(
+            input=dense_scores, k=min(k_sparse, len(self.documents_keys)), dim=-1
+        )
 
-        matchs = [
-            torch.index_select(
-                input=torch.tensor(query_matchs).to(self.model.device),
-                dim=0,
-                index=query_ranks,
-            )
-            for query_matchs, query_ranks in zip(matchs, ranks)
-        ]
+        dense_scores = dense_scores.tolist()
+        dense_matchs = (
+            torch.gather(sparse_matchs, 1, dense_matchs).detach().cpu().tolist()
+        )
 
         return [
             [
                 {
-                    self.key: self.documents_keys[document.item()],
-                    "similarity": score.item(),
+                    self.key: self.documents_keys[document],
+                    "similarity": score,
                 }
                 for score, document in zip(query_scores, query_matchs)
             ]
-            for query_scores, query_matchs in zip(scores, matchs)
+            for query_scores, query_matchs in zip(dense_scores, dense_matchs)
         ]
 
     def _build_index(
         self,
         X: list[str],
         batch_size: int,
         k_token: int,
-    ) -> tuple[list, list, sparse.csr_matrix]:
-        """Build"""
-        index_embeddings, index_activations, rows, columns, values = [], [], [], [], []
-        n = 0
+    ) -> tuple[list, list, torch.Tensor]:
+        """Build a sparse matrix index."""
+        index_embeddings, index_activations, sparse_activations = [], [], []
 
         for batch in self._to_batch(X, batch_size=batch_size):
             batch_embeddings = self.model.encode(batch, k=k_token)
 
-            for activations, embeddings, sparse_activations in zip(
+            sparse_activations.append(
+                batch_embeddings["sparse_activations"].to_sparse()
+            )
+
+            for activations, activations_idx, embeddings in zip(
                 batch_embeddings["activations"],
+                batch_embeddings["activations"].detach().cpu().tolist(),
                 batch_embeddings["embeddings"],
-                batch_embeddings["sparse_activations"],
             ):
                 index_activations.append(activations)
                 index_embeddings.append(
                     {
-                        token.item(): embedding
-                        for token, embedding in zip(activations, embeddings)
+                        token: embedding
+                        for token, embedding in zip(activations_idx, embeddings)
                     }
                 )
 
-                tokens_scores = torch.index_select(
-                    sparse_activations, dim=-1, index=activations
-                )
-
-                rows.extend([n for _ in range(len(activations))])
-                columns.extend(activations.tolist())
-                values.extend(tokens_scores.tolist())
-                n += 1
-
-        sparse_matrix = sparse.csc_matrix(
-            (values, (rows, columns)), shape=(len(X), self.vocabulary_size)
+        return (
+            index_embeddings,
+            index_activations,
+            torch.cat(sparse_activations),
         )
 
-        return index_embeddings, index_activations, sparse_matrix
-
-    def top_k_by_partition(
-        self, similarities: np.ndarray, k_sparse: int
-    ) -> tuple[np.ndarray, np.ndarray]:
-        """Top k elements by partition."""
-        similarities *= -1
-
-        if k_sparse < len(self.documents_keys):
-            ind = np.argpartition(similarities, k_sparse, axis=-1)
-
-            # k non-sorted indices
-            ind = np.take(ind, np.arange(k_sparse), axis=-1)
-
-            # k non-sorted values
-            similarities = np.take_along_axis(similarities, ind, axis=-1)
-
-            # sort within k elements
-            ind_part = np.argsort(similarities, axis=-1)
-            ind = np.take_along_axis(ind, ind_part, axis=-1)
-
-        else:
-            ind_part = np.argsort(similarities, axis=-1)
-            ind = ind_part
-
-        similarities *= -1
-        val = np.take_along_axis(similarities, ind_part, axis=-1)
-        return ind, val
-
     @staticmethod
     def _to_batch(X: list, batch_size: int) -> list:
         """Convert input list to batch."""
         for X in tqdm.tqdm(
             [X[pos : pos + batch_size] for pos in range(0, len(X), batch_size)],
             position=0,
             total=1 + len(X) // batch_size,
```

### Comparing `sparsembed-0.0.1/sparsembed/utils/iter.py` & `sparsembed-0.0.2/sparsembed/utils/iter.py`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.1/sparsembed/utils/scores.py` & `sparsembed-0.0.2/sparsembed/utils/scores.py`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.1/sparsembed.egg-info/SOURCES.txt` & `sparsembed-0.0.2/sparsembed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

