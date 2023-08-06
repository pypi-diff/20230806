# Comparing `tmp/happy_python-0.3.6-py3-none-any.whl.zip` & `tmp/happy_python-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 22361 bytes, number of entries: 18
+Zip file size: 22807 bytes, number of entries: 18
 -rw-r--r--  2.0 unx     2636 b- defN 80-Jan-01 00:00 happy_python/__init__.py
 -rw-r--r--  2.0 unx     5497 b- defN 80-Jan-01 00:00 happy_python/cmd.py
 -rw-r--r--  2.0 unx     1423 b- defN 80-Jan-01 00:00 happy_python/datetime.py
 -rw-r--r--  2.0 unx     1553 b- defN 80-Jan-01 00:00 happy_python/digest.py
 -rw-r--r--  2.0 unx     5506 b- defN 80-Jan-01 00:00 happy_python/domain.py
--rw-r--r--  2.0 unx     3725 b- defN 80-Jan-01 00:00 happy_python/happy_config.py
+-rw-r--r--  2.0 unx     5357 b- defN 80-Jan-01 00:00 happy_python/happy_config.py
 -rw-r--r--  2.0 unx      173 b- defN 80-Jan-01 00:00 happy_python/happy_exception.py
 -rw-r--r--  2.0 unx     5690 b- defN 80-Jan-01 00:00 happy_python/happy_log.py
 -rw-r--r--  2.0 unx      512 b- defN 80-Jan-01 00:00 happy_python/json.py
 -rw-r--r--  2.0 unx     3234 b- defN 80-Jan-01 00:00 happy_python/mail.py
 -rw-r--r--  2.0 unx      930 b- defN 80-Jan-01 00:00 happy_python/misc.py
 -rw-r--r--  2.0 unx     2969 b- defN 80-Jan-01 00:00 happy_python/parameter_manager.py
 -rw-r--r--  2.0 unx    12457 b- defN 80-Jan-01 00:00 happy_python/resource/tlds.txt
 -rw-r--r--  2.0 unx     2206 b- defN 80-Jan-01 00:00 happy_python/str_util.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 happy_python-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx     1361 b- defN 80-Jan-01 00:00 happy_python-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx     1072 b- defN 80-Jan-01 00:00 happy_python-0.3.6.dist-info/LICENSE
-?rw-r--r--  2.0 unx     1452 b- defN 16-Jan-01 00:00 happy_python-0.3.6.dist-info/RECORD
-18 files, 52484 bytes uncompressed, 20003 bytes compressed:  61.9%
+-rw-r--r--  2.0 unx     1072 b- defN 80-Jan-01 00:00 happy_python-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1331 b- defN 80-Jan-01 00:00 happy_python-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 happy_python-0.4.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1452 b- defN 16-Jan-01 00:00 happy_python-0.4.0.dist-info/RECORD
+18 files, 54086 bytes uncompressed, 20449 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: happy_python/resource/tlds.txt
 Comment: 
 
 Filename: happy_python/str_util.py
 Comment: 
 
-Filename: happy_python-0.3.6.dist-info/WHEEL
+Filename: happy_python-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: happy_python-0.3.6.dist-info/METADATA
+Filename: happy_python-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: happy_python-0.3.6.dist-info/LICENSE
+Filename: happy_python-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: happy_python-0.3.6.dist-info/RECORD
+Filename: happy_python-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## happy_python/happy_config.py

