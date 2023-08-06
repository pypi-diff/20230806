# Comparing `tmp/pyGrained-1.0.2.tar.gz` & `tmp/pyGrained-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGrained-1.0.2.tar", last modified: Fri May  5 15:37:19 2023, max compression
+gzip compressed data, was "pyGrained-1.0.3.tar", last modified: Sun Aug  6 10:37:34 2023, max compression
```

## Comparing `pyGrained-1.0.2.tar` & `pyGrained-1.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.919853 pyGrained-1.0.2/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-01-03 17:19:11.000000 pyGrained-1.0.2/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       71 2023-05-03 14:59:01.000000 pyGrained-1.0.2/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2711 2023-05-05 15:37:19.919853 pyGrained-1.0.2/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2051 2023-01-03 18:53:54.000000 pyGrained-1.0.2/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.915853 pyGrained-1.0.2/pyGrained/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    27509 2023-05-05 13:55:29.000000 pyGrained-1.0.2/pyGrained/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.915853 pyGrained-1.0.2/pyGrained/data/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     3579 2023-03-24 16:55:13.000000 pyGrained-1.0.2/pyGrained/data/BetancourtThirumalaiEnergyParm.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)    54297 2023-03-24 17:03:10.000000 pyGrained-1.0.2/pyGrained/data/KaranicolasBrooksDiheParm.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)     4303 2023-03-24 17:05:26.000000 pyGrained-1.0.2/pyGrained/data/MiyazawaJerniga1999EnergyParm.json
--rw-------   0 pablo     (1000) pablo     (1000)     3573 2023-03-24 17:06:13.000000 pyGrained-1.0.2/pyGrained/data/MiyazawaJernigaEnergyParm.json
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      231 2023-03-17 18:40:11.000000 pyGrained-1.0.2/pyGrained/data/aminoacidCharges.json
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      306 2023-03-17 18:40:18.000000 pyGrained-1.0.2/pyGrained/data/aminoacidMasses.json
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      218 2023-03-17 18:40:26.000000 pyGrained-1.0.2/pyGrained/data/aminoacidRadii.json
--rw-------   0 pablo     (1000) pablo     (1000)      277 2023-03-24 16:52:18.000000 pyGrained-1.0.2/pyGrained/data/aminoacidRndCoilSASA.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)      280 2023-03-24 16:51:17.000000 pyGrained-1.0.2/pyGrained/data/aminoacids.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)       75 2023-03-24 16:52:57.000000 pyGrained-1.0.2/pyGrained/data/atomMasses.json
--rw-r--r--   0 pablo     (1000) pablo     (1000)       46 2023-03-24 16:48:30.000000 pyGrained-1.0.2/pyGrained/data/atomRadiiSobolev.json
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.915853 pyGrained-1.0.2/pyGrained/models/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    19150 2023-05-05 13:44:28.000000 pyGrained-1.0.2/pyGrained/models/AlphaCarbon.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    20193 2023-05-05 15:26:26.000000 pyGrained-1.0.2/pyGrained/models/SBCG.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-05 09:33:49.000000 pyGrained-1.0.2/pyGrained/models/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.919853 pyGrained-1.0.2/pyGrained/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      187 2023-03-18 18:27:20.000000 pyGrained-1.0.2/pyGrained/utils/SASA.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-18 16:17:48.000000 pyGrained-1.0.2/pyGrained/utils/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3625 2023-03-23 17:54:04.000000 pyGrained-1.0.2/pyGrained/utils/atomList.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4645 2023-03-24 16:47:01.000000 pyGrained-1.0.2/pyGrained/utils/bonds.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3778 2023-04-25 10:35:41.000000 pyGrained-1.0.2/pyGrained/utils/coarseGrained.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.919853 pyGrained-1.0.2/pyGrained/utils/computeK/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-17 18:13:15.000000 pyGrained-1.0.2/pyGrained/utils/computeK/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2022-12-23 23:49:41.000000 pyGrained-1.0.2/pyGrained/utils/computeK/computeK.cpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      905 2023-03-24 18:28:04.000000 pyGrained-1.0.2/pyGrained/utils/geometric.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    11144 2023-05-05 12:56:26.000000 pyGrained-1.0.2/pyGrained/utils/nativeContacts.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      582 2023-03-24 10:35:09.000000 pyGrained-1.0.2/pyGrained/utils/output.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      387 2023-03-18 17:23:11.000000 pyGrained-1.0.2/pyGrained/utils/sequence.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1284 2023-05-05 14:42:46.000000 pyGrained-1.0.2/pyGrained/utils/trajectory.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 15:37:19.915853 pyGrained-1.0.2/pyGrained.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2711 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1126 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       25 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       10 2023-05-05 15:37:19.000000 pyGrained-1.0.2/pyGrained.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      802 2023-05-05 15:36:24.000000 pyGrained-1.0.2/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-05 15:37:19.919853 pyGrained-1.0.2/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      582 2023-05-03 15:03:41.000000 pyGrained-1.0.2/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-08-06 10:37:34.671119 pyGrained-1.0.3/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-01-03 17:19:11.000000 pyGrained-1.0.3/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       71 2023-05-03 14:59:01.000000 pyGrained-1.0.3/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2711 2023-08-06 10:37:34.671119 pyGrained-1.0.3/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2051 2023-01-03 18:53:54.000000 pyGrained-1.0.3/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-08-06 10:37:34.667119 pyGrained-1.0.3/pyGrained/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    27509 2023-05-05 13:55:29.000000 pyGrained-1.0.3/pyGrained/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-08-06 10:37:34.667119 pyGrained-1.0.3/pyGrained/data/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     3579 2023-03-24 16:55:13.000000 pyGrained-1.0.3/pyGrained/data/BetancourtThirumalaiEnergyParm.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)    54297 2023-03-24 17:03:10.000000 pyGrained-1.0.3/pyGrained/data/KaranicolasBrooksDiheParm.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     4303 2023-03-24 17:05:26.000000 pyGrained-1.0.3/pyGrained/data/MiyazawaJerniga1999EnergyParm.json
+-rw-------   0 pablo     (1000) pablo     (1000)     3573 2023-03-24 17:06:13.000000 pyGrained-1.0.3/pyGrained/data/MiyazawaJernigaEnergyParm.json
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      231 2023-03-17 18:40:11.000000 pyGrained-1.0.3/pyGrained/data/aminoacidCharges.json
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      306 2023-03-17 18:40:18.000000 pyGrained-1.0.3/pyGrained/data/aminoacidMasses.json
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      218 2023-03-17 18:40:26.000000 pyGrained-1.0.3/pyGrained/data/aminoacidRadii.json
+-rw-------   0 pablo     (1000) pablo     (1000)      277 2023-03-24 16:52:18.000000 pyGrained-1.0.3/pyGrained/data/aminoacidRndCoilSASA.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      280 2023-03-24 16:51:17.000000 pyGrained-1.0.3/pyGrained/data/aminoacids.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       75 2023-03-24 16:52:57.000000 pyGrained-1.0.3/pyGrained/data/atomMasses.json
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       46 2023-03-24 16:48:30.000000 pyGrained-1.0.3/pyGrained/data/atomRadiiSobolev.json
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-08-06 10:37:34.667119 pyGrained-1.0.3/pyGrained/models/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    19450 2023-07-02 16:42:24.000000 pyGrained-1.0.3/pyGrained/models/AlphaCarbon.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    23390 2023-06-26 15:57:31.000000 pyGrained-1.0.3/pyGrained/models/SBCG.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-05 09:33:49.000000 pyGrained-1.0.3/pyGrained/models/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-08-06 10:37:34.671119 pyGrained-1.0.3/pyGrained/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      187 2023-03-18 18:27:20.000000 pyGrained-1.0.3/pyGrained/utils/SASA.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-18 16:17:48.000000 pyGrained-1.0.3/pyGrained/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3625 2023-03-23 17:54:04.000000 pyGrained-1.0.3/pyGrained/utils/atomList.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4645 2023-03-24 16:47:01.000000 pyGrained-1.0.3/pyGrained/utils/bonds.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3778 2023-04-25 10:35:41.000000 pyGrained-1.0.3/pyGrained/utils/coarseGrained.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-08-06 10:37:34.671119 pyGrained-1.0.3/pyGrained/utils/computeK/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-17 18:13:15.000000 pyGrained-1.0.3/pyGrained/utils/computeK/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      645 2022-12-23 23:49:41.000000 pyGrained-1.0.3/pyGrained/utils/computeK/computeK.cpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      905 2023-03-24 18:28:04.000000 pyGrained-1.0.3/pyGrained/utils/geometric.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    11144 2023-05-05 12:56:26.000000 pyGrained-1.0.3/pyGrained/utils/nativeContacts.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1011 2023-07-02 15:43:20.000000 pyGrained-1.0.3/pyGrained/utils/output.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      387 2023-03-18 17:23:11.000000 pyGrained-1.0.3/pyGrained/utils/sequence.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1284 2023-05-05 14:42:46.000000 pyGrained-1.0.3/pyGrained/utils/trajectory.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-08-06 10:37:34.667119 pyGrained-1.0.3/pyGrained.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2711 2023-08-06 10:37:34.000000 pyGrained-1.0.3/pyGrained.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1126 2023-08-06 10:37:34.000000 pyGrained-1.0.3/pyGrained.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-08-06 10:37:34.000000 pyGrained-1.0.3/pyGrained.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       25 2023-08-06 10:37:34.000000 pyGrained-1.0.3/pyGrained.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       10 2023-08-06 10:37:34.000000 pyGrained-1.0.3/pyGrained.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      802 2023-07-24 15:22:08.000000 pyGrained-1.0.3/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-08-06 10:37:34.671119 pyGrained-1.0.3/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      582 2023-05-03 15:03:41.000000 pyGrained-1.0.3/setup.py
```

### Comparing `pyGrained-1.0.2/LICENSE` & `pyGrained-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/PKG-INFO` & `pyGrained-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGrained
-Version: 1.0.2
+Version: 1.0.3
 Summary: Coarse grained library for Python
 Home-page: https://github.com/PabloIbannez/pyGrained
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyGrained-1.0.2/README.md` & `pyGrained-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/__init__.py` & `pyGrained-1.0.3/pyGrained/__init__.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/data/BetancourtThirumalaiEnergyParm.json` & `pyGrained-1.0.3/pyGrained/data/BetancourtThirumalaiEnergyParm.json`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/data/KaranicolasBrooksDiheParm.json` & `pyGrained-1.0.3/pyGrained/data/KaranicolasBrooksDiheParm.json`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/data/MiyazawaJerniga1999EnergyParm.json` & `pyGrained-1.0.3/pyGrained/data/MiyazawaJerniga1999EnergyParm.json`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/data/MiyazawaJernigaEnergyParm.json` & `pyGrained-1.0.3/pyGrained/data/MiyazawaJernigaEnergyParm.json`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/models/AlphaCarbon.py` & `pyGrained-1.0.3/pyGrained/models/AlphaCarbon.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,23 @@
 
     def __init__(self,
                  name:str,
                  inputPDBfilePath:str,
                  params:dict,
                  debug = False):
 
