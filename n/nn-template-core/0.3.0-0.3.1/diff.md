# Comparing `tmp/nn-template-core-0.3.0.tar.gz` & `tmp/nn-template-core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn-template-core-0.3.0.tar", last modified: Sun Aug  6 08:30:54 2023, max compression
+gzip compressed data, was "nn-template-core-0.3.1.tar", last modified: Sun Aug  6 08:39:08 2023, max compression
```

## Comparing `nn-template-core-0.3.0.tar` & `nn-template-core-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3648 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     4056 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/env.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-08-06 08:30:54.931515 nn-template-core-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/src/nn_core/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/src/nn_core/common/
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/console_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     8500 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/model_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/nn_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     4398 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/resume.py
--rw-r--r--   0 runner    (1001) docker     (122)     6835 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/src/nn_template_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 08:30:08.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:39:08.080565 nn-template-core-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:39:08.068564 nn-template-core-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:39:08.076564 nn-template-core-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3648 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     4056 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-08-06 08:39:08.080565 nn-template-core-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-08-06 08:39:08.084565 nn-template-core-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:39:08.072564 nn-template-core-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:39:08.076564 nn-template-core-0.3.1/src/nn_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-06 08:39:08.000000 nn-template-core-0.3.1/src/nn_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:39:08.080565 nn-template-core-0.3.1/src/nn_core/common/
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/console_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8500 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/model_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/nn_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4398 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/resume.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6835 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-08-06 08:31:19.000000 nn-template-core-0.3.1/src/nn_core/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:39:08.080565 nn-template-core-0.3.1/src/nn_template_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-08-06 08:39:08.000000 nn-template-core-0.3.1/src/nn_template_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-08-06 08:39:08.000000 nn-template-core-0.3.1/src/nn_template_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 08:39:08.000000 nn-template-core-0.3.1/src/nn_template_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 08:38:14.000000 nn-template-core-0.3.1/src/nn_template_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-08-06 08:39:08.000000 nn-template-core-0.3.1/src/nn_template_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-08-06 08:39:08.000000 nn-template-core-0.3.1/src/nn_template_core.egg-info/top_level.txt
```

### Comparing `nn-template-core-0.3.0/.github/workflows/publish_pypi.yml` & `nn-template-core-0.3.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/.gitignore` & `nn-template-core-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/.pre-commit-config.yaml` & `nn-template-core-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/LICENSE` & `nn-template-core-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/pyproject.toml` & `nn-template-core-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/setup.cfg` & `nn-template-core-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/src/nn_core/callbacks.py` & `nn-template-core-0.3.1/src/nn_core/callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pylogger = logging.getLogger(__name__)
 
 
 class NNTemplateCore(Callback):
     def __init__(self, restore_cfg: Optional[DictConfig]):
         self.resume_ckpt_path, self.resume_run_version = parse_restore(restore_cfg)
         self.restore_mode: Optional[str] = restore_cfg.get("mode", None) if restore_cfg is not None else None
+        self.restore_strict: bool = restore_cfg.get("strict", True) if restore_cfg is not None else True
 
     @property
     def resume_id(self) -> Optional[str]:
         return self.resume_run_version
 
     @property
     def trainer_ckpt_path(self) -> Optional[str]:
@@ -37,15 +38,15 @@
             trainer.logger.log_configuration(model=pl_module)
             trainer.logger.watch_model(pl_module=pl_module)
 
     def setup(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule", stage: Optional[str] = None) -> None:
         if self.restore_mode == "finetune":
             checkpoint = NNCheckpointIO.load(path=Path(self.resume_ckpt_path))
 
-            pl_module.load_state_dict(checkpoint["state_dict"])
+            pl_module.load_state_dict(checkpoint["state_dict"], strict=self.restore_strict)
 
     def on_train_end(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
         if self._is_nnlogger(trainer):
             trainer.logger: NNLogger
             trainer.logger.upload_run_files()
 
     def on_save_checkpoint(
```

### Comparing `nn-template-core-0.3.0/src/nn_core/common/utils.py` & `nn-template-core-0.3.1/src/nn_core/common/utils.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/src/nn_core/console_logging.py` & `nn-template-core-0.3.1/src/nn_core/console_logging.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/src/nn_core/model_logging.py` & `nn-template-core-0.3.1/src/nn_core/model_logging.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/src/nn_core/resume.py` & `nn-template-core-0.3.1/src/nn_core/resume.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/src/nn_core/serialization.py` & `nn-template-core-0.3.1/src/nn_core/serialization.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/src/nn_core/ui.py` & `nn-template-core-0.3.1/src/nn_core/ui.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.3.0/src/nn_template_core.egg-info/SOURCES.txt` & `nn-template-core-0.3.1/src/nn_template_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

