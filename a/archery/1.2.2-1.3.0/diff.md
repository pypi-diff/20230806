# Comparing `tmp/archery-1.2.2.tar.gz` & `tmp/archery-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/archery-1.2.2.tar", last modified: Thu Nov  1 13:12:28 2018, max compression
+gzip compressed data, was "archery-1.3.0.tar", last modified: Sun Aug  6 19:22:23 2023, max compression
```

## Comparing `archery-1.2.2.tar` & `archery-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 jul       (1000) jul       (1000)        0 2018-11-01 13:12:28.000000 archery-1.2.2/
--rw-r--r--   0 jul       (1000) jul       (1000)    12223 2018-10-30 14:27:57.000000 archery-1.2.2/consistent_algebrae.py
--rw-r--r--   0 jul       (1000) jul       (1000)     1840 2018-10-30 14:47:33.000000 archery-1.2.2/setup.py
-drwxr-xr-x   0 jul       (1000) jul       (1000)        0 2018-11-01 13:12:28.000000 archery-1.2.2/archery/
--rw-r--r--   0 jul       (1000) jul       (1000)      438 2018-11-01 13:11:36.000000 archery-1.2.2/archery/__init__.py
--rw-r--r--   0 jul       (1000) jul       (1000)     3940 2018-10-30 14:09:43.000000 archery-1.2.2/archery/barrack.py
--rw-r--r--   0 jul       (1000) jul       (1000)     7332 2018-11-01 12:23:31.000000 archery-1.2.2/archery/trait.py
--rw-r--r--   0 jul       (1000) jul       (1000)    10832 2018-11-01 11:58:36.000000 archery-1.2.2/archery/test_archery.py
--rw-r--r--   0 jul       (1000) jul       (1000)     2531 2018-11-01 12:25:01.000000 archery-1.2.2/archery/bow.py
--rw-r--r--   0 jul       (1000) jul       (1000)      839 2018-11-01 12:06:57.000000 archery-1.2.2/archery/quiver.py
--rw-r--r--   0 jul       (1000) jul       (1000)      985 2018-10-30 14:13:19.000000 archery-1.2.2/archery/test_fun.py
--rw-r--r--   0 jul       (1000) jul       (1000)     5284 2018-11-01 13:07:27.000000 archery-1.2.2/README.txt
--rw-r--r--   0 jul       (1000) jul       (1000)     7630 2018-11-01 13:12:28.000000 archery-1.2.2/PKG-INFO
--rw-r--r--   0 jul       (1000) jul       (1000)     9469 2018-10-30 14:27:57.000000 archery-1.2.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 19:22:23.751074 archery-1.3.0/
+-rw-rw-rw-   0        0        0     9469 2017-01-14 21:46:12.000000 archery-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       82 2017-01-14 21:46:12.000000 archery-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6586 2023-08-06 19:22:23.750074 archery-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2018-11-07 21:59:34.000000 archery-1.3.0/README.rst
+-rw-rw-rw-   0        0        0     5284 2018-11-07 21:59:38.000000 archery-1.3.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 19:22:23.717054 archery-1.3.0/archery/
+-rw-rw-rw-   0        0        0      438 2023-08-06 19:20:50.000000 archery-1.3.0/archery/__init__.py
+-rw-rw-rw-   0        0        0     4017 2023-08-06 19:04:55.000000 archery-1.3.0/archery/barrack.py
+-rw-rw-rw-   0        0        0     2608 2023-08-06 19:05:50.000000 archery-1.3.0/archery/bow.py
+-rw-rw-rw-   0        0        0      839 2018-11-07 21:59:38.000000 archery-1.3.0/archery/quiver.py
+-rw-rw-rw-   0        0        0    11364 2023-08-06 18:47:52.000000 archery-1.3.0/archery/test_archery.py
+-rw-rw-rw-   0        0        0      985 2018-11-07 21:59:38.000000 archery-1.3.0/archery/test_fun.py
+-rw-rw-rw-   0        0        0     7677 2023-08-06 19:03:54.000000 archery-1.3.0/archery/trait.py
+drwxrwxrwx   0        0        0        0 2023-08-06 19:22:23.738066 archery-1.3.0/archery.egg-info/
+-rw-rw-rw-   0        0        0     6586 2023-08-06 19:22:23.000000 archery-1.3.0/archery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-08-06 19:22:23.000000 archery-1.3.0/archery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 19:22:23.000000 archery-1.3.0/archery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-06 19:22:23.000000 archery-1.3.0/archery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12223 2018-11-07 21:59:38.000000 archery-1.3.0/consistent_algebrae.py
+-rw-rw-rw-   0        0        0       42 2023-08-06 19:22:23.752075 archery-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2682 2023-08-06 19:07:12.000000 archery-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `archery-1.2.2/consistent_algebrae.py` & `archery-1.3.0/consistent_algebrae.py`

 * *Files identical despite different names*

