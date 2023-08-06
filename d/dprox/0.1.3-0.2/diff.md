# Comparing `tmp/dprox-0.1.3.tar.gz` & `tmp/dprox-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/hyper-pnp/submit/Delta-Prox/dist/.tmp-otob2k3v/dprox-0.1.3.tar", last modified: Fri May 26 06:26:21 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/hyper-pnp/submit/Delta-Prox/dist/.tmp-vstotite/dprox-0.2.tar", last modified: Sun Aug  6 07:52:09 2023, max compression
```

## Comparing `dprox-0.1.3.tar` & `dprox-0.2.tar`

### file list

```diff
@@ -1,170 +1,157 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-05-26 06:26:21.000000 dprox-0.1.3/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3141 2023-05-22 07:49:24.000000 dprox-0.1.3/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      126 2023-05-26 05:55:22.000000 dprox-0.1.3/dprox/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      276 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3676 2023-05-24 07:18:47.000000 dprox-0.1.3/dprox/algo/admm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7654 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/algo/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/hqs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      685 2023-05-24 07:17:40.000000 dprox-0.1.3/dprox/algo/invert.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/lp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/lp/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13337 2023-05-22 14:14:30.000000 dprox-0.1.3/dprox/algo/lp/solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6017 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/lp/utils.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/opt/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/opt/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.1.3/dprox/algo/opt/absorb.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/opt/equil.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2241 2023-05-22 07:49:41.000000 dprox-0.1.3/dprox/algo/opt/merge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/algo/pc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/pgd.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4625 2023-05-24 07:18:27.000000 dprox-0.1.3/dprox/algo/problem.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/special/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       72 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6866 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/special/deq_utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/jacobian.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/layer_utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/optimizations.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/radam.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/deq_utils/solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/special/unroll.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/algo/tune/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       23 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/tune/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12895 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/tune/autotune.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1850 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/tune/dpir.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/algo/tune/learnable.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/linalg/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-22 11:53:09.000000 dprox-0.1.3/dprox/linalg/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1785 2023-05-22 12:39:40.000000 dprox-0.1.3/dprox/linalg/custom.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/linalg/solve/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      410 2023-05-22 11:53:09.000000 dprox-0.1.3/dprox/linalg/solve/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6498 2023-05-22 14:14:30.000000 dprox-0.1.3/dprox/linalg/solve/cg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9704 2023-05-22 14:14:30.000000 dprox-0.1.3/dprox/linalg/solve/minres.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3448 2023-05-22 14:14:30.000000 dprox-0.1.3/dprox/linalg/solve/plss.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/linop/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-10 14:07:17.000000 dprox-0.1.3/dprox/linop/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7440 2023-05-20 03:13:06.000000 dprox-0.1.3/dprox/linop/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2365 2023-05-24 07:38:28.000000 dprox-0.1.3/dprox/linop/blackbox.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15084 2023-05-20 09:13:41.000000 dprox-0.1.3/dprox/linop/comp_graph.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.1.3/dprox/linop/constaints.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2882 2023-05-24 07:43:37.000000 dprox-0.1.3/dprox/linop/constant.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5480 2023-05-24 07:43:49.000000 dprox-0.1.3/dprox/linop/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.1.3/dprox/linop/edge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/linop/grad.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      489 2023-05-24 06:31:56.000000 dprox-0.1.3/dprox/linop/placeholder.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2580 2023-05-24 07:43:58.000000 dprox-0.1.3/dprox/linop/scale.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3459 2023-05-24 07:38:58.000000 dprox-0.1.3/dprox/linop/subsample.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3051 2023-05-24 07:44:13.000000 dprox-0.1.3/dprox/linop/sum.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2988 2023-05-24 07:44:22.000000 dprox-0.1.3/dprox/linop/variable.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3717 2023-05-24 07:44:41.000000 dprox-0.1.3/dprox/linop/vstack.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      285 2023-05-22 11:53:09.000000 dprox-0.1.3/dprox/proxfn/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2693 2023-05-20 01:26:10.000000 dprox-0.1.3/dprox/proxfn/base.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/fast/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/fast/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/fast/cs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      884 2023-05-20 03:23:29.000000 dprox-0.1.3/dprox/proxfn/fast/csmri.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/fast/pr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/fast/spi.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.1.3/dprox/proxfn/fast/sr.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/linalg/
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5069 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/bicgstab.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1134 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/broyden.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6501 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/gmres.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1631 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/linalg/solve/plss.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/nlm/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/nlm/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/nlm/nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/nlm/patch_nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/nonneg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/norm.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/composite.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_unet.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.1.3/dprox/proxfn/pnp/denoisers/wrapper.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2902 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/proxfn/pnp/prior.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5751 2023-05-24 07:40:18.000000 dprox-0.1.3/dprox/proxfn/sum_square.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/proxfn/unrolling/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/unrolling/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/unrolling/dgu.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      482 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/proxfn/unrolling/prior.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      173 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1504 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/containar.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-05-13 14:43:30.000000 dprox-0.1.3/dprox/utils/examples/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/csmri/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       82 2023-05-13 14:45:34.000000 dprox-0.1.3/dprox/utils/examples/csmri/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3011 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/csmri/common.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4146 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/csmri/dataset.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2083 2023-05-22 15:23:16.000000 dprox-0.1.3/dprox/utils/examples/csmri/misc.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/derain/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       40 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/derain/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2564 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/derain/custom_linop.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/energy_system/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      947 2023-05-20 03:14:24.000000 dprox-0.1.3/dprox/utils/examples/energy_system/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/examples/optic/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       46 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/optic/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9960 2023-05-26 05:40:51.000000 dprox-0.1.3/dprox/utils/examples/optic/common.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    18268 2023-05-26 05:40:51.000000 dprox-0.1.3/dprox/utils/examples/optic/doe_model.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3063 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/examples/optic/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2488 2023-05-14 13:57:57.000000 dprox-0.1.3/dprox/utils/examples/restoration.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox/utils/init/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.3/dprox/utils/init/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/init/mosaic.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      756 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/init/sr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5788 2023-05-26 05:40:51.000000 dprox-0.1.3/dprox/utils/io.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4630 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/metrics.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4958 2023-05-24 06:20:38.000000 dprox-0.1.3/dprox/utils/misc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3978 2023-05-24 04:36:39.000000 dprox-0.1.3/dprox/utils/psf2otf.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4287 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      108 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-05-26 06:26:21.000000 dprox-0.1.3/dprox.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-26 06:26:21.000000 dprox-0.1.3/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      656 2023-05-26 06:25:51.000000 dprox-0.1.3/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 06:26:21.000000 dprox-0.1.3/tests/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2715 2023-05-20 03:13:06.000000 dprox-0.1.3/tests/test_algorithms.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1043 2023-05-24 07:09:33.000000 dprox-0.1.3/tests/test_derain.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      318 2023-05-22 14:14:30.000000 dprox-0.1.3/tests/test_energy_system.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-05-23 08:23:24.000000 dprox-0.1.3/tests/test_inverse_problems.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      790 2023-05-24 07:49:26.000000 dprox-0.1.3/tests/test_jd23.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2586 2023-05-24 04:36:39.000000 dprox-0.1.3/tests/test_linear_solver.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3280 2023-05-22 11:53:09.000000 dprox-0.1.3/tests/test_linear_solver_grad.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6231 2023-05-24 08:13:09.000000 dprox-0.1.3/tests/test_linear_solver_torch.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2692 2023-05-20 03:13:06.000000 dprox-0.1.3/tests/test_linop.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.1.3/tests/test_linop_primitive.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1198 2023-05-24 04:36:39.000000 dprox-0.1.3/tests/test_ml_problems.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      302 2023-08-06 07:52:09.000000 dprox-0.2/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5423 2023-08-06 07:49:15.000000 dprox-0.2/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      217 2023-08-06 02:06:06.000000 dprox-0.2/dprox/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      375 2023-08-06 07:23:41.000000 dprox-0.2/dprox/algo/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3676 2023-06-17 08:34:57.000000 dprox-0.2/dprox/algo/admm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9623 2023-07-06 07:36:05.000000 dprox-0.2/dprox/algo/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.2/dprox/algo/hqs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      685 2023-05-24 07:17:40.000000 dprox-0.2/dprox/algo/invert.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/lp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.2/dprox/algo/lp/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16158 2023-08-06 02:42:27.000000 dprox-0.2/dprox/algo/lp/solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6540 2023-08-03 11:55:44.000000 dprox-0.2/dprox/algo/lp/utils.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/opt/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/opt/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.2/dprox/algo/opt/absorb.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/opt/equil.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2241 2023-05-22 07:49:41.000000 dprox-0.2/dprox/algo/opt/merge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.2/dprox/algo/pc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/pgd.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5636 2023-08-06 07:26:09.000000 dprox-0.2/dprox/algo/primitives.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3607 2023-08-06 07:22:38.000000 dprox-0.2/dprox/algo/problem.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/specialization/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      126 2023-08-06 07:26:19.000000 dprox-0.2/dprox/algo/specialization/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/specialization/deq/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-06-12 08:45:35.000000 dprox-0.2/dprox/algo/specialization/deq/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3620 2023-07-04 03:59:17.000000 dprox-0.2/dprox/algo/specialization/deq/solver.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3600 2023-06-12 08:46:04.000000 dprox-0.2/dprox/algo/specialization/deq/training.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/specialization/deq/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/jacobian.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/layer_utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/optimizations.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/radam.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/specialization/deq/utils/solvers.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/specialization/rl/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       21 2023-06-12 08:44:42.000000 dprox-0.2/dprox/algo/specialization/rl/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    14224 2023-06-19 14:51:52.000000 dprox-0.2/dprox/algo/specialization/rl/solver.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1875 2023-08-06 07:27:33.000000 dprox-0.2/dprox/algo/specialization/unroll.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/algo/tune/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-06-12 08:44:51.000000 dprox-0.2/dprox/algo/tune/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2941 2023-08-06 06:03:25.000000 dprox-0.2/dprox/algo/tune/dpir.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.2/dprox/algo/tune/learnable.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/contrib/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-08-05 14:30:04.000000 dprox-0.2/dprox/contrib/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8716 2023-08-06 07:19:08.000000 dprox-0.2/dprox/contrib/csmri.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2563 2023-08-05 13:25:05.000000 dprox-0.2/dprox/contrib/derain.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      953 2023-08-06 01:49:45.000000 dprox-0.2/dprox/contrib/energy_system.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/contrib/optic/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       69 2023-08-05 14:37:30.000000 dprox-0.2/dprox/contrib/optic/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    17055 2023-08-06 07:35:24.000000 dprox-0.2/dprox/contrib/optic/doe_model.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3739 2023-08-06 01:05:50.000000 dprox-0.2/dprox/contrib/optic/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6059 2023-08-06 01:10:44.000000 dprox-0.2/dprox/contrib/optic/utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2497 2023-08-05 13:36:36.000000 dprox-0.2/dprox/contrib/restoration.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/linalg/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-22 11:53:09.000000 dprox-0.2/dprox/linalg/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3314 2023-07-23 02:25:37.000000 dprox-0.2/dprox/linalg/custom.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/linalg/solve/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      335 2023-06-02 14:40:15.000000 dprox-0.2/dprox/linalg/solve/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6513 2023-08-03 11:55:44.000000 dprox-0.2/dprox/linalg/solve/solver_cg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10190 2023-06-02 14:39:42.000000 dprox-0.2/dprox/linalg/solve/solver_minres.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5311 2023-06-12 08:09:04.000000 dprox-0.2/dprox/linalg/solve/solver_plss.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/linop/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      658 2023-07-01 02:33:34.000000 dprox-0.2/dprox/linop/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7715 2023-07-23 02:25:42.000000 dprox-0.2/dprox/linop/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2365 2023-05-24 07:38:28.000000 dprox-0.2/dprox/linop/blackbox.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15257 2023-07-01 02:35:05.000000 dprox-0.2/dprox/linop/comp_graph.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.2/dprox/linop/constaints.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2882 2023-05-24 07:43:37.000000 dprox-0.2/dprox/linop/constant.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5480 2023-05-24 07:43:49.000000 dprox-0.2/dprox/linop/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.2/dprox/linop/edge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.2/dprox/linop/grad.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      489 2023-05-24 06:31:56.000000 dprox-0.2/dprox/linop/placeholder.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2580 2023-05-24 07:43:58.000000 dprox-0.2/dprox/linop/scale.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3459 2023-05-24 07:38:58.000000 dprox-0.2/dprox/linop/subsample.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3051 2023-05-24 07:44:13.000000 dprox-0.2/dprox/linop/sum.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2988 2023-05-24 07:44:22.000000 dprox-0.2/dprox/linop/variable.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3717 2023-05-24 07:44:41.000000 dprox-0.2/dprox/linop/vstack.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      285 2023-05-22 11:53:09.000000 dprox-0.2/dprox/proxfn/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2700 2023-06-07 15:13:18.000000 dprox-0.2/dprox/proxfn/base.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/fast/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/fast/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/fast/cs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      604 2023-05-27 03:46:05.000000 dprox-0.2/dprox/proxfn/fast/csmri.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/fast/pr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/fast/spi.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.2/dprox/proxfn/fast/sr.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/nlm/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/nlm/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/nlm/nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/nlm/patch_nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/nonneg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/norm.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/composite.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_unet.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.2/dprox/proxfn/pnp/denoisers/wrapper.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3091 2023-08-06 05:32:51.000000 dprox-0.2/dprox/proxfn/pnp/prior.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5751 2023-06-19 10:50:01.000000 dprox-0.2/dprox/proxfn/sum_square.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/proxfn/unrolling/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/unrolling/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.2/dprox/proxfn/unrolling/dgu.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      587 2023-07-04 04:49:45.000000 dprox-0.2/dprox/proxfn/unrolling/prior.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      278 2023-08-05 15:59:24.000000 dprox-0.2/dprox/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1504 2023-08-05 14:24:40.000000 dprox-0.2/dprox/utils/containar.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3204 2023-08-06 05:52:06.000000 dprox-0.2/dprox/utils/huggingface.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox/utils/init/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.2/dprox/utils/init/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-05-24 04:36:39.000000 dprox-0.2/dprox/utils/init/mosaic.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      756 2023-05-24 04:36:39.000000 dprox-0.2/dprox/utils/init/sr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-08-06 05:29:49.000000 dprox-0.2/dprox/utils/io.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4618 2023-06-27 12:39:39.000000 dprox-0.2/dprox/utils/metrics.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7989 2023-08-05 16:12:43.000000 dprox-0.2/dprox/utils/misc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3978 2023-05-24 04:36:39.000000 dprox-0.2/dprox/utils/psf2otf.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      302 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3981 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      108 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-08-06 07:52:09.000000 dprox-0.2/dprox.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-08-06 07:52:09.000000 dprox-0.2/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      652 2023-08-06 07:39:29.000000 dprox-0.2/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-08-06 07:52:09.000000 dprox-0.2/tests/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2740 2023-08-06 01:53:38.000000 dprox-0.2/tests/test_algorithms.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2675 2023-08-06 01:54:49.000000 dprox-0.2/tests/test_linop.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.2/tests/test_linop_primitive.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      136 2023-08-06 01:55:22.000000 dprox-0.2/tests/test_primitive.py
```

### Comparing `dprox-0.1.3/dprox/algo/admm.py` & `dprox-0.2/dprox/algo/admm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/base.py` & `dprox-0.2/dprox/algo/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import abc
 import torch
 import torch.nn as nn
 import numpy as np