+        self.logger.info(f"Creating SelfOrganizedPolymer object {name} from {inputPDBfilePath}")
+
         fixPDB = params.get("fixPDB",False)
+        self.logger.info(f"Fixing PDB: {fixPDB}")
+
+        modelParams = params.get("parameters",{})
+
+        epsNC  = modelParams.get("epsilonNC",1.0)
+        self.logger.info(f"epsilonNC: {epsNC}")
 
         super().__init__(name   = name,
                          inputPDBfilePath = inputPDBfilePath,
                          fixPDB = fixPDB,
                          params = params,
                          debug  = debug)
 
@@ -219,15 +227,15 @@
             pos_i = beads[id_i].get_coord()
             pos_j = beads[id_j].get_coord()
             r0 = np.linalg.norm(pos_i-pos_j)
             forceField["bonds"]["data"].append([id_i,id_j,r0])
 
         forceField["nativeContacts"] = {}
         forceField["nativeContacts"]["type"]       = ["Bond2","LennardJonesType2Common_epsilon"]
-        forceField["nativeContacts"]["parameters"] = {"epsilon":1.0}
+        forceField["nativeContacts"]["parameters"] = {"epsilon":epsNC}
         forceField["nativeContacts"]["labels"]     = ["id_i", "id_j", "sigma"]
         forceField["nativeContacts"]["data"]       = []
 
         for nc in nativeContacts:
             id_i,id_j = nc
             pos_i = beads[id_i].get_coord()
             pos_j = beads[id_j].get_coord()
