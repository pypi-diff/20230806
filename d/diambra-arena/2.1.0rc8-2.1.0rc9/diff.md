# Comparing `tmp/diambra-arena-2.1.0rc8.tar.gz` & `tmp/diambra-arena-2.1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-arena-2.1.0rc8.tar", last modified: Wed Jun  7 20:04:33 2023, max compression
+gzip compressed data, was "diambra-arena-2.1.0rc9.tar", last modified: Sun Jun 11 18:27:28 2023, max compression
```

## Comparing `diambra-arena-2.1.0rc8.tar` & `diambra-arena-2.1.0rc9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16903 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.914884 diambra-arena-2.1.0rc8/diambra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/arena_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/arena_imitation_learning_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/engine/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/env_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/make_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/ray_rllib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/ray_rllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/ray_rllib/make_ray_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/make_sb_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/sb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/p2_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/make_sb3_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/sb3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.922884 diambra-arena-2.1.0rc8/diambra/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   167633 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/.splash_screen.gif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/engine_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/gym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/integratedGames.json
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/splash_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.922884 diambra-arena-2.1.0rc8/diambra/arena/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/arena_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/obs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/obs_wrapper_hardcore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/traj_rec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/diambra_arena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_gym_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_imitation_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5084 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_recording_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_wrappers_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.671248 diambra-arena-2.1.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-06-11 18:27:28.671248 diambra-arena-2.1.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16903 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.655247 diambra-arena-2.1.0rc9/diambra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.655247 diambra-arena-2.1.0rc9/diambra/arena/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/arena_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/arena_imitation_learning_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.655247 diambra-arena-2.1.0rc9/diambra/arena/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/engine/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/env_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/make_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.659247 diambra-arena-2.1.0rc9/diambra/arena/ray_rllib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/ray_rllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/ray_rllib/make_ray_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.659247 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/make_sb_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/sb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.659247 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/p2_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.659247 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/make_sb3_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/sb3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.663248 diambra-arena-2.1.0rc9/diambra/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   167633 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/.splash_screen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/engine_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/gym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/integratedGames.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/splash_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.667248 diambra-arena-2.1.0rc9/diambra/arena/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/arena_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/obs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/obs_wrapper_hardcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/traj_rec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.667248 diambra-arena-2.1.0rc9/diambra_arena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:27:28.671248 diambra-arena-2.1.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.671248 diambra-arena-2.1.0rc9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_gym_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_imitation_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5084 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_recording_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_wrappers_settings.py
```

### Comparing `diambra-arena-2.1.0rc8/LICENSE.txt` & `diambra-arena-2.1.0rc9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/PKG-INFO` & `diambra-arena-2.1.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc8
+Version: 2.1.0rc9
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc8 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc9 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
```

### Comparing `diambra-arena-2.1.0rc8/README.md` & `diambra-arena-2.1.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/arena_gym.py` & `diambra-arena-2.1.0rc9/diambra/arena/arena_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/arena_imitation_learning_gym.py` & `diambra-arena-2.1.0rc9/diambra/arena/arena_imitation_learning_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/engine/interface.py` & `diambra-arena-2.1.0rc9/diambra/arena/engine/interface.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     """Diambra Environment gym interface"""
 
     def __init__(self, env_address, grpc_timeout=60):
         self.logger = logging.getLogger(__name__)
 
         try:
             # Opening gRPC channel
-            self.client = Client(env_address, grpc_timeout)
             self.logger.info("Trying to connect to DIAMBRA Engine server (timeout={}s)...".format(grpc_timeout))
+            self.client = Client(env_address, grpc_timeout)
         except grpc.FutureTimeoutError as e:
             raise Exception(CONNECTION_FAILED_ERROR_TEXT) from e
 
         self.logger.info("... done.")
 
         # Splash Screen
         if 'DISPLAY' in os.environ:
```

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/env_settings.py` & `diambra-arena-2.1.0rc9/diambra/arena/env_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # System level
     step_ratio: int = 6
     disable_keyboard:bool = True
     disable_joystick: bool = True
     rank: int = 0
     seed: int = -1
     env_address: str = "localhost:50051"
-    grpc_timeout: int = 60
+    grpc_timeout: int = 600
 
     # Game level
     player: str = "Random"
     continue_game: float = 0.0
     show_final: bool = True
     difficulty: int = 3
     frame_shape: Tuple[int, int, int] = (0, 0, 0)
@@ -44,15 +44,15 @@
     def sanity_check(self):
         self.games_dict = available_games(False)
 
         # TODO: consider using typing.Literal to specify lists of admissible values: NOTE: It requires Python 3.8+
         check_num_in_range("step_ratio", self.step_ratio, [1, 6])
         check_num_in_range("rank", self.rank, [0, MAX_VAL])
         check_num_in_range("seed", self.seed, [-1, MAX_VAL])
-        check_num_in_range("grpc_timeout", self.grpc_timeout, [0, 120])
+        check_num_in_range("grpc_timeout", self.grpc_timeout, [0, 3600])
 
         check_val_in_list("game_id", self.game_id, self.games_dict.keys())
         check_val_in_list("player", self.player, ["P1", "P2", "Random", "P1P2"])
         check_num_in_range("continue_game", self.continue_game, [MIN_VAL, 1.0])
         check_num_in_range("difficulty", self.difficulty, self.games_dict[self.game_id]["difficulty"][:2])
 
         check_num_in_range("frame_shape[0]", self.frame_shape[0], [0, MAX_FRAME_RES])
```

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/make_env.py` & `diambra-arena-2.1.0rc9/diambra/arena/make_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/ray_rllib/make_ray_env.py` & `diambra-arena-2.1.0rc9/diambra/arena/ray_rllib/make_ray_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/make_sb_env.py` & `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/make_sb_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/sb_utils.py` & `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/sb_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py` & `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/p2_wrap.py` & `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/p2_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py` & `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/make_sb3_env.py` & `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/make_sb3_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/sb3_utils.py` & `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/sb3_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/utils/.splash_screen.gif` & `diambra-arena-2.1.0rc9/diambra/arena/utils/.splash_screen.gif`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/utils/controller.py` & `diambra-arena-2.1.0rc9/diambra/arena/utils/controller.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/utils/engine_mock.py` & `diambra-arena-2.1.0rc9/diambra/arena/utils/engine_mock.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/utils/gym_utils.py` & `diambra-arena-2.1.0rc9/diambra/arena/utils/gym_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/utils/integratedGames.json` & `diambra-arena-2.1.0rc9/diambra/arena/utils/integratedGames.json`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/utils/policies.py` & `diambra-arena-2.1.0rc9/diambra/arena/utils/policies.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/utils/splash_screen.py` & `diambra-arena-2.1.0rc9/diambra/arena/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/wrappers/arena_wrappers.py` & `diambra-arena-2.1.0rc9/diambra/arena/wrappers/arena_wrappers.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/wrappers/obs_wrapper.py` & `diambra-arena-2.1.0rc9/diambra/arena/wrappers/obs_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/wrappers/obs_wrapper_hardcore.py` & `diambra-arena-2.1.0rc9/diambra/arena/wrappers/obs_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/wrappers/traj_rec_wrapper.py` & `diambra-arena-2.1.0rc9/diambra/arena/wrappers/traj_rec_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py` & `diambra-arena-2.1.0rc9/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/diambra_arena.egg-info/PKG-INFO` & `diambra-arena-2.1.0rc9/diambra_arena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc8
+Version: 2.1.0rc9
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc8 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc9 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
```

### Comparing `diambra-arena-2.1.0rc8/diambra_arena.egg-info/SOURCES.txt` & `diambra-arena-2.1.0rc9/diambra_arena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/setup.py` & `diambra-arena-2.1.0rc9/setup.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/tests/test_gym_settings.py` & `diambra-arena-2.1.0rc9/tests/test_gym_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/tests/test_imitation_learning.py` & `diambra-arena-2.1.0rc9/tests/test_imitation_learning.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/tests/test_integration.py` & `diambra-arena-2.1.0rc9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/tests/test_random.py` & `diambra-arena-2.1.0rc9/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/tests/test_recording_settings.py` & `diambra-arena-2.1.0rc9/tests/test_recording_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/tests/test_speed.py` & `diambra-arena-2.1.0rc9/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc8/tests/test_wrappers_settings.py` & `diambra-arena-2.1.0rc9/tests/test_wrappers_settings.py`

 * *Files identical despite different names*