-from typing import List
+from typing import List, Callable, Union, Iterable
 from tqdm import tqdm
 
 from dprox.proxfn import ProxFn
 from dprox.linop import CompGraph, vstack
 from dprox.utils import to_torch_tensor
 
 
 def expand(r):
     if len(r.shape) == 1:
         r = r.view(r.shape[0], 1, 1, 1)
     return r
 
 
-def auto_convert_to_tensor(names, batchify):
-    """
-    A decorator that automatically converts specified arguments to PyTorch tensors.
-    
-    :param names: A list of strings representing the names of the arguments that should be converted to tensors
-    :param batchify: A list of names of arguments that should be batched together when converting to a tensor
-    :return: a decorator function `outter_wrapper`.
+def auto_convert_to_tensor(names: List[str], batchify: bool):
+    """ A decorator that automatically converts specified arguments to PyTorch tensors.
     """
     def outter_wrapper(fn):
         def wrapper(*args, **kwargs):
             for k, v in kwargs.items():
                 if k in names:
                     if v is not None:
                         kwargs[k] = to_tensor(v, batch=k in batchify)
@@ -52,18 +47,19 @@
     return to_torch_tensor(x, batch)
 
 
 def isscalar(x):
     return np.isscalar(x) or (isinstance(x, torch.Tensor) and len(x.shape) == 0)
 
 
-# The Algorithm class is an abstract class that defines methods and properties for solving
-# optimization problems using proximal algorithms.
 class Algorithm(nn.Module):
-    # class method
+    """
+    The Algorithm class is an abstract class that defines methods and properties for solving
+    optimization problems using proximal algorithms.
+    """
 
     @abc.abstractclassmethod
     def partition(cls, prox_fns: List[ProxFn]):
         return NotImplementedError
 
     @classmethod
     def create(cls, *args, **kwargs):
@@ -79,46 +75,87 @@
         self.Kall = CompGraph(vstack([fn.linop for fn in psi_fns + omega_fns]))
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     @auto_convert_to_tensor(['x0', 'rhos', 'lams'], batchify=['x0'])
-    def solve(self, x0=None, rhos=None, lams=None, max_iter=24, pbar=False):
+    def solve(
+        self,
+        x0: Union[torch.Tensor, np.ndarray] = None,
+        rhos: Union[float, Iterable[float]] = None,
+        lams: Union[float, Iterable[float], dict] = None,
+        max_iter: int = 24,
+        pbar: bool = False,
+        callback: Callable = None
+    ) -> torch.Tensor:
         """
-        This function solves a problem using an iterative algorithm with given parameters and returns
+        Solve a problem using an iterative algorithm with given parameters and return
         the solution.
-        
-        :param x0: initial guess for the solution
-        :param rhos: A list of penalty parameters for each constraint in the optimization problem
-        :param lams: lams is a list of regularization parameters used in the optimization algorithm.
-        These parameters control the trade-off between fitting the data and keeping the model simple. A
-        higher value of lambda will result in a simpler model with less overfitting, while a lower value
-        of lambda will result in a more complex model
-        :param max_iter: The maximum number of iterations to run the optimization algorithm for,
-        defaults to 24 (optional)
-        :param pbar: A boolean flag indicating whether or not to display a progress bar during the
-        optimization process, defaults to False (optional)
-        :return: the first element of the state tuple, which is the solution to the optimization
-        problem.
+
+        Args:
+          x0: initial guess for the solution
+          rhos: A list of penalty parameters for each constraint in the optimization problem
+          lams: lams is a list of regularization parameters used in the optimization algorithm.
+            These parameters control the trade-off between fitting the data and keeping the model simple. A
+            higher value of lambda will result in a simpler model with less overfitting, while a lower value
+            of lambda will result in a more complex model
+          max_iter: The maximum number of iterations to run the optimization algorithm for,
+            defaults to 24 (optional)
+          pbar: A boolean flag indicating whether or not to display a progress bar during the
+            optimization process, defaults to False (optional)
+
+        Return:
+          the first element of the state tuple, which is the solution to the optimization problem.
         """
+
         x0, rhos, lams, max_iter = self.defaults(x0, rhos, lams, max_iter)
         x0, rhos, lams = move(x0, rhos, lams, device=self.device)
 
         state = self.initialize(x0)
-        state = self.iters(state, rhos, lams, max_iter, pbar)
+        state = self.iters(state, rhos, lams, max_iter, pbar, callback=callback)
 
         return state[0]
 
-    def iters(self, state, rhos, lams, max_iter, pbar=False):
+    def iters(
+        self,
+        state,
+        rhos,
+        lams,
+        max_iter,
+        pbar=False,
+        callback=None
+    ):
+        """
+        Iterate over a given number of iterations and update the state using the given
+        rhos and lams.
+
+        Args:
+          state: The current state of the optimization algorithm
+          rhos: A numpy array of shape (..., max_iter) containing the values of the penalty
+            parameter rho for each iteration
+          lams: A dictionary containing the Lagrange multipliers for each constraint in the
+            optimization problem. The keys of the dictionary are the names of the constraints and the values
+            are arrays containing the Lagrange multipliers for each iteration of the optimization algorithm
+          max_iter: The maximum number of iterations to run the algorithm for
+          pbar: A boolean flag indicating whether to display a progress bar during the iterations.
+            If set to True, a progress bar will be displayed to show the progress of the iterations. If set
+            to False, no progress bar will be displayed, defaults to False (optional)
+
+        Return:
+          the final state after iterating over the given number of iterations using the `iter` 
+          function with the given `rho` and `lam` values.
+        """
         for iter in tqdm(range(max_iter), disable=not pbar):
             rho = rhos[..., iter]
             lam = {k: v[..., iter] for k, v in lams.items()}
             self._notify_all_op_current_step(iter)
             state = self.iter(state, rho, lam)
+            if callback is not None:
+                callback(iter=iter, state=state, rho=rho, lam=lam)
         return state
 
     def _notify_all_op_current_step(self, step):
         for fn in self.psi_fns:
             fn.step = step
         for fn in self.omega_fns:
             fn.step = step
@@ -141,16 +178,16 @@
 
     @abc.abstractmethod
     def _iter(self, state, rho, lam):
         return NotImplementedError
 
     def _notify_all_op_current_step(self, step):
         """
