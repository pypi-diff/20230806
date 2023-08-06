# Comparing `tmp/speedtools-0.4.0.tar.gz` & `tmp/speedtools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtools-0.4.0.tar", last modified: Sun Jul 30 13:53:43 2023, max compression
+gzip compressed data, was "speedtools-0.5.0.tar", last modified: Sun Aug  6 17:02:08 2023, max compression
```

## Comparing `speedtools-0.4.0.tar` & `speedtools-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.136143 speedtools-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 13:53:26.000000 speedtools-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-30 13:53:43.136143 speedtools-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-30 13:53:26.000000 speedtools-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-30 13:53:26.000000 speedtools-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 13:53:43.136143 speedtools-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-30 13:53:26.000000 speedtools-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.132143 speedtools-0.4.0/speedtools/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.132143 speedtools-0.4.0/speedtools/blender/
--rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/blender/io_nfs4_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/frd_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.132143 speedtools-0.4.0/speedtools/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/qfs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/refpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.136143 speedtools-0.4.0/speedtools/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/fce.ksy
--rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/frd.ksy
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/fsh.ksy
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/qfs.ksy
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/viv.ksy
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/speedtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/tr_ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/track_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/viv_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.132143 speedtools-0.4.0/speedtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:02:08.683599 speedtools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-06 17:01:50.000000 speedtools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-06 17:02:08.683599 speedtools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-06 17:01:50.000000 speedtools-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-08-06 17:01:50.000000 speedtools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 17:02:08.683599 speedtools-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-06 17:01:50.000000 speedtools-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:02:08.679598 speedtools-0.5.0/speedtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:02:08.679598 speedtools-0.5.0/speedtools/blender/
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/blender/io_nfs4_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/frd_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/fsh_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:02:08.679598 speedtools-0.5.0/speedtools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/refpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:02:08.683599 speedtools-0.5.0/speedtools/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/specs/fce.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/specs/frd.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/specs/fsh.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/specs/qfs.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/specs/viv.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/speedtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/tr_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-08-06 17:01:50.000000 speedtools-0.5.0/speedtools/viv_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:02:08.679598 speedtools-0.5.0/speedtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-06 17:02:08.000000 speedtools-0.5.0/speedtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-06 17:02:08.000000 speedtools-0.5.0/speedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:02:08.000000 speedtools-0.5.0/speedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-06 17:02:08.000000 speedtools-0.5.0/speedtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 17:02:08.000000 speedtools-0.5.0/speedtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 17:02:08.000000 speedtools-0.5.0/speedtools.egg-info/top_level.txt
```

### Comparing `speedtools-0.4.0/LICENSE` & `speedtools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/PKG-INFO` & `speedtools-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.4.0
+Version: 0.5.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -59,13 +59,12 @@
 * [Kaitai Struct compiler][3]
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
-* Road lanes are missing
 * The bear has left the park!
 
 [1]: https://pypi.org/project/speedtools/
 [2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.4.0/README.md` & `speedtools-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -40,13 +40,12 @@
 * [Kaitai Struct compiler][3]
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
-* Road lanes are missing
 * The bear has left the park!
 
 [1]: https://pypi.org/project/speedtools/
 [2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.4.0/pyproject.toml` & `speedtools-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speedtools"
-version = "0.4.0"
+version = "0.5.0"
 description = "NFS4 HS (PC) resource utilities"
 authors = [{ name = "Rafał Kuźnia" }, { email = "rafal.kuznia@protonmail.com" }]
 readme = { file = 'README.md', content-type = 'text/markdown' }
 dependencies = ["kaitaistruct", "pillow", "click", "more-itertools", "parse"]
 license = { text = "GPL-3.0-or-later" }
 classifiers = [
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
@@ -68,15 +68,15 @@
     "wm",
 ]
 
 [tool.pylint.design]
 # Maximum number of arguments for function / method.
 max-args = 8
 # Maximum number of attributes for a class (see R0902).
-max-attributes = 10
+max-attributes = 15
 # Maximum number of locals for function / method body.
 max-locals = 16
 # Minimum number of public methods for a class (see R0903).
 min-public-methods = 1
 
 [tool.pylint."messages control"]
 # Disable the message, report, category or checker with the given id(s). You can
```

### Comparing `speedtools-0.4.0/setup.py` & `speedtools-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/speedtools/blender/io_nfs4_import.py` & `speedtools-0.5.0/speedtools/blender/io_nfs4_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,16 +327,20 @@
 
     def invoke(self, context: bpy.types.Context, event: bpy.types.Event) -> set[int] | set[str]:
         wm = context.window_manager
         wm.fileselect_add(self)
         return {"RUNNING_MODAL"}
 
     def execute(self, context: bpy.types.Context) -> set[int] | set[str]:
+        directory = Path(self.directory)
+        # This should get us from track directory to game root directory
+        game_root = directory.parent.parent.parent
         track = TrackData(
-            directory=self.directory,
+            directory=Path(self.directory),
+            game_root=game_root,
             mirrored=self.mirrored,
             night=self.night,
             weather=self.weather,
         )
         import_strategy: TrackImportStrategy
         if self.mode == "SIMPLE":
             import_strategy = TrackImportSimple(material_map=track.get_polygon_material)
```

### Comparing `speedtools-0.4.0/speedtools/frd_data.py` & `speedtools-0.5.0/speedtools/frd_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     high_poly_chunks = [
         False,  # Low-resolution track geometry
         False,  # Low-resolution misc geometry
         False,  # Medium-resolution track geometry
         False,  # Medium-resolution misc geometry
         True,  # High-resolution track geometry
         True,  # High-resolution misc geometry
-        False,  # Road lanes
+        True,  # Road lanes
         True,  # High-resolution misc geometry
         True,  # High-resolution misc geometry
         True,  # High-resolution misc geometry
         True,  # High-resolution misc geometry
     ]
 
     def __init__(self, parser: FrdParser) -> None:
@@ -66,23 +66,24 @@
         cls, face: Sequence[int], *iterables: Iterable[Any]
     ) -> Iterator[tuple[Any, ...]]:
         polygon_data_zipped = zip(face, *iterables)
         return unique_everseen(polygon_data_zipped, key=lambda x: nth(x, 0))
 
     @classmethod
     def _make_polygon(cls, polygon: FrdParser.Polygon) -> Polygon:
-        material = polygon.texture & 0x7FF
+        material = polygon.texture_id
         backface_culling = polygon.backface_culling
         quads_or_triangles = cls._validate_polygon(polygon.face, cls._texture_flags_to_uv(polygon))
         face, uv = unzip(quads_or_triangles)  # pylint: disable=unbalanced-tuple-unpacking
         return Polygon(
             face=tuple(face),
             uv=tuple(uv),
             material=material,
             backface_culling=backface_culling,
+            is_lane=polygon.lane,
         )
 
     @classmethod
     def _get_object_collision_type(
         cls, segment: Optional[FrdParser.SegmentData], obj: FrdParser.ObjectHeader
     ) -> CollisionType:
         logger.info(f"Object: {vars(obj)}")
```

### Comparing `speedtools-0.4.0/speedtools/qfs_data.py` & `speedtools-0.5.0/speedtools/fsh_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,47 +17,63 @@
 
 from speedtools.parsers import FshParser, QfsParser
 from speedtools.types import Bitmap, FshDataType, Resource
 
 logger = logging.getLogger(__name__)
 
 
-class QfsData:
-    def __init__(self, qfs_parser: QfsParser) -> None:
-        self.qfs = qfs_parser
+class FshData:
+    def __init__(self, fsh_parser: FshParser) -> None:
+        self.fsh = fsh_parser
 
     @classmethod
-    def from_file(cls, filename: Path) -> QfsData:
-        parser = QfsParser.from_file(filename=filename)
-        return cls(qfs_parser=parser)
+    def from_file(cls, filename: Path) -> FshData:
+        suffix = filename.suffix.lower()
+        if suffix == ".qfs":
+            parser = QfsParser.from_file(filename=filename).data
+        elif suffix == ".fsh":
+            parser = FshParser.from_file(filename=filename)
+        else:
+            raise ValueError("Invalid fsh file extension")
+        return cls(fsh_parser=parser)
 
     @classmethod
     def _get_data_by_code(
         cls, codes: Container[FshDataType], resource: FshParser.DataBlock
     ) -> Iterator[FshParser.DataBlock]:
         return filter(lambda x: x.code in codes, resource.body.blocks)
 
     @classmethod
     def _make_bitmap(cls, resource: FshParser.Resource) -> Bitmap:
         bitmap = one(
             cls._get_data_by_code(
-                codes=[FshDataType.bitmap8, FshDataType.bitmap32], resource=resource
+                codes=(
+                    FshDataType.bitmap8,
+                    FshDataType.bitmap32,
+                    FshDataType.bitmap16,
+                    FshDataType.bitmap16_alpha,
+                ),
+                resource=resource,
             )
         )
         if bitmap.code is FshDataType.bitmap8:
             palette = one(cls._get_data_by_code(codes=[FshDataType.palette], resource=resource))
             palette_colors = [element.color for element in palette.data.data]
             rgba_int = [palette_colors[element] for element in bitmap.data.data]
             rgba_bytes = pack(f"<{len(rgba_int)}I", *rgba_int)
             bitmap_object = Bitmap(
                 width=bitmap.width,
                 height=bitmap.height,
                 data=rgba_bytes,
             )
-        elif bitmap.code is FshDataType.bitmap32:
+        elif bitmap.code in (
+            FshDataType.bitmap32,
+            FshDataType.bitmap16,
+            FshDataType.bitmap16_alpha,
+        ):
             rgba_int = [elem.color for elem in bitmap.data.data]
             rgba_bytes = pack(f"<{len(rgba_int)}I", *rgba_int)
             bitmap_object = Bitmap(
                 width=bitmap.width,
                 height=bitmap.height,
                 data=rgba_bytes,
             )
@@ -79,8 +95,8 @@
             mirrored=mirrored,
             nonmirrored=nonmirrored,
             additive=additive,
         )
 
     @property
     def resources(self) -> Iterator[Resource]:
