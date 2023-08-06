# Comparing `tmp/db2text-0.0.9.tar.gz` & `tmp/db2text-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/db2text-0.0.9.tar", last modified: Thu Jul 29 12:59:03 2021, max compression
+gzip compressed data, was "db2text-0.1.1.tar", last modified: Sat Mar 18 07:02:23 2023, max compression
```

## Comparing `db2text-0.0.9.tar` & `db2text-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 12:59:03.000000 db2text-0.0.9/
--rwxrw-rw-   0 root         (0) root         (0)       44 2021-06-03 14:29:28.000000 db2text-0.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      621 2021-07-29 12:59:03.000000 db2text-0.0.9/PKG-INFO
--rwxrw-rw-   0 root         (0) root         (0)      154 2021-03-14 10:39:32.000000 db2text-0.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 12:59:03.000000 db2text-0.0.9/bin/
--rwxrw-rw-   0 root         (0) root         (0)     1862 2021-07-28 13:44:51.000000 db2text-0.0.9/bin/dbt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 12:59:03.000000 db2text-0.0.9/database2text/
--rwxrw-rw-   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 db2text-0.0.9/database2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 12:59:03.000000 db2text-0.0.9/database2text/datafile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 12:59:03.000000 db2text-0.0.9/database2text/datafile/sample/
--rwxrw-rw-   0 root         (0) root         (0)      988 2021-07-12 14:11:19.000000 db2text-0.0.9/database2text/datafile/sample/dbt_oracle11.txt
--rwxrw-rw-   0 root         (0) root         (0)     4634 2021-07-29 02:21:47.000000 db2text-0.0.9/database2text/datafile/usermenual.md
--rwxrw-rw-   0 root         (0) root         (0)     1398 2021-07-29 03:16:49.000000 db2text-0.0.9/database2text/mysql.py
--rwxrw-rw-   0 root         (0) root         (0)     4676 2021-07-29 02:38:43.000000 db2text-0.0.9/database2text/oracle11.py
--rwxrw-rw-   0 root         (0) root         (0)     5473 2021-07-29 09:38:13.000000 db2text-0.0.9/database2text/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 12:59:03.000000 db2text-0.0.9/db2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)      621 2021-07-29 12:59:02.000000 db2text-0.0.9/db2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      373 2021-07-29 12:59:02.000000 db2text-0.0.9/db2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-29 12:59:02.000000 db2text-0.0.9/db2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-03 14:11:16.000000 db2text-0.0.9/db2text.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2021-07-29 12:59:02.000000 db2text-0.0.9/db2text.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-29 12:59:03.000000 db2text-0.0.9/setup.cfg
--rwxrw-rw-   0 root         (0) root         (0)      761 2021-07-29 12:58:30.000000 db2text-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 07:02:23.000000 db2text-0.1.1/
+-rwxr--r--   0 root         (0) root         (0)     1063 2021-03-12 13:21:32.000000 db2text-0.1.1/LICENSE
+-rwxr--r--   0 root         (0) root         (0)       44 2021-06-03 14:29:28.000000 db2text-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      553 2023-03-18 07:02:23.000000 db2text-0.1.1/PKG-INFO
+-rwxr--r--   0 root         (0) root         (0)      154 2021-03-14 10:39:32.000000 db2text-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 07:02:22.000000 db2text-0.1.1/bin/
+-rwxr--r--   0 root         (0) root         (0)     1862 2021-07-28 13:44:51.000000 db2text-0.1.1/bin/dbt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 07:02:22.000000 db2text-0.1.1/database2text/
+-rwxr--r--   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 db2text-0.1.1/database2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 07:02:22.000000 db2text-0.1.1/database2text/datafile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 07:02:22.000000 db2text-0.1.1/database2text/datafile/sample/
+-rwxr--r--   0 root         (0) root         (0)      988 2021-07-12 14:11:19.000000 db2text-0.1.1/database2text/datafile/sample/dbt_oracle11.txt
+-rwxr--r--   0 root         (0) root         (0)     4634 2021-07-29 02:21:47.000000 db2text-0.1.1/database2text/datafile/usermenual.md
+-rwxr--r--   0 root         (0) root         (0)     1363 2022-03-25 06:10:04.000000 db2text-0.1.1/database2text/mysql.py
+-rwxr--r--   0 root         (0) root         (0)     6071 2023-03-18 06:52:30.000000 db2text-0.1.1/database2text/oracle11.py
+-rwxr--r--   0 root         (0) root         (0)     5915 2021-07-30 06:11:52.000000 db2text-0.1.1/database2text/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 07:02:22.000000 db2text-0.1.1/db2text.egg-info/
+-rwxr--r--   0 root         (0) root         (0)      553 2023-03-18 07:02:22.000000 db2text-0.1.1/db2text.egg-info/PKG-INFO
+-rwxr--r--   0 root         (0) root         (0)      381 2023-03-18 07:02:22.000000 db2text-0.1.1/db2text.egg-info/SOURCES.txt
+-rwxr--r--   0 root         (0) root         (0)        1 2023-03-18 07:02:22.000000 db2text-0.1.1/db2text.egg-info/dependency_links.txt
+-rwxr--r--   0 root         (0) root         (0)        1 2021-06-03 14:11:16.000000 db2text-0.1.1/db2text.egg-info/not-zip-safe
+-rwxr--r--   0 root         (0) root         (0)       14 2023-03-18 07:02:22.000000 db2text-0.1.1/db2text.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-18 07:02:23.000000 db2text-0.1.1/setup.cfg
+-rwxr--r--   0 root         (0) root         (0)      759 2023-03-18 06:57:35.000000 db2text-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `db2text-0.0.9/bin/dbt` & `db2text-0.1.1/bin/dbt`

 * *Files identical despite different names*