-        This function sets the step attribute for various functions and their associated linear operators.
-        
+        set the step attribute for various functions and their associated linear operators.
+
         :param step: an integer representing the current step in a process or algorithm
         """
         for fn in self.psi_fns:
             fn.step = step
         for fn in self.omega_fns:
             fn.step = step
 
@@ -176,14 +213,24 @@
         return x0, rhos, lams, max_iter
 
     # ---------------------------------------------------------------------------- #
     #                  Helper functions for reinforcement learning                 #
     # ---------------------------------------------------------------------------- #
 
     def pack(self, state):
+        """
+        take a list of tensors and concatenates them along the second dimension.
+
+        :param state: a list of tensors or lists of tensors that need to be
+        concatenated along the second dimension. The function first flattens the list of tensors or
+        lists of tensors into a single list, and then concatenates them along the second dimension using
+        PyTorch's "torch.cat"
+        :return: a tensor that is the concatenation of all the tensors in the input state, after
+        flattening any nested lists. The concatenation is done along the second dimension (dim=1).
+        """
         flatten = []
         for s in state:
             if isinstance(s, list): flatten += s
             else: flatten += [s]
         return torch.cat(flatten, dim=1)
 
     #TODO: refactor
```

### Comparing `dprox-0.1.3/dprox/algo/hqs.py` & `dprox-0.2/dprox/algo/hqs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/invert.py` & `dprox-0.2/dprox/algo/invert.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/lp/solvers.py` & `dprox-0.2/dprox/algo/lp/solvers.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from functools import partial
 
 import scipy
 import torch
 import torch.nn as nn
 from tqdm import tqdm
 
-from dprox.linalg.solve import PCG
+from dprox.linalg.custom import pcg
 from .utils import *
 
 
 class LPConvergenceLoss(nn.Module):
     def __init__(self) -> None:
         super().__init__()
-        
+
     def forward(self, r_norm, s_norm, eps_primal, eps_dual):
-        primal_loss = (r_norm / eps_primal) 
+        primal_loss = (r_norm / eps_primal)
         dual_loss = (s_norm / eps_dual)
         # balancing_loss = torch.abs(primal_loss - dual_loss)
         # loss = primal_loss + dual_loss + balancing_loss
         loss = torch.log(primal_loss) + torch.log(dual_loss)
         return loss
 
 
@@ -29,61 +29,71 @@
         self.A_ub = A_ub
         self.b_ub = b_ub
         self.A_eq = A_eq
         self.b_eq = b_eq
         n = c.shape[0]
         self.device = device
         if x_lb is None:
-            x_lb = torch.zeros(n, 1, dtype=dtype, device=device)
+            # x_lb = torch.zeros(n, 1, dtype=dtype, device=device)
+            x_lb = np.zeros((n, 1))
         if x_ub is None:
-            x_ub = float('inf') * torch.ones(n, 1, dtype=dtype, device=device)
+            # x_ub = float('inf') * torch.ones(n, 1, dtype=dtype, device=device)
+            x_ub = float('inf') * np.ones((n, 1))
         self.x_lb = x_lb
         self.x_ub = x_ub
+        self.original_problem = self.c, self.A_ub, self.b_ub, self.A_eq, self.b_eq, self.x_lb, self.x_ub
         self._preprocess(norm_ord, sparse)
-    
+
+    def unpack(self):
+        return self.original_problem
+
     @torch.no_grad()
     def _preprocess(self, norm_ord, sparse):
-        c, A_ub, b_ub, A_eq, b_eq, x_lb, x_ub = self.c, self.A_ub, self.b_ub, self.A_eq, self.b_eq, self.x_lb, self.x_ub
+        c, A_ub, b_ub, A_eq, b_eq, x_lb, x_ub = self.original_problem
         device = self.device
         m_ub = A_ub.shape[0]
         m_eq = A_eq.shape[0]
         n = c.shape[0]
         if not sparse:
-            A = torch.vstack([A_ub, A_eq, torch.eye(n, device=device)])            
-            self.d, self.e, self.gamma_c, self.gamma_b, self.A = Ruiz_equilibration_th(A, c, b, ord=norm_ord, max_iters=100)
+            A = torch.vstack([A_ub, A_eq, torch.eye(n, device=device)])
+            self.d, self.e, self.gamma_c, self.gamma_b, self.A = Ruiz_equilibration_th(A, c, b=torch.concatenate([b_ub, b_eq, x_ub]), ord=norm_ord, max_iters=100)
             self.AT = self.A.T
             self.Acnorm = torch.linalg.norm(A, axis=0)
-        else: #NOTE use numpy instead as many functions are not supported in torch.sparse
+        else:  # NOTE use numpy instead as many functions are not supported in torch.sparse
             A = scipy.sparse.vstack([A_ub, A_eq, scipy.sparse.eye(n)])
             m, _ = A.shape
-            d, e, gamma_c, gamma_b, A = Ruiz_equilibration_sparse_np(A, c, b=np.concatenate([b_ub, b_eq]), ord=float('inf'), max_iters=20, verbose=True)
+            d, e, gamma_c, gamma_b, A = Ruiz_equilibration_sparse_np(A, c, b=np.concatenate([b_ub, b_eq, x_ub[:, 0]]), ord=float('inf'), max_iters=20, verbose=True)
             Acnorm = slinalg.norm(A, axis=0)
             self.A, self.AT = scipy_sparse_to_torchop(A, device=device)
-            self.A_eq =scipy_sparse_to_torchop(A_eq, device=device, output_AT=False)
-            self.A_ub =scipy_sparse_to_torchop(A_ub, device=device, output_AT=False)
+            self.A_eq = scipy_sparse_to_torchop(A_eq, device=device, output_AT=False)
+            self.A_ub = scipy_sparse_to_torchop(A_ub, device=device, output_AT=False)
             self.c = c = torch.from_numpy(c).to(device).view(n, 1)
             self.b_eq = b_eq = torch.from_numpy(b_eq).to(device).view(m_eq, 1)
             self.b_ub = b_ub = torch.from_numpy(b_ub).to(device).view(m_ub, 1)
             self.d = torch.from_numpy(d).to(device).view(1, n)
             self.e = torch.from_numpy(e).to(device).view(m, 1)
             self.Acnorm = torch.from_numpy(Acnorm).to(device)
             self.gamma_b = gamma_b
             self.gamma_c = gamma_c
 
+        if isinstance(x_lb, np.ndarray):
+            self.x_lb = x_lb = torch.from_numpy(x_lb).to(device).view(n, 1)
+        if isinstance(x_ub, np.ndarray):
+            self.x_ub = x_ub = torch.from_numpy(x_ub).to(device).view(n, 1)
+
         lb = torch.vstack([-float('inf') * torch.ones(m_ub, 1, device=device), b_eq, x_lb])
-        b = torch.vstack([b_ub, b_eq])
-        ub = torch.vstack([b, x_ub])
+        ub = torch.vstack([b_ub, b_eq, x_ub])
         self.lb, self.ub = lb, ub
 
     def get_data(self):
         return self.d.detach().clone(), self.e.detach().clone(),\
             self.gamma_c, self.gamma_b, \
             self.A, self.AT, self.Acnorm, \
             self.ub.detach().clone(), self.lb.detach().clone(), self.c.detach().clone()
-    
+
     @property
     def problem_scale(self):
         return self.A.shape
 
 
 class LPSolverADMM(nn.Module):
     def __init__(self, rho=1, problem_scale=None, abstol=1e-4, reltol=1e-3, norm_ord=float('inf'), max_iters=5000, dtype=torch.float64, verbose=True) -> None:
@@ -92,201 +102,252 @@
         self.abstol = abstol
         self.reltol = reltol
         self.norm_ord = norm_ord
         self.max_iters = max_iters
         self.dtype = dtype
         self.verbose = verbose
         self._init_params(rho=rho)
-    
+
     def _init_params(self, rho):
         self.rho = nn.Parameter(torch.tensor(rho, dtype=self.dtype))
         # self.rho_log = nn.Parameter(torch.tensor(np.log(rho), dtype=self.dtype))
-        
+
         # self.sigma = nn.Parameter(torch.tensor(1e-6, dtype=self.dtype))
         self.sigma_log = nn.Parameter(torch.tensor(np.log(1e-6), dtype=self.dtype))
         self.alpha = nn.Parameter(torch.tensor(1.6, dtype=self.dtype))
-        
+
         self.gamma_c_mul = nn.Parameter(torch.tensor(1., dtype=self.dtype))
         self.gamma_b_mul = nn.Parameter(torch.tensor(1., dtype=self.dtype))
-        
+
         # self.gamma_c_mul_log = nn.Parameter(torch.tensor(0., dtype=self.dtype))
         # self.gamma_b_mul_log = nn.Parameter(torch.tensor(0., dtype=self.dtype))
 
         # self.register_buffer('sigma', torch.tensor(1e-6, dtype=self.dtype))
         # self.register_buffer('alpha', torch.tensor(1.6, dtype=self.dtype))
-        
+
         if self.problem_scale is not None:
             m, n = self.problem_scale
             self.d_mul_log = nn.Parameter(torch.zeros(1, n, dtype=self.dtype))
             self.e_mul_log = nn.Parameter(torch.zeros(m, 1, dtype=self.dtype))
 
-
-    def solve(self, lpproblem, rho=None, sigma=None, alpha=None, max_iters=None, eval_freq=25, residual_balance=False):
+    def solve(self, lpproblem, rho=None, sigma=None, alpha=None, max_iters=None, eval_freq=25, residual_balance=False, direct=False, polish=False):
         if max_iters is None: max_iters = self.max_iters
         vector_norm = partial(torch.linalg.vector_norm, ord=self.norm_ord)
         d, e, gamma_c, gamma_b, A, AT, Acnorm, ub, lb, c = lpproblem.get_data()
-        
-        if self.problem_scale is not None:  #NOTE do not use as it doesn't work well 
-            d_mul = torch.exp(self.d_mul_log)
-            e_mul = torch.exp(self.e_mul_log)
-            d = d * d_mul
-            e = e * e_mul
-            A = A * e_mul * d_mul
+        m, n = A.shape
+        m_ub = lpproblem.A_ub.shape[0]
 
-        # gamma_c = torch.exp(self.gamma_c_mul_log) * gamma_c
-        # gamma_b = torch.exp(self.gamma_b_mul_log) * gamma_b
-        
-        gamma_c = self.gamma_c_mul * gamma_c
-        gamma_b = self.gamma_b_mul * gamma_b
-        
         device = c.device
         dtype = self.dtype
 
         rho = rho if rho is not None else self.rho
         # rho = rho if rho is not None else torch.exp(self.rho_log)
         sigma = sigma if sigma is not None else torch.exp(self.sigma_log)
         # sigma = sigma if sigma is not None else self.sigma
         alpha = alpha if alpha is not None else self.alpha
 
-        # alpha = torch.clamp(alpha, min=0, max=2)
-        
-        m, n = A.shape
-        m_ub = lpproblem.A_ub.shape[0]
+        if self.problem_scale is not None:  # NOTE do not use as it doesn't work well
+            d_mul = torch.exp(self.d_mul_log)
+            e_mul = torch.exp(self.e_mul_log)
+            d = d * d_mul
+            e = e * e_mul
+            A = A * e_mul * d_mul
+
+        # gamma_c = torch.exp(self.gamma_c_mul_log) * gamma_c
+        # gamma_b = torch.exp(self.gamma_b_mul_log) * gamma_b
+
+        gamma_c = self.gamma_c_mul * gamma_c
+        gamma_b = self.gamma_b_mul * gamma_b
         d = d.view(n, 1)
         e = e.view(m, 1)
-        
         c = gamma_c * (d * c)
-        # lb = e * lb * gamma_b
-        # ub = e * ub * gamma_b
-        # lb = e * lb
-        # ub = e * ub
-        lb[m_ub:] *= gamma_b * e[m_ub:]
-        ub[:-n] *= gamma_b * e[:-n]
-        
+
+        mask_lb = ~torch.isinf(lb)
+        mask_ub = ~torch.isinf(ub)
+        lb[mask_lb] *= gamma_b * e[mask_lb]
+        ub[mask_ub] *= gamma_b * e[mask_ub]
+
+        # rho_base = torch.ones(m, 1, dtype=dtype, device=device)
+        # mask_rho = (lb == ub)
+        # rho_base[mask_rho] *= 1e3
+        # rho = rho_base * rho
+
         x = torch.zeros(n, 1, dtype=dtype, device=device)
         z = torch.zeros(m, 1, dtype=dtype, device=device)
         y = torch.zeros(m, 1, dtype=dtype, device=device)
         xtilde = torch.zeros_like(x)
-    
+
         rtols = torch.logspace(-6, -10, 10000)
-        history = defaultdict(lambda : [])
+        history = defaultdict(lambda: [])
+
+        Kinv = None
+        if direct:
+            K = (AT @ A) * rho + sigma * torch.eye(n, device=device, dtype=dtype)
+            Kinv = torch.inverse(K)
 
-        # K = (AT @ A).to_dense() * rho + sigma * torch.eye(n, device=device, dtype=dtype)
-        # L = torch.linalg.cholesky(K)  # K = L @ LT
-        L = None
-        
         ATAfun = LPATA_Func(A, AT, rho, sigma)
         ATAop = LinearOp(A_fun=ATAfun, AT_fun=ATAfun, shape=(n, n))
-        
-        M_constant = sigma * torch.ones(n, dtype=dtype, device=device)
-        M = (M_constant + rho * (Acnorm ** 2)).unsqueeze(1)
-        Minv = lambda x: x / M
-        
+
+        M_constant = sigma * torch.ones((n, 1), dtype=dtype, device=device)
+        M = (M_constant + rho * (Acnorm.unsqueeze(1) ** 2))
+        def Minv(x): return x / M
+
         for k in tqdm(range(max_iters)):
             rtol = 1e-10 if k >= 10000 else rtols[k]
             variables = x, z, y, xtilde
-            x, z, y, xtilde = self._solve_one_iter_precond(variables, c, A, AT, ATAop, Minv, lb, ub, rtol, rho, sigma, alpha, L=L)
-                
+            x, z, y, xtilde = self._solve_one_iter_precond(variables, c, A, AT, ATAop, Minv, lb, ub, rtol, rho, sigma, alpha, Kinv=Kinv)
+
             if k % eval_freq == 0:
-                objval, r_norm, s_norm, eps_primal, eps_dual = self.eval_result(c, A, AT, d, e, gamma_c, gamma_b, x, z, y)                                
+                objval, r_norm, s_norm, eps_primal, eps_dual = self.eval_result(c, A, AT, d, e, gamma_c, gamma_b, x, z, y)
 
                 # update rho (residual balance)
                 if residual_balance and k % 1000 == 0 and k != 0:
                     if r_norm > 10 * eps_primal or eps_dual > 10 * s_norm:
                         rho = rho * 2
                         flag = True
                     elif s_norm > 10 * eps_dual or eps_primal > 10 * r_norm:
                         rho = rho / 2
                         flag = True
                     else:
                         flag = False
                     if flag:
-                        M = (M_constant + rho * (Acnorm ** 2)).unsqueeze(1)
-                        Minv = lambda x: x / M
-                        ATAfun = LPATA_Func(A, AT, rho, sigma)
-                        ATAop = LinearOp(A_fun=ATAfun, AT_fun=ATAfun, shape=(n, n))
-                    
+                        if direct:
+                            K = (AT @ A) * rho + sigma * torch.eye(n, device=device, dtype=dtype)
+                            Kinv = torch.inverse(K)
+                        else:
+                            M = (M_constant + rho * (Acnorm.unsqueeze(1) ** 2))
+                            def Minv(x): return x / M
+                            ATAfun = LPATA_Func(A, AT, rho, sigma)
+                            ATAop = LinearOp(A_fun=ATAfun, AT_fun=ATAfun, shape=(n, n))
+
                 # if residual_balance and k >= 10000 and k % 500 == 0:
                 #     if (r_norm / eps_primal) > (1 / self.reltol / 1e2) * (s_norm / eps_dual):
                 #         rho = rho * 2
                 #         flag = True
                 #     elif (s_norm / eps_dual) > (1 / self.reltol / 1e2) * (r_norm / eps_primal):
                 #         rho = rho / 2
                 #         flag = True
                 #     else:
                 #         flag = False
-                    
+
                 #     if flag:
                 #         M = (M_constant + rho * (Acnorm ** 2)).unsqueeze(1)
                 #         Minv = lambda x: x / M
                 #         ATAfun = LPATA_Func(A, AT, rho, sigma)
                 #         ATAop = LinearOp(A_fun=ATAfun, AT_fun=ATAfun, shape=(n, n))
-                
+
                 history['r_norm'].append(r_norm.item())
                 history['s_norm'].append(s_norm.item())
                 history['eps_primal'].append(eps_primal.item())
                 history['eps_dual'].append(eps_dual.item())
                 history['objval'].append(objval.item())
-                
+
                 if not self.training and r_norm < eps_primal and s_norm < eps_dual:
+                    if self.verbose:
+                        print(f'Obj: {objval.item():.2e}, res_primal: {r_norm.item():.2e}, res_dual: {s_norm.item():.2e}, eps_primal: {eps_primal.item():.2e}, eps_dual: {eps_dual.item():.2e}, rho: {float(rho):.2e}')
                     break
 
                 if not self.training and self.verbose:
                     if k % 1000 == 0:
-                        print(objval.item(), r_norm.item(), s_norm.item(), eps_primal.item(), eps_dual.item(), float(rho))
-                    
+                        print(f'Obj: {objval.item():.2e}, res_primal: {r_norm.item():.2e}, res_dual: {s_norm.item():.2e}, eps_primal: {eps_primal.item():.2e}, eps_dual: {eps_dual.item():.2e}, rho: {float(rho):.2e}')
+
+        if polish:
+            x, z, y = self.solution_polishing(c, A, x, z, y)
+        dz = z - torch.clip(z, min=lb, max=ub)
+        res_z = vector_norm(dz)
         objval, r_norm, s_norm, eps_primal, eps_dual = self.eval_result(c, A, AT, d, e, gamma_c, gamma_b, x, z, y)
-        
-        print(objval.item(), r_norm.item(), s_norm.item(), eps_primal.item(), eps_dual.item(), float(rho))
+
+        print(f'Obj: {objval.item():.2e}, res_z: {res_z.item():.2e}, res_primal: {r_norm.item():.2e}, res_dual: {s_norm.item():.2e}, eps_primal: {eps_primal.item():.2e}, eps_dual: {eps_dual.item():.2e}, rho: {float(rho):.2e}')
+
         results = objval, r_norm, s_norm, eps_primal, eps_dual
         return x * d / gamma_b, history, results
-        
-    def _solve_one_iter_precond(self, variables, c, A, AT, ATAop, Minv, lb, ub, rtol, rho, sigma, alpha, L=None):
+
+    def solution_polishing(self, c, A, x, z, y):
+        n = x.shape[0]
+        device = c.device
+        Il = (y < 0)[:, 0]
+        Iu = (y > 0)[:, 0]
+        zl = z[Il, 0]
+        zu = z[Iu, 0]
+        Al = A[Il, :]
+        Au = A[Iu, :]
+        delta = 1e-6
+
+        # solution polishing matrix Kp
+        Kp = torch.vstack([
+            torch.hstack([delta * torch.eye(n, device=device), Al.T, Au.T]),
+            torch.hstack([Al, -delta * torch.eye(Al.shape[0], device=device), torch.zeros((Al.shape[0], Au.shape[0]), device=device)]),
+            torch.hstack([Au, torch.zeros((Au.shape[0], Al.shape[0]), device=device), -delta * torch.eye(Au.shape[0], device=device)])
+        ])
+
+        Kp_gt = torch.vstack([
+            torch.hstack([torch.zeros((n, n), device=device), Al.T, Au.T]),
+            torch.hstack([Al, torch.zeros((Al.shape[0], Al.shape[0]), device=device), torch.zeros((Al.shape[0], Au.shape[0]), device=device)]),
+            torch.hstack([Au, torch.zeros((Au.shape[0], Al.shape[0]), device=device), torch.zeros((Au.shape[0], Au.shape[0]), device=device)])
+        ])
+
+        rhs = torch.concatenate([-c[:, 0], zl, zu]).unsqueeze_(1)
+        Kpinv = torch.inverse(Kp)
+        t_hat = Kpinv @ rhs
+
+        for _ in range(2):
+            dt = Kpinv @ (rhs - Kp_gt @ t_hat)
+            t_hat = t_hat + dt
+
+        x, yl, yu = torch.split(t_hat, [x.shape[0], zl.shape[0], zu.shape[0]])
+        z = A @ x
+        y[Il, :] = yl
+        y[Iu, :] = yu
+        return x, z, y
+
+    def _solve_one_iter_precond(self, variables, c, A, AT, ATAop, Minv, lb, ub, rtol, rho, sigma, alpha, Kinv=None):
         x, z, y, xtilde = variables
 
         # x-update
         right = sigma * x - c + AT @ (rho * z - y)
-        if L is not None:  # seems very slow, why?
-            tmp = torch.linalg.solve_triangular(L, right, upper=False)
-            xtilde = torch.linalg.solve_triangular(L.T, tmp, upper=True)
+        if Kinv is not None:
+            xtilde = Kinv @ right
         else:
-            xtilde = PCG(ATAop, right, Minv, x0=xtilde.detach(), rtol=rtol, max_iters=200, verbose=False)
+            # verbose = True if rtol < 1e-10 else False
+            xtilde = pcg(ATAop, right, Minv=Minv, x0=xtilde.detach(), rtol=rtol, max_iters=int(1e3), verbose=False)
         ztilde = A @ (xtilde)
         x = alpha * xtilde + (1 - alpha) * x
 
         # z-update with relaxation
-        z_hat = alpha * ztilde + (1 - alpha) * z
-        z = torch.clip(z_hat + 1 / rho * y, min=lb, max=ub)
-        
+        ztilde = alpha * ztilde + (1 - alpha) * z
+        z = torch.clip(ztilde + 1 / rho * y, min=lb, max=ub)
+
         # dual update
-        y = y + rho * (z_hat - z)
-        
+        y = y + rho * (ztilde - z)
+
         return x, z, y, xtilde
-    
+
     def eval_result(self, c, A, AT, d, e, gamma_c, gamma_b, x, z, y):
         vector_norm = partial(torch.linalg.vector_norm, ord=self.norm_ord)
         m, n = A.shape
         objval = (c / d / gamma_c).T @ (x * d / gamma_b)
         Ax = A @ x
         ATy = AT @ y
         r_norm = vector_norm((Ax - z) / e / gamma_b)
         s_norm = vector_norm((c + ATy) / d / gamma_c)
-        eps_primal = self.abstol * (m**0.5) + self.reltol * max(vector_norm(Ax / e / gamma_b), vector_norm(z / e / gamma_b))
-        eps_dual = self.abstol * (n**0.5) + self.reltol * max(vector_norm(ATy / d / gamma_c),  vector_norm(c / d / gamma_c))
+        # eps_primal = self.abstol * (m**0.5) + self.reltol * max(vector_norm(Ax / e / gamma_b), vector_norm(z / e / gamma_b))
+        # eps_dual = self.abstol * (n**0.5) + self.reltol * max(vector_norm(ATy / d / gamma_c),  vector_norm(c / d / gamma_c))
+        eps_primal = self.abstol + self.reltol * max(vector_norm(Ax / e / gamma_b), vector_norm(z / e / gamma_b))
+        eps_dual = self.abstol + self.reltol * max(vector_norm(ATy / d / gamma_c), vector_norm(c / d / gamma_c))
         return objval, r_norm, s_norm, eps_primal, eps_dual
 
     def extra_repr(self) -> str:
         # gamma_b_mul = torch.exp(self.gamma_b_mul_log).item()
         # gamma_c_mul = torch.exp(self.gamma_c_mul_log).item()
         # rho = torch.exp(self.rho_log).item()
-        
+
         gamma_b_mul = self.gamma_b_mul.item()
         gamma_c_mul = self.gamma_c_mul.item()
-        rho = self.rho.item()        
-        
+        rho = self.rho.item()
+
         sigma = torch.exp(self.sigma_log).item()
         info = f"rho={rho:.3e}; sigma={sigma:.3e}; alpha={self.alpha.item():.3e}; gamma_c_mul={gamma_c_mul:.3e}; gamma_b_mul={gamma_b_mul:.3e};"
         if self.problem_scale is not None:
             d_mul_m = torch.exp(self.d_mul_log).mean()
             e_mul_m = torch.exp(self.e_mul_log).mean()
-            info = info + f" e_mul_m={e_mul_m}; d_mul_m={d_mul_m}"            
+            info = info + f" e_mul_m={e_mul_m}; d_mul_m={d_mul_m}"
         return info
```

### Comparing `dprox-0.1.3/dprox/algo/lp/utils.py` & `dprox-0.2/dprox/algo/lp/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,21 @@
         super().__init__()
         self.A = A
         self.AT = AT
         self.rho = rho
         self.sigma = sigma
 
     def forward(self, x):
-        tmp = (self.A @ x) * self.rho
+        tmp = self.rho * (self.A @ x)
         out = (self.AT @ tmp) + self.sigma * x
         return out
 
+    def clone(self):
+        return LPATA_Func(self.A.clone(), self.AT.clone(), self.rho, self.sigma)
+
 
 class LinearOp(torch.nn.Module):
     def __init__(self, A_fun, AT_fun, shape) -> None:
         super().__init__()
         self.A_fun = A_fun
         self.AT_fun = AT_fun
         self.shape = shape
@@ -42,14 +45,20 @@
         Returns a LinearOperator that represents the transpose of this one.
         Can be abbreviated self.T instead of self.transpose().
         """
         return LinearOp(A_fun=self.AT_fun, AT_fun=self.A_fun, shape=(self.shape[1], self.shape[0]))
 
     T = property(transpose)
 
