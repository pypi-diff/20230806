# Comparing `tmp/lnctApi-0.0.1.tar.gz` & `tmp/lnctApi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnctApi-0.0.1.tar", last modified: Sun Aug  6 09:55:58 2023, max compression
+gzip compressed data, was "lnctApi-0.0.2.tar", last modified: Sun Aug  6 12:39:08 2023, max compression
```

## Comparing `lnctApi-0.0.1.tar` & `lnctApi-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 09:55:58.135613 lnctApi-0.0.1/
--rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 lnctApi-0.0.1/LICENSE.txt
--rw-r--r--   0 cro        (501) staff       (20)      891 2023-08-06 09:55:58.135491 lnctApi-0.0.1/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      336 2023-08-05 18:56:59.000000 lnctApi-0.0.1/README.md
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 09:55:58.134485 lnctApi-0.0.1/lnctApi/
--rw-r--r--   0 cro        (501) staff       (20)       32 2023-08-04 19:28:06.000000 lnctApi-0.0.1/lnctApi/__init__.py
--rw-r--r--   0 cro        (501) staff       (20)    23081 2023-08-06 08:49:15.000000 lnctApi-0.0.1/lnctApi/accsoft_api.py
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 09:55:58.135313 lnctApi-0.0.1/lnctApi.egg-info/
--rw-r--r--   0 cro        (501) staff       (20)      891 2023-08-06 09:55:58.000000 lnctApi-0.0.1/lnctApi.egg-info/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      227 2023-08-06 09:55:58.000000 lnctApi-0.0.1/lnctApi.egg-info/SOURCES.txt
--rw-r--r--   0 cro        (501) staff       (20)        1 2023-08-06 09:55:58.000000 lnctApi-0.0.1/lnctApi.egg-info/dependency_links.txt
--rw-r--r--   0 cro        (501) staff       (20)       37 2023-08-06 09:55:58.000000 lnctApi-0.0.1/lnctApi.egg-info/requires.txt
--rw-r--r--   0 cro        (501) staff       (20)        8 2023-08-06 09:55:58.000000 lnctApi-0.0.1/lnctApi.egg-info/top_level.txt
--rw-r--r--   0 cro        (501) staff       (20)       38 2023-08-06 09:55:58.135660 lnctApi-0.0.1/setup.cfg
--rw-r--r--   0 cro        (501) staff       (20)      868 2023-08-06 09:55:28.000000 lnctApi-0.0.1/setup.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 12:39:08.295482 lnctApi-0.0.2/
+-rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 lnctApi-0.0.2/LICENSE.txt
+-rw-r--r--   0 cro        (501) staff       (20)      891 2023-08-06 12:39:08.295374 lnctApi-0.0.2/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      336 2023-08-05 18:56:59.000000 lnctApi-0.0.2/README.md
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 12:39:08.294558 lnctApi-0.0.2/lnctApi/
+-rw-r--r--   0 cro        (501) staff       (20)       32 2023-08-04 19:28:06.000000 lnctApi-0.0.2/lnctApi/__init__.py
+-rw-r--r--   0 cro        (501) staff       (20)    23093 2023-08-06 12:33:58.000000 lnctApi-0.0.2/lnctApi/accsoft_api.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 12:39:08.295200 lnctApi-0.0.2/lnctApi.egg-info/
+-rw-r--r--   0 cro        (501) staff       (20)      891 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      227 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/SOURCES.txt
+-rw-r--r--   0 cro        (501) staff       (20)        1 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/dependency_links.txt
+-rw-r--r--   0 cro        (501) staff       (20)       37 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/requires.txt
+-rw-r--r--   0 cro        (501) staff       (20)        8 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/top_level.txt
+-rw-r--r--   0 cro        (501) staff       (20)       38 2023-08-06 12:39:08.295522 lnctApi-0.0.2/setup.cfg
+-rw-r--r--   0 cro        (501) staff       (20)      868 2023-08-06 12:38:57.000000 lnctApi-0.0.2/setup.py
```

### Comparing `lnctApi-0.0.1/LICENSE.txt` & `lnctApi-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lnctApi-0.0.1/PKG-INFO` & `lnctApi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnctApi
-Version: 0.0.1
+Version: 0.0.2
 Summary: LNCT API wrapper, written in Python.
 Home-page: https://github.com/cro2003/lnctApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
 Project-URL: Documnetation, https://cro2003.github.io/lnctApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `lnctApi-0.0.1/lnctApi/accsoft_api.py` & `lnctApi-0.0.2/lnctApi/accsoft_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         viewstate = soup.find_all(id='__VIEWSTATE')[0]['value']
         viewstategenerator = soup.find_all(id='__VIEWSTATEGENERATOR')[0]['value']
         eventvalidation = soup.find_all(id='__EVENTVALIDATION')[0]['value']
         self.session.headers = {'Host': 'portal.lnct.ac.in', 'sec-ch-ua': '"Not/A)Brand";v="99", "Google Chrome";v="115", "Chromium";v="115"', 'DNT': '1', 'sec-ch-ua-mobile': '?0', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36', 'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8', 'Cache-Control': 'no-cache', 'X-Requested-With': 'XMLHttpRequest', 'X-MicrosoftAjax': 'Delta=true', 'sec-ch-ua-platform': '"macOS"', 'Accept': '*/*', 'Origin': 'https://portal.lnct.ac.in', 'Sec-Fetch-Site': 'same-origin', 'Sec-Fetch-Mode': 'cors', 'Sec-Fetch-Dest': 'empty', 'Referer': 'https://portal.lnct.ac.in/Accsoft2/StudentLogin.aspx', 'Accept-Language': 'en-GB,en;q=0.9', 'Cookie': f"ASP.NET_SessionId={requests.utils.dict_from_cookiejar(response.cookies)['ASP.NET_SessionId']}",}
         data = {'ctl00$ScriptManager1': 'ctl00$cph1$UpdatePanel5|ctl00$cph1$btnStuLogin', '__EVENTTARGET': '', '__EVENTARGUMENT': '', '__LASTFOCUS': '', '__VIEWSTATE': viewstate, '__VIEWSTATEGENERATOR': viewstategenerator, '__EVENTVALIDATION': eventvalidation, 'ctl00$cph1$rdbtnlType': '2', 'ctl00$cph1$hdnSID': '', 'ctl00$cph1$hdnSNO': '', 'ctl00$cph1$hdnRDURL': '', 'ctl00$cph1$txtStuUser': self.userId, 'ctl00$cph1$txtStuPsw': self.pswd, '__ASYNCPOST': 'true', 'ctl00$cph1$btnStuLogin': 'Login >>'}
         response = self.session.post('https://portal.lnct.ac.in/Accsoft2/StudentLogin.aspx', data=data)
         if BeautifulSoup(response.text, 'html.parser').find(id='ctl00_cph1_lblErrMsgStu')!=None:
-            return {"error": BeautifulSoup(response.text, 'html.parser').find(id='ctl00_cph1_lblErrMsgStu').get_text()}
+            return json.dumps({"error": BeautifulSoup(response.text, 'html.parser').find(id='ctl00_cph1_lblErrMsgStu').get_text()})
 
     def profile(self):
         """This Function fetches profile information of the Student
 
         :return:
             json: Returns profile information in following format
                   {
```

### Comparing `lnctApi-0.0.1/lnctApi.egg-info/PKG-INFO` & `lnctApi-0.0.2/lnctApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnctApi
-Version: 0.0.1
+Version: 0.0.2
 Summary: LNCT API wrapper, written in Python.
 Home-page: https://github.com/cro2003/lnctApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
 Project-URL: Documnetation, https://cro2003.github.io/lnctApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `lnctApi-0.0.1/setup.py` & `lnctApi-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lnctApi",
-    version="0.0.1",
+    version="0.0.2",
     description="LNCT API wrapper, written in Python.",
     packages=['lnctApi'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cro2003/lnctApi",
     project_urls = {
     'Documnetation': 'https://cro2003.github.io/lnctApi/',
```

