# Comparing `tmp/teneva_bm-0.7.1.tar.gz` & `tmp/teneva_bm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.7.1.tar", last modified: Fri Aug  4 11:55:05 2023, max compression
+gzip compressed data, was "teneva_bm-0.7.2.tar", last modified: Sun Aug  6 12:05:58 2023, max compression
```

## Comparing `teneva_bm-0.7.1.tar` & `teneva_bm-0.7.2.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.565480 teneva_bm-0.7.1/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.7.1/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.7.1/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    19956 2023-08-04 11:55:05.565716 teneva_bm-0.7.1/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)    18695 2023-08-04 11:51:29.000000 teneva_bm-0.7.1/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.7.1/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.7.1/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-04 11:55:05.566424 teneva_bm-0.7.1/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.7.1/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.530841 teneva_bm-0.7.1/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      211 2023-08-04 11:51:18.000000 teneva_bm-0.7.1/teneva_bm/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.539025 teneva_bm-0.7.1/teneva_bm/agent/
--rw-r--r--   0 andrei     (501) staff       (20)      409 2023-08-04 11:48:43.000000 teneva_bm-0.7.1/teneva_bm/agent/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7561 2023-08-02 11:35:35.000000 teneva_bm-0.7.1/teneva_bm/agent/agent.py
--rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_ant.py
--rw-r--r--   0 andrei     (501) staff       (20)     2114 2023-08-04 11:40:40.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_cheetah.py
--rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_human.py
--rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_human_stand.py
--rw-r--r--   0 andrei     (501) staff       (20)     7432 2023-08-02 12:46:42.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_lake.py
--rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_pend_inv.py
--rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_pend_inv_double.py
--rw-r--r--   0 andrei     (501) staff       (20)     2100 2023-08-04 11:48:23.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_reacher.py
--rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.7.1/teneva_bm/agent/bm_agent_swimmer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.7.1/teneva_bm/agent/policy.py
--rw-r--r--   0 andrei     (501) staff       (20)    35400 2023-08-04 11:50:27.000000 teneva_bm-0.7.1/teneva_bm/bm.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.546337 teneva_bm-0.7.1/teneva_bm/func/
--rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.7.1/teneva_bm/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     3641 2023-08-02 10:12:25.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3623 2023-08-02 10:10:43.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     3130 2023-08-02 10:10:09.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3165 2023-08-02 10:10:07.000000 teneva_bm-0.7.1/teneva_bm/func/bm_func_schwefel.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.548519 teneva_bm-0.7.1/teneva_bm/hs/
--rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.7.1/teneva_bm/hs/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.7.1/teneva_bm/hs/bm_hs_func001.py
--rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.7.1/teneva_bm/hs/bm_hs_func006.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.553973 teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
--rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
--rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
--rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
--rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.557980 teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
--rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
--rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
--rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
--rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.560001 teneva_bm-0.7.1/teneva_bm/odeoc/
--rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.7.1/teneva_bm/odeoc/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4218 2023-08-02 10:06:50.000000 teneva_bm-0.7.1/teneva_bm/odeoc/bm_odeoc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.7.1/teneva_bm/odeoc/bm_odeoc_simple_constr.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.562833 teneva_bm-0.7.1/teneva_bm/qubo/
--rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.7.1/teneva_bm/qubo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.7.1/teneva_bm/qubo/bm_qubo_knap_det.py
--rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.7.1/teneva_bm/qubo/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2962 2023-08-02 10:05:08.000000 teneva_bm-0.7.1/teneva_bm/qubo/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2968 2023-08-02 10:04:56.000000 teneva_bm-0.7.1/teneva_bm/qubo/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.7.1/teneva_bm/teneva_bm_demo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.564777 teneva_bm-0.7.1/teneva_bm/various/
--rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.7.1/teneva_bm/various/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7774 2023-08-02 10:24:54.000000 teneva_bm-0.7.1/teneva_bm/various/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)    12683 2023-08-02 10:23:16.000000 teneva_bm-0.7.1/teneva_bm/various/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.7.1/teneva_bm/various/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 11:55:05.533591 teneva_bm-0.7.1/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    19956 2023-08-04 11:55:05.000000 teneva_bm-0.7.1/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2384 2023-08-04 11:55:05.000000 teneva_bm-0.7.1/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-04 11:55:05.000000 teneva_bm-0.7.1/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-08-04 11:55:05.000000 teneva_bm-0.7.1/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-08-04 11:55:05.000000 teneva_bm-0.7.1/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.877107 teneva_bm-0.7.2/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.7.2/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.7.2/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    19872 2023-08-06 12:05:58.877315 teneva_bm-0.7.2/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    18611 2023-08-06 12:04:15.000000 teneva_bm-0.7.2/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.7.2/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.7.2/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-06 12:05:58.878231 teneva_bm-0.7.2/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.7.2/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.833621 teneva_bm-0.7.2/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      211 2023-08-06 12:04:10.000000 teneva_bm-0.7.2/teneva_bm/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.844985 teneva_bm-0.7.2/teneva_bm/agent/
+-rw-r--r--   0 andrei     (501) staff       (20)      452 2023-08-06 10:02:09.000000 teneva_bm-0.7.2/teneva_bm/agent/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7615 2023-08-06 09:59:09.000000 teneva_bm-0.7.2/teneva_bm/agent/agent.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_ant.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2114 2023-08-04 11:40:40.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_cheetah.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_human.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_human_stand.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7445 2023-08-06 09:58:29.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_lake.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2258 2023-08-06 11:17:21.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_lander.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_pend_inv.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_pend_inv_double.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2100 2023-08-04 11:48:23.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_reacher.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_swimmer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.7.2/teneva_bm/agent/policy.py
+-rw-r--r--   0 andrei     (501) staff       (20)    35400 2023-08-04 13:13:26.000000 teneva_bm-0.7.2/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.853047 teneva_bm-0.7.2/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.7.2/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3641 2023-08-02 10:12:25.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3623 2023-08-02 10:10:43.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3130 2023-08-02 10:10:09.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3165 2023-08-02 10:10:07.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.854750 teneva_bm-0.7.2/teneva_bm/hs/
+-rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.7.2/teneva_bm/hs/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.7.2/teneva_bm/hs/bm_hs_func001.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.7.2/teneva_bm/hs/bm_hs_func006.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.860406 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.868365 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.871395 teneva_bm-0.7.2/teneva_bm/odeoc/
+-rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.7.2/teneva_bm/odeoc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4218 2023-08-02 10:06:50.000000 teneva_bm-0.7.2/teneva_bm/odeoc/bm_odeoc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.7.2/teneva_bm/odeoc/bm_odeoc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.874750 teneva_bm-0.7.2/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.7.2/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_knap_det.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2782 2023-08-06 12:03:27.000000 teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2845 2023-08-06 12:01:41.000000 teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.7.2/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.876677 teneva_bm-0.7.2/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.7.2/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7774 2023-08-02 10:24:54.000000 teneva_bm-0.7.2/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    12683 2023-08-02 10:23:16.000000 teneva_bm-0.7.2/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.7.2/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.837409 teneva_bm-0.7.2/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    19872 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2419 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.7.1/LICENSE.txt` & `teneva_bm-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/PKG-INFO` & `teneva_bm-0.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_bm
-Version: 0.7.1
+Version: 0.7.2
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,32 +30,32 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.7.1".
-
-The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
-
-> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
-
-Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
-
-- Collections `func`, `hs` and `various` do not require installation of additional libraries.
-
-- Сollections `odeoc` and `qubo` require installation of the following libraries:
+1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
+    pip install teneva_bm==0.7.2
     ```
+    > The package can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and be installed by `python setup.py install` command from the root folder of the project.
 
-- Сollection `agent` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+2. Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the script [install_all.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_all.py) for existing [anaconda](https://www.anaconda.com) environment `ENV_NAME` (except the colab platform, where `env` flag should not be used):
+    ```bash
+    conda create --name ENV_NAME python=3.8 -y
+    wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py
+    python install_all.py --env ENV_NAME --silent
+    ```
+    > Please note that the collection `agent` requires a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so the script `install_all.py` is rather complicated. You can find mode details for using this script in the header of the file.
 
-> To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.4`).
+3. To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer:
+    ```bash
+    pip install protes==0.3.4
+    ```
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
@@ -71,15 +71,15 @@
 ```
 
 > We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer). We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentCheetah`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentReacher`, `BmAgentSwimmer`.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentCheetah`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentLander`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentReacher`, `BmAgentSwimmer`.
     > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (if `direct` policy name is set) or discrete Toeplitz policy may be used (if `toeplitz` policy name is set; it is the default value); you can also set your own custom policy as an instance of the correct class (see `agent/policy.py` for details).
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
@@ -89,15 +89,15 @@
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
 ## Usage
 