```

### Comparing `pyGrained-1.0.2/pyGrained/models/SBCG.py` & `pyGrained-1.0.3/pyGrained/models/SBCG.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,14 +100,63 @@
         bondBeads = {bnd:0 for bnd in set(bondBeadsTmp)}
 
         for bnd in bondBeadsTmp:
             bondBeads[bnd]+=1
 
         return bondBeads
 
+    def __generateCountBonds(self,structure,cgMap):
+
+        atom2bead = {}
+        chainsCg = set()
+        #Invert map
+        for bead,atomsList in cgMap.items():
+            chId      = bead[1]
+            chainsCg.add(chId) #Not all chains can be in the cg model
+
+            beadIndex = bead[4]
+            for atm in atomsList:
+                atomIndex = atm[4]
+                atom2bead[atomIndex] = beadIndex
+
+        atomsCA      = [atm for atm in structure.get_atoms() if atm.get_name() == "CA"]
+        atomsCACoord = np.asarray([atm.get_coord() for atm in structure.get_atoms() if atm.get_name() == "CA"])
+
+        kd = cKDTree(atomsCACoord)
+        bondCAAtoms = kd.query_pairs(5.0)
+
+        bondBeadsTmp = []
+        for bnd in bondCAAtoms:
+
+            mdl1Index = atomsCA[bnd[0]].get_parent().get_parent().get_parent().get_id()
+            mdl2Index = atomsCA[bnd[1]].get_parent().get_parent().get_parent().get_id()
+
+            ch1Index = atomsCA[bnd[0]].get_parent().get_parent().get_id()
+            ch2Index = atomsCA[bnd[1]].get_parent().get_parent().get_id()
+
+            res1Index = atomsCA[bnd[0]].get_parent().get_id()[1]
+            res2Index = atomsCA[bnd[1]].get_parent().get_id()[1]
+
+            if (ch1Index in chainsCg) and (ch2Index in chainsCg):
+                if ch1Index == ch2Index and mdl1Index == mdl2Index:
+                    if abs(res1Index-res2Index) == 1:
+                        bead1Index = atom2bead[atomsCA[bnd[0]].get_serial_number()]
+                        bead2Index = atom2bead[atomsCA[bnd[1]].get_serial_number()]
+                        if bead1Index != bead2Index:
+                            bondBeadsTmp.append((bead1Index,bead2Index))
+            else:
+                self.logger.debug(f"While generating enm, the chain {ch1Index} or the chain {ch2Index} has been found in the all atom model but not in CG")
+
+        bondBeads = {bnd:0 for bnd in set(bondBeadsTmp)}
+
+        for bnd in bondBeadsTmp:
+            bondBeads[bnd]+=1
+
+        return bondBeads
+
     def __generateNC(self,structure,cgMap,ncCut,n):
 
         atom2bead = {}
         chainsCg = set()
         #Invert map
         for bead,atomsList in cgMap.items():
             chId      = bead[1]