-        return map(self._make_resource, self.qfs.data.resources)
+        return map(self._make_resource, self.fsh.resources)
```

### Comparing `speedtools-0.4.0/speedtools/refpack.py` & `speedtools-0.5.0/speedtools/refpack.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/speedtools/specs/fce.ksy` & `speedtools-0.5.0/speedtools/specs/fce.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/speedtools/specs/frd.ksy` & `speedtools-0.5.0/speedtools/specs/frd.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/speedtools/specs/fsh.ksy` & `speedtools-0.5.0/speedtools/specs/fsh.ksy`

 * *Files 17% similar despite different names*

```diff
@@ -79,16 +79,18 @@
         type: u2
       - id: y_pos
         type: u2
       - id: data
         type:
           switch-on: _parent.code
           cases:
+            data_type::bitmap16: pixel_16_element
             data_type::bitmap8: u1
             data_type::bitmap32: pixel_32_element
+            data_type::bitmap16_alpha: pixel_16_alpha_element
             data_type::palette: palette_element
         repeat: expr
         repeat-expr: _parent.width * _parent.height
   pixel_32_element:
     seq:
       - id: value
         type: u4
@@ -101,14 +103,48 @@
       blue:
         value: (value >> 16) & 0xff
       alpha:
         value: (value >> 24) & 0xff
       color:
         value: 'blue + green * 0x100 + red * 0x10000 + alpha * 0x1000000'
         doc: ARGB color value