-A typical scenario for working with a benchmark is as follows.
+A typical scenario for working with any benchmark from our package is as follows.
 
 ##### Benchmark initialization
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
```

### Comparing `teneva_bm-0.7.1/README.md` & `teneva_bm-0.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.7.1".
-
-The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
-
-> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
-
-Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
-
-- Collections `func`, `hs` and `various` do not require installation of additional libraries.
-
-- Сollections `odeoc` and `qubo` require installation of the following libraries:
+1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
+    pip install teneva_bm==0.7.2
     ```
+    > The package can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and be installed by `python setup.py install` command from the root folder of the project.
 
-- Сollection `agent` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+2. Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the script [install_all.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_all.py) for existing [anaconda](https://www.anaconda.com) environment `ENV_NAME` (except the colab platform, where `env` flag should not be used):
+    ```bash
+    conda create --name ENV_NAME python=3.8 -y
+    wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py
+    python install_all.py --env ENV_NAME --silent
+    ```
+    > Please note that the collection `agent` requires a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so the script `install_all.py` is rather complicated. You can find mode details for using this script in the header of the file.
 
-> To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.4`).
+3. To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer:
+    ```bash
+    pip install protes==0.3.4
+    ```
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
@@ -45,15 +45,15 @@
 ```
 
 > We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer). We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentCheetah`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentReacher`, `BmAgentSwimmer`.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentCheetah`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentLander`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentReacher`, `BmAgentSwimmer`.
     > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (if `direct` policy name is set) or discrete Toeplitz policy may be used (if `toeplitz` policy name is set; it is the default value); you can also set your own custom policy as an instance of the correct class (see `agent/policy.py` for details).
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
@@ -63,15 +63,15 @@
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
 ## Usage
 
