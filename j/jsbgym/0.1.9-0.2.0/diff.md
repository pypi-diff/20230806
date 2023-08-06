# Comparing `tmp/jsbgym-0.1.9.tar.gz` & `tmp/jsbgym-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsbgym-0.1.9.tar", last modified: Sat May 27 04:13:12 2023, max compression
+gzip compressed data, was "jsbgym-0.2.0.tar", last modified: Sun Aug  6 11:51:14 2023, max compression
```

## Comparing `jsbgym-0.1.9.tar` & `jsbgym-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.954995 jsbgym-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-27 04:12:57.000000 jsbgym-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 04:12:57.000000 jsbgym-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-27 04:13:12.954995 jsbgym-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-27 04:12:57.000000 jsbgym-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.950995 jsbgym-0.1.9/jsbgym/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.954995 jsbgym-0.1.9/jsbgym/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/aircraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/assessors.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/basic_ic.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/flightgear.xml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/minimal_ic.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.954995 jsbgym-0.1.9/jsbgym/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/manual_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_assessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_geodetic_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/tests/test_visualiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-05-27 04:12:57.000000 jsbgym-0.1.9/jsbgym/visualiser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:13:12.954995 jsbgym-0.1.9/jsbgym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 04:13:12.000000 jsbgym-0.1.9/jsbgym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-27 04:12:57.000000 jsbgym-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 04:13:12.954995 jsbgym-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:51:14.722613 jsbgym-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-06 11:51:05.000000 jsbgym-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:51:05.000000 jsbgym-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-06 11:51:14.722613 jsbgym-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-08-06 11:51:05.000000 jsbgym-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:51:14.718613 jsbgym-0.2.0/jsbgym/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:51:14.722613 jsbgym-0.2.0/jsbgym/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/aircraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/assessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/basic_ic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/flightgear.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/minimal_ic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:51:14.722613 jsbgym-0.2.0/jsbgym/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/manual_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_assessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_geodetic_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/tests/test_visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-08-06 11:51:05.000000 jsbgym-0.2.0/jsbgym/visualiser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:51:14.722613 jsbgym-0.2.0/jsbgym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-06 11:51:14.000000 jsbgym-0.2.0/jsbgym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-06 11:51:14.000000 jsbgym-0.2.0/jsbgym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:51:14.000000 jsbgym-0.2.0/jsbgym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:51:14.000000 jsbgym-0.2.0/jsbgym.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-06 11:51:14.000000 jsbgym-0.2.0/jsbgym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 11:51:14.000000 jsbgym-0.2.0/jsbgym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-06 11:51:05.000000 jsbgym-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:51:14.722613 jsbgym-0.2.0/setup.cfg
```

### Comparing `jsbgym-0.1.9/LICENSE` & `jsbgym-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/PKG-INFO` & `jsbgym-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 Metadata-Version: 2.1
 Name: jsbgym
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
 Author: sryu1
 License: MIT
 Project-URL: Homepage, https://github.com/sryu1/jsbgym
 Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSBGym
 
