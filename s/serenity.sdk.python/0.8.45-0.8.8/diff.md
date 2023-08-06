# Comparing `tmp/serenity.sdk.python-0.8.45.tar.gz` & `tmp/serenity.sdk.python-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serenity.sdk.python-0.8.45.tar", max compression
+gzip compressed data, was "serenity.sdk.python-0.8.8.tar", max compression
```

## Comparing `serenity.sdk.python-0.8.45.tar` & `serenity.sdk.python-0.8.8.tar`

### file list

```diff
@@ -1,87 +1,8 @@
--rw-r--r--   0        0        0    11072 2023-08-06 01:03:45.014870 serenity.sdk.python-0.8.45/LICENSE
--rw-r--r--   0        0        0     1363 2023-08-06 01:03:45.014870 serenity.sdk.python-0.8.45/README.md
--rw-r--r--   0        0        0     1070 2023-08-06 01:04:19.091242 serenity.sdk.python-0.8.45/pyproject.toml
--rw-r--r--   0        0        0       22 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/__init__.py
--rw-r--r--   0        0        0     3679 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/account.py
--rw-r--r--   0        0        0     2291 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/core.py
--rw-r--r--   0        0        0     2908 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/model.py
--rw-r--r--   0        0        0     7001 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/portfolio.py
--rw-r--r--   0        0        0     9946 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/pricing.py
--rw-r--r--   0        0        0     2570 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/provider.py
--rw-r--r--   0        0        0     8532 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/refdata.py
--rw-r--r--   0        0        0    11880 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/risk.py
--rw-r--r--   0        0        0    10351 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/scenarios.py
--rw-r--r--   0        0        0     2840 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/api/valuation.py
--rw-r--r--   0        0        0      111 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/auth.py
--rw-r--r--   0        0        0      109 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/client/__init__.py
--rw-r--r--   0        0        0     2805 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/client/auth.py
--rw-r--r--   0        0        0     4294 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/client/config.py
--rw-r--r--   0        0        0     9342 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/client/raw.py
--rw-r--r--   0        0        0      112 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/config.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/asset_search/__init__.py
--rw-r--r--   0        0        0     1533 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/asset_search/result_views.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/__init__.py
--rw-r--r--   0        0        0     1777 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/converters.py
--rw-r--r--   0        0        0     1296 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/market_data.py
--rw-r--r--   0        0        0     2885 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/option_finders.py
--rw-r--r--   0        0        0     3730 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/overrides.py
--rw-r--r--   0        0        0     1595 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/reference_data.py
--rw-r--r--   0        0        0     1909 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/request_helpers.py
--rw-r--r--   0        0        0    14120 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/table_plot.py
--rw-r--r--   0        0        0      618 2023-08-06 01:03:45.018870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/utils.py
--rw-r--r--   0        0        0     6538 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/derivatives/widget_tools.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/risk_measures/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/shared/__init__.py
--rw-r--r--   0        0        0     1042 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/shared/dropdown_select.py
--rw-r--r--   0        0        0      558 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/shared/simple_widgets.py
--rw-r--r--   0        0        0      291 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/shared/utils.py
--rw-r--r--   0        0        0     9708 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/renderers/table.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/types/__init__.py
--rw-r--r--   0        0        0     4661 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/types/common.py
--rw-r--r--   0        0        0      250 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/types/core.py
--rw-r--r--   0        0        0    10844 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/types/factors.py
--rw-r--r--   0        0        0      434 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/types/measures.py
--rw-r--r--   0        0        0     2584 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/types/model.py
--rw-r--r--   0        0        0     4861 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/types/refdata.py
--rw-r--r--   0        0        0     3504 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/types/valuation.py
--rw-r--r--   0        0        0     1926 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_sdk/widgets.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/account/__init__.py
--rw-r--r--   0        0        0     3032 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/account/core.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/ledger/__init__.py
--rw-r--r--   0        0        0      626 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/ledger/balance.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/portfolio/__init__.py
--rw-r--r--   0        0        0     7150 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/portfolio/core.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/pricing/__init__.py
--rw-r--r--   0        0        0     3297 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/pricing/core.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/pricing/derivatives/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/pricing/derivatives/options/__init__.py
--rw-r--r--   0        0        0    19105 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/pricing/derivatives/options/valuation.py
--rw-r--r--   0        0        0    10949 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/pricing/derivatives/options/volsurface.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/pricing/derivatives/rates/__init__.py
--rw-r--r--   0        0        0     8209 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/pricing/derivatives/rates/yield_curve.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/__init__.py
--rw-r--r--   0        0        0     6037 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/asset.py
--rw-r--r--   0        0        0      395 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/currency.py
--rw-r--r--   0        0        0     2603 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/derivatives.py
--rw-r--r--   0        0        0     3174 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/exposure.py
--rw-r--r--   0        0        0      874 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/futures.py
--rw-r--r--   0        0        0     2322 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/legacy.py
--rw-r--r--   0        0        0     1424 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/options.py
--rw-r--r--   0        0        0     1709 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/organization.py
--rw-r--r--   0        0        0      653 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/symbology.py
--rw-r--r--   0        0        0     2809 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/refdata/token.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/risk/__init__.py
--rw-r--r--   0        0        0     9854 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/risk/factor.py
--rw-r--r--   0        0        0    12066 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/risk/measures.py
--rw-r--r--   0        0        0     9028 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/risk/scenarios.py
--rw-r--r--   0        0        0     4689 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/risk/var.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/utils/__init__.py
--rw-r--r--   0        0        0     1939 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/utils/common.py
--rw-r--r--   0        0        0     1963 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/utils/serialization.py
--rw-r--r--   0        0        0        0 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/valuation/__init__.py
--rw-r--r--   0        0        0     3581 2023-08-06 01:03:45.022870 serenity.sdk.python-0.8.45/src/python/serenity_types/valuation/core.py
--rw-r--r--   0        0        0     2667 2023-08-06 01:04:27.632180 serenity.sdk.python-0.8.45/setup.py
--rw-r--r--   0        0        0     2374 2023-08-06 01:04:27.632636 serenity.sdk.python-0.8.45/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-08-27 18:56:36.694795 serenity.sdk.python-0.8.8/LICENSE
+-rw-r--r--   0        0        0     1140 2022-08-27 18:56:36.694795 serenity.sdk.python-0.8.8/README.md
+-rw-r--r--   0        0        0      639 2022-08-27 18:57:54.475063 serenity.sdk.python-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-08-27 18:57:54.483063 serenity.sdk.python-0.8.8/src/python/serenity_sdk/__init__.py
+-rw-r--r--   0        0        0     1163 2022-08-27 18:56:36.694795 serenity.sdk.python-0.8.8/src/python/serenity_sdk/auth.py
+-rw-r--r--   0        0        0     3891 2022-08-27 18:56:36.694795 serenity.sdk.python-0.8.8/src/python/serenity_sdk/client.py
+-rw-r--r--   0        0        0     1936 2022-08-27 18:58:01.122829 serenity.sdk.python-0.8.8/setup.py
+-rw-r--r--   0        0        0     1792 2022-08-27 18:58:01.123091 serenity.sdk.python-0.8.8/PKG-INFO
```

### Comparing `serenity.sdk.python-0.8.45/setup.py` & `serenity.sdk.python-0.8.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src/python'}
 
 packages = \
