# Comparing `tmp/dprox-0.2.tar.gz` & `tmp/dprox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/hyper-pnp/submit/Delta-Prox/dist/.tmp-vstotite/dprox-0.2.tar", last modified: Sun Aug  6 07:52:09 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/hyper-pnp/submit/Delta-Prox/dist/.tmp-kcdapes2/dprox-0.2.1.tar", last modified: Sun Aug  6 17:27:08 2023, max compression
```

## Comparing `dprox-0.2.tar` & `dprox-0.2.1.tar`

### file list

```diff
@@ -1,157 +1,158 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      302 2023-08-06 07:52:09.000000 dprox-0.2/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5423 2023-08-06 07:49:15.000000 dprox-0.2/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      217 2023-08-06 02:06:06.000000 dprox-0.2/dprox/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      375 2023-08-06 07:23:41.000000 dprox-0.2/dprox/algo/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3676 2023-06-17 08:34:57.000000 dprox-0.2/dprox/algo/admm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9623 2023-07-06 07:36:05.000000 dprox-0.2/dprox/algo/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.2/dprox/algo/hqs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      685 2023-05-24 07:17:40.000000 dprox-0.2/dprox/algo/invert.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/lp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.2/dprox/algo/lp/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16158 2023-08-06 02:42:27.000000 dprox-0.2/dprox/algo/lp/solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6540 2023-08-03 11:55:44.000000 dprox-0.2/dprox/algo/lp/utils.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/opt/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/opt/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.2/dprox/algo/opt/absorb.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/opt/equil.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2241 2023-05-22 07:49:41.000000 dprox-0.2/dprox/algo/opt/merge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.2/dprox/algo/pc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/pgd.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5636 2023-08-06 07:26:09.000000 dprox-0.2/dprox/algo/primitives.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3607 2023-08-06 07:22:38.000000 dprox-0.2/dprox/algo/problem.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/specialization/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      126 2023-08-06 07:26:19.000000 dprox-0.2/dprox/algo/specialization/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/specialization/deq/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-06-12 08:45:35.000000 dprox-0.2/dprox/algo/specialization/deq/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3620 2023-07-04 03:59:17.000000 dprox-0.2/dprox/algo/specialization/deq/solver.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3600 2023-06-12 08:46:04.000000 dprox-0.2/dprox/algo/specialization/deq/training.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/specialization/deq/utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/jacobian.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/layer_utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/optimizations.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/radam.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/solvers.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/specialization/rl/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       21 2023-06-12 08:44:42.000000 dprox-0.2/dprox/algo/specialization/rl/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    14224 2023-06-19 14:51:52.000000 dprox-0.2/dprox/algo/specialization/rl/solver.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1875 2023-08-06 07:27:33.000000 dprox-0.2/dprox/algo/specialization/unroll.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/tune/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-12 08:44:51.000000 dprox-0.2/dprox/algo/tune/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2941 2023-08-06 06:03:25.000000 dprox-0.2/dprox/algo/tune/dpir.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/tune/learnable.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/contrib/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-08-05 14:30:04.000000 dprox-0.2/dprox/contrib/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8716 2023-08-06 07:19:08.000000 dprox-0.2/dprox/contrib/csmri.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2563 2023-08-05 13:25:05.000000 dprox-0.2/dprox/contrib/derain.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      953 2023-08-06 01:49:45.000000 dprox-0.2/dprox/contrib/energy_system.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/contrib/optic/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       69 2023-08-05 14:37:30.000000 dprox-0.2/dprox/contrib/optic/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    17055 2023-08-06 07:35:24.000000 dprox-0.2/dprox/contrib/optic/doe_model.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3739 2023-08-06 01:05:50.000000 dprox-0.2/dprox/contrib/optic/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6059 2023-08-06 01:10:44.000000 dprox-0.2/dprox/contrib/optic/utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2497 2023-08-05 13:36:36.000000 dprox-0.2/dprox/contrib/restoration.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/linalg/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-22 11:53:09.000000 dprox-0.2/dprox/linalg/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3314 2023-07-23 02:25:37.000000 dprox-0.2/dprox/linalg/custom.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/linalg/solve/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      335 2023-06-02 14:40:15.000000 dprox-0.2/dprox/linalg/solve/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6513 2023-08-03 11:55:44.000000 dprox-0.2/dprox/linalg/solve/solver_cg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10190 2023-06-02 14:39:42.000000 dprox-0.2/dprox/linalg/solve/solver_minres.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5311 2023-06-12 08:09:04.000000 dprox-0.2/dprox/linalg/solve/solver_plss.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/linop/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      658 2023-07-01 02:33:34.000000 dprox-0.2/dprox/linop/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7715 2023-07-23 02:25:42.000000 dprox-0.2/dprox/linop/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2365 2023-05-24 07:38:28.000000 dprox-0.2/dprox/linop/blackbox.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15257 2023-07-01 02:35:05.000000 dprox-0.2/dprox/linop/comp_graph.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.2/dprox/linop/constaints.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2882 2023-05-24 07:43:37.000000 dprox-0.2/dprox/linop/constant.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5480 2023-05-24 07:43:49.000000 dprox-0.2/dprox/linop/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.2/dprox/linop/edge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.2/dprox/linop/grad.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      489 2023-05-24 06:31:56.000000 dprox-0.2/dprox/linop/placeholder.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2580 2023-05-24 07:43:58.000000 dprox-0.2/dprox/linop/scale.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3459 2023-05-24 07:38:58.000000 dprox-0.2/dprox/linop/subsample.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3051 2023-05-24 07:44:13.000000 dprox-0.2/dprox/linop/sum.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2988 2023-05-24 07:44:22.000000 dprox-0.2/dprox/linop/variable.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3717 2023-05-24 07:44:41.000000 dprox-0.2/dprox/linop/vstack.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      285 2023-05-22 11:53:09.000000 dprox-0.2/dprox/proxfn/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2700 2023-06-07 15:13:18.000000 dprox-0.2/dprox/proxfn/base.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/fast/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/fast/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/fast/cs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      604 2023-05-27 03:46:05.000000 dprox-0.2/dprox/proxfn/fast/csmri.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/fast/pr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/fast/spi.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.2/dprox/proxfn/fast/sr.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/nlm/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/nlm/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/nlm/nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/nlm/patch_nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/nonneg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/norm.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/composite.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_unet.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/wrapper.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3091 2023-08-06 05:32:51.000000 dprox-0.2/dprox/proxfn/pnp/prior.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5751 2023-06-19 10:50:01.000000 dprox-0.2/dprox/proxfn/sum_square.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/unrolling/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/unrolling/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/unrolling/dgu.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      587 2023-07-04 04:49:45.000000 dprox-0.2/dprox/proxfn/unrolling/prior.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      278 2023-08-05 15:59:24.000000 dprox-0.2/dprox/utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1504 2023-08-05 14:24:40.000000 dprox-0.2/dprox/utils/containar.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3204 2023-08-06 05:52:06.000000 dprox-0.2/dprox/utils/huggingface.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/utils/init/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2/dprox/utils/init/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-05-24 04:36:39.000000 dprox-0.2/dprox/utils/init/mosaic.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      756 2023-05-24 04:36:39.000000 dprox-0.2/dprox/utils/init/sr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-08-06 05:29:49.000000 dprox-0.2/dprox/utils/io.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4618 2023-06-27 12:39:39.000000 dprox-0.2/dprox/utils/metrics.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7989 2023-08-05 16:12:43.000000 dprox-0.2/dprox/utils/misc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3978 2023-05-24 04:36:39.000000 dprox-0.2/dprox/utils/psf2otf.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      302 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3981 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      108 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-08-06 07:52:09.000000 dprox-0.2/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      652 2023-08-06 07:39:29.000000 dprox-0.2/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/tests/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2740 2023-08-06 01:53:38.000000 dprox-0.2/tests/test_algorithms.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2675 2023-08-06 01:54:49.000000 dprox-0.2/tests/test_linop.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.2/tests/test_linop_primitive.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      136 2023-08-06 01:55:22.000000 dprox-0.2/tests/test_primitive.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-08-06 17:27:08.000000 dprox-0.2.1/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5577 2023-08-06 17:02:17.000000 dprox-0.2.1/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      217 2023-08-06 02:06:06.000000 dprox-0.2.1/dprox/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/algo/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      375 2023-08-06 07:23:41.000000 dprox-0.2.1/dprox/algo/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3676 2023-06-17 08:34:57.000000 dprox-0.2.1/dprox/algo/admm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9623 2023-07-06 07:36:05.000000 dprox-0.2.1/dprox/algo/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.2.1/dprox/algo/hqs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      685 2023-05-24 07:17:40.000000 dprox-0.2.1/dprox/algo/invert.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/algo/lp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.2.1/dprox/algo/lp/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16158 2023-08-06 02:42:27.000000 dprox-0.2.1/dprox/algo/lp/solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6540 2023-08-03 11:55:44.000000 dprox-0.2.1/dprox/algo/lp/utils.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/algo/opt/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/opt/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.2.1/dprox/algo/opt/absorb.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/opt/equil.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2241 2023-05-22 07:49:41.000000 dprox-0.2.1/dprox/algo/opt/merge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.2.1/dprox/algo/pc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/pgd.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5900 2023-08-06 08:27:22.000000 dprox-0.2.1/dprox/algo/primitives.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3607 2023-08-06 07:22:38.000000 dprox-0.2.1/dprox/algo/problem.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/algo/specialization/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      126 2023-08-06 07:26:19.000000 dprox-0.2.1/dprox/algo/specialization/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/algo/specialization/deq/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-06-12 08:45:35.000000 dprox-0.2.1/dprox/algo/specialization/deq/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3620 2023-07-04 03:59:17.000000 dprox-0.2.1/dprox/algo/specialization/deq/solver.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3600 2023-06-12 08:46:04.000000 dprox-0.2.1/dprox/algo/specialization/deq/training.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/algo/specialization/deq/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/specialization/deq/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/specialization/deq/utils/jacobian.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/specialization/deq/utils/layer_utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/specialization/deq/utils/optimizations.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/specialization/deq/utils/radam.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/specialization/deq/utils/solvers.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/algo/specialization/rl/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       21 2023-06-12 08:44:42.000000 dprox-0.2.1/dprox/algo/specialization/rl/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    14245 2023-08-06 08:28:48.000000 dprox-0.2.1/dprox/algo/specialization/rl/solver.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1875 2023-08-06 07:27:33.000000 dprox-0.2.1/dprox/algo/specialization/unroll.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/algo/tune/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-12 08:44:51.000000 dprox-0.2.1/dprox/algo/tune/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2941 2023-08-06 06:03:25.000000 dprox-0.2.1/dprox/algo/tune/dpir.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/algo/tune/learnable.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/contrib/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-08-05 14:30:04.000000 dprox-0.2.1/dprox/contrib/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8716 2023-08-06 07:19:08.000000 dprox-0.2.1/dprox/contrib/csmri.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2563 2023-08-05 13:25:05.000000 dprox-0.2.1/dprox/contrib/derain.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      953 2023-08-06 01:49:45.000000 dprox-0.2.1/dprox/contrib/energy_system.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/contrib/optic/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       69 2023-08-05 14:37:30.000000 dprox-0.2.1/dprox/contrib/optic/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    17055 2023-08-06 07:35:24.000000 dprox-0.2.1/dprox/contrib/optic/doe_model.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3739 2023-08-06 01:05:50.000000 dprox-0.2.1/dprox/contrib/optic/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6059 2023-08-06 01:10:44.000000 dprox-0.2.1/dprox/contrib/optic/utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2497 2023-08-05 13:36:36.000000 dprox-0.2.1/dprox/contrib/restoration.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/linalg/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-22 11:53:09.000000 dprox-0.2.1/dprox/linalg/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3314 2023-07-23 02:25:37.000000 dprox-0.2.1/dprox/linalg/custom.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/linalg/solve/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      335 2023-06-02 14:40:15.000000 dprox-0.2.1/dprox/linalg/solve/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6513 2023-08-03 11:55:44.000000 dprox-0.2.1/dprox/linalg/solve/solver_cg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10190 2023-06-02 14:39:42.000000 dprox-0.2.1/dprox/linalg/solve/solver_minres.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5311 2023-06-12 08:09:04.000000 dprox-0.2.1/dprox/linalg/solve/solver_plss.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/linop/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      468 2023-08-06 15:30:52.000000 dprox-0.2.1/dprox/linop/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7715 2023-07-23 02:25:42.000000 dprox-0.2.1/dprox/linop/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2365 2023-05-24 07:38:28.000000 dprox-0.2.1/dprox/linop/blackbox.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15257 2023-07-01 02:35:05.000000 dprox-0.2.1/dprox/linop/comp_graph.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.2.1/dprox/linop/constaints.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2882 2023-05-24 07:43:37.000000 dprox-0.2.1/dprox/linop/constant.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5480 2023-05-24 07:43:49.000000 dprox-0.2.1/dprox/linop/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.2.1/dprox/linop/edge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/linop/grad.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1025 2023-08-06 15:31:07.000000 dprox-0.2.1/dprox/linop/mul.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      489 2023-05-24 06:31:56.000000 dprox-0.2.1/dprox/linop/placeholder.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2580 2023-05-24 07:43:58.000000 dprox-0.2.1/dprox/linop/scale.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3459 2023-05-24 07:38:58.000000 dprox-0.2.1/dprox/linop/subsample.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3051 2023-05-24 07:44:13.000000 dprox-0.2.1/dprox/linop/sum.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2988 2023-05-24 07:44:22.000000 dprox-0.2.1/dprox/linop/variable.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3717 2023-05-24 07:44:41.000000 dprox-0.2.1/dprox/linop/vstack.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      285 2023-05-22 11:53:09.000000 dprox-0.2.1/dprox/proxfn/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2700 2023-06-07 15:13:18.000000 dprox-0.2.1/dprox/proxfn/base.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/fast/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/fast/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-08-06 15:24:30.000000 dprox-0.2.1/dprox/proxfn/fast/cs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      604 2023-05-27 03:46:05.000000 dprox-0.2.1/dprox/proxfn/fast/csmri.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/fast/pr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/fast/spi.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.2.1/dprox/proxfn/fast/sr.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/nlm/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/nlm/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/nlm/nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/nlm/patch_nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/nonneg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/norm.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/pnp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/composite.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/network_unet.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/unet/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/unet/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.2.1/dprox/proxfn/pnp/denoisers/wrapper.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3098 2023-08-06 17:26:03.000000 dprox-0.2.1/dprox/proxfn/pnp/prior.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5751 2023-06-19 10:50:01.000000 dprox-0.2.1/dprox/proxfn/sum_square.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/proxfn/unrolling/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/unrolling/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/proxfn/unrolling/dgu.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      587 2023-07-04 04:49:45.000000 dprox-0.2.1/dprox/proxfn/unrolling/prior.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      278 2023-08-05 15:59:24.000000 dprox-0.2.1/dprox/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1504 2023-08-05 14:24:40.000000 dprox-0.2.1/dprox/utils/containar.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3217 2023-08-06 15:03:47.000000 dprox-0.2.1/dprox/utils/huggingface.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox/utils/init/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2.1/dprox/utils/init/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-05-24 04:36:39.000000 dprox-0.2.1/dprox/utils/init/mosaic.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      756 2023-05-24 04:36:39.000000 dprox-0.2.1/dprox/utils/init/sr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-08-06 05:29:49.000000 dprox-0.2.1/dprox/utils/io.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4618 2023-06-27 12:39:39.000000 dprox-0.2.1/dprox/utils/metrics.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7989 2023-08-05 16:12:43.000000 dprox-0.2.1/dprox/utils/misc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3978 2023-05-24 04:36:39.000000 dprox-0.2.1/dprox/utils/psf2otf.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4000 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      124 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-08-06 17:27:08.000000 dprox-0.2.1/dprox.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-08-06 17:27:08.000000 dprox-0.2.1/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      678 2023-08-06 17:26:46.000000 dprox-0.2.1/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 17:27:08.000000 dprox-0.2.1/tests/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2740 2023-08-06 01:53:38.000000 dprox-0.2.1/tests/test_algorithms.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2675 2023-08-06 01:54:49.000000 dprox-0.2.1/tests/test_linop.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.2.1/tests/test_linop_primitive.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      136 2023-08-06 01:55:22.000000 dprox-0.2.1/tests/test_primitive.py
```

### Comparing `dprox-0.2/README.md` & `dprox-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 
 <p align="center">
 Differentiable Proximal Algorithm Modeling for Large-Scale Optimization
 </p>
 
 <p align="center">
 <a href="https://light.princeton.edu/publication/delta_prox/">Paper</a> |