@@ -361,46 +410,35 @@
         self.logger.info(f"Generating bonds ...")
 
         bondsModelName = bondsModel["name"]
         if bondsModelName == "ENM":
             self.logger.info(f"Generating ENM bonds ...")
             enmCut = bondsModel["parameters"]["enmCut"]
             bonds = self.__generateENM(self.getSpreadedStructure(),spreadedCgMap,enmCut)
+        elif bondsModelName == "count":
+            self.logger.info(f"Generating count bonds ...")
+            bonds = self.__generateCountBonds(self.getSpreadedStructure(),spreadedCgMap)
         else:
             self.logger.error(f"Bonds model {bondsModelName} is not availble")
             raise Exception(f"Bonds model not available")
 
         self.logger.info(f"Generating native contacts ...")
 
         nativeContacsModelName = nativeContactsModel["name"]
-        if nativeContacsModelName == "CA":
+        if nativeContacsModelName == "CA" or nativeContacsModelName == "count":
             self.logger.info(f"Generating CA native contacts ...")
-            ncCut = nativeContactsModel["parameters"]["ncCut"]
+            if "parameters" in nativeContactsModel:
+                ncCut = nativeContactsModel["parameters"].get("ncCut",8.0)
+            else:
+                ncCut = 8.0
             nativeContacts = self.__generateNC(self.getSpreadedStructure(),spreadedCgMap,ncCut,2)
         else:
             self.logger.error(f"Native contacts model {nativeContacsModelName} is not availble")
             raise Exception(f"Native contacts model not available")
 
-        #########################################
-
-        exclusions = {}
-
-        for bead in spreadedCgStructure.get_atoms():
-            exclusions[bead.get_serial_number()]=set()
-
-        for bnd in bonds.keys():
-            id_i,id_j = bnd
-            exclusions[id_i].add(id_j)
-            exclusions[id_j].add(id_i)
-
-        for nc in nativeContacts.keys():
-            id_i,id_j = nc
-            exclusions[id_i].add(id_j)
-            exclusions[id_j].add(id_i)
-
         self.logger.info(f"Topology generation end")
 
         #########################################
 
         #ForceField
 
         self.logger.info(f"Generating force field ...")
