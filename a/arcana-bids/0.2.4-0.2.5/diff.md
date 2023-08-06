# Comparing `tmp/arcana_bids-0.2.4.tar.gz` & `tmp/arcana_bids-0.2.5.tar.gz`

## Comparing `arcana_bids-0.2.4.tar` & `arcana_bids-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/_version.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/cli.py
--rw-r--r--   0        0        0    23277 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/data.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/deploy.py
--rw-r--r--   0        0        0    15156 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/tasks.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/tests/test_cli.py
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/tests/test_data.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/tests/test_tasks.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/LICENSE
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/README.rst
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/_version.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/cli.py
+-rw-r--r--   0        0        0    23318 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/data.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/deploy.py
+-rw-r--r--   0        0        0    15435 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/tasks.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/tests/test_cli.py
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/tests/test_data.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/tests/test_tasks.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/README.rst
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/PKG-INFO
```

### Comparing `arcana_bids-0.2.4/arcana/bids/cli.py` & `arcana_bids-0.2.5/arcana/bids/cli.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.4/arcana/bids/data.py` & `arcana_bids-0.2.5/arcana/bids/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from arcana.core.data.store import LocalStore
 from fileformats.core import FileSet, Field
 from fileformats.generic import Directory
 from fileformats.medimage.nifti import WithBids, NiftiGzX
 from arcana.core.exceptions import ArcanaUsageError
 from arcana.core.data.tree import DataTree
 from arcana.core.data.set import Dataset
-from arcana.stdlib import Clinical
+from arcana.common import Clinical
 from arcana.core.data.entry import DataEntry
 from arcana.core.data.row import DataRow
 
 logger = logging.getLogger("arcana")
 
 
 @attrs.define
@@ -224,17 +224,17 @@
 
     def put_fileset(self, fileset: FileSet, entry: DataEntry) -> FileSet:
         """
         Inserts or updates a fileset in the store
         """
         fspath = self._fileset_fspath(entry)
         # Create target directory if it doesn't exist already
-        copied_fileset = fileset.copy_to(
+        copied_fileset = fileset.copy(
             dest_dir=fspath.parent,
-            stem=fspath.name[: -len(fileset.ext)],
+            new_stem=fspath.name[: -len(fileset.ext)],
             make_dirs=True,
             overwrite=entry.is_derivative,
         )
         if isinstance(copied_fileset, WithBids):
             # Ensure TaskName field is present in the JSON side-car if task
             # is in the filename
             self._edit_nifti_x(copied_fileset, entry)
@@ -245,15 +245,15 @@
         return datatype(self.read_from_json(fspath, key))
 
     def put_field(self, field: Field, entry: DataEntry):
         """
         Inserts or updates a field in the store
         """
         fspath, key = self._fields_fspath_and_key(entry)
-        self.update_json(fspath, key, field.raw_type(field))
+        self.update_json(fspath, key, field.primitive(field))
 
     def get_fileset_provenance(self, entry: DataEntry) -> dict[str, ty.Any]:
         with open(self._fileset_prov_fspath(entry)) as f:
             provenance = json.load(f)
         return provenance
 
     def put_fileset_provenance(self, provenance: dict[str, ty.Any], entry: DataEntry):
@@ -311,25 +311,25 @@
                 for subject_id, group_id in subjects_group_id.items():
                     f.write(f"sub-{subject_id}\t{group_id}\n")
 
     ####################
     # Overrides of API #
     ####################
 
-    def save_dataset(self, dataset: Dataset, name: str = None):
+    def save_dataset(self, dataset: Dataset, name: ty.Optional[str] = None):
         super().save_dataset(dataset, name=name)
         self._save_metadata(dataset)
 
     def create_dataset(
         self,
         id: str,
         leaves: list[tuple[str, ...]],
         hierarchy: list[str] = ["session"],
         space: type = Clinical,
-        name: str = None,
+        name: ty.Optional[str] = None,
         **kwargs,
     ):
         """Creates a new dataset with new rows to store data in
 
         Parameters
         ----------
         id : str
@@ -490,15 +490,15 @@
         for key, val in entities:
             if key not in ("sub", "ses"):
                 entry_path += f"/{key}={val}"
         return entry_path + "/" + suffix
 
     @classmethod
     def _entry2fs_path(
-        cls, entry_path: str, subject_id: str, timepoint_id: str = None, ext: str = ""
+        cls, entry_path: str, subject_id: str, timepoint_id: ty.Optional[str] = None, ext: str = ""
     ) -> Path:
         """Converts a BIDS filename into an Arcana "entry-path".
         Entities not corresponding to subject and session IDs
 
         Parameters
         ----------
         path : str
```

### Comparing `arcana_bids-0.2.4/arcana/bids/tasks.py` & `arcana_bids-0.2.5/arcana/bids/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     DockerSpec,
     SingularitySpec,
     ShellOutSpec,
 )
 from arcana.core import __version__
 from arcana.core.data.set import Dataset
 from fileformats.core import FileSet