-A typical scenario for working with a benchmark is as follows.
+A typical scenario for working with any benchmark from our package is as follows.
 
 ##### Benchmark initialization
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
```

### Comparing `teneva_bm-0.7.1/demo.py` & `teneva_bm-0.7.2/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/setup.py` & `teneva_bm-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/agent.py` & `teneva_bm-0.7.2/teneva_bm/agent/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,26 +179,27 @@
 
         self.set_dimension(self._policy.d)
         self.set_size(self._n_raw)
         if self.is_func:
             self.set_grid(self._policy.a, self._policy.b)
         self._reset()
 
-    def render(self, fpath=None, i=None, best=True, fps=20.):
+    def render(self, fpath=None, i=None, best=True, fps=20., sz=None):
         self._with_render = True
         i, y = self.get_solution(i, best)
         self._with_render = False
 
         if not len(self._frames):
             msg = 'Can not save rendered video for agent (empty frames)'
             self.wrn(msg)
 
         frames = self._frames
         frames = [cv2.cvtColor(frame, cv2.COLOR_RGB2BGR) for frame in frames]
-        # frame = cv2.resize(frame,(512, 512))
+        if sz is not None:
+            frames = [cv2.resize(frame, sz) for frame in frames]
 
         fpath = self.path_build(fpath, 'mp4')
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         out = cv2.VideoWriter(fpath, fourcc, fps, (frames[0].shape[:2]))
         for frame in frames:
             out.write(frame)
         out.release()