### Comparing `archery-1.2.2/setup.py` & `archery-1.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,82 @@
-#!/usr/bin/env python
-# -*- coding: "utf-8" -*-
-
-#from setuptools import setup, find_packages
-#import unittest
-#import sys
-from distutils.command.build_py import build_py as _build_py
-from distutils.core import setup
-from archery import __version__
-from archery import __author__
-from archery import __author_email__
-import unittest
-import sys
-
-def test():
-    """Specialized Python source builder."""
-    from archery import test_archery
-    loader= unittest.TestLoader()
-    suite=loader.loadTestsFromModule(test_archery)
-    runner=unittest.TextTestRunner()
-    result=runner.run(suite)
-    if  not result.wasSuccessful():
-        raise Exception( "Test Failed: Aborting install")
-
-if "install" in sys.argv or "sdist" in sys.argv or "update" in sys.argv:
-    test()
-
-setup(
-        name='archery',
-        version=__version__,
-        author=__author__,
-        author_email=__author_email__,
-        packages=['archery'],
-        url='http://archery.readthedocs.org/',
-        license="Python Software Foundation License",
-        description='Traits (Mixins) to give +,/,-,* to MutableMapping ',
-        long_description=open("README.txt").read(),
-        requires=[ ],
-        classifiers=[
-          'Development Status :: 5 - Production/Stable',
-          'License :: OSI Approved :: Python Software Foundation License',
-          'Programming Language :: Python :: 2.7',
-          'Programming Language :: Python :: 3.3',
-          'Programming Language :: Python :: 3.4',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 3',
-          'Operating System :: OS Independent',
-          'Programming Language :: Python',
-          ],
-)
+#!/usr/bin/env python
+# -*- coding: "utf-8" -*-
+
+#from setuptools import setup, find_packages
+#import unittest
+#import sys
+from distutils.command.build_py import build_py as _build_py
+from distutils.core import setup
+from distutils.cmd import Command
+from archery import __version__
+from archery import __author__
+from archery import __author_email__
+import unittest
+import sys
+
+class Test(Command):
+  """A custom command to run Pylint on all Python source files."""
+  def initialize_options(self):
+    """Set default values for options."""
+    self.verbosity=1
+    pass
+
+  def finalize_options(self):
+    """Post-process options."""
+    pass
+
+  description = 'test the module'
+  user_options = [
+  ('verbosity=', 'V', 'verbosity level'),
+  ]
+
+
+  def run(self):
+    """Run command."""
+    test(int(self.verbosity))
+
+def test(verbosity=1):
+    """Specialized Python source builder."""
+    from archery import test_archery
+    loader= unittest.TestLoader()
+    suite=loader.loadTestsFromModule(test_archery)
+    runner=unittest.TextTestRunner(verbosity=verbosity)
+    result=runner.run(suite)
+    if  not result.wasSuccessful():
+        raise Exception( "Test Failed: Aborting install")
+
+if "install" in sys.argv or "sdist" in sys.argv or "update" in sys.argv:
+    test()
+
+setup(
+        cmdclass=dict(
+        test=Test,
+        ),
+        name='archery',
+        version=__version__,
+        author=__author__,
+        author_email=__author_email__,
+        packages=['archery'],
+        url='http://archery.readthedocs.org/',
+        license="Python Software Foundation License",
+        description='Traits (Mixins) to give +,/,-,* to MutableMapping ',
+        long_description=open("README.txt").read(),
+        requires=[ ],
+        classifiers=[
+          'Development Status :: 5 - Production/Stable',
+          'License :: OSI Approved :: Python Software Foundation License',
+          'Programming Language :: Python :: 2.7',
+          'Programming Language :: Python :: 3.3',
+          'Programming Language :: Python :: 3.4',
+          'Programming Language :: Python :: 3.5',
+          'Programming Language :: Python :: 3.6',
+          'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
+          'Programming Language :: Python :: 2',
+          'Programming Language :: Python :: 3',
+          'Operating System :: OS Independent',
+          'Programming Language :: Python',
+          ],
+)
```

### Comparing `archery-1.2.2/archery/barrack.py` & `archery-1.3.0/archery/barrack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 Traits / mixins are the heart of archery, but sometimes you need functions to help you
 
 """
-from collections import MutableMapping
+try:
+    from collections import MutableMapping
+except ImportError:
+    from collections.abc import MutableMapping
+
 
 MARKER=object()
 
 class Path(tuple):
     def endswith( self, *a_tuple ):
         """check if path ends with the consecutive given has argumenbts value