-[![Python: 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Python: 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
 [![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-> **Note**: This library will only work with Windows.
-
 JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
 
+![Example](docs/J3.gif)
+
+Pretrained models can be found [here](https://huggingface.co/sryu1/jsbgym_models)
+
 ## Setup
 
-Firstly, install [JSBSim](https://github.com/JSBSim-Team/jsbsim). Make sure that it is installed in `C:/JSBSim`
+Open a terminal and install jsbgym:
 
-If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). If you have installed the aircraft to a different location, add the folder to the `FG_AIRCRAFT` system variable.
-3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+```console
+pip install jsbgym
+```
+
+For Linux systems, rendering with "human" mode will require an additional package:
 
 ```console
-fgfs --version
+sudo apt-get install python3-tk
 ```
 
-Open the console and install jsbgym:
+To render the environment with FlightGear, dowloand and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). For Linux, rename the AppImage file to fgfs.AppImage and place it in /usr/local/bin/fgfs. The data file must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
 
 ```console
-pip install jsbgym
+export FG_ROOT=/path/to/folder
+```
+
+If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
+3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+
+```console
+fgfs --version
 ```
 
 ## Getting Started
 
 ```python
 import jsbgym
 import gymnasium as gym
@@ -62,44 +73,46 @@
 
 ```python
 f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
 ```
 
 ### Aircraft
 
-The environment can be configured to use one of Six aircraft:
+The environment can be configured to use one of seven aircraft:
 
 * **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
 * **PA28** Piper PA-28-161 Warrior II
 * **J3** Piper J-3 Cub
 * **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
 * **F16** General Dynamics F-16CJ Block 52
+* **OV10** North American OV-10A USAFE Bronco
 * **A320** Airbus A320 (A320 Familiy in Flightgear)
 * **B747** Boeing 747-400
+* **MD11** McDonnell Douglas MD-11
 
 All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
 
 ### Task
 
 JSBGym implements two tasks for controlling the altitude and heading of aircraft:
 
-* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
-* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
+* **HeadingControlTask** aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
+* **TurnHeadingControlTask** aircraft must turn to face a random target heading while maintaining their initial altitude
 
 ### Shaping
 
 The environment can use three different shaping types:
 
 * **Shaping.STANDARD**
 * **Shaping.EXTRA**
 * **Shaping.EXTRA_SEQUENTIAL**
 
 ### FlightGear
 
-If using FlightGear as a render mode, use "FG", if not, use "NoFG"
+If using FlightGear as a render mode, use `FG`, if not, use `NoFG`
 
 ### Environment ID
 
 To fly a Cessna on the Heading Control task withoug using FlightGear,
 
 ```python
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0")
@@ -154,11 +167,7 @@
  Actions are 3-tuples of floats in the range [-1,+1] describing commands to move the aircraft's control surfaces (ailerons, elevator, rudder):
 
  ```python
  (name='fcs/aileron-cmd-norm', description='aileron commanded position, normalised', min=-1.0, max=1.0)
  (name='fcs/elevator-cmd-norm', description='elevator commanded position, normalised', min=-1.0, max=1.0)
  (name='fcs/rudder-cmd-norm', description='rudder commanded position, normalised', min=-1.0, max=1.0)
  ```
-
-## Known Issues
-
-* A320 has and error when rendering with flightgear.
```

### Comparing `jsbgym-0.1.9/README.md` & `jsbgym-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 # JSBGym
 
-[![Python: 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Python: 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
 [![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-> **Note**: This library will only work with Windows.
-
 JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
 
+![Example](docs/J3.gif)
+
+Pretrained models can be found [here](https://huggingface.co/sryu1/jsbgym_models)
+
 ## Setup
 
-Firstly, install [JSBSim](https://github.com/JSBSim-Team/jsbsim). Make sure that it is installed in `C:/JSBSim`
+Open a terminal and install jsbgym:
 
-If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). If you have installed the aircraft to a different location, add the folder to the `FG_AIRCRAFT` system variable.
-3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+```console
+pip install jsbgym
+```
+
+For Linux systems, rendering with "human" mode will require an additional package:
 
 ```console
-fgfs --version
+sudo apt-get install python3-tk
 ```
 
-Open the console and install jsbgym:
+To render the environment with FlightGear, dowloand and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). For Linux, rename the AppImage file to fgfs.AppImage and place it in /usr/local/bin/fgfs. The data file must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
 
 ```console
-pip install jsbgym
+export FG_ROOT=/path/to/folder
+```
+
+If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
+3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+
+```console
+fgfs --version
 ```
 
 ## Getting Started
 
 ```python
 import jsbgym
 import gymnasium as gym
@@ -43,44 +55,46 @@
 
 ```python
 f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
 ```
 
 ### Aircraft
 
-The environment can be configured to use one of Six aircraft:
+The environment can be configured to use one of seven aircraft:
 
 * **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
 * **PA28** Piper PA-28-161 Warrior II
 * **J3** Piper J-3 Cub
 * **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
 * **F16** General Dynamics F-16CJ Block 52
+* **OV10** North American OV-10A USAFE Bronco
 * **A320** Airbus A320 (A320 Familiy in Flightgear)
 * **B747** Boeing 747-400
+* **MD11** McDonnell Douglas MD-11
 
 All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
 
 ### Task
 
 JSBGym implements two tasks for controlling the altitude and heading of aircraft:
 
-* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
-* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
+* **HeadingControlTask** aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
+* **TurnHeadingControlTask** aircraft must turn to face a random target heading while maintaining their initial altitude
 
 ### Shaping
 
 The environment can use three different shaping types:
 
 * **Shaping.STANDARD**
 * **Shaping.EXTRA**
 * **Shaping.EXTRA_SEQUENTIAL**
 
 ### FlightGear
 
-If using FlightGear as a render mode, use "FG", if not, use "NoFG"
+If using FlightGear as a render mode, use `FG`, if not, use `NoFG`
 
 ### Environment ID
 
 To fly a Cessna on the Heading Control task withoug using FlightGear,
 
 ```python
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0")
@@ -135,11 +149,7 @@
  Actions are 3-tuples of floats in the range [-1,+1] describing commands to move the aircraft's control surfaces (ailerons, elevator, rudder):
 
  ```python
  (name='fcs/aileron-cmd-norm', description='aileron commanded position, normalised', min=-1.0, max=1.0)
  (name='fcs/elevator-cmd-norm', description='elevator commanded position, normalised', min=-1.0, max=1.0)
  (name='fcs/rudder-cmd-norm', description='rudder commanded position, normalised', min=-1.0, max=1.0)
  ```
-
-## Known Issues
-
-* A320 has and error when rendering with flightgear.
```

### Comparing `jsbgym-0.1.9/jsbgym/__init__.py` & `jsbgym-0.2.0/jsbgym/__init__.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/agents/agents.py` & `jsbgym-0.2.0/jsbgym/agents/agents.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/aircraft.py` & `jsbgym-0.2.0/jsbgym/aircraft.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,9 +21,11 @@
 
 
 cessna172P = Aircraft("c172p", "c172p", "Cessna172P", 120)
 pa28 = Aircraft("pa28", "PA28-161-180", "PA28", 130)
 j3 = Aircraft("J3Cub", "J3Cub", "J3", 70)
 f15 = Aircraft("f15", "f15c", "F15", 500)
 f16 = Aircraft("f16", "f16-block-52", "F16", 550)
-a320 = Aircraft("A320", "A320-200-CFM", "A320", 480)
-b747 = Aircraft("B747", "747-400", "B747", 490)
+ov10 = Aircraft("OV10", "OV10_USAFE", "OV10", 200)
+a320 = Aircraft("A320", "A320-200-CFM", "A320", 250)
+b747 = Aircraft("B747", "747-400", "B747", 250)
+md11 = Aircraft("MD11", "MD-11", "MD11", 250)
```

### Comparing `jsbgym-0.1.9/jsbgym/assessors.py` & `jsbgym-0.2.0/jsbgym/assessors.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/basic_ic.xml` & `jsbgym-0.2.0/jsbgym/basic_ic.xml`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/environment.py` & `jsbgym-0.2.0/jsbgym/environment.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/flightgear.xml` & `jsbgym-0.2.0/jsbgym/flightgear.xml`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/properties.py` & `jsbgym-0.2.0/jsbgym/properties.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/rewards.py` & `jsbgym-0.2.0/jsbgym/rewards.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/simulation.py` & `jsbgym-0.2.0/jsbgym/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class Simulation(object):
     """
     A class which wraps an instance of JSBSim and manages communication with it.
     """
 
     encoding = "utf-8"  # encoding of bytes returned by JSBSim Cython funcs
-    ROOT_DIR = os.path.abspath("C:\JSBSim")
+    ROOT_DIR = os.path.abspath(jsbsim.__path__[0])
     OUTPUT_FILE = "flightgear.xml"
     LONGITUDINAL = "longitudinal"
     FULL = "full"
 
     def __init__(
         self,
         sim_frequency_hz: float = 60.0,
```

### Comparing `jsbgym-0.1.9/jsbgym/tasks.py` & `jsbgym-0.2.0/jsbgym/tasks.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/manual_tests.py` & `jsbgym-0.2.0/jsbgym/tests/manual_tests.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/stubs.py` & `jsbgym-0.2.0/jsbgym/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_agents.py` & `jsbgym-0.2.0/jsbgym/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_assessors.py` & `jsbgym-0.2.0/jsbgym/tests/test_assessors.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_environment.py` & `jsbgym-0.2.0/jsbgym/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_functional.py` & `jsbgym-0.2.0/jsbgym/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_geodetic_position.py` & `jsbgym-0.2.0/jsbgym/tests/test_geodetic_position.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_rewards.py` & `jsbgym-0.2.0/jsbgym/tests/test_rewards.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_simulation.py` & `jsbgym-0.2.0/jsbgym/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_tasks.py` & `jsbgym-0.2.0/jsbgym/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/tests/test_visualiser.py` & `jsbgym-0.2.0/jsbgym/tests/test_visualiser.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/jsbgym/utils.py` & `jsbgym-0.2.0/jsbgym/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import operator
 from typing import Tuple
-from jsbgym.aircraft import cessna172P, a320, f15, pa28, b747, f16, j3
+from jsbgym.aircraft import cessna172P, a320, f15, pa28, b747, f16, j3, md11, ov10
 from typing import Dict, Iterable
 
 
 class AttributeFormatter(object):
     """
     Replaces characters that would be illegal in an attribute name
 
@@ -39,15 +39,15 @@
 def get_env_id_kwargs_map() -> Dict[str, Tuple]:
     """Returns all environment IDs mapped to tuple of (task, aircraft, shaping, flightgear)"""
     # lazy import to avoid circular dependencies
     from jsbgym.tasks import Shaping, HeadingControlTask, TurnHeadingControlTask
 
     map = {}
     for task_type in (HeadingControlTask, TurnHeadingControlTask):
-        for plane in (cessna172P, a320, f15, pa28, b747, f16, j3):
+        for plane in (cessna172P, a320, f15, pa28, b747, f16, j3, md11, ov10):
             for shaping in (Shaping.STANDARD, Shaping.EXTRA, Shaping.EXTRA_SEQUENTIAL):
                 for enable_flightgear in (True, False):
                     id = get_env_id(plane, task_type, shaping, enable_flightgear)
                     assert id not in map
                     map[id] = (plane, task_type, shaping, enable_flightgear)
     return map
```

### Comparing `jsbgym-0.1.9/jsbgym/visualiser.py` & `jsbgym-0.2.0/jsbgym/visualiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import gymnasium as gym
 import subprocess
 import time
 import os
+import matplotlib as mpt
 import matplotlib.pyplot as plt
 import jsbgym.properties as prp
 from jsbgym.aircraft import Aircraft
 from jsbgym.simulation import Simulation
 from typing import NamedTuple, Tuple
 
 
@@ -50,14 +51,15 @@
         self.value_texts: Tuple[plt.Text] = None
 
     def plot(self, sim: Simulation) -> None:
         """
         Creates or updates a 3D plot of the episode.
         :param sim: Simulation that will be plotted
         """
+        mpt.use("TkAgg")
         if not self.figure:
             self.figure, self.axes = self._plot_configure()
 
         # delete old control surface data points
         for subplot in self.axes[1:]:
             # pop and translate all data points
             while subplot.lines:
@@ -267,15 +269,16 @@
 
     TYPE = "socket"
     DIRECTION = "in"
     RATE = 60
     SERVER = ""
     PORT = 5550
     PROTOCOL = "udp"
-    LOADED_MESSAGE = "Starting hard-coded terrain presampling"
+    LOADED_MESSAGE = "loading cities done"
+    LOADED_MESSAGE1 = "Starting hard-coded terrain presampling"
     FLIGHTGEAR_TIME_FACTOR = 1  # sim speed relative to realtime, higher is faster
     TIME = "morning"
 
     def __init__(
         self, sim: Simulation, print_props: Tuple[prp.Property], block_until_loaded=True
     ):
         """
@@ -347,17 +350,17 @@
             disable_live_weather_arg,
             time_of_day_arg,
         )
 
     def _block_until_flightgear_loaded(self):
         while True:
             msg_out = self.flightgear_process.stdout.readline().decode()
-            if self.LOADED_MESSAGE in msg_out:
+            if self.LOADED_MESSAGE in msg_out or self.LOADED_MESSAGE1 in msg_out:
                 time.sleep(5)
-                print("FlightGear loading complete")
+                print("FlightGear Loading Complete")
                 break
             else:
                 time.sleep(0.1)
 
     def close(self):
         if self.flightgear_process:
             self.flightgear_process.kill()
```

### Comparing `jsbgym-0.1.9/jsbgym.egg-info/PKG-INFO` & `jsbgym-0.2.0/jsbgym.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 Metadata-Version: 2.1
 Name: jsbgym
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
 Author: sryu1
 License: MIT
 Project-URL: Homepage, https://github.com/sryu1/jsbgym
 Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSBGym
 
-[![Python: 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Python: 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
 [![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-> **Note**: This library will only work with Windows.
-
 JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
 
+![Example](docs/J3.gif)
+
+Pretrained models can be found [here](https://huggingface.co/sryu1/jsbgym_models)
+
 ## Setup
 
-Firstly, install [JSBSim](https://github.com/JSBSim-Team/jsbsim). Make sure that it is installed in `C:/JSBSim`
+Open a terminal and install jsbgym:
 
-If you would like to render the environment with FlightGear, install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`)and there is a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). If you have installed the aircraft to a different location, add the folder to the `FG_AIRCRAFT` system variable.
-3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+```console
+pip install jsbgym
+```
+
+For Linux systems, rendering with "human" mode will require an additional package:
 
 ```console
-fgfs --version
+sudo apt-get install python3-tk
 ```
 
-Open the console and install jsbgym:
+To render the environment with FlightGear, dowloand and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). For Linux, rename the AppImage file to fgfs.AppImage and place it in /usr/local/bin/fgfs. The data file must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
 
 ```console
-pip install jsbgym
+export FG_ROOT=/path/to/folder
+```
+
+If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
+3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+
+```console
+fgfs --version
 ```
 
 ## Getting Started
 
 ```python
 import jsbgym
 import gymnasium as gym
@@ -62,44 +73,46 @@
 
 ```python
 f"{aircraft}-{task}-{shaping}-{flightgear}-v0"
 ```
 
 ### Aircraft
 
-The environment can be configured to use one of Six aircraft:
+The environment can be configured to use one of seven aircraft:
 
 * **Cessna172P** Cessna 172P Skyhawk (Default FlightGear Aircraft)
 * **PA28** Piper PA-28-161 Warrior II
 * **J3** Piper J-3 Cub
 * **F15** McDonnell Douglas F-15C Eagle (F-15C in FlightGear)
 * **F16** General Dynamics F-16CJ Block 52
+* **OV10** North American OV-10A USAFE Bronco
 * **A320** Airbus A320 (A320 Familiy in Flightgear)
 * **B747** Boeing 747-400
+* **MD11** McDonnell Douglas MD-11
 
 All aircraft except the Cessna 172P requires the aircraft to be downloaded via the launcher using the default FlightGear Hangar.
 
 ### Task
 
 JSBGym implements two tasks for controlling the altitude and heading of aircraft:
 
-* **HeadingControlTask**: aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
-* **TurnHeadingControlTask**: aircraft must turn to face a random target heading while maintaining their initial altitude
+* **HeadingControlTask** aircraft must fly in a straight line, maintaining its initial altitude and direction of travel (heading)
+* **TurnHeadingControlTask** aircraft must turn to face a random target heading while maintaining their initial altitude
 
 ### Shaping
 
 The environment can use three different shaping types:
 
 * **Shaping.STANDARD**
 * **Shaping.EXTRA**
 * **Shaping.EXTRA_SEQUENTIAL**
 
 ### FlightGear
 
-If using FlightGear as a render mode, use "FG", if not, use "NoFG"
+If using FlightGear as a render mode, use `FG`, if not, use `NoFG`
 
 ### Environment ID
 
 To fly a Cessna on the Heading Control task withoug using FlightGear,
 
 ```python
 env = gym.make("Cessna172P-HeadingControlTask-Shaping.STANDARD-NoFG-v0")
@@ -154,11 +167,7 @@
  Actions are 3-tuples of floats in the range [-1,+1] describing commands to move the aircraft's control surfaces (ailerons, elevator, rudder):
 
  ```python
  (name='fcs/aileron-cmd-norm', description='aileron commanded position, normalised', min=-1.0, max=1.0)
  (name='fcs/elevator-cmd-norm', description='elevator commanded position, normalised', min=-1.0, max=1.0)
  (name='fcs/rudder-cmd-norm', description='rudder commanded position, normalised', min=-1.0, max=1.0)
  ```
-
-## Known Issues
-
-* A320 has and error when rendering with flightgear.
```

### Comparing `jsbgym-0.1.9/jsbgym.egg-info/SOURCES.txt` & `jsbgym-0.2.0/jsbgym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsbgym-0.1.9/pyproject.toml` & `jsbgym-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsbgym"
-version = "0.1.9"
+version = "0.2.0"
 authors = [{ name = "sryu1" }]
 readme = "README.md"
 license = { text = "MIT" }
 description = "A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model."
 classifiers = [
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = ["numpy", "gymnasium", "jsbsim", "matplotlib"]
 
 [project.urls]
 Homepage = "https://github.com/sryu1/jsbgym"
 "Bug Tracker" = "https://github.com/sryu1/jsbgym/issues"
```

