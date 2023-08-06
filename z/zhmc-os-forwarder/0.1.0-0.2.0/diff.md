# Comparing `tmp/zhmc_os_forwarder-0.1.0.tar.gz` & `tmp/zhmc_os_forwarder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmc_os_forwarder-0.1.0.tar", last modified: Fri Jul 14 11:29:27 2023, max compression
+gzip compressed data, was "zhmc_os_forwarder-0.2.0.tar", last modified: Sun Aug  6 11:49:49 2023, max compression
```

## Comparing `zhmc_os_forwarder-0.1.0.tar` & `zhmc_os_forwarder-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-07-14 11:29:27.876648 zhmc_os_forwarder-0.1.0/
--rw-r--r--   0 maiera     (501) staff       (20)    10143 2023-06-30 05:20:15.000000 zhmc_os_forwarder-0.1.0/LICENSE
--rw-r--r--   0 maiera     (501) staff       (20)      429 2023-07-14 11:18:16.000000 zhmc_os_forwarder-0.1.0/MANIFEST.in
--rw-r--r--   0 maiera     (501) staff       (20)     5138 2023-07-14 11:29:27.876244 zhmc_os_forwarder-0.1.0/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)     3788 2023-07-14 07:53:56.000000 zhmc_os_forwarder-0.1.0/README.rst
--rw-r--r--   0 maiera     (501) staff       (20)     1203 2023-07-14 09:25:34.000000 zhmc_os_forwarder-0.1.0/requirements.txt
--rw-r--r--   0 maiera     (501) staff       (20)       38 2023-07-14 11:29:27.876748 zhmc_os_forwarder-0.1.0/setup.cfg
--rw-r--r--   0 maiera     (501) staff       (20)     4891 2023-07-10 15:47:33.000000 zhmc_os_forwarder-0.1.0/setup.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-07-14 11:29:27.866270 zhmc_os_forwarder-0.1.0/tests/
--rw-r--r--   0 maiera     (501) staff       (20)     1555 2023-07-13 20:17:17.000000 zhmc_os_forwarder-0.1.0/tests/test_parse_args.py
--rw-r--r--   0 maiera     (501) staff       (20)     3084 2023-07-13 20:17:17.000000 zhmc_os_forwarder-0.1.0/tests/test_parse_yaml.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-07-14 11:29:27.870798 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/
--rw-r--r--   0 maiera     (501) staff       (20)      718 2023-07-13 20:17:17.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)      927 2023-07-14 11:03:35.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/_version.py
--rw-r--r--   0 maiera     (501) staff       (20)     4570 2023-07-14 07:53:56.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/forwarded_lpars.py
--rw-r--r--   0 maiera     (501) staff       (20)     5161 2023-07-14 07:53:56.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/forwarder_config.py
--rw-r--r--   0 maiera     (501) staff       (20)    13574 2023-07-14 07:53:56.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/forwarder_server.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-07-14 11:29:27.875798 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/schemas/
--rw-r--r--   0 maiera     (501) staff       (20)     3315 2023-07-14 07:53:56.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/schemas/config_schema.yaml
--rw-r--r--   0 maiera     (501) staff       (20)    17538 2023-07-13 20:17:17.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/utils.py
--rwxr-xr-x   0 maiera     (501) staff       (20)     7334 2023-07-13 20:17:17.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/zhmc_os_forwarder.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-07-14 11:29:27.875183 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/
--rw-r--r--   0 maiera     (501) staff       (20)     5138 2023-07-14 11:29:27.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)      674 2023-07-14 11:29:27.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/SOURCES.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-07-14 11:29:27.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/dependency_links.txt
--rw-r--r--   0 maiera     (501) staff       (20)       79 2023-07-14 11:29:27.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/entry_points.txt
--rw-r--r--   0 maiera     (501) staff       (20)      301 2023-07-14 11:29:27.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/requires.txt
--rw-r--r--   0 maiera     (501) staff       (20)       18 2023-07-14 11:29:27.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/top_level.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-07-14 11:29:27.000000 zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:49:49.207854 zhmc_os_forwarder-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-06 11:49:36.000000 zhmc_os_forwarder-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-06 11:49:49.203854 zhmc_os_forwarder-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:49:49.207854 zhmc_os_forwarder-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:49:49.195854 zhmc_os_forwarder-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/tests/test_parse_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/tests/test_parse_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:49:49.199854 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/forwarded_lpars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/forwarder_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/forwarder_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:49:49.203854 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/schemas/config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7791 2023-08-06 11:48:59.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/zhmc_os_forwarder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:49:49.203854 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-06 11:49:49.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-06 11:49:49.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:49:49.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-06 11:49:49.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-06 11:49:49.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 11:49:49.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:49:48.000000 zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/zip-safe
```

### Comparing `zhmc_os_forwarder-0.1.0/LICENSE` & `zhmc_os_forwarder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmc_os_forwarder-0.1.0/PKG-INFO` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zhmc_os_forwarder
-Version: 0.1.0
+Name: zhmc-os-forwarder
+Version: 0.2.0
 Summary: IBM Z HMC OS Message Forwarder
 Home-page: https://github.com/zhmcclient/zhmc-os-forwarder
 Author: Andreas Maier
 Author-email: maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
@@ -60,72 +60,81 @@
 
 .. image:: https://coveralls.io/repos/github/zhmcclient/zhmc-os-forwarder/badge.svg?branch=master
     :target: https://coveralls.io/github/zhmcclient/zhmc-os-forwarder?branch=master
     :alt: Test coverage (master)
 
 The **IBM Z HMC OS Message Forwarder** connects to the console of operating
 systems running in LPARs on Z systems and forwards the messages written by the
-operating system to its console to a remote syslog server.
+operating systems in the LPARs to remote syslog servers.
 
-The Z systems can be in classic or DPM operatonal mode.
+The Z systems can be in classic or DPM operational mode.
 
-.. # The forwarder attempts to stay up as much as possible, for example it performs
-.. # automatic session renewals with the HMC if the logon session expires, and it
-.. # survives HMC reboots and automatically picks up message forwarding at the
-.. # right message sequence number once the HMC come back up.
-
-.. _IBM Z: https://www.ibm.com/it-infrastructure/z
+The forwarder attempts to stay up as much as possible, for example it performs
+automatic session renewals with the HMC if the logon session expires, and it
+survives HMC reboots and automatically resumes forwarding again once
+the HMC come back up, without loosing or duplicating any messages.
 
 Documentation
 -------------
 
-* `Documentation`_ (not yet)
-* `Change log`_ (not yet)
+* `Documentation`_
+* `Change log`_
 
 .. _Documentation: https://zhmc-os-forwarder.readthedocs.io/en/stable/
 .. _Change log: https://zhmc-os-forwarder.readthedocs.io/en/stable/changes.html
 
+Supported environments
+----------------------
+
+* Operating systems: Linux, macOS, Windows
+* Python versions: 3.5 and higher
+* HMC versions: 2.11.1 and higher
+
 Quickstart
 ----------
 
 * Install the forwarder and all of its Python dependencies as follows:
 
   .. code-block:: bash
 
       $ pip install zhmc-os-forwarder
 
-* Provide a config file for use by the forwarder.
+* Provide a *config file* for use by the forwarder.
 
   The config file tells the forwarder which HMC to use, and for which CPCs
-  and partitions it should forward to which syslog servers.
+  and LPARs it should forward to which syslog servers.
 
-  Download the `example config file`_ as ``config.yaml`` and edit that copy
-  according to your environment.
+  Download the `Example forwarder config file`_ and edit that copy according
+  to your needs.
 
-.. # For details, see `forwarder config file`_.
+  For details, see `Forwarder config file`_.
 
-.. _forwarder config file: https://zhmc-os-forwarder.readthedocs.io/en/stable/usage.html#hmc-credentials-file
-.. _example config file: examples/config_example.yaml
+.. _Example forwarder config file: examples/config_example.yaml
+.. _Forwarder config file: https://zhmc-os-forwarder.readthedocs.io/en/stable/usage.html#forwarder-config-file
 
 * Run the forwarder as follows:
 
   .. code-block:: bash
 
       $ zhmc_os_forwarder -c config.yaml
+      zhmc_os_forwarder version: 0.2.0
+      zhmcclient version: 1.10.0
+      Verbosity level: 0
+      Opening session with HMC 10.11.12.13 (user: johndoe@us.ibm.com, certificate validation: False)
+      Forwarder is up and running (Press Ctrl-C to shut down)
 
 Limitations
 -----------
 
 At this point, the forwarder has several limitations. All of them are intended
 to be resolved in future releases.
 
 * The forwarder does not recover from HMC restart or connection loss
 * Restarting the forwarder will send again all OS messages the HMC has buffered
-* New and deleted partitions in DPM mode are not automatically detected.
-* No documentation
+* New and deleted LPARs in DPM mode are not automatically detected.
 
 Reporting issues
 ----------------
 
 If you encounter a problem, please report it as an `issue on GitHub`_.
 
 .. _issue on GitHub: https://github.com/zhmcclient/zhmc-os-forwarder/issues
```