```

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_ant.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_ant.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_cheetah.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_cheetah.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_human.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_human.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_human_stand.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_human_stand.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_lake.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_lake.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,16 +188,16 @@
 
         env = Agent.make('FrozenLake-v1', desc=self._map, is_slippery=False)
 
         self._state_goal = self._discretize(self.size*self.size-1)
 
         return super().prep_bm(env)
 
-    def render(self, fpath=None, i=None, best=True, fps=5.):
-        return super().render(fpath, i, best, fps)
+    def render(self, fpath=None, i=None, best=True, fps=5., sz=None):
+        return super().render(fpath, i, best, fps, sz)
 
     def _discretize(self, state):
         x, y = (state // self.size, state % self.size)
         return np.array([x, y], dtype=int)
 
     def _parse_action_gym(self, action):
         return action[0]
```

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_pend_inv.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_pend_inv.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_pend_inv_double.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_pend_inv_double.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_reacher.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_reacher.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/bm_agent_swimmer.py` & `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_swimmer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/agent/policy.py` & `teneva_bm-0.7.2/teneva_bm/agent/policy.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/bm.py` & `teneva_bm-0.7.2/teneva_bm/bm.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/__init__.py` & `teneva_bm-0.7.2/teneva_bm/func/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_ackley.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_ackley.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_alpine.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_alpine.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_dixon.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_dixon.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_exp.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_exp.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_griewank.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_griewank.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_michalewicz.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_michalewicz.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_piston.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_piston.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_qing.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_qing.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_rastrigin.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_rastrigin.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_rosenbrock.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_schaffer.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_schaffer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/func/bm_func_schwefel.py` & `teneva_bm-0.7.2/teneva_bm/func/bm_func_schwefel.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/bm_hs_func001.py` & `teneva_bm-0.7.2/teneva_bm/hs/bm_hs_func001.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/bm_hs_func006.py` & `teneva_bm-0.7.2/teneva_bm/hs/bm_hs_func006.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs007.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs007.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs008.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs008.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs009.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs009.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs010.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs010.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs011.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs011.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_constrained_functions/bm_hs012.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs012.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py` & `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/odeoc/bm_odeoc_simple.py` & `teneva_bm-0.7.2/teneva_bm/odeoc/bm_odeoc_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/odeoc/bm_odeoc_simple_constr.py` & `teneva_bm-0.7.2/teneva_bm/odeoc/bm_odeoc_simple_constr.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/qubo/bm_qubo_knap_det.py` & `teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_knap_det.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/qubo/bm_qubo_knap_quad.py` & `teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/qubo/bm_qubo_maxcut.py` & `teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,25 @@
     with_qubogen = False
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Quadratic unconstrained binary optimization (QUBO) Max-Cut problem
-    represented as a discrete function. The dimension may be any (default
-    is 100), and the mode size should be 2. The benchmark needs
-    "networkx==3.0" and "qubogen==0.1.1" libraries.
+    Quadratic unconstrained binary optimization (QUBO) Minimum Vertex Cover
+    (MVC) problem represented as a discrete function. The dimension may be
+    any (default is 100), and the mode size should be 2. The default value
+    of the probability of the connection in the graph if 0.5 (pcon).
+    The benchmark needs "networkx==3.0" and "qubogen==0.1.1" libraries.
+    TODO: fix inner bm name from "QuboMVC" to "QuboMvc".
 """
 
 
-class BmQuboMaxcut(Bm):
-    def __init__(self, d=100, n=2, name='QuboMaxcut', desc=DESC):
+class BmQuboMvc(Bm):
+    def __init__(self, d=100, n=2, name='QuboMVC', desc=DESC, pcon=0.5):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
@@ -39,65 +41,56 @@
             self.set_err(msg)
 
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
+        self.pcon = pcon
+
     @property
     def identity(self):
-        return ['d', 'seed']
+        return ['d', 'pcon', 'seed']
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['prob_con'] = self.prob_con
+        conf['pcon'] = self.pcon
         return conf
 
     def info(self, footer=''):
         text = ''
 
-        text += 'Param prob_con (connection probability)  : '
-        v = self.prob_con
+        text += 'Param pcon (connection probability)      : '
+        v = self.pcon
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self):
         d = self.d
-        p = self.prob_con
+        p = self.pcon
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
-        self._Q = qubogen.qubo_max_cut(g)
-
-    def set_opts(self, prob_con=0.5):
-        """Setting options specific to the benchmark.
-
-        There are no plans to manually change the default values.
-
-        Args:
-            prob_con (float): probability of the connection in the graph.
-
-        """
-        self.prob_con = prob_con
+        self._Q = qubogen.qubo_mvc(g)
 
     def target_batch(self, I):
         return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmQuboMaxcut().prep()
+    bm = BmQuboMvc().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.7.1/teneva_bm/qubo/bm_qubo_mvc.py` & `teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     with_qubogen = False
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Quadratic unconstrained binary optimization (QUBO) Minimum Vertex Cover
-    (MVC) problem represented as a discrete function. The dimension may be
-    any (default is 100), and the mode size should be 2. The benchmark needs
-    "networkx==3.0" and "qubogen==0.1.1" libraries.
+    Quadratic unconstrained binary optimization (QUBO) Max-Cut problem
+    represented as a discrete function. The dimension may be any (default
+    is 100), and the mode size should be 2. The default value of the
+    probability of the connection in the graph if 0.5 (pcon). The benchmark
+    needs "networkx==3.0" and "qubogen==0.1.1" libraries.
 """
 
 
-class BmQuboMvc(Bm):
-    def __init__(self, d=100, n=2, name='QuboMVC', desc=DESC):
+class BmQuboMaxcut(Bm):
+    def __init__(self, d=100, n=2, name='QuboMaxcut', desc=DESC, pcon=0.5):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
@@ -39,65 +40,56 @@
             self.set_err(msg)
 
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
+        self.pcon = pcon
+
     @property
     def identity(self):