```

### Comparing `archery-1.2.2/archery/test_archery.py` & `archery-1.3.0/archery/test_archery.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,380 +1,386 @@
-#/usr/bin/env python
-import os
-import sys
-
-import warnings
-import unittest
-from  archery.bow import Hankyu, Daikyu, sdict, vdict, mdict, edict
-from archery.barrack import bowyer, Path, make_from_path, paired_row_iter
-
-from math import sqrt, cos, pi, sin, acos
-
-class TestDeprecation(unittest.TestCase):
-    def test_deprec_edict(self):
-        """ edict (ExpDict is becoming searchable """
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter('always')
-            edict(x=1)
-            self.assertTrue(
-                issubclass(w[-1].category, DeprecationWarning),
-            )
-
-class TestKyleExpectation(unittest.TestCase):
-
-    def test_commutativity(self):
-        a = mdict({"a": 1, "y": {"b": 4, "c": [5]}})
-        b=  mdict({"a": 1, "x": 5, "y": {"b": 6, "c": [12]}})
-        expected_ab = {"a": 2, "x": 5, "y": {"b": 10, "c": [5, 12]}}
-        expected_ba = {"a": 2, "x": 5, "y": {"b": 10, "c": [12, 5]}}
-        self.assertEqual(a + b, expected_ab)
-        a = mdict({"a": 1, "y": mdict({"b": 4, "c": [5]})})
-        b=  mdict({"a": 1, "x": 5, "y": mdict({"b": 6, "c": [12]})})
-        self.assertEqual(b + a, expected_ba)
-        a = mdict({"a": 1, "y": mdict({"b": 4, "c": [5]})})
-        b=  mdict({"a": 1, "x": 5, "y": mdict({"b": 6, "c": [12]})})
-        a += b
-        self.assertEqual(a, expected_ab)
-
-
-    def test_bug_iadd(self):
-        a = mdict({"a": 1, "y": mdict({"b": 4, "c": [5]})})
-        b=  mdict({"a": 1, "x": 5, "y": mdict({"b": 6, "c": [12]})})
-        expected_ab = {"a": 2, "x": 5, "y": {"b": 10, "c": [5, 12]}}
-        expected_ba = {"a": 2, "x": 5, "y": {"b": 10, "c": [12, 5]}}
-        self.assertEqual(a + b, expected_ab)
-        self.assertEqual(b + a, expected_ba)
-        a += b
-        self.assertEqual(a, expected_ab)
-
-
-class TestVectorDict(unittest.TestCase):
-    """test a dict with Vector properies (cos, dot, abs)"""
-
-    def setUp(self):
-        self.point = vdict( x=3, y=3, z=0)
-        self.point2 = vdict( x=1, y=1, z=1)
-    
-    def testNorm(self):
-        self.assertAlmostEqual(
-                abs(self.point),
-                sqrt(3*3+3*3)
-        )
-    def testCos(self):
-        self.assertAlmostEqual(
-                vdict(x=1,y=0).cos(vdict(x=1,y=1)),
-                cos(pi/4)
-        )
-
-class TestBarrack(unittest.TestCase):
-    def test_path(self):
-        self.assertEqual(
-            Path(("a","b",1)).key(),
-            ("a","b")
-        )
-        self.assertFalse(
-            Path(("a","b",1)).contains("a","b","c")
-        )
-        self.assertEqual(
-            Path(("a","b",1)).value(),
-            1
-        )
-        self.assertTrue(Path(("x", "y", 1)).startswith("x"))
-        self.assertTrue(Path(("s", "x", "y", 1)).contains("x","y"))
-
-    def test_paired_row_iter(self):
-        self.assertEqual(set(paired_row_iter(dict(x=1, a=dict(b=dict(c=1))))),
-            { (("x",),1), (("a","b","c"), 1)}
-        )
-
-
-class TestBugWeired(unittest.TestCase):
-
-    def test_stay_same(self):
-
-        class Matrix(mdict):
-            def __call__(self, other):
-                other = other.copy()
-                res= vdict()
-                for (src, dst), functor in self.items():
-                    res += mdict({ dst: functor(other[src])})
-                return res
-
-
-        theta = pi/6
-
-        u = mdict(x=1, y=2)
-        v = mdict(x=1, y=0)
-        alien = vdict(x=u, y=v)
-
-        def rotation_maker(theta):
-            """"Matrix takes as key (SRC, DST) (which is the opposite of "actual notation")
-            """
-            return Matrix({
-                ("x", "x") : lambda v:1.0 *  v * cos(theta),
-                ("y", "x") : lambda v:1.0 * -v * sin(theta),
-                ("x", "y") : lambda v:1.0 *  v * sin(theta),
-                ("y", "y") : lambda v:1.0 *  v * cos(theta)
-            })
-
-        rotation = rotation_maker(pi/6)
-        self.assertAlmostEqual(
-            rotation(u),
-            {'x': -0.13397459621556118, 'y': 2.232050807568877}
-            )
-# OUT:{'x': 1, 'y': 0}
-        self.assertAlmostEqual(rotation(v),
-            {'x': 0.8660254037844387, 'y': 0.49999999999999994}
-        )
-        self.assertAlmostEqual(
-            acos(vdict(u).cos(vdict(rotation(u))))/2 / pi * 360,
-            29.999999999999993
-        )
-        self.assertEqual(u, dict(x=1, y=2))
-        self.assertAlmostEqual(acos(vdict(v).cos(vdict(rotation_maker(pi/3)(v))))/2 / pi * 360,
-60.0)
-        self.assertAlmostEqual(
-            acos(vdict(v).cos(vdict(rotation_maker(pi/5)(v))))/2 / pi * 360,
-            36.0
-        )
-        self.assertEqual(
-            alien,
-            {'x': {'x': 1, 'y': 2}, 'y': {'x': 1, 'y': 0}}
-        )
-        """
-        undefined behaviour until I can make a sense of this
-
-
-
-        self.assertAlmostEqual(
-            rotation_maker(pi/4)(alien),
-            {
-                'x': {'x': 1.1102230246251565e-16, 'y': 1.4142135623730951},
-                'y': {'x': -1.1102230246251565e-16, 'y': 1.414213562373095}
-            }
-        )
-        self.assertAlmostEqual(
-            acos(alien.cos(rotation_maker(pi/4)(alien)))/2 / pi * 360,
-            54.73561031724534
-        )
-
-        self.assertAlmostEqual(rotation_maker(pi/4)(alien),
-            {'x':
-                {'x': 1.1102230246251565e-16, 'y': 1.4142135623730951},
-             'y': {'x': -1.1102230246251565e-16, 'y': 1.414213562373095}})
-        """
-
-
-class TestSearchableDict(unittest.TestCase):
-    def setUp(self):
-        self.easy = vdict( x=1, y=1, z=0)
-        
-        self.tree = sdict(
-            a = 1,
-            b = dict(
-                c = 3.0,
-                d = dict(e=True)
-            ),
-            point = self.easy
-        )
-
-    def test_rec_type(self):
-        """test that if created with another mutale mapping
-        does not converts it on the fly to himself"""
-        self.assertNotEqual(
-            type(self.tree["point"]),
-            sdict
-        )
-
-    def test_search(self):
-        self.assertEqual(
-                set([ x for x in self.tree.search(
-                    lambda x : Path(x).contains("point","x") 
-                        or Path(x).endswith(3.0)
-                    )
-                ]),
-                set([('b', 'c', 3.0), ('point', 'x', 1)])
-        )
-        self.assertEqual(
-                set([ x for x in self.tree.search(
-                    lambda x : Path(x).startswith("a")
-                    )
-                ]),
-                set([('a', 1)])
-        )
-
-    def test_leaf_search(self):
-        self.assertEqual(
-                [ i for i in self.tree.leaf_search(lambda x : type(x) is  float)],
-                [ 3.0 ]
-        )
-        self.assertEqual(
-                [ i for i in self.tree.leaf_search(lambda x : type(x) is  bool)],
-                [ True ]
-        )
-        
-
-
-        
-
-class TestHankyu(unittest.TestCase):
-    def setUp(self):
-        self.easy = Hankyu( x=1, y=1, z=0)
-        self.easy_too = Hankyu( x=0, y=-2, o=0)
-        
-        self.a_tree = dict(
-            a = 1,
-            b = dict(
-                c = 3.0,
-                d = dict(e=True)
-            ),
-            point = self.easy
-        )
-        self.cplx = bowyer(Hankyu,self.a_tree)
-
-    def test_convert(self):
-        self.assertEqual(
-            bowyer(Hankyu, {'a': {'b': 1}}),
-            Hankyu( {'a': Hankyu(b=1)})
-            )
-        
-
-    def test_add_not_exists(self):
-        self.easy += dict(a=1)
-        self.assertEqual(self.easy['a'], 1)
-        self.assertEqual(
-                self.easy + self.easy_too, 
-                sum([ self.easy_too, self.easy])
-        )
-
-    def test_add_exists(self):
-        self.easy += dict(x=1)
-        self.assertEqual(self.easy['x'] , 2)
-
-    def test_number_inc(self):
-        self.easy += 1
-        self.assertEqual(self.easy['x'] , 2)
-
-
-    def test_bug_convert_empty_mapping(self):
-        """bug #8 : empty mapping intialisation dont work"""
-        bug = bowyer( Hankyu,dict( a={}))
-        expected = Hankyu( {'a': {}})
-        self.assertEqual(
-            expected,
-            bug
-        )
-
-class TestDaikyu(unittest.TestCase):
-    def setUp(self):
-        self.easy = Daikyu( x=1, y=1, z=0)
-        self.easy_too = Daikyu( x=0, y=-2, o=0)
-        
-        self.a_tree = dict(
-            a = 1,
-            b = dict(
-                c = 3.0,
-                d = dict(e=True)
-            ),
-            point = self.easy
-        )
-        self.cplx = bowyer(Daikyu,self.a_tree)
-
-
-    def test_bug_1(self):
-        """bug  #1 : * returns a copy where a reference is needed"""
-        pt = self.easy
-        pt *= -1
-        self.assertEqual(
-            self.easy,
-            pt
-        )
-    def test_bug_2(self):
-        """bug #2 : self * other without affectation should not modify self.
-        """
-        self.easy *= -1
-        a_copy = self.easy.copy()
-        self.easy * a_copy
-        self.assertEqual(
-            self.easy,
-            a_copy
-        )
-
-
-    def test_bug_4(self):
-        """bug #4 : self / other without affectation should not modify self.
-        """
-        del(self.easy['z'])
-        self.easy /= -1
-        a_copy = self.easy.copy()
-        self.easy / a_copy
-        self.assertEqual(
-            self.easy,
-            a_copy
-        )
-
-    def test_bug_5(self):
-        """bug #5 : int * dict without affectation should not modify self.
-        """
-        a_copy = self.easy.copy()
-        2 * self.easy
-        self.assertEqual(
-            self.easy,
-            a_copy
-        )
-
-    def test_bug_6(self):
-        """bug #6 : int / dict without affectation should not modify self.
-        """
-        del(self.easy['z'])
-        a_copy = self.easy.copy()
-        2.0 / self.easy
-        self.assertEqual(
-            self.easy,
-            a_copy
-        )
-
-
-    def test_for_fun(self):
-        """just for fun """
-        a = self.easy
-        b = self.easy_too
-        aa = a.copy()
-        bb = b.copy()
-        self.assertEqual(
-            (a - b) * (a + b),
-            aa * aa - bb * bb
-        )
-
-
-    def test_for_fun2(self):
-        """just for fun """
-        a = self.easy
-        b = self.easy_too
-        aa = a.copy()
-        bb = b.copy()
-        self.assertEqual(
-            -(a + b) * (a + b),
-            -1 * ((aa * aa) + 2 * aa * bb + (bb * bb))
-        )
-    
-    def test_dyslexia_bug4(self):
-        """counfonding right & left in all r(div/add/sub/mul) operator """
-        a = self.easy
-        self.assertEqual(
-            2/Daikyu({'a':1}),
-            {'a' : 2}
-        )
-        self.assertEqual(
-            2-a,
-            -(a-2)
-        )
-    def test_inplace_bug5(self):
-        """a/b in place"""
-        a = self.easy*4
-        self.assertEqual(
-            a/{'x':2},
-            {'x' : 2}
-        )
-
-if __name__ == '__main__':
-    unittest.main(verbosity=4)
+#/usr/bin/env python
+import os
+import sys
+
+import warnings
+import unittest
+from  archery.bow import Hankyu, Daikyu, sdict, vdict, mdict, edict
+from archery.barrack import bowyer, Path, make_from_path, paired_row_iter
+
+from math import sqrt, cos, pi, sin, acos
+
+class TestDeprecation(unittest.TestCase):
+    def test_deprec_edict(self):
+        """ edict (ExpDict is becoming searchable """
+        with warnings.catch_warnings(record=True) as w:
+            warnings.simplefilter('always')
+            edict(x=1)
+            self.assertTrue(
+                issubclass(w[-1].category, DeprecationWarning),
+            )
+
+class TestKyleExpectation(unittest.TestCase):
+
+    def test_commutativity(self):
+        a = mdict({"a": 1, "y": {"b": 4, "c": [5]}})
+        b=  mdict({"a": 1, "x": 5, "y": {"b": 6, "c": [12]}})
+        expected_ab = {"a": 2, "x": 5, "y": {"b": 10, "c": [5, 12]}}
+        expected_ba = {"a": 2, "x": 5, "y": {"b": 10, "c": [12, 5]}}
+        self.assertEqual(a + b, expected_ab)
+        a = mdict({"a": 1, "y": mdict({"b": 4, "c": [5]})})
+        b=  mdict({"a": 1, "x": 5, "y": mdict({"b": 6, "c": [12]})})
+        self.assertEqual(b + a, expected_ba)
+        a = mdict({"a": 1, "y": mdict({"b": 4, "c": [5]})})
+        b=  mdict({"a": 1, "x": 5, "y": mdict({"b": 6, "c": [12]})})
+        a += b
+        self.assertEqual(a, expected_ab)
+
+
+    def test_bug_iadd(self):
+        a = mdict({"a": 1, "y": mdict({"b": 4, "c": [5]})})
+        c = mdict({"a": 1, "y": mdict({"b": 4, "c": 5})})
+        b=  mdict({"a": 1, "x": 5, "y": mdict({"b": 6, "c": [12]})})
+        expected_ab = {"a": 2, "x": 5, "y": {"b": 10, "c": [5, 12]}}
+        expected_ba = {"a": 2, "x": 5, "y": {"b": 10, "c": [12, 5]}}
+        self.assertEqual(a + b, expected_ab)
+        self.assertEqual(b + a, expected_ba)
+        a += b
+        c+=1
+        d=c.copy()
+        e=4
+        e+=c
+        self.assertEqual(c, d)
+        self.assertEqual(a, expected_ab)
+
+
+class TestVectorDict(unittest.TestCase):
+    """test a dict with Vector properies (cos, dot, abs)"""
+
+    def setUp(self):
+        self.point = vdict( x=3, y=3, z=0)
+        self.point2 = vdict( x=1, y=1, z=1)
+    
+    def testNorm(self):
+        self.assertAlmostEqual(
+                abs(self.point),
+                sqrt(3*3+3*3)
+        )
+    def testCos(self):
+        self.assertAlmostEqual(
+                vdict(x=1,y=0).cos(vdict(x=1,y=1)),
+                cos(pi/4)
+        )
+
+class TestBarrack(unittest.TestCase):
+    def test_path(self):
+        self.assertEqual(
+            Path(("a","b",1)).key(),
+            ("a","b")
+        )
+        self.assertFalse(
+            Path(("a","b",1)).contains("a","b","c")
+        )
+        self.assertEqual(
+            Path(("a","b",1)).value(),
+            1
+        )
+        self.assertTrue(Path(("x", "y", 1)).startswith("x"))
+        self.assertTrue(Path(("s", "x", "y", 1)).contains("x","y"))
+
+    def test_paired_row_iter(self):
+        self.assertEqual(set(paired_row_iter(dict(x=1, a=dict(b=dict(c=1))))),
+            { (("x",),1), (("a","b","c"), 1)}
+        )
+
+
+class TestBugWeired(unittest.TestCase):
+
+    def test_stay_same(self):
+
+        class Matrix(mdict):
+            def __call__(self, other):
+                other = other.copy()
+                res= vdict()
+                for (src, dst), functor in self.items():
+                    res += mdict({ dst: functor(other[src])})
+                return res
+
+
+        theta = pi/6
+
+        u = mdict(x=1, y=2)
+        v = mdict(x=1, y=0)
+        alien = vdict(x=u, y=v)
+
+        def rotation_maker(theta):
+            """"Matrix takes as key (SRC, DST) (which is the opposite of "actual notation")
+            """
+            return Matrix({
+                ("x", "x") : lambda v:1.0 *  v * cos(theta),
+                ("y", "x") : lambda v:1.0 * -v * sin(theta),
+                ("x", "y") : lambda v:1.0 *  v * sin(theta),
+                ("y", "y") : lambda v:1.0 *  v * cos(theta)
+            })
+
+        rotation = rotation_maker(pi/6)
+        self.assertAlmostEqual(
+            rotation(u),
+            {'x': -0.13397459621556118, 'y': 2.232050807568877}
+            )
+# OUT:{'x': 1, 'y': 0}
+        self.assertAlmostEqual(rotation(v),
+            {'x': 0.8660254037844387, 'y': 0.49999999999999994}
+        )
+        self.assertAlmostEqual(
+            acos(vdict(u).cos(vdict(rotation(u))))/2 / pi * 360,
+            29.999999999999993
+        )
+        self.assertEqual(u, dict(x=1, y=2))
+        self.assertAlmostEqual(acos(vdict(v).cos(vdict(rotation_maker(pi/3)(v))))/2 / pi * 360,
+60.0)
+        self.assertAlmostEqual(
+            acos(vdict(v).cos(vdict(rotation_maker(pi/5)(v))))/2 / pi * 360,
+            36.0
+        )
+        self.assertEqual(
+            alien,
+            {'x': {'x': 1, 'y': 2}, 'y': {'x': 1, 'y': 0}}
+        )
+        """
+        undefined behaviour until I can make a sense of this
+
+
+
+        self.assertAlmostEqual(
+            rotation_maker(pi/4)(alien),
+            {
+                'x': {'x': 1.1102230246251565e-16, 'y': 1.4142135623730951},
+                'y': {'x': -1.1102230246251565e-16, 'y': 1.414213562373095}
+            }
+        )
+        self.assertAlmostEqual(
+            acos(alien.cos(rotation_maker(pi/4)(alien)))/2 / pi * 360,
+            54.73561031724534
+        )
+
+        self.assertAlmostEqual(rotation_maker(pi/4)(alien),
+            {'x':
+                {'x': 1.1102230246251565e-16, 'y': 1.4142135623730951},
+             'y': {'x': -1.1102230246251565e-16, 'y': 1.414213562373095}})
+        """
+
+
+class TestSearchableDict(unittest.TestCase):
+    def setUp(self):
+        self.easy = vdict( x=1, y=1, z=0)
+        
+        self.tree = sdict(
+            a = 1,
+            b = dict(
+                c = 3.0,
+                d = dict(e=True)
+            ),
+            point = self.easy
+        )
+
+    def test_rec_type(self):
+        """test that if created with another mutale mapping
+        does not converts it on the fly to himself"""
+        self.assertNotEqual(
+            type(self.tree["point"]),
+            sdict
+        )
+
+    def test_search(self):
+        self.assertEqual(
+                set([ x for x in self.tree.search(
+                    lambda x : Path(x).contains("point","x") 
+                        or Path(x).endswith(3.0)
+                    )
+                ]),
+                set([('b', 'c', 3.0), ('point', 'x', 1)])
+        )
+        self.assertEqual(
+                set([ x for x in self.tree.search(
+                    lambda x : Path(x).startswith("a")
+                    )
+                ]),
+                set([('a', 1)])
+        )
+
+    def test_leaf_search(self):
+        self.assertEqual(
+                [ i for i in self.tree.leaf_search(lambda x : type(x) is  float)],
+                [ 3.0 ]
+        )
+        self.assertEqual(
+                [ i for i in self.tree.leaf_search(lambda x : type(x) is  bool)],
+                [ True ]
+        )
+        
+
+
+        
+
+class TestHankyu(unittest.TestCase):
+    def setUp(self):
+        self.easy = Hankyu( x=1, y=1, z=0)
+        self.easy_too = Hankyu( x=0, y=-2, o=0)
+        
+        self.a_tree = dict(
+            a = 1,
+            b = dict(
+                c = 3.0,
+                d = dict(e=True)
+            ),
+            point = self.easy
+        )
+        self.cplx = bowyer(Hankyu,self.a_tree)
+
+    def test_convert(self):
+        self.assertEqual(
+            bowyer(Hankyu, {'a': {'b': 1}}),
+            Hankyu( {'a': Hankyu(b=1)})
+            )
+        
+
+    def test_add_not_exists(self):
+        self.easy += dict(a=1)
+        self.assertEqual(self.easy['a'], 1)
+        self.assertEqual(
+                self.easy + self.easy_too, 
+                sum([ self.easy_too, self.easy])
+        )
+
+    def test_add_exists(self):
+        self.easy += dict(x=1)
+        self.assertEqual(self.easy['x'] , 2)
+
+    def test_number_inc(self):
+        self.easy += 1
+        self.assertEqual(self.easy['x'] , 2)
+
+
+    def test_bug_convert_empty_mapping(self):
+        """bug #8 : empty mapping intialisation dont work"""
+        bug = bowyer( Hankyu,dict( a={}))
+        expected = Hankyu( {'a': {}})
+        self.assertEqual(
+            expected,
+            bug
+        )
+
+class TestDaikyu(unittest.TestCase):
+    def setUp(self):
+        self.easy = Daikyu( x=1, y=1, z=0)
+        self.easy_too = Daikyu( x=0, y=-2, o=0)
+        
+        self.a_tree = dict(
+            a = 1,
+            b = dict(
+                c = 3.0,
+                d = dict(e=True)
+            ),
+            point = self.easy
+        )
+        self.cplx = bowyer(Daikyu,self.a_tree)
+
+
+    def test_bug_1(self):
+        """bug  #1 : * returns a copy where a reference is needed"""
+        pt = self.easy
+        pt *= -1
+        self.assertEqual(
+            self.easy,
+            pt
+        )
+    def test_bug_2(self):
+        """bug #2 : self * other without affectation should not modify self.
+        """
+        self.easy *= -1
+        a_copy = self.easy.copy()
+        self.easy * a_copy
+        self.assertEqual(
+            self.easy,
+            a_copy
+        )
+
+
+    def test_bug_4(self):
+        """bug #4 : self / other without affectation should not modify self.
+        """
+        del(self.easy['z'])
+        self.easy /= -1
+        a_copy = self.easy.copy()
+        self.easy / a_copy
+        self.assertEqual(
+            self.easy,
+            a_copy
+        )
+
+    def test_bug_5(self):
+        """bug #5 : int * dict without affectation should not modify self.
+        """
+        a_copy = self.easy.copy()
+        2 * self.easy
+        self.assertEqual(
+            self.easy,
+            a_copy
+        )
+
+    def test_bug_6(self):
+        """bug #6 : int / dict without affectation should not modify self.
+        """
+        del(self.easy['z'])
+        a_copy = self.easy.copy()
+        2.0 / self.easy
+        self.assertEqual(
+            self.easy,
+            a_copy
+        )
+
+
+    def test_for_fun(self):
+        """just for fun """
+        a = self.easy
+        b = self.easy_too
+        aa = a.copy()
+        bb = b.copy()
+        self.assertEqual(
+            (a - b) * (a + b),
+            aa * aa - bb * bb
+        )
+
+
+    def test_for_fun2(self):
+        """just for fun """
+        a = self.easy
+        b = self.easy_too
+        aa = a.copy()
+        bb = b.copy()
+        self.assertEqual(
+            -(a + b) * (a + b),
+            -1 * ((aa * aa) + 2 * aa * bb + (bb * bb))
+        )
+    
+    def test_dyslexia_bug4(self):
+        """counfonding right & left in all r(div/add/sub/mul) operator """
+        a = self.easy
+        self.assertEqual(
+            2/Daikyu({'a':1}),
+            {'a' : 2}
+        )
+        self.assertEqual(
+            2-a,
+            -(a-2)
+        )
+    def test_inplace_bug5(self):
+        """a/b in place"""
+        a = self.easy*4
+        self.assertEqual(
+            a/{'x':2},
+            {'x' : 2}
+        )
+
+if __name__ == '__main__':
+    unittest.main(verbosity=4)
```

### Comparing `archery-1.2.2/archery/bow.py` & `archery-1.3.0/archery/bow.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 
 from .trait import (
         InclusiveAdder, InclusiveSubber, ExclusiveMuler, 
         Iterator, Searchable 
     )
 from .quiver import LinearAlgebrae, VectorDict
 from .barrack import bowyer
-from collections import MutableMapping
+try:
+    from collections import MutableMapping
+except ImportError:
+    from collections.abc import MutableMapping
+
 from warnings import warn
 
 
 
 class _Hankyu(InclusiveAdder,dict):
     pass
```

### Comparing `archery-1.2.2/archery/quiver.py` & `archery-1.3.0/archery/quiver.py`

 * *Files identical despite different names*

### Comparing `archery-1.2.2/archery/test_fun.py` & `archery-1.3.0/archery/test_fun.py`

 * *Files identical despite different names*

### Comparing `archery-1.2.2/README.txt` & `archery-1.3.0/README.txt`

 * *Files identical despite different names*

### Comparing `archery-1.2.2/LICENSE.txt` & `archery-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

