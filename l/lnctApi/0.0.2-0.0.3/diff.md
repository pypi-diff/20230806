# Comparing `tmp/lnctApi-0.0.2.tar.gz` & `tmp/lnctApi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnctApi-0.0.2.tar", last modified: Sun Aug  6 12:39:08 2023, max compression
+gzip compressed data, was "lnctApi-0.0.3.tar", last modified: Sun Aug  6 16:46:56 2023, max compression
```

## Comparing `lnctApi-0.0.2.tar` & `lnctApi-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 12:39:08.295482 lnctApi-0.0.2/
--rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 lnctApi-0.0.2/LICENSE.txt
--rw-r--r--   0 cro        (501) staff       (20)      891 2023-08-06 12:39:08.295374 lnctApi-0.0.2/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      336 2023-08-05 18:56:59.000000 lnctApi-0.0.2/README.md
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 12:39:08.294558 lnctApi-0.0.2/lnctApi/
--rw-r--r--   0 cro        (501) staff       (20)       32 2023-08-04 19:28:06.000000 lnctApi-0.0.2/lnctApi/__init__.py
--rw-r--r--   0 cro        (501) staff       (20)    23093 2023-08-06 12:33:58.000000 lnctApi-0.0.2/lnctApi/accsoft_api.py
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 12:39:08.295200 lnctApi-0.0.2/lnctApi.egg-info/
--rw-r--r--   0 cro        (501) staff       (20)      891 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      227 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/SOURCES.txt
--rw-r--r--   0 cro        (501) staff       (20)        1 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/dependency_links.txt
--rw-r--r--   0 cro        (501) staff       (20)       37 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/requires.txt
--rw-r--r--   0 cro        (501) staff       (20)        8 2023-08-06 12:39:08.000000 lnctApi-0.0.2/lnctApi.egg-info/top_level.txt
--rw-r--r--   0 cro        (501) staff       (20)       38 2023-08-06 12:39:08.295522 lnctApi-0.0.2/setup.cfg
--rw-r--r--   0 cro        (501) staff       (20)      868 2023-08-06 12:38:57.000000 lnctApi-0.0.2/setup.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 16:46:56.385861 lnctApi-0.0.3/
+-rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 lnctApi-0.0.3/LICENSE.txt
+-rw-r--r--   0 cro        (501) staff       (20)      891 2023-08-06 16:46:56.385746 lnctApi-0.0.3/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      336 2023-08-05 18:56:59.000000 lnctApi-0.0.3/README.md
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 16:46:56.384813 lnctApi-0.0.3/lnctApi/
+-rw-r--r--   0 cro        (501) staff       (20)       32 2023-08-04 19:28:06.000000 lnctApi-0.0.3/lnctApi/__init__.py
+-rw-r--r--   0 cro        (501) staff       (20)    23148 2023-08-06 16:44:26.000000 lnctApi-0.0.3/lnctApi/accsoft_api.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 16:46:56.385577 lnctApi-0.0.3/lnctApi.egg-info/
+-rw-r--r--   0 cro        (501) staff       (20)      891 2023-08-06 16:46:56.000000 lnctApi-0.0.3/lnctApi.egg-info/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      227 2023-08-06 16:46:56.000000 lnctApi-0.0.3/lnctApi.egg-info/SOURCES.txt
+-rw-r--r--   0 cro        (501) staff       (20)        1 2023-08-06 16:46:56.000000 lnctApi-0.0.3/lnctApi.egg-info/dependency_links.txt
+-rw-r--r--   0 cro        (501) staff       (20)       37 2023-08-06 16:46:56.000000 lnctApi-0.0.3/lnctApi.egg-info/requires.txt
+-rw-r--r--   0 cro        (501) staff       (20)        8 2023-08-06 16:46:56.000000 lnctApi-0.0.3/lnctApi.egg-info/top_level.txt
+-rw-r--r--   0 cro        (501) staff       (20)       38 2023-08-06 16:46:56.385895 lnctApi-0.0.3/setup.cfg
+-rw-r--r--   0 cro        (501) staff       (20)      868 2023-08-06 16:46:28.000000 lnctApi-0.0.3/setup.py
```

### Comparing `lnctApi-0.0.2/LICENSE.txt` & `lnctApi-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lnctApi-0.0.2/PKG-INFO` & `lnctApi-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lnctApi
-Version: 0.0.2
+Version: 0.0.3
 Summary: LNCT API wrapper, written in Python.
 Home-page: https://github.com/cro2003/lnctApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
-Project-URL: Documnetation, https://cro2003.github.io/lnctApi/
+Project-URL: Documentation, https://cro2003.github.io/lnctApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `lnctApi-0.0.2/lnctApi/accsoft_api.py` & `lnctApi-0.0.3/lnctApi/accsoft_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class accsoft:
     """This Class Contains all the Function for getting Student Accsoft information
 
     :arg:
         userId (str): Accsoft Identification Number given by College
         pswd (str): Password for the Accsoft Id
     """
-    def __init__(self, userId, pswd):
+    def __init__(self, userId: str, pswd: str):
         self.session = requests.Session()
         self.userId = userId
         self.pswd = pswd
         self.session.headers = None
 
     def _getLogin(self):
         if self.session.headers!=None:
@@ -94,15 +94,15 @@
         present = int(re.sub('\D', '', soup.find_all(id='ctl00_ContentPlaceHolder1_lbltotalp')[0].get_text()))
         absent = int(re.sub('\D', '', soup.find_all(id='ctl00_ContentPlaceHolder1_lbltotala')[0].get_text()))
         if TotalLectures != 0:
             percentage = decimal.Decimal(present * 100 / TotalLectures)
             percentage = round(percentage, 2)
         else:
             percentage = 0