### Comparing `db2text-0.0.9/database2text/datafile/sample/dbt_oracle11.txt` & `db2text-0.1.1/database2text/datafile/sample/dbt_oracle11.txt`

 * *Files identical despite different names*

### Comparing `db2text-0.0.9/database2text/datafile/usermenual.md` & `db2text-0.1.1/database2text/datafile/usermenual.md`

 * *Files identical despite different names*

### Comparing `db2text-0.0.9/database2text/mysql.py` & `db2text-0.1.1/database2text/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import sys,pymysql
 import database2text.tool as dbtt
 from database2text.tool import *
 
 class mysql(object):
     def ana_TABLE(otype):
         for oname, in db.exec("show tables"):
-            _,odata=db.res1("show create table %s" %(oname))
+            res=db.res1("show create table %s" %(oname))
+            odata=res[1]
             oridata=[]
             coldata=[]
             tdesc=db.res1("SELECT TABLE_COMMENT FROM INFORMATION_SCHEMA.TABLES  WHERE TABLE_NAME ='%s' AND TABLE_SCHEMA = '%s'" %(oname,database))
             for i in db.exec2("select * from information_schema.COLUMNS where TABLE_SCHEMA='%s' and table_name='%s'" %(database,oname)):
                 oridata.append(i)
             dbdata["sql"]["TABLE"][oname]=odata
             dbdata["exp"]["TABLE"].append({"tname":oname,"tdesc":tdesc,"ori":oridata,"c":coldata})
@@ -28,16 +29,13 @@
             getattr(mysql,i)(otype)
 
 def connect():
     global database
     database=stdata["database"]
     if "port" in stdata:
         stdata["port"]=int(stdata["port"])
-    try:
-        db.conn=pymysql.connect(**stdata)
-    except:
-        quit("connect error!")
+    db.conn=pymysql.connect(**stdata)
 
 def export(stdata,storidata):
     dbtt.export(stdata,storidata,dbdata)
 
 __all__=[]
```

### Comparing `db2text-0.0.9/database2text/oracle11.py` & `db2text-0.1.1/database2text/oracle11.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,28 @@
 import sys,cx_Oracle,json
 import database2text.tool as dbtt
 from database2text.tool import *
 
 class oracle(object):
     def ana_TABLE(otype):
         for oname, in db.exec("select object_name from user_objects where object_type=:ot",ot=otype):
