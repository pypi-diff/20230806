# Comparing `tmp/astroid-3.0.0a7.tar.gz` & `tmp/astroid-3.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-3.0.0a7.tar", last modified: Sat Jul  8 18:21:24 2023, max compression
+gzip compressed data, was "astroid-3.0.0a8.tar", last modified: Sat Jul 15 13:54:38 2023, max compression
```

## Comparing `astroid-3.0.0a7.tar` & `astroid-3.0.0a8.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.028925 astroid-3.0.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-08 18:21:06.000000 astroid-3.0.0a7/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-08 18:21:06.000000 astroid-3.0.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 18:21:06.000000 astroid-3.0.0a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-08 18:21:24.028925 astroid-3.0.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-08 18:21:06.000000 astroid-3.0.0a7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:23.992925 astroid-3.0.0a7/astroid/
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/_backport_stdlib_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    27153 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.020925 astroid-3.0.0a7/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    37079 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22134 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18802 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.020925 astroid-3.0.0a7/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.020925 astroid-3.0.0a7/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.020925 astroid-3.0.0a7/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (123)   166863 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    27201 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.024925 astroid-3.0.0a7/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/scoped_nodes/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)   104617 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/scoped_nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    31226 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    71204 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:23.992925 astroid-3.0.0a7/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-08 18:21:06.000000 astroid-3.0.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-08 18:21:06.000000 astroid-3.0.0a7/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-08 18:21:06.000000 astroid-3.0.0a7/requirements_full.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-08 18:21:06.000000 astroid-3.0.0a7/requirements_minimal.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-08 18:21:24.032925 astroid-3.0.0a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.028925 astroid-3.0.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    34680 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_group_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)   223797 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_inference_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19631 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    55463 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_nodes_lineno.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_nodes_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_python3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_regrtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    93424 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_type_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.111012 astroid-3.0.0a8/
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-15 13:54:19.000000 astroid-3.0.0a8/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-15 13:54:19.000000 astroid-3.0.0a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 13:54:19.000000 astroid-3.0.0a8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-15 13:54:38.111012 astroid-3.0.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-15 13:54:19.000000 astroid-3.0.0a8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.095010 astroid-3.0.0a8/astroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27153 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.103011 astroid-3.0.0a8/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37079 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22134 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18802 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.103011 astroid-3.0.0a8/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.107012 astroid-3.0.0a8/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.107012 astroid-3.0.0a8/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166874 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27201 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.107012 astroid-3.0.0a8/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104617 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31226 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71204 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-15 13:54:19.000000 astroid-3.0.0a8/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.095010 astroid-3.0.0a8/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-15 13:54:38.000000 astroid-3.0.0a8/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-15 13:54:38.000000 astroid-3.0.0a8/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:54:38.000000 astroid-3.0.0a8/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 13:54:38.000000 astroid-3.0.0a8/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 13:54:38.000000 astroid-3.0.0a8/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-15 13:54:19.000000 astroid-3.0.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-15 13:54:19.000000 astroid-3.0.0a8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-15 13:54:19.000000 astroid-3.0.0a8/requirements_full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-15 13:54:19.000000 astroid-3.0.0a8/requirements_minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-15 13:54:38.111012 astroid-3.0.0a8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:38.111012 astroid-3.0.0a8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34680 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223597 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19631 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55445 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93424 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-15 13:54:19.000000 astroid-3.0.0a8/tox.ini
```

### Comparing `astroid-3.0.0a7/CONTRIBUTORS.txt` & `astroid-3.0.0a8/CONTRIBUTORS.txt`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 - Peter de Blanc <peter@standard.ai>
 - Peter Talley <peterctalley@gmail.com>
 - Ovidiu Sabou <ovidiu@sabou.org>
 - Nicolas Noirbent <nicolas@noirbent.fr>
 - Neil Girdhar <mistersheik@gmail.com>
 - Michał Masłowski <m.maslowski@clearcode.cc>
 - Mateusz Bysiek <mb@mbdev.pl>
+- Marcelo Trylesinski <marcelotryle@gmail.com>
 - Leandro T. C. Melo <ltcmelo@gmail.com>
 - Konrad Weihmann <kweihmann@outlook.com>
 - Kian Meng, Ang <kianmeng.ang@gmail.com>
 - Kai Mueller <15907922+kasium@users.noreply.github.com>
 - Jörg Thalheim <Mic92@users.noreply.github.com>
 - Josef Kemetmüller <josef.kemetmueller@gmail.com>
 - Jonathan Striebel <jstriebel@users.noreply.github.com>
```