-        return ['d', 'seed']
+        return ['d', 'pcon', 'seed']
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['prob_con'] = self.prob_con
+        conf['pcon'] = self.pcon
         return conf
 
     def info(self, footer=''):
         text = ''
 
-        text += 'Param prob_con (connection probability)  : '
-        v = self.prob_con
+        text += 'Param pcon (connection probability)      : '
+        v = self.pcon
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self):
         d = self.d
-        p = self.prob_con
+        p = self.pcon
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
-        self._Q = qubogen.qubo_mvc(g)
-
-    def set_opts(self, prob_con=0.5):
-        """Setting options specific to the benchmark.
-
-        There are no plans to manually change the default values.
-
-        Args:
-            prob_con (float): probability of the connection in the graph.
-
-        """
-        self.prob_con = prob_con
+        self._Q = qubogen.qubo_max_cut(g)
 
     def target_batch(self, I):
         return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmQuboMvc().prep()
+    bm = BmQuboMaxcut().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.7.1/teneva_bm/teneva_bm_demo.py` & `teneva_bm-0.7.2/teneva_bm/teneva_bm_demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/various/bm_matmul.py` & `teneva_bm-0.7.2/teneva_bm/various/bm_matmul.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/various/bm_topopt.py` & `teneva_bm-0.7.2/teneva_bm/various/bm_topopt.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm/various/bm_wall_simple.py` & `teneva_bm-0.7.2/teneva_bm/various/bm_wall_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.1/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.7.2/teneva_bm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-bm
-Version: 0.7.1
+Version: 0.7.2
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,32 +30,32 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.7.1".
-
-The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
-
-> Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
-
-Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
-
-- Collections `func`, `hs` and `various` do not require installation of additional libraries.
-
-- Сollections `odeoc` and `qubo` require installation of the following libraries:
+1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
+    pip install teneva_bm==0.7.2
     ```
+    > The package can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and be installed by `python setup.py install` command from the root folder of the project.
 
-- Сollection `agent` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+2. Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the script [install_all.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_all.py) for existing [anaconda](https://www.anaconda.com) environment `ENV_NAME` (except the colab platform, where `env` flag should not be used):
+    ```bash
+    conda create --name ENV_NAME python=3.8 -y
+    wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py
+    python install_all.py --env ENV_NAME --silent
+    ```
+    > Please note that the collection `agent` requires a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so the script `install_all.py` is rather complicated. You can find mode details for using this script in the header of the file.
 
-> To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.4`).
+3. To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer:
+    ```bash
+    pip install protes==0.3.4
+    ```
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
@@ -71,15 +71,15 @@
 ```
 
 > We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer). We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentCheetah`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentReacher`, `BmAgentSwimmer`.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentAnt`, `BmAgentCheetah`, `BmAgentHuman`, `BmAgentHumanStand`, `BmAgentLake`, `BmAgentLander`, `BmAgentPendInv`, `BmAgentPendInvDouble`, `BmAgentReacher`, `BmAgentSwimmer`.
     > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (if `direct` policy name is set) or discrete Toeplitz policy may be used (if `toeplitz` policy name is set; it is the default value); you can also set your own custom policy as an instance of the correct class (see `agent/policy.py` for details).
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
@@ -89,15 +89,15 @@
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
 ## Usage
 
-A typical scenario for working with a benchmark is as follows.
+A typical scenario for working with any benchmark from our package is as follows.
 
 ##### Benchmark initialization
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
```

### Comparing `teneva_bm-0.7.1/teneva_bm.egg-info/SOURCES.txt` & `teneva_bm-0.7.2/teneva_bm.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 teneva_bm/agent/__init__.py
 teneva_bm/agent/agent.py
 teneva_bm/agent/bm_agent_ant.py
 teneva_bm/agent/bm_agent_cheetah.py
 teneva_bm/agent/bm_agent_human.py
 teneva_bm/agent/bm_agent_human_stand.py
 teneva_bm/agent/bm_agent_lake.py
+teneva_bm/agent/bm_agent_lander.py
 teneva_bm/agent/bm_agent_pend_inv.py
 teneva_bm/agent/bm_agent_pend_inv_double.py
 teneva_bm/agent/bm_agent_reacher.py
 teneva_bm/agent/bm_agent_swimmer.py
 teneva_bm/agent/policy.py
 teneva_bm/func/__init__.py
 teneva_bm/func/bm_func_ackley.py
```

