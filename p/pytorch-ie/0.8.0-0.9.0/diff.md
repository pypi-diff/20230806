# Comparing `tmp/pytorch-ie-0.8.0.tar.gz` & `tmp/pytorch-ie-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-ie-0.8.0.tar", max compression
+gzip compressed data, was "pytorch-ie-0.9.0.tar", max compression
```

## Comparing `pytorch-ie-0.8.0.tar` & `pytorch-ie-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1080 2022-07-28 14:34:27.651863 pytorch-ie-0.8.0/LICENSE
--rw-r--r--   0        0        0     9557 2022-07-28 14:34:27.651863 pytorch-ie-0.8.0/README.md
--rw-r--r--   0        0        0     2842 2022-07-28 14:34:40.263696 pytorch-ie-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      224 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/__init__.py
--rw-r--r--   0        0        0     4973 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/annotations.py
--rw-r--r--   0        0        0     3952 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/auto.py
--rw-r--r--   0        0        0      160 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/core/__init__.py
--rw-r--r--   0        0        0     8491 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/core/document.py
--rw-r--r--   0        0        0    17440 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/core/hf_hub_mixin.py
--rw-r--r--   0        0        0      735 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/core/model.py
--rw-r--r--   0        0        0     1718 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/core/registrable.py
--rw-r--r--   0        0        0    10240 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/core/taskmodule.py
--rw-r--r--   0        0        0      332 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/__init__.py
--rw-r--r--   0        0        0     1954 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/builder.py
--rw-r--r--   0        0        0        0 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datamodules/__init__.py
--rw-r--r--   0        0        0     4569 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datamodules/datamodule.py
--rw-r--r--   0        0        0     3843 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/dataset.py
--rw-r--r--   0        0        0      852 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/dataset_formatter.py
--rw-r--r--   0        0        0       81 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/__init__.py
--rw-r--r--   0        0        0    11629 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/brat.py
--rw-r--r--   0        0        0        0 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/__init__.py
--rw-r--r--   0        0        0     6956 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/ace2004.py
--rw-r--r--   0        0        0     6009 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/ace2005.py
--rw-r--r--   0        0        0    12258 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/brat.py
--rw-r--r--   0        0        0     7415 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/chemprot.py
--rw-r--r--   0        0        0    10437 2022-07-28 14:34:27.663863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/fewrel.py
--rw-r--r--   0        0        0    17488 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/genia.py
--rw-r--r--   0        0        0     5113 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/ontonotes.py
--rw-r--r--   0        0        0     5720 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/scierc.py
--rw-r--r--   0        0        0     6715 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/semeval_2010_task_8.py
--rw-r--r--   0        0        0    10010 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/tacred.py
--rw-r--r--   0        0        0    21825 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/webred.py
--rw-r--r--   0        0        0     6619 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/wiki80.py
--rw-r--r--   0        0        0     3563 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/wikigold.py
--rw-r--r--   0        0        0      351 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/documents.py
--rw-r--r--   0        0        0     1828 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/models/__init__.py
--rw-r--r--   0        0        0        0 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/models/genre/__init__.py
--rw-r--r--   0        0        0        0 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/models/modules/__init__.py
--rw-r--r--   0        0        0      612 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/models/modules/mlp.py
--rw-r--r--   0        0        0     2438 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/models/transformer_seq2seq.py
--rw-r--r--   0        0        0     8726 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/models/transformer_span_classification.py
--rw-r--r--   0        0        0     4797 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/models/transformer_text_classification.py
--rw-r--r--   0        0        0     3237 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/models/transformer_token_classification.py
--rw-r--r--   0        0        0    14070 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/pipeline.py
--rw-r--r--   0        0        0      409 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/__init__.py
--rw-r--r--   0        0        0    20526 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_re_text_classification.py
--rw-r--r--   0        0        0     9585 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_seq2seq.py
--rw-r--r--   0        0        0    11454 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_span_classification.py
--rw-r--r--   0        0        0     8797 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_text_classification.py
--rw-r--r--   0        0        0    14821 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_token_classification.py
--rw-r--r--   0        0        0        0 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/utils/__init__.py
--rw-r--r--   0        0        0    11517 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/utils/span.py
--rw-r--r--   0        0        0     3272 2022-07-28 14:34:27.667863 pytorch-ie-0.8.0/src/pytorch_ie/utils/window.py
--rw-r--r--   0        0        0    10915 2022-07-28 14:34:42.293513 pytorch-ie-0.8.0/setup.py
--rw-r--r--   0        0        0    10772 2022-07-28 14:34:42.294483 pytorch-ie-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-08-09 13:26:32.703425 pytorch-ie-0.9.0/LICENSE
+-rw-r--r--   0        0        0    13800 2022-08-09 13:26:32.703425 pytorch-ie-0.9.0/README.md
+-rw-r--r--   0        0        0     2842 2022-08-09 13:26:44.771419 pytorch-ie-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/__init__.py
+-rw-r--r--   0        0        0     4973 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/annotations.py
+-rw-r--r--   0        0        0     3952 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/auto.py
+-rw-r--r--   0        0        0      160 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/core/__init__.py
+-rw-r--r--   0        0        0     8740 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/core/document.py
+-rw-r--r--   0        0        0    17440 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/core/hf_hub_mixin.py
+-rw-r--r--   0        0        0      735 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/core/model.py
+-rw-r--r--   0        0        0     1718 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/core/registrable.py
+-rw-r--r--   0        0        0    10240 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/core/taskmodule.py
+-rw-r--r--   0        0        0      332 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/__init__.py
+-rw-r--r--   0        0        0     1954 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/builder.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datamodules/__init__.py
+-rw-r--r--   0        0        0     4569 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datamodules/datamodule.py
+-rw-r--r--   0        0        0     7306 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/dataset.py
+-rw-r--r--   0        0        0      852 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/dataset_formatter.py
+-rw-r--r--   0        0        0       81 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/__init__.py
+-rw-r--r--   0        0        0    11629 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/brat.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/__init__.py
+-rw-r--r--   0        0        0     6956 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/ace2004.py
+-rw-r--r--   0        0        0     6009 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/ace2005.py
+-rw-r--r--   0        0        0    12258 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/brat.py
+-rw-r--r--   0        0        0     7415 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/chemprot.py
+-rw-r--r--   0        0        0    10437 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/fewrel.py
+-rw-r--r--   0        0        0    17488 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/genia.py
+-rw-r--r--   0        0        0     5113 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/ontonotes.py
+-rw-r--r--   0        0        0     5720 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/scierc.py
+-rw-r--r--   0        0        0     6715 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/semeval_2010_task_8.py
+-rw-r--r--   0        0        0    10010 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/tacred.py
+-rw-r--r--   0        0        0    21825 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/webred.py
+-rw-r--r--   0        0        0     6619 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/wiki80.py
+-rw-r--r--   0        0        0     3563 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/wikigold.py
+-rw-r--r--   0        0        0      351 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/documents.py
+-rw-r--r--   0        0        0     1828 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/models/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/models/genre/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/models/modules/__init__.py
+-rw-r--r--   0        0        0      612 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/models/modules/mlp.py
+-rw-r--r--   0        0        0     2438 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/models/transformer_seq2seq.py
+-rw-r--r--   0        0        0     8726 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/models/transformer_span_classification.py
+-rw-r--r--   0        0        0     4797 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/models/transformer_text_classification.py
+-rw-r--r--   0        0        0     3237 2022-08-09 13:26:32.719424 pytorch-ie-0.9.0/src/pytorch_ie/models/transformer_token_classification.py
+-rw-r--r--   0        0        0    14070 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/pipeline.py
+-rw-r--r--   0        0        0      409 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/__init__.py
+-rw-r--r--   0        0        0    20526 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_re_text_classification.py
+-rw-r--r--   0        0        0     9585 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_seq2seq.py
+-rw-r--r--   0        0        0    11454 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_span_classification.py
+-rw-r--r--   0        0        0     8797 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_text_classification.py
+-rw-r--r--   0        0        0    14821 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_token_classification.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/utils/__init__.py
+-rw-r--r--   0        0        0    11517 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/utils/span.py
+-rw-r--r--   0        0        0     3272 2022-08-09 13:26:32.723424 pytorch-ie-0.9.0/src/pytorch_ie/utils/window.py
+-rw-r--r--   0        0        0    15244 2022-08-09 13:26:47.297097 pytorch-ie-0.9.0/setup.py
+-rw-r--r--   0        0        0    15015 2022-08-09 13:26:47.298274 pytorch-ie-0.9.0/PKG-INFO
```

### Comparing `pytorch-ie-0.8.0/LICENSE` & `pytorch-ie-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/pyproject.toml` & `pytorch-ie-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # requires = ["poetry-core>=1.1.0"]
 requires = ["poetry-core @ git+https://github.com/python-poetry/poetry-core.git@master"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pytorch-ie"
-version = "0.8.0"
+version = "0.9.0"
 description = "State-of-the-art Information Extraction in PyTorch"
 readme = "README.md"
 authors = ["Christoph Alt <christoph.alt@posteo.de>"]
 license = "MIT"
 homepage = "https://github.com/christophalt/pytorch-ie"
 repository = "https://github.com/christophalt/pytorch-ie"
 documentation = "https://pytorch-ie.readthedocs.io"
```

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/annotations.py` & `pytorch-ie-0.9.0/src/pytorch_ie/annotations.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/auto.py` & `pytorch-ie-0.9.0/src/pytorch_ie/auto.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/core/document.py` & `pytorch-ie-0.9.0/src/pytorch_ie/core/document.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,29 +112,32 @@
 
         return super().__eq__(other) and self.predictions == other.predictions
 
     def __repr__(self) -> str:
         return f"AnnotationList({str(self._annotations)})"
 
 
+D = TypeVar("D", bound="Document")
+
+
 @dataclasses.dataclass
 class Document(Mapping[str, Any]):
     _annotation_graph: Dict[str, List[str]] = dataclasses.field(
         default_factory=dict, init=False, repr=False
     )
     _annotation_fields: Set[str] = dataclasses.field(default_factory=set, init=False, repr=False)
     _root_annotation: Optional[str] = dataclasses.field(default=None, init=False, repr=False)
 
     def __getitem__(self, key: str) -> AnnotationList:
         if key not in self._annotation_fields:
             raise KeyError(f"Document has no attribute '{key}'.")
         return getattr(self, key)
 
     def __iter__(self):
-        return iter((field.name, getattr(self, field.name)) for field in self._annotation_fields)
+        return iter(self._annotation_fields)
 
     def __len__(self):
         return len(self._annotation_fields)
 
     def __post_init__(self):
         edges = set()
         for field in dataclasses.fields(self):
@@ -243,7 +246,12 @@
         for field_name, annotation in annotations.values():
             getattr(doc, field_name).append(annotation)
 
         for field_name, annotation in predictions.values():
             getattr(doc, field_name).predictions.append(annotation)
 
         return doc
+
+    def as_type(self, new_type: typing.Type[D], field_mapping: Optional[Dict[str, str]] = None):
+        field_mapping = field_mapping or {}
+        new_doc = new_type.fromdict({field_mapping.get(k, k): v for k, v in self.asdict().items()})
+        return new_doc
```

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/core/hf_hub_mixin.py` & `pytorch-ie-0.9.0/src/pytorch_ie/core/hf_hub_mixin.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/core/model.py` & `pytorch-ie-0.9.0/src/pytorch_ie/core/model.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/core/registrable.py` & `pytorch-ie-0.9.0/src/pytorch_ie/core/registrable.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/core/taskmodule.py` & `pytorch-ie-0.9.0/src/pytorch_ie/core/taskmodule.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/builder.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/builder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datamodules/datamodule.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datamodules/datamodule.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/dataset_formatter.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/dataset_formatter.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/brat.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/brat.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/ace2004.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/ace2004.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/ace2005.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/ace2005.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/brat.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/brat.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/chemprot.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/chemprot.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/fewrel.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/fewrel.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/genia.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/genia.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/ontonotes.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/ontonotes.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/scierc.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/scierc.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/semeval_2010_task_8.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/semeval_2010_task_8.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/tacred.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/tacred.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/webred.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/webred.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/wiki80.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/wiki80.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/data/datasets/hf_datasets/wikigold.py` & `pytorch-ie-0.9.0/src/pytorch_ie/data/datasets/hf_datasets/wikigold.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/models/__init__.py` & `pytorch-ie-0.9.0/src/pytorch_ie/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/models/modules/mlp.py` & `pytorch-ie-0.9.0/src/pytorch_ie/models/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/models/transformer_seq2seq.py` & `pytorch-ie-0.9.0/src/pytorch_ie/models/transformer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/models/transformer_span_classification.py` & `pytorch-ie-0.9.0/src/pytorch_ie/models/transformer_span_classification.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/models/transformer_text_classification.py` & `pytorch-ie-0.9.0/src/pytorch_ie/models/transformer_text_classification.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/models/transformer_token_classification.py` & `pytorch-ie-0.9.0/src/pytorch_ie/models/transformer_token_classification.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/pipeline.py` & `pytorch-ie-0.9.0/src/pytorch_ie/pipeline.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_re_text_classification.py` & `pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_re_text_classification.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_seq2seq.py` & `pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_span_classification.py` & `pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_span_classification.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_text_classification.py` & `pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_text_classification.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/taskmodules/transformer_token_classification.py` & `pytorch-ie-0.9.0/src/pytorch_ie/taskmodules/transformer_token_classification.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/utils/span.py` & `pytorch-ie-0.9.0/src/pytorch_ie/utils/span.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/src/pytorch_ie/utils/window.py` & `pytorch-ie-0.9.0/src/pytorch_ie/utils/window.py`

 * *Files identical despite different names*

### Comparing `pytorch-ie-0.8.0/setup.py` & `pytorch-ie-0.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,17 +25,17 @@
  'huggingface-hub>=0.5.1,<0.6.0',
  'pytorch-lightning>=1.6.1,<2.0.0',
  'torchmetrics>=0.8.0,<0.9.0',
  'transformers>=4.18.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pytorch-ie',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'State-of-the-art Information Extraction in PyTorch',
-    'long_description': '# PyTorch-IE: State-of-the-art Information Extraction in PyTorch\n\n[![PyPI](https://img.shields.io/pypi/v/pytorch-ie.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/pytorch-ie.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/pytorch-ie)][pypi status]\n[![License](https://img.shields.io/pypi/l/pytorch-ie)][license]\n\n[![Read the documentation at https://pytorch-ie.readthedocs.io/](https://img.shields.io/readthedocs/pytorch-ie/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/christophalt/pytorch-ie/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/christophalt/pytorch-ie/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/pytorch-ie/\n[read the docs]: https://pytorch-ie.readthedocs.io/\n[tests]: https://github.com/christophalt/pytorch-ie/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/christophalt/pytorch-ie\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## 🤯 What\'s this about?\n\nThis is an experimental framework that aims to combine the lessons learned from five years of information extraction research.\n\n-   **Focus on the core task:** The main goal is to develop information extraction methods not dataset loading and evaluation logic. We use external well-maintained libraries for non-core functionality. PyTorch-Lightning for training and logging, Huggingface datasets for dataset reading, and Huggingface evaluate for evaluation (coming soon).\n-   **Sharing is caring:** Being able to quickly and easily share models is key to promote your work and facilitate further research. All models developed in PyTorch-IE can be easily shared via the Huggingface model hub. This further allows to quickly build demos based on Huggingface spaces, gradio or streamlit.\n-   **Unified document format:** A unified document format allows for quick experimentation on any dataset or task.\n-   **Beyond sentence level:** Most information extraction frameworks assume text inputs at a sentence granularity. We do not make any assumption on the granularity but generally aim for document-level information extraction.\n-   **Beyond unstructured text:** Unstructured text is only one possible area for information extraction. We developed the framework to also support information extraction from semi-structured text (e.g. HTML), two-dimensional text (e.g. OCR\'d images), and images.\n-   **Character-level annotation and evaluation:** Many information extraction frameworks annotate and evaluate on a token level. We believe that annotation and evaluation should be done on a character level as this also considers the suitability of the tokenizer for the task.\n-   **Make no assumptions on the structure of models:** The last years have seen many different and creative approaches to information extraction and a framework that imposes a structure on those will most certainly be to limiting. With PyTorch-iE you have full control over how a document is prepared for a model and how the model is structured. The logic is self-contained and thus can be easily shared and inspected by others. The only assumption we make is that the input is a document and the output are targets (training) or annotations (inference).\n\n## 🚀️ Quickstart\n\n```console\n$ pip install pytorch-ie\n```\n\n## 🔭 Demos\n\n| Task                                                       | Link (Huggingface Spaces)                                                   |\n| ---------------------------------------------------------- | --------------------------------------------------------------------------- |\n| Named Entity Recognition (Span-based)                      | [LINK](https://huggingface.co/spaces/pie/NER)                               |\n| Joint Named Entity Recognition and Relation Classification | [LINK](https://huggingface.co/spaces/pie/Joint-NER-and-Relation-Extraction) |\n\n## 📚 Datasets\n\nWe parse all datasets into a common format that can be loaded directly from the model hub via Huggingface datasets. The documents are cached in an arrow table and serialized / deserialized on the fly. Any changes or preprocessing applied to the documents will be cached as well.\n\n```python\nimport datasets\n\ndataset = datasets.load_dataset("pie/conll2003")\n\nprint(dataset["train"][0])\n# >>> CoNLL2003Document(text=\'EU rejects German call to boycott British lamb .\', id=\'0\', metadata={})\n\ndataset["train"][0].entities\n# >>> AnnotationList([LabeledSpan(start=0, end=2, label=\'ORG\', score=1.0), LabeledSpan(start=11, end=17, label=\'MISC\', score=1.0), LabeledSpan(start=34, end=41, label=\'MISC\', score=1.0)])\n\nentity = dataset["train"][0].entities[1]\n\nprint(f"[{entity.start}, {entity.end}] {entity}")\n# >>> [11, 17] German\n```\n\n## ⚡️ Example\n\n**Note:** Setting `num_workers=0` in the pipeline is only necessary when running an example in an\ninteractive python session. The reason is that multiprocessing doesn\'t play well with the interactive python\ninterpreter, see [here](https://docs.python.org/3/library/multiprocessing.html#using-a-pool-of-workers)\nfor details.\n\n### Span-classification-based Named Entity Recognition\n\n```python\nfrom dataclasses import dataclass\n\nfrom pytorch_ie.annotations import LabeledSpan\nfrom pytorch_ie.auto import AutoPipeline\nfrom pytorch_ie.core import AnnotationList, annotation_field\nfrom pytorch_ie.documents import TextDocument\n\n@dataclass\nclass ExampleDocument(TextDocument):\n    entities: AnnotationList[LabeledSpan] = annotation_field(target="text")\n\ndocument = ExampleDocument(\n    "“Making a super tasty alt-chicken wing is only half of it,” said Po Bronson, general partner at SOSV and managing director of IndieBio."\n)\n\n# see below for the long version\nner_pipeline = AutoPipeline.from_pretrained("pie/example-ner-spanclf-conll03", device=-1, num_workers=0)\n\nner_pipeline(document, predict_field="entities")\n\nfor entity in document.entities.predictions:\n    print(f"{entity} -> {entity.label}")\n\n# Result:\n# IndieBio -> ORG\n# Po Bronson -> PER\n# SOSV -> ORG\n```\n\nTo create the same pipeline as above without `AutoPipeline`:\n\n```python\nfrom pytorch_ie.auto import AutoTaskModule, AutoModel\nfrom pytorch_ie.pipeline import Pipeline\n\nmodel_name_or_path = "pie/example-ner-spanclf-conll03"\nner_taskmodule = AutoTaskModule.from_pretrained(model_name_or_path)\nner_model = AutoModel.from_pretrained(model_name_or_path)\nner_pipeline = Pipeline(model=ner_model, taskmodule=ner_taskmodule, device=-1, num_workers=0)\n```\n\nOr, without `Auto` classes at all:\n\n```python\nfrom pytorch_ie.pipeline import Pipeline\nfrom pytorch_ie.models import TransformerSpanClassificationModel\nfrom pytorch_ie.taskmodules import TransformerSpanClassificationTaskModule\n\nmodel_name_or_path = "pie/example-ner-spanclf-conll03"\nner_taskmodule = TransformerSpanClassificationTaskModule.from_pretrained(model_name_or_path)\nner_model = TransformerSpanClassificationModel.from_pretrained(model_name_or_path)\nner_pipeline = Pipeline(model=ner_model, taskmodule=ner_taskmodule, device=-1, num_workers=0)\n```\n\n## ⚡️️️️ More Examples\n\n### Text-classification-based Relation Extraction\n\n```python\nfrom dataclasses import dataclass\n\nfrom pytorch_ie.annotations import BinaryRelation, LabeledSpan\nfrom pytorch_ie.auto import AutoPipeline\nfrom pytorch_ie.core import AnnotationList, annotation_field\nfrom pytorch_ie.documents import TextDocument\n\n\n@dataclass\nclass ExampleDocument(TextDocument):\n    entities: AnnotationList[LabeledSpan] = annotation_field(target="text")\n    relations: AnnotationList[BinaryRelation] = annotation_field(target="entities")\n\ndocument = ExampleDocument(\n    "“Making a super tasty alt-chicken wing is only half of it,” said Po Bronson, general partner at SOSV and managing director of IndieBio."\n)\n\nre_pipeline = AutoPipeline.from_pretrained("pie/example-re-textclf-tacred", device=-1, num_workers=0)\n\nfor start, end, label in [(65, 75, "PER"), (96, 100, "ORG"), (126, 134, "ORG")]:\n    document.entities.append(LabeledSpan(start=start, end=end, label=label))\n\nre_pipeline(document, predict_field="relations", batch_size=2)\n\nfor relation in document.relations.predictions:\n    print(f"({relation.head} -> {relation.tail}) -> {relation.label}")\n\n# Result:\n# (Po Bronson -> SOSV) -> per:employee_of\n# (Po Bronson -> IndieBio) -> per:employee_of\n# (SOSV -> Po Bronson) -> org:top_members/employees\n# (IndieBio -> Po Bronson) -> org:top_members/employees\n```\n\n<!-- github-only -->\n\n✨📚✨ [Read the full documentation](https://pytorch-ie.readthedocs.io/)\n\n## 🔧 Development Setup\n\n## 🏅 Acknowledgements\n\n-   This package is based on the [sourcery-ai/python-best-practices-cookiecutter](https://github.com/sourcery-ai/python-best-practices-cookiecutter) and [cjolowicz/cookiecutter-hypermodern-python](https://github.com/cjolowicz/cookiecutter-hypermodern-python) project templates.\n\n## 📃 Citation\n\nIf you find the framework useful please consider citing it:\n\n```bibtex\n@misc{alt2022pytorchie,\n    author={Christoph Alt, Arne Binder},\n    title = {PyTorch-IE: State-of-the-art Information Extraction in PyTorch},\n    year = {2022},\n    publisher = {GitHub},\n    journal = {GitHub repository},\n    howpublished = {\\url{https://github.com/ChristophAlt/pytorch-ie}}\n}\n```\n\n[license]: https://github.com/christophalt/pytorch-ie/blob/main/LICENSE\n',
+    'long_description': '# PyTorch-IE: State-of-the-art Information Extraction in PyTorch\n\n[![PyPI](https://img.shields.io/pypi/v/pytorch-ie.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/pytorch-ie.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/pytorch-ie)][pypi status]\n[![License](https://img.shields.io/pypi/l/pytorch-ie)][license]\n\n[![Read the documentation at https://pytorch-ie.readthedocs.io/](https://img.shields.io/readthedocs/pytorch-ie/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/christophalt/pytorch-ie/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/christophalt/pytorch-ie/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/pytorch-ie/\n[read the docs]: https://pytorch-ie.readthedocs.io/\n[tests]: https://github.com/christophalt/pytorch-ie/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/christophalt/pytorch-ie\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## 🤯 What\'s this about?\n\nThis is an experimental framework that aims to combine the lessons learned from five years of information extraction research.\n\n-   **Focus on the core task:** The main goal is to develop information extraction methods not dataset loading and evaluation logic. We use external well-maintained libraries for non-core functionality. PyTorch-Lightning for training and logging, Huggingface datasets for dataset reading, and Huggingface evaluate for evaluation (coming soon).\n-   **Sharing is caring:** Being able to quickly and easily share models is key to promote your work and facilitate further research. All models developed in PyTorch-IE can be easily shared via the Huggingface model hub. This further allows to quickly build demos based on Huggingface spaces, gradio or streamlit.\n-   **Unified document format:** A unified document format allows for quick experimentation on any dataset or task.\n-   **Beyond sentence level:** Most information extraction frameworks assume text inputs at a sentence granularity. We do not make any assumption on the granularity but generally aim for document-level information extraction.\n-   **Beyond unstructured text:** Unstructured text is only one possible area for information extraction. We developed the framework to also support information extraction from semi-structured text (e.g. HTML), two-dimensional text (e.g. OCR\'d images), and images.\n-   **Character-level annotation and evaluation:** Many information extraction frameworks annotate and evaluate on a token level. We believe that annotation and evaluation should be done on a character level as this also considers the suitability of the tokenizer for the task.\n-   **Make no assumptions on the structure of models:** The last years have seen many different and creative approaches to information extraction and a framework that imposes a structure on those will most certainly be to limiting. With PyTorch-iE you have full control over how a document is prepared for a model and how the model is structured. The logic is self-contained and thus can be easily shared and inspected by others. The only assumption we make is that the input is a document and the output are targets (training) or annotations (inference).\n\n## 🚀️ Quickstart\n\n```console\n$ pip install pytorch-ie\n```\n\n## 🔭 Demos\n\n| Task                                                       | Link                                                                                                                                                                  |\n| ---------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| Named Entity Recognition (Span-based)                      | [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/pie/NER)                               |\n| Joint Named Entity Recognition and Relation Classification | [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/pie/Joint-NER-and-Relation-Extraction) |\n\n## 📚 Datasets\n\nWe parse all datasets into a common format that can be loaded directly from the model hub via Huggingface datasets. The documents are cached in an arrow table and serialized / deserialized on the fly. Any changes or preprocessing applied to the documents will be cached as well.\n\n```python\nimport datasets\n\ndataset = datasets.load_dataset("pie/conll2003")\n\nprint(dataset["train"][0])\n# >>> CoNLL2003Document(text=\'EU rejects German call to boycott British lamb .\', id=\'0\', metadata={})\n\ndataset["train"][0].entities\n# >>> AnnotationList([LabeledSpan(start=0, end=2, label=\'ORG\', score=1.0), LabeledSpan(start=11, end=17, label=\'MISC\', score=1.0), LabeledSpan(start=34, end=41, label=\'MISC\', score=1.0)])\n\nentity = dataset["train"][0].entities[1]\n\nprint(f"[{entity.start}, {entity.end}] {entity}")\n# >>> [11, 17] German\n```\n\n<details>\n<summary><b>How to create your own Pytorch-IE dataset</b></summary>\n\nPyTorch-IE datasets are built on top of Huggingface datasets. For instance, consider the\n[conll2003 from the Huggingface Hub](https://huggingface.co/datasets/conll2003) and especially their respective\n[dataset loading script](https://huggingface.co/datasets/conll2003/blob/main/conll2003.py). To create a PyTorch-IE\ndataset from that, you have to implement:\n\n1. A Document class. This will be the type of individual dataset examples.\n\n```python\n@dataclass\nclass CoNLL2003Document(TextDocument):\n    entities: AnnotationList[LabeledSpan] = annotation_field(target="text")\n```\n\nHere we derive from `TextDocument` that has a simple `text` string as base annotation target. The `CoNLL2003Document`\nadds one single annotation list called `entities` that consists of `LabeledSpan`s which reference the `text` field of\nthe document. You can add further annotation types by adding `AnnotationList` fields that may also reference (i.e.\n`target`) other annotations as you like. See [\'pytorch_ie.annotations`](src/pytorch_ie/annotations.py) for predefined\nannotation types.\n\n2. A dataset config. This is similar to\n   [creating a Huggingface dataset config](https://huggingface.co/docs/datasets/dataset_script#multiple-configurations).\n\n```python\nclass CoNLL2003Config(datasets.BuilderConfig):\n    """BuilderConfig for CoNLL2003"""\n\n    def __init__(self, **kwargs):\n        """BuilderConfig for CoNLL2003.\n        Args:\n          **kwargs: keyword arguments forwarded to super.\n        """\n        super().__init__(**kwargs)\n```\n\n3. A dataset builder class. This should inherit from\n   [`pytorch_ie.data.builder.GeneratorBasedBuilder`](src/pytorch_ie/data/builder.py) which is a wrapper around the\n   [Huggingface dataset builder class](https://huggingface.co/docs/datasets/v2.4.0/en/package_reference/builder_classes#datasets.GeneratorBasedBuilder)\n   with some utility functionality to work with PyTorch-IE `Documents`. The key elements to implement are: `DOCUMENT_TYPE`,\n   `BASE_DATASET_PATH`, and `_generate_document`.\n\n```python\nclass Conll2003(pytorch_ie.data.builder.GeneratorBasedBuilder):\n    # Specify the document type. This will be the class of individual dataset examples.\n    DOCUMENT_TYPE = CoNLL2003Document\n\n    # The Huggingface identifier that points to the base dataset. This may be any string that works\n    # as path with Huggingface `datasets.load_dataset`.\n    BASE_DATASET_PATH = "conll2003"\n\n    # The builder configs, see https://huggingface.co/docs/datasets/dataset_script for further information.\n    BUILDER_CONFIGS = [\n        CoNLL2003Config(\n            name="conll2003", version=datasets.Version("1.0.0"), description="CoNLL2003 dataset"\n        ),\n    ]\n\n    # [Optional] Define additional keyword arguments which will be passed to `_generate_document` below.\n    def _generate_document_kwargs(self, dataset):\n        return {"int_to_str": dataset.features["ner_tags"].feature.int2str}\n\n    # Define how a Pytorch-IE Document will be created from a Huggingface dataset example.\n    def _generate_document(self, example, int_to_str):\n        doc_id = example["id"]\n        tokens = example["tokens"]\n        ner_tags = [int_to_str(tag) for tag in example["ner_tags"]]\n\n        text, ner_spans = tokens_and_tags_to_text_and_labeled_spans(tokens=tokens, tags=ner_tags)\n\n        document = CoNLL2003Document(text=text, id=doc_id)\n\n        for span in sorted(ner_spans, key=lambda span: span.start):\n            document.entities.append(span)\n\n        return document\n```\n\nThe full script can be found here: [datasets/conll2003/conll2003.py](datasets/conll2003/conll2003.py). Note, that to\nload the dataset with `datasets.load_dataset`, the script has to be located in a directory with the same name (as it\nis the case for standard Huggingface dataset loading scripts).\n\n</details>\n\n## ⚡️ Example\n\n**Note:** Setting `num_workers=0` in the pipeline is only necessary when running an example in an\ninteractive python session. The reason is that multiprocessing doesn\'t play well with the interactive python\ninterpreter, see [here](https://docs.python.org/3/library/multiprocessing.html#using-a-pool-of-workers)\nfor details.\n\n### Span-classification-based Named Entity Recognition\n\n```python\nfrom dataclasses import dataclass\n\nfrom pytorch_ie.annotations import LabeledSpan\nfrom pytorch_ie.auto import AutoPipeline\nfrom pytorch_ie.core import AnnotationList, annotation_field\nfrom pytorch_ie.documents import TextDocument\n\n@dataclass\nclass ExampleDocument(TextDocument):\n    entities: AnnotationList[LabeledSpan] = annotation_field(target="text")\n\ndocument = ExampleDocument(\n    "“Making a super tasty alt-chicken wing is only half of it,” said Po Bronson, general partner at SOSV and managing director of IndieBio."\n)\n\n# see below for the long version\nner_pipeline = AutoPipeline.from_pretrained("pie/example-ner-spanclf-conll03", device=-1, num_workers=0)\n\nner_pipeline(document, predict_field="entities")\n\nfor entity in document.entities.predictions:\n    print(f"{entity} -> {entity.label}")\n\n# Result:\n# IndieBio -> ORG\n# Po Bronson -> PER\n# SOSV -> ORG\n```\n\nTo create the same pipeline as above without `AutoPipeline`:\n\n```python\nfrom pytorch_ie.auto import AutoTaskModule, AutoModel\nfrom pytorch_ie.pipeline import Pipeline\n\nmodel_name_or_path = "pie/example-ner-spanclf-conll03"\nner_taskmodule = AutoTaskModule.from_pretrained(model_name_or_path)\nner_model = AutoModel.from_pretrained(model_name_or_path)\nner_pipeline = Pipeline(model=ner_model, taskmodule=ner_taskmodule, device=-1, num_workers=0)\n```\n\nOr, without `Auto` classes at all:\n\n```python\nfrom pytorch_ie.pipeline import Pipeline\nfrom pytorch_ie.models import TransformerSpanClassificationModel\nfrom pytorch_ie.taskmodules import TransformerSpanClassificationTaskModule\n\nmodel_name_or_path = "pie/example-ner-spanclf-conll03"\nner_taskmodule = TransformerSpanClassificationTaskModule.from_pretrained(model_name_or_path)\nner_model = TransformerSpanClassificationModel.from_pretrained(model_name_or_path)\nner_pipeline = Pipeline(model=ner_model, taskmodule=ner_taskmodule, device=-1, num_workers=0)\n```\n\n## ⚡️️️️ More Examples\n\n### Text-classification-based Relation Extraction\n\n```python\nfrom dataclasses import dataclass\n\nfrom pytorch_ie.annotations import BinaryRelation, LabeledSpan\nfrom pytorch_ie.auto import AutoPipeline\nfrom pytorch_ie.core import AnnotationList, annotation_field\nfrom pytorch_ie.documents import TextDocument\n\n\n@dataclass\nclass ExampleDocument(TextDocument):\n    entities: AnnotationList[LabeledSpan] = annotation_field(target="text")\n    relations: AnnotationList[BinaryRelation] = annotation_field(target="entities")\n\ndocument = ExampleDocument(\n    "“Making a super tasty alt-chicken wing is only half of it,” said Po Bronson, general partner at SOSV and managing director of IndieBio."\n)\n\nre_pipeline = AutoPipeline.from_pretrained("pie/example-re-textclf-tacred", device=-1, num_workers=0)\n\nfor start, end, label in [(65, 75, "PER"), (96, 100, "ORG"), (126, 134, "ORG")]:\n    document.entities.append(LabeledSpan(start=start, end=end, label=label))\n\nre_pipeline(document, predict_field="relations", batch_size=2)\n\nfor relation in document.relations.predictions:\n    print(f"({relation.head} -> {relation.tail}) -> {relation.label}")\n\n# Result:\n# (Po Bronson -> SOSV) -> per:employee_of\n# (Po Bronson -> IndieBio) -> per:employee_of\n# (SOSV -> Po Bronson) -> org:top_members/employees\n# (IndieBio -> Po Bronson) -> org:top_members/employees\n```\n\n<!-- github-only -->\n\n✨📚✨ [Read the full documentation](https://pytorch-ie.readthedocs.io/)\n\n## 🔧 Development Setup\n\n## 🏅 Acknowledgements\n\n-   This package is based on the [sourcery-ai/python-best-practices-cookiecutter](https://github.com/sourcery-ai/python-best-practices-cookiecutter) and [cjolowicz/cookiecutter-hypermodern-python](https://github.com/cjolowicz/cookiecutter-hypermodern-python) project templates.\n\n## 📃 Citation\n\nIf you find the framework useful please consider citing it:\n\n```bibtex\n@misc{alt2022pytorchie,\n    author={Christoph Alt, Arne Binder},\n    title = {PyTorch-IE: State-of-the-art Information Extraction in PyTorch},\n    year = {2022},\n    publisher = {GitHub},\n    journal = {GitHub repository},\n    howpublished = {\\url{https://github.com/ChristophAlt/pytorch-ie}}\n}\n```\n\n[license]: https://github.com/christophalt/pytorch-ie/blob/main/LICENSE\n',
     'author': 'Christoph Alt',
     'author_email': 'christoph.alt@posteo.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/christophalt/pytorch-ie',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pytorch-ie-0.8.0/PKG-INFO` & `pytorch-ie-0.9.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: pytorch-ie
-Version: 0.8.0
-Summary: State-of-the-art Information Extraction in PyTorch
-Home-page: https://github.com/christophalt/pytorch-ie
-License: MIT
-Author: Christoph Alt
-Author-email: christoph.alt@posteo.de
-Requires-Python: >=3.9,<4.0
-Classifier: Framework :: Pytest
-Classifier: Framework :: Sphinx
-Classifier: Framework :: tox
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: datasets (>=2.3.2,<3.0.0)
-Requires-Dist: huggingface-hub (>=0.5.1,<0.6.0)
-Requires-Dist: pytorch-lightning (>=1.6.1,<2.0.0)
-Requires-Dist: torchmetrics (>=0.8.0,<0.9.0)
-Requires-Dist: transformers (>=4.18.0,<5.0.0)
-Project-URL: Bug Tracker, https://github.com/christophalt/pytorch-ie/issues
-Project-URL: Changelog, https://github.com/christophalt/pytorch-ie/releases
-Project-URL: Documentation, https://pytorch-ie.readthedocs.io
-Project-URL: Repository, https://github.com/christophalt/pytorch-ie
-Description-Content-Type: text/markdown
-
 # PyTorch-IE: State-of-the-art Information Extraction in PyTorch
 
 [![PyPI](https://img.shields.io/pypi/v/pytorch-ie.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/pytorch-ie.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/pytorch-ie)][pypi status]
 [![License](https://img.shields.io/pypi/l/pytorch-ie)][license]
 
@@ -64,18 +35,18 @@
 
 ```console
 $ pip install pytorch-ie
 ```
 
 ## 🔭 Demos
 
-| Task                                                       | Link (Huggingface Spaces)                                                   |
-| ---------------------------------------------------------- | --------------------------------------------------------------------------- |
-| Named Entity Recognition (Span-based)                      | [LINK](https://huggingface.co/spaces/pie/NER)                               |
-| Joint Named Entity Recognition and Relation Classification | [LINK](https://huggingface.co/spaces/pie/Joint-NER-and-Relation-Extraction) |
+| Task                                                       | Link                                                                                                                                                                  |
+| ---------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Named Entity Recognition (Span-based)                      | [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/pie/NER)                               |
+| Joint Named Entity Recognition and Relation Classification | [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/pie/Joint-NER-and-Relation-Extraction) |
 
 ## 📚 Datasets
 
 We parse all datasets into a common format that can be loaded directly from the model hub via Huggingface datasets. The documents are cached in an arrow table and serialized / deserialized on the fly. Any changes or preprocessing applied to the documents will be cached as well.
 
 ```python
 import datasets
@@ -90,14 +61,99 @@
 
 entity = dataset["train"][0].entities[1]
 
 print(f"[{entity.start}, {entity.end}] {entity}")
 # >>> [11, 17] German
 ```
 
+<details>
+<summary><b>How to create your own Pytorch-IE dataset</b></summary>
+
+PyTorch-IE datasets are built on top of Huggingface datasets. For instance, consider the
+[conll2003 from the Huggingface Hub](https://huggingface.co/datasets/conll2003) and especially their respective
+[dataset loading script](https://huggingface.co/datasets/conll2003/blob/main/conll2003.py). To create a PyTorch-IE
+dataset from that, you have to implement:
+
+1. A Document class. This will be the type of individual dataset examples.
+
+```python
+@dataclass
+class CoNLL2003Document(TextDocument):
+    entities: AnnotationList[LabeledSpan] = annotation_field(target="text")
+```
+
+Here we derive from `TextDocument` that has a simple `text` string as base annotation target. The `CoNLL2003Document`
+adds one single annotation list called `entities` that consists of `LabeledSpan`s which reference the `text` field of
+the document. You can add further annotation types by adding `AnnotationList` fields that may also reference (i.e.
+`target`) other annotations as you like. See ['pytorch_ie.annotations`](src/pytorch_ie/annotations.py) for predefined
+annotation types.
+
+2. A dataset config. This is similar to
+   [creating a Huggingface dataset config](https://huggingface.co/docs/datasets/dataset_script#multiple-configurations).
+
+```python
+class CoNLL2003Config(datasets.BuilderConfig):
+    """BuilderConfig for CoNLL2003"""
+
+    def __init__(self, **kwargs):
+        """BuilderConfig for CoNLL2003.
+        Args:
+          **kwargs: keyword arguments forwarded to super.
+        """
+        super().__init__(**kwargs)
+```
+
+3. A dataset builder class. This should inherit from
+   [`pytorch_ie.data.builder.GeneratorBasedBuilder`](src/pytorch_ie/data/builder.py) which is a wrapper around the
+   [Huggingface dataset builder class](https://huggingface.co/docs/datasets/v2.4.0/en/package_reference/builder_classes#datasets.GeneratorBasedBuilder)
+   with some utility functionality to work with PyTorch-IE `Documents`. The key elements to implement are: `DOCUMENT_TYPE`,
+   `BASE_DATASET_PATH`, and `_generate_document`.
+
+```python
+class Conll2003(pytorch_ie.data.builder.GeneratorBasedBuilder):
+    # Specify the document type. This will be the class of individual dataset examples.
+    DOCUMENT_TYPE = CoNLL2003Document
+
+    # The Huggingface identifier that points to the base dataset. This may be any string that works
+    # as path with Huggingface `datasets.load_dataset`.
+    BASE_DATASET_PATH = "conll2003"
+
+    # The builder configs, see https://huggingface.co/docs/datasets/dataset_script for further information.
+    BUILDER_CONFIGS = [
+        CoNLL2003Config(
+            name="conll2003", version=datasets.Version("1.0.0"), description="CoNLL2003 dataset"
+        ),
+    ]
+
+    # [Optional] Define additional keyword arguments which will be passed to `_generate_document` below.
+    def _generate_document_kwargs(self, dataset):
+        return {"int_to_str": dataset.features["ner_tags"].feature.int2str}
+
+    # Define how a Pytorch-IE Document will be created from a Huggingface dataset example.
+    def _generate_document(self, example, int_to_str):
+        doc_id = example["id"]
+        tokens = example["tokens"]
+        ner_tags = [int_to_str(tag) for tag in example["ner_tags"]]
+
+        text, ner_spans = tokens_and_tags_to_text_and_labeled_spans(tokens=tokens, tags=ner_tags)
+
+        document = CoNLL2003Document(text=text, id=doc_id)
+
+        for span in sorted(ner_spans, key=lambda span: span.start):
+            document.entities.append(span)
+
+        return document
+```
+
+The full script can be found here: [datasets/conll2003/conll2003.py](datasets/conll2003/conll2003.py). Note, that to
+load the dataset with `datasets.load_dataset`, the script has to be located in a directory with the same name (as it
+is the case for standard Huggingface dataset loading scripts).
+
+</details>
+
 ## ⚡️ Example
 
 **Note:** Setting `num_workers=0` in the pipeline is only necessary when running an example in an
 interactive python session. The reason is that multiprocessing doesn't play well with the interactive python
 interpreter, see [here](https://docs.python.org/3/library/multiprocessing.html#using-a-pool-of-workers)
 for details.
 
@@ -219,8 +275,7 @@
     publisher = {GitHub},
     journal = {GitHub repository},
     howpublished = {\url{https://github.com/ChristophAlt/pytorch-ie}}
 }
 ```
 
 [license]: https://github.com/christophalt/pytorch-ie/blob/main/LICENSE
-
```