+  pixel_16_element:
+    seq:
+      - id: value
+        type: u2
+        doc: Raw 16-bit pixel value
+    instances:
+      red:
+        value: (value & 0x1f) * 8
+      green:
+        value: ((value >> 5) & 0x3f) * 4
+      blue:
+        value: ((value >> 11) & 0x1f) * 8
+      alpha:
+        value: 0xff
+      color:
+        value: 'blue + green * 0x100 + red * 0x10000  + alpha * 0x1000000'
+        doc: ARGB color value
+  pixel_16_alpha_element:
+    seq:
+      - id: value
+        type: u2
+        doc: Raw 16-bit pixel value
+    instances:
+      red:
+        value: (value & 0x1f) * 8
+      green:
+        value: ((value >> 5) & 0x1f) * 8
+      blue:
+        value: ((value >> 10) & 0x1f) * 8
+      alpha:
+        value: '(value & 0x8000) != 0 ? 0xff : 0'
+      color:
+        value: 'blue + green * 0x100 + red * 0x10000 + alpha * 0x1000000'
+        doc: ARGB color value
   palette_element:
     seq:
       - id: value
         type: u2
         doc: Raw palette value
     instances:
       red:
@@ -120,11 +156,13 @@
       alpha:
         value: '(value & 0x8000) != 0 ? 0xff : 0'
       color:
         value: 'blue + green * 0x100 + red * 0x10000 + alpha * 0x1000000'
         doc: ARGB color value
 enums:
   data_type:
