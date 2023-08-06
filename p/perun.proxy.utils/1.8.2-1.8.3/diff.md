# Comparing `tmp/perun.proxy.utils-1.8.2.tar.gz` & `tmp/perun.proxy.utils-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxy.utils-1.8.2.tar", last modified: Tue Jul 18 09:20:15 2023, max compression
+gzip compressed data, was "perun.proxy.utils-1.8.3.tar", last modified: Sun Aug  6 20:30:10 2023, max compression
```

## Comparing `perun.proxy.utils-1.8.2.tar` & `perun.proxy.utils-1.8.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:15.199113 perun.proxy.utils-1.8.2/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4053 2023-07-18 09:20:15.199113 perun.proxy.utils-1.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2899 2023-07-18 09:07:26.000000 perun.proxy.utils-1.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:15.107111 perun.proxy.utils-1.8.2/perun/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:15.107111 perun.proxy.utils-1.8.2/perun/proxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:15.155112 perun.proxy.utils-1.8.2/perun/proxy/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/metadata_expiration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:15.195113 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_custom_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1414 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_dockers.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_exabgp_propagation.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_ldap.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_ldap_syncrepl.py
--rw-rw-rw-   0 root         (0) root         (0)    72117 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_mongodb.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_nginx.py
--rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_rpc_status.py
--rwxrwxrwx   0 root         (0) root         (0)    18784 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_saml.py
--rw-rw-rw-   0 root         (0) root         (0)     3199 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_user_logins.py
--rwxrwxrwx   0 root         (0) root         (0)      945 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/webserver_availability.py
--rwxrwxrwx   0 root         (0) root         (0)     2652 2023-07-11 11:16:08.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/print_docker_versions.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-07-18 09:07:26.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/run_probes.py
--rw-rw-rw-   0 root         (0) root         (0)     3215 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/run_version_script.py
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/separate_oidc_logs.py
--rwxrwxrwx   0 root         (0) root         (0)     2531 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.2/perun/proxy/utils/separate_ssp_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:15.111111 perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4053 2023-07-18 09:20:14.000000 perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1080 2023-07-18 09:20:15.000000 perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 09:20:14.000000 perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1121 2023-07-18 09:20:14.000000 perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-18 09:20:14.000000 perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-18 09:20:14.000000 perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-07-18 09:20:15.199113 perun.proxy.utils-1.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-07-18 09:07:26.000000 perun.proxy.utils-1.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:30:10.082268 perun.proxy.utils-1.8.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4053 2023-08-06 20:30:10.082268 perun.proxy.utils-1.8.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2899 2023-08-06 20:24:01.000000 perun.proxy.utils-1.8.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:30:10.054268 perun.proxy.utils-1.8.3/perun/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:30:10.054268 perun.proxy.utils-1.8.3/perun/proxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:30:10.078268 perun.proxy.utils-1.8.3/perun/proxy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-06 20:28:39.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/metadata_expiration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:30:10.082268 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-06 20:28:39.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_custom_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_dockers.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_exabgp_propagation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_ldap.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-10 14:19:41.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_ldap_syncrepl.py
+-rw-rw-rw-   0 root         (0) root         (0)    72117 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_nginx.py
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_rpc_status.py
+-rwxrwxrwx   0 root         (0) root         (0)    18784 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_saml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_user_logins.py
+-rwxrwxrwx   0 root         (0) root         (0)      945 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/webserver_availability.py
+-rwxrwxrwx   0 root         (0) root         (0)     2652 2023-07-11 11:16:08.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/print_docker_versions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1805 2023-08-06 19:24:20.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/run_probes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3215 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/run_version_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/separate_oidc_logs.py
+-rwxrwxrwx   0 root         (0) root         (0)     2531 2023-07-11 10:59:57.000000 perun.proxy.utils-1.8.3/perun/proxy/utils/separate_ssp_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:30:10.078268 perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4053 2023-08-06 20:30:09.000000 perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-08-06 20:30:10.000000 perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:30:09.000000 perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-08-06 20:30:09.000000 perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      182 2023-08-06 20:30:09.000000 perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-08-06 20:30:09.000000 perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-08-06 20:30:10.082268 perun.proxy.utils-1.8.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-08-06 20:24:01.000000 perun.proxy.utils-1.8.3/setup.py
```

### Comparing `perun.proxy.utils-1.8.2/LICENSE` & `perun.proxy.utils-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/PKG-INFO` & `perun.proxy.utils-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxy.utils
-Version: 1.8.2
+Version: 1.8.3
 Summary: Module with utilities and monitoring probes
 Home-page: https://gitlab.ics.muni.cz/perun-proxy-aai/proxyidp-scripts.git
 License: UNKNOWN
 Description: # Perun proxy utils
         
         ## Scripts
```

### Comparing `perun.proxy.utils-1.8.2/README.md` & `perun.proxy.utils-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/metadata_expiration.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/metadata_expiration.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_custom_command.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_custom_command.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_dockers.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_dockers.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_exabgp_propagation.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_exabgp_propagation.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_ldap.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_ldap.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_mongodb.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_mongodb.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_rpc_status.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_rpc_status.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_saml.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_saml.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/check_user_logins.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/check_user_logins.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/nagios/webserver_availability.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/nagios/webserver_availability.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/print_docker_versions.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/print_docker_versions.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/run_probes.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/run_probes.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,24 +38,25 @@
     if not config:
         return
 
     for _, options in config.items():
         module = options["module"]
         for name, args in options.get("runs").items():
             command = ["python3", "-m", module]
-            for arg_name, arg_val in args.items():
-                if len(arg_name) == 1:
-                    arg_name = "-" + arg_name
-                else:
-                    arg_name = "--" + arg_name
-                if arg_val is True:
-                    arg_val = "true"
-                elif arg_val is False:
-                    arg_val = "false"
-                command.append(arg_name)
-                if arg_val is not None:
-                    command.append(str(arg_val))
+            if args is not None:
+                for arg_name, arg_val in args.items():
+                    if len(arg_name) == 1:
+                        arg_name = "-" + arg_name
+                    else:
+                        arg_name = "--" + arg_name
+                    if arg_val is True:
+                        arg_val = "true"
+                    elif arg_val is False:
+                        arg_val = "false"
+                    command.append(arg_name)
+                    if arg_val is not None:
+                        command.append(str(arg_val))
             Thread(target=run_probe, args=[name, command]).start()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/run_version_script.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/run_version_script.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/separate_oidc_logs.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/separate_oidc_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun/proxy/utils/separate_ssp_logs.py` & `perun.proxy.utils-1.8.3/perun/proxy/utils/separate_ssp_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/PKG-INFO` & `perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxy.utils
-Version: 1.8.2
+Version: 1.8.3
 Summary: Module with utilities and monitoring probes
 Home-page: https://gitlab.ics.muni.cz/perun-proxy-aai/proxyidp-scripts.git
 License: UNKNOWN
 Description: # Perun proxy utils
         
         ## Scripts
```

### Comparing `perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/SOURCES.txt` & `perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/perun.proxy.utils.egg-info/entry_points.txt` & `perun.proxy.utils-1.8.3/perun.proxy.utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.8.2/setup.py` & `perun.proxy.utils-1.8.3/setup.py`

 * *Files identical despite different names*