### Comparing `zhmc_os_forwarder-0.1.0/README.rst` & `zhmc_os_forwarder-0.2.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -29,72 +29,81 @@
 
 .. image:: https://coveralls.io/repos/github/zhmcclient/zhmc-os-forwarder/badge.svg?branch=master
     :target: https://coveralls.io/github/zhmcclient/zhmc-os-forwarder?branch=master
     :alt: Test coverage (master)
 
 The **IBM Z HMC OS Message Forwarder** connects to the console of operating
 systems running in LPARs on Z systems and forwards the messages written by the
-operating system to its console to a remote syslog server.
+operating systems in the LPARs to remote syslog servers.
 
-The Z systems can be in classic or DPM operatonal mode.
+The Z systems can be in classic or DPM operational mode.
 
-.. # The forwarder attempts to stay up as much as possible, for example it performs
-.. # automatic session renewals with the HMC if the logon session expires, and it
-.. # survives HMC reboots and automatically picks up message forwarding at the
-.. # right message sequence number once the HMC come back up.
-
-.. _IBM Z: https://www.ibm.com/it-infrastructure/z
+The forwarder attempts to stay up as much as possible, for example it performs
+automatic session renewals with the HMC if the logon session expires, and it
+survives HMC reboots and automatically resumes forwarding again once
+the HMC come back up, without loosing or duplicating any messages.
 
 Documentation
 -------------
 