+<a href="https://deltaprox.readthedocs.io/en/latest/">Doc</a> |
 <a href="https://github.com/princeton-computational-imaging/Delta-Prox/tree/main/notebooks">Tutorials</a> |
 <a href="https://github.com/princeton-computational-imaging/Delta-Prox/tree/main/examples">Examples</a> |
+<a href="https://deltaprox.readthedocs.io/en/latest/">Documentation</a> |
 <a href="https://github.com/princeton-computational-imaging/Delta-Prox#citation">Citation</a> 
 </p>
 
 <p align="center">
     <a href="https://pypi.org/project/dprox/">
         <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/v/dprox">
     </a>
@@ -42,15 +44,15 @@
 
 We recommend installing $\nabla$-Prox in a virtual environment from PyPI.
 
 ```bash
 pip install dprox
 ```
 
-<!-- Please refer to the [Installation](https://deltaprox.readthedocs.io/started/install) guide for other options. -->
+Please refer to the [Installation](https://deltaprox.readthedocs.io/en/latest/started/install.html) guide for other options.
 
 ## Quickstart
 ![pipeline2](docs/source/_static/pipeline_dprox.gif)
 
 
 Consider a simple image deconvolution problem, where we want to find a clean image $x$ given the blurred observation $y$ that minimizes the following objective function:
 
@@ -79,15 +81,15 @@
 
 We can also specialize the solver via bi-level optimization.
 For example, we can specialize the solver into a reinforcement learning (RL) solver for automatic parameter tuning.
 
 ```python
 solver = compile(data_term + reg_term, method='admm')
 rl_solver = specialize(solver, method='rl')
-rl_solver = train(rl_solver, dataset)
+rl_solver = train(rl_solver, **training_kwargs)
 ```
 
 Alternatively, we can specialize the solver into an unrolled solver for end-to-end optics optimization.
 
 ```python
 x = Variable()
 y = Placeholder()
```

### Comparing `dprox-0.2/dprox/algo/admm.py` & `dprox-0.2.1/dprox/algo/admm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/base.py` & `dprox-0.2.1/dprox/algo/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/hqs.py` & `dprox-0.2.1/dprox/algo/hqs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/invert.py` & `dprox-0.2.1/dprox/algo/invert.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/lp/solvers.py` & `dprox-0.2.1/dprox/algo/lp/solvers.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/lp/utils.py` & `dprox-0.2.1/dprox/algo/lp/utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/opt/absorb.py` & `dprox-0.2.1/dprox/algo/opt/absorb.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/opt/equil.py` & `dprox-0.2.1/dprox/algo/opt/equil.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/opt/merge.py` & `dprox-0.2.1/dprox/algo/opt/merge.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/pc.py` & `dprox-0.2.1/dprox/algo/pc.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/pgd.py` & `dprox-0.2.1/dprox/algo/pgd.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/primitives.py` & `dprox-0.2.1/dprox/algo/primitives.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 SPECAILIZATIONS = {
     'deq': DEQSolver,
     'rl': AutoTuneSolver,
     'unroll': build_unrolled_solver,
 }
 
+
 def compile(
     prox_fns: List[ProxFn],
     method: str = 'admm',
     device: Union[str, torch.device] = 'cuda' if torch.cuda.is_available() else 'cpu',
     **kwargs
 ):
     """
@@ -105,14 +106,26 @@
 
 
 def visualize():
     pass
 
 
 def train(
+    solver=None,
+    **kwargs,
+):
+    if solver is None:
+        return _train(**kwargs)
+    if isinstance(solver, AutoTuneSolver):
+        return solver.train(**kwargs)
+    else:
+        raise ValueError(f'Training {solver} is not supported yet.')
+
+
+def _train(
     model,
     step_fn,
     dataset='BSD500',
     savedir='saved',
     epochs=10,
     bs=2,
     lr=1e-4,
```

### Comparing `dprox-0.2/dprox/algo/problem.py` & `dprox-0.2.1/dprox/algo/problem.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/specialization/deq/solver.py` & `dprox-0.2.1/dprox/algo/specialization/deq/solver.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/specialization/deq/training.py` & `dprox-0.2.1/dprox/algo/specialization/deq/training.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/specialization/deq/utils/jacobian.py` & `dprox-0.2.1/dprox/algo/specialization/deq/utils/jacobian.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/specialization/deq/utils/layer_utils.py` & `dprox-0.2.1/dprox/algo/specialization/deq/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/specialization/deq/utils/optimizations.py` & `dprox-0.2.1/dprox/algo/specialization/deq/utils/optimizations.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/specialization/deq/utils/radam.py` & `dprox-0.2.1/dprox/algo/specialization/deq/utils/radam.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/specialization/deq/utils/solvers.py` & `dprox-0.2.1/dprox/algo/specialization/deq/utils/solvers.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/specialization/rl/solver.py` & `dprox-0.2.1/dprox/algo/specialization/rl/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from torch.utils.data.dataset import Dataset
 from tqdm import tqdm
 
 from dprox.utils import to_torch_tensor
 
 default_config = dict(
     rmsize=480,
-    max_episode_step=6,
+    max_episode_step=30,
     train_steps=15000,
     warmup=20,
     save_freq=1000,
     validate_interval=50,
     episode_train_times=10,
     env_batch=48,
     loop_penalty=0.05,
@@ -111,15 +111,15 @@
         vars = [v[:, chs:chs + 1, :, :] for v in vars]
         variables = torch.cat(vars, dim=1)
         x0 = ob.x0[:, chs:chs + 1, :, :]
         return torch.cat([
             variables,
             x0,
             ob.T,
-        ], 1)
+        ], 1).real
 
     def get_eval_ob(self, ob):
         return self.get_policy_ob(ob)
 
     def _get_attribute(self, ob, key):
         if key == 'gt':
             return ob.gt
@@ -297,19 +297,19 @@
             dic = {'y0': x0, 'x0': x0, 'gt': gt, 'output': x0, 'input': x0}
             dic['params'] = params
             return dic
     return Dataset
 
 
 class AutoTuneSolver(nn.Module):
-    def __init__(self, solver, policy='resnet', action_pack=5, max_episode_step=6, custom_policy_ob_pack_fn=None):
+    def __init__(self, solver, policy='resnet', action_pack=5, ob_dim=9, max_episode_step=6, custom_policy_ob_pack_fn=None):
         super().__init__()
         self.solver = solver
         # TODO: compute ob_dim based on ckpt
-        self.policy = make_policy(solver, action_pack, ob_dim=9, type=policy)
+        self.policy = make_policy(solver, action_pack, ob_dim=ob_dim, type=policy)
         self.policy.eval()
         self.max_episode_step = max_episode_step
         self.custom_policy_ob_pack_fn = custom_policy_ob_pack_fn
 
     def solve(self, x0, aux_state=None, pbar=False, callback=None):
         x0 = x0.to(self.solver.device)
         state = self.solver.initialize(x0)
```

### Comparing `dprox-0.2/dprox/algo/specialization/unroll.py` & `dprox-0.2.1/dprox/algo/specialization/unroll.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/algo/tune/dpir.py` & `dprox-0.2.1/dprox/algo/tune/dpir.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/contrib/csmri.py` & `dprox-0.2.1/dprox/contrib/csmri.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/contrib/derain.py` & `dprox-0.2.1/dprox/contrib/derain.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/contrib/energy_system.py` & `dprox-0.2.1/dprox/contrib/energy_system.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/contrib/optic/doe_model.py` & `dprox-0.2.1/dprox/contrib/optic/doe_model.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/contrib/optic/unet.py` & `dprox-0.2.1/dprox/contrib/optic/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/contrib/optic/utils.py` & `dprox-0.2.1/dprox/contrib/optic/utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/contrib/restoration.py` & `dprox-0.2.1/dprox/contrib/restoration.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linalg/custom.py` & `dprox-0.2.1/dprox/linalg/custom.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linalg/solve/solver_cg.py` & `dprox-0.2.1/dprox/linalg/solve/solver_cg.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linalg/solve/solver_minres.py` & `dprox-0.2.1/dprox/linalg/solve/solver_minres.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linalg/solve/solver_plss.py` & `dprox-0.2.1/dprox/linalg/solve/solver_plss.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/base.py` & `dprox-0.2.1/dprox/linop/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/blackbox.py` & `dprox-0.2.1/dprox/linop/blackbox.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/comp_graph.py` & `dprox-0.2.1/dprox/linop/comp_graph.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/constant.py` & `dprox-0.2.1/dprox/linop/constant.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/conv.py` & `dprox-0.2.1/dprox/linop/conv.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/grad.py` & `dprox-0.2.1/dprox/linop/grad.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/scale.py` & `dprox-0.2.1/dprox/linop/scale.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/subsample.py` & `dprox-0.2.1/dprox/linop/subsample.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/sum.py` & `dprox-0.2.1/dprox/linop/sum.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/variable.py` & `dprox-0.2.1/dprox/linop/variable.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/linop/vstack.py` & `dprox-0.2.1/dprox/linop/vstack.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/base.py` & `dprox-0.2.1/dprox/proxfn/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/fast/cs.py` & `dprox-0.2.1/dprox/proxfn/fast/cs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/fast/csmri.py` & `dprox-0.2.1/dprox/proxfn/fast/csmri.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/fast/pr.py` & `dprox-0.2.1/dprox/proxfn/fast/pr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/fast/spi.py` & `dprox-0.2.1/dprox/proxfn/fast/spi.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/fast/sr.py` & `dprox-0.2.1/dprox/proxfn/fast/sr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/nlm/nlm.py` & `dprox-0.2.1/dprox/proxfn/nlm/nlm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/norm.py` & `dprox-0.2.1/dprox/proxfn/norm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/base.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/composite.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/composite.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/TV_denoising.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/TV_denoising.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/basicblock.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_dncnn.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/network_dncnn.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_unet.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/network_unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/unet.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/denoisers/wrapper.py` & `dprox-0.2.1/dprox/proxfn/pnp/denoisers/wrapper.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/pnp/prior.py` & `dprox-0.2.1/dprox/proxfn/pnp/prior.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 from .denoisers import (DRUNetDenoiser, FFDNetColorDenoiser, FFDNetDenoiser,
                         GRUNetDenoiser, IRCNNDenoiser, UNetDenoiser)
 from .denoisers.composite import Augment
 
 
 def get_denoiser(type):
     if type == 'ffdnet':
-        model_path = hf.load_path('pnp_denoiser/ffdnet_gray.pth', repo_type='models')
+        model_path = hf.load_path('pnp_denoisers/ffdnet_gray.pth', repo_type='models')
         return FFDNetDenoiser(model_path)
     if type == 'ffdnet_color':
-        model_path = hf.load_path('pnp_denoiser/ffdnet_color.pth', repo_type='models')
+        model_path = hf.load_path('pnp_denoisers/ffdnet_color.pth', repo_type='models')
         return FFDNetColorDenoiser(model_path)
     if type == 'drunet_color':
-        model_path = hf.load_path('pnp_denoiser/drunet_color.pth', repo_type='models')
+        model_path = hf.load_path('pnp_denoisers/drunet_color.pth', repo_type='models')
         return DRUNetDenoiser(3, model_path)
     if type == 'drunet':
-        model_path = hf.load_path('pnp_denoiser/drunet_gray.pth', repo_type='models')
+        model_path = hf.load_path('pnp_denoisers/drunet_gray.pth', repo_type='models')
         return DRUNetDenoiser(1, model_path)
     if type == 'ircnn':
-        model_path = hf.load_path('pnp_denoiser/ircnn_gray.pth', repo_type='models')
+        model_path = hf.load_path('pnp_denoisers/ircnn_gray.pth', repo_type='models')
         return IRCNNDenoiser(1, model_path)
     if type == 'grunet':
-        model_path = hf.load_path('pnp_denoiser/unet_qrnn3d.pth', repo_type='models')
+        model_path = hf.load_path('pnp_denoisers/unet_qrnn3d.pth', repo_type='models')
         return GRUNetDenoiser(model_path)
     if type == 'unet':
-        model_path = hf.load_path('pnp_denoiser/unet-nm.pt', repo_type='models')
+        model_path = hf.load_path('pnp_denoisers/unet-nm.pt', repo_type='models')
         return UNetDenoiser(model_path)
 
 
 def clone(x, nums, shared):
     return [x if shared else copy.deepcopy(x) for _ in range(nums)]
```

### Comparing `dprox-0.2/dprox/proxfn/sum_square.py` & `dprox-0.2.1/dprox/proxfn/sum_square.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/unrolling/dgu.py` & `dprox-0.2.1/dprox/proxfn/unrolling/dgu.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/proxfn/unrolling/prior.py` & `dprox-0.2.1/dprox/proxfn/unrolling/prior.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/utils/containar.py` & `dprox-0.2.1/dprox/utils/containar.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/utils/huggingface.py` & `dprox-0.2.1/dprox/utils/huggingface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import urllib.request
 import huggingface_hub
 
 from tqdm import tqdm
 
-CACHE_DIR = os.path.join(os.path.expanduser('~'), '.cache/dprox')
+CACHE_DIR = os.path.join(os.path.expanduser("~"), ".cache/dprox")
 
 
 class DownloadProgressBar(tqdm):
     # The DownloadProgressBar class is a subclass of the tqdm class in Python used to
     # display progress bars for downloading files.
     def update_to(self, b=1, bsize=1, tsize=None):
         if tsize is not None:
@@ -22,67 +22,72 @@
     displaying a progress bar.
 
     Args:
       url (str): The URL of the file to be downloaded
       output_path (str): output_path is a string representing the file path where the downloaded file
         will be saved. It should include the file name and extension
     """
-    with DownloadProgressBar(unit='B', unit_scale=True,
-                             miniters=1, desc=url.split('/')[-1]) as t:
+    with DownloadProgressBar(
+        unit="B", unit_scale=True, miniters=1, desc=url.split("/")[-1]
+    ) as t:
         urllib.request.urlretrieve(url, filename=output_path, reporthook=t.update_to)
 
 
-def load_path(base_path: str, repo_type='datasets', user_id='delta-prox') -> str:
+def load_path(base_path: str, repo_type="datasets", user_id="delta-prox") -> str:
     """
     check if a file exists in a specific directory and download it from a URL if it
     doesn't exist.
 
     Args:
       base_path (str): The base path is a string that represents the path to a file or directory that the
         function is trying to locate or download. It is used to construct the full path to the file or
         directory by appending it to the DPROX_DIR path
 
-    Return: 
+    Return:
       a string which is the path to the file specified by the input parameter `base_path`.
     """
     if os.path.exists(base_path):
         return base_path
 
     save_path = os.path.join(CACHE_DIR, base_path)
     if not os.path.exists(save_path):
-        base_url = 'https://huggingface.co'
-        if repo_type == 'datasets':
-            base_url += '/' + repo_type
-        repo_id = base_path.split('/')[0]
-        path = os.path.join(*(base_path.split('/')[1:]))
+        base_url = "https://huggingface.co"
+        if repo_type == "datasets":
+            base_url += "/" + repo_type
+        repo_id = base_path.split("/")[0]
+        path = os.path.join(*(base_path.split("/")[1:]))
         url = f"{base_url}/{user_id}/{repo_id}/resolve/main/{path}"
-        print(f'{base_path} not found')
-        print('Try to download from huggingface: ', url)
+        print(f"{base_path} not found")
+        print("Try to download from huggingface: ", url)
         os.makedirs(os.path.dirname(save_path), exist_ok=True)
+        if "\\" in url:  ## fix url for windows
+            url = url.replace("\\", "/")
         download_url(url, save_path)
-        print('Downloaded to ', save_path)
+        print("Downloaded to ", save_path)
     return save_path
 
 
-def load_image(path, user_id='delta-prox'):
+def load_image(path, user_id="delta-prox"):
     import imageio
     import numpy as np
+
     path = load_path(path, user_id=user_id)
     img = imageio.imread(path)
     return np.float32(img) / 255
 
 
-def load_checkpoint(path, user_id='delta-prox'):
+def load_checkpoint(path, user_id="delta-prox"):
     import torch
-    ckpt_path = load_path(path, repo_type='models', user_id=user_id)
+
+    ckpt_path = load_path(path, repo_type="models", user_id=user_id)
     return torch.load(ckpt_path)
 
 
-def download_dataset(path, user_id='delta-prox', local_dir=None, force_download=True):
+def download_dataset(path, user_id="delta-prox", local_dir=None, force_download=True):
     if local_dir is None:
         local_dir = os.path.join(CACHE_DIR, path)
     if os.path.exists(local_dir) and not force_download:
         return local_dir
-    huggingface_hub.snapshot_download(repo_id=f"{user_id}/{path}",
-                                      local_dir=local_dir,
-                                      repo_type="dataset")
+    huggingface_hub.snapshot_download(
+        repo_id=f"{user_id}/{path}", local_dir=local_dir, repo_type="dataset"
+    )
     return local_dir
```

### Comparing `dprox-0.2/dprox/utils/init/mosaic.py` & `dprox-0.2.1/dprox/utils/init/mosaic.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/utils/init/sr.py` & `dprox-0.2.1/dprox/utils/init/sr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/utils/io.py` & `dprox-0.2.1/dprox/utils/io.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/utils/metrics.py` & `dprox-0.2.1/dprox/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/utils/misc.py` & `dprox-0.2.1/dprox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox/utils/psf2otf.py` & `dprox-0.2.1/dprox/utils/psf2otf.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/dprox.egg-info/SOURCES.txt` & `dprox-0.2.1/dprox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 dprox/linop/blackbox.py
 dprox/linop/comp_graph.py
 dprox/linop/constaints.py
 dprox/linop/constant.py
 dprox/linop/conv.py
 dprox/linop/edge.py
 dprox/linop/grad.py
+dprox/linop/mul.py
 dprox/linop/placeholder.py
 dprox/linop/scale.py
 dprox/linop/subsample.py
 dprox/linop/sum.py
 dprox/linop/variable.py
 dprox/linop/vstack.py
 dprox/proxfn/__init__.py
```

### Comparing `dprox-0.2/setup.py` & `dprox-0.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,21 +7,22 @@
     'munch',
     'tfpnp',
     'cvxpy',
     'torchlights',
     'tensorboardX',
     'termcolor',
     'proximal',
-    'opencv-python'
+    'opencv-python',
+    'huggingface_hub',
 ]
 
 setup(
     name='dprox',
     description='A domain-specific language and compiler that transforms optimization problems into differentiable proximal solvers.',
     url='https://github.com/princeton-computational-imaging/Delta-Prox',
     author='Zeqiang Lai',
     author_email='laizeqiang@outlook.com',
     packages=find_packages(),
-    version='0.2',
+    version='0.2.1',
     include_package_data=True,
     install_requires=deps,
 )
```

### Comparing `dprox-0.2/tests/test_algorithms.py` & `dprox-0.2.1/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `dprox-0.2/tests/test_linop.py` & `dprox-0.2.1/tests/test_linop.py`

 * *Files identical despite different names*