+    def clone(self):
+        """ The deep copy of this linear operator.
+        """
+        A_fun = self.A_fun.clone()
+        return LinearOp(A_fun, A_fun, self.shape)
+
 
 def Ruiz_equilibration_th(A, c, b, ord=float('inf'), max_iters=20, max_tolerance=1e1, verbose=True):
     vector_norm = partial(torch.linalg.vector_norm, ord=ord)
     MAX_ITER = max_iters
     device = A.device
     m, n = A.shape
     eps_equil = 1e-3
@@ -82,18 +91,18 @@
     Acnorm = torch.linalg.norm(A_bar, ord=ord, dim=0)
 
     b_bar = b * e.view(m, 1)[:b.shape[0]]
     gamma_c = 1 / vector_norm(c_bar) * Arnorm.mean()
     gamma_b = 1 / vector_norm(b_bar) * Acnorm.mean()
 
     if verbose:
-        print(Acnorm.max(), Acnorm.mean())
-        print(Arnorm.max(), Arnorm.mean())
-        print(d.max())
-        print(e.max())
+        print(f'Acnorm: {Acnorm.max():.3f}, {Acnorm.mean():.3f}')
+        print(f'Arnorm: {Arnorm.max():.3f}, {Arnorm.mean():.3f}')
+        print(f'dmax: {d.max():.3f}')
+        print(f'emax: {e.max():.3f}')
 
     return d, e, gamma_c, gamma_b, A_bar
 
 
 def Ruiz_equilibration_sparse_np(A, c, b, ord=float('inf'), max_iters=100, max_tolerance=1e1, verbose=True):
     vector_norm = partial(np.linalg.norm, ord=ord)
     MAX_ITER = max_iters
@@ -124,24 +133,26 @@
         # if ord < float('inf') and (e.max() / d.max() > max_tolerance or d.max() / e.max() > max_tolerance):
         #     break
 
     c_bar = c * d
     Arnorm = slinalg.norm(A_bar, ord=ord, axis=1)
     Acnorm = slinalg.norm(A_bar, ord=ord, axis=0)
 
-    b_bar = b * e[:b.shape[0]]
+    mask = ~np.isinf(b)
+    b_bar = b[mask] * e[mask]
     gamma_c = 1 / vector_norm(c_bar) * Arnorm.mean()
     gamma_b = 1 / vector_norm(b_bar) * Acnorm.mean()
-    # gamma_b = 1
 
     if verbose:
-        print(Acnorm.max(), Acnorm.mean())
-        print(Arnorm.max(), Arnorm.mean())
-        print(d.max())
-        print(e.max())
+        print(f'Acnorm: {Acnorm.max():.3f}, {Acnorm.mean():.3f}')
+        print(f'Arnorm: {Arnorm.max():.3f}, {Arnorm.mean():.3f}')
+        print(f'dmax: {d.max():.3f}')
+        print(f'emax: {e.max():.3f}')
+        print(f'gamma_c: {gamma_c:.3e}')
+        print(f'gamma_b: {gamma_b:.3e}')
 
     return d, e, gamma_c, gamma_b, A_bar
 
 
 def scipy_sparse_to_torchop(A, device=None, output_AT=True):
     A = sparse.coo_matrix(A)
     A_th = torch.sparse_coo_tensor(np.vstack([A.row, A.col]), A.data, size=A.shape).to_sparse_csr().to(device)
```

### Comparing `dprox-0.1.3/dprox/algo/opt/absorb.py` & `dprox-0.2/dprox/algo/opt/absorb.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/opt/equil.py` & `dprox-0.2/dprox/algo/opt/equil.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/opt/merge.py` & `dprox-0.2/dprox/algo/opt/merge.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/pc.py` & `dprox-0.2/dprox/algo/pc.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/pgd.py` & `dprox-0.2/dprox/algo/pgd.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/problem.py` & `dprox-0.2/dprox/algo/problem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,17 @@
-from dprox.linop.constaints import matmul, less, equality
 from typing import List, Union
 
 import torch
 
-from dprox.proxfn import ProxFn
 from dprox.linalg import LinearSolveConfig
+from dprox.linop.constaints import equality, less, matmul
+from dprox.proxfn import ProxFn
 
-from . import opt
 from . import lp
-from .admm import ADMM, ADMM_vxu, LinearizedADMM
-from .base import Algorithm
-from .hqs import HQS
-from .pc import PockChambolle
-from .pgd import ProximalGradientDescent
-from .special import DEQSolver
-
-SOLVERS = {
-    'admm': ADMM,
-    'admm_vxu': ADMM_vxu,
-    'ladmm': LinearizedADMM,
-    'hqs': HQS,
-    'pc': PockChambolle,
-    'pgd': ProximalGradientDescent,
-}
-
-SPECAILIZATIONS = {
-    'deq': DEQSolver
-}
-
-
-def compile(prox_fns, method='admm', device='cuda', **kwargs):
-    algorithm: Algorithm = SOLVERS[method]
-    device = torch.device(device) if isinstance(device, str) else device
-
-    psi_fns, omega_fns = algorithm.partition(prox_fns)
-    solver = algorithm.create(psi_fns, omega_fns, **kwargs)
-    solver = solver.to(device)
-    return solver
-
-
-def specialize(solver, method='deq', **kwargs):
-    return SPECAILIZATIONS[method](solver, **kwargs)
-
-
-def optimize(prox_fns, merge=False, absorb=False):
-    if absorb:
-        prox_fns = opt.absorb.absorb_all_linops(prox_fns)
-    return prox_fns
-
-
-def visualize():
-    pass
+from .primitives import compile
 
 
 class Problem:
     def __init__(
         self,
         prox_fns: Union[ProxFn, List[ProxFn]],
         constraints=[],
```

### Comparing `dprox-0.1.3/dprox/algo/special/deq_utils/jacobian.py` & `dprox-0.2/dprox/algo/specialization/deq/utils/jacobian.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/special/deq_utils/layer_utils.py` & `dprox-0.2/dprox/algo/specialization/deq/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/special/deq_utils/optimizations.py` & `dprox-0.2/dprox/algo/specialization/deq/utils/optimizations.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/special/deq_utils/radam.py` & `dprox-0.2/dprox/algo/specialization/deq/utils/radam.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/special/deq_utils/solvers.py` & `dprox-0.2/dprox/algo/specialization/deq/utils/solvers.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/algo/special/unroll.py` & `dprox-0.2/dprox/algo/specialization/unroll.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-import torch.nn as nn
 import copy
+from functools import partial
+
 import torch
+import torch.nn as nn
+
+from ..base import auto_convert_to_tensor, move
+
+
+def clone(x, nums, share):
+    return [x if share else copy.deepcopy(x) for _ in range(nums)]
 
-from ..base import move, auto_convert_to_tensor
 
-def clone(x, nums, shared):
-    return [x if shared else copy.deepcopy(x) for _ in range(nums)]
+def build_unrolled_solver(solver, share=True, **kwargs):
+    if share == True:
+        solver.solve = partial(solver.solve, **kwargs)
+        return solver
+    return UnrolledSolver(solver, share=share, **kwargs)
 
 
 class UnrolledSolver(nn.Module):
-    def __init__(self, solver, max_iter, shared=False, learned_params=False):
+    def __init__(self, solver, max_iter, share=False, learned_params=False):
         super().__init__()
-        if shared==False:   
-            self.solvers = nn.ModuleList(clone(solver, max_iter, shared=shared))
+        if share == False:
+            self.solvers = nn.ModuleList(clone(solver, max_iter, share=share))
         else:
             self.solver = solver
             self.solvers = [self.solver for _ in range(max_iter)]
-            
+
         self.max_iter = max_iter
-        self.shared = shared
-        
+        self.share = share
+
         self.learned_params = learned_params
         if learned_params:
             self.rhos = nn.parameter.Parameter(torch.ones(max_iter))
             self.lams = {}
             for fn in solver.psi_fns:
                 lam = nn.parameter.Parameter(torch.ones(max_iter))
                 setattr(self, str(fn), lam)
@@ -31,18 +41,18 @@
 
     @auto_convert_to_tensor(['x0', 'rhos', 'lams'], batchify=['x0'])
     def solve(self, x0=None, rhos=None, lams=None, max_iter=None):
         x0, rhos, lams = move(x0, rhos, lams, device=self.solvers[0].device)
 
         if self.learned_params:
             rhos, lams = self.rhos, self.lams
-            
+
         max_iter = self.max_iter if max_iter is None else max_iter
-        
+
         state = self.solvers[0].initialize(x0)
-        
+
         for i in range(max_iter):
-            rho = rhos[..., i:i+1]
-            lam = {self.solvers[i].psi_fns[0]: v[..., i:i+1] for k, v in lams.items()}
+            rho = rhos[..., i:i + 1]
+            lam = {self.solvers[i].psi_fns[0]: v[..., i:i + 1] for k, v in lams.items()}
             state = self.solvers[i].iters(state, rho, lam, 1, False)
-        
-        return state[0]
+
+        return state[0]
```

### Comparing `dprox-0.1.3/dprox/algo/tune/autotune.py` & `dprox-0.2/dprox/algo/specialization/rl/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,23 @@
     random.seed(seed)
     if torch.cuda.is_available(): torch.cuda.manual_seed_all(seed)
     torch.backends.cudnn.deterministic = True
     torch.backends.cudnn.benchmark = True
 
 
 def complex2channel(x):
+    """
+    convert a complex tensor with shape (N, C, H, W, 2) to a real tensor with shape (N,
+    2C, H, W).
+
+    :param x: The input tensor to the function `complex2channel`. It is expected to have a shape of `(N,
+    C, H, W, 2)`, where `N` is the batch size, `C` is the number of channels, `H` and `W` are the height
+    :return: a tensor of shape `(N, 2C, H, W)` where the last dimension of `x` has been flattened and moved to the
+    second dimension of the output tensor. 
+    """
     x = torch.view_as_real(x)
     N, C, H, W, _ = x.shape
     # N C H W 2 -> N 2 C H W
     x = x.permute(0, 1, 4, 2, 3).contiguous()
     x = x.view(N, C * 2, H, W)
     return x
 
@@ -144,15 +153,14 @@
 
 
 class TFPnPSolver(PnPSolver):
     def __init__(self, solver, solver_params):
         super().__init__(None)
         self.solver = solver
         self.solver_params = solver_params
-
         self.state_dim = solver.state_dim
 
     def forward(self, inputs, parameters, iter_num=None):
         variables, additional_params = inputs
         rhos, weights = parameters
 
         # infer iter_num from provided hyperparameters
@@ -166,24 +174,39 @@
                                    rhos=rhos,
                                    lams=weights,
                                    max_iter=iter_num)
 
         return self.solver.pack(states)
 
     def reset(self, data):
