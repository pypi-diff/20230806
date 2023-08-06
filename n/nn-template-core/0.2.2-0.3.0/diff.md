# Comparing `tmp/nn-template-core-0.2.2.tar.gz` & `tmp/nn-template-core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn-template-core-0.2.2.tar", last modified: Mon Mar 20 14:41:06 2023, max compression
+gzip compressed data, was "nn-template-core-0.3.0.tar", last modified: Sun Aug  6 08:30:54 2023, max compression
```

## Comparing `nn-template-core-0.2.2.tar` & `nn-template-core-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 14:41:06.031937 nn-template-core-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 14:41:06.027937 nn-template-core-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 14:41:06.031937 nn-template-core-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3648 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     4056 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-03-20 14:41:06.031937 nn-template-core-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/env.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-03-20 14:41:06.031937 nn-template-core-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 14:41:06.027937 nn-template-core-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 14:41:06.031937 nn-template-core-0.2.2/src/nn_core/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-20 14:41:05.000000 nn-template-core-0.2.2/src/nn_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 14:41:06.031937 nn-template-core-0.2.2/src/nn_core/common/
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/console_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/model_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/nn_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     4398 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/resume.py
--rw-r--r--   0 runner    (1001) docker     (122)     6835 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-03-20 14:39:04.000000 nn-template-core-0.2.2/src/nn_core/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 14:41:06.031937 nn-template-core-0.2.2/src/nn_template_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-03-20 14:41:06.000000 nn-template-core-0.2.2/src/nn_template_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-03-20 14:41:06.000000 nn-template-core-0.2.2/src/nn_template_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 14:41:06.000000 nn-template-core-0.2.2/src/nn_template_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 14:40:19.000000 nn-template-core-0.2.2/src/nn_template_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-03-20 14:41:06.000000 nn-template-core-0.2.2/src/nn_template_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-20 14:41:06.000000 nn-template-core-0.2.2/src/nn_template_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3648 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     4056 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-08-06 08:30:54.931515 nn-template-core-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/src/nn_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/src/nn_core/common/
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/console_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8500 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/model_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/nn_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4398 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/resume.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6835 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-08-06 08:23:41.000000 nn-template-core-0.3.0/src/nn_core/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 08:30:54.927515 nn-template-core-0.3.0/src/nn_template_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 08:30:08.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-08-06 08:30:54.000000 nn-template-core-0.3.0/src/nn_template_core.egg-info/top_level.txt
```

### Comparing `nn-template-core-0.2.2/.github/workflows/publish_pypi.yml` & `nn-template-core-0.3.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/.gitignore` & `nn-template-core-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/.pre-commit-config.yaml` & `nn-template-core-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/LICENSE` & `nn-template-core-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/pyproject.toml` & `nn-template-core-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/setup.cfg` & `nn-template-core-0.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [options]
 zip_safe = False
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	pytorch-lightning==1.7.*
+	lightning==2.0.*
 	hydra-core
 	wandb
 	
 	python-dotenv
 	stqdm
 	rich
```

### Comparing `nn-template-core-0.2.2/src/nn_core/callbacks.py` & `nn-template-core-0.3.0/src/nn_core/callbacks.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/src/nn_core/common/utils.py` & `nn-template-core-0.3.0/src/nn_core/common/utils.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/src/nn_core/console_logging.py` & `nn-template-core-0.3.0/src/nn_core/console_logging.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/src/nn_core/model_logging.py` & `nn-template-core-0.3.0/src/nn_core/model_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from typing import Any, Dict, Optional, Union
 
 import hydra
 import pytorch_lightning
 from omegaconf import DictConfig, OmegaConf
 from pytorch_lightning import LightningModule, Trainer
 from pytorch_lightning.callbacks import ModelCheckpoint
-from pytorch_lightning.loggers import LightningLoggerBase
+from pytorch_lightning.loggers.logger import Logger
 
 from nn_core.common import PROJECT_ROOT
 
 pylogger = logging.getLogger(__name__)
 
 
 _STATS_KEY: str = "stats"
 
 
-class NNLogger(LightningLoggerBase):
+class NNLogger(Logger):
 
-    __doc__ = LightningLoggerBase.__doc__
+    __doc__ = Logger.__doc__
 
     def __init__(self, logging_cfg: DictConfig, cfg: DictConfig, resume_id: Optional[str]):
         super().__init__()
         self.logging_cfg = logging_cfg
         self.cfg = cfg
         self.resume_id = resume_id
 
@@ -35,15 +35,15 @@
 
         if self.cfg.train.trainer.fast_dev_run and self.wandb:
             # Switch wandb mode to offline to prevent online logging
             pylogger.info("Setting the logger in 'offline' mode")
             self.logging_cfg.logger.mode = "offline"
 
         pylogger.info(f"Instantiating <{self.logging_cfg.logger['_target_'].split('.')[-1]}>")
-        self.wrapped: LightningLoggerBase = hydra.utils.instantiate(
+        self.wrapped: Logger = hydra.utils.instantiate(
             self.logging_cfg.logger,
             version=self.resume_id,
             dir=os.getenv("WANDB_DIR", "."),
         )
 
         # force experiment lazy initialization
         _ = self.wrapped.experiment
@@ -111,15 +111,15 @@
         return self.wrapped.experiment
 
     def log_metrics(self, metrics: Dict[str, float], step: Optional[int] = None):
         """Records metrics.
 
         This method logs metrics as as soon as it received them. If you want to aggregate
         metrics for one specific `step`, use the
-        :meth:`~pytorch_lightning.loggers.base.LightningLoggerBase.agg_and_log_metrics` method.
+        :meth:`~pytorch_lightning.loggers.base.Logger.agg_and_log_metrics` method.
 
         Args:
             metrics: Dictionary with metric names as keys and measured quantities as values
             step: Step number at which the metrics should be recorded
         """
         return self.wrapped.log_metrics(metrics=metrics, step=step)
```

### Comparing `nn-template-core-0.2.2/src/nn_core/resume.py` & `nn-template-core-0.3.0/src/nn_core/resume.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/src/nn_core/serialization.py` & `nn-template-core-0.3.0/src/nn_core/serialization.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/src/nn_core/ui.py` & `nn-template-core-0.3.0/src/nn_core/ui.py`

 * *Files identical despite different names*

### Comparing `nn-template-core-0.2.2/src/nn_template_core.egg-info/SOURCES.txt` & `nn-template-core-0.3.0/src/nn_template_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