@@ -421,14 +459,27 @@
 
             for bnd in bonds.keys():
                 id_i,id_j = bnd
                 pos_i = beads[id_i].get_coord()
                 pos_j = beads[id_j].get_coord()
                 r0 = np.linalg.norm(pos_i-pos_j)
                 forceField["bonds"]["data"].append([id_i,id_j,r0])
+        elif bondsModelName == "count":
+            forceField["bonds"] = {}
+            forceField["bonds"]["type"]       = ["Bond2","r0Count"]
+            forceField["bonds"]["parameters"] = {}
+            forceField["bonds"]["labels"] = ["id_i", "id_j", "r0", "n"]
+            forceField["bonds"]["data"]   = []
+
+            for bnd in bonds.keys():
+                id_i,id_j = bnd
+                pos_i = beads[id_i].get_coord()
+                pos_j = beads[id_j].get_coord()
+                r0 = np.linalg.norm(pos_i-pos_j)
+                forceField["bonds"]["data"].append([id_i,id_j,r0,bonds[bnd]])
         else:
             self.logger.error(f"Bonds model {bondsModelName} is not availble")
             raise Exception(f"Bonds model not available")
 
         #Native contacts
         if nativeContacsModelName == "CA":
             forceField["nativeContacts"] = {}
@@ -441,14 +492,28 @@
                 id_i,id_j = nc
                 pos_i = beads[id_i].get_coord()
                 pos_j = beads[id_j].get_coord()
                 dst = round(np.linalg.norm(pos_i-pos_j),3)
                 E   = nativeContactsModel["parameters"]["epsilon"]*nativeContacts[nc]
                 D   = nativeContactsModel["parameters"]["D"]
                 forceField["nativeContacts"]["data"].append([id_i,id_j,dst,E,D])
+        elif nativeContacsModelName == "count":
+
+            forceField["nativeContacts"] = {}
+            forceField["nativeContacts"]["type"]       = ["Bond2","roCount"]
+            forceField["nativeContacts"]["parameters"] = {}
+            forceField["nativeContacts"]["labels"]     = ["id_i", "id_j", "r0", "n"]
+            forceField["nativeContacts"]["data"]       = []
+
+            for nc in nativeContacts.keys():
+                id_i,id_j = nc
+                pos_i = beads[id_i].get_coord()
+                pos_j = beads[id_j].get_coord()
+                dst = round(np.linalg.norm(pos_i-pos_j),3)
+                forceField["nativeContacts"]["data"].append([id_i,id_j,dst,nativeContacts[nc]])
         else:
             self.logger.error(f"Native contacts model {nativeContacsModelName} is not availble")
             raise Exception(f"Native contacts model not available")
 
         #Verlet list
 
         forceField["nl"] = {}
```

### Comparing `pyGrained-1.0.2/pyGrained/utils/atomList.py` & `pyGrained-1.0.3/pyGrained/utils/atomList.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/utils/bonds.py` & `pyGrained-1.0.3/pyGrained/utils/bonds.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/utils/coarseGrained.py` & `pyGrained-1.0.3/pyGrained/utils/coarseGrained.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/utils/computeK/computeK.cpp` & `pyGrained-1.0.3/pyGrained/utils/computeK/computeK.cpp`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/utils/geometric.py` & `pyGrained-1.0.3/pyGrained/utils/geometric.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/utils/nativeContacts.py` & `pyGrained-1.0.3/pyGrained/utils/nativeContacts.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained/utils/trajectory.py` & `pyGrained-1.0.3/pyGrained/utils/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyGrained.egg-info/PKG-INFO` & `pyGrained-1.0.3/pyGrained.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGrained
-Version: 1.0.2
+Version: 1.0.3
 Summary: Coarse grained library for Python
 Home-page: https://github.com/PabloIbannez/pyGrained
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyGrained-1.0.2/pyGrained.egg-info/SOURCES.txt` & `pyGrained-1.0.3/pyGrained.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGrained-1.0.2/pyproject.toml` & `pyGrained-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="pyGrained"
-version="1.0.2"
+version="1.0.3"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "Coarse grained library for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

### Comparing `pyGrained-1.0.2/setup.py` & `pyGrained-1.0.3/setup.py`

 * *Files identical despite different names*