-* `Documentation`_ (not yet)
-* `Change log`_ (not yet)
+* `Documentation`_
+* `Change log`_
 
 .. _Documentation: https://zhmc-os-forwarder.readthedocs.io/en/stable/
 .. _Change log: https://zhmc-os-forwarder.readthedocs.io/en/stable/changes.html
 
+Supported environments
+----------------------
+
+* Operating systems: Linux, macOS, Windows
+* Python versions: 3.5 and higher
+* HMC versions: 2.11.1 and higher
+
 Quickstart
 ----------
 
 * Install the forwarder and all of its Python dependencies as follows:
 
   .. code-block:: bash
 
       $ pip install zhmc-os-forwarder
 
-* Provide a config file for use by the forwarder.
+* Provide a *config file* for use by the forwarder.
 
   The config file tells the forwarder which HMC to use, and for which CPCs
-  and partitions it should forward to which syslog servers.
+  and LPARs it should forward to which syslog servers.
 
-  Download the `example config file`_ as ``config.yaml`` and edit that copy
-  according to your environment.
+  Download the `Example forwarder config file`_ and edit that copy according
+  to your needs.
 
-.. # For details, see `forwarder config file`_.
+  For details, see `Forwarder config file`_.
 
-.. _forwarder config file: https://zhmc-os-forwarder.readthedocs.io/en/stable/usage.html#hmc-credentials-file
-.. _example config file: examples/config_example.yaml
+.. _Example forwarder config file: examples/config_example.yaml
+.. _Forwarder config file: https://zhmc-os-forwarder.readthedocs.io/en/stable/usage.html#forwarder-config-file
 
 * Run the forwarder as follows:
 
   .. code-block:: bash
 
       $ zhmc_os_forwarder -c config.yaml