-['serenity_sdk',
- 'serenity_sdk.api',
- 'serenity_sdk.client',
- 'serenity_sdk.renderers',
- 'serenity_sdk.renderers.asset_search',
- 'serenity_sdk.renderers.derivatives',
- 'serenity_sdk.renderers.risk_measures',
- 'serenity_sdk.renderers.shared',
- 'serenity_sdk.types']
+['serenity_sdk']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['azure-identity>=1.10.0,<2.0.0',
- 'bidict>=0.22.0,<0.23.0',
- 'fire>=0.4.0,<0.5.0',
- 'humps>=0.2.2,<0.3.0',
- 'pandas>=1.4.2,<2.0.0',
- 'plotly>=5.11.0,<6.0.0',
- 'poetry-bumpversion==0.3.0',
- 'pydantic>=1.9.1,<2.0.0',
- 'requests>=2.18.4,<3.0.0',
- 'scipy>=1.7.3,<2.0.0',
- 'seaborn>=0.11.2,<0.12.0',
- 'typing-extensions==4.5.0']
+['azure-identity>=1.10.0,<2.0.0', 'fire>=0.4.0,<0.5.0']
 
 setup_kwargs = {
     'name': 'serenity.sdk.python',
-    'version': '0.8.45',
+    'version': '0.8.8',
     'description': 'Python SDK for the Serenity digital asset risk API',
-    'long_description': "## Serenity SDK - Python\n\n### Introduction\n\nThe Serenity digital asset risk platform exposes all functionality via an API -- currently REST only.\n\nAlthough it's possible to call the API with simple HTTP client code in most any modern language, there are conventions that need to be followed -- especially for authentication and authorization -- and to make it easier we have provided this lightweight SDK.\n\n### Installation\n\nInstallation for Python 3.x users is very simple using pip:\n\n```plain\npip install serenity.sdk.python\n```\n\nIf you have already installed the SDK and want to upgrade to latest:\n\n```plain\npip install -U serenity.sdk.python\n```\n\n### API documentation\n\nThe latest API documentation is always available at [ReadTheDocs](https://serenitysdkpython.readthedocs.io/en/stable/).\n\n### Maintainer setup\n\nIf you are checking in code for ```serenity.sdk.python``` you may wish to run ```setup.sh``` to install appropriate pre-commit and pre-push git hooks in your local repo. Once you run setup you will also get a Python virtual environment in ```.venv``` generated by Poetry; if using VSCode, you should select this as your IDE's virtual environment.\n\n### Learning more\n\nIf you want to learn more about the Serenity digital asset risk platform, book a demo or get in touch, you can reach out to us at [https://cloudwall.tech](https://cloudwall.tech).",
+    'long_description': "## Serenity SDK - Python\n\n### Introduction\n\nThe Serenity digital asset risk platform exposes all functionality via an API -- currently REST only.\n\nAlthough it's possible to call the API with simple HTTP client code in most any modern language, there\nare conventions that need to be followed -- especially for authentication and authorization -- and to\nmake it easier we have provided this lightweight SDK.\n\n### Installation\n\nInstallation for Python 3.x users is very simple using pip:\n\n```plain\npip install serenity.sdk.python\n```\n\n### Building locally\n\nIf you wish to run the local setup you can use the provided ```Makefile```, however this\nis primarily aimed for internal Cloudwall use; we recommend clients use pip install.\n\n```bash\n# set up a virtual environment with dependencies\nmake venv\n\n# check code\nmake link\n\n# run tests\nmake test\n\n# publish latest code to PyPi (token required)\nmake publish\n\n# clean up\nmake clean\n```\n\n### Learning more\n\nAt this time the API and its documentation are only available to members of our private beta, via\ntheir personal Serenity Developer Portal, e.g. https://developer.$client.cloudwall.network.",
     'author': 'Cloudwall Support',
     'author_email': 'support@cloudwall.tech',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4',
+    'python_requires': '>=3.7,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `serenity.sdk.python-0.8.45/PKG-INFO` & `serenity.sdk.python-0.8.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 Metadata-Version: 2.1
 Name: serenity.sdk.python
-Version: 0.8.45
+Version: 0.8.8
 Summary: Python SDK for the Serenity digital asset risk API
 License: MIT
 Author: Cloudwall Support
 Author-email: support@cloudwall.tech
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
-Requires-Dist: bidict (>=0.22.0,<0.23.0)
 Requires-Dist: fire (>=0.4.0,<0.5.0)
-Requires-Dist: humps (>=0.2.2,<0.3.0)
-Requires-Dist: pandas (>=1.4.2,<2.0.0)
-Requires-Dist: plotly (>=5.11.0,<6.0.0)
-Requires-Dist: poetry-bumpversion (==0.3.0)
-Requires-Dist: pydantic (>=1.9.1,<2.0.0)
-Requires-Dist: requests (>=2.18.4,<3.0.0)
-Requires-Dist: scipy (>=1.7.3,<2.0.0)
-Requires-Dist: seaborn (>=0.11.2,<0.12.0)
-Requires-Dist: typing-extensions (==4.5.0)
 Description-Content-Type: text/markdown
 
 ## Serenity SDK - Python
 
 ### Introduction
 
 The Serenity digital asset risk platform exposes all functionality via an API -- currently REST only.
 
-Although it's possible to call the API with simple HTTP client code in most any modern language, there are conventions that need to be followed -- especially for authentication and authorization -- and to make it easier we have provided this lightweight SDK.
+Although it's possible to call the API with simple HTTP client code in most any modern language, there
+are conventions that need to be followed -- especially for authentication and authorization -- and to
+make it easier we have provided this lightweight SDK.
 
 ### Installation
 
 Installation for Python 3.x users is very simple using pip:
 
 ```plain
 pip install serenity.sdk.python
 ```
 
-If you have already installed the SDK and want to upgrade to latest:
+### Building locally
 
-```plain
-pip install -U serenity.sdk.python
-```
+If you wish to run the local setup you can use the provided ```Makefile```, however this
+is primarily aimed for internal Cloudwall use; we recommend clients use pip install.
 
-### API documentation
+```bash
+# set up a virtual environment with dependencies
+make venv
 
-The latest API documentation is always available at [ReadTheDocs](https://serenitysdkpython.readthedocs.io/en/stable/).
+# check code
+make link
 
-### Maintainer setup
+# run tests
+make test
 
-If you are checking in code for ```serenity.sdk.python``` you may wish to run ```setup.sh``` to install appropriate pre-commit and pre-push git hooks in your local repo. Once you run setup you will also get a Python virtual environment in ```.venv``` generated by Poetry; if using VSCode, you should select this as your IDE's virtual environment.
+# publish latest code to PyPi (token required)
+make publish
+
+# clean up
+make clean
+```
 
 ### Learning more
 
-If you want to learn more about the Serenity digital asset risk platform, book a demo or get in touch, you can reach out to us at [https://cloudwall.tech](https://cloudwall.tech).
+At this time the API and its documentation are only available to members of our private beta, via
+their personal Serenity Developer Portal, e.g. https://developer.$client.cloudwall.network.
```

