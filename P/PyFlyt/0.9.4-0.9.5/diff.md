# Comparing `tmp/PyFlyt-0.9.4.tar.gz` & `tmp/PyFlyt-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.9.4.tar", last modified: Fri Jul 28 12:22:31 2023, max compression
+gzip compressed data, was "PyFlyt-0.9.5.tar", last modified: Mon Jul 31 14:32:57 2023, max compression
```

## Comparing `PyFlyt-0.9.4.tar` & `PyFlyt-0.9.5.tar`

### file list

```diff
@@ -1,57 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.593266 PyFlyt-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-28 12:22:31.593266 PyFlyt-0.9.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.585266 PyFlyt-0.9.4/PyFlyt/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.585266 PyFlyt-0.9.4/PyFlyt/core/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.589266 PyFlyt-0.9.4/PyFlyt/core/abstractions/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/base_drone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/base_wind_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/boosters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/boring_bodies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/gimbals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/motors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/abstractions/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/aviary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.589266 PyFlyt-0.9.4/PyFlyt/core/drones/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/drones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/drones/fixedwing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/drones/quadx.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/drones/rocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/load_objs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.589266 PyFlyt-0.9.4/PyFlyt/core/wind/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/core/wind/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.589266 PyFlyt-0.9.4/PyFlyt/gym_envs/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.593266 PyFlyt-0.9.4/PyFlyt/gym_envs/fixedwing_envs/
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.593266 PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.593266 PyFlyt-0.9.4/PyFlyt/gym_envs/rocket_envs/
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/gym_envs/waypoint_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.593266 PyFlyt-0.9.4/PyFlyt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/PyFlyt/utils/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.585266 PyFlyt-0.9.4/PyFlyt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-28 12:22:31.000000 PyFlyt-0.9.4/PyFlyt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-28 12:22:31.000000 PyFlyt-0.9.4/PyFlyt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:22:31.000000 PyFlyt-0.9.4/PyFlyt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 12:22:31.000000 PyFlyt-0.9.4/PyFlyt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 12:22:31.000000 PyFlyt-0.9.4/PyFlyt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:22:31.593266 PyFlyt-0.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:22:31.593266 PyFlyt-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-28 12:22:19.000000 PyFlyt-0.9.4/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.479559 PyFlyt-0.9.5/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.9.5/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4337 2023-07-31 14:32:57.479559 PyFlyt-0.9.5/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.463559 PyFlyt-0.9.5/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-07-26 11:45:21.000000 PyFlyt-0.9.5/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.467559 PyFlyt-0.9.5/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.9.5/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.471559 PyFlyt-0.9.5/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-12 22:54:11.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12160 2023-07-19 16:05:50.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-29 18:39:28.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7999 2023-07-26 11:45:21.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-06-07 19:10:09.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-06-07 19:14:24.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-06-07 19:08:30.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.9.5/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-07-25 10:38:46.000000 PyFlyt-0.9.5/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.471559 PyFlyt-0.9.5/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.9.5/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-29 18:39:28.000000 PyFlyt-0.9.5/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-07-25 10:38:45.000000 PyFlyt-0.9.5/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-29 18:39:28.000000 PyFlyt-0.9.5/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-14 18:31:25.000000 PyFlyt-0.9.5/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.471559 PyFlyt-0.9.5/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.9.5/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.471559 PyFlyt-0.9.5/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.471559 PyFlyt-0.9.5/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9283 2023-07-26 11:45:21.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-05-29 18:39:28.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.471559 PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9017 2023-07-26 11:45:21.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3977 2023-07-19 17:39:31.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-05-29 18:39:28.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.471559 PyFlyt-0.9.5/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11657 2023-07-26 11:45:21.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-07-19 16:01:20.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.9.5/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.475559 PyFlyt-0.9.5/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.9.5/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.9.5/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.9.5/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.463559 PyFlyt-0.9.5/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.475559 PyFlyt-0.9.5/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.475559 PyFlyt-0.9.5/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.475559 PyFlyt-0.9.5/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.475559 PyFlyt-0.9.5/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.479559 PyFlyt-0.9.5/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.9.5/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.479559 PyFlyt-0.9.5/PyFlyt/utils/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       56 2023-07-26 11:45:21.000000 PyFlyt-0.9.5/PyFlyt/utils/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-07-28 12:16:56.000000 PyFlyt-0.9.5/PyFlyt/utils/checks.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.467559 PyFlyt-0.9.5/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4337 2023-07-31 14:32:57.000000 PyFlyt-0.9.5/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2007 2023-07-31 14:32:57.000000 PyFlyt-0.9.5/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-31 14:32:57.000000 PyFlyt-0.9.5/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       68 2023-07-31 14:32:57.000000 PyFlyt-0.9.5/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-31 14:32:57.000000 PyFlyt-0.9.5/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1362 2023-07-31 14:30:37.000000 PyFlyt-0.9.5/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2421 2023-07-19 13:24:00.000000 PyFlyt-0.9.5/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-31 14:32:57.479559 PyFlyt-0.9.5/setup.cfg
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-31 14:32:57.479559 PyFlyt-0.9.5/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9638 2023-07-26 11:45:21.000000 PyFlyt-0.9.5/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5304 2023-07-26 11:45:21.000000 PyFlyt-0.9.5/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.9.4/LICENSE.txt` & `PyFlyt-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PKG-INFO` & `PyFlyt-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.9.4
+Version: 0.9.5
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.9.5/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/aviary.py` & `PyFlyt-0.9.5/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.9.5/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.9.5/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.9.5/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/core/load_objs.py` & `PyFlyt-0.9.5/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.9.5/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt/utils/checks.py` & `PyFlyt-0.9.5/PyFlyt/utils/checks.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.9.5/PyFlyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.9.4
+Version: 0.9.5
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.9.4/pyproject.toml` & `PyFlyt-0.9.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.9.4"
+version = "0.9.5"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -27,15 +27,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["PyFlyt", "PyFlyt.*"]
 
 [tool.setuptools.package-data]
 pyflyt = [
-    "PyFlyt/models/**",
+    "models/**",
 ]
 
 [project.urls]
 Repository = "https://github.com/jjshoots/PyFlyt"
 Documentation = "https://jjshoots.github.io/PyFlyt/documentation.html"
 "Bug Report" = "https://github.com/jjshoots/PyFlyt/issues"
```

### Comparing `PyFlyt-0.9.4/readme.md` & `PyFlyt-0.9.5/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/tests/test_core.py` & `PyFlyt-0.9.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.4/tests/test_gym_envs.py` & `PyFlyt-0.9.5/tests/test_gym_envs.py`

 * *Files identical despite different names*