### Comparing `astroid-3.0.0a7/LICENSE` & `astroid-3.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/PKG-INFO` & `astroid-3.0.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a7
+Version: 3.0.0a8
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a7/README.rst` & `astroid-3.0.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/__init__.py` & `astroid-3.0.0a8/astroid/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/_ast.py` & `astroid-3.0.0a8/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/_backport_stdlib_names.py` & `astroid-3.0.0a8/astroid/_backport_stdlib_names.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/arguments.py` & `astroid-3.0.0a8/astroid/arguments.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/astroid_manager.py` & `astroid-3.0.0a8/astroid/astroid_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/bases.py` & `astroid-3.0.0a8/astroid/bases.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_argparse.py` & `astroid-3.0.0a8/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_attrs.py` & `astroid-3.0.0a8/astroid/brain/brain_attrs.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_boto3.py` & `astroid-3.0.0a8/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_builtin_inference.py` & `astroid-3.0.0a8/astroid/brain/brain_builtin_inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_collections.py` & `astroid-3.0.0a8/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_crypt.py` & `astroid-3.0.0a8/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_ctypes.py` & `astroid-3.0.0a8/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_curses.py` & `astroid-3.0.0a8/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_dataclasses.py` & `astroid-3.0.0a8/astroid/brain/brain_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_datetime.py` & `astroid-3.0.0a8/astroid/brain/brain_datetime.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_dateutil.py` & `astroid-3.0.0a8/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_fstrings.py` & `astroid-3.0.0a8/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_functools.py` & `astroid-3.0.0a8/astroid/brain/brain_functools.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_gi.py` & `astroid-3.0.0a8/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_hashlib.py` & `astroid-3.0.0a8/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_http.py` & `astroid-3.0.0a8/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_hypothesis.py` & `astroid-3.0.0a8/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_io.py` & `astroid-3.0.0a8/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_mechanize.py` & `astroid-3.0.0a8/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_multiprocessing.py` & `astroid-3.0.0a8/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.0.0a8/astroid/brain/brain_namedtuple_enum.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_nose.py` & `astroid-3.0.0a8/astroid/brain/brain_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_core_einsumfunc.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_ma.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_numpy_utils.py` & `astroid-3.0.0a8/astroid/brain/brain_numpy_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_pathlib.py` & `astroid-3.0.0a8/astroid/brain/brain_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_pkg_resources.py` & `astroid-3.0.0a8/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_pytest.py` & `astroid-3.0.0a8/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_qt.py` & `astroid-3.0.0a8/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_random.py` & `astroid-3.0.0a8/astroid/brain/brain_random.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_re.py` & `astroid-3.0.0a8/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_regex.py` & `astroid-3.0.0a8/astroid/brain/brain_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_responses.py` & `astroid-3.0.0a8/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_scipy_signal.py` & `astroid-3.0.0a8/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_signal.py` & `astroid-3.0.0a8/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_six.py` & `astroid-3.0.0a8/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_sqlalchemy.py` & `astroid-3.0.0a8/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_ssl.py` & `astroid-3.0.0a8/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_subprocess.py` & `astroid-3.0.0a8/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_threading.py` & `astroid-3.0.0a8/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_type.py` & `astroid-3.0.0a8/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_typing.py` & `astroid-3.0.0a8/astroid/brain/brain_typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_unittest.py` & `astroid-3.0.0a8/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/brain_uuid.py` & `astroid-3.0.0a8/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/brain/helpers.py` & `astroid-3.0.0a8/astroid/brain/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/builder.py` & `astroid-3.0.0a8/astroid/builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/const.py` & `astroid-3.0.0a8/astroid/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/constraint.py` & `astroid-3.0.0a8/astroid/constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/context.py` & `astroid-3.0.0a8/astroid/context.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/decorators.py` & `astroid-3.0.0a8/astroid/decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/exceptions.py` & `astroid-3.0.0a8/astroid/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/filter_statements.py` & `astroid-3.0.0a8/astroid/filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/helpers.py` & `astroid-3.0.0a8/astroid/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/inference_tip.py` & `astroid-3.0.0a8/astroid/inference_tip.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/interpreter/_import/spec.py` & `astroid-3.0.0a8/astroid/interpreter/_import/spec.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/interpreter/_import/util.py` & `astroid-3.0.0a8/astroid/interpreter/_import/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/interpreter/dunder_lookup.py` & `astroid-3.0.0a8/astroid/interpreter/dunder_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/interpreter/objectmodel.py` & `astroid-3.0.0a8/astroid/interpreter/objectmodel.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/manager.py` & `astroid-3.0.0a8/astroid/manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/mixins.py` & `astroid-3.0.0a8/astroid/mixins.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/modutils.py` & `astroid-3.0.0a8/astroid/modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/node_classes.py` & `astroid-3.0.0a8/astroid/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/__init__.py` & `astroid-3.0.0a8/astroid/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/_base_nodes.py` & `astroid-3.0.0a8/astroid/nodes/_base_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/as_string.py` & `astroid-3.0.0a8/astroid/nodes/as_string.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/const.py` & `astroid-3.0.0a8/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/node_classes.py` & `astroid-3.0.0a8/astroid/nodes/node_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     `exceptions` may be a list of exception names. If specified, discard If
     branches and check one of the statement is in an exception handler catching
     one of the given exceptions.
 
     algorithm :
      1) index stmt1's parents
      2) climb among stmt2's parents until we find a common parent
