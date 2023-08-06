# Comparing `tmp/option_trader-0.2.0.tar.gz` & `tmp/option_trader-0.2.1.tar.gz`

## Comparing `option_trader-0.2.0.tar` & `option_trader-0.2.1.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 option_trader-0.2.0/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 option_trader-0.2.0/.vscode/launch.json
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 option_trader-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0    85832 2020-02-02 00:00:00.000000 option_trader-0.2.0/admin/account.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 option_trader-0.2.0/admin/option_summary.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 option_trader-0.2.0/admin/position.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 option_trader-0.2.0/admin/quote.py
--rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 option_trader-0.2.0/admin/site.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 option_trader-0.2.0/admin/transaction.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 option_trader-0.2.0/admin/user.py
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/option/butterfly.py
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/option/credit_iron_condor.py
--rw-r--r--   0        0        0    10029 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/option/single_option.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/option/spread.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/option/strategy.py
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/stock/bollingerBands.py
--rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/stock/macd.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/stock/mfi.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 option_trader-0.2.0/backtest/stock/rsi.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 option_trader-0.2.0/consts/asset.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 option_trader-0.2.0/consts/predictor.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 option_trader-0.2.0/consts/rgb.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 option_trader-0.2.0/consts/strategy.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 option_trader-0.2.0/jobs/account.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 option_trader-0.2.0/jobs/core.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 option_trader-0.2.0/jobs/site.py
--rw-r--r--   0        0        0    25258 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/Ananlyzer.ipynb
--rw-r--r--   0        0        0   431156 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/ML_TensorFlow_good.ipynb
--rw-r--r--   0        0        0   370663 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/ML_ochl.ipynb
--rw-r--r--   0        0        0   252673 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/MP_TensorFlow_bad.ipynb
--rw-r--r--   0        0        0   110764 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/admin.ipynb
--rw-r--r--   0        0        0   193512 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/ib.ipynb
--rw-r--r--   0        0        0   266277 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/ml.ipynb
--rw-r--r--   0        0        0    64170 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/option_geeks.ipynb
--rw-r--r--   0        0        0    58956 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/option_tools.ipynb
--rw-r--r--   0        0        0    28065 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/watchlist.ipynb
--rw-r--r--   0        0        0   251657 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/Ananlyzer-checkpoint.ipynb
--rw-r--r--   0        0        0   359863 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/ML_TensorFlow_good-checkpoint.ipynb
--rw-r--r--   0        0        0   370671 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/ML_ochl-checkpoint.ipynb
--rw-r--r--   0        0        0   359863 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/MP_TensorFlow_bad-checkpoint.ipynb
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0    37481 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/admin-checkpoint.ipynb
--rw-r--r--   0        0        0    25565 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/ib-checkpoint.ipynb
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/ml-checkpoint.ipynb
--rw-r--r--   0        0        0    46403 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/option_geeks-checkpoint.ipynb
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/option_tools-checkpoint.ipynb
--rw-r--r--   0        0        0    44140 2020-02-02 00:00:00.000000 option_trader-0.2.0/notebook/.ipynb_checkpoints/watchlist-checkpoint.ipynb
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 option_trader-0.2.0/settings/app_settings.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 option_trader-0.2.0/settings/ib_config.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 option_trader-0.2.0/settings/log_config.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 option_trader-0.2.0/settings/logging.conf
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 option_trader-0.2.0/settings/schema.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 option_trader-0.2.0/settings/ta_strategy.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 option_trader-0.2.0/settings/trade_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 option_trader-0.2.0/shell/analyzer.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 option_trader-0.2.0/shell/backtester.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 option_trader-0.2.0/shell/dataset_tool.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 option_trader-0.2.0/shell/line.py
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 option_trader-0.2.0/utils/calc_prob.py
--rw-r--r--   0        0        0    72821 2020-02-02 00:00:00.000000 option_trader-0.2.0/utils/data_getter.py
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 option_trader-0.2.0/utils/data_getter_ib.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 option_trader-0.2.0/utils/line_norify.py
--rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 option_trader-0.2.0/utils/monitor.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 option_trader-0.2.0/utils/optionTool.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 option_trader-0.2.0/utils/predictor.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 option_trader-0.2.0/.gitignore
--rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 option_trader-0.2.0/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 option_trader-0.2.0/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 option_trader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 option_trader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 option_trader-0.2.1/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 option_trader-0.2.1/.vscode/launch.json
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 option_trader-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0    85832 2020-02-02 00:00:00.000000 option_trader-0.2.1/admin/account.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 option_trader-0.2.1/admin/option_summary.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 option_trader-0.2.1/admin/position.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 option_trader-0.2.1/admin/quote.py
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 option_trader-0.2.1/admin/site.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 option_trader-0.2.1/admin/transaction.py
+-rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 option_trader-0.2.1/admin/user.py
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/option/butterfly.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/option/credit_iron_condor.py
+-rw-r--r--   0        0        0    10029 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/option/single_option.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/option/spread.py
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/option/strategy.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/stock/bollingerBands.py
+-rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/stock/macd.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/stock/mfi.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 option_trader-0.2.1/backtest/stock/rsi.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 option_trader-0.2.1/consts/asset.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 option_trader-0.2.1/consts/predictor.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 option_trader-0.2.1/consts/rgb.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 option_trader-0.2.1/consts/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 option_trader-0.2.1/jobs/__init__.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 option_trader-0.2.1/jobs/account.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 option_trader-0.2.1/jobs/core.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 option_trader-0.2.1/jobs/site.py
+-rw-r--r--   0        0        0    25258 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/Ananlyzer.ipynb
+-rw-r--r--   0        0        0   431156 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/ML_TensorFlow_good.ipynb
+-rw-r--r--   0        0        0   370663 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/ML_ochl.ipynb
+-rw-r--r--   0        0        0   252673 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/MP_TensorFlow_bad.ipynb
+-rw-r--r--   0        0        0   110764 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/admin.ipynb
+-rw-r--r--   0        0        0   193512 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/ib.ipynb
+-rw-r--r--   0        0        0   266277 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/ml.ipynb
+-rw-r--r--   0        0        0    64170 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/option_geeks.ipynb
+-rw-r--r--   0        0        0    58956 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/option_tools.ipynb
+-rw-r--r--   0        0        0    28065 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/watchlist.ipynb
+-rw-r--r--   0        0        0   251657 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/Ananlyzer-checkpoint.ipynb
+-rw-r--r--   0        0        0   359863 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/ML_TensorFlow_good-checkpoint.ipynb
+-rw-r--r--   0        0        0   370671 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/ML_ochl-checkpoint.ipynb
+-rw-r--r--   0        0        0   359863 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/MP_TensorFlow_bad-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0    37481 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/admin-checkpoint.ipynb
+-rw-r--r--   0        0        0    25565 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/ib-checkpoint.ipynb
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/ml-checkpoint.ipynb
+-rw-r--r--   0        0        0    46403 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/option_geeks-checkpoint.ipynb
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/option_tools-checkpoint.ipynb
+-rw-r--r--   0        0        0    44140 2020-02-02 00:00:00.000000 option_trader-0.2.1/notebook/.ipynb_checkpoints/watchlist-checkpoint.ipynb
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 option_trader-0.2.1/settings/app_settings.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 option_trader-0.2.1/settings/ib_config.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 option_trader-0.2.1/settings/log_config.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 option_trader-0.2.1/settings/logging.conf
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 option_trader-0.2.1/settings/schema.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 option_trader-0.2.1/settings/ta_strategy.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 option_trader-0.2.1/settings/trade_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 option_trader-0.2.1/shell/analyzer.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 option_trader-0.2.1/shell/backtester.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 option_trader-0.2.1/shell/dataset_tool.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 option_trader-0.2.1/shell/line.py
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 option_trader-0.2.1/utils/calc_prob.py
+-rw-r--r--   0        0        0    72821 2020-02-02 00:00:00.000000 option_trader-0.2.1/utils/data_getter.py
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 option_trader-0.2.1/utils/data_getter_ib.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 option_trader-0.2.1/utils/line_norify.py
+-rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 option_trader-0.2.1/utils/monitor.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 option_trader-0.2.1/utils/optionTool.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 option_trader-0.2.1/utils/predictor.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 option_trader-0.2.1/.gitignore
+-rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 option_trader-0.2.1/LICENSE
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 option_trader-0.2.1/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 option_trader-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 option_trader-0.2.1/PKG-INFO
```

### Comparing `option_trader-0.2.0/.vscode/launch.json` & `option_trader-0.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/admin/account.py` & `option_trader-0.2.1/admin/account.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/admin/option_summary.py` & `option_trader-0.2.1/admin/option_summary.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/admin/position.py` & `option_trader-0.2.1/admin/position.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/admin/quote.py` & `option_trader-0.2.1/admin/quote.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/admin/site.py` & `option_trader-0.2.1/admin/site.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/admin/transaction.py` & `option_trader-0.2.1/admin/transaction.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/admin/user.py` & `option_trader-0.2.1/admin/user.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/option/butterfly.py` & `option_trader-0.2.1/backtest/option/butterfly.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/option/credit_iron_condor.py` & `option_trader-0.2.1/backtest/option/credit_iron_condor.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/option/single_option.py` & `option_trader-0.2.1/backtest/option/single_option.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/option/spread.py` & `option_trader-0.2.1/backtest/option/spread.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/option/strategy.py` & `option_trader-0.2.1/backtest/option/strategy.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/stock/bollingerBands.py` & `option_trader-0.2.1/backtest/stock/bollingerBands.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/stock/macd.py` & `option_trader-0.2.1/backtest/stock/macd.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/stock/mfi.py` & `option_trader-0.2.1/backtest/stock/mfi.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/backtest/stock/rsi.py` & `option_trader-0.2.1/backtest/stock/rsi.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/consts/asset.py` & `option_trader-0.2.1/consts/asset.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/consts/strategy.py` & `option_trader-0.2.1/consts/strategy.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/jobs/account.py` & `option_trader-0.2.1/jobs/account.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/jobs/site.py` & `option_trader-0.2.1/jobs/site.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/Ananlyzer.ipynb` & `option_trader-0.2.1/notebook/Ananlyzer.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/ML_TensorFlow_good.ipynb` & `option_trader-0.2.1/notebook/ML_TensorFlow_good.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/ML_ochl.ipynb` & `option_trader-0.2.1/notebook/ML_ochl.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/MP_TensorFlow_bad.ipynb` & `option_trader-0.2.1/notebook/MP_TensorFlow_bad.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/admin.ipynb` & `option_trader-0.2.1/notebook/admin.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/ib.ipynb` & `option_trader-0.2.1/notebook/ib.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/ml.ipynb` & `option_trader-0.2.1/notebook/ml.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/option_geeks.ipynb` & `option_trader-0.2.1/notebook/option_geeks.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/option_tools.ipynb` & `option_trader-0.2.1/notebook/option_tools.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/watchlist.ipynb` & `option_trader-0.2.1/notebook/watchlist.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/Ananlyzer-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/Ananlyzer-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/ML_TensorFlow_good-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/ML_TensorFlow_good-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/ML_ochl-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/ML_ochl-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/MP_TensorFlow_bad-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/MP_TensorFlow_bad-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/admin-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/admin-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/ib-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/ib-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/ml-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/ml-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/option_geeks-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/option_geeks-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/option_tools-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/option_tools-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/notebook/.ipynb_checkpoints/watchlist-checkpoint.ipynb` & `option_trader-0.2.1/notebook/.ipynb_checkpoints/watchlist-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/settings/app_settings.py` & `option_trader-0.2.1/settings/app_settings.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/settings/log_config.py` & `option_trader-0.2.1/settings/log_config.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/settings/logging.conf` & `option_trader-0.2.1/settings/logging.conf`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/settings/schema.py` & `option_trader-0.2.1/settings/schema.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/settings/trade_config.py` & `option_trader-0.2.1/settings/trade_config.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/shell/analyzer.py` & `option_trader-0.2.1/shell/analyzer.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/shell/backtester.py` & `option_trader-0.2.1/shell/backtester.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/shell/dataset_tool.py` & `option_trader-0.2.1/shell/dataset_tool.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/shell/line.py` & `option_trader-0.2.1/shell/line.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/utils/calc_prob.py` & `option_trader-0.2.1/utils/calc_prob.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/utils/data_getter.py` & `option_trader-0.2.1/utils/data_getter.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/utils/data_getter_ib.py` & `option_trader-0.2.1/utils/data_getter_ib.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/utils/line_norify.py` & `option_trader-0.2.1/utils/line_norify.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/utils/monitor.py` & `option_trader-0.2.1/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/utils/optionTool.py` & `option_trader-0.2.1/utils/optionTool.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/utils/predictor.py` & `option_trader-0.2.1/utils/predictor.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/LICENSE` & `option_trader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.0/pyproject.toml` & `option_trader-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "option_trader"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Jim Huang", email="jim.huang.taipei@outlook.com" },
 ]
 description = "Option Trading Robot package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `option_trader-0.2.0/PKG-INFO` & `option_trader-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: option_trader
-Version: 0.2.0
+Version: 0.2.1
 Summary: Option Trading Robot package
 Project-URL: Homepage, https://github.com/pypa/OptionTradeproject
 Project-URL: Bug Tracker, https://github.com/pypa/OptionTrader/issues
 Author-email: Jim Huang <jim.huang.taipei@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