-        product = {"name": name, "totalLectures": TotalLectures, "present": present, "absent": absent, "percentage": f"{percentage}"}
+        product = {"name": name, "totalLectures": TotalLectures, "present": present, "absent": absent, "percentage": percentage}
         return json.dumps(product)
 
     def attendanceDatewise(self):
         """This Function fetches Attendance of the Student Datewise
 
         :return:
             json: Returns datewise attendance in following format
@@ -238,15 +238,15 @@
             soup = BeautifulSoup(response.text, 'html.parser')
             if soup.find(id='ctl00_ContentPlaceHolder1_VSFlexGrid1').find('td').get_text().strip() == 'There is No Record to View !':continue
             table = soup.find(id='ctl00_ContentPlaceHolder1_VSFlexGrid1')
             for z in table.find_all('tr'):
                 if z.find_all('th') == []:
                     date = z.find_all('td')[2].get_text().replace('\n', '')
                     voucherNumber = z.find_all('td')[3].get_text().replace('\n', '')
-                    ttlAmt = z.find_all('td')[4].get_text().replace('\n', '')
+                    ttlAmt = float(z.find_all('td')[4].get_text().replace('\n', ''))
                     value = {"txnDate": date, "VNumber": voucherNumber, "totalAmt": ttlAmt}
                     feelo.append(value)
         product['feesInfo'] = list(reversed(feelo))
         return json.dumps(product)
 
     def feetxn(self):
         """This Function fetches All the Fees Transaction which are Initiated through Accosft
@@ -285,15 +285,15 @@
             soup = BeautifulSoup(response.text, 'html.parser')
             table = soup.find(id='ctl00_ContentPlaceHolder1_grdHistory')
             if table==None:continue
             for z in table.find_all('tr'):
                 if z.find_all('th') == []:
                     date = z.find_all('td')[0].get_text().replace('\n', '')
                     pId = z.find_all('td')[1].get_text().replace('\n', '')
-                    txnAmt = z.find_all('td')[2].get_text().replace('\n', '')
+                    txnAmt = float(z.find_all('td')[2].get_text().replace('\n', ''))
                     status = z.find_all('td')[3].get_text().replace('\n', '')
                     value = {"date": date, "paymentId": pId, "amount": txnAmt, "status":status}
                     feelo.append(value)
         product['feetxn'] = list(reversed(feelo))
         return json.dumps(product)
 
     def libRecord(self):
@@ -323,23 +323,23 @@
             return show
         response = self.session.get('https://portal.lnct.ac.in/Accsoft2/Parents/CirculationLedger.aspx')
         soup = BeautifulSoup(response.text, 'html.parser')
         name = soup.find(class_='mr-2 d-none d-lg-inline small text-gray-500').get_text().strip()
         product = {"name": name, "bookRecord": []}
         table = soup.find(id='ctl00_ContentPlaceHolder1_grdCRList')
         if table==None:
-            return product
+            return json.dumps(product)
         records = []
         for x in table.find_all('tr'):
             if x.find_all('td')==[]:continue
             date = x.find_all('td')[1].get_text()
             bookName = x.find_all('td')[4].get_text()
             dueDate = x.find_all('td')[6].get_text()
             returnedDate = x.find_all('td')[7].get_text().replace('\n', '')
-            lateDay = x.find_all('td')[8].get_text()
+            lateDay = int(x.find_all('td')[8].get_text())
             value = {'date': date, 'bookName': bookName, 'dueDate': dueDate, 'returnedDate': returnedDate, 'lateDay': lateDay}
             records.append(value)
         product['bookRecord'] = records
         return json.dumps(product)
 
     def fineRecord(self):
         """This Function fetches All the Fine Records of the Library
@@ -367,17 +367,17 @@
         response = self.session.get('https://portal.lnct.ac.in/Accsoft2/Parents/FineRecord.aspx')
         soup = BeautifulSoup(response.text, 'html.parser')
         name = soup.find(class_='mr-2 d-none d-lg-inline small text-gray-500').get_text().strip()
         product = {"name": name, "fine": []}
         record = []
         table = soup.find(id='ctl00_ContentPlaceHolder1_GrdFine')
         if table==None:
-            return product
+            return json.dumps(product)
         for x in table.find_all('tr'):
             if x.find_all('td')==[]:continue
             libName = x.find_all('td')[1].get_text()
             collectedBy = x.find_all('td')[2].get_text()
             date = x.find_all('td')[3].get_text()
-            amt = x.find_all('td')[8].get_text()
+            amt = float(x.find_all('td')[8].get_text())
             record.append({'libName':libName, 'collectedBy':collectedBy, 'date':date, 'amt':amt})
         product['fine'] = record
         return json.dumps(product)
```

### Comparing `lnctApi-0.0.2/lnctApi.egg-info/PKG-INFO` & `lnctApi-0.0.3/lnctApi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lnctApi
-Version: 0.0.2
+Version: 0.0.3
 Summary: LNCT API wrapper, written in Python.
 Home-page: https://github.com/cro2003/lnctApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
-Project-URL: Documnetation, https://cro2003.github.io/lnctApi/
+Project-URL: Documentation, https://cro2003.github.io/lnctApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `lnctApi-0.0.2/setup.py` & `lnctApi-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lnctApi",
-    version="0.0.2",
+    version="0.0.3",
     description="LNCT API wrapper, written in Python.",
     packages=['lnctApi'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cro2003/lnctApi",
     project_urls = {
-    'Documnetation': 'https://cro2003.github.io/lnctApi/',
+    'Documentation': 'https://cro2003.github.io/lnctApi/',
     },
     author="cro2003",
     author_email="cro@chirag.software",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.11",
```