-from arcana.stdlib import Clinical
+from fileformats.generic import Directory
+from arcana.common import Clinical
 from arcana.bids.data import JsonEdit
 from arcana.core.exceptions import ArcanaUsageError
 from arcana.core.utils.serialize import (
     ClassResolver,
     ObjectListConverter,
 )
 from arcana.core.utils.misc import func_task
@@ -41,32 +42,32 @@
 
 
 @attrs.define(kw_only=True)
 class BidsOutput:
 
     name: str
     datatype: FileSet = attrs.field(converter=ClassResolver(FileSet))
-    path: str = None
+    path: ty.Optional[str] = None
 
 
 logger = logging.getLogger("arcana")
 
 
 def bids_app(
     name: str,
     inputs: list[ty.Union[BidsInput, dict[str, str]]],
     outputs: list[ty.Union[BidsOutput, dict[str, str]]],
     executable: str = "",  # Use entrypoint of container,
-    container_image: str = None,
+    container_image: ty.Optional[str] = None,
     parameters: ty.Dict[str, type] = None,
-    row_frequency: Clinical or str = Clinical.session,
+    row_frequency: ty.Union[Clinical, str] = Clinical.session,
     container_type: str = "docker",
     dataset: ty.Optional[ty.Union[str, Path, Dataset]] = None,
-    app_output_dir: Path = None,
-    app_work_dir: Path = None,
+    app_output_dir: ty.Optional[Path] = None,
+    app_work_dir: ty.Optional[Path] = None,
     json_edits: ty.List[ty.Tuple[str, str]] = None,
 ) -> Workflow:
     """Creates a Pydra workflow which takes file inputs, maps them to
     a BIDS dataset, executes a BIDS app, and then extracts the
     the derivatives that were stored back in the BIDS dataset by the app
 
     Parameters
@@ -121,14 +122,20 @@
     if parameters is None:
         parameters = {}
     if app_output_dir is None:
         app_output_dir = Path(tempfile.mkdtemp())
     else:
         app_output_dir = Path(app_output_dir)
         app_output_dir.mkdir(parents=True, exist_ok=True)
+    if app_work_dir is None:
+        app_work_dir = Path(tempfile.mkdtemp())
+    else:
+        app_work_dir = Path(app_work_dir)
+        app_work_dir.mkdir(parents=True, exist_ok=True)
+
     if json_edits is None:
         json_edits = []
 
     if isinstance(row_frequency, str):
         row_frequency = Clinical[row_frequency]
 
     # Create BIDS dataset to hold translated data
@@ -169,16 +176,16 @@
     # arguments
     wf.add(
         func_task(
             to_bids,
             in_fields=(
                 [
                     ("row_frequency", Clinical),
-                    ("inputs", ty.List[ty.Tuple[str, type, str]]),
-                    ("dataset", Dataset or str),
+                    ("inputs", ty.List[BidsInput]),
+                    ("dataset", ty.Union[Dataset, str]),
                     ("id", str),
                     ("json_edits", str),
                     ("fixed_json_edits", ty.List[ty.Tuple[str, str]]),
                 ]
                 + [(i, ty.Union[str, Path]) for i in input_names]
             ),
             out_fields=[
@@ -220,20 +227,19 @@
     # If 'image' is None, don't use any virtualisation (i.e. assume we are running from "inside" the
     # container or extension of it)
     if container_image is None:
         task_cls = ShellCommandTask
         base_spec_cls = ShellSpec
         kwargs["executable"] = executable
         app_output_path = str(app_output_dir)
-        app_dataset_path = Path(dataset.id)
     else:
 
         # Set input and output directories to "internal" paths within the
         # container
-        app_dataset_path = CONTAINER_DATASET_PATH
+        # app_dataset_path = CONTAINER_DATASET_PATH
         app_output_path = CONTAINER_DERIV_PATH
         kwargs["image"] = container_image
 
         if container_type == "docker":
             task_cls = DockerTask
             base_spec_cls = DockerSpec
         elif container_type == "singularity":
@@ -253,40 +259,40 @@
 
     main_task = task_cls(
         name="bids_app",
         input_spec=SpecInfo(name="Input", fields=input_fields, bases=(base_spec_cls,)),
         output_spec=SpecInfo(
             name="Output", fields=BIDS_APP_OUTPUTS, bases=(ShellOutSpec,)
         ),
-        dataset_path=str(app_dataset_path),
+        dataset_path=dataset.id,
         output_path=str(app_output_path),
-        work_dir=app_work_dir,
+        work_dir=str(app_work_dir),
         analysis_level=analysis_level,
         flags=wf.lzin.flags,
         setup_completed=wf.to_bids.lzout.completed,
         **kwargs,
     )
 
     if container_image is not None:
         main_task.bindings = {
-            dataset.id: (CONTAINER_DATASET_PATH, "ro"),
-            app_output_dir: (CONTAINER_DERIV_PATH, "rw"),
+            # str(dataset.id): (CONTAINER_DATASET_PATH, "ro"),
+            str(app_output_dir): (CONTAINER_DERIV_PATH, "rw"),
         }
 
     wf.add(main_task)
 
     wf.add(
         func_task(
             extract_bids,
             in_fields=[
                 ("dataset", Dataset),
                 ("row_frequency", Clinical),
                 ("app_name", str),
                 ("output_dir", Path),
-                ("outputs", ty.List[ty.Tuple[str, type, str]]),
+                ("outputs", ty.List[BidsOutput]),
                 ("id", str),
                 ("app_completed", bool),
             ],
             out_fields=[(o, str) for o in output_names],
             name="extract_bids",
             app_name=name,
             # We pass dataset object modified by to_bids rather than initial one passed
@@ -391,25 +397,25 @@
             output_paths.append(row[output.name])
     return tuple(output_paths) if len(outputs) > 1 else output_paths[0]
 
 
 BIDS_APP_INPUTS = [
     (
         "dataset_path",
-        str,
+        Directory,  # Needs to be path for internal container paths
         {
             "help_string": "Path to BIDS dataset in the container",
             "position": 1,
             "mandatory": True,
             "argstr": "'{dataset_path}'",
         },
     ),
     (
         "output_path",
-        str,
+        Path,
         {
             "help_string": "Directory where outputs will be written in the container",
             "position": 2,
             "argstr": "'{output_path}'",
         },
     ),
     (
@@ -419,15 +425,15 @@
             "help_string": "The analysis level the app will be run at",
             "position": 3,
             "argstr": "",
         },
     ),
     (
         "participant_label",
-        ty.List[str],
+        str,
         {
             "help_string": "The IDs to include in the analysis",
             "argstr": "--participant-label ",
             "position": 4,
         },
     ),
     (
@@ -437,15 +443,15 @@
             "help_string": "Additional flags to pass to the app",
             "argstr": "",
             "position": -1,
         },
     ),
     (
         "work_dir",
-        str,
+        Path,
         {
             "help_string": "Directory where the nipype temporary working directories will be stored",
             "argstr": "--work-dir '{work_dir}'",
         },
     ),
     (
         "setup_completed",
```

### Comparing `arcana_bids-0.2.4/arcana/bids/tests/test_cli.py` & `arcana_bids-0.2.5/arcana/bids/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import reduce
 from operator import mul
 import pytest
 from fileformats.text import Plain as Text
 from arcana.testing.data.blueprint import (
     TestDatasetBlueprint, FileSetEntryBlueprint as FileBP
 )
-from arcana.stdlib import Clinical
+from arcana.common import Clinical
 from fileformats.medimage import NiftiGzX
 from arcana.bids.cli import app_entrypoint
 from arcana.core.utils.serialize import ClassResolver
 from arcana.core.utils.misc import path2varname
 from arcana.core.utils.misc import show_cli_trace
 from arcana.core.deploy import App
 from arcana.bids.data import Bids
```

### Comparing `arcana_bids-0.2.4/arcana/bids/tests/test_data.py` & `arcana_bids-0.2.5/arcana/bids/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy.random
 import shutil
 from dataclasses import dataclass
 import pytest
 import docker
 from fileformats.medimage import NiftiX
 from arcana.core import __version__
-from arcana.stdlib import Clinical
+from arcana.common import Clinical
 from arcana.bids.data import Bids
 
 
 MOCK_BIDS_APP_NAME = "mockapp"
 MOCK_README = "A dummy readme\n" * 100
 MOCK_AUTHORS = ["Dumm Y. Author", "Another D. Author"]
```

### Comparing `arcana_bids-0.2.4/arcana/bids/tests/test_tasks.py` & `arcana_bids-0.2.5/arcana/bids/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.4/LICENSE` & `arcana_bids-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.4/README.rst` & `arcana_bids-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.4/pyproject.toml` & `arcana_bids-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.4/PKG-INFO` & `arcana_bids-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-bids
-Version: 0.2.4
+Version: 0.2.5
 Summary: An Arcana extension for interacting with Brain Imaging Structure (BIDS) datasets and associated "Apps"
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-bids.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