+            if "table" in stdata and oname.lower() not in stdata["table"].split() and oname not in stdata["table"].split():
+                continue
+            if oname.startswith("SYS_EXPORT_TABLE"):
+                continue
             odata="create table %s\n(\n" %(oname)
             coldata=[]  #记录列数据，包括type类型，name列名，desc注释信息，size长度，ns名称+长度如name[5]这样
             maxcsize=db.res1("select max(length(column_name)) from all_tab_cols where owner='%s' and table_name='%s'" %(owner,oname))
             tdesc=db.res1("select comments from user_tab_comments where table_name=:1",[oname])
             oridata=[]
+            for col in db.exec2("select * from all_tab_cols where owner='%s' and table_name='%s' order by column_id" %(owner,oname)):
+                col["COLUMN_COMMENT"]=db.res1("select comments from user_col_comments where table_name=:n and column_name=:cn",n=oname,cn=col["COLUMN_NAME"])
+                if col["DATA_DEFAULT"]!=None:
+                    col["DATA_DEFAULT"]=col["DATA_DEFAULT"].strip()
+                oridata.append(col)
             for column_name,data_type,char_length,data_precision,data_scale,nullable,default_length,data_default in db.exec("select column_name,data_type,char_length,data_precision,data_scale,nullable,default_length,data_default from all_tab_cols where owner='%s' and table_name='%s' order by column_id" %(owner,oname)):
                 odata=odata+"  %s%*s" %(column_name,maxcsize-len(column_name)+1," ")
                 ctype="char"
                 cns="%s[%d]" %(column_name,char_length+1)
                 desc=db.res1("select comments from user_col_comments where table_name=:n and column_name=:cn",n=oname,cn=column_name)
                 if not desc:desc=""
                 if data_type=="NUMBER":
@@ -31,50 +40,64 @@
                     elif data_precision is None and data_scale==0:
                         ctype="long"
                         odata=odata+"INTEGER"
                     elif char_length==0:
                         ctype="long"
                         odata=odata+"NUMBER"
                     else:
-                        print("table %s column %s length %s %s %s" %(oname,column_name,char_length,data_precision,data_scale))
-                        sys.exit(0)
+                        print("table %s column %s type %s length %s %s %s" %(oname,column_name,data_type,char_length,data_precision,data_scale))
+                        sys.exit(-1)
                     cns=column_name
-                elif data_type in ("VARCHAR2","VARCHAR","CHAR"):
+                elif data_type in ("VARCHAR2","VARCHAR","CHAR","NVARCHAR2","NVARCHAR"):
                     if char_length==1:cns=column_name
                     odata=odata+"%s(%d)" %(data_type,char_length)
                 elif data_type.startswith("TIMESTAMP"):
                     cns="%s[20]" %(column_name)
                     odata=odata+"%s" %(data_type)
-                elif data_type in("DATE","BLOB"):
+                elif data_type in("DATE"):
                     cns="%s[20]" %(column_name)
                     odata=odata+"%s" %(data_type)
+                elif data_type in("CLOB","BLOB","NCLOB","LONG","RAW"):
+                    cns="%s[2000]" %(column_name)
+                    odata=odata+"%s" %(data_type)
+                elif data_type in ("FLOAT"):
+                    ctype="double"
+                    odata=odata+"FLOAT(%d)" %(data_precision)
+                elif data_type in ("ROWID"):
+                    cns="%s[100]" %(column_name)
+                    odata=odata+"%s" %(data_type)
                 else:
-                    print("table %s column %s length %s %s %s" %(oname,column_name,char_length,data_precision,data_scale))
-                    sys.exit(0)
+                    print("table %s column %s type %s length %s %s %s" %(oname,column_name,data_type,char_length,data_precision,data_scale))
+                    sys.exit(-1)
                 if default_length:
                     odata=odata+" default %s" %(data_default.strip())
                 if nullable=="N":
                     odata=odata+" not null"
                 odata=odata+",\n"
                 coldata.append({"type":ctype,"name":column_name,"ns":cns,"desc":desc})
             odata=odata[:-2]
             odata=odata+"\n);"
             dbdata["sql"]["TABLE"][oname]=odata
             dbdata["exp"]["TABLE"].append({"tname":oname,"tdesc":tdesc,"ori":oridata,"c":coldata})
 
     def ana_VIEW(otype):
         for oname, in db.exec("select object_name from user_objects where object_type=:ot",ot=otype):