-     3) if the common parent is a If or TryExcept statement, look if nodes are
+     3) if the common parent is a If or Try statement, look if nodes are
         in exclusive branches
     """
     # index stmt1's parents
     stmt1_parents = {}
     children = {}
     previous = stmt1
     for node in stmt1.node_ancestors():
@@ -2538,15 +2538,15 @@
     >>> node = astroid.extract_node('''
         try:
             do_something()
         except Exception as error:
             print("Error!")
         ''')
     >>> node
-    <TryExcept l.2 at 0x7f23b2e9d908>
+    <Try l.2 at 0x7f23b2e9d908>
     >>> node.handlers
     [<ExceptHandler l.4 at 0x7f23b2e9e860>]
     """
 
     _astroid_fields = ("type", "name", "body")
     _multi_line_block_fields = ("body",)
 
@@ -4006,15 +4006,15 @@
 
         :param index: The node to use as a subscript index.
         :type index: Const or Slice
         """
         return _container_getitem(self, self.elts, index, context=context)
 
 
-class TypeAlias(_base_nodes.AssignTypeNode):
+class TypeAlias(_base_nodes.AssignTypeNode, _base_nodes.Statement):
     """Class representing a :class:`ast.TypeAlias` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('type Point = tuple[float, float]')
     >>> node
     <TypeAlias l.1 at 0x7f23b2e4e198>
     """
```

### Comparing `astroid-3.0.0a7/astroid/nodes/node_ng.py` & `astroid-3.0.0a8/astroid/nodes/node_ng.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.0.0a8/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/scoped_nodes/mixin.py` & `astroid-3.0.0a8/astroid/nodes/scoped_nodes/mixin.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.0.0a8/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/nodes/scoped_nodes/utils.py` & `astroid-3.0.0a8/astroid/nodes/scoped_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/objects.py` & `astroid-3.0.0a8/astroid/objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/protocols.py` & `astroid-3.0.0a8/astroid/protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/raw_building.py` & `astroid-3.0.0a8/astroid/raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/rebuilder.py` & `astroid-3.0.0a8/astroid/rebuilder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/scoped_nodes.py` & `astroid-3.0.0a8/astroid/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/test_utils.py` & `astroid-3.0.0a8/astroid/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/transforms.py` & `astroid-3.0.0a8/astroid/transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/typing.py` & `astroid-3.0.0a8/astroid/typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid/util.py` & `astroid-3.0.0a8/astroid/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/astroid.egg-info/PKG-INFO` & `astroid-3.0.0a8/astroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a7
+Version: 3.0.0a8
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a7/astroid.egg-info/SOURCES.txt` & `astroid-3.0.0a8/astroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/pyproject.toml` & `astroid-3.0.0a8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/resources.py` & `astroid-3.0.0a8/tests/resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_builder.py` & `astroid-3.0.0a8/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_constraint.py` & `astroid-3.0.0a8/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_decorators.py` & `astroid-3.0.0a8/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_filter_statements.py` & `astroid-3.0.0a8/tests/test_filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_group_exceptions.py` & `astroid-3.0.0a8/tests/test_group_exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_helpers.py` & `astroid-3.0.0a8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_inference.py` & `astroid-3.0.0a8/tests/test_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,14 @@
 
 def get_node_of_class(start_from: nodes.FunctionDef, klass: type) -> nodes.Attribute:
     return next(start_from.nodes_of_class(klass))
 
 
 builder = AstroidBuilder()
 
-EXC_MODULE = "builtins"
-BOOL_SPECIAL_METHOD = "__bool__"
 DATA_DIR = Path(__file__).parent / "testdata" / "python3" / "data"
 
 
 class InferenceUtilsTest(unittest.TestCase):
     def test_path_wrapper(self) -> None:
         def infer_default(self: Any, *args: InferenceContext) -> None:
             raise InferenceError
@@ -195,15 +193,15 @@
         self.assertRaises(StopIteration, partial(next, inferred))
 
     def test_tupleassign_name_inference(self) -> None:
         inferred = self.ast["a"].infer()
         exc = next(inferred)
         self.assertIsInstance(exc, Instance)
         self.assertEqual(exc.name, "Exception")
-        self.assertEqual(exc.root().name, EXC_MODULE)
+        self.assertEqual(exc.root().name, "builtins")
         self.assertRaises(StopIteration, partial(next, inferred))
         inferred = self.ast["b"].infer()
         const = next(inferred)
         self.assertIsInstance(const, nodes.Const)
         self.assertEqual(const.value, 1)
         self.assertRaises(StopIteration, partial(next, inferred))
         inferred = self.ast["c"].infer()
@@ -213,15 +211,15 @@
         self.assertRaises(StopIteration, partial(next, inferred))
 
     def test_listassign_name_inference(self) -> None:
         inferred = self.ast["d"].infer()
         exc = next(inferred)
         self.assertIsInstance(exc, Instance)
         self.assertEqual(exc.name, "Exception")
-        self.assertEqual(exc.root().name, EXC_MODULE)
+        self.assertEqual(exc.root().name, "builtins")
         self.assertRaises(StopIteration, partial(next, inferred))
         inferred = self.ast["e"].infer()
         const = next(inferred)
         self.assertIsInstance(const, nodes.Const)
         self.assertEqual(const.value, 1.0)
         self.assertRaises(StopIteration, partial(next, inferred))
         inferred = self.ast["f"].infer()
@@ -264,23 +262,23 @@
         self.assertIsInstance(const, nodes.Const)
         self.assertEqual(const.value, 1)
         self.assertRaises(StopIteration, partial(next, inferred))
         inferred = self.ast.locals["b"][1].infer()
         exc = next(inferred)
         self.assertIsInstance(exc, Instance)
         self.assertEqual(exc.name, "Exception")
-        self.assertEqual(exc.root().name, EXC_MODULE)
+        self.assertEqual(exc.root().name, "builtins")
         self.assertRaises(StopIteration, partial(next, inferred))
 
     def test_getattr_inference1(self) -> None:
         inferred = self.ast["ex"].infer()
         exc = next(inferred)
         self.assertIsInstance(exc, Instance)
         self.assertEqual(exc.name, "Exception")
-        self.assertEqual(exc.root().name, EXC_MODULE)
+        self.assertEqual(exc.root().name, "builtins")
         self.assertRaises(StopIteration, partial(next, inferred))
 
     def test_getattr_inference2(self) -> None:
         inferred = get_node_of_class(self.ast["C"]["meth2"], nodes.Attribute).infer()
         meth1 = next(inferred)
         self.assertEqual(meth1.name, "meth1")
         self.assertEqual(meth1.root().name, __name__)
@@ -532,21 +530,21 @@
                 pass
         """
         ast = parse(code, __name__)
         w = ast["Warning"]
         ancestors = w.ancestors()
         ancestor = next(ancestors)
         self.assertEqual(ancestor.name, "Warning")