```diff
@@ -3,20 +3,34 @@
 
 """
 配置文件（INI）转换类
 """
 
 import os
 from abc import ABCMeta
+from dataclasses import dataclass
 
 from happy_python import HappyPyException
 
 
+@dataclass
+class HappyConfigXListNode:
+    prefix: str
+    keys: list[str]
+
+
+@dataclass
+class HappyConfigXList:
+    section: str
+    node: HappyConfigXListNode
+
+
 class HappyConfigBase(object, metaclass=ABCMeta):
     _section = 'main'
+    _xlist: list[HappyConfigXList] = []
 
     def __init__(self):
         pass
 
     @property
     def section(self):
         """
@@ -28,14 +42,42 @@
     @section.setter
     def section(self, value):
         if value:
             self._section = value
         else:
             raise ValueError("指定的 section 属性值无效。")
 
+    def xlist_add(self, prefix: str, key: str, section: str = ''):
+        __section = self._section if section == '' else section
+        _key = '%s.%s' % (prefix, key)
+
+        if len(self._xlist) == 0:
+            self._xlist.append(HappyConfigXList(section=__section,
+                                                node=HappyConfigXListNode(prefix=prefix,
+                                                                          keys=[_key])))
+        else:
+            for xlist in self._xlist:
+                if xlist.section == __section and xlist.node.prefix == prefix:
+                    if _key not in xlist.node.keys:
+                        xlist.node.keys.append(_key)
+
+    def xlist_key(self, prefix: str, section: str = '') -> list[str]:
+        __section = self._section if section == '' else section
+
+        for xlist in self._xlist:
+            if xlist.section == __section and xlist.node.prefix == prefix:
+                return xlist.node.keys
+
+        return []
+
+    def xlist_get(self, prefix: str, key: str = ''):
+        key = prefix + ('.' + key if key else '')
+
+        return self.__dict__[key] if key in self.__dict__ else None
+
 
 class HappyConfigParser(object):
     @staticmethod
     def load(filename: str, happy_config_object: HappyConfigBase):
         if not isinstance(happy_config_object, HappyConfigBase):
             raise HappyPyException('happy_config_object 不是 HappyConfigBase 类的子类对象。')
 
@@ -49,14 +91,30 @@
                 HappyConfigParser._loads(''.join(content), happy_config_object)
         except Exception as e:
             print("[Error] 配置文件读取错误：%s" % str(e))
             exit(1)
 
     @staticmethod
     def _loads(content: str, happy_config_object: HappyConfigBase):
+        def set_attr(t, _name, _new_name):
+            if t is str:
+                v = cfg.get(section, _name)
+            elif t is int:
+                v = cfg.getint(section, _name)
+            elif t is bool:
+                v = cfg.getboolean(section, _name)
+            elif t is float:
+                v = cfg.getfloat(section, _name)
+            elif t is list:
+                v = cfg.get(section, _name).split(',')
+            else:
+                v = cfg.getboolean(section, _name)
+
+            setattr(happy_config_object, _new_name, v)
+
         from configparser import ConfigParser
 
         if not isinstance(happy_config_object, HappyConfigBase):
             raise HappyPyException('happy_config_object 不是 HappyConfigBase 类的子类对象。')
 
         try:
             cfg = ConfigParser()
@@ -64,35 +122,29 @@
 
             class_attrs = happy_config_object.__dict__
             section = happy_config_object.section
 
             for name, value in class_attrs.items():
                 if name == '_section':
                     continue
+                set_attr(type(value), name, name)
+            for section, section_obj in cfg.items():
+                if section == '_section':
+                    continue
 
-                t = type(value)
-
-                if t is str:
-                    v = cfg.get(section, name)
-                    exec("happy_config_object.%s='%s'" % (name, v))
-                elif t is int:
-                    v = cfg.getint(section, name)
-                    exec("happy_config_object.%s=%d" % (name, v))
-                elif t is bool:
-                    v = cfg.getboolean(section, name)
-                    exec("happy_config_object.%s=%s" % (name, v))
-                elif t is float:
-                    v = cfg.getfloat(section, name)
-                    exec("happy_config_object.%s=%f" % (name, v))
-                elif t is list:
-                    v = cfg.get(section, name).split(',')
-                    exec("happy_config_object.%s=%s" % (name, v))
-                else:
-                    v = cfg.getboolean(section, name)
-                    exec("happy_config_object.%s=%s" % (name, v))
+                for name, value in section_obj.items():
+                    if not name.startswith('!'):
+                        continue
+
+                    new_name = name[1:]
+                    parts = new_name.split('.')
+
+                    if len(parts) >= 2:
+                        happy_config_object.xlist_add(section=section, prefix=parts[0], key=parts[1])
+                        set_attr(type(value), name, new_name)
         except Exception as e:
             print("[Error] 配置文件读取错误：%s" % str(e))
             exit(1)
 
     @staticmethod
     def load_with_var(filename: str, var_dict: dict, happy_config_object: HappyConfigBase):
         try:
```