+    0x78: bitmap16
     0x7b: bitmap8
     0x7d: bitmap32
+    0x7e: bitmap16_alpha
     0x2d: palette
     0x6f: text
```

### Comparing `speedtools-0.4.0/speedtools/specs/viv.ksy` & `speedtools-0.5.0/speedtools/specs/viv.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/speedtools/speedtool.py` & `speedtools-0.5.0/speedtools/speedtool.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 logger.addHandler(sh)
 
 
 @click.command()
 @click.option("--output", help="Output directory", type=click.Path())
 @click.argument("path", type=click.Path())
 def unpack(output: Path, path: Path) -> None:
-    data = TrackData(path)
+    data = TrackData(directory=path, game_root=path.parent.parent.parent)
     nonmirrored = filter(lambda x: not x.mirrored, data.track_resources)
     export_resource(nonmirrored, directory=output)
 
 
 @click.command()
 @click.option("--output", help="Output directory", type=click.Path())
 @click.argument("path", type=click.Path())
 def mesh(output: Path, path: Path) -> None:
     with suppress(FileExistsError):
         os.makedirs(output)
-    data = TrackData(path)
+    data = TrackData(directory=path, game_root=path.parent.parent.parent)
     materials = set()
     for index, obj in enumerate(data.objects):
         with open(Path(output, f"object_{index}.obj"), "w", encoding="utf-8") as obj_file:
             obj_file.write(f"mtllib materials_{index}.mtl{os.linesep}")
             for vertex in obj.mesh.vertices:
                 obj_file.write(f"v {vertex.x} {vertex.y} {vertex.z}{os.linesep}")
             for i, polygon in enumerate(obj.mesh.polygons):
```

### Comparing `speedtools-0.4.0/speedtools/tr_ini.py` & `speedtools-0.5.0/speedtools/tr_ini.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/speedtools/track_data.py` & `speedtools-0.5.0/speedtools/track_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from collections.abc import Callable, Iterator
 from contextlib import suppress
 from math import atan2, cos, tau
 from pathlib import Path
 from typing import TypeVar
 
 from speedtools.frd_data import FrdData