-        self.assertEqual(ancestor.root().name, EXC_MODULE)
+        self.assertEqual(ancestor.root().name, "builtins")
         ancestor = next(ancestors)
         self.assertEqual(ancestor.name, "Exception")
-        self.assertEqual(ancestor.root().name, EXC_MODULE)
+        self.assertEqual(ancestor.root().name, "builtins")
         ancestor = next(ancestors)
         self.assertEqual(ancestor.name, "BaseException")
-        self.assertEqual(ancestor.root().name, EXC_MODULE)
+        self.assertEqual(ancestor.root().name, "builtins")
         ancestor = next(ancestors)
         self.assertEqual(ancestor.name, "object")
         self.assertEqual(ancestor.root().name, "builtins")
         self.assertRaises(StopIteration, partial(next, ancestors))
 
     def test_method_argument(self) -> None:
         code = '''
@@ -2885,20 +2883,20 @@
         good_callfunc = next(module["good_callfunc"].infer())
         self.assertTrue(good_callfunc.bool_value())
         compare = module["compare"].parent.value
         self.assertEqual(compare.bool_value(), util.Uninferable)
 
     def test_bool_value_instances(self) -> None:
         instances = extract_node(
-            f"""
+            """
         class FalseBoolInstance(object):
-            def {BOOL_SPECIAL_METHOD}(self):
+            def __bool__(self):
                 return False
         class TrueBoolInstance(object):
-            def {BOOL_SPECIAL_METHOD}(self):
+            def __bool__(self):
                 return True
         class FalseLenInstance(object):
             def __len__(self):
                 return 0
         class TrueLenInstance(object):
             def __len__(self):
                 return 14
@@ -2923,19 +2921,19 @@
         expected = (False, True, False, True, True, util.Uninferable, util.Uninferable)
         for node, expected_value in zip(instances, expected):
             inferred = next(node.infer())
             self.assertEqual(inferred.bool_value(), expected_value)
 
     def test_bool_value_variable(self) -> None:
         instance = extract_node(
-            f"""
+            """
         class VariableBoolInstance(object):
             def __init__(self, value):
                 self.value = value
-            def {BOOL_SPECIAL_METHOD}(self):
+            def __bool__(self):
                 return self.value
 
         not VariableBoolInstance(True)
         """
         )
         inferred = next(instance.infer())
         self.assertIs(inferred.bool_value(), util.Uninferable)
@@ -4852,28 +4850,28 @@
             if expected is util.Uninferable:
                 self.assertEqual(expected, inferred)
             else:
                 self.assertEqual(inferred.value, expected)
 
     def test_bool_bool_special_method(self) -> None:
         ast_nodes = extract_node(
-            f"""
+            """
         class FalseClass:
-           def {BOOL_SPECIAL_METHOD}(self):
+           def __bool__(self):
                return False
         class TrueClass:
-           def {BOOL_SPECIAL_METHOD}(self):
+           def __bool__(self):
                return True
         class C(object):
            def __call__(self):
                return False
         class B(object):
-           {BOOL_SPECIAL_METHOD} = C()
+           __bool__ = C()
         class LambdaBoolFalse(object):
-            {BOOL_SPECIAL_METHOD} = lambda self: self.foo
+            __bool__ = lambda self: self.foo
             @property
             def foo(self): return 0
         class FalseBoolLen(object):
             __len__ = lambda self: self.foo
             @property
             def foo(self): return 0
         bool(FalseClass) #@
@@ -4888,17 +4886,17 @@
         expected = [True, True, False, True, False, False, False]
         for node, expected_value in zip(ast_nodes, expected):
             inferred = next(node.infer())
             self.assertEqual(inferred.value, expected_value)
 
     def test_bool_instance_not_callable(self) -> None:
         ast_nodes = extract_node(
-            f"""
+            """
         class BoolInvalid(object):
-           {BOOL_SPECIAL_METHOD} = 42
+           __bool__ = 42
         class LenInvalid(object):
            __len__ = "a"
         bool(BoolInvalid()) #@
         bool(LenInvalid()) #@
         """
         )
         for node in ast_nodes:
@@ -6023,16 +6021,15 @@
     assert isinstance(node, nodes.NodeNG)
     inferred = node.inferred()
     assert len(inferred) == 1
     inferred_exc = inferred[0]
     assert isinstance(inferred_exc, Instance)
     assert inferred_exc.name == "OSError"
 
-    # Check that two except handlers on the same TryExcept works the same as separate
-    # TryExcepts
+    # Two except handlers on the same Try work the same as separate
     node = extract_node(
         """
     try:
         1/0
     except ZeroDivisionError as exc:
         pass
     except ValueError as exc:
```

### Comparing `astroid-3.0.0a7/tests/test_inference_calls.py` & `astroid-3.0.0a8/tests/test_inference_calls.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_lookup.py` & `astroid-3.0.0a8/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_manager.py` & `astroid-3.0.0a8/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_modutils.py` & `astroid-3.0.0a8/tests/test_modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_nodes.py` & `astroid-3.0.0a8/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_nodes_lineno.py` & `astroid-3.0.0a8/tests/test_nodes_lineno.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,15 +733,15 @@
         d2 = ast_nodes[1]
         assert isinstance(d2, nodes.DictUnpack)
         assert (d2.lineno, d2.col_offset) == (3, 6)
         assert (d2.end_lineno, d2.end_col_offset) == (3, 18)
 
     @staticmethod
     def test_end_lineno_try() -> None:
-        """TryExcept, TryFinally, ExceptHandler."""
+        """Try, ExceptHandler."""
         code = textwrap.dedent(
             """
         try:  #@
             pass
         except KeyError as ex:
             pass
         except AttributeError as ex:
```

### Comparing `astroid-3.0.0a7/tests/test_nodes_position.py` & `astroid-3.0.0a8/tests/test_nodes_position.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_object_model.py` & `astroid-3.0.0a8/tests/test_object_model.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_objects.py` & `astroid-3.0.0a8/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_protocols.py` & `astroid-3.0.0a8/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_python3.py` & `astroid-3.0.0a8/tests/test_python3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_raw_building.py` & `astroid-3.0.0a8/tests/test_raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_regrtest.py` & `astroid-3.0.0a8/tests/test_regrtest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_scoped_nodes.py` & `astroid-3.0.0a8/tests/test_scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_stdlib.py` & `astroid-3.0.0a8/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_transforms.py` & `astroid-3.0.0a8/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a7/tests/test_type_params.py` & `astroid-3.0.0a8/tests/test_type_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     assert node.value.value.name == "list"
     assert node.value.slice.name == "tuple"
     assert all(elt.name == "float" for elt in node.value.slice.elts)
 
     assert node.inferred()[0] is node
     assert node.type_params[0].inferred()[0] is node.type_params[0]
 
+    assert node.statement() is node
+
 
 def test_type_param_spec() -> None:
     node = extract_node("type Alias[**P] = Callable[P, int]")
     params = node.type_params[0]
     assert isinstance(params, ParamSpec)
     assert isinstance(params.name, AssignName)
     assert params.name.name == "P"
```

### Comparing `astroid-3.0.0a7/tests/test_utils.py` & `astroid-3.0.0a8/tests/test_utils.py`

 * *Files identical despite different names*