+        """
+        reset the solver with new data and return the packed states.
+
+        :param data: a dictionary containing the input data for the function
+        :return: the packed states after initializing the solver with the given data.
+        """
         x0 = data['x0'].clone().detach()  # [B,1,W,H,2]
         for k in self.solver_params:
             self.solver_params[k].value = data['params'][k]
         states = self.solver.initialize(x0)
         return self.solver.pack(states)
 
     def get_output(self, state):
         return self.solver.unpack(state)[0].real
 
     def filter_hyperparameter(self, action):
+        """
+        filter out the 'idx_stop' and 'rho' keys from the input dictionary and return
+        the remaining keys as weights, along with the value of 'rho'.
+
+        :param action: a dictionary that contains hyperparameters for a proximal solver. 
+        :return: a tuple containing two values: `rhos` and `weights`. `rhos` is the value of the 'rho'
+        key in the `action` dictionary, and `weights` is a new dictionary that contains all the
+        key-value pairs from `action` except for the 'idx_stop' and 'rho' keys.
+        """
         rhos = action['rho']
         weights = {k: v for k, v in action.items() if k not in ['idx_stop', 'rho']}
         return rhos, weights
 
     def filter_aux_inputs(self, state):
         return state['params']
 
@@ -283,20 +306,20 @@
         self.solver = solver
         # TODO: compute ob_dim based on ckpt
         self.policy = make_policy(solver, action_pack, ob_dim=9, type=policy)
         self.policy.eval()
         self.max_episode_step = max_episode_step
         self.custom_policy_ob_pack_fn = custom_policy_ob_pack_fn
 
-    def solve(self, x0, aux_state=None, pbar=False):
+    def solve(self, x0, aux_state=None, pbar=False, callback=None):
         x0 = x0.to(self.solver.device)
         state = self.solver.initialize(x0)
         for i in tqdm(range(self.max_episode_step), disable=not pbar):
             rhos, lams, idx_stop = self.estimate(state, i, x0, aux_state)
-            state = self.solver.iters(state, rhos, lams, self.policy.action_bundle)
+            state = self.solver.iters(state, rhos, lams, self.policy.action_bundle, callback=callback)
         return state[0]
 
     @torch.no_grad()
     def estimate(self, states, iter, b, aux_state=None):
         policy_ob = self.solver.pack(states)
         B, _, W, H = policy_ob.shape
```

### Comparing `dprox-0.1.3/dprox/linalg/solve/minres.py` & `dprox-0.2/dprox/linalg/solve/solver_minres.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 # MIT-licensed code imported from https://github.com/cornellius-gp/linear_operator
 # Minor modifications for torchsparsegradutils to remove dependencies
+from typing import Callable
+
 import torch
-from dprox import LinOp
+from typing import Callable
 
 
 def _pad_with_singletons(obj, num_singletons_before=0, num_singletons_after=0):
     """
     Pad obj with singleton dimensions on the left and right
     Example:
         >>> x = torch.randn(10, 5)
         >>> _pad_width_singletons(x, 2, 3).shape
         >>> # [1, 1, 10, 5, 1, 1, 1]
     """
     new_shape = [1] * num_singletons_before + list(obj.shape) + [1] * num_singletons_after
     return obj.view(*new_shape)
 
 