-from speedtools.qfs_data import QfsData
+from speedtools.fsh_data import FshData
 from speedtools.tr_ini import TrackIni
 from speedtools.types import (
     DirectionalLight,
     Light,
     LightAttributes,
     LightStub,
     Polygon,
@@ -30,39 +30,45 @@
 logger = logging.getLogger(__name__)
 T = TypeVar("T")
 
 
 class TrackData:
     SUN_DISTANCE = 3000
     ANIMATION_FPS = 64
+    SFX_RESOURCE_FILE = "Data/GAMEART/SFX.FSH"
 
     def __init__(
-        self, directory: Path, mirrored: bool = False, night: bool = False, weather: bool = False
+        self,
+        directory: Path,
+        game_root: Path,
+        mirrored: bool = False,
+        night: bool = False,
+        weather: bool = False,
     ) -> None:
         logger.debug(f"Opening directory {directory}")
         self.frd: FrdData = self.tr_open(
             constructor=FrdData.from_file,
             directory=directory,
             prefix="TR",
             postfix=".FRD",
             mirrored=mirrored,
             night=night,
             weather=weather,
         )
-        self.qfs: QfsData = self.tr_open(
-            constructor=QfsData.from_file,
+        self.qfs: FshData = self.tr_open(
+            constructor=FshData.from_file,
             directory=directory,
             prefix="TR",
             postfix="0.QFS",
             mirrored=mirrored,
             night=night,
             weather=weather,
         )
-        self.sky: QfsData = self.tr_open(
-            constructor=QfsData.from_file,
+        self.sky: FshData = self.tr_open(
+            constructor=FshData.from_file,
             directory=directory,
             prefix="SKY",
             postfix=".QFS",
             mirrored=mirrored,
             night=night,
             weather=weather,
         )
@@ -71,15 +77,17 @@
             directory=directory,
             prefix="TR",
             postfix=".INI",
             mirrored=mirrored,
             night=night,
             weather=weather,
         )
+        self.sfx: FshData = FshData.from_file(Path(game_root, self.SFX_RESOURCE_FILE))
         self.resources: dict[int, Resource] = {}
+        self.sfx_resources: dict[str, Resource] = {}
         self.light_glows: dict[int, LightAttributes] = {}
         self.mirrored: bool = mirrored
         self.night: bool = night
         self.weather: bool = weather
 
     @classmethod
     def tr_open(
@@ -134,19 +142,23 @@
             resources = filter(lambda resource: not resource.nonmirrored, self.qfs.resources)
         else:
             resources = filter(lambda resource: not resource.mirrored, self.qfs.resources)
         unique_named_resources = count_repeats_and_map(
             iterable=resources, func=self._make_unique_resource_name, key=lambda x: x.name
         )
         self.resources = dict(enumerate(unique_named_resources))
+        self.sfx_resources = {res.name: res for res in self.sfx.resources}
 
     def get_polygon_material(self, polygon: Polygon) -> Resource:
+        mat = polygon.material
         if not self.resources:
             self._init_resources()
-        return self.resources[polygon.material]
+        if polygon.is_lane:
+            return self.sfx_resources[f"lin{mat}"]
+        return self.resources[mat]
 
     def _make_light(self, stub: LightStub) -> Light:
         attributes = self.light_glows[stub.glow_id]
         return Light(location=stub.location, attributes=attributes)
 
     @property
     def lights(self) -> Iterator[Light]:
```

### Comparing `speedtools-0.4.0/speedtools/types.py` & `speedtools-0.5.0/speedtools/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 
 @dataclass(frozen=True)
 class Polygon(BasePolygon):
     face: tuple[int, ...]
     uv: tuple[UV, ...]
     material: int
     backface_culling: bool
+    is_lane: bool = False
 
 
 @dataclass(frozen=True)
 class Animation:
     length: int
     delay: int
     locations: Sequence[Vector3d]
```

### Comparing `speedtools-0.4.0/speedtools/utils.py` & `speedtools-0.5.0/speedtools/utils.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/speedtools/viv_data.py` & `speedtools-0.5.0/speedtools/viv_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.4.0/speedtools.egg-info/PKG-INFO` & `speedtools-0.5.0/speedtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.4.0
+Version: 0.5.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -59,13 +59,12 @@
 * [Kaitai Struct compiler][3]
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
-* Road lanes are missing
 * The bear has left the park!
 
 [1]: https://pypi.org/project/speedtools/
 [2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.4.0/speedtools.egg-info/SOURCES.txt` & `speedtools-0.5.0/speedtools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 speedtools/__init__.py
 speedtools/frd_data.py
-speedtools/qfs_data.py
+speedtools/fsh_data.py
 speedtools/refpack.py
 speedtools/speedtool.py
 speedtools/tr_ini.py
 speedtools/track_data.py
 speedtools/types.py
 speedtools/utils.py
 speedtools/viv_data.py
```

