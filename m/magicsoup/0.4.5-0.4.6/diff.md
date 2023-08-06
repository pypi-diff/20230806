# Comparing `tmp/magicsoup-0.4.5.tar.gz` & `tmp/magicsoup-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.4.5.tar", last modified: Thu Aug  3 19:35:22 2023, max compression
+gzip compressed data, was "magicsoup-0.4.6.tar", last modified: Sat Aug  5 17:36:38 2023, max compression
```

## Comparing `magicsoup-0.4.5.tar` & `magicsoup-0.4.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.086588 magicsoup-0.4.5/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.5/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5377 2023-08-03 19:35:22.086588 magicsoup-0.4.5/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4440 2023-08-03 19:34:38.000000 magicsoup-0.4.5/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.5/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-08-03 19:35:22.086588 magicsoup-0.4.5/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.082588 magicsoup-0.4.5/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.082588 magicsoup-0.4.5/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-08-03 19:35:12.000000 magicsoup-0.4.5/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.5/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    25390 2023-06-19 19:49:05.000000 magicsoup-0.4.5/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.086588 magicsoup-0.4.5/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.5/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.5/src/magicsoup/examples/co2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.5/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.5/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.5/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.5/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    40808 2023-07-10 19:08:24.000000 magicsoup-0.4.5/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.5/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.5/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45270 2023-06-19 19:47:46.000000 magicsoup-0.4.5/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.086588 magicsoup-0.4.5/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5377 2023-08-03 19:35:22.000000 magicsoup-0.4.5/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-08-03 19:35:22.000000 magicsoup-0.4.5/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-08-03 19:35:22.000000 magicsoup-0.4.5/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-08-03 19:35:22.000000 magicsoup-0.4.5/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-03 19:35:22.086588 magicsoup-0.4.5/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.5/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.5/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.5/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4961 2023-07-09 21:24:24.000000 magicsoup-0.4.5/tests/test_kinetics_integration.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.5/tests/test_mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.5/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.5/tests/test_world.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 21:29:47.000000 magicsoup-0.4.5/tests/test_world_integration.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-05 17:36:38.341850 magicsoup-0.4.6/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.6/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5447 2023-08-05 17:36:38.337850 magicsoup-0.4.6/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4510 2023-08-04 09:40:26.000000 magicsoup-0.4.6/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.6/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-08-05 17:36:38.341850 magicsoup-0.4.6/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-05 17:36:38.337850 magicsoup-0.4.6/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-05 17:36:38.337850 magicsoup-0.4.6/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-08-05 17:36:22.000000 magicsoup-0.4.6/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.6/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    25605 2023-08-05 13:24:08.000000 magicsoup-0.4.6/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-05 17:36:38.337850 magicsoup-0.4.6/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.6/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.6/src/magicsoup/examples/co2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.6/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.6/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.6/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.6/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    41184 2023-08-05 13:26:59.000000 magicsoup-0.4.6/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.6/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.6/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45698 2023-08-05 13:26:35.000000 magicsoup-0.4.6/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-05 17:36:38.337850 magicsoup-0.4.6/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5447 2023-08-05 17:36:38.000000 magicsoup-0.4.6/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-08-05 17:36:38.000000 magicsoup-0.4.6/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-08-05 17:36:38.000000 magicsoup-0.4.6/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-08-05 17:36:38.000000 magicsoup-0.4.6/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-08-05 17:36:38.337850 magicsoup-0.4.6/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.6/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.6/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.6/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4961 2023-07-09 21:24:24.000000 magicsoup-0.4.6/tests/test_kinetics_integration.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.6/tests/test_mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.6/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.6/tests/test_world.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 21:29:47.000000 magicsoup-0.4.6/tests/test_world_integration.py
```

### Comparing `magicsoup-0.4.5/LICENSE` & `magicsoup-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/PKG-INFO` & `magicsoup-0.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.5
+Version: 0.4.6
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
@@ -36,21 +36,21 @@
 This game simulates cell metabolic and transduction pathway evolution.
 Define a 2D world with certain molecules and reactions.
 Add a few cells and create evolutionary pressure by selectively replicating and killing them.
 Then run and see what random mutations can do.
 
 ![random cells](https://raw.githubusercontent.com/mRcSchwering/magic-soup/main/docs/img/animation.gif)
 
-_Cell growth of 1000 cells with different genomes were simulated. Top row: Cell map showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line when energy levels were high, celline 2 when they wer low. Middle and bottom rows: Development of total cell count and molecule species concentrations over time._
+_Cell growth of 1000 cells with different genomes was simulated. Top row: Cell maps showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line at high energy levels, celline 2 at low energy levels. Middle and bottom rows: Development of total cell count and molecule concentrations over time._
 
 ### Installation
 
 For CPU alone you can just do:
 
-```
+```bash
 pip install magicsoup
 ```
 
 This simulation relies on [PyTorch](https://pytorch.org/).
 To increase performance you can move calculations to a GPU.
 In this case you should setup PyTorch first before installing MagicSoup.
 To setup pytorch correctly for your GPU see [Get Started (pytorch.org)](https://pytorch.org/get-started/locally/).
@@ -93,50 +93,50 @@
 ```
 
 Cells discover new proteins by chance through mutations.
 In the function below all cells experience 1E-3 random point mutations per nucleotide.
 10% of them will be indels.
 
 ```python
-def mutate_cells():
+def mutate_cells(world: ms.World):
     mutated = ms.point_mutations(seqs=world.genomes)
     world.update_cells(genome_idx_pairs=mutated)
 ```
 
 Evolutionary pressure can be applied by selectively killing or replicating cells.
 Here, cells have an increased chance of dying when formiat gets too low
 and an increased chance of replicating when formiat gets high.
 
 ```python
 def sample(p: torch.Tensor) -> list[int]:
     idxs = torch.argwhere(torch.bernoulli(p))
     return idxs.flatten().tolist()
 
-def kill_cells():
+def kill_cells(world: ms.World):
     x = world.cell_molecules[:, 2]
     idxs = sample(.01 / (.01 + x))
     world.kill_cells(cell_idxs=idxs)
 
-def replicate_cells():
+def replicate_cells(world: ms.World):
     x = world.cell_molecules[:, 2]
     idxs = sample(x ** 3 / (x ** 3 + 20.0 ** 3))
     world.divide_cells(cell_idxs=idxs)
 ```
 
 Finally, the simulation itself is run in a python loop by repetitively calling the different steps.
 With `world.enzymatic_activity()` chemical reactions and molecule transport
 in cells advance by one time step.
 `world.diffuse_molecules()` lets molecules on the world map diffuse and permeate through cell membranes
 (if they can) by one time step.
 
 ```python
 for _ in range(1000):
     world.enzymatic_activity()
-    kill_cells()
-    replicate_cells()
-    mutate_cells()
+    kill_cells(world=world)
+    replicate_cells(world=world)
+    mutate_cells(world=world)
     world.diffuse_molecules()
     world.increment_cell_lifetimes()
 ```
 
 See the [Docs](https://magic-soup.readthedocs.io/) for more examples and a description of all the mechanics of this simulation
```

### Comparing `magicsoup-0.4.5/README.md` & `magicsoup-0.4.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 This game simulates cell metabolic and transduction pathway evolution.
 Define a 2D world with certain molecules and reactions.
 Add a few cells and create evolutionary pressure by selectively replicating and killing them.
 Then run and see what random mutations can do.
 
 ![random cells](https://raw.githubusercontent.com/mRcSchwering/magic-soup/main/docs/img/animation.gif)
 
-_Cell growth of 1000 cells with different genomes were simulated. Top row: Cell map showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line when energy levels were high, celline 2 when they wer low. Middle and bottom rows: Development of total cell count and molecule species concentrations over time._
+_Cell growth of 1000 cells with different genomes was simulated. Top row: Cell maps showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line at high energy levels, celline 2 at low energy levels. Middle and bottom rows: Development of total cell count and molecule concentrations over time._
 
 ### Installation
 
 For CPU alone you can just do:
 
-```
+```bash
 pip install magicsoup
 ```
 
 This simulation relies on [PyTorch](https://pytorch.org/).
 To increase performance you can move calculations to a GPU.
 In this case you should setup PyTorch first before installing MagicSoup.
 To setup pytorch correctly for your GPU see [Get Started (pytorch.org)](https://pytorch.org/get-started/locally/).
@@ -70,50 +70,50 @@
 ```
 
 Cells discover new proteins by chance through mutations.
 In the function below all cells experience 1E-3 random point mutations per nucleotide.
 10% of them will be indels.
 
 ```python
-def mutate_cells():
+def mutate_cells(world: ms.World):
     mutated = ms.point_mutations(seqs=world.genomes)
     world.update_cells(genome_idx_pairs=mutated)
 ```
 
 Evolutionary pressure can be applied by selectively killing or replicating cells.
 Here, cells have an increased chance of dying when formiat gets too low
 and an increased chance of replicating when formiat gets high.
 
 ```python
 def sample(p: torch.Tensor) -> list[int]:
     idxs = torch.argwhere(torch.bernoulli(p))
     return idxs.flatten().tolist()
 
-def kill_cells():
+def kill_cells(world: ms.World):
     x = world.cell_molecules[:, 2]
     idxs = sample(.01 / (.01 + x))
     world.kill_cells(cell_idxs=idxs)
 
-def replicate_cells():
+def replicate_cells(world: ms.World):
     x = world.cell_molecules[:, 2]
     idxs = sample(x ** 3 / (x ** 3 + 20.0 ** 3))
     world.divide_cells(cell_idxs=idxs)
 ```
 
 Finally, the simulation itself is run in a python loop by repetitively calling the different steps.
 With `world.enzymatic_activity()` chemical reactions and molecule transport
 in cells advance by one time step.
 `world.diffuse_molecules()` lets molecules on the world map diffuse and permeate through cell membranes
 (if they can) by one time step.
 
 ```python
 for _ in range(1000):
     world.enzymatic_activity()
-    kill_cells()
-    replicate_cells()
-    mutate_cells()
+    kill_cells(world=world)
+    replicate_cells(world=world)
+    mutate_cells(world=world)
     world.diffuse_molecules()
     world.increment_cell_lifetimes()
 ```
 
 See the [Docs](https://magic-soup.readthedocs.io/) for more examples and a description of all the mechanics of this simulation
```

### Comparing `magicsoup-0.4.5/pyproject.toml` & `magicsoup-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/constants.py` & `magicsoup-0.4.6/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/containers.py` & `magicsoup-0.4.6/src/magicsoup/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 class Molecule:
     """
     Represents a molecule species which is part of the world, can diffuse, degrade,
     and be converted into other molecules.
 
     Arguments:
         name: Used to uniquely identify this molecule species.
-        energy: Energy for 1 mol of this molecule species.
-            This amount of energy is released if the molecule would be deconstructed.
-            Energetically coupled in a protein it could power other activities.
-        half_life: Half life of this molecule species in time steps.
+        energy: Energy for 1 mol of this molecule species (in J).
+            This amount of energy is released if the molecule would be deconstructed to nothing.
+        half_life: Half life of this molecule species in time steps (in s by default).
             Molecules degrade by one step if you call `world.degrade_molecules()`.
             Must be > 0.0.
-        diffusivity: A measure for how quick this molecule species diffuses over the molecule map during each time step.
+        diffusivity: A measure for how quick this molecule species diffuses over the molecule map during each time step (in s by default).
             Molecules diffuse when calling `world.diffuse_molecules()`.
             0.0 would mean it doesn't diffuse at all.
             1.0 would mean it is spread out equally around its Moore's neighborhood within one time step.
-        permeability: A measure for how quick this molecule species permeates cell membranes during each time step.
+        permeability: A measure for how quick this molecule species permeates cell membranes during each time step (in s by default).
             Molecules permeate cell membranes when calling `world.diffuse_molecules()`.
             0.0 would mean it can't permeate cell membranes.
             1.0 would mean it spreads equally between cell and molecule map pixel within one time step.
 
     Each molecule species which is supposed to be unique should have a unique `name`.
     In fact, if you initialize a molecule with the same name multiple times,
     only one instance of this molecule will be created.
@@ -41,18 +40,22 @@
     However, this also means that if 2 molecules have the same name, other attributes like e.g. energy must also match:
 
     ```
         atp = Molecule("ATP", 10)
         Molecule("ATP", 20)  # raises error
     ```
 
+    By default in this simulation molecule numbers can be thought of as being in mM, time steps in s, energies in J/mol.
+    Eventually, they are just numbers and can be interpreted as anything.
+    However, together with the default parameters in [Kinetics][magicsoup.kinetics.Kinetics]
+    it makes sense to interpret them in mM, s, and J.
+
     Molecule half life should represent the half life if the molecule is not actively deconstructed by a protein.
     Molecules degrade by one step whenever you call [degrade_molecules()][magicsoup.world.World.degrade_molecules].
     You can setup the simulation to always call [degrade_molecules()][magicsoup.world.World.degrade_molecules] whenever a time step is finished.
-    You could define one time step to equal one second and then use the real half life value for your molecule species.
 
     Molecular diffusion in the 2D molecule map happens whenever you call [diffuse_molecules()][magicsoup.world.World.diffuse_molecules].
     The molecule map is `world.molecule_map`.
     It is a 3D tensor where dimension 0 represents all molecule species of the simulation.
     They are ordered in the same way the attribute `molecules` is ordered in the [Chemistry][magicsoup.containers.Chemistry] you defined.
     Dimension 1 represents x-positions and dimension 2 y-positions.
     Diffusion is implemented as a 2D convolution over the x-y tensor for each molecule species.
```

### Comparing `magicsoup-0.4.5/src/magicsoup/examples/co2_fixing.py` & `magicsoup-0.4.6/src/magicsoup/examples/co2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.4.6/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.4.6/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.4.6/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/genetics.py` & `magicsoup-0.4.6/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/kinetics.py` & `magicsoup-0.4.6/src/magicsoup/kinetics.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,14 +320,20 @@
 
     When this class is initialized it generates the mappings from nucleotide sequences to domains by random sampling.
     These mappings are then used throughout the simulation.
     If you initialize this class again, these mappings will be different.
     Initializing [World][magicsoup.world.World] will also create one `Kinetics` instance. It is on `world.kinetics`.
     If you want to access nucleotide to domain mappings of your simulation, you should use `world.kinetics`.
 
+    Note: All default values are based on the assumption that energies are in J, a time step represents 1s,
+    and molecule numbers are in mM
+    If you change the defaults, you might reconsider how these numbers should be interpreted.
+    If you lower the minimum `Km` or raise the maximum `Vmax`, please also note the comments about
+    `n_computation` and `alpha` below.
+
     The kinetics used here can never create negative molecule concentrations and make the reaction quotient move
     towards to equilibrium constant at all times.
     However, this simulation computes these things one step at a time
     (with the premise that one step should be something similar to 1s).
     This and the numerical limits of data types used here can create edge cases that need to be dealth with:
     reaction quotients overshooting the equilibrium state and negative concentrations.
     Both are caused by high $V_{max}$ with low $K_m$ values.
```

### Comparing `magicsoup-0.4.5/src/magicsoup/mutations.py` & `magicsoup-0.4.6/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/util.py` & `magicsoup-0.4.6/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/src/magicsoup/world.py` & `magicsoup-0.4.6/src/magicsoup/world.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,22 +69,22 @@
         genomes: A list of cell genomes. Each cell's index in this list is what is referred to as the cell index.
             The cell index is used for the same cell in other orderings of cells (_e.g._ `labels`, `cell_divisions`, `cell_molecules`).
         labels: List of cell labels. Cells are ordered as in `world.genomes`. Labels are strings that can be used to
             track cell origins. When adding new cells (`world.add_cells()`) a random label is assigned to each cell.
             If a cell divides, its descendants will have the same label.
         cell_map: Boolean 2D tensor referencing which pixels are occupied by a cell.
             Dimension 0 represents the x, dimension 1 y.
-        molecule_map: Float 3D tensor describing how many molecules (in mmol) of each molecule species exist on every pixel in this world.
+        molecule_map: Float 3D tensor describing concentrations (in mM by default) for each molecule species on each pixel in this world.
             Dimension 0 describes the molecule species. They are in the same order as `chemistry.molecules`.
             Dimension 1 represents x, dimension 2 y.
             So, `world.molecule_map[0, 1, 2]` is number of molecules of the 0th molecule species on pixel 1, 2.
-        cell_molecules: Float 2D tensor describing the number of molecules (in mmol) for each molecule species in each cell.
+        cell_molecules: Float 2D tensor describing concentrations (in mM by default) for each molecule species in each cell.
             Dimension 0 is the cell index. It is the same as in `world.genomes` and the same as on a cell object (`cell.idx`).
             Dimension 1 describes the molecule species. They are in the same order as `chemistry.molecules`.
-            So, `world.cell_molecules[0, 1]` represents how many mmol of the 1st molecule species the 0th cell contains.
+            So, `world.cell_molecules[0, 1]` represents concentration in mM of the 1st molecule species the 0th cell.
         cell_lifetimes: Integer 1D tensor describing how many time steps each cell survived since the last division.
             This tensor is for monitoring and doesn't have any other effect.
             Cells are in the same as in `world.genomes` and the same as on a cell object (`cell.idx`).
         cell_divisions: Integer 1D tensor describing how many times each cell's ancestors divided.
             This tensor is for monitoring and doesn't have any other effect.
             Cells are in the same order as in `world.genomes` and the same as on a cell object (`cell.idx`).
 
@@ -106,18 +106,24 @@
     Furthermore, there are methods for saving and loading a simulation.
     For any new simulation use [save()][magicsoup.world.World.save] once to save the whole world object (with chemistry, genetics, kinetics)
     to a pickle file. You can restore it with [from_file()][magicsoup.world.World.from_file] later on.
     Then, to save the world's state you can use [save_state()][magicsoup.world.World.save_state].
     This is a quick, lightweight save, but it only saves things that change during the simulation.
     Use [load_state()][magicsoup.world.World.load_state] to re-load a certain state.
 
-    Finally, the `world` object carries `world.genetics`, `world.kinetics`, and `world.chemistry`
+    The `world` object carries `world.genetics`, `world.kinetics`, and `world.chemistry`
     (which is just a reference to the chemistry object that was used when initializing `world`).
     Usually, you don't need to touch them.
     But, if you want to override them or look into some details, see the docstrings of their classes for more information.
+
+    By default in this simulation molecule numbers can be thought of as being in mM, time steps in s, energies J/mol.
+    Eventually, they are just numbers and can be interpreted as anything.
+    However, with the default parameters in [Kinetics][magicsoup.kinetics.Kinetics]
+    and the way [Molecule][magicsoup.containers.Molecule] objects are defined
+    it makes sense to interpret them in mM, s, and J.
     """
 
     def __init__(
         self,
         chemistry: Chemistry,
         map_size: int = 128,
         abs_temp: float = 310.0,
@@ -667,15 +673,15 @@
         new_ys = new_pos[:, 1]
 
         self.cell_map[new_xs, new_ys] = True
         self.cell_positions[cell_idxs] = new_pos
 
     def enzymatic_activity(self):
         """
-        Catalyze reactions for one time step.
+        Catalyze reactions for one time step (1s by default).
         This includes molecule transport into or out of the cell.
         `world.molecule_map` and `world.cell_molecules` are updated.
         """
         if self.n_cells == 0:
             return
 
         xs = self.cell_positions[:, 0]
@@ -686,15 +692,15 @@
         self.molecule_map[:, xs, ys] = X[:, self._ext_mol_idxs].T
         self.cell_molecules = X[:, self._int_mol_idxs]
 
     @torch.no_grad()
     def diffuse_molecules(self):
         """
         Let molecules in molecule map diffuse and permeate through cell membranes
-        by one time step.
+        by one time step (1s by default).
         `world.molecule_map` and `world.cell_molecules` are updated.
 
         By how much each molcule species diffuses around the world map and permeates
         into or out of cells if defined on the `Molecule` objects itself.
         See `Molecule` for more information.
         """
         n_pxls = self.map_size**2
```

### Comparing `magicsoup-0.4.5/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.4.6/src/magicsoup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.5
+Version: 0.4.6
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
@@ -36,21 +36,21 @@
 This game simulates cell metabolic and transduction pathway evolution.
 Define a 2D world with certain molecules and reactions.
 Add a few cells and create evolutionary pressure by selectively replicating and killing them.
 Then run and see what random mutations can do.
 
 ![random cells](https://raw.githubusercontent.com/mRcSchwering/magic-soup/main/docs/img/animation.gif)
 
-_Cell growth of 1000 cells with different genomes were simulated. Top row: Cell map showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line when energy levels were high, celline 2 when they wer low. Middle and bottom rows: Development of total cell count and molecule species concentrations over time._
+_Cell growth of 1000 cells with different genomes was simulated. Top row: Cell maps showing all cells (left), cellline 1 (middle), and cellline 2 (right). Celline 1 was the fastest growing cell line at high energy levels, celline 2 at low energy levels. Middle and bottom rows: Development of total cell count and molecule concentrations over time._
 
 ### Installation
 
 For CPU alone you can just do:
 
-```
+```bash
 pip install magicsoup
 ```
 
 This simulation relies on [PyTorch](https://pytorch.org/).
 To increase performance you can move calculations to a GPU.
 In this case you should setup PyTorch first before installing MagicSoup.
 To setup pytorch correctly for your GPU see [Get Started (pytorch.org)](https://pytorch.org/get-started/locally/).
@@ -93,50 +93,50 @@
 ```
 
 Cells discover new proteins by chance through mutations.
 In the function below all cells experience 1E-3 random point mutations per nucleotide.
 10% of them will be indels.
 
 ```python
-def mutate_cells():
+def mutate_cells(world: ms.World):
     mutated = ms.point_mutations(seqs=world.genomes)
     world.update_cells(genome_idx_pairs=mutated)
 ```
 
 Evolutionary pressure can be applied by selectively killing or replicating cells.
 Here, cells have an increased chance of dying when formiat gets too low
 and an increased chance of replicating when formiat gets high.
 
 ```python
 def sample(p: torch.Tensor) -> list[int]:
     idxs = torch.argwhere(torch.bernoulli(p))
     return idxs.flatten().tolist()
 
-def kill_cells():
+def kill_cells(world: ms.World):
     x = world.cell_molecules[:, 2]
     idxs = sample(.01 / (.01 + x))
     world.kill_cells(cell_idxs=idxs)
 
-def replicate_cells():
+def replicate_cells(world: ms.World):
     x = world.cell_molecules[:, 2]
     idxs = sample(x ** 3 / (x ** 3 + 20.0 ** 3))
     world.divide_cells(cell_idxs=idxs)
 ```
 
 Finally, the simulation itself is run in a python loop by repetitively calling the different steps.
 With `world.enzymatic_activity()` chemical reactions and molecule transport
 in cells advance by one time step.
 `world.diffuse_molecules()` lets molecules on the world map diffuse and permeate through cell membranes
 (if they can) by one time step.
 
 ```python
 for _ in range(1000):
     world.enzymatic_activity()
-    kill_cells()
-    replicate_cells()
-    mutate_cells()
+    kill_cells(world=world)
+    replicate_cells(world=world)
+    mutate_cells(world=world)
     world.diffuse_molecules()
     world.increment_cell_lifetimes()
 ```
 
 See the [Docs](https://magic-soup.readthedocs.io/) for more examples and a description of all the mechanics of this simulation
```

### Comparing `magicsoup-0.4.5/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.4.6/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/tests/test_containers.py` & `magicsoup-0.4.6/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/tests/test_genetics.py` & `magicsoup-0.4.6/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/tests/test_kinetics.py` & `magicsoup-0.4.6/tests/test_kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/tests/test_kinetics_integration.py` & `magicsoup-0.4.6/tests/test_kinetics_integration.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/tests/test_mutations.py` & `magicsoup-0.4.6/tests/test_mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/tests/test_util.py` & `magicsoup-0.4.6/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/tests/test_world.py` & `magicsoup-0.4.6/tests/test_world.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.5/tests/test_world_integration.py` & `magicsoup-0.4.6/tests/test_world_integration.py`

 * *Files identical despite different names*