-# NOTE: MINRES solver does not support Unrolling mode 
-def MINRES(
-    A: LinOp,
-    b,
-    eps=1e-25,
-    shifts=None,
-    value=None,
-    rtol=1e-6,
-    max_iters=100,
-    preconditioner=None,    
-    verbose=False,
+def minres(
+    A: Callable,
+    b: torch.Tensor,
+    x0: torch.Tensor = None,
+    rtol: float = 1e-6,
+    max_iters: int = 100,
+    verbose: bool = False,
+    Minv: Callable = None,
+    eps: float =1e-25,
+    shifts: torch.Tensor =None,
+    value: float =None,
 ):
     r"""
-    Perform MINRES to find solutions to :math:`(\mathbf K + \alpha \sigma \mathbf I) \mathbf x = \mathbf b`.
+    Perform MINRES to find solutions to :math:`(K + \alpha \sigma  I) x =  b`.
     Will find solutions for multiple shifts :math:`\sigma` at the same time.
 
-    :param callable A: Function to perform matmul with.
-    :param torch.Tensor b: The vector :math:`\mathbf b` to solve against.
-    :param torch.Tensor shifts: (default None) The shift :math:`\sigma` values. If set to None,
-        then :math:`\sigma=0`.
-    :param float value: (default None) The multiplicative constant :math:`\alpha`. If set to None,
-        then :math:`\alpha=0`.
-    :param int max_iters: (default None) The maximum number of minres iterations. 
-    :rtype: torch.Tensor
-    :return: The solves :math:`\mathbf x`. The shape will correspond to the size of `b` and `shifts`.
+    Args:
+      A (Callable): A is a callable function representing the forward operator A(x) of a matrix free linear operator.
+      b (torch.Tensor): The parameter `b` is a tensor representing the right-hand side of the linear
+        system of equations `Ax = b`.
+      x0 (torch.Tensor): The initial guess for the solution vector. If not provided, it is initialized
+        to a vector of zeros.
+      rtol (float): Relative tolerance for convergence criteria. Default to 1e-6
+      max_iters (int): The maximum number of iterations. Defaults to 100
+      verbose (bool): Whether to logging intermediate information. Defaults to False
+      Minv (Callable):  A callable function representing the preconditioner.
+      shifts (torch.Tensor): The shift :math:`\sigma` values. If set to None, then :math:`\sigma=0`.
+      vlaue (float): The multiplicative constant :math:`\alpha`. If set to None, then :math:`\alpha=0`.
+
+    Returns:
+      The solves :math:`x`. The shape will correspond to the size of `b` and `shifts`.
+
+    Note:
+      MINRES solver does not support Unrolling mode
     """
-    # Default values    
-    if preconditioner is None:
-        preconditioner = lambda x: x.clone()
+    # Default values
+    if Minv is None:
+        def Minv(x): return x.clone()
 
     if shifts is None:
         shifts = torch.tensor(0.0, dtype=b.dtype, device=b.device)
 
     # Scale the b
     squeeze = False
     if b.dim() == 1:
@@ -74,15 +85,15 @@
     # Resize shifts
     shifts = _pad_with_singletons(shifts, 0, prod.dim() - shifts.dim() + 1)
     solution = torch.zeros(shifts.shape[:1] + prod.shape, dtype=b.dtype, device=b.device)
 
     # Variables for Lanczos terms
     zvec_prev2 = torch.zeros_like(prod)
     zvec_prev1 = b.clone().expand_as(prod).contiguous()
-    qvec_prev1 = preconditioner(zvec_prev1)
+    qvec_prev1 = Minv(zvec_prev1)
     alpha_curr = torch.empty(prod.shape[:-2] + (1, prod.size(-1)), dtype=b.dtype, device=b.device)
     alpha_shifted_curr = torch.empty(solution.shape[:-2] + (1, prod.size(-1)), dtype=b.dtype, device=b.device)
     beta_prev = (zvec_prev1 * qvec_prev1).sum(dim=-2, keepdim=True).sqrt_()
     beta_curr = torch.empty_like(beta_prev)
     tmpvec = torch.empty_like(qvec_prev1)
 
     # Divide by beta_prev
@@ -118,15 +129,15 @@
     scale_curr = torch.empty_like(scale_prev)
 
     # Terms for checking for convergence
     solution_norm = torch.zeros(*solution.shape[:-2], solution.size(-1), dtype=solution.dtype, device=solution.device)
     search_update_norm = torch.zeros_like(solution_norm)
 
     # Maybe log
-    if verbose:        
+    if verbose:
         print(
             f"Running MINRES on a {b.shape} RHS for {max_iters} iterations (rtol={rtol}). "
             f"Output: {solution.shape}."
         )
 
     bnorm = torch.linalg.vector_norm(b)
     # Perform iterations
@@ -139,15 +150,15 @@
         # Get next Lanczos terms
         # --> alpha_curr, beta_curr, qvec_curr
         torch.mul(prod, qvec_prev1, out=tmpvec)
         torch.sum(tmpvec, -2, keepdim=True, out=alpha_curr)
 
         zvec_curr = prod.addcmul_(alpha_curr, zvec_prev1, value=-1).addcmul_(beta_prev, zvec_prev2, value=-1)
 
-        qvec_curr = preconditioner(zvec_curr)
+        qvec_curr = Minv(zvec_curr)
         torch.mul(zvec_curr, qvec_curr, out=tmpvec)
         torch.sum(tmpvec, -2, keepdim=True, out=beta_curr)
         beta_curr.sqrt_()
         beta_curr.clamp_min_(eps)
 
         zvec_curr.div_(beta_curr)
         qvec_curr.div_(beta_curr)
```

### Comparing `dprox-0.1.3/dprox/linop/__init__.py` & `dprox-0.2/dprox/linop/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .blackbox import LinOpFactory, BlackBox
 from .conv import conv, conv_doe
 from .constant import Constant
-from .comp_graph import CompGraph, est_CompGraph_norm, eval, adjoint, gram
+from .comp_graph import CompGraph, est_CompGraph_norm, eval, adjoint, gram, validate
 from .scale import scale
 from .subsample import mosaic
 from .sum import sum, copy
 from .variable import Variable
 from .base import LinOp
 from .vstack import vstack, split
 from .placeholder import Placeholder
```

### Comparing `dprox-0.1.3/dprox/linop/base.py` & `dprox-0.2/dprox/linop/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Converts a non-LinOp to a Constant.
     """
     from .constant import Constant
     return expr if isinstance(expr, LinOp) else Constant(expr)
 
 
 class LinOp(nn.Module):
-    """Represents a linear operator.
+    """ Abstract class for all linear operator.
     """
 
     class MultOutput(list): pass
 
     instanceCnt = 0
 
     def __init__(self, input_nodes=[]):
@@ -152,28 +152,34 @@
         return NotImplemented
 
     # ---------------------------------------------------------------------------- #
     #                                     Util                                     #
     # ---------------------------------------------------------------------------- #
 
     @property
-    def T(self):
+    def T(self) -> 'LinOp':
+        """ The transpose :math:`A^T` of this linear operator :math:`A`.
+        """
         op = self.clone()
         op.forward, op.adjoint = op.adjoint, op.forward
         return op
 
     @property
-    def gram(self):
+    def gram(self) -> 'LinOp':
+        """ The gram :math:`A^TA` of this linear operator :math:`A`$`.
+        """
         op = self.clone()
         forward, adjoint = op.forward, op.adjoint
         op.forward = lambda inputs: adjoint(forward(inputs))
         op.adjoint = lambda inputs: forward(adjoint(inputs))
         return op
 
-    def clone(self):
+    def clone(self) -> 'LinOp':
+        """ The deep copy of this linear operator.
+        """
         return copy.deepcopy(self)
 
     def unwrap(self, value):
         from .placeholder import Placeholder
         if isinstance(value, Placeholder):
             return value.value
         return to_torch_tensor(value, batch=True)
```

### Comparing `dprox-0.1.3/dprox/linop/blackbox.py` & `dprox-0.2/dprox/linop/blackbox.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/linop/comp_graph.py` & `dprox-0.2/dprox/linop/comp_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,15 +339,15 @@
         if save_path is None:
             display(dot)
 
     def sanity_check(self, eps=1e-5):
         """ Perform dot product test to check the sanity of this linear operator
         """
         from scipy.misc import face
-        m = torch.from_numpy(face().copy()).float().cuda() / 255
+        m = torch.from_numpy(face().copy()).float() / 255
         m = m.permute(2, 0, 1).unsqueeze(0)
         d = self.forward(m)
 
         if isinstance(d, LinOp.MultOutput):
             d2 = [torch.rand_like(e) for e in d]
             m2 = self.adjoint(*d2)
             sum_m = torch.sum(m * m2)
@@ -419,14 +419,21 @@
     A = LinearOperator((K.input_size, K.input_size),
                        KtK, KtK)
 
     Knorm = np.sqrt(eigs(A, k=1, M=None, sigma=None, which='LM', tol=tol)[0].real)
     return np.float(Knorm)
 
 
+def validate(linop: LinOp) -> bool:
+    """ Validate the implementation of the linear operator via dot-product test.
+    """
+    K = CompGraph(linop)
+    return K.sanity_check()
+
+
 def eval(linop, *inputs, zero_out_constant=True):
     G = CompGraph(linop, zero_out_constant)
     if len(inputs) > 1:
         return G.forward(*inputs)
     elif len(inputs) == 1:
         return G.forward(inputs[0])
     else:
```

### Comparing `dprox-0.1.3/dprox/linop/constant.py` & `dprox-0.2/dprox/linop/constant.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/linop/conv.py` & `dprox-0.2/dprox/linop/conv.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/linop/grad.py` & `dprox-0.2/dprox/linop/grad.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/linop/scale.py` & `dprox-0.2/dprox/linop/scale.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/linop/subsample.py` & `dprox-0.2/dprox/linop/subsample.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/linop/sum.py` & `dprox-0.2/dprox/linop/sum.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/linop/variable.py` & `dprox-0.2/dprox/linop/variable.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/linop/vstack.py` & `dprox-0.2/dprox/linop/vstack.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/base.py` & `dprox-0.2/dprox/proxfn/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 def prox_translated(prox, b):
     def _prox(v, lam):
         return prox(v - b, lam) + b
     return _prox
 
 
 class ProxFn(nn.Module):
-    """ The definition of proximal operator is
+    """ The abstract class for the proximal operator.
         f(x) = argmin_x f(x) + 1/(2*lam) * ||x-v||_2^2 
     """
 
     def __init__(self, linop: LinOp, alpha=1, beta=1):
         super().__init__()
         self.linop = linop
         self.alpha = alpha
```

### Comparing `dprox-0.1.3/dprox/proxfn/fast/cs.py` & `dprox-0.2/dprox/proxfn/fast/cs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/fast/pr.py` & `dprox-0.2/dprox/proxfn/fast/pr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/fast/spi.py` & `dprox-0.2/dprox/proxfn/fast/spi.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/fast/sr.py` & `dprox-0.2/dprox/proxfn/fast/sr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/nlm/nlm.py` & `dprox-0.2/dprox/proxfn/nlm/nlm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/norm.py` & `dprox-0.2/dprox/proxfn/norm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/base.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/composite.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/composite.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/TV_denoising.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/TV_denoising.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/basicblock.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_dncnn.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_dncnn.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/network_unet.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/network_unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/models/unet/unet.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/denoisers/wrapper.py` & `dprox-0.2/dprox/proxfn/pnp/denoisers/wrapper.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/pnp/prior.py` & `dprox-0.2/dprox/proxfn/pnp/prior.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import copy
 
 import torch
 import torch.nn as nn
 
-from dprox.utils.io import get_path
+from dprox.utils import hf
 
 from ..base import ProxFn
 from .denoisers import (DRUNetDenoiser, FFDNetColorDenoiser, FFDNetDenoiser,
                         GRUNetDenoiser, IRCNNDenoiser, UNetDenoiser)
 from .denoisers.composite import Augment
 
 
 def get_denoiser(type):
     if type == 'ffdnet':
-        model_path = get_path('denoiser/ffdnet_gray.pth')
+        model_path = hf.load_path('pnp_denoiser/ffdnet_gray.pth', repo_type='models')
         return FFDNetDenoiser(model_path)
     if type == 'ffdnet_color':
-        model_path = get_path('denoiser/ffdnet_color.pth')
+        model_path = hf.load_path('pnp_denoiser/ffdnet_color.pth', repo_type='models')
         return FFDNetColorDenoiser(model_path)
     if type == 'drunet_color':
-        model_path = get_path('denoiser/drunet_color.pth')
+        model_path = hf.load_path('pnp_denoiser/drunet_color.pth', repo_type='models')
         return DRUNetDenoiser(3, model_path)
     if type == 'drunet':
-        model_path = get_path('denoiser/drunet_gray.pth')
+        model_path = hf.load_path('pnp_denoiser/drunet_gray.pth', repo_type='models')
         return DRUNetDenoiser(1, model_path)
     if type == 'ircnn':
-        model_path = get_path('denoiser/ircnn_gray.pth')
+        model_path = hf.load_path('pnp_denoiser/ircnn_gray.pth', repo_type='models')
         return IRCNNDenoiser(1, model_path)
     if type == 'grunet':
-        model_path = get_path('denoiser/unet_qrnn3d.pth')
+        model_path = hf.load_path('pnp_denoiser/unet_qrnn3d.pth', repo_type='models')
         return GRUNetDenoiser(model_path)
     if type == 'unet':
-        model_path = get_path('denoiser/unet-nm.pt')
+        model_path = hf.load_path('pnp_denoiser/unet-nm.pt', repo_type='models')
         return UNetDenoiser(model_path)
 
 
 def clone(x, nums, shared):
     return [x if shared else copy.deepcopy(x) for _ in range(nums)]
 
 
@@ -70,15 +70,15 @@
     def eval(self, v):
         raise NotImplementedError('deep prior cannot be explictly evaluated')
 
     def _prox(self, v: torch.Tensor, lam: torch.Tensor):
         """ v: [N, C, H, W] or [N, H, W]
             lam: [1]
         """
-        if self.sqrt: lam = lam.sqrt()
+        # if self.sqrt: lam = lam.sqrt()
         if self.clamp: v = v.clamp(0, 1)
         if torch.is_complex(v): v = v.real
         if len(v.shape) == 3: input = v.unsqueeze(1)
         else: input = v
         if self.unroll: out = self.denoisers[self.step].denoise(input, lam)
         else: out = self.denoiser.denoise(input, lam)
         out = out.type_as(v)
```

### Comparing `dprox-0.1.3/dprox/proxfn/sum_square.py` & `dprox-0.2/dprox/proxfn/sum_square.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/proxfn/unrolling/dgu.py` & `dprox-0.2/dprox/proxfn/unrolling/dgu.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/utils/containar.py` & `dprox-0.2/dprox/utils/containar.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/utils/examples/derain/custom_linop.py` & `dprox-0.2/dprox/contrib/derain.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,7 @@
         if step is None: step = self.step
         if step == 0:
             return self.phid_0(x)
         elif step == self.max_step + 1:
             return self.phid_6(x)
         else:
             return self.phid_1(x)
-
```

### Comparing `dprox-0.1.3/dprox/utils/examples/energy_system/__init__.py` & `dprox-0.2/dprox/contrib/energy_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from scipy import io
 
-from dprox.utils.io import get_path
+from dprox.utils.huggingface import load_path
 
 
 def load_simple_cep_model():
-    model_components = io.loadmat(get_path("data/energy_system/simple_cep_model_20220916/esm_instance.mat"))
+    model_components = io.loadmat(load_path("energy_system/simple_cep_model_20220916/esm_instance.mat"))
     n_con, n_var = model_components["A"].shape
     print("Number of linear constraints (w/o bound constraints):", n_con)
     print("Number of decision variables:", n_var)
 
     A = model_components["A"].astype(np.float64)
     b = model_components["rhs"].astype(np.float64)
     types = model_components["sense"]
```

### Comparing `dprox-0.1.3/dprox/utils/examples/optic/doe_model.py` & `dprox-0.2/dprox/contrib/optic/doe_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-#%%
+from dataclasses import dataclass, field
+
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-import numpy as np
 
 
 def get_coordinate(nx, ny, dx, dy):
     """
     return the coordinates of a 2D grid with given dimensions and spacing.
-    
+
     :param nx: The number of points in the x-direction
     :param ny: The number of points along the y-axis in a 2D grid
     :param dx: The spacing between two adjacent points along the x-axis
     :param dy: The spacing between the y-coordinates of the grid points. 
     :return: two tensors `xx` and `yy` which represent the x and y
     coordinates of a 2D grid. The size of the grid is determined by the input parameters `nx` and `ny`,
     and the spacing between grid points is determined by `dx` and `dy`.
@@ -23,15 +24,15 @@
     return xx, yy
 
 
 def area_downsampling(input, target_side_length):
     """
     downsample an input image to a target side length by averaging the pixel values in
     each block of pixels.
-    
+
     :param input: a 3-dimensional tensor representing an image, with dimensions (channels, height,
     width)
     :param target_side_length: The target side length is the desired length of one side of the output
     image after downsampling
     :return: the downsampled version of the input image with the target side length using average
     pooling.
     """
@@ -44,15 +45,15 @@
 
 
 def psf2otf(psf, output_size):
     """
     take a point spread function and output size as inputs, pad the PSF with zeros to
     match the output size, circularly shifts the PSF so the center pixel is at 0,0, and returns the
     optical transfer function.
-    
+
     :param psf: The point spread function (PSF) is a 4-dimensional tensor representing the blur kernel
     used in image processing. It is typically used in image deconvolution to recover the original image
     from a blurred image
     :param output_size: The desired size of the output Optical Transfer Function (OTF) after padding the
     Point Spread Function (PSF) with zeros. It is a tuple of the form (batch_size, num_channels, height,
     width)
     :return: the optical transfer function (OTF) of the point spread function (PSF) after padding and
@@ -81,15 +82,15 @@
     return otf
 
 
 def img_psf_conv(img, psf, circular=False):
     """
     perform image convolution with a point spread function (PSF) and can handle both
     circular and linearized convolutions.
-    
+
     :param img: a 4-dimensional tensor representing an image, with dimensions (batch_size, channels,
     height, width)
     :param psf: The point spread function (PSF) is a 4-dimensional tensor representing the blur kernel
     used in image processing. It is typically used in image deconvolution to recover the original image
     from a blurred image
     :param circular: A boolean parameter that determines whether the convolution should be circular or
     linearized. If circular is True, then circular convolution is performed. If circular is False, then
@@ -123,15 +124,15 @@
         self.input_shape = input_shape
         self.distance = distance
         self.wave_lengths = wave_lengths
         self.wave_nos = 2. * torch.pi / wave_lengths
         self.discretization_size = discretization_size
         H = self._setup_H()
         self.register_buffer('H', H, persistent=False)
-        
+
     def _setup_H(self):
         """
         set up the transfer function H for a Fresnel propagator.
         :return: the complex-valued transfer function H.
         """
         _, _, M_orig, N_orig = self.input_shape
         # zero padding.
@@ -147,26 +148,26 @@
         fy = yy / (self.discretization_size * M)
 
         fx = torch.fft.ifftshift(fx)
         fy = torch.fft.ifftshift(fy)
 
         squared_sum = (fx ** 2 + fy ** 2)[None][None]
         phi = - torch.pi * self.distance * self.wave_lengths.view(1, 3, 1, 1) * squared_sum
-        H = torch.exp(1j * phi)        
+        H = torch.exp(1j * phi)
         return H
-        
+
     def forward(self, input_field):
         Npad, Mpad = self.Npad, self.Mpad
         padded_input_field = F.pad(input=input_field, pad=[Npad, Npad, Mpad, Mpad])
-        
+
         objFT = torch.fft.fft2(padded_input_field)
         out_field = torch.fft.ifft2(objFT * self.H)
         return out_field[:, :, Mpad:-Mpad, Npad:-Npad]
-        
-        
+
+
 def get_one_phase_shift_thickness(wave_lengths, refractive_index):
     """Calculate the thickness (in meter) of a phaseshift of 2pi.
     """
     # refractive index difference
     delta_N = refractive_index - 1.
     # wave number
     wave_nos = 2. * torch.pi / wave_lengths
@@ -184,66 +185,66 @@
         wave_nos = 2. * torch.pi / wave_lengths
         wave_nos = wave_nos.view([1, -1, 1, 1])
         self.register_buffer('delta_N', delta_N, persistent=False)
         self.register_buffer('wave_nos', wave_nos, persistent=False)
         self.xx = xx
         self.yy = yy
         self.sensor_distance = sensor_distance
-        
+
         # height_map_sqrt = torch.ones(size=height_map_shape) * 1e-4
         height_map_sqrt = self._fresnel_phase_init(1)
         self.height_map_sqrt = nn.Parameter(height_map_sqrt)
-        
+
     def _fresnel_phase_init(self, idx=1):
         """
         calculate the Fresnel lens phase and convert it to a height map.
-        
+
         :param idx: idx is an optional parameter that specifies the index of the wavelength to use in
         the calculation. It is set to 1 by default, defaults to 1 (optional)
         :return: the square root of the height map calculated from the Fresnel phase.
         """
         k = 2 * torch.pi / self.wave_lengths[idx]
-        fresnel_phase = - k * ((self.xx**2 + self.yy**2)[None][None] / (2*self.sensor_distance))
+        fresnel_phase = - k * ((self.xx**2 + self.yy**2)[None][None] / (2 * self.sensor_distance))
         fresnel_phase = fresnel_phase % (torch.pi * 2)
         height_map = self.phase_to_height_map(fresnel_phase, idx)
         return height_map ** 0.5
-        
+
     def get_phase_profile(self, height_map=None):
         """
         calculate the phase profile of a height map using wave numbers and phase delay.
-        
+
         :param height_map: A 2D tensor representing the height map of the surface. It is used to
         calculate the phase delay induced by the height field
         :return: a complex exponential phase profile calculated from the input height map.
         """
         if height_map is None:
-            height_map = torch.square(self.height_map_sqrt+1e-7)
+            height_map = torch.square(self.height_map_sqrt + 1e-7)
         # phase delay indiced by height field
         phi = self.wave_nos * self.delta_N * height_map
         return torch.exp(1j * phi)
 
     def phase_to_height_map(self, phi, wave_length_idx=1):
         """
         take in a phase map and return a corresponding height map using the given wave
         length and refractive index.
-        
+
         :param phi: The phase profile of the height map at a specific wavelength associated with `wave_length_idx`
         :param wave_length_idx: The index of the wavelength in the list of available wavelengths. This
         is used to retrieve the corresponding `delta_N` value for the given wavelength, defaults to 1
         (optional)
         :return: a height map calculated from the input phase and other parameters such as wave length
         and delta N.
         """
         wave_length = self.wave_lengths[wave_length_idx]
         delta_n = self.delta_N.view(-1)[wave_length_idx]
         k = 2. * torch.pi / wave_length
         phi = phi % (2 * torch.pi)
         height_map = phi / k / delta_n
         return height_map
-        
+
 
 class RGBCollimator(nn.Module):
     def __init__(self,
                  sensor_distance,
                  refractive_idcs,
                  wave_lengths,
                  patch_size,
@@ -254,20 +255,20 @@
         self.wave_res = wave_resolution
         self.wave_lengths = wave_lengths
         self.sensor_distance = sensor_distance
         self.sample_interval = sample_interval
         self.patch_size = patch_size
         self.refractive_idcs = refractive_idcs
         self._init_setup()
-        
+
     def get_psf(self, phase_profile=None):
         """
         calculate the point spread function (PSF) of an optical system given a phase
         profile and other parameters.
-        
+
         :param phase_profile: A 2D tensor representing the phase profile of the optical system. It is
         multiplied element-wise with the input field before propagation
         :return: a PSF (Point Spread Function) which is a 2D tensor representing the intensity
         distribution of the image formed by a point source after passing through the optical system.
         """
         if phase_profile is None:
             phase_profile = self.height_map.get_phase_profile()
@@ -275,148 +276,104 @@
         field = self.aperture * field
         field = self.propagator(field)
         psfs = (torch.abs(field) ** 2).float()
         psfs = area_downsampling(psfs, self.patch_size)
         # psfs = psfs / psfs.sum(dim=[2, 3], keepdim=True)
         psfs = psfs / psfs.sum()
         return psfs
-        
+
     def forward(self, input_img, phase_profile=None, circular=False):
         psfs = self.get_psf(phase_profile)
         output_image = img_psf_conv(input_img, psfs, circular=circular)
         return output_image, psfs
-    
+
     def _init_setup(self):
         input_field = torch.ones((1, len(self.wave_lengths), self.wave_res[0], self.wave_res[1]))
         self.register_buffer("input_field", input_field, persistent=False)
-        
-        xx, yy = get_coordinate(self.wave_res[0], self.wave_res[1], 
+
+        xx, yy = get_coordinate(self.wave_res[0], self.wave_res[1],
                                 self.sample_interval, self.sample_interval)
         self.register_buffer("xx", xx, persistent=False)
         self.register_buffer("yy", yy, persistent=False)
 
         aperture = self._get_circular_aperture(xx, yy)
         self.register_buffer("aperture", aperture, persistent=False)
-        
+
         self.height_map = self._get_height_map()
         self.propagator = self._get_propagator()
 
     def _get_height_map(self):
         height_map_shape = (1, 3, self.wave_res[0], self.wave_res[1])
-        height_map = HeightMap(height_map_shape, 
+        height_map = HeightMap(height_map_shape,
                                self.wave_lengths,
                                self.refractive_idcs,
                                self.xx, self.yy,
                                self.sensor_distance)
         return height_map
-    
+
     def _get_propagator(self):
         input_shape = (1, 3, self.wave_res[0], self.wave_res[1])
-        propagator = FresnelPropagator(input_shape, 
-                                       self.sensor_distance, 
-                                       self.sample_interval, 
+        propagator = FresnelPropagator(input_shape,
+                                       self.sensor_distance,
+                                       self.sample_interval,
                                        self.wave_lengths)
         return propagator
-        
+
     def _get_circular_aperture(self, xx, yy):
         max_val = xx.max()
         r = torch.sqrt(xx ** 2 + yy ** 2)
         aperture = (r < max_val).float()[None][None]
         return aperture
 
 
-def center_crop(im, new_height, new_width):
-    width, height = im.size   # Get dimensions
-
-    left = round((width - new_width)/2)
-    top = round((height - new_height)/2)
-    x_right = round(width - new_width) - left
-    x_bottom = round(height - new_height) - top
-    right = width - x_right
-    bottom = height - x_bottom
-
-    # Crop the center of the image
-    im = im.crop((left, top, right, bottom))    
-    return im
-
-
-if __name__ == '__main__':
-    import matplotlib.pylab as plt
-    import PIL.Image as Image
-    
-    aperture_diameter = 3e-3
-    sensor_distance = 15e-3  # Distance of sensor to aperture
+@dataclass
+class DOEModelConfig:
+    circular: bool = True  # circular convolution
+    aperture_diameter: float = 3e-3  # aperture diameter
+    sensor_distance: float = 15e-3  # Distance of sensor to aperture
     refractive_idcs = torch.tensor([1.4648, 1.4599, 1.4568])  # Refractive idcs of the phaseplate
     wave_lengths = torch.tensor([460, 550, 640]) * 1e-9  # Wave lengths to be modeled and optimized for
-    num_steps = 10001  # Number of SGD steps
+    num_steps: int = 10001  # Number of SGD steps
     # patch_size = 1248  # Size of patches to be extracted from images, and resolution of simulated sensor
-    patch_size = 748  # Size of patches to be extracted from images, and resolution of simulated sensor
-    sample_interval = 2e-6  # Sampling interval (size of one "pixel" in the simulated wavefront)
+    patch_size: int = 748  # Size of patches to be extracted from images, and resolution of simulated sensor
+    sample_interval: float = 2e-6  # Sampling interval (size of one "pixel" in the simulated wavefront)
     wave_resolution = 1496, 1496  # Resolution of the simulated wavefront
+    model_kwargs: dict = field(default_factory=dict)
 
-    device = torch.device('cuda')
-    
-    img = Image.open('./8068.jpg')
-    img = center_crop(img, patch_size // 2, patch_size // 2)
-    img = img.resize((patch_size, patch_size), Image.BICUBIC)
-    x = torch.from_numpy(np.array(img).transpose((2, 0, 1)) / 255.)[None].to(device)
-    
-    # x = torch.zeros((1, 3, patch_size, patch_size), device=device)    
-    # x[..., patch_size//2, patch_size//2] = 1
-
-    rgb_collim_model = RGBCollimator(sensor_distance,
-                                     refractive_idcs=refractive_idcs,
-                                     wave_lengths=wave_lengths,
-                                     patch_size=patch_size,
-                                     sample_interval=sample_interval,
-                                     wave_resolution=wave_resolution,
+
+def build_doe_model(config: DOEModelConfig = DOEModelConfig()):
+    """
+    build a DOE (Diffractive Optical Element) model using the input configuration.
+
+    :param config: DOEModelConfig object that contains the following parameters:
+    :type config: DOEModelConfig
+    :return: The function `build_doe_model` is returning an instance of the `RGBCollimator` class, which
+    is initialized with the parameters passed in the `DOEModelConfig` object `config`.
+    """
+    rgb_collim_model = RGBCollimator(config.sensor_distance,
+                                     refractive_idcs=config.refractive_idcs,
+                                     wave_lengths=config.wave_lengths,
+                                     patch_size=config.patch_size,
+                                     sample_interval=config.sample_interval,
+                                     wave_resolution=config.wave_resolution,
                                      )
-    
-    # ideal fresnel lens 
-    # k = 2 * torch.pi / wave_lengths.to(device)
-    # fresnel_phase_c = - k.view(3, 1, 1) * ((rgb_collim_model.xx**2 + rgb_collim_model.yy**2)[None] / (2*sensor_distance))
-    # fresnel_phase_c = fresnel_phase_c % (torch.pi * 2)
-    # fresnel_phase_c = torch.exp(1j * fresnel_phase_c)[None]
-
-    # real fresnel lens
-    k = 2 * torch.pi / wave_lengths[1]
-    fresnel_phase = - k * ((rgb_collim_model.xx**2 + rgb_collim_model.yy**2)[None][None] / (2*sensor_distance))
+    return rgb_collim_model
+
+
+def build_baseline_profile(rgb_collim_model: RGBCollimator):
+    """
+    build a baseline profile for a given RGB collimator model by calculating the Fresnel
+    phase and height map.
+
+    :param rgb_collim_model: An instance of the RGBCollimator class, which likely represents a system
+    for collimating light of different wavelengths (red, green, and blue) onto a sensor or detector
+    :type rgb_collim_model: RGBCollimator
+    :return: the fresnel phase profile of the collimator model after applying the fresnel phase shift
+    due to propagation to a sensor distance. The fresnel phase profile is calculated using the height
+    map obtained from the phase-to-height map conversion function.
+    """
+    k = 2 * torch.pi / rgb_collim_model.wave_lengths[1]
+    fresnel_phase = - k * ((rgb_collim_model.xx**2 + rgb_collim_model.yy**2)[None][None] / (2 * rgb_collim_model.sensor_distance))
     fresnel_phase = fresnel_phase % (torch.pi * 2)
     height_map = rgb_collim_model.height_map.phase_to_height_map(fresnel_phase, 1)
     fresnel_phase_c = rgb_collim_model.height_map.get_phase_profile(height_map)
-
-    plt.figure()
-    plt.imshow(height_map.squeeze().cpu().numpy())
-    plt.show()
-    
-    from common import plot3d
-    # plot3d(height_map, 'height_map.png')
-    # for i in range(3):
-    #     plt.figure()
-    #     plt.imshow(torch.angle(fresnel_phase_c[0, i]).cpu().numpy())
-    #     # plt.imshow(fresnel_phase[i].cpu().numpy())
-    #     plt.show()
-    
-    # with torch.no_grad():
-    #     # out, psf = rgb_collim_model(x, phase_profile=None)
-    #     out, psf = rgb_collim_model(x, phase_profile=fresnel_phase_c, circular=True)
-    psf = rgb_collim_model.get_psf(fresnel_phase_c)
-        
-    _, axes = plt.subplots(1, 3)    
-    for i in range(3):
-        axes[i].imshow(psf[0, i].cpu().numpy())
-    
-    plt.show()
-    
-    psf = psf[0].cpu().numpy().transpose((1, 2, 0))
-    psf = (psf - psf.min()) / (psf.max() - psf.min())
-    # psf[:,:,0] = (psf[:,:,0]-psf[:,:,0].min()) / (psf[:,:,0].max()-psf[:,:,0].min())
-    # psf[:,:,1] = (psf[:,:,1]-psf[:,:,1].min()) / (psf[:,:,1].max()-psf[:,:,1].min())
-    # psf[:,:,2] = (psf[:,:,2]-psf[:,:,2].min()) / (psf[:,:,2].max()-psf[:,:,2].min())
-    plt.imshow(psf* 255)
-    plt.show()
-    
-    # out = out.cpu().numpy()
-    # plt.imshow(out[0, :, ...].transpose((1, 2, 0)))
-    # plt.show()
-
-# %%
+    return fresnel_phase_c
```

### Comparing `dprox-0.1.3/dprox/utils/examples/optic/unet.py` & `dprox-0.2/dprox/contrib/optic/unet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,57 @@
 import torch.nn as nn
 import torch.utils.data
 import torch
+import torch.nn.functional as F
+
+
+def pad_to_ratio_of_32(tensor):
+    B, C, H, W = tensor.size()
+
+    next_h_multiple_of_32 = (H + 31) // 32 * 32
+    next_w_multiple_of_32 = (W + 31) // 32 * 32
+
+    padding_h = next_h_multiple_of_32 - H
+    padding_w = next_w_multiple_of_32 - W
+
+    padded_tensor = F.pad(tensor, (0, padding_w, 0, padding_h), mode='circular')
+
+    return padded_tensor
+
+
+def unpad_from_ratio_of_32(padded_tensor, original_shape):
+    B, C, H, W = original_shape
+    unpadded_tensor = padded_tensor[:, :, :H, :W]
+    return unpadded_tensor
 
 
 class conv_block(nn.Module):
     def __init__(self, in_ch, out_ch):
         super(conv_block, self).__init__()
-        
+
         self.conv = nn.Sequential(
             nn.Conv2d(in_ch, out_ch, kernel_size=3, stride=1, padding=1, bias=True),
             nn.LeakyReLU(negative_slope=0.01, inplace=True),
             nn.Conv2d(out_ch, out_ch, kernel_size=3, stride=1, padding=1, bias=True),
             nn.LeakyReLU(negative_slope=0.01, inplace=True))
-        
+
         self.conv_residual = nn.Conv2d(in_ch, out_ch, kernel_size=1, stride=1, bias=True)
 
     def forward(self, x):
         x = self.conv(x) + self.conv_residual(x)
         return x
 
 
 class U_Net(nn.Module):
     def __init__(self, in_ch=3, out_ch=3):
         super(U_Net, self).__init__()
 
         n1 = 32
         filters = [n1, n1 * 2, n1 * 4, n1 * 8, n1 * 16]
-        
+
         self.Down1 = nn.Conv2d(filters[0], filters[0], kernel_size=4, stride=2, padding=1, bias=True)
         self.Down2 = nn.Conv2d(filters[1], filters[1], kernel_size=4, stride=2, padding=1, bias=True)
         self.Down3 = nn.Conv2d(filters[2], filters[2], kernel_size=4, stride=2, padding=1, bias=True)
         self.Down4 = nn.Conv2d(filters[3], filters[3], kernel_size=4, stride=2, padding=1, bias=True)
 
         self.Conv1 = conv_block(in_ch, filters[0])
         self.Conv2 = conv_block(filters[0], filters[1])
@@ -49,15 +70,17 @@
 
         self.Up2 = nn.ConvTranspose2d(filters[1], filters[0], kernel_size=2, stride=2, padding=0, bias=True)
         self.Up_conv2 = conv_block(filters[1], filters[0])
 
         self.Conv = nn.Conv2d(filters[0], out_ch, kernel_size=1, stride=1, padding=0)
 
     def forward(self, x):
-
+        shape = x.shape
+        x = pad_to_ratio_of_32(x)
+        
         e1 = self.Conv1(x)
 
         e2 = self.Down1(e1)
         e2 = self.Conv2(e2)
 
         e3 = self.Down2(e2)
         e3 = self.Conv3(e3)
@@ -81,9 +104,12 @@
         d3 = self.Up_conv3(d3)
 
         d2 = self.Up2(d3)
         d2 = torch.cat((e1, d2), dim=1)
         d2 = self.Up_conv2(d2)
 
         out = self.Conv(d2)
+        
+        out = out + x
 
-        return out+x
+        out = unpad_from_ratio_of_32(out, shape)
+        return out
```

### Comparing `dprox-0.1.3/dprox/utils/examples/restoration.py` & `dprox-0.2/dprox/contrib/restoration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import scipy.misc
 import scipy.ndimage
 import numpy as np
 
-from .. import to_torch_tensor, to_ndarray
+from dprox.utils import to_torch_tensor, to_ndarray
 
 samples = {
     'face': scipy.misc.face(),
     'ascent': scipy.misc.ascent(),
 }
```

### Comparing `dprox-0.1.3/dprox/utils/init/mosaic.py` & `dprox-0.2/dprox/utils/init/mosaic.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/utils/init/sr.py` & `dprox-0.2/dprox/utils/init/sr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/dprox/utils/io.py` & `dprox-0.2/dprox/utils/io.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,117 @@
 import os
-import urllib.request
+from typing import List
 
 import imageio
 import numpy as np
-from tqdm import tqdm
+import matplotlib.pyplot as plt
 
-from . import to_ndarray
+from .misc import to_ndarray
 
 
-def imread_rgb(path) -> np.ndarray:
+def imread_rgb(path: str) -> np.ndarray:
     """
-    read an image file from a given path and return it as a NumPy array with RGB color
-    channels.
-    
-    :param path: The path to the image file that needs to be read
-    :return: a NumPy array representing the RGB image read from the
-    specified file path.
+    Read an image file from a given path and return it as a NumPy array with RGB color channels.
+
+    Args:
+      path (str): The path to the image file that needs to be read
+
+    Return:
+      A NumPy array representing the RGB image read from the specified file path.
     """
     import numpy as np
     from PIL import Image
     img = Image.open(path)
     return np.asarray(img)
 
 
-def imshow(*imgs, maxcol=3, gray=False, titles=None, off_axis=False) -> None:
+def imshow(*imgs: List[np.ndarray],
+           maxcol: int = 3,
+           gray: bool = False,
+           titles: List[str] = None,
+           off_axis: bool = True) -> None:
     """
-    display one or more images in a grid with customizable parameters such as
+    Display one or more images in a grid with customizable parameters such as 
     maximum number of columns, grayscale, and titles.
-    
-    :param maxcol: The maximum number of columns to display the images in. If there are more images than
-    maxcol, they will be displayed in multiple rows. The default value is 3, defaults to 3 (optional)
-    :param gray: A boolean parameter that determines whether the image(s) should be displayed in
-    grayscale or in color. If set to True, the images will be displayed in grayscale. If set to False,
-    the images will be displayed in color, defaults to False (optional)
-    :param titles: titles is a list of strings that contains the titles for each image being displayed.
-    If titles is None, then no titles will be displayed
+
+    Args:
+      imgs (List[np.ndarray]): a list of images.
+      maxcol (int): The maximum number of columns to display the images in. If there are more images than
+        maxcol, they will be displayed in multiple rows. The default value is 3, defaults to 3 (optional)
+      gray (bool): A boolean parameter that determines whether the image(s) should be displayed in
+        grayscale or in color. If set to True, the images will be displayed in grayscale. If set to False,
+        the images will be displayed in color, defaults to False (optional)
+      titles (List[str]): titles is a list of strings that contains the titles for each image being displayed. If titles is None, then no titles will be displayed
+      off_axis (bool): whether to remove axis in the images.
     """
-    import matplotlib.pyplot as plt
     if len(imgs) != 1:
-        plt.figure(figsize=(10, 5))
+        plt.figure(figsize=(10, 5), dpi=300)
     row = (len(imgs) - 1) // maxcol + 1
     col = maxcol if len(imgs) >= maxcol else len(imgs)
     for idx, img in enumerate(imgs):
         img = to_ndarray(img, debatch=True)
         if img.max() > 2: img = img / 255
         img = img.clip(0, 1)
-        if gray or len(img.shape) == 2: plt.gray()
+        if gray: plt.gray()
         plt.subplot(row, col, idx + 1)
         plt.imshow(img)
         if titles is not None: plt.title(titles[idx])
         if off_axis: plt.axis('off')
     plt.show()
 
 
-def imread(path) -> np.ndarray:
+def imread(path: str) -> np.ndarray:
     """
     read an image from a given path and return it as a numpy array of float values
     between 0 and 1.
-    
-    :param path: a string representing the file path of an image file to be read
-    :return: a NumPy array of type `float32` representing an image that
-    has been read from the file path specified in the input argument. The pixel values of the image are
-    normalized to the range [0, 1] by dividing each pixel value by 255.
+
+    Args:
+      path (str): a string representing the file path of an image file to be read
+
+    Return: 
+      a NumPy array of type `float32` representing an image that has been read from the file path specified in the input argument. The pixel values of the image are normalized to the range [0, 1] by dividing each pixel value by 255.
     """
-    img = imageio.imread(get_path(path))
+    img = imageio.imread(path)
     return np.float32(img) / 255
 
 
-def filter_ckpt(prefix, ckpt, remove_prefix=True):
+def filter_ckpt(prefix: str, ckpt: dict, remove_prefix: bool = True):
     """
-    filter a checkpoint dictionary by a given prefix and optionally remove the prefix
-    from the keys.
-    
-    :param prefix: The prefix is a string that is used to filter the keys of the checkpoint dictionary.
-    Only the keys that start with this prefix will be included in the new checkpoint dictionary
-    :param ckpt: The ckpt parameter is a dictionary containing the keys and values of a TensorFlow
-    checkpoint file. It typically contains the weights and biases of a trained model
-    :param remove_prefix: remove_prefix is a boolean parameter that determines whether the prefix should
-    be removed from the keys of the returned dictionary. If set to True, the prefix will be removed,
-    otherwise, the keys will remain unchanged, defaults to True (optional)
-    :return: a new dictionary `new_ckpt` that contains the same values as the input dictionary `ckpt`,
-    but with the keys that start with the `prefix` string removed (if `remove_prefix` is True) or
-    unchanged (if `remove_prefix` is False).
+    filter a checkpoint dictionary by a given prefix and optionally remove the prefix from the keys.
+
+    Args:
+      prefix (str): The prefix is a string that is used to filter the keys of the checkpoint dictionary. 
+        Only the keys that start with this prefix will be included in the new checkpoint dictionary
+      ckpt (dict): The ckpt parameter is a dictionary containing the keys and values of a TensorFlow
+        checkpoint file. It typically contains the weights and biases of a trained model
+      remove_prefix (bool): remove_prefix is a boolean parameter that determines whether the prefix should
+        be removed from the keys of the returned dictionary. If set to True, the prefix will be removed,
+        otherwise, the keys will remain unchanged, defaults to True (optional)
+
+    Return: 
+      a new dictionary `new_ckpt` that contains the same values as the input dictionary `ckpt`,
+      but with the keys that start with the `prefix` string removed (if `remove_prefix` is True) or
+      unchanged (if `remove_prefix` is False).
     """
     new_ckpt = {}
     for k, v in ckpt.items():
         if k.startswith(prefix):
             if remove_prefix: new_k = k.replace(prefix, '')
             else: new_k = k
             new_ckpt[new_k] = v
     return new_ckpt
 
 
-# The DownloadProgressBar class is a subclass of the tqdm class in Python used to display progress
-# bars for downloading files.
-class DownloadProgressBar(tqdm):
-    def update_to(self, b=1, bsize=1, tsize=None):
-        if tsize is not None:
-            self.total = tsize
-        self.update(b * bsize - self.n)
-
-
-def get_path(base_path) -> str:
-    """
-    check if a file exists in a specific directory and download it from a URL if it
-    doesn't exist.
-    
-    :param base_path: The base path is a string that represents the path to a file or directory that the
-    function is trying to locate or download. It is used to construct the full path to the file or
-    directory by appending it to the DPROX_DIR path
-    :return: a string which is the path to the file specified by the input parameter `base_path`.
-    """
-    DPROX_DIR = os.path.join(os.path.expanduser('~'), '.cache/dprox')
-
-    save_path = os.path.join(DPROX_DIR, base_path)
-    if not os.path.exists(save_path):
-        url = f"https://huggingface.co/aaronb/DeltaProx/resolve/main/{base_path}"
-        print(f'{base_path} not found')
-        print('Try to download from huggingface: ', url)
-        os.makedirs(os.path.dirname(save_path), exist_ok=True)
-        download_url(url, save_path)
-        print('Downloaded to ', save_path)
-    return save_path
-
-
-def download_url(url, output_path) -> None:
-    """
-    download a file from a given URL and save it to a specified output path while
-    displaying a progress bar.
-    
-    :param url: The URL of the file to be downloaded
-    :param output_path: output_path is a string representing the file path where the downloaded file
-    will be saved. It should include the file name and extension
-    """
-    with DownloadProgressBar(unit='B', unit_scale=True,
-                             miniters=1, desc=url.split('/')[-1]) as t:
-        urllib.request.urlretrieve(url, filename=output_path, reporthook=t.update_to)
+def is_image_file(filename):
+    # List of common image file extensions
+    image_extensions = ['.jpg', '.jpeg', '.png', '.gif', '.bmp', '.tiff', '.webp']
+    # Check if the file extension is in the image extensions list (case insensitive)
+    return any(filename.lower().endswith(ext) for ext in image_extensions)
+
+
+def list_image_files(directory):
+    image_files = []
+    for filename in os.listdir(directory):
+        filepath = os.path.join(directory, filename)
+        if os.path.isfile(filepath) and is_image_file(filename):
+            image_files.append(filename)
+    return image_files
```

### Comparing `dprox-0.1.3/dprox/utils/metrics.py` & `dprox-0.2/dprox/utils/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # helper
 
 
 def autoconvert(func):
     """
     a decorator that automatically converts the input arguments `output`
     and `target` to numpy arrays before passing them to the decorated function.
-    
+
     :param func: The function that will be decorated with the `autoconvert` functionality
     :return: a decorated version of the input function `func`. The `wrapped` function takes 
     in two arguments `output` and `target`, and any additional arguments and keyword arguments 
     that `func` may take. It first converts `output` and `target` to numpy arrays using 
     the `to_ndarray` function with the `debatch=True` argument
     """
     @functools.wraps(func)
@@ -39,15 +39,15 @@
 
 
 def bandwise(func):
     """
     take a function as input and return a wrapped version of that function
     that applies the input function to each color band of the input arrays and returns the average of
     the results.
-    
+
     :param func: A function that takes in two arrays (output and target) and any additional arguments,
     and returns a scalar value representing the loss or metric value
     :return: The function `wrapped` is being returned, which takes in `output`, `target`, `*args`, and
     `**kwargs` as arguments and applies the `func` function to each channel of the `output` and `target`
     arrays. The final output is the average of the results obtained from applying `func` to each
     channel. The `@functools.wraps(func)` decorator
     """
@@ -89,15 +89,15 @@
 
 
 @autoconvert
 def ergas(output, target, r=1):
     """
     calculate the ERGAS (Error Relative Global Average Squared) metric between the output
     and target images.
-    
+
     :param output: This is a numpy array representing the output image generated by a remote sensing
     algorithm
     :param target: The target parameter is a numpy array representing the true or desired output of a
     model or system. It has a shape of (height, width, bands), where height and width represent the
     dimensions of the image and bands represent the number of spectral bands in the image
     :param r: The parameter "r" is a scaling factor used to adjust the magnitude of the ERGAS value. It
     is set to 1 by default, defaults to 1 (optional)
```

### Comparing `dprox-0.1.3/dprox/utils/psf2otf.py` & `dprox-0.2/dprox/utils/psf2otf.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.3/setup.py` & `dprox-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from setuptools import setup, find_packages
 
-
 deps = [
     'imageio',
     'scikit_image',
     'matplotlib',
     'munch',
     'tfpnp',
     'cvxpy',
     'torchlights',
     'tensorboardX',
     'termcolor',
     'proximal',
     'opencv-python'
 ]
 
-
 setup(
     name='dprox',
     description='A domain-specific language and compiler that transforms optimization problems into differentiable proximal solvers.',
     url='https://github.com/princeton-computational-imaging/Delta-Prox',
     author='Zeqiang Lai',
     author_email='laizeqiang@outlook.com',
     packages=find_packages(),
-    version='0.1.3',
+    version='0.2',
     include_package_data=True,
     install_requires=deps,
 )
```

### Comparing `dprox-0.1.3/tests/test_algorithms.py` & `dprox-0.2/tests/test_algorithms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,104 @@
 from dprox import *
 from dprox.utils import *
-from dprox.utils import examples
+from dprox import contrib
 
 
 def test_admm():
-    img = examples.sample('face')
-    psf = examples.point_spread_function(15, 5)
-    b = examples.blurring(img, psf)
+    img = contrib.sample('face')
+    psf = contrib.point_spread_function(15, 5)
+    b = contrib.blurring(img, psf)
 
     x = Variable()
     data_term = sum_squares(conv(x, psf) - b)
     reg_term = deep_prior(x, denoiser='ffdnet_color')
     reg2 = nonneg(x)
     prob = Problem(data_term + reg_term + reg2)
 
     out = prob.solve(method='admm', x0=b, pbar=True)
 
     print(psnr(out, img))
-    assert abs(psnr(out, img) - 31.9) < 0.1
+    assert abs(psnr(out, img) - 34.51) < 0.1
 
 
 def test_ladmm():
-    img = examples.sample('face')
-    psf = examples.point_spread_function(15, 5)
-    b = examples.blurring(img, psf)
+    img = contrib.sample('face')
+    psf = contrib.point_spread_function(15, 5)
+    b = contrib.blurring(img, psf)
 
     x = Variable()
     data_term = sum_squares(conv(x, psf) - b)
     reg_term = deep_prior(x, denoiser='ffdnet_color')
     reg2 = nonneg(x)
     prob = Problem(data_term + reg_term + reg2)
 
     out = prob.solve(method='ladmm', x0=b, pbar=True)
 
     print(psnr(out, img))
-    assert abs(psnr(out, img) - 31.9) < 0.1
+    assert abs(psnr(out, img) - 34.51) < 0.1
 
 
 def test_admm_vxu():
-    img = examples.sample('face')
-    psf = examples.point_spread_function(15, 5)
-    b = examples.blurring(img, psf)
+    img = contrib.sample('face')
+    psf = contrib.point_spread_function(15, 5)
+    b = contrib.blurring(img, psf)
 
     x = Variable()
     data_term = sum_squares(conv(x, psf) - b)
     reg_term = deep_prior(x, denoiser='ffdnet_color')
     reg2 = nonneg(x)
     prob = Problem(data_term + reg_term + reg2)
 
     out = prob.solve(method='admm_vxu', x0=b, pbar=True)
 
     print(psnr(out, img))
-    assert abs(psnr(out, img) - 31.9) < 0.1
+    assert abs(psnr(out, img) - 34.50) < 0.1
 
 
 def test_hqs():
-    img = examples.sample('face')
-    psf = examples.point_spread_function(15, 5)
-    b = examples.blurring(img, psf)
+    img = contrib.sample('face')
+    psf = contrib.point_spread_function(15, 5)
+    b = contrib.blurring(img, psf)
 
     x = Variable()
     data_term = sum_squares(conv(x, psf) - b)
     reg_term = deep_prior(x, denoiser='ffdnet_color')
     reg2 = nonneg(x)
     prob = Problem(data_term + reg_term + reg2)
 
     out = prob.solve(method='hqs', x0=b, pbar=True)
 
     print(psnr(out, img))
-    assert abs(psnr(out, img) - 31.6) < 0.1
+    assert abs(psnr(out, img) - 34.08) < 0.1
 
 
 def test_pc():
-    img = examples.sample('face')
-    psf = examples.point_spread_function(15, 5)
-    b = examples.blurring(img, psf)
+    img = contrib.sample('face')
+    psf = contrib.point_spread_function(15, 5)
+    b = contrib.blurring(img, psf)
 
     x = Variable()
     data_term = sum_squares(conv(x, psf) - b)
     reg_term = deep_prior(x, denoiser='ffdnet_color')
     reg2 = nonneg(x)
     prob = Problem(data_term + reg_term + reg2)
 
     out = prob.solve(method='pc', x0=b, pbar=True)
 
     print(psnr(out, img))
-    assert abs(psnr(out, img) - 29.6) < 0.1
+    assert abs(psnr(out, img) - 29.87) < 0.1
 
 
 def test_pgd():
-    img = examples.sample('face')
-    psf = examples.point_spread_function(15, 5)
-    b = examples.blurring(img, psf)
+    img = contrib.sample('face')
+    psf = contrib.point_spread_function(15, 5)
+    b = contrib.blurring(img, psf)
 
     x = Variable()
     data_term = sum_squares(conv(x, psf) - b)
     reg_term = deep_prior(x, denoiser='ffdnet_color')
     prob = Problem(data_term + reg_term)
 
     out = prob.solve(method='pgd', x0=b, pbar=True)
 
     print(psnr(out, img))
+    assert abs(psnr(out, img) - 21.44) < 0.1
```

### Comparing `dprox-0.1.3/tests/test_linop.py` & `dprox-0.2/tests/test_linop.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import dprox as dp
 
-from dprox.utils.examples import fspecial_gaussian
+from dprox.contrib import fspecial_gaussian
 from dprox.utils import to_torch_tensor
 
 from scipy.misc import face
 
 
 def test_conv():
     x = dp.Variable()
@@ -100,19 +100,19 @@
     outputs = K.forward(img)
     inputs = K.adjoint(outputs)
     print(inputs.shape)
     K.sanity_check()
 
 
 def test_complex():
-    from dprox.utils import examples
+    from dprox import contrib
 
-    img = examples.sample('face')
-    psf = examples.point_spread_function(15, 5)
-    b = examples.blurring(img, psf)
+    img = contrib.sample('face')
+    psf = contrib.point_spread_function(15, 5)
+    b = contrib.blurring(img, psf)
 
     x = dp.Variable()
     data_term = dp.sum_squares(dp.conv(x, psf) - b)
     reg_term = dp.deep_prior(x, denoiser='ffdnet_color')
     reg2 = dp.nonneg(x)
     K = dp.CompGraph(dp.vstack([fn.linop for fn in [data_term, reg_term, reg2]]))
     K.forward(b)
```