+      zhmc_os_forwarder version: 0.2.0
+      zhmcclient version: 1.10.0
+      Verbosity level: 0
+      Opening session with HMC 10.11.12.13 (user: johndoe@us.ibm.com, certificate validation: False)
+      Forwarder is up and running (Press Ctrl-C to shut down)
 
 Limitations
 -----------
 
 At this point, the forwarder has several limitations. All of them are intended
 to be resolved in future releases.
 
 * The forwarder does not recover from HMC restart or connection loss
 * Restarting the forwarder will send again all OS messages the HMC has buffered
-* New and deleted partitions in DPM mode are not automatically detected.
-* No documentation
+* New and deleted LPARs in DPM mode are not automatically detected.
 
 Reporting issues
 ----------------
 
 If you encounter a problem, please report it as an `issue on GitHub`_.
 
 .. _issue on GitHub: https://github.com/zhmcclient/zhmc-os-forwarder/issues
```

### Comparing `zhmc_os_forwarder-0.1.0/requirements.txt` & `zhmc_os_forwarder-0.2.0/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance.
 #
 
 # Direct dependencies for runtime (must be consistent with minimum-constraints.txt)
 
 # zhmcclient @ git+https://github.com/zhmcclient/python-zhmcclient.git@master
-zhmcclient>=1.9.0
+zhmcclient>=1.10.0
 
 urllib3>=1.25.9; python_version <= '3.9'
 urllib3>=1.26.5; python_version >= '3.10'
 jsonschema>=3.2.0
 
-# PyYAML pulled in by zhmcclient examples
-# PyYAML 5.3.1 addressed issue 38100 reported by safety
-# PyYAML is also used by dparse and python-coveralls
-# PyYAML 5.4 has removed support for py35
-PyYAML>=5.3.1; python_version == '3.5'
-PyYAML>=5.4; python_version >= '3.6'
+# PyYAML pulled in by zhmcclient, dparse, python-coveralls
+# PyYAML 5.3 has wheel archives for Python 2.7, 3.5 - 3.9
+# PyYAML 5.4 has wheel archives for Python 2.7, 3.6 - 3.9
+# PyYAML 6.0 has wheel archives for Python 3.6 - 3.11
+# PyYAML 5.4 and 6.0.0 fails install since Cython 3 was released, see issue
+#   https://github.com/yaml/pyyaml/issues/724.
+PyYAML>=5.3.1; python_version <= '3.5'
+PyYAML>=5.3.1,!=5.4.0,!=5.4.1; python_version >= '3.6' and python_version <= '3.11'
+PyYAML>=5.3.1,!=5.4.0,!=5.4.1,!=6.0.0; python_version >= '3.12'
+
 
 # Indirect dependencies for runtime (must be consistent with minimum-constraints.txt)
 
 # pyrsistent is pulled in by jsonschema.
 # Before its version 0.17.0, pyrsistent did not or not correctly declare its
 # required Python versions in the package metadata.
 # pyrsistent 0.15.0 fixes import errors on Python>=3.10, but only 0.18.1 has
