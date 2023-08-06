# Comparing `tmp/audioldm2-0.0.7.tar.gz` & `tmp/audioldm2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm2-0.0.7.tar", last modified: Sat Aug  5 16:22:48 2023, max compression
+gzip compressed data, was "audioldm2-0.0.8.tar", last modified: Sat Aug  5 16:44:19 2023, max compression
```

## Comparing `audioldm2-0.0.7.tar` & `audioldm2-0.0.8.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.647388 audioldm2-0.0.7/
--rw-r--r--   0 root         (0) root         (0)    20845 2023-08-05 14:48:09.000000 audioldm2-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       87 2023-08-05 14:48:09.000000 audioldm2-0.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5011 2023-08-05 16:22:48.644195 audioldm2-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4354 2023-08-05 16:03:02.000000 audioldm2-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)    13995 2023-08-05 14:49:05.000000 audioldm2-0.0.7/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.032657 audioldm2-0.0.7/audioldm2/
--rwxr-xr-x   0 root         (0) root         (0)      105 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.077152 audioldm2-0.0.7/audioldm2/audiomae_gen/
--rwxr-xr-x   0 root         (0) root         (0)       46 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/audiomae_gen/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    16876 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/audiomae_gen/sequence_input.py
--rw-r--r--   0 root         (0) root         (0)      730 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/audiomae_gen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.082058 audioldm2-0.0.7/audioldm2/clap/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.194959 audioldm2-0.0.7/audioldm2/clap/open_clip/
--rwxr-xr-x   0 root         (0) root         (0)      639 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)  1356917 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 root         (0) root         (0)    10985 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/factory.py
--rwxr-xr-x   0 root         (0) root         (0)     7177 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/feature_fusion.py
--rwxr-xr-x   0 root         (0) root         (0)    48069 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/htsat.py
--rwxr-xr-x   0 root         (0) root         (0)    16096 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/loss.py
--rwxr-xr-x   0 root         (0) root         (0)    32924 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.328551 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/
--rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
--rwxr-xr-x   0 root         (0) root         (0)      498 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
--rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
--rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-10.json
--rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
--rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14.json
--rwxr-xr-x   0 root         (0) root         (0)      495 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-6.json
--rwxr-xr-x   0 root         (0) root         (0)      388 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
--rwxr-xr-x   0 root         (0) root         (0)      364 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN101.json
--rwxr-xr-x   0 root         (0) root         (0)      389 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
--rwxr-xr-x   0 root         (0) root         (0)      364 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN50.json
--rwxr-xr-x   0 root         (0) root         (0)      365 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN50x16.json
--rwxr-xr-x   0 root         (0) root         (0)      365 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN50x4.json
--rwxr-xr-x   0 root         (0) root         (0)      294 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
--rwxr-xr-x   0 root         (0) root         (0)      318 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rwxr-xr-x   0 root         (0) root         (0)      294 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
--rwxr-xr-x   0 root         (0) root         (0)      296 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
--rwxr-xr-x   0 root         (0) root         (0)     5023 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/openai.py
--rwxr-xr-x   0 root         (0) root         (0)    23369 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/pann_model.py
--rwxr-xr-x   0 root         (0) root         (0)     6440 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/pretrained.py
--rwxr-xr-x   0 root         (0) root         (0)     4332 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/timm_model.py
--rwxr-xr-x   0 root         (0) root         (0)     6400 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)     1051 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/transform.py
--rwxr-xr-x   0 root         (0) root         (0)    11963 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.361736 audioldm2-0.0.7/audioldm2/clap/training/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    84448 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/audioset_textmap.npy
--rw-r--r--   0 root         (0) root         (0)  1356917 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 root         (0) root         (0)    29672 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/data.py
--rwxr-xr-x   0 root         (0) root         (0)    17202 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.379886 audioldm2-0.0.7/audioldm2/hifigan/
--rwxr-xr-x   0 root         (0) root         (0)      230 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/hifigan/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5524 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/hifigan/models.py
--rwxr-xr-x   0 root         (0) root         (0)    12819 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/hifigan/models_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.390679 audioldm2-0.0.7/audioldm2/latent_diffusion/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.411725 audioldm2-0.0.7/audioldm2/latent_diffusion/models/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/models/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    17259 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/models/ddim.py
--rwxr-xr-x   0 root         (0) root         (0)    65617 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/models/ddpm.py
--rwxr-xr-x   0 root         (0) root         (0)    12849 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/models/plms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.427396 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    15753 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/attention.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.448757 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/
--rwxr-xr-x   0 root         (0) root         (0)     5381 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    21105 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
--rwxr-xr-x   0 root         (0) root         (0)     7684 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.498199 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/
--rwxr-xr-x   0 root         (0) root         (0)     1363 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
--rwxr-xr-x   0 root         (0) root         (0)     1924 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
--rwxr-xr-x   0 root         (0) root         (0)     2026 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
--rwxr-xr-x   0 root         (0) root         (0)     2445 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
--rwxr-xr-x   0 root         (0) root         (0)      885 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
--rwxr-xr-x   0 root         (0) root         (0)    14517 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
--rwxr-xr-x   0 root         (0) root         (0)     4381 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
--rwxr-xr-x   0 root         (0) root         (0)     8632 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
--rwxr-xr-x   0 root         (0) root         (0)     2259 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.520019 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    34452 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
--rwxr-xr-x   0 root         (0) root         (0)    40223 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
--rwxr-xr-x   0 root         (0) root         (0)     9870 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.530202 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/distributions/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/distributions/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3097 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/distributions/distributions.py
--rwxr-xr-x   0 root         (0) root         (0)     3066 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/ema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.540312 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/encoders/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/encoders/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    27449 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/encoders/modules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.561139 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14860 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
--rwxr-xr-x   0 root         (0) root         (0)     4960 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
--rwxr-xr-x   0 root         (0) root         (0)     1590 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
--rwxr-xr-x   0 root         (0) root         (0)     6022 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.570904 audioldm2-0.0.7/audioldm2/latent_encoder/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_encoder/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    11286 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_encoder/autoencoder.py
--rwxr-xr-x   0 root         (0) root         (0)     5657 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.592930 audioldm2-0.0.7/audioldm2/utilities/
--rwxr-xr-x   0 root         (0) root         (0)       62 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.614077 audioldm2-0.0.7/audioldm2/utilities/audio/
--rwxr-xr-x   0 root         (0) root         (0)       73 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/audio/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2642 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/audio/audio_processing.py
--rwxr-xr-x   0 root         (0) root         (0)     6312 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/audio/stft.py
--rwxr-xr-x   0 root         (0) root         (0)     2528 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/audio/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.629353 audioldm2-0.0.7/audioldm2/utilities/data/
--rwxr-xr-x   0 root         (0) root         (0)       29 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/data/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    15063 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/data/add_on.py
--rwxr-xr-x   0 root         (0) root         (0)    20175 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/data/dataset.py
--rwxr-xr-x   0 root         (0) root         (0)     3589 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/model.py
--rwxr-xr-x   0 root         (0) root         (0)    19538 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/sampler.py
--rwxr-xr-x   0 root         (0) root         (0)    18077 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/tools.py
--rwxr-xr-x   0 root         (0) root         (0)    12389 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.060819 audioldm2-0.0.7/audioldm2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5011 2023-08-05 16:22:46.000000 audioldm2-0.0.7/audioldm2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4806 2023-08-05 16:22:47.000000 audioldm2-0.0.7/audioldm2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 16:22:46.000000 audioldm2-0.0.7/audioldm2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      218 2023-08-05 16:22:46.000000 audioldm2-0.0.7/audioldm2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-08-05 16:22:46.000000 audioldm2-0.0.7/audioldm2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.640820 audioldm2-0.0.7/bin/
--rwxr-xr-x   0 root         (0) root         (0)     3007 2023-08-05 16:22:02.000000 audioldm2-0.0.7/bin/audioldm2
--rwxr-xr-x   0 root         (0) root         (0)       32 2023-08-05 14:48:09.000000 audioldm2-0.0.7/bin/audioldm2.cmd
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 16:22:48.646195 audioldm2-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4445 2023-08-05 16:22:46.000000 audioldm2-0.0.7/setup.py
--rw-r--r--   0 root         (0) root         (0)     6448 2023-08-05 14:48:09.000000 audioldm2-0.0.7/share_btn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.157977 audioldm2-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)    20845 2023-08-05 14:48:09.000000 audioldm2-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       87 2023-08-05 14:48:09.000000 audioldm2-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-08-05 16:44:19.154777 audioldm2-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-08-05 16:03:02.000000 audioldm2-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)    13995 2023-08-05 14:49:05.000000 audioldm2-0.0.8/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.533460 audioldm2-0.0.8/audioldm2/
+-rwxr-xr-x   0 root         (0) root         (0)      105 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.589854 audioldm2-0.0.8/audioldm2/audiomae_gen/
+-rwxr-xr-x   0 root         (0) root         (0)       46 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/audiomae_gen/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16876 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/audiomae_gen/sequence_input.py
+-rw-r--r--   0 root         (0) root         (0)      730 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/audiomae_gen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.595030 audioldm2-0.0.8/audioldm2/clap/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.715474 audioldm2-0.0.8/audioldm2/clap/open_clip/
+-rwxr-xr-x   0 root         (0) root         (0)      639 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)  1356917 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 root         (0) root         (0)    10985 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/factory.py
+-rwxr-xr-x   0 root         (0) root         (0)     7177 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/feature_fusion.py
+-rwxr-xr-x   0 root         (0) root         (0)    48069 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/htsat.py
+-rwxr-xr-x   0 root         (0) root         (0)    16096 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)    32924 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.826059 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
+-rwxr-xr-x   0 root         (0) root         (0)      498 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/PANN-10.json
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/PANN-14.json
+-rwxr-xr-x   0 root         (0) root         (0)      495 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/PANN-6.json
+-rwxr-xr-x   0 root         (0) root         (0)      388 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
+-rwxr-xr-x   0 root         (0) root         (0)      364 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/RN101.json
+-rwxr-xr-x   0 root         (0) root         (0)      389 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
+-rwxr-xr-x   0 root         (0) root         (0)      364 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/RN50.json
+-rwxr-xr-x   0 root         (0) root         (0)      365 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/RN50x16.json
+-rwxr-xr-x   0 root         (0) root         (0)      365 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/RN50x4.json
+-rwxr-xr-x   0 root         (0) root         (0)      294 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
+-rwxr-xr-x   0 root         (0) root         (0)      318 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rwxr-xr-x   0 root         (0) root         (0)      294 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
+-rwxr-xr-x   0 root         (0) root         (0)      296 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
+-rwxr-xr-x   0 root         (0) root         (0)     5023 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/openai.py
+-rwxr-xr-x   0 root         (0) root         (0)    23369 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/pann_model.py
+-rwxr-xr-x   0 root         (0) root         (0)     6440 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/pretrained.py
+-rwxr-xr-x   0 root         (0) root         (0)     4332 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/timm_model.py
+-rwxr-xr-x   0 root         (0) root         (0)     6400 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/tokenizer.py
+-rwxr-xr-x   0 root         (0) root         (0)     1051 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/transform.py
+-rwxr-xr-x   0 root         (0) root         (0)    11963 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/open_clip/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.855062 audioldm2-0.0.8/audioldm2/clap/training/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/training/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    84448 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/training/audioset_textmap.npy
+-rw-r--r--   0 root         (0) root         (0)  1356917 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 root         (0) root         (0)    29672 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/training/data.py
+-rwxr-xr-x   0 root         (0) root         (0)    17202 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/clap/training/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.870529 audioldm2-0.0.8/audioldm2/hifigan/
+-rwxr-xr-x   0 root         (0) root         (0)      230 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/hifigan/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5524 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/hifigan/models.py
+-rwxr-xr-x   0 root         (0) root         (0)    12819 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/hifigan/models_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.880130 audioldm2-0.0.8/audioldm2/latent_diffusion/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.900584 audioldm2-0.0.8/audioldm2/latent_diffusion/models/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    17259 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/models/ddim.py
+-rwxr-xr-x   0 root         (0) root         (0)    65617 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/models/ddpm.py
+-rwxr-xr-x   0 root         (0) root         (0)    12849 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/models/plms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.923446 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    15753 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/attention.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.942444 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/
+-rwxr-xr-x   0 root         (0) root         (0)     5381 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21105 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
+-rwxr-xr-x   0 root         (0) root         (0)     7684 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.989373 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/
+-rwxr-xr-x   0 root         (0) root         (0)     1363 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
+-rwxr-xr-x   0 root         (0) root         (0)     1924 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
+-rwxr-xr-x   0 root         (0) root         (0)     2026 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
+-rwxr-xr-x   0 root         (0) root         (0)     2445 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
+-rwxr-xr-x   0 root         (0) root         (0)      885 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
+-rwxr-xr-x   0 root         (0) root         (0)    14517 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
+-rwxr-xr-x   0 root         (0) root         (0)     4381 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
+-rwxr-xr-x   0 root         (0) root         (0)     8632 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
+-rwxr-xr-x   0 root         (0) root         (0)     2259 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.009070 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/diffusionmodules/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    34452 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
+-rwxr-xr-x   0 root         (0) root         (0)    40223 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
+-rwxr-xr-x   0 root         (0) root         (0)     9870 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.018574 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/distributions/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/distributions/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3097 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/distributions/distributions.py
+-rwxr-xr-x   0 root         (0) root         (0)     3066 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/ema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.028451 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/encoders/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/encoders/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    27449 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/encoders/modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.048014 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/phoneme_encoder/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14860 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
+-rwxr-xr-x   0 root         (0) root         (0)     4960 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
+-rwxr-xr-x   0 root         (0) root         (0)     1590 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
+-rwxr-xr-x   0 root         (0) root         (0)     6022 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_diffusion/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.057548 audioldm2-0.0.8/audioldm2/latent_encoder/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_encoder/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    11286 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/latent_encoder/autoencoder.py
+-rwxr-xr-x   0 root         (0) root         (0)     5657 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.102159 audioldm2-0.0.8/audioldm2/utilities/
+-rwxr-xr-x   0 root         (0) root         (0)       62 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.123985 audioldm2-0.0.8/audioldm2/utilities/audio/
+-rwxr-xr-x   0 root         (0) root         (0)       73 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/audio/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2642 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/audio/audio_processing.py
+-rwxr-xr-x   0 root         (0) root         (0)     6312 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/audio/stft.py
+-rwxr-xr-x   0 root         (0) root         (0)     2528 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/audio/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.139869 audioldm2-0.0.8/audioldm2/utilities/data/
+-rwxr-xr-x   0 root         (0) root         (0)       29 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/data/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    15063 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/data/add_on.py
+-rwxr-xr-x   0 root         (0) root         (0)    20175 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/data/dataset.py
+-rwxr-xr-x   0 root         (0) root         (0)     3589 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/model.py
+-rwxr-xr-x   0 root         (0) root         (0)    19538 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/sampler.py
+-rwxr-xr-x   0 root         (0) root         (0)    18077 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utilities/tools.py
+-rwxr-xr-x   0 root         (0) root         (0)    12389 2023-08-05 14:48:09.000000 audioldm2-0.0.8/audioldm2/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:18.560412 audioldm2-0.0.8/audioldm2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-08-05 16:44:17.000000 audioldm2-0.0.8/audioldm2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-08-05 16:44:18.000000 audioldm2-0.0.8/audioldm2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 16:44:17.000000 audioldm2-0.0.8/audioldm2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      218 2023-08-05 16:44:17.000000 audioldm2-0.0.8/audioldm2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-05 16:44:17.000000 audioldm2-0.0.8/audioldm2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:44:19.151226 audioldm2-0.0.8/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     3007 2023-08-05 16:43:48.000000 audioldm2-0.0.8/bin/audioldm2
+-rwxr-xr-x   0 root         (0) root         (0)       32 2023-08-05 14:48:09.000000 audioldm2-0.0.8/bin/audioldm2.cmd
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 16:44:19.157777 audioldm2-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-08-05 16:43:39.000000 audioldm2-0.0.8/setup.py
+-rw-r--r--   0 root         (0) root         (0)     6448 2023-08-05 14:48:09.000000 audioldm2-0.0.8/share_btn.py
```

### Comparing `audioldm2-0.0.7/LICENSE` & `audioldm2-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/PKG-INFO` & `audioldm2-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioldm2
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/haoheliu/audioldm2
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audioldm2-0.0.7/README.md` & `audioldm2-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/app.py` & `audioldm2-0.0.8/app.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/audiomae_gen/sequence_input.py` & `audioldm2-0.0.8/audioldm2/audiomae_gen/sequence_input.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/audiomae_gen/utils.py` & `audioldm2-0.0.8/audioldm2/audiomae_gen/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/__init__.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.8/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/factory.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/feature_fusion.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/htsat.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/loss.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/model.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/openai.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/pann_model.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/pretrained.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/timm_model.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/tokenizer.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/transform.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/open_clip/utils.py` & `audioldm2-0.0.8/audioldm2/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/training/audioset_textmap.npy` & `audioldm2-0.0.8/audioldm2/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.8/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/training/data.py` & `audioldm2-0.0.8/audioldm2/clap/training/data.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/clap/training/params.py` & `audioldm2-0.0.8/audioldm2/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/hifigan/models.py` & `audioldm2-0.0.8/audioldm2/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/hifigan/models_v2.py` & `audioldm2-0.0.8/audioldm2/hifigan/models_v2.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/models/ddim.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/models/ddim.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/models/ddpm.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/models/ddpm.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/models/plms.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/models/plms.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/attention.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/attention.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/models_mae.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/models_mae.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/models_vit.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/models_vit.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/crop.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/crop.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lars.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/lars.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/misc.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/misc.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/stat.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/audiomae/util/stat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/model.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/util.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/distributions/distributions.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/ema.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/ema.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/encoders/modules.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_diffusion/util.py` & `audioldm2-0.0.8/audioldm2/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/latent_encoder/autoencoder.py` & `audioldm2-0.0.8/audioldm2/latent_encoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/pipeline.py` & `audioldm2-0.0.8/audioldm2/pipeline.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utilities/audio/audio_processing.py` & `audioldm2-0.0.8/audioldm2/utilities/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utilities/audio/stft.py` & `audioldm2-0.0.8/audioldm2/utilities/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utilities/audio/tools.py` & `audioldm2-0.0.8/audioldm2/utilities/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utilities/data/add_on.py` & `audioldm2-0.0.8/audioldm2/utilities/data/add_on.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utilities/data/dataset.py` & `audioldm2-0.0.8/audioldm2/utilities/data/dataset.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utilities/model.py` & `audioldm2-0.0.8/audioldm2/utilities/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utilities/sampler.py` & `audioldm2-0.0.8/audioldm2/utilities/sampler.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utilities/tools.py` & `audioldm2-0.0.8/audioldm2/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2/utils.py` & `audioldm2-0.0.8/audioldm2/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/audioldm2.egg-info/PKG-INFO` & `audioldm2-0.0.8/audioldm2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioldm2
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/haoheliu/audioldm2
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audioldm2-0.0.7/audioldm2.egg-info/SOURCES.txt` & `audioldm2-0.0.8/audioldm2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.7/bin/audioldm2` & `audioldm2-0.0.8/bin/audioldm2`

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,8 @@
         duration=duration,
         guidance_scale=guidance_scale,
         ddim_steps=args.ddim_steps,
         n_candidate_gen_per_text=n_candidate_gen_per_text,
         batchsize=args.batchsize,
     )
      
-    save_wave(waveform, save_path, name=text[:256])
+    save_wave(waveform, save_path, name=text[:128])
```

### Comparing `audioldm2-0.0.7/setup.py` & `audioldm2-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audioldm2"
 DESCRIPTION = "This package is written for text-to-audio/music generation."
 URL = "https://github.com/haoheliu/audioldm2"
 EMAIL = "haoheliu@gmail.com"
 AUTHOR = "Haohe Liu"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

### Comparing `audioldm2-0.0.7/share_btn.py` & `audioldm2-0.0.8/share_btn.py`

 * *Files identical despite different names*