-            dbdata["sql"][otype][oname]=getobjtext(otype,oname)
+            if "view" in stdata and oname.lower() not in stdata["view"].split() and oname not in stdata["view"].split():
+                continue
+            dbdata["sql"][otype][oname]=oracle.getobjtext(otype,oname)
 
     def getobjtext(otype,oname):
         c=db.conn.cursor()
-        c.callproc('DBMS_METADATA.SET_TRANSFORM_PARAM',(-1, 'TABLESPACE',False))
-        c.callproc("DBMS_METADATA.SET_TRANSFORM_PARAM",(-1,'STORAGE',False))
-        c.callproc("DBMS_METADATA.SET_TRANSFORM_PARAM",(-1,'SEGMENT_ATTRIBUTES',False))
-        c.callproc("DBMS_METADATA.SET_TRANSFORM_PARAM",(-1,'PRETTY',False))
+        try:
+            c.callproc('DBMS_METADATA.SET_TRANSFORM_PARAM',(-1, 'TABLESPACE',False))
+            c.callproc("DBMS_METADATA.SET_TRANSFORM_PARAM",(-1,'STORAGE',False))
+            c.callproc("DBMS_METADATA.SET_TRANSFORM_PARAM",(-1,'SEGMENT_ATTRIBUTES',False))
+            c.callproc("DBMS_METADATA.SET_TRANSFORM_PARAM",(-1,'PRETTY',False))
+        except:
+            pass
         ssql=db.res1("SELECT dbms_metadata.get_ddl(:otype,:oname) FROM DUAL",otype=otype,oname=oname).read()
         return ssql
 
 def readdata():
     for i in vars(oracle):
         if i.startswith("ana_"):
             otype=i[4:]
```

### Comparing `db2text-0.0.9/database2text/tool.py` & `db2text-0.1.1/database2text/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import sys,os,difflib,jinja2,re,json
+import sys,os,difflib,jinja2,re,json,datetime
 
 __all__=["db","ckd","dbdata","storidata","stdata"]
 
 def mkdir(dirname):
     if not os.path.isdir(dirname):
         os.mkdir(dirname)
 
 def quit(errinfo,exitcode=0):
     print(errinfo)
     sys.exit(exitcode)
 
+class ComplexEncoder(json.JSONEncoder):
+    def default(self, obj):
+        print(obj,type(obj))
+        if isinstance(obj, datetime.datetime):
+            return obj.strftime('%Y-%m-%d %H:%M:%S')
+        elif isinstance(obj, datetime.date):
+            return obj.strftime('%Y-%m-%d')
+        elif isinstance(obj,bytes):
+            return ""
+        else:
+            return json.JSONEncoder.default(self, obj)
+
 class dblib(object):
     def res1(self,ssql,*args,**kwargs):
         c=self.conn.cursor()
         c.execute(ssql,*args,**kwargs)
         res=c.fetchone()
         c.close()
         if res==None:
@@ -102,15 +114,15 @@
 class render(object):
     def __init__(self):
         for t in dbdata["exp"]["TABLE"]:
             if not "table" in stdata or t["tname"].lower() in stdata["table"].split():
                 self.rendertable(t)
     def rendertable(self,t):
         if "help" in stdata and stdata["help"].lower() in ["y","1"]:
-            print(json.dumps(t,ensure_ascii=False,skipkeys=False,indent=4))
+            print(json.dumps(t,ensure_ascii=False,skipkeys=False,indent=4,cls=ComplexEncoder))
         tpl=""  #模板
         k=False
         for l in storidata:
             if l.startswith("start="):
                 k=True
                 continue
             if l.startswith("end="):
```

### Comparing `db2text-0.0.9/setup.py` & `db2text-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="db2text",
-    version="0.0.9",
+    version="0.1.1",
     author="Chen chuan",
-    author_email="chenc224@163.com",
+    author_email="kcchen@139.com",
     description="database to text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/chenc224/dbt",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