## Comparing `happy_python-0.3.6.dist-info/METADATA` & `happy_python-0.4.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: happy-python
-Version: 0.3.6
+Version: 0.4.0
 Summary: Happy-Python是一个简单易用的Python库，让编程轻松愉快
 Home-page: https://github.com/geekcampchina/happy-python
 License: MIT
 Author: Chengdu Geek Camp
 Author-email: info@cdgeekcamp.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Documentation, https://github.com/geekcampchina/happy-python
 Project-URL: Repository, https://github.com/geekcampchina/happy-python
 Description-Content-Type: text/markdown
 
 # happy-python
 
 Happy-Python是一个简单易用的Python库，让编程轻松愉快
 
-## 安装依赖
+## 安装开发依赖
 
 `pip install poetry pytest`
 
 ## 单元测试
 
 运行单元测试：
 
 `poetry run pytest`
 
-## 安装
+## 安装happy-python
 
 ### Pip安装
 
 `pip install happy-python`
 
 ## 本地安装
```

## Comparing `happy_python-0.3.6.dist-info/LICENSE` & `happy_python-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `happy_python-0.3.6.dist-info/RECORD` & `happy_python-0.4.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 happy_python/__init__.py,sha256=aEJ0nsDdFpD17KzO4GHhAtMFmQZhYipb_5NVYlGWk0s,2636
 happy_python/cmd.py,sha256=BmCkYtvEmgOyKMt-Rg6cO1KErhodOo2Zf2yOxH9tl58,5497
 happy_python/datetime.py,sha256=FARm_pGu9s_a7g-1-JHdkvjexmgUztu7KzIBUAbD7pI,1423
 happy_python/digest.py,sha256=6CAJHnR8YvuCnQ3hQ7ZxPCAM7K4oV0DnG3sK_yIiJKQ,1553
 happy_python/domain.py,sha256=bDNBpCtEp8s1huw5KVt3fEOT4DBl7-OiYTz7S1Pr_h0,5506
-happy_python/happy_config.py,sha256=S6kWwPm0QlgjPBjsoRGncMvLyJxLWHNtU-ARfrnaEG4,3725
+happy_python/happy_config.py,sha256=mKitQ3ppGASsDKDKFo7jyjNgy2LReMN-RqzppQ5-TkI,5357
 happy_python/happy_exception.py,sha256=m5qHXKxWALonI8P_baKbpdgHA7yj6EvcYggc7lJDAms,173
 happy_python/happy_log.py,sha256=I_KTf_RP5mAFiduCPiBkUapgcp_1C1Efk5flE16h00Y,5690
 happy_python/json.py,sha256=nuhZMlHLgB_wzgGV2EYHX9Cpl0GosLWuDWOsyM3jslU,512
 happy_python/mail.py,sha256=KLZ6qJvZ7s-FMQKSU8iYyABMCcUEGYnUWqdm6jX9-54,3234
 happy_python/misc.py,sha256=t5CTIODdBhy5JZ7wUve_it38OgeGekZzLaZY0V-kxTM,930
 happy_python/parameter_manager.py,sha256=dJTLRJupwndffoeFjYAuHSP5gqw4CIhIwNefAvKSAb4,2969
 happy_python/resource/tlds.txt,sha256=lMRU0YxFqK0nZt_P-rtx_i-klVPcjzEjNHWsYjnwFVY,12457
 happy_python/str_util.py,sha256=L5ESKAouh_3IGQXIjWBcOpvaHePIadaX0A0FcGyEbVk,2206
-happy_python-0.3.6.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-happy_python-0.3.6.dist-info/METADATA,sha256=WJ2oS33EuLXlJXxBoFxmupfYt0kBrF7WeP4V-3jSOoA,1361
-happy_python-0.3.6.dist-info/LICENSE,sha256=NrK0nvgt_x7V38ZcVzPA06RWRUyUMGdWba9i1-svAO0,1072
-happy_python-0.3.6.dist-info/RECORD,,
+happy_python-0.4.0.dist-info/LICENSE,sha256=NrK0nvgt_x7V38ZcVzPA06RWRUyUMGdWba9i1-svAO0,1072
+happy_python-0.4.0.dist-info/METADATA,sha256=9bBCO_NoCkesyZFrLwiy7D1fkeQrG4472ddxsSmHry4,1331
+happy_python-0.4.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+happy_python-0.4.0.dist-info/RECORD,,
```