```

### Comparing `zhmc_os_forwarder-0.1.0/setup.py` & `zhmc_os_forwarder-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `zhmc_os_forwarder-0.1.0/tests/test_parse_args.py` & `zhmc_os_forwarder-0.2.0/tests/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `zhmc_os_forwarder-0.1.0/tests/test_parse_yaml.py` & `zhmc_os_forwarder-0.2.0/tests/test_parse_yaml.py`

 * *Files identical despite different names*

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/__init__.py` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/_version.py` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/forwarded_lpars.py` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/forwarded_lpars.py`

 * *Files identical despite different names*

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/forwarder_config.py` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/forwarder_config.py`

 * *Files identical despite different names*

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/forwarder_server.py` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/forwarder_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,24 +41,26 @@
           config_data (dict): Content of forwarder config file.
           config_filename (string): Path name of forwarder config file.
         """
         self.config_data = config_data
         self.config_filename = config_filename
 
         self.thread = Thread(target=self.run)  # forwarder thread
+        self.thread_started = False
         self.stop_event = Event()  # Set event to stop forwarder thread
 
         self.session = None  # zhmcclient.Session with the HMC
 
         self.all_cpcs = None  # List of all managed CPCs as zhmcclient.Cpc
         self.all_lpars = None  # List of all partitions/LPARs as zhmcclient obj
 
         self.forwarded_lpars = None  # ForwardedLpars object
 
         self.receiver = None  # NotificationReceiver
+        self.num_subscriptions = None
 
     def startup(self):
         """
         Set up the forwarder server and start the forwarder thread.
         """
 
         hmc_data = self.config_data['hmc']
@@ -114,14 +116,15 @@
 
         self.receiver = zhmcclient.NotificationReceiver(
             [],  # self.session.object_topic to get notifications to ignore
             hmc_data['host'],
             hmc_data['userid'],
             hmc_data['password'])
 
+        self.num_subscriptions = 0
         logger_id = 0  # ID number used in Python logger name
         for lpar_info in self.forwarded_lpars.forwarded_lpar_infos.values():
             lpar = lpar_info.lpar
             cpc = lpar.manager.parent
 
             logprint(logging.INFO, PRINT_VV,
                      "Opening OS message channel for LPAR {p!r} on CPC {c!r}".
@@ -151,37 +154,46 @@
                     if os_topic is None:
                         raise RuntimeError(
                             "An OS message notification topic for LPAR {p!r} "
                             "on CPC {c!r} supposedly exists, but cannot be "
                             "found in the existing topics for this session: "
                             "{t}".
                             format(p=lpar.name, c=cpc.name, t=topic_dicts))
-                if exc.http_status == 409 and exc.reason == 332:
+                elif exc.http_status == 409 and exc.reason == 332:
                     # The OS does not support OS messages.
                     logprint(logging.WARNING, PRINT_ALWAYS,
                              "Warning: The OS in LPAR {p!r} on CPC {c!r} does "
                              "not support OS messages - ignoring the LPAR".
                              format(p=lpar.name, c=cpc.name))
+                    os_topic = None
                 else:
                     raise
-            self.receiver.subscribe(os_topic)
-            lpar_info.topic = os_topic
+
+            if os_topic:
+                logprint(logging.INFO, PRINT_VV,
+                         "Subscribing for OS message notifications for LPAR "
+                         "{p!r} on CPC {c!r} (topic: {t})".
+                         format(p=lpar.name, c=cpc.name, t=os_topic))
+                self.receiver.subscribe(os_topic)
+                lpar_info.topic = os_topic
+                self.num_subscriptions += 1
 
             # Prepare sending to syslogs by creating Python loggers
             for syslog in self.forwarded_lpars.get_syslogs(lpar):
                 try:
                     logger = self._create_logger(syslog, logger_id)
                 except ConnectionError as exc:
                     logprint(logging.WARNING, PRINT_ALWAYS,
                              "Warning: Skipping syslog server: {}".format(exc))
                     continue
                 logger_id += 1
                 syslog.logger = logger
 
         self._start()
+        self.thread_started = True
 
     @staticmethod
     def _create_logger(syslog, logger_id):
         facility_code = logging.handlers.SysLogHandler.facility_names[
             syslog.facility]
         if syslog.port_type == 'tcp':
             # Newer syslog protocols, e.g. rsyslog
@@ -190,14 +202,15 @@
             assert syslog.port_type == 'udp'
             # Older syslog protocols, e.g. BSD
             socktype = socket.SOCK_DGRAM
         try:
             handler = logging.handlers.SysLogHandler(
                 (syslog.host, syslog.port), facility_code,
                 socktype=socktype)
+        # pylint: disable=broad-exception-caught
         except Exception as exc:
             raise ConnectionError(
                 "Cannot create log handler for syslog server at "
                 "{host}, port {port}/{port_type}: {msg}".
                 format(host=syslog.host, port=syslog.port,
                        port_type=syslog.port_type, msg=str(exc)))
         handler.setFormatter(logging.Formatter('%(message)s'))
@@ -208,60 +221,80 @@
         return logger
 
     def shutdown(self):
         """
         Stop the forwarder thread and clean up the forwarder server.
         """
 
-        try:
-
+        if self.forwarded_lpars:
             for lpar_info in self.forwarded_lpars.forwarded_lpar_infos.values():
                 lpar = lpar_info.lpar
                 cpc = lpar.manager.parent
 
-                logprint(logging.INFO, PRINT_VV,
-                         "Unsubscribing OS message channel for LPAR {p!r} on "
-                         "CPC {c!r}".
-                         format(p=lpar.name, c=cpc.name))
-                self.receiver.unsubscribe(lpar_info.topic)
+                if lpar_info.topic:
+                    logprint(logging.INFO, PRINT_VV,
+                             "Unsubscribing OS message channel for LPAR {p!r} "
+                             "on CPC {c!r} (topic: {t})".
+                             format(p=lpar.name, c=cpc.name, t=lpar_info.topic))
+                    try:
+                        self.receiver.unsubscribe(lpar_info.topic)
+                    except zhmcclient.Error as exc:
+                        logprint(logging.ERROR, PRINT_ALWAYS,
+                                 "Error unsubscribing OS message channel for "
+                                 "LPAR {p!r} on CPC {c!r} (topic: {t}): {m}".
+                                 format(p=lpar.name, c=cpc.name,
+                                        t=lpar_info.topic, m=exc))
 
-            logprint(logging.INFO, PRINT_ALWAYS,
-                     "Closing notification receiver")
-            self.receiver.close()
+        if self.receiver:
+            try:
+                logprint(logging.INFO, PRINT_ALWAYS,
+                         "Closing notification receiver")
+                self.receiver.close()
+            except zhmcclient.Error as exc:
+                logprint(logging.ERROR, PRINT_ALWAYS,
+                         "Error closing notification receiver: {m}".
+                         format(m=exc))
 
-            if self.thread:
+        if self.thread_started:
+            try:
                 logprint(logging.INFO, PRINT_ALWAYS,
                          "Stopping forwarder thread")
                 self._stop()
+            # pylint: disable=broad-exception-caught
+            except Exception as exc:
+                logprint(logging.ERROR, PRINT_ALWAYS,
+                         "Error stopping forwarder thread: {m}".
+                         format(m=exc))
+            self.thread_started = False
+
+        # logprint(logging.INFO, PRINT_ALWAYS,
+        #          "Cleaning up partition notifications on HMC")
+        # for lpar_tuple in self.forwarded_lpars.values():
+        #     lpar = lpar_tuple[0]
+        #     try:
+        #         lpar.disable_auto_update()
+        #     except zhmcclient.HTTPError as exc:
+        #         if exc.http_status == 403:
+        #             # The session does not exist anymore
+        #             pass
 
-            # logprint(logging.INFO, PRINT_ALWAYS,
-            #          "Cleaning up partition notifications on HMC")
-            # for lpar_tuple in self.forwarded_lpars.values():
-            #     lpar = lpar_tuple[0]
-            #     try:
-            #         lpar.disable_auto_update()
-            #     except zhmcclient.HTTPError as exc:
-            #         if exc.http_status == 403:
-            #             # The session does not exist anymore
-            #             pass
-
-            if self.session:
-                logprint(logging.INFO, PRINT_ALWAYS,
-                         "Closing session with HMC")
-                try:
-                    self.session.logoff()
-                except zhmcclient.HTTPError as exc:
-                    if exc.http_status == 403:
-                        # The session does not exist anymore
-                        pass
-                self.session = None
-
-        except zhmcclient.Error as exc:
-            logprint(logging.ERROR, PRINT_ALWAYS,
-                     "Error when cleaning up: {}".format(exc))
+        if self.session:
+            logprint(logging.INFO, PRINT_ALWAYS,
+                     "Closing session with HMC")
+            try:
+                self.session.logoff()
+            except zhmcclient.HTTPError as exc:
+                if exc.http_status == 403:
+                    # The session does not exist anymore
+                    pass
+                else:
+                    logprint(logging.ERROR, PRINT_ALWAYS,
+                             "Error closing session with HMC: {m}".
+                             format(m=exc))
+            self.session = None
 
     def _start(self):
         """
         Start the forwarder thread.
         """
         self.stop_event.clear()
         self.thread.start()
```

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/schemas/config_schema.yaml` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/schemas/config_schema.yaml`

 * *Files identical despite different names*

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/utils.py` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 DEFAULT_CONFIG_FILE = '/etc/zhmc-os-forwarder/config.yaml'
 
 
 #
 # Retry
 #
 
-# Sleep time in seconds when retrying metrics retrieval
+# Sleep time in seconds when retrying HMC connections
 RETRY_SLEEP_TIME = 10
 
 # Retry / timeout configuration for zhmcclient (used at the socket level)
 RETRY_TIMEOUT_CONFIG = zhmcclient.RetryTimeoutConfig(
     connect_timeout=10,
     connect_retries=2,
     read_timeout=300,
```

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder/zhmc_os_forwarder.py` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder/zhmc_os_forwarder.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,15 +167,26 @@
         logprint(logging.INFO, PRINT_V,
                  "Timeout/retry configuration: "
                  "connect: {r.connect_timeout} sec / {r.connect_retries} "
                  "retries, read: {r.read_timeout} sec / {r.read_retries} "
                  "retries.".format(r=RETRY_TIMEOUT_CONFIG))
 
         forwarder_server = ForwarderServer(config_data, config_filename)
-        forwarder_server.startup()
+        try:
+            forwarder_server.startup()
+        except zhmcclient.Error as exc:
+            new_exc = ImproperExit(
+                "{}: {}".format(exc.__class__.__name__, exc))
+            new_exc.__cause__ = None  # pylint: disable=invalid-name
+            raise new_exc
+
+        logprint(logging.INFO, PRINT_V,
+                 "Current number of subscriptions for OS message "
+                 "notifications: {}".
+                 format(forwarder_server.num_subscriptions))
 
         logprint(logging.INFO, PRINT_ALWAYS,
                  "Forwarder is up and running (Press Ctrl-C to shut down)")
 
         while True:
             try:
                 time.sleep(1)
```

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/PKG-INFO` & `zhmc_os_forwarder-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zhmc-os-forwarder
-Version: 0.1.0
+Name: zhmc_os_forwarder
+Version: 0.2.0
 Summary: IBM Z HMC OS Message Forwarder
 Home-page: https://github.com/zhmcclient/zhmc-os-forwarder
 Author: Andreas Maier
 Author-email: maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
@@ -60,72 +60,81 @@
 
 .. image:: https://coveralls.io/repos/github/zhmcclient/zhmc-os-forwarder/badge.svg?branch=master
     :target: https://coveralls.io/github/zhmcclient/zhmc-os-forwarder?branch=master
     :alt: Test coverage (master)
 
 The **IBM Z HMC OS Message Forwarder** connects to the console of operating
 systems running in LPARs on Z systems and forwards the messages written by the
-operating system to its console to a remote syslog server.
+operating systems in the LPARs to remote syslog servers.
 
-The Z systems can be in classic or DPM operatonal mode.
+The Z systems can be in classic or DPM operational mode.
 
-.. # The forwarder attempts to stay up as much as possible, for example it performs
-.. # automatic session renewals with the HMC if the logon session expires, and it
-.. # survives HMC reboots and automatically picks up message forwarding at the
-.. # right message sequence number once the HMC come back up.
-
-.. _IBM Z: https://www.ibm.com/it-infrastructure/z
+The forwarder attempts to stay up as much as possible, for example it performs
+automatic session renewals with the HMC if the logon session expires, and it
+survives HMC reboots and automatically resumes forwarding again once
+the HMC come back up, without loosing or duplicating any messages.
 
 Documentation
 -------------
 
-* `Documentation`_ (not yet)
-* `Change log`_ (not yet)
+* `Documentation`_
+* `Change log`_
 
 .. _Documentation: https://zhmc-os-forwarder.readthedocs.io/en/stable/
 .. _Change log: https://zhmc-os-forwarder.readthedocs.io/en/stable/changes.html
 
+Supported environments
+----------------------
+
+* Operating systems: Linux, macOS, Windows
+* Python versions: 3.5 and higher
+* HMC versions: 2.11.1 and higher
+
 Quickstart
 ----------
 
 * Install the forwarder and all of its Python dependencies as follows:
 
   .. code-block:: bash
 
       $ pip install zhmc-os-forwarder
 
-* Provide a config file for use by the forwarder.
+* Provide a *config file* for use by the forwarder.
 
   The config file tells the forwarder which HMC to use, and for which CPCs
-  and partitions it should forward to which syslog servers.
+  and LPARs it should forward to which syslog servers.
 
-  Download the `example config file`_ as ``config.yaml`` and edit that copy
-  according to your environment.
+  Download the `Example forwarder config file`_ and edit that copy according
+  to your needs.
 
-.. # For details, see `forwarder config file`_.
+  For details, see `Forwarder config file`_.
 
-.. _forwarder config file: https://zhmc-os-forwarder.readthedocs.io/en/stable/usage.html#hmc-credentials-file
-.. _example config file: examples/config_example.yaml
+.. _Example forwarder config file: examples/config_example.yaml
+.. _Forwarder config file: https://zhmc-os-forwarder.readthedocs.io/en/stable/usage.html#forwarder-config-file
 
 * Run the forwarder as follows:
 
   .. code-block:: bash
 
       $ zhmc_os_forwarder -c config.yaml
+      zhmc_os_forwarder version: 0.2.0
+      zhmcclient version: 1.10.0
+      Verbosity level: 0
+      Opening session with HMC 10.11.12.13 (user: johndoe@us.ibm.com, certificate validation: False)
+      Forwarder is up and running (Press Ctrl-C to shut down)
 
 Limitations
 -----------
 
 At this point, the forwarder has several limitations. All of them are intended
 to be resolved in future releases.
 
 * The forwarder does not recover from HMC restart or connection loss
 * Restarting the forwarder will send again all OS messages the HMC has buffered
-* New and deleted partitions in DPM mode are not automatically detected.
-* No documentation
+* New and deleted LPARs in DPM mode are not automatically detected.
 
 Reporting issues
 ----------------
 
 If you encounter a problem, please report it as an `issue on GitHub`_.
 
 .. _issue on GitHub: https://github.com/zhmcclient/zhmc-os-forwarder/issues
```

### Comparing `zhmc_os_forwarder-0.1.0/zhmc_os_forwarder.egg-info/SOURCES.txt` & `zhmc_os_forwarder-0.2.0/zhmc_os_forwarder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

