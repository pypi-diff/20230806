# Comparing `tmp/fileformats_medimage_extras-0.1.4.tar.gz` & `tmp/fileformats_medimage_extras-0.1.5.tar.gz`

## Comparing `fileformats_medimage_extras-0.1.4.tar` & `fileformats_medimage_extras-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/.codespell-ignorewords
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/_version.py
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/converters.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/dicom.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/diffusion.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/mrtrix3.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/nifti.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/LICENSE
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/README.rst
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/.codespell-ignorewords
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/_version.py
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/converters.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/dicom.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/diffusion.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/mrtrix3.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/nifti.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/README.rst
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.5/PKG-INFO
```

### Comparing `fileformats_medimage_extras-0.1.4/.pre-commit-config.yaml` & `fileformats_medimage_extras-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/conftest.py` & `fileformats_medimage_extras-0.1.5/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/.github/workflows/publish.yml` & `fileformats_medimage_extras-0.1.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/.github/workflows/tests.yml` & `fileformats_medimage_extras-0.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/converters.py` & `fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     return MRConvert(name=name, out_file="out" + out_ext)
 
 
 @pydra.mark.task
 def ensure_dicom_dir(dicom: DicomCollection) -> DicomDir:
     if isinstance(dicom, DicomSet):
         dicom_dir_fspath = tempfile.mkdtemp()
-        dicom.copy(dicom_dir_fspath, link_type="symbolic")
+        dicom.copy(dicom_dir_fspath, mode=DicomDir.CopyMode.link)
         dicom = DicomDir(dicom_dir_fspath)
     elif not isinstance(dicom, DicomDir):
         raise RuntimeError(
             "Unrecognised input to ensure_dicom_dir, should be DicomSet or DicomDir "
             f"not {dicom}"
         )
     return dicom
```

### Comparing `fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/dicom.py` & `fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/diffusion.py` & `fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/nifti.py` & `fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/fileformats/extras/medimage/tests/test_neuro_converters.py` & `fileformats_medimage_extras-0.1.5/fileformats/extras/medimage/tests/test_neuro_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/LICENSE` & `fileformats_medimage_extras-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/README.rst` & `fileformats_medimage_extras-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/pyproject.toml` & `fileformats_medimage_extras-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.4/PKG-INFO` & `fileformats_medimage_extras-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-medimage-extras
-Version: 0.1.4
+Version: 0.1.5
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage-extras
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

