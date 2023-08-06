# Comparing `tmp/streamflow-0.2.0.dev6.tar.gz` & `tmp/streamflow-0.2.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamflow-0.2.0.dev6.tar", last modified: Thu Jun 15 00:43:44 2023, max compression
+gzip compressed data, was "streamflow-0.2.0.dev7.tar", last modified: Sun Aug  6 12:02:31 2023, max compression
```

## Comparing `streamflow-0.2.0.dev6.tar` & `streamflow-0.2.0.dev7.tar`

### file list

```diff
@@ -1,180 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/bandit-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.554962 streamflow-0.2.0.dev6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/report-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.554962 streamflow-0.2.0.dev6/streamflow/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.558962 streamflow-0.2.0.dev6/streamflow/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.550962 streamflow-0.2.0.dev6/streamflow/config/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.558962 streamflow-0.2.0.dev6/streamflow/config/schemas/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/config/schemas/v1.0/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/config/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.558962 streamflow-0.2.0.dev6/streamflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/asyncache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/antlr/
--rw-r--r--   0 runner    (1001) docker     (123)    52296 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33065 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   228650 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    49556 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/requirement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/kubernetes.json
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)   113743 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)    40610 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/data/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/data/remotepath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/data/schemas/data_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/aiotarstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    52606 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    43726 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/occam.py
--rw-r--r--   0 runner    (1001) docker     (123)    43252 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/docker-compose.json
--rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/flux.json
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/helm3.json
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/kubernetes.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/local.json
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/occam.json
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/pbs.json
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/queue_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (123)    21318 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/slurm.json
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/ssh.json
--rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/deployment_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/filter/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/filter/schemas/shuffle.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/filter/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/future.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/schemas/deployment_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/ext/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/loading_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/persistence/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/schemas/sqlite.json
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/schemas/sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64182 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/provenance/run_crate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/recovery/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/checkpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/failure_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/recovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/recovery/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/schemas/default_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/schemas/default_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/schemas/dummy_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/schemas/dummy_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/scheduling/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/policy/data_locality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/scheduling/policy/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/policy/schemas/data_locality.json
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/scheduling/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/schemas/scheduler.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/streamflow/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    66334 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.558962 streamflow-0.2.0.dev6/streamflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_cwl_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_cwl_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_cwl_provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    20695 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_remotepath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.775186 streamflow-0.2.0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-08-06 12:02:31.775186 streamflow-0.2.0.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/bandit-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.751186 streamflow-0.2.0.dev7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/report-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:02:31.775186 streamflow-0.2.0.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.751186 streamflow-0.2.0.dev7/streamflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.751186 streamflow-0.2.0.dev7/streamflow/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.747186 streamflow-0.2.0.dev7/streamflow/config/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.751186 streamflow-0.2.0.dev7/streamflow/config/schemas/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/config/schemas/v1.0/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/config/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.755186 streamflow-0.2.0.dev7/streamflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/asyncache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.759186 streamflow-0.2.0.dev7/streamflow/cwl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.759186 streamflow-0.2.0.dev7/streamflow/cwl/antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)    52296 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/antlr/ECMAScriptLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33065 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/antlr/ECMAScriptListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   228650 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/antlr/ECMAScriptParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/antlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53062 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49556 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.759186 streamflow-0.2.0.dev7/streamflow/cwl/requirement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.759186 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.759186 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113838 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40610 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/cwl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.759186 streamflow-0.2.0.dev7/streamflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/data/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/data/remotepath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.759186 streamflow-0.2.0.dev7/streamflow/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/data/schemas/data_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.763186 streamflow-0.2.0.dev7/streamflow/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/aiotarstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.763186 streamflow-0.2.0.dev7/streamflow/deployment/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52606 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43726 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/occam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43741 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/docker-compose.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/flux.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/helm3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/local.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/occam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/pbs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/queue_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21274 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/slurm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/ssh.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/connector/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/deployment_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/deployment/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/deployment/filter/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/filter/schemas/shuffle.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/filter/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/future.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/deployment/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/schemas/deployment_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/deployment/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/ext/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/persistence/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/persistence/loading_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/persistence/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/persistence/schemas/sqlite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/persistence/schemas/sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/persistence/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64181 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/provenance/run_crate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.767186 streamflow-0.2.0.dev7/streamflow/recovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/recovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/recovery/checkpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/recovery/failure_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/recovery/recovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.771186 streamflow-0.2.0.dev7/streamflow/recovery/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/recovery/schemas/default_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/recovery/schemas/default_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/recovery/schemas/dummy_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/recovery/schemas/dummy_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.771186 streamflow-0.2.0.dev7/streamflow/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.771186 streamflow-0.2.0.dev7/streamflow/scheduling/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/scheduling/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/scheduling/policy/data_locality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.771186 streamflow-0.2.0.dev7/streamflow/scheduling/policy/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/scheduling/policy/schemas/data_locality.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/scheduling/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.771186 streamflow-0.2.0.dev7/streamflow/scheduling/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/scheduling/schemas/scheduler.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.771186 streamflow-0.2.0.dev7/streamflow/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/workflow/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/workflow/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66334 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/workflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/workflow/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/workflow/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/streamflow/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.751186 streamflow-0.2.0.dev7/streamflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-08-06 12:02:31.000000 streamflow-0.2.0.dev7/streamflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-08-06 12:02:31.000000 streamflow-0.2.0.dev7/streamflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:02:31.000000 streamflow-0.2.0.dev7/streamflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-06 12:02:31.000000 streamflow-0.2.0.dev7/streamflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-06 12:02:31.000000 streamflow-0.2.0.dev7/streamflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 12:02:31.000000 streamflow-0.2.0.dev7/streamflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:02:31.000000 streamflow-0.2.0.dev7/streamflow.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:02:31.775186 streamflow-0.2.0.dev7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_cwl_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24693 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_cwl_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21328 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_cwl_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17890 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_remotepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-08-06 12:02:19.000000 streamflow-0.2.0.dev7/tests/test_transfer.py
```

### Comparing `streamflow-0.2.0.dev6/LICENSE` & `streamflow-0.2.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/PKG-INFO` & `streamflow-0.2.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev6
+Version: 0.2.0.dev7
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
```

### Comparing `streamflow-0.2.0.dev6/README.md` & `streamflow-0.2.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/pyproject.toml` & `streamflow-0.2.0.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -107,7 +107,10 @@
     "if logger.isEnabledFor"
 ]
 ignore_errors = true
 omit = [
     "streamflow/__main__.py",
     "tests/*"
 ]
+
+[tool.black]
+exclude = "streamflow/cwl/antlr"
```

### Comparing `streamflow-0.2.0.dev6/streamflow/config/config.py` & `streamflow-0.2.0.dev7/streamflow/config/config.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/config/schemas/v1.0/config_schema.json` & `streamflow-0.2.0.dev7/streamflow/config/schemas/v1.0/config_schema.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5508848248106061%*

 * *Differences: {"'$defs'": "OrderedDict([('binding', OrderedDict([('oneOf', [OrderedDict([('type', 'object'), "*

 * *            "('properties', OrderedDict([('step', OrderedDict([('type', 'string')])), ('target', "*

 * *            "OrderedDict([('oneOf', [OrderedDict([('type', 'object'), ('$ref', "*

 * *            "'#/$defs/target')]), OrderedDict([('type', 'array'), ('items', OrderedDict([('type', "*

 * *            "'object'), ('$ref', '#/$defs/target')]))])])])), ('filters', OrderedDict([('type', "*

 * *            "'array'), ('items', Orde […]*

```diff
@@ -1,13 +1,10 @@
 {
-    "$id": "config_schema.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "definitions": {
+    "$defs": {
         "binding": {
-            "$id": "#/definitions/binding",
             "oneOf": [
                 {
                     "additionalProperties": false,
                     "properties": {
                         "filters": {
                             "description": "The filters used to manipulate the targets associated with this binding.",
                             "items": {
@@ -17,20 +14,20 @@
                         },
                         "step": {
                             "type": "string"
                         },
                         "target": {
                             "oneOf": [
                                 {
-                                    "$ref": "#/definitions/target",
+                                    "$ref": "#/$defs/target",
                                     "type": "object"
                                 },
                                 {
                                     "items": {
-                                        "$ref": "#/definitions/target",
+                                        "$ref": "#/$defs/target",
                                         "type": "object"
                                     },
                                     "type": "array"
                                 }
                             ]
                         }
                     },
@@ -43,45 +40,43 @@
                 {
                     "additionalProperties": false,
                     "properties": {
                         "port": {
                             "type": "string"
                         },
                         "target": {
-                            "$ref": "#/definitions/target",
+                            "$ref": "#/$defs/target",
                             "type": "object"
                         }
                     },
                     "required": [
                         "port",
                         "target"
                     ],
                     "type": "object"
                 }
             ]
         },
         "bindingFilter": {
             "$comment": "The `config` property is injected by each BindingFilter extension",
-            "$id": "#/definitions/bindingFilter",
-            "definitions": {},
+            "$defs": {},
             "properties": {
                 "type": {
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "config"
             ],
             "type": "object"
         },
         "checkpointManager": {
             "$comment": "The `config` property is injected by each CheckpointManager extension",
-            "$id": "#/definitions/checkpointManager",
-            "definitions": {},
+            "$defs": {},
             "if": {
                 "properties": {
                     "enabled": {
                         "const": true
                     }
                 }
             },
@@ -100,19 +95,17 @@
                     "type",
                     "config"
                 ]
             },
             "type": "object"
         },
         "cwl": {
-            "$id": "#/definitions/cwl",
             "docker": {
                 "$comment": "The `config` property is injected by each CWLDockerTranslator extension",
-                "$id": "#/definitions/cwl/docker",
-                "definitions": {},
+                "$defs": {},
                 "properties": {
                     "type": {
                         "type": "string"
                     },
                     "wrapper": {
                         "default": true,
                         "description": "If true, the Docker target wraps the original target bound to the step. If false, it overrides it.",
@@ -125,46 +118,43 @@
                 ],
                 "type": "object"
             },
             "type": "object"
         },
         "dataManager": {
             "$comment": "The `config` property is injected by each DataManager extension",
-            "$id": "#/definitions/dataManager",
-            "definitions": {},
+            "$defs": {},
             "properties": {
                 "type": {
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "config"
             ],
             "type": "object"
         },
         "database": {
             "$comment": "The `config` property is injected by each Database extension",
-            "$id": "#/definitions/database",
-            "definitions": {},
+            "$defs": {},
             "properties": {
                 "type": {
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "config"
             ],
             "type": "object"
         },
         "deployment": {
             "$comment": "The `config` property is injected by each Connector extension",
-            "$id": "#/definitions/deployment",
-            "definitions": {},
+            "$defs": {},
             "properties": {
                 "external": {
                     "default": false,
                     "description": "If set, StreamFlow does not manage the lifecycle of the execution environment. This means that all required services must be up and running when the workflow starts",
                     "type": "boolean"
                 },
                 "lazy": {
@@ -194,31 +184,29 @@
                 "type",
                 "config"
             ],
             "type": "object"
         },
         "deploymentManager": {
             "$comment": "The `config` property is injected by each DeploymentManager extension",
-            "$id": "#/definitions/deploymentManager",
-            "definitions": {},
+            "$defs": {},
             "properties": {
                 "type": {
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "config"
             ],
             "type": "object"
         },
         "failureManager": {
             "$comment": "The `config` property is injected by each FailureManager extension",
-            "$id": "#/definitions/failureManager",
-            "definitions": {},
+            "$defs": {},
             "if": {
                 "properties": {
                     "enabled": {
                         "const": true
                     }
                 }
             },
@@ -238,44 +226,41 @@
                     "config"
                 ]
             },
             "type": "object"
         },
         "policy": {
             "$comment": "The `config` property is injected by each Policy extension",
-            "$id": "#/definitions/policy",
-            "definitions": {},
+            "$defs": {},
             "properties": {
                 "type": {
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "config"
             ],
             "type": "object"
         },
         "scheduler": {
             "$comment": "The `config` property is injected by each Scheduler extension",
-            "$id": "#/definitions/scheduler",
-            "definitions": {},
+            "$defs": {},
             "properties": {
                 "type": {
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "config"
             ],
             "type": "object"
         },
         "target": {
-            "$id": "#/definitions/target",
             "additionalProperties": false,
             "oneOf": [
                 {
                     "required": [
                         "deployment"
                     ]
                 },
@@ -315,46 +300,24 @@
                     "description": "Path to the working directory. It overrides the deployment-level setting.",
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "workflow": {
-            "$id": "#/definitions/workflow",
-            "allOf": [
-                {
-                    "if": {
-                        "properties": {
-                            "type": {
-                                "const": "cwl"
-                            }
-                        }
-                    },
-                    "then": {
-                        "properties": {
-                            "config": {
-                                "$id": "#/definitions/workflow/properties/config",
-                                "$ref": "#/definitions/workflow/definitions/cwl",
-                                "type": "object"
-                            }
-                        }
-                    }
-                }
-            ],
-            "definitions": {
+            "$defs": {
                 "cwl": {
-                    "$id": "#/definitions/workflow/definitions/cwl",
                     "additionalProperties": false,
                     "properties": {
                         "docker": {
                             "items": {
                                 "additionalProperties": false,
                                 "properties": {
                                     "deployment": {
-                                        "$ref": "#/definitions/cwl/docker",
+                                        "$ref": "#/$defs/cwl/docker",
                                         "type": "object"
                                     },
                                     "step": {
                                         "type": "string"
                                     }
                                 },
                                 "required": [
@@ -374,134 +337,142 @@
                     },
                     "required": [
                         "file"
                     ],
                     "type": "object"
                 }
             },
+            "allOf": [
+                {
+                    "if": {
+                        "properties": {
+                            "type": {
+                                "const": "cwl"
+                            }
+                        }
+                    },
+                    "then": {
+                        "properties": {
+                            "config": {
+                                "$ref": "#/$defs/workflow/$defs/cwl",
+                                "type": "object"
+                            }
+                        }
+                    }
+                }
+            ],
             "properties": {
                 "bindings": {
-                    "$id": "#/definitions/workflow/properties/bindings",
                     "items": {
                         "oneOf": [
                             {
-                                "$ref": "#/definitions/binding",
+                                "$ref": "#/$defs/binding",
                                 "type": "object"
                             },
                             {
                                 "items": {
-                                    "$ref": "#/definitions/binding",
+                                    "$ref": "#/$defs/binding",
                                     "type": "object"
                                 },
                                 "type": "array"
                             }
                         ]
                     },
                     "type": "array",
                     "uniqueItems": true
                 },
                 "type": {
-                    "$id": "#/definitions/workflow/properties/type",
                     "enum": [
                         "cwl"
                     ],
                     "type": "string"
                 }
             },
             "required": [
                 "type",
                 "config"
             ],
             "type": "object"
         }
     },
+    "$id": "config_schema.json",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
+    "additionalProperties": false,
     "properties": {
         "bindingFilters": {
-            "$id": "#/properties/bindingFilters",
             "patternProperties": {
                 "^[a-z][a-zA-Z0-9._-]*$": {
-                    "$ref": "#/definitions/bindingFilter"
+                    "$ref": "#/$defs/bindingFilter"
                 }
             },
             "type": "object"
         },
         "checkpointManager": {
-            "$id": "#/properties/checkpointManager",
-            "$ref": "#/definitions/checkpointManager",
+            "$ref": "#/$defs/checkpointManager",
             "type": "object"
         },
         "dataManager": {
-            "$id": "#/properties/dataManager",
-            "$ref": "#/definitions/dataManager",
+            "$ref": "#/$defs/dataManager",
             "type": "object"
         },
         "database": {
-            "$id": "#/properties/database",
-            "$ref": "#/definitions/database",
+            "$ref": "#/$defs/database",
             "type": "object"
         },
         "deploymentManager": {
-            "$id": "#/properties/deploymentManager",
-            "$ref": "#/definitions/deploymentManager",
+            "$ref": "#/$defs/deploymentManager",
             "type": "object"
         },
         "deployments": {
-            "$id": "#/properties/deployments",
             "additionalProperties": false,
             "patternProperties": {
                 "^[a-z][a-zA-Z0-9._-]*$": {
-                    "$ref": "#/definitions/deployment"
+                    "$ref": "#/$defs/deployment"
                 }
             },
             "type": "object"
         },
         "failureManager": {
-            "$id": "#/properties/failureManager",
-            "$ref": "#/definitions/failureManager",
+            "$ref": "#/$defs/failureManager",
             "type": "object"
         },
         "models": {
-            "$id": "#/properties/deployments",
             "additionalProperties": false,
             "patternProperties": {
                 "^[a-z][a-zA-Z0-9._-]*$": {
-                    "$ref": "#/definitions/deployment"
+                    "$ref": "#/$defs/deployment"
                 }
             },
             "type": "object"
         },
         "scheduling": {
-            "$id": "#/properties/scheduling",
             "properties": {
                 "policies": {
-                    "$id": "#/properties/scheduling/policies",
                     "patternProperties": {
                         "^[a-z][a-zA-Z0-9._-]*$": {
-                            "$ref": "#/definitions/policy"
+                            "$ref": "#/$defs/policy"
                         }
                     },
                     "type": "object"
                 },
                 "scheduler": {
-                    "$id": "#/properties/scheduling/scheduler",
-                    "$ref": "#/definitions/scheduler",
+                    "$ref": "#/$defs/scheduler",
                     "type": "object"
                 }
             },
             "type": "object"
         },
         "version": {
             "type": "string"
         },
         "workflows": {
-            "$id": "#/properties/workflows",
             "additionalProperties": false,
             "patternProperties": {
                 "^[a-z][a-zA-Z0-9._-]*$": {
-                    "$ref": "#/definitions/workflow"
+                    "$ref": "#/$defs/workflow"
                 }
             },
             "type": "object"
         }
     },
     "required": [
         "version"
```

### Comparing `streamflow-0.2.0.dev6/streamflow/config/validator.py` & `streamflow-0.2.0.dev7/streamflow/config/validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import os
 from typing import TYPE_CHECKING
 
 import jsonref
 import pkg_resources
-from jsonschema import Draft7Validator
+from jsonschema.validators import validator_for
 from ruamel.yaml import YAML
 
 from streamflow.core import utils
 from streamflow.core.exception import WorkflowDefinitionException
 from streamflow.cwl.requirement.docker import cwl_docker_translator_classes
 from streamflow.data import data_manager_classes
 from streamflow.deployment import deployment_manager_classes
@@ -32,24 +32,32 @@
         "The StreamFlow configuration is invalid because:\n{error_msgs}".format(
             error_msgs="\n".join([f" - {err}" for err in errors])
         )
     )
 
 
 def load_jsonschema(config_file: MutableMapping[str, Any]):
+    if "version" not in config_file:
+        raise WorkflowDefinitionException(
+            "The `version` clause is mandatory and should be equal to `v1.0`."
+        )
     try:
         base_path = pkg_resources.resource_filename(
             __name__, os.path.join("schemas", config_file["version"])
         )
     except pkg_resources.ResolutionError:
-        raise Exception(f"Version {config_file['version']} is unsupported")
+        raise WorkflowDefinitionException(
+            f"Version {config_file['version']} is unsupported. The `version` clause should be equal to `v1.0`."
+        )
     filename = os.path.join(base_path, "config_schema.json")
     if not os.path.exists(filename):
-        raise Exception(f'Version in "{filename}" is unsupported')
-    with open(filename) as f:
+        raise WorkflowDefinitionException(
+            f"Version {config_file['version']} is unsupported. The `version` clause should be equal to `v1.0`."
+        )
+    with open(os.path.join(base_path, "config_schema.json")) as f:
         return jsonref.loads(f.read(), base_uri=f"file://{base_path}/", jsonschema=True)
 
 
 class SfValidator:
     def __init__(self) -> None:
         super().__init__()
         self.yaml = YAML(typ="safe")
@@ -67,10 +75,11 @@
         utils.inject_schema(schema, database_classes, "database")
         utils.inject_schema(schema, data_manager_classes, "dataManager")
         utils.inject_schema(schema, connector_classes, "deployment")
         utils.inject_schema(schema, deployment_manager_classes, "deploymentManager")
         utils.inject_schema(schema, failure_manager_classes, "failureManager")
         utils.inject_schema(schema, policy_classes, "policy")
         utils.inject_schema(schema, scheduler_classes, "scheduler")
-        validator = Draft7Validator(schema)
+        cls = validator_for(schema)
+        validator = cls(schema)
         handle_errors(validator.iter_errors(streamflow_config))
         return streamflow_config
```

### Comparing `streamflow-0.2.0.dev6/streamflow/core/asyncache.py` & `streamflow-0.2.0.dev7/streamflow/core/asyncache.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/config.py` & `streamflow-0.2.0.dev7/streamflow/core/config.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/context.py` & `streamflow-0.2.0.dev7/streamflow/core/context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/data.py` & `streamflow-0.2.0.dev7/streamflow/core/data.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/deployment.py` & `streamflow-0.2.0.dev7/streamflow/core/deployment.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/exception.py` & `streamflow-0.2.0.dev7/streamflow/core/exception.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/persistence.py` & `streamflow-0.2.0.dev7/streamflow/core/persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/provenance.py` & `streamflow-0.2.0.dev7/streamflow/core/provenance.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/recovery.py` & `streamflow-0.2.0.dev7/streamflow/core/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/scheduling.py` & `streamflow-0.2.0.dev7/streamflow/core/scheduling.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/core/utils.py` & `streamflow-0.2.0.dev7/streamflow/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,19 +256,19 @@
         if entity_schema := entity.get_schema():
             with open(entity_schema) as f:
                 entity_schema = jsonref.loads(
                     f.read(),
                     base_uri=f"file://{os.path.dirname(entity_schema)}/",
                     jsonschema=True,
                 )
-            definition = schema["definitions"]
+            definition = schema["$defs"]
             for el in definition_name.split(posixpath.sep):
                 definition = definition[el]
             definition["properties"]["type"].setdefault("enum", []).append(name)
-            definition["definitions"][name] = entity_schema
+            definition["$defs"][name] = entity_schema
             definition.setdefault("allOf", []).append(
                 {
                     "if": {"properties": {"type": {"const": name}}},
                     "then": {"properties": {"config": entity_schema}},
                 }
             )
```

### Comparing `streamflow-0.2.0.dev6/streamflow/core/workflow.py` & `streamflow-0.2.0.dev7/streamflow/core/workflow.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptLexer.py` & `streamflow-0.2.0.dev7/streamflow/cwl/antlr/ECMAScriptLexer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptListener.py` & `streamflow-0.2.0.dev7/streamflow/cwl/antlr/ECMAScriptListener.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptParser.py` & `streamflow-0.2.0.dev7/streamflow/cwl/antlr/ECMAScriptParser.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/combinator.py` & `streamflow-0.2.0.dev7/streamflow/cwl/combinator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/command.py` & `streamflow-0.2.0.dev7/streamflow/cwl/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 import logging
 import posixpath
 import re
 import shlex
 import time
 from abc import ABC
 from asyncio.subprocess import STDOUT
+from decimal import Decimal
 from types import ModuleType
 from typing import Any, IO, Iterable, MutableMapping, MutableSequence, Type, cast
 
+from ruamel.yaml import RoundTripRepresenter
+from ruamel.yaml.scalarfloat import ScalarFloat
+
 from streamflow.core.context import StreamFlowContext
 from streamflow.core.data import DataLocation
 from streamflow.core.deployment import Connector
 from streamflow.core.exception import (
     WorkflowDefinitionException,
     WorkflowExecutionException,
 )
@@ -241,42 +245,53 @@
 
 def _get_value_for_command(token: Any, item_separator: str | None) -> Any:
     if isinstance(token, MutableSequence):
         value = []
         for element in token:
             value.append(_get_value_for_command(element, item_separator))
         if item_separator is not None:
-            value = item_separator.join([str(v) for v in value])
+            value = item_separator.join([_get_value_repr(v) for v in value])
         return value or None
     elif isinstance(token, MutableMapping):
         if (path := utils.get_path_from_token(token)) is not None:
             return path
         else:
             raise WorkflowExecutionException(
                 "Unsupported value " + str(token) + " from expression"
             )
     else:
         return token
 
 
+def _get_value_repr(value: Any) -> str | None:
+    if isinstance(value, ScalarFloat):
+        rep = RoundTripRepresenter()
+        dec_value = Decimal(rep.represent_scalar_float(value).value)
+        if "E" in str(dec_value):
+            return str(dec_value.quantize(1))
+        return str(dec_value)
+    else:
+        return str(value)
+
+
 def _escape_value(value: Any) -> Any:
     if isinstance(value, MutableSequence):
         return [_escape_value(v) for v in value]
     else:
-        return shlex.quote(str(value))
+        return shlex.quote(_get_value_repr(value))
 
 
 def _merge_tokens(
     bindings_map: MutableMapping[str, MutableSequence[Any]]
 ) -> MutableSequence[Any]:
     command = []
     for binding_position in alphanumeric_sorting(bindings_map.keys()):
         for binding in bindings_map[binding_position]:
             command.extend(flatten_list(binding))
-    return [str(token) for token in command]
+    return [_get_value_repr(token) for token in command]
 
 
 def alphanumeric_sorting(list_to_sort: Iterable) -> Iterable:
     regex = "(-{0,1}[0-9]+)"
     return sorted(
         list_to_sort,
         key=lambda key: [
@@ -896,15 +911,15 @@
                     if isinstance(value, MutableSequence):
                         value = [self.prefix] + list(value)
                     else:
                         value = [self.prefix, value]
                 elif isinstance(value, MutableSequence):
                     value = [self.prefix].extend(value)
                 else:
-                    value = [self.prefix + str(value)]
+                    value = [self.prefix + _get_value_repr(value)]
             # If value is a boolean with no prefix, skip it
             if isinstance(value, bool):
                 return bindings_map
             # Ensure value is a list
             if not isinstance(value, MutableSequence):
                 value = [value]
             # Process shell escape only on the single command token
```

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/expression.py` & `streamflow-0.2.0.dev7/streamflow/cwl/expression.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/hardware.py` & `streamflow-0.2.0.dev7/streamflow/cwl/hardware.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/main.py` & `streamflow-0.2.0.dev7/streamflow/cwl/main.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/processor.py` & `streamflow-0.2.0.dev7/streamflow/cwl/processor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/docker.py` & `streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/docker.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/kubernetes.py` & `streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/kubernetes.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/docker.json` & `streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/docker.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "docker.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "addHost": {
             "description": "Add a custom host-to-IP mapping (host:ip)",
             "items": {
                 "type": "string"
             },
```

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2` & `streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/kubernetes.json` & `streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/kubernetes.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "kubernetes.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "debug": {
             "description": "Enable verbose output",
             "type": "boolean"
         },
         "file": {
```

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/singularity.json` & `streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/schemas/singularity.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "singularity.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "addCaps": {
             "description": "A comma separated capability list to add",
             "type": "string"
         },
         "allowSetuid": {
```

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/singularity.py` & `streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/singularity.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/translator.py` & `streamflow-0.2.0.dev7/streamflow/cwl/requirement/docker/translator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/runner.py` & `streamflow-0.2.0.dev7/streamflow/cwl/runner.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/step.py` & `streamflow-0.2.0.dev7/streamflow/cwl/step.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/token.py` & `streamflow-0.2.0.dev7/streamflow/cwl/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/transformer.py` & `streamflow-0.2.0.dev7/streamflow/cwl/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/translator.py` & `streamflow-0.2.0.dev7/streamflow/cwl/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1291,14 +1291,16 @@
                 workflow=workflow,
                 value=element_input["default"],
             )
         # Return port
         return input_port
 
     def _get_source_port(self, workflow: Workflow, source_name: str) -> Port:
+        if source_name in self.output_ports:
+            return self.output_ports[source_name]
         if source_name not in self.input_ports:
             if source_name not in self.output_ports:
                 self.output_ports[source_name] = workflow.create_port()
             return self.output_ports[source_name]
         else:
             return self.input_ports[source_name]
```

### Comparing `streamflow-0.2.0.dev6/streamflow/cwl/utils.py` & `streamflow-0.2.0.dev7/streamflow/cwl/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/data/data_manager.py` & `streamflow-0.2.0.dev7/streamflow/data/data_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/data/remotepath.py` & `streamflow-0.2.0.dev7/streamflow/data/remotepath.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/aiotarstream.py` & `streamflow-0.2.0.dev7/streamflow/deployment/aiotarstream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/__init__.py` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from streamflow.deployment.connector.kubernetes import (
     Helm3Connector,
     KubernetesConnector,
 )
 from streamflow.deployment.connector.local import LocalConnector
 from streamflow.deployment.connector.occam import OccamConnector
 from streamflow.deployment.connector.queue_manager import (
+    FluxConnector,
     PBSConnector,
     SlurmConnector,
-    FluxConnector,
 )
 from streamflow.deployment.connector.ssh import SSHConnector
 
 connector_classes = {
     "docker": DockerConnector,
     "docker-compose": DockerComposeConnector,
     "flux": FluxConnector,
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/base.py` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/base.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/container.py` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/container.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/kubernetes.py` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/kubernetes.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/local.py` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/local.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/occam.py` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/occam.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/queue_manager.py` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/queue_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,17 +354,21 @@
                 sshKey=sshKey,
                 sshKeyPassphraseFile=sshKeyPassphraseFile,
                 transferBufferSize=transferBufferSize,
                 username=username,
             )
         super().__init__(deployment_name, config_dir, connector)
         files_map: MutableMapping[str, Any] = {}
-        self.services: MutableMapping[str, QueueManagerService] = services or {}
-        if services:
-            for name, service in services.items():
+        self.services = (
+            {k: self._service_class(**v) for k, v in services.items()}
+            if services
+            else {}
+        )
+        if self.services:
+            for name, service in self.services.items():
                 if service.file is not None:
                     with open(os.path.join(self.config_dir, service.file)) as f:
                         files_map[name] = f.read()
         if file is not None:
             if logger.isEnabledFor(logging.WARN):
                 logger.warn(
                     "The `file` keyword is deprecated and will be removed in StreamFlow 0.3.0. "
@@ -422,14 +426,19 @@
         stdin: int | str | None = None,
         stdout: int | str = asyncio.subprocess.STDOUT,
         stderr: int | str = asyncio.subprocess.STDOUT,
         timeout: int | None = None,
     ) -> str:
         ...
 
+    @property
+    @abstractmethod
+    def _service_class(self) -> type[QueueManagerService]:
+        ...
+
     async def get_available_locations(
         self,
         service: str | None = None,
         input_directory: str | None = None,
         output_directory: str | None = None,
         tmp_directory: str | None = None,
     ) -> MutableMapping[str, AvailableLocation]:
@@ -623,14 +632,18 @@
         stdout, _ = await self.connector.run(
             location=location,
             command=command,
             capture_output=True,
         )
         return [j.strip() for j in stdout.strip().splitlines()]
 
+    @property
+    def _service_class(self) -> type[QueueManagerService]:
+        return SlurmService
+
     async def _remove_jobs(self, location: Location) -> None:
         await self.connector.run(
             location=location, command=["scancel", " ".join(self.scheduledJobs)]
         )
 
     async def _run_batch_command(
         self,
@@ -914,14 +927,18 @@
         stdout, _ = await self.connector.run(
             location=location,
             command=command,
             capture_output=True,
         )
         return stdout.strip()
 
+    @property
+    def _service_class(self) -> type[QueueManagerService]:
+        return PBSService
+
 
 class FluxConnector(QueueManagerConnector):
     @classmethod
     def get_schema(cls) -> str:
         return pkg_resources.resource_filename(
             __name__, os.path.join("schemas", "flux.json")
         )
@@ -1077,7 +1094,11 @@
         )
         if returncode == 0:
             return stdout.strip()
         else:
             raise WorkflowExecutionException(
                 f"Error submitting job {job_name} to Flux: {stdout.strip()}"
             )
+
+    @property
+    def _service_class(self) -> type[QueueManagerService]:
+        return FluxService
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/docker-compose.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/docker-compose.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "docker-compose.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "alwaysRecreateDeps": {
             "description": "Recreate dependent containers (incompatible with noRecreate)",
             "type": "boolean"
         },
         "build": {
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/docker.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/docker.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "docker.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "addHost": {
             "description": "Add a custom host-to-IP mapping (host:ip)",
             "items": {
                 "type": "string"
             },
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/flux.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/flux.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49884259259259256%*

 * *Differences: {"'$defs'": "OrderedDict([('service', OrderedDict([('type', 'object'), ('title', 'FluxService'), "*

 * *            "('description', 'This complex type represents a submission to the Flux queue "*

 * *            "manager.'), ('properties', OrderedDict([('beginTime', OrderedDict([('type', "*

 * *            "'string'), ('description', 'Convenience option for setting a ``begin-time`` "*

 * *            'dependency for a job. The job is guaranteed to start after the specified date and '*

 * *            "time')])), ('brokerOpts', Ord […]*

```diff
@@ -1,19 +1,10 @@
 {
-    "$id": "flux.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": false,
-    "allOf": [
-        {
-            "$ref": "queue_manager.json"
-        }
-    ],
-    "definitions": {
+    "$defs": {
         "service": {
-            "$id": "#/definitions/service",
             "description": "This complex type represents a submission to the Flux queue manager.",
             "properties": {
                 "beginTime": {
                     "description": "Convenience option for setting a ``begin-time`` dependency for a job. The job is guaranteed to start after the specified date and time",
                     "type": "string"
                 },
                 "brokerOpts": {
@@ -144,20 +135,28 @@
                     "type": "integer"
                 }
             },
             "title": "FluxService",
             "type": "object"
         }
     },
+    "$id": "flux.json",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
+    "allOf": [
+        {
+            "$ref": "queue_manager.json"
+        }
+    ],
     "properties": {
         "services": {
             "description": "Map containing named configurations of Flux submissions. Parameters can be either specified as #flux directives in a file or directly in YAML format.",
             "patternProperties": {
                 "^[a-z][a-zA-Z0-9._-]*$": {
-                    "$ref": "#/definitions/service"
+                    "$ref": "#/$defs/service"
                 }
             },
             "type": "object"
         }
     },
-    "type": "object"
+    "type": "object",
+    "unevaluatedProperties": false
 }
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/helm3.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/helm3.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "helm3.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "atomic": {
             "description": "If set, installation process purges chart on fail (also sets wait flag)",
             "type": "boolean"
         },
         "caFile": {
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/kubernetes.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/kubernetes.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "kubernetes.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "debug": {
             "description": "Enable verbose output",
             "type": "boolean"
         },
         "files": {
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/occam.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/occam.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "occam.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "file": {
             "description": "Path to the file describing Occam environment",
             "type": "string"
         },
         "hostname": {
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/pbs.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/pbs.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49884259259259256%*

 * *Differences: {"'$defs'": "OrderedDict([('service', OrderedDict([('type', 'object'), ('title', 'PBSService'), "*

 * *            "('description', 'This complex type represents a submission to the PBS queue "*

 * *            "manager.'), ('properties', OrderedDict([('account', OrderedDict([('type', 'string'), "*

 * *            "('description', 'Defines the account string associated with the job')])), "*

 * *            "('additionalAttributes', OrderedDict([('type', 'object'), ('description', 'Specify "*

 * *            "additional job attribut […]*

```diff
@@ -1,19 +1,10 @@
 {
-    "$id": "pbs.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": false,
-    "allOf": [
-        {
-            "$ref": "queue_manager.json"
-        }
-    ],
-    "definitions": {
+    "$defs": {
         "service": {
-            "$id": "#/definitions/service",
             "description": "This complex type represents a submission to the PBS queue manager.",
             "properties": {
                 "account": {
                     "description": "Defines the account string associated with the job",
                     "type": "string"
                 },
                 "additionalAttributes": {
@@ -77,20 +68,28 @@
                     "type": "string"
                 }
             },
             "title": "PBSService",
             "type": "object"
         }
     },
+    "$id": "pbs.json",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
+    "allOf": [
+        {
+            "$ref": "queue_manager.json"
+        }
+    ],
     "properties": {
         "services": {
             "description": "Map containing named configurations of PBS submissions. Parameters can be either specified as #BSUB directives in a file or directly in YAML format.",
             "patternProperties": {
                 "^[a-z][a-zA-Z0-9._-]*$": {
-                    "$ref": "#/definitions/service"
+                    "$ref": "#/$defs/service"
                 }
             },
             "type": "object"
         }
     },
-    "type": "object"
+    "type": "object",
+    "unevaluatedProperties": false
 }
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/queue_manager.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/queue_manager.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8741164434523809%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'",*

 * * "'properties'": "{'dataTransferConnection': {'oneOf': {1: {'$ref': "*

 * *                 "'ssh.json#/$defs/connection'}}}, 'tunnel': {'$ref': "*

 * *                 "'ssh.json#/$defs/connection'}}"}*

```diff
@@ -1,24 +1,24 @@
 {
     "$id": "queue_manager.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "properties": {
         "checkHostKey": {
             "default": true,
             "description": "(**Deprecated.** Use the `wraps` directive to wrap a standalone SSH connector.) Perform a strict validation of the host SSH keys (and return exception if key is not recognized as valid)",
             "type": "boolean"
         },
         "dataTransferConnection": {
             "description": "(**Deprecated.** Use the `wraps` directive to wrap a standalone SSH connector.) Sometimes HPC clusters provide dedicated hostnames for large data transfers, which guarantee a higher efficiency for data movements",
             "oneOf": [
                 {
                     "type": "string"
                 },
                 {
-                    "$ref": "ssh.json#/definitions/connection",
+                    "$ref": "ssh.json#/$defs/connection",
                     "type": "object"
                 }
             ]
         },
         "file": {
             "description": "(**Deprecated.** Use services.) Path to a file containing a Jinja2 template, describing how the StreamFlow command should be executed in the remote environment",
             "type": "string"
@@ -61,15 +61,15 @@
         },
         "transferBufferSize": {
             "default": "64kiB",
             "description": "Buffer size allocated for local and remote data transfers",
             "type": "integer"
         },
         "tunnel": {
-            "$ref": "ssh.json#/definitions/connection",
+            "$ref": "ssh.json#/$defs/connection",
             "description": "(**Deprecated.** Use the `wraps` directive to wrap a standalone SSH connector.) External SSH connection parameters for tunneling",
             "type": "object"
         },
         "username": {
             "description": "(**Deprecated.** Use the `wraps` directive to wrap a standalone SSH connector.) Username needed to connect with the SSH environment",
             "type": "string"
         }
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/singularity.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/singularity.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "singularity.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
     "additionalProperties": false,
     "properties": {
         "addCaps": {
             "description": "A comma separated capability list to add",
             "type": "string"
         },
         "allowSetuid": {
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/slurm.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/slurm.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49884259259259256%*

 * *Differences: {"'$defs'": "OrderedDict([('service', OrderedDict([('type', 'object'), ('title', 'SlurmService'), "*

 * *            "('description', 'This complex type represents a submission to the Slurm queue "*

 * *            "manager.'), ('properties', OrderedDict([('account', OrderedDict([('type', 'string'), "*

 * *            "('description', 'Charge resources used by this job to specified account')])), "*

 * *            "('acctgFreq', OrderedDict([('type', 'string'), ('description', 'Define the job "*

 * *            "accounting and prof […]*

```diff
@@ -1,19 +1,10 @@
 {
-    "$id": "slurm.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": false,
-    "allOf": [
-        {
-            "$ref": "queue_manager.json"
-        }
-    ],
-    "definitions": {
+    "$defs": {
         "service": {
-            "$id": "#/definitions/service",
             "description": "This complex type represents a submission to the Slurm queue manager.",
             "properties": {
                 "account": {
                     "description": "Charge resources used by this job to specified account",
                     "type": "string"
                 },
                 "acctgFreq": {
@@ -396,20 +387,28 @@
                     "type": "string"
                 }
             },
             "title": "SlurmService",
             "type": "object"
         }
     },
+    "$id": "slurm.json",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
+    "allOf": [
+        {
+            "$ref": "queue_manager.json"
+        }
+    ],
     "properties": {
         "services": {
             "description": "Map containing named configurations of Slurm submissions. Parameters can be either specified as #SBATCH directives in a file or directly in YAML format.",
             "patternProperties": {
                 "^[a-z][a-zA-Z0-9._-]*$": {
-                    "$ref": "#/definitions/service"
+                    "$ref": "#/$defs/service"
                 }
             },
             "type": "object"
         }
     },
-    "type": "object"
+    "type": "object",
+    "unevaluatedProperties": false
 }
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/ssh.json` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/schemas/ssh.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6870349702380952%*

 * *Differences: {"'$defs'": "OrderedDict([('connection', OrderedDict([('type', 'object'), ('title', "*

 * *            "'SSHConnection'), ('description', 'This complex type represents an SSH connection to "*

 * *            "a remote node, identified by its hostname.'), ('properties', "*

 * *            "OrderedDict([('checkHostKey', OrderedDict([('type', 'boolean'), ('description', "*

 * *            "'Perform a strict validation of the host SSH keys (and return exception if key is not "*

 * *            "recognized as valid)'), ('default', True) […]*

```diff
@@ -1,14 +1,10 @@
 {
-    "$id": "ssh.json",
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": false,
-    "definitions": {
+    "$defs": {
         "connection": {
-            "$id": "#/definitions/connection",
             "additionalProperties": false,
             "description": "This complex type represents an SSH connection to a remote node, identified by its hostname.",
             "properties": {
                 "checkHostKey": {
                     "default": true,
                     "description": "Perform a strict validation of the host SSH keys (and return exception if key is not recognized as valid)",
                     "type": "boolean"
@@ -38,15 +34,15 @@
                         "null"
                     ]
                 },
                 "tunnel": {
                     "description": "External SSH connection parameters for tunneling",
                     "oneOf": [
                         {
-                            "$ref": "#/definitions/connection",
+                            "$ref": "#/$defs/connection",
                             "type": "object"
                         },
                         {
                             "type": "null"
                         }
                     ]
                 },
@@ -61,28 +57,31 @@
             "required": [
                 "hostname"
             ],
             "title": "SSHConnection",
             "type": "object"
         }
     },
+    "$id": "ssh.json",
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
+    "additionalProperties": false,
     "properties": {
         "checkHostKey": {
             "default": true,
             "description": "Perform a strict validation of the host SSH keys (and return exception if key is not recognized as valid)",
             "type": "boolean"
         },
         "dataTransferConnection": {
             "description": "Sometimes HPC clusters provide dedicated hostnames for large data transfers, which guarantee a higher efficiency for data movements",
             "oneOf": [
                 {
                     "type": "string"
                 },
                 {
-                    "$ref": "#/definitions/connection",
+                    "$ref": "#/$defs/connection",
                     "type": "object"
                 }
             ]
         },
         "file": {
             "description": "(**Deprecated.** Use services.) Path to a file containing a Jinja2 template, describing how the StreamFlow command should be executed in the remote environment",
             "type": "string"
@@ -101,15 +100,15 @@
             "description": "List of worker nodes. They can be represented as either single hostnames or connection objects. When a property is missing, it is inherited from the connector context",
             "items": {
                 "oneOf": [
                     {
                         "type": "string"
                     },
                     {
-                        "$ref": "#/definitions/connection",
+                        "$ref": "#/$defs/connection",
                         "type": "object"
                     }
                 ]
             },
             "type": "array"
         },
         "passwordFile": {
@@ -142,15 +141,15 @@
         },
         "transferBufferSize": {
             "default": "64kiB",
             "description": "Buffer size allocated for local and remote data transfers",
             "type": "integer"
         },
         "tunnel": {
-            "$ref": "#/definitions/connection",
+            "$ref": "#/$defs/connection",
             "description": "External SSH connection parameters for tunneling",
             "type": "object"
         },
         "username": {
             "description": "Username needed to connect with the SSH environment",
             "type": "string"
         }
```

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/connector/ssh.py` & `streamflow-0.2.0.dev7/streamflow/deployment/connector/ssh.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/deployment_manager.py` & `streamflow-0.2.0.dev7/streamflow/deployment/deployment_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/filter/shuffle.py` & `streamflow-0.2.0.dev7/streamflow/deployment/filter/shuffle.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/future.py` & `streamflow-0.2.0.dev7/streamflow/deployment/future.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/stream.py` & `streamflow-0.2.0.dev7/streamflow/deployment/stream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/template.py` & `streamflow-0.2.0.dev7/streamflow/deployment/template.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/utils.py` & `streamflow-0.2.0.dev7/streamflow/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/deployment/wrapper.py` & `streamflow-0.2.0.dev7/streamflow/deployment/wrapper.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/ext/plugin.py` & `streamflow-0.2.0.dev7/streamflow/ext/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from streamflow.deployment.filter import binding_filter_classes
 from streamflow.log_handler import logger
 from streamflow.persistence import database_classes
 from streamflow.recovery import checkpoint_manager_classes, failure_manager_classes
 from streamflow.scheduling import scheduler_classes
 from streamflow.scheduling.policy import policy_classes
 
-
 extension_points = {
     "binding_filter": binding_filter_classes,
     "checkpoint_manager": checkpoint_manager_classes,
     "cwl_docker_translator": cwl_docker_translator_classes,
     "connector": connector_classes,
     "data_manager": data_manager_classes,
     "database": database_classes,
```

### Comparing `streamflow-0.2.0.dev6/streamflow/ext/utils.py` & `streamflow-0.2.0.dev7/streamflow/ext/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 import os
 import sys
-from typing import Any, MutableMapping
+from typing import Any, MutableMapping, MutableSequence
 
 import jsonref
 from importlib_metadata import entry_points
 
 from streamflow.core.exception import InvalidPluginException
 from streamflow.core.utils import get_class_fullname
 from streamflow.ext.plugin import StreamFlowPlugin, extension_points
@@ -33,48 +33,82 @@
             **obj.get("properties", {}),
             **entity_schema.get("properties", {}),
         }
     del entity_schema["allOf"]
     return dict(sorted(entity_schema["properties"].items()))
 
 
-def _get_property_desc(k: str, obj: MutableMapping[str, Any]) -> str:
+def _get_property_desc(
+    k: str, obj: MutableMapping[str, Any], refs: MutableMapping[str, Any]
+) -> str:
     property_desc = [k]
     if "type" in obj:
-        property_desc[0] = f"{property_desc[0]}: {_get_type_repr(obj)}"
+        property_desc[0] = f"{property_desc[0]}: {_get_type_repr(obj, refs)}"
     elif "oneOf" in obj:
-        types = [_get_type_repr(oo) for oo in obj["oneOf"] if "type" in oo]
+        types = [_get_type_repr(oo, refs) for oo in obj["oneOf"] if "type" in oo]
         property_desc[0] = f"{property_desc[0]}: Union[{', '.join(types)}]"
     if "default" in obj:
         property_desc[0] = f"{property_desc[0]} (default: {obj['default']})"
     if "description" in obj:
         property_desc.append(obj["description"])
     return "\n".join(property_desc)
 
 
-def _get_type_repr(obj: MutableMapping[str, Any]) -> str | None:
+def _get_type_repr(
+    obj: MutableMapping[str, Any], refs: MutableMapping[str, Any]
+) -> str | None:
     if "type" in obj:
         if obj["type"] == "object":
             if "patternProperties" in obj:
                 if len(obj["patternProperties"]) > 1:
                     types = [
-                        _get_type_repr(t) for t in obj["patternProperties"].values()
+                        _get_type_repr(t, refs)
+                        for t in obj["patternProperties"].values()
                     ]
                     type_ = f"Union[{', '.join(types)}]"
                 else:
-                    type_ = _get_type_repr(list(obj["patternProperties"].values())[0])
+                    type_ = _get_type_repr(
+                        list(obj["patternProperties"].values())[0], refs
+                    )
                 return f"Map[str, {type_}]"
+            elif "title" in obj:
+                refs[obj["title"]] = obj.get("properties", {})
+                return obj["title"]
             else:
-                return obj.get("title", "object")
+                return "object"
         else:
             return obj["type"]
     else:
         return None
 
 
+def _split_refs(refs: MutableMapping[str, Any], processed: MutableSequence[str]):
+    refs_descs = {}
+    subrefs = {}
+    for k, v in refs.items():
+        refs_descs[k] = [
+            _get_property_desc(name, prop, subrefs) for name, prop in v.items()
+        ]
+        processed.append(k)
+    if subrefs := {k: v for k, v in subrefs.items() if k not in processed}:
+        refs_descs = {**refs_descs, **_split_refs(subrefs, processed)}
+    return refs_descs
+
+
+def _split_schema(schema: MutableMapping[str, Any]):
+    required, optional = [], []
+    refs = {}
+    for k, v in schema.get("properties", {}).items():
+        if k in schema.get("required", []):
+            required.append(_get_property_desc(k, v, refs))
+        else:
+            optional.append(_get_property_desc(k, v, refs))
+    return required, optional, refs
+
+
 def list_extensions(name: str | None, type_: str | None):
     extensions = {}
     max_sizes = {
         "name": 0,
         "class": 0,
         "plugin": 0,
     }
@@ -255,28 +289,29 @@
             + "}"
             + "{:<"
             + str(max(len(plugin), 8))
             + "}"
         )
         print(format_string.format("NAME", "CLASS_NAME", "PLUGIN"))
         print(format_string.format(name, class_name, plugin))
-        property_descs = []
-        for k, v in entity_schema.get("properties", {}).items():
-            if k in entity_schema.get("required", []):
-                property_descs.append(_get_property_desc(k, v))
-        if property_descs:
-            print("\nREQUIRED\n")
-            print("\n---\n".join(property_descs))
-            property_descs = []
-        for k, v in entity_schema.get("properties", {}).items():
-            if k not in entity_schema.get("required", []):
-                property_descs.append(_get_property_desc(k, v))
-        if property_descs:
-            print("\nOPTIONAL\n")
-            print("\n---\n".join(property_descs))
+        required, optional, refs = _split_schema(entity_schema)
+        if required:
+            print("\n===================\nREQUIRED PROPERTIES\n===================\n")
+            print("\n---\n".join(required))
+        if optional:
+            print("\n===================\nOPTIONAL PROPERTIES\n===================\n")
+            print("\n---\n".join(optional))
+        if refs:
+            print("\n================\nTYPE DEFINITIONS\n================")
+            refs = _split_refs(refs, [])
+            for key, ref in refs.items():
+                print("\n" + "-" * len(key))
+                print(key)
+                print("-" * len(key) + "\n")
+                print("\n---\n".join(ref))
     else:
         print(
             f"No StreamFlow extension `{name}` of type `{type_}` detected.",
             file=sys.stderr,
         )
```

### Comparing `streamflow-0.2.0.dev6/streamflow/log_handler.py` & `streamflow-0.2.0.dev7/streamflow/log_handler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/main.py` & `streamflow-0.2.0.dev7/streamflow/main.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/parser.py` & `streamflow-0.2.0.dev7/streamflow/parser.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/persistence/base.py` & `streamflow-0.2.0.dev7/streamflow/persistence/base.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/persistence/loading_context.py` & `streamflow-0.2.0.dev7/streamflow/persistence/loading_context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/persistence/schemas/sqlite.sql` & `streamflow-0.2.0.dev7/streamflow/persistence/schemas/sqlite.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 CREATE TABLE IF NOT EXISTS workflow
 (
-    id     INTEGER PRIMARY KEY,
-    name   TEXT,
-    params TEXT,
-    status INTEGER,
-    type   TEXT,
+    id         INTEGER PRIMARY KEY,
+    name       TEXT,
+    params     TEXT,
+    status     INTEGER,
+    type       TEXT,
     start_time INTEGER,
     end_time   INTEGER
 );
 
 CREATE TABLE IF NOT EXISTS step
 (
     id       INTEGER PRIMARY KEY,
```

### Comparing `streamflow-0.2.0.dev6/streamflow/persistence/sqlite.py` & `streamflow-0.2.0.dev7/streamflow/persistence/sqlite.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/provenance/run_crate.py` & `streamflow-0.2.0.dev7/streamflow/provenance/run_crate.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from streamflow.core.provenance import ProvenanceManager
 from streamflow.core.workflow import Port, Status, Token, Workflow
 from streamflow.log_handler import logger
 from streamflow.version import VERSION
 from streamflow.workflow.token import FileToken, ListToken, ObjectToken
 from streamflow.workflow.utils import get_token_value
 
-
 ESCAPED_COMMA = re.compile(r"\\,")
 ESCAPED_DOT = re.compile(r"\\.")
 ESCAPED_EQUAL = re.compile(r"\\=")
 
 
 def _checksum(data: str) -> str:
     sha1_checksum = hashlib.new("sha1", usedforsecurity=False)
```

### Comparing `streamflow-0.2.0.dev6/streamflow/recovery/checkpoint_manager.py` & `streamflow-0.2.0.dev7/streamflow/recovery/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/recovery/failure_manager.py` & `streamflow-0.2.0.dev7/streamflow/recovery/failure_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/recovery/recovery.py` & `streamflow-0.2.0.dev7/streamflow/recovery/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/report.py` & `streamflow-0.2.0.dev7/streamflow/report.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/scheduling/policy/data_locality.py` & `streamflow-0.2.0.dev7/streamflow/scheduling/policy/data_locality.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/scheduling/scheduler.py` & `streamflow-0.2.0.dev7/streamflow/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/workflow/combinator.py` & `streamflow-0.2.0.dev7/streamflow/workflow/combinator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/workflow/executor.py` & `streamflow-0.2.0.dev7/streamflow/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/workflow/port.py` & `streamflow-0.2.0.dev7/streamflow/workflow/port.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/workflow/step.py` & `streamflow-0.2.0.dev7/streamflow/workflow/step.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/workflow/token.py` & `streamflow-0.2.0.dev7/streamflow/workflow/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/workflow/transformer.py` & `streamflow-0.2.0.dev7/streamflow/workflow/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/streamflow/workflow/utils.py` & `streamflow-0.2.0.dev7/streamflow/workflow/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from typing import MutableSequence, TYPE_CHECKING
 
 from streamflow.core.exception import WorkflowExecutionException
 from streamflow.core.workflow import Token
 from streamflow.workflow.token import (
     IterationTerminationToken,
+    JobToken,
     ListToken,
     ObjectToken,
     TerminationToken,
-    JobToken,
 )
 
 if TYPE_CHECKING:
     from typing import Any, Iterable
 
 
 def check_iteration_termination(inputs: Token | Iterable[Token]) -> bool:
```

### Comparing `streamflow-0.2.0.dev6/streamflow.egg-info/PKG-INFO` & `streamflow-0.2.0.dev7/streamflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev6
+Version: 0.2.0.dev7
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
```

### Comparing `streamflow-0.2.0.dev6/streamflow.egg-info/SOURCES.txt` & `streamflow-0.2.0.dev7/streamflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -138,8 +138,9 @@
 tests/test_cwl_loop.py
 tests/test_cwl_persistence.py
 tests/test_cwl_provenance.py
 tests/test_persistence.py
 tests/test_provenance.py
 tests/test_remotepath.py
 tests/test_scheduler.py
+tests/test_schema.py
 tests/test_transfer.py
```

### Comparing `streamflow-0.2.0.dev6/streamflow.egg-info/requires.txt` & `streamflow-0.2.0.dev7/streamflow.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-aiohttp==3.8.4
+aiohttp==3.8.5
 aiosqlite==0.19.0
 antlr4-python3-runtime==4.13.0
-asyncssh==2.13.1
+asyncssh==2.13.2
 bcrypt==4.0.1
 cachetools==5.3.1
-cwltool==3.1.20230601100705
+cwltool==3.1.20230719185429
 cwl-utils==0.28
-importlib_metadata==6.6.0
+importlib_metadata==6.8.0
 Jinja2==3.1.2
 jsonref==1.1.0
-jsonschema==4.17.3
+jsonschema==4.18.6
 kubernetes_asyncio==24.2.3
 psutil==5.9.5
 rdflib==6.3.2
 yattag==1.15.1
 
 [bandit]
 bandit==1.7.5
 
 [docs]
-sphinx==7.0.1
+sphinx==7.1.2
 sphinx-jsonschema==1.19.1
 sphinx-rtd-theme==1.2.2
 
 [lint]
-black==23.3.0
-codespell==2.2.4
-flake8-bugbear==23.6.5
-pyupgrade==3.6.0
+black==23.7.0
+codespell==2.2.5
+flake8-bugbear==23.7.10
+pyupgrade==3.10.1
 
 [report]
-pandas==2.0.2
+pandas==2.0.3
 plotly==5.15.0
 kaleido==0.2.1
 
 [test]
 cwltest==2.3.20230527113600
-pytest==7.3.2
-pytest-asyncio==0.21.0
+pytest==7.4.0
+pytest-asyncio==0.21.1
 pytest-cov==4.1.0
 pytest-xdist==3.3.1
```

### Comparing `streamflow-0.2.0.dev6/tests/test_cwl_loop.py` & `streamflow-0.2.0.dev7/tests/test_cwl_loop.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/tests/test_cwl_persistence.py` & `streamflow-0.2.0.dev7/tests/test_cwl_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,63 @@
+from __future__ import annotations
+
 import posixpath
-from rdflib import Graph
-from ruamel.yaml.scalarstring import LiteralScalarString, DoubleQuotedScalarString
+from typing import Any, MutableSequence
 
 import pytest
-
-from tests.conftest import save_load_and_test
+from rdflib import Graph
+from ruamel.yaml.scalarstring import DoubleQuotedScalarString, LiteralScalarString
 
 from streamflow.core import utils
 from streamflow.core.context import StreamFlowContext
-from streamflow.core.workflow import Workflow
-
-from streamflow.workflow.step import CombinatorStep, ExecuteStep
-
-# abstract classes the extend the Step class: ConditionalStep, InputInjectorStep, LoopOutputStep, TransferStep, Transformer
-from streamflow.cwl.utils import LoadListing, SecondaryFile
-from streamflow.cwl.step import (
-    CWLTransferStep,  # TransferStep
-    CWLConditionalStep,  # ConditionalStep
-    CWLInputInjectorStep,  # InputInjectorStep
-    CWLLoopOutputAllStep,  # LoopOutputStep
-    CWLLoopOutputLastStep,  # LoopOutputStep
+from streamflow.core.workflow import Step, Workflow
+from streamflow.cwl.combinator import ListMergeCombinator
+from streamflow.cwl.command import (
+    CWLCommand,
+    CWLCommandToken,
+    CWLExpressionCommand,
+    CWLMapCommandToken,
+    CWLObjectCommandToken,
+    CWLStepCommand,
+    CWLUnionCommandToken,
 )
-from streamflow.cwl.combinator import ListMergeCombinator  # CombinatorStep
 from streamflow.cwl.processor import (
-    CWLTokenProcessor,
+    CWLFileToken,
     CWLMapTokenProcessor,
     CWLObjectTokenProcessor,
+    CWLTokenProcessor,
     CWLUnionTokenProcessor,
-    CWLFileToken,
+)
+from streamflow.cwl.step import (
+    CWLConditionalStep,
+    CWLInputInjectorStep,
+    CWLLoopOutputAllStep,
+    CWLLoopOutputLastStep,
+    CWLTransferStep,
 )
 from streamflow.cwl.transformer import (
-    DefaultTransformer,
-    DefaultRetagTransformer,
-    CWLTokenTransformer,
-    ValueFromTransformer,
-    LoopValueFromTransformer,
     AllNonNullTransformer,
+    CWLTokenTransformer,
+    DefaultRetagTransformer,
+    DefaultTransformer,
     FirstNonNullTransformer,
     ForwardTransformer,
     ListToElementTransformer,
+    LoopValueFromTransformer,
     OnlyNonNullTransformer,
+    ValueFromTransformer,
 )
-from streamflow.cwl.command import (
-    CWLCommand,
-    CWLCommandToken,
-    CWLObjectCommandToken,
-    CWLExpressionCommand,
-    CWLStepCommand,
-    CWLUnionCommandToken,
-    CWLMapCommandToken,
-)
-
-
-def create_cwl_token_processor(name, workflow):
-    return CWLTokenProcessor(
-        name=name,
-        workflow=workflow,
-        token_type="enum",
-        enum_symbols=["path1", "path2"],
-        expression_lib=["expr_lib1", "expr_lib2"],
-        secondary_files=[SecondaryFile("file1", True)],
-        format_graph=Graph(),
-        load_listing=LoadListing.no_listing,
-    )
+from streamflow.cwl.utils import LoadListing, SecondaryFile
+from streamflow.workflow.step import CombinatorStep, ExecuteStep
+from tests.conftest import save_load_and_test
 
 
-def create_cwl_command(step, command_tokens):
+def _create_cwl_command(
+    step: Step, command_tokens: MutableSequence[CWLCommandToken]
+) -> CWLCommand:
     return CWLCommand(
         step=step,
         absolute_initial_workdir_allowed=False,
         base_command=["command", "tool"],
         command_tokens=command_tokens,
         expression_lib=["Requirement"],
         failure_codes=[0, 0],
@@ -81,28 +69,43 @@
         step_stderr=None,
         step_stdin=None,
         step_stdout=None,
         time_limit=1000,
     )
 
 
-def create_cwl_command_token(cls=CWLCommandToken, value=None):
+def _create_cwl_command_token(
+    cls: type[CWLCommandToken] = CWLCommandToken, value: Any | None = None
+):
     return cls(
         is_shell_command=False,
         item_separator="&",
         name="test",
         position=2,
         prefix="--test",
         separate=True,
         shell_quote=True,
         token_type="string",
         value=value,
     )
 
 
+def _create_cwl_token_processor(name: str, workflow: Workflow) -> CWLTokenProcessor:
+    return CWLTokenProcessor(
+        name=name,
+        workflow=workflow,
+        token_type="enum",
+        enum_symbols=["path1", "path2"],
+        expression_lib=["expr_lib1", "expr_lib2"],
+        secondary_files=[SecondaryFile("file1", True)],
+        format_graph=Graph(),
+        load_listing=LoadListing.no_listing,
+    )
+
+
 @pytest.mark.asyncio
 async def test_cwl_file_token(context: StreamFlowContext):
     """Test saving and loading CWLFileToken from database"""
     token = CWLFileToken(
         value={
             "location": "file:///home/ubuntu/output.txt",
             "basename": "output.txt",
@@ -122,15 +125,15 @@
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
-    step.command = create_cwl_command(step, [])
+    step.command = _create_cwl_command(step, [])
     await save_load_and_test(step, context)
 
 
 @pytest.mark.asyncio
 async def test_cwl_expression_command(context: StreamFlowContext):
     """Test saving and loading ExecuteStep with CWLExpressionCommand from database"""
     workflow = Workflow(
@@ -185,19 +188,19 @@
     )
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
 
-    step.command = create_cwl_command(
+    step.command = _create_cwl_command(
         step,
         [
-            create_cwl_command_token(value=DoubleQuotedScalarString("60")),
-            create_cwl_command_token(
+            _create_cwl_command_token(value=DoubleQuotedScalarString("60")),
+            _create_cwl_command_token(
                 value=LiteralScalarString("${ return 10 + 20 - (5 * 4) }")
             ),
         ],
     )
     await save_load_and_test(step, context)
 
 
@@ -209,19 +212,19 @@
     )
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
 
-    step.command = create_cwl_command(
+    step.command = _create_cwl_command(
         step,
         [
-            create_cwl_command_token(value=create_cwl_command_token(value=1123)),
-            create_cwl_command_token(value=create_cwl_command_token(value="hello")),
+            _create_cwl_command_token(value=_create_cwl_command_token(value=1123)),
+            _create_cwl_command_token(value=_create_cwl_command_token(value="hello")),
         ],
     )
     await save_load_and_test(step, context)
 
 
 @pytest.mark.asyncio
 async def test_cwl_object_command_token(context: StreamFlowContext):
@@ -230,22 +233,22 @@
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
-    step.command = create_cwl_command(
+    step.command = _create_cwl_command(
         step,
         [
-            create_cwl_command_token(
+            _create_cwl_command_token(
                 cls=CWLObjectCommandToken,
                 value={
-                    "a": create_cwl_command_token(value=10),
-                    "b": create_cwl_command_token(value=234),
+                    "a": _create_cwl_command_token(value=10),
+                    "b": _create_cwl_command_token(value=234),
                 },
             )
         ],
     )
     await save_load_and_test(step, context)
 
 
@@ -258,69 +261,65 @@
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
 
     command_tokens = [
-        create_cwl_command_token(
+        _create_cwl_command_token(
             cls=CWLObjectCommandToken,
-            # in CWL this structure is named record
-            # zero:
-            #   type: File
-            #   params: null
             value={
-                "zero": create_cwl_command_token(
+                "zero": _create_cwl_command_token(
                     cls=CWLObjectCommandToken,
                     value={
-                        "type": create_cwl_command_token(value="File"),
-                        "params": create_cwl_command_token(value=None),
+                        "type": _create_cwl_command_token(value="File"),
+                        "params": _create_cwl_command_token(value=None),
                     },
                 )
             },
         ),
-        create_cwl_command_token(
+        _create_cwl_command_token(
             cls=CWLObjectCommandToken,
             value={
-                "zero": create_cwl_command_token(
+                "zero": _create_cwl_command_token(
                     cls=CWLObjectCommandToken,
                     value={
-                        "one": create_cwl_command_token(value="89"),
-                        "two": create_cwl_command_token(value=29),
-                        "three": create_cwl_command_token(value=None),
+                        "one": _create_cwl_command_token(value="89"),
+                        "two": _create_cwl_command_token(value=29),
+                        "three": _create_cwl_command_token(value=None),
                     },
                 )
             },
         ),
-        create_cwl_command_token(value=11),
+        _create_cwl_command_token(value=11),
     ]
-    step.command = create_cwl_command(step, command_tokens)
+    step.command = _create_cwl_command(step, command_tokens)
     await save_load_and_test(step, context)
 
 
 @pytest.mark.asyncio
 async def test_cwl_union_command_token(context: StreamFlowContext):
     """Test saving and loading CWLCommannd with CWLUnionCommandTokens from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
-    step.command = create_cwl_command(
+    step.command = _create_cwl_command(
         step,
         [
-            create_cwl_command_token(
+            _create_cwl_command_token(
                 cls=CWLUnionCommandToken,
                 value=[
-                    create_cwl_command_token(value="qwerty"),
-                    create_cwl_command_token(value=987),
-                    create_cwl_command_token(value="qaz"),
+                    _create_cwl_command_token(value="qwerty"),
+                    _create_cwl_command_token(value=987),
+                    _create_cwl_command_token(value="qaz"),
                 ],
             )
         ],
     )
     await save_load_and_test(step, context)
 
 
@@ -331,32 +330,32 @@
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
-    step.command = create_cwl_command(
+    step.command = _create_cwl_command(
         step,
         [
-            create_cwl_command_token(
+            _create_cwl_command_token(
                 cls=CWLUnionCommandToken,
                 value=[
-                    create_cwl_command_token(
+                    _create_cwl_command_token(
                         cls=CWLUnionCommandToken,
                         value=[
-                            create_cwl_command_token(value="aaa"),
-                            create_cwl_command_token(value="bbb"),
+                            _create_cwl_command_token(value="aaa"),
+                            _create_cwl_command_token(value="bbb"),
                         ],
                     ),
-                    create_cwl_command_token(
+                    _create_cwl_command_token(
                         cls=CWLUnionCommandToken,
                         value=[
-                            create_cwl_command_token(value="ccc"),
-                            create_cwl_command_token(value="ddd"),
+                            _create_cwl_command_token(value="ccc"),
+                            _create_cwl_command_token(value="ddd"),
                         ],
                     ),
                 ],
             )
         ],
     )
     await save_load_and_test(step, context)
@@ -369,22 +368,22 @@
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
-    step.command = create_cwl_command(
+    step.command = _create_cwl_command(
         step,
         [
-            create_cwl_command_token(
-                cls=CWLMapCommandToken, value=create_cwl_command_token(value="z")
+            _create_cwl_command_token(
+                cls=CWLMapCommandToken, value=_create_cwl_command_token(value="z")
             ),
-            create_cwl_command_token(
-                cls=CWLMapCommandToken, value=create_cwl_command_token(value="xy")
+            _create_cwl_command_token(
+                cls=CWLMapCommandToken, value=_create_cwl_command_token(value="xy")
             ),
         ],
     )
     await save_load_and_test(step, context)
 
 
 @pytest.mark.asyncio
@@ -453,15 +452,15 @@
     await workflow.save(context)
 
     name = utils.random_name()
     transformer = workflow.create_step(
         cls=CWLTokenTransformer,
         name=name + "-transformer",
         port_name=port.name,
-        processor=create_cwl_token_processor(port.name, workflow),
+        processor=_create_cwl_token_processor(port.name, workflow),
     )
     await save_load_and_test(transformer, context)
 
 
 @pytest.mark.asyncio
 async def test_value_from_transformer(context: StreamFlowContext):
     """Test saving and loading ValueFromTransformer with CWLTokenProcessor from database"""
@@ -471,15 +470,15 @@
     port = workflow.create_port()
     await workflow.save(context)
 
     name = utils.random_name()
     transformer = workflow.create_step(
         cls=ValueFromTransformer,
         name=name + "-value-from-transformer",
-        processor=create_cwl_token_processor(port.name, workflow),
+        processor=_create_cwl_token_processor(port.name, workflow),
         port_name=port.name,
         expression_lib=True,
         full_js=False,
         value_from="$(1 + 1)",
     )
     await save_load_and_test(transformer, context)
 
@@ -493,15 +492,15 @@
     port = workflow.create_port()
     await workflow.save(context)
 
     name = utils.random_name()
     transformer = workflow.create_step(
         cls=LoopValueFromTransformer,
         name=name + "-loop-value-from-transformer",
-        processor=create_cwl_token_processor(port.name, workflow),
+        processor=_create_cwl_token_processor(port.name, workflow),
         port_name=port.name,
         expression_lib=True,
         full_js=False,
         value_from="$(1 + 1 == 0)",
     )
     await save_load_and_test(transformer, context)
 
@@ -519,15 +518,15 @@
     transformer = workflow.create_step(
         cls=CWLTokenTransformer,
         name=name + "-transformer",
         port_name=port.name,
         processor=CWLMapTokenProcessor(
             name=port.name,
             workflow=workflow,
-            processor=create_cwl_token_processor(port.name, workflow),
+            processor=_create_cwl_token_processor(port.name, workflow),
         ),
     )
     await save_load_and_test(transformer, context)
 
 
 @pytest.mark.asyncio
 async def test_cwl_object_token_transformer(context: StreamFlowContext):
@@ -543,15 +542,15 @@
         cls=CWLTokenTransformer,
         name=name + "-transformer",
         port_name=port.name,
         processor=CWLObjectTokenProcessor(
             name=port.name,
             workflow=workflow,
             processors={
-                utils.random_name(): create_cwl_token_processor(port.name, workflow)
+                utils.random_name(): _create_cwl_token_processor(port.name, workflow)
             },
         ),
     )
     await save_load_and_test(transformer, context)
 
 
 @pytest.mark.asyncio
@@ -567,15 +566,15 @@
     transformer = workflow.create_step(
         cls=CWLTokenTransformer,
         name=name + "-transformer",
         port_name=port.name,
         processor=CWLUnionTokenProcessor(
             name=port.name,
             workflow=workflow,
-            processors=[create_cwl_token_processor(port.name, workflow)],
+            processors=[_create_cwl_token_processor(port.name, workflow)],
         ),
     )
     await save_load_and_test(transformer, context)
 
 
 @pytest.mark.asyncio
 async def test_all_non_null_transformer(context: StreamFlowContext):
@@ -680,15 +679,15 @@
     )
     await workflow.save(context)
 
     step = workflow.create_step(
         cls=CWLConditionalStep,
         name=utils.random_name() + "-when",
         expression="$(inputs.name.length == 10)",
-        expression_lib=[],  # MutableSequence[Any]
+        expression_lib=[],
         full_js=True,
     )
     await save_load_and_test(step, context)
 
 
 @pytest.mark.asyncio
 async def test_transfer_step(context: StreamFlowContext):
```

### Comparing `streamflow-0.2.0.dev6/tests/test_persistence.py` & `streamflow-0.2.0.dev7/tests/test_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 import posixpath
 
 import pytest
 
-from tests.conftest import get_docker_deployment_config, save_load_and_test
-
 from streamflow.core import utils
-from streamflow.core.context import StreamFlowContext
 from streamflow.core.config import BindingConfig
-from streamflow.core.deployment import Target, LocalTarget
+from streamflow.core.context import StreamFlowContext
+from streamflow.core.deployment import LocalTarget, Target
 from streamflow.core.workflow import Job, Token, Workflow
-
-from streamflow.workflow.port import JobPort, ConnectorPort
+from streamflow.workflow.combinator import (
+    CartesianProductCombinator,
+    DotProductCombinator,
+    LoopCombinator,
+    LoopTerminationCombinator,
+)
+from streamflow.workflow.port import ConnectorPort, JobPort
 from streamflow.workflow.step import (
     CombinatorStep,
     DeployStep,
     ExecuteStep,
     GatherStep,
-    ScheduleStep,
-    ScatterStep,
     LoopCombinatorStep,
-)
-from streamflow.workflow.combinator import (
-    CartesianProductCombinator,
-    DotProductCombinator,
-    LoopCombinator,
-    LoopTerminationCombinator,
+    ScatterStep,
+    ScheduleStep,
 )
 from streamflow.workflow.token import (
+    IterationTerminationToken,
     JobToken,
     ListToken,
     ObjectToken,
     TerminationToken,
-    IterationTerminationToken,
 )
+from tests.conftest import get_docker_deployment_config, save_load_and_test
 
 
-# Testing Workflow
 @pytest.mark.asyncio
 async def test_workflow(context: StreamFlowContext):
     """Test saving and loading Workflow from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await save_load_and_test(workflow, context)
 
 
-# Testing Port and its extension classes
 @pytest.mark.asyncio
 async def test_port(context: StreamFlowContext):
     """Test saving and loading Port from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
@@ -75,15 +71,14 @@
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
     port = workflow.create_port(ConnectorPort)
     await save_load_and_test(port, context)
 
 
-# Testing Step and its extension classes
 @pytest.mark.asyncio
 async def test_combinator_step(context: StreamFlowContext):
     """Test saving and loading CombinatorStep with CartesianProductCombinator from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
@@ -196,15 +191,14 @@
     )
     await workflow.save(context)
 
     step = workflow.create_step(cls=ScatterStep, name=utils.random_name() + "-scatter")
     await save_load_and_test(step, context)
 
 
-# Subtest - Step param combinator
 @pytest.mark.asyncio
 async def test_dot_product_combinator(context: StreamFlowContext):
     """Test saving and loading CombinatorStep with DotProductCombinator from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
@@ -250,15 +244,14 @@
         combinator=LoopTerminationCombinator(
             name=utils.random_name(), workflow=workflow
         ),
     )
     await save_load_and_test(step, context)
 
 
-# Testing the Target and its extension classes
 @pytest.mark.asyncio
 async def test_target(context: StreamFlowContext):
     """Test saving and loading Target from database"""
     target = Target(
         deployment=get_docker_deployment_config(),
         service="test-persistence",
         workdir=utils.random_name(),
@@ -269,15 +262,14 @@
 @pytest.mark.asyncio
 async def test_local_target(context: StreamFlowContext):
     """Test saving and loading LocalTarget from database"""
     target = LocalTarget(workdir=utils.random_name())
     await save_load_and_test(target, context)
 
 
-# Testing the Token and its extension classes
 @pytest.mark.asyncio
 async def test_token(context: StreamFlowContext):
     """Test saving and loading Token from database"""
     token = Token(value=["test", "token"])
     await save_load_and_test(token, context)
 
 
@@ -321,13 +313,12 @@
 @pytest.mark.asyncio
 async def test_iteration_termination_token(context: StreamFlowContext):
     """Test saving and loading IterationTerminationToken from database"""
     token = IterationTerminationToken("1")
     await save_load_and_test(token, context)
 
 
-# Deployment test
 @pytest.mark.asyncio
 async def test_deployment(context: StreamFlowContext):
     """Test saving and loading deployment configuration from database"""
     config = get_docker_deployment_config()
     await save_load_and_test(config, context)
```

### Comparing `streamflow-0.2.0.dev6/tests/test_provenance.py` & `streamflow-0.2.0.dev7/tests/test_provenance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,268 +1,296 @@
+from __future__ import annotations
+
 import asyncio
 import posixpath
-from typing import MutableMapping, Any, MutableSequence
+from typing import Any, MutableMapping, MutableSequence, cast
 
 import pytest
 
+from streamflow.core import utils
+from streamflow.core.config import BindingConfig
+from streamflow.core.context import StreamFlowContext
+from streamflow.core.deployment import Target
+from streamflow.core.persistence import DatabaseLoadingContext
+from streamflow.core.workflow import Port, Status, Step, Token, Workflow
 from streamflow.cwl.command import CWLCommand, CWLCommandToken
 from streamflow.cwl.translator import _create_command_output_processor_base
 from streamflow.persistence.loading_context import DefaultDatabaseLoadingContext
 from streamflow.workflow.combinator import (
-    DotProductCombinator,
     CartesianProductCombinator,
+    DotProductCombinator,
     LoopCombinator,
     LoopTerminationCombinator,
 )
 from streamflow.workflow.executor import StreamFlowExecutor
-from tests.conftest import get_docker_deployment_config
-
-from streamflow.core import utils
-from streamflow.core.context import StreamFlowContext
-from streamflow.core.config import BindingConfig
-from streamflow.core.deployment import Target
-from streamflow.core.workflow import Token, Workflow, Status, Port, Step
-
 from streamflow.workflow.port import ConnectorPort
 from streamflow.workflow.step import (
+    CombinatorStep,
     DeployStep,
     ExecuteStep,
-    ScheduleStep,
-    ScatterStep,
     GatherStep,
-    CombinatorStep,
     LoopCombinatorStep,
+    ScatterStep,
+    ScheduleStep,
 )
-
 from streamflow.workflow.token import (
+    IterationTerminationToken,
     ListToken,
     TerminationToken,
-    IterationTerminationToken,
 )
+from tests.conftest import get_docker_deployment_config
 
 
-async def _put_tokens(token_list, in_port, context):
+def _contains_id(id_: int, token_list: MutableSequence[Token]) -> bool:
     for t in token_list:
-        if not isinstance(t, TerminationToken):
-            await t.save(context, in_port.persistent_id)
-        in_port.put(t)
-    in_port.put(TerminationToken())
+        if id_ == t.persistent_id:
+            return True
+    return False
+
+
+async def _load_dependees(
+    token_id: int, loading_context: DatabaseLoadingContext, context: StreamFlowContext
+) -> MutableSequence[Token]:
+    rows = await context.database.get_dependees(token_id)
+    return cast(
+        MutableSequence[Token],
+        await asyncio.gather(
+            *(
+                asyncio.create_task(
+                    loading_context.load_token(context, row["dependee"])
+                )
+                for row in rows
+            )
+        ),
+    )
+
+
+async def _load_dependers(
+    token_id: int, loading_context: DatabaseLoadingContext, context: StreamFlowContext
+) -> MutableSequence[Token]:
+    rows = await context.database.get_dependers(token_id)
+    return cast(
+        MutableSequence[Token],
+        await asyncio.gather(
+            *(
+                asyncio.create_task(
+                    loading_context.load_token(context, row["depender"])
+                )
+                for row in rows
+            )
+        ),
+    )
 
 
-async def _create_workflow(context: StreamFlowContext, num_port=2):
+def create_deploy_step(workflow, deployment_config=None):
+    connector_port = workflow.create_port(cls=ConnectorPort)
+    if not deployment_config:
+        deployment_config = get_docker_deployment_config()
+    return workflow.create_step(
+        cls=DeployStep,
+        name=posixpath.join("__deploy__", deployment_config.name),
+        deployment_config=deployment_config,
+        connector_port=connector_port,
+    )
+
+
+def create_schedule_step(workflow, deploy_step, binding_config=None):
+    if not binding_config:
+        binding_config = BindingConfig(
+            targets=[
+                Target(
+                    deployment=deploy_step.deployment_config,
+                    workdir=utils.random_name(),
+                )
+            ]
+        )
+    return workflow.create_step(
+        cls=ScheduleStep,
+        name=posixpath.join(utils.random_name(), "__schedule__"),
+        job_prefix="something",
+        connector_ports={
+            binding_config.targets[0].deployment.name: deploy_step.get_output_port()
+        },
+        binding_config=binding_config,
+    )
+
+
+async def create_workflow(
+    context: StreamFlowContext, num_port: int = 2
+) -> tuple[Workflow, tuple[Port]]:
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     ports = []
     for _ in range(num_port):
         ports.append(workflow.create_port())
     await workflow.save(context)
-    return workflow, *ports
+    return workflow, tuple(cast(MutableSequence[Port], ports))
 
 
-async def _general_test(
+async def general_test(
     context: StreamFlowContext,
     workflow: Workflow,
     in_port: Port,
     out_port: Port,
-    step_cls: Step,
-    kargs_step: MutableMapping[str, Any],
+    step_cls: type[Step],
+    kwargs_step: MutableMapping[str, Any],
     token_list: MutableSequence[Token],
     port_name: str = "test",
-):
+) -> Step:
     """ """
-    step = workflow.create_step(cls=step_cls, **kargs_step)
+    step = workflow.create_step(cls=step_cls, **kwargs_step)
     step.add_input_port(port_name, in_port)
     step.add_output_port(port_name, out_port)
 
-    await _put_tokens(token_list, in_port, context)
+    await put_tokens(token_list, in_port, context)
 
     await workflow.save(context)
     executor = StreamFlowExecutor(workflow)
     await executor.run()
     return step
 
 
-async def _load_dependees(token_id, loading_context, context):
-    rows = await context.database.get_dependees(token_id)
-    return await asyncio.gather(
-        *(
-            asyncio.create_task(loading_context.load_token(context, row["dependee"]))
-            for row in rows
-        )
-    )
-
-
-async def _load_dependers(token_id, loading_context, context):
-    rows = await context.database.get_dependers(token_id)
-    return await asyncio.gather(
-        *(
-            asyncio.create_task(loading_context.load_token(context, row["depender"]))
-            for row in rows
-        )
-    )
-
-
-def contains_id(id, token_list):
+async def put_tokens(
+    token_list: MutableSequence[Token], in_port: Port, context: StreamFlowContext
+) -> None:
     for t in token_list:
-        if id == t.persistent_id:
-            return True
-    return False
+        if not isinstance(t, TerminationToken):
+            await t.save(context, in_port.persistent_id)
+        in_port.put(t)
+    in_port.put(TerminationToken())
 
 
 async def verify_dependency_tokens(
-    token,
-    port,
-    expected_depender,
-    expected_dependee,
+    token: Token,
+    port: Port,
     context: StreamFlowContext,
-    alternative_expected_dependee=None,
+    expected_depender: MutableSequence[Token] | None = None,
+    expected_dependee: MutableSequence[Token] | None = None,
+    alternative_expected_dependee: MutableSequence[Token] | None = None,
 ):
     loading_context = DefaultDatabaseLoadingContext()
+    expected_depender = expected_depender or []
+    expected_dependee = expected_dependee or []
 
     token_reloaded = await context.database.get_token(token_id=token.persistent_id)
     assert token_reloaded["port"] == port.persistent_id
 
     depender_list = await _load_dependers(token.persistent_id, loading_context, context)
     print(
         "depender:",
         {token.persistent_id: [t.persistent_id for t in depender_list]},
     )
-    print("expected_depender", [t.persistent_id for t in expected_depender])
+    print(
+        "expected_depender",
+        [t.persistent_id for t in expected_depender],
+    )
     assert len(depender_list) == len(expected_depender)
     for t1 in depender_list:
-        assert contains_id(t1.persistent_id, expected_depender)
+        assert _contains_id(t1.persistent_id, expected_depender)
 
     dependee_list = await _load_dependees(token.persistent_id, loading_context, context)
     print(
         "dependee:",
         {token.persistent_id: [t.persistent_id for t in dependee_list]},
     )
-    print("expected_dependee", [t.persistent_id for t in expected_dependee])
+    print(
+        "expected_dependee",
+        [t.persistent_id for t in expected_dependee],
+    )
     try:
         assert len(dependee_list) == len(expected_dependee)
         for t1 in dependee_list:
-            assert contains_id(t1.persistent_id, expected_dependee)
+            assert _contains_id(t1.persistent_id, expected_dependee)
     except AssertionError as err:
         if alternative_expected_dependee is None:
             raise err
         else:
             assert len(dependee_list) == len(alternative_expected_dependee)
             for t1 in dependee_list:
-                assert contains_id(t1.persistent_id, alternative_expected_dependee)
-
-
-def _create_deploy_step(workflow, deployment_config=None):
-    connector_port = workflow.create_port(cls=ConnectorPort)
-    if not deployment_config:
-        deployment_config = get_docker_deployment_config()
-    return workflow.create_step(
-        cls=DeployStep,
-        name=posixpath.join("__deploy__", deployment_config.name),
-        deployment_config=deployment_config,
-        connector_port=connector_port,
-    )
-
-
-def _create_schedule_step(workflow, deploy_step, binding_config=None):
-    if not binding_config:
-        binding_config = BindingConfig(
-            targets=[
-                Target(
-                    deployment=deploy_step.deployment_config,
-                    workdir=utils.random_name(),
-                )
-            ]
-        )
-    return workflow.create_step(
-        cls=ScheduleStep,
-        name=posixpath.join(utils.random_name(), "__schedule__"),
-        job_prefix="something",
-        connector_ports={
-            binding_config.targets[0].deployment.name: deploy_step.get_output_port()
-        },
-        binding_config=binding_config,
-    )
+                assert _contains_id(t1.persistent_id, alternative_expected_dependee)
 
 
 @pytest.mark.asyncio
 async def test_scatter_step(context: StreamFlowContext):
-    """ """
-    workflow, in_port, out_port = await _create_workflow(context)
+    """Test token provenance for ScatterStep"""
+    workflow, (in_port, out_port) = await create_workflow(context)
     token_list = [ListToken([Token("a"), Token("b"), Token("c")])]
-    await _general_test(
-        context,
-        workflow,
-        in_port,
-        out_port,
-        ScatterStep,
-        {"name": utils.random_name() + "-scatter"},
-        token_list,
+    await general_test(
+        context=context,
+        workflow=workflow,
+        in_port=in_port,
+        out_port=out_port,
+        step_cls=ScatterStep,
+        kwargs_step={"name": utils.random_name() + "-scatter"},
+        token_list=token_list,
     )
     assert len(out_port.token_list) == 4
     for curr_token in out_port.token_list[:-1]:
         await verify_dependency_tokens(
-            curr_token, out_port, (), [in_port.token_list[0]], context
+            token=curr_token,
+            port=out_port,
+            context=context,
+            expected_dependee=[in_port.token_list[0]],
         )
 
 
 @pytest.mark.asyncio
 async def test_deploy_step(context: StreamFlowContext):
-    """ """
-    workflow = (await _create_workflow(context, num_port=0))[0]
-    step = _create_deploy_step(workflow)
+    """Test token provenance for DeployStep"""
+    workflow = (await create_workflow(context, num_port=0))[0]
+    step = create_deploy_step(workflow)
 
     await workflow.save(context)
     executor = StreamFlowExecutor(workflow)
     await executor.run()
 
-    # len(token_list) = N output tokens + 1 termination token
     assert len(step.get_output_port().token_list) == 2
     await verify_dependency_tokens(
-        step.get_output_port().token_list[0], step.get_output_port(), (), (), context
+        token=step.get_output_port().token_list[0],
+        port=step.get_output_port(),
+        context=context,
     )
 
 
 @pytest.mark.asyncio
 async def test_schedule_step(context: StreamFlowContext):
-    """ """
-    workflow = (await _create_workflow(context, num_port=0))[0]
-    deploy_step = _create_deploy_step(workflow)
-    schedule_step = _create_schedule_step(workflow, deploy_step)
+    """Test token provenance for ScheduleStep"""
+    workflow = (await create_workflow(context, num_port=0))[0]
+    deploy_step = create_deploy_step(workflow)
+    schedule_step = create_schedule_step(workflow, deploy_step)
 
     await workflow.save(context)
     executor = StreamFlowExecutor(workflow)
     await executor.run()
     job_token = schedule_step.get_output_port("__job__").token_list[0]
     await context.scheduler.notify_status(job_token.value.name, Status.COMPLETED)
 
     await verify_dependency_tokens(
-        deploy_step.get_output_port().token_list[0],
-        deploy_step.get_output_port(),
-        [job_token],
-        [],
-        context,
+        token=deploy_step.get_output_port().token_list[0],
+        port=deploy_step.get_output_port(),
+        context=context,
+        expected_depender=[job_token],
     )
     await verify_dependency_tokens(
-        job_token,
-        schedule_step.get_output_port("__job__"),
-        [],
-        [deploy_step.get_output_port().token_list[0]],
-        context,
+        token=job_token,
+        port=schedule_step.get_output_port("__job__"),
+        context=context,
+        expected_dependee=[deploy_step.get_output_port().token_list[0]],
     )
 
 
 @pytest.mark.asyncio
 async def test_execute_step(context: StreamFlowContext):
-    """ """
-    workflow, in_port_schedule, in_port, out_port = await _create_workflow(
+    """Test token provenance for ExecuteStep"""
+    workflow, (in_port_schedule, in_port, out_port) = await create_workflow(
         context, num_port=3
     )
-    deploy_step = _create_deploy_step(workflow)
-    schedule_step = _create_schedule_step(workflow, deploy_step)
+    deploy_step = create_deploy_step(workflow)
+    schedule_step = create_schedule_step(workflow, deploy_step)
 
     in_port_name = "in-1"
     out_port_name = "out-1"
     token_value = "Hello"
 
     execute_step = workflow.create_step(
         cls=ExecuteStep,
@@ -285,64 +313,66 @@
             {},
             {"hints": {}, "requirements": {}},
         ),
     )
     token_list = [Token(token_value)]
 
     execute_step.add_input_port(in_port_name, in_port)
-    await _put_tokens(token_list, in_port, context)
+    await put_tokens(token_list, in_port, context)
 
     schedule_step.add_input_port(in_port_name, in_port_schedule)
-    await _put_tokens(token_list, in_port_schedule, context)
+    await put_tokens(token_list, in_port_schedule, context)
 
     await workflow.save(context)
     executor = StreamFlowExecutor(workflow)
     await executor.run()
 
     job_token = execute_step.get_input_port("__job__").token_list[0]
     await verify_dependency_tokens(
-        job_token,
-        execute_step.get_input_port("__job__"),
-        [execute_step.get_output_port(out_port_name).token_list[0]],
-        [deploy_step.get_output_port().token_list[0], token_list[0]],
-        context,
+        token=job_token,
+        port=execute_step.get_input_port("__job__"),
+        context=context,
+        expected_depender=[execute_step.get_output_port(out_port_name).token_list[0]],
+        expected_dependee=[deploy_step.get_output_port().token_list[0], token_list[0]],
     )
     await verify_dependency_tokens(
-        execute_step.get_output_port(out_port_name).token_list[0],
-        execute_step.get_output_port(out_port_name),
-        [],
-        list(job_token.value.inputs.values()) + [job_token],
-        context,
+        token=execute_step.get_output_port(out_port_name).token_list[0],
+        port=execute_step.get_output_port(out_port_name),
+        context=context,
+        expected_dependee=list(job_token.value.inputs.values()) + [job_token],
     )
 
 
 @pytest.mark.asyncio
 async def test_gather_step(context: StreamFlowContext):
-    """ """
-    workflow, in_port, out_port = await _create_workflow(context)
+    """Test token provenance for GatherStep"""
+    workflow, (in_port, out_port) = await create_workflow(context)
     token_list = [Token(i) for i in range(3)]
-    await _general_test(
-        context,
-        workflow,
-        in_port,
-        out_port,
-        GatherStep,
-        {"name": utils.random_name() + "-gather"},
-        token_list,
+    await general_test(
+        context=context,
+        workflow=workflow,
+        in_port=in_port,
+        out_port=out_port,
+        step_cls=GatherStep,
+        kwargs_step={"name": utils.random_name() + "-gather"},
+        token_list=token_list,
     )
     assert len(out_port.token_list) == 2
     await verify_dependency_tokens(
-        out_port.token_list[0], out_port, (), token_list, context
+        token=out_port.token_list[0],
+        port=out_port,
+        context=context,
+        expected_dependee=token_list,
     )
 
 
 @pytest.mark.asyncio
 async def test_combinator_step_dot_product(context: StreamFlowContext):
-    """ """
-    workflow, in_port, out_port, in_port_2, out_port_2 = await _create_workflow(
+    """Test token provenance for DotProductCombinator"""
+    workflow, (in_port, out_port, in_port_2, out_port_2) = await create_workflow(
         context, num_port=4
     )
     step = workflow.create_step(
         cls=CombinatorStep,
         name=utils.random_name() + "-combinator",
         combinator=DotProductCombinator(name=utils.random_name(), workflow=workflow),
     )
@@ -352,39 +382,45 @@
 
     port_name_2 = f"{port_name}_2"
     step.add_input_port(port_name_2, in_port_2)
     step.add_output_port(port_name_2, out_port_2)
 
     await workflow.save(context)
     list_token = ListToken([Token("fst"), Token("snd")])
-    await _put_tokens([list_token], in_port, context)
+    await put_tokens([list_token], in_port, context)
     step.combinator.add_item(port_name)
 
     tt = Token("4")
-    await _put_tokens([tt], in_port_2, context)
+    await put_tokens([tt], in_port_2, context)
     step.combinator.add_item(port_name_2)
 
     await workflow.save(context)
     executor = StreamFlowExecutor(workflow)
     await executor.run()
 
     assert len(out_port.token_list) == 2
     await verify_dependency_tokens(
-        out_port.token_list[0], out_port, [], [list_token, tt], context
+        token=out_port.token_list[0],
+        port=out_port,
+        context=context,
+        expected_dependee=[list_token, tt],
     )
     assert len(out_port_2.token_list) == 2
     await verify_dependency_tokens(
-        out_port_2.token_list[0], out_port_2, [], [list_token, tt], context
+        token=out_port_2.token_list[0],
+        port=out_port_2,
+        context=context,
+        expected_dependee=[list_token, tt],
     )
 
 
 @pytest.mark.asyncio
 async def test_combinator_step_cartesian_product(context: StreamFlowContext):
-    """ """
-    workflow, in_port, out_port, in_port_2, out_port_2 = await _create_workflow(
+    """Test token provenance for CartesianProductCombinator"""
+    workflow, (in_port, out_port, in_port_2, out_port_2) = await create_workflow(
         context, num_port=4
     )
     step = workflow.create_step(
         cls=CombinatorStep,
         name=utils.random_name() + "-combinator",
         combinator=CartesianProductCombinator(
             name=utils.random_name(), workflow=workflow
@@ -396,44 +432,46 @@
 
     port_name_2 = f"{port_name}_2"
     step.add_input_port(port_name_2, in_port_2)
     step.add_output_port(port_name_2, out_port_2)
 
     await workflow.save(context)
     token_list = [ListToken([Token("a"), Token("b")])]
-    await _put_tokens(token_list, in_port, context)
+    await put_tokens(token_list, in_port, context)
     step.combinator.add_item(port_name)
 
     token_list_2 = [Token("4")]
-    await _put_tokens(token_list_2, in_port_2, context)
+    await put_tokens(token_list_2, in_port_2, context)
     step.combinator.add_item(port_name_2)
 
     await workflow.save(context)
     executor = StreamFlowExecutor(workflow)
     await executor.run()
 
     assert len(out_port.token_list) == 2
     await verify_dependency_tokens(
-        out_port.token_list[0], out_port, [], [token_list[0], token_list_2[0]], context
+        token=out_port.token_list[0],
+        port=out_port,
+        context=context,
+        expected_dependee=[token_list[0], token_list_2[0]],
     )
 
     assert len(out_port_2.token_list) == 2
     await verify_dependency_tokens(
-        out_port_2.token_list[0],
-        out_port_2,
-        [],
-        [token_list[0], token_list_2[0]],
-        context,
+        token=out_port_2.token_list[0],
+        port=out_port_2,
+        context=context,
+        expected_dependee=[token_list[0], token_list_2[0]],
     )
 
 
 @pytest.mark.asyncio
 async def test_loop_combinator_step(context: StreamFlowContext):
-    """ """
-    workflow, in_port, out_port, in_port_2, out_port_2 = await _create_workflow(
+    """Test token provenance for LoopCombinator"""
+    workflow, (in_port, out_port, in_port_2, out_port_2) = await create_workflow(
         context, num_port=4
     )
     name = utils.random_name()
     step = workflow.create_step(
         cls=LoopCombinatorStep,
         name=name + "-combinator",
         combinator=LoopCombinator(name=name, workflow=workflow),
@@ -448,35 +486,38 @@
 
     await workflow.save(context)
     tag = "0.0"
     token_list = [
         ListToken([Token("a"), Token("b")], tag=tag),
         IterationTerminationToken(tag),
     ]
-    await _put_tokens(token_list, in_port, context)
+    await put_tokens(token_list, in_port, context)
     step.combinator.add_item(port_name)
 
     token_list_2 = [Token("4", tag=tag), IterationTerminationToken(tag=tag)]
-    await _put_tokens(token_list_2, in_port_2, context)
+    await put_tokens(token_list_2, in_port_2, context)
     step.combinator.add_item(port_name_2)
 
     await workflow.save(context)
     executor = StreamFlowExecutor(workflow)
     await executor.run()
 
     assert len(out_port.token_list) == 2
     await verify_dependency_tokens(
-        out_port.token_list[0], out_port, [], [token_list[0], token_list_2[0]], context
+        token=out_port.token_list[0],
+        port=out_port,
+        context=context,
+        expected_dependee=[token_list[0], token_list_2[0]],
     )
 
 
 @pytest.mark.asyncio
 async def test_loop_termination_combinator(context: StreamFlowContext):
-    """ """
-    workflow, in_port, out_port = await _create_workflow(context, num_port=2)
+    """Test token provenance for LoopTerminationCombinator"""
+    workflow, (in_port, out_port) = await create_workflow(context, num_port=2)
     step_name = utils.random_name()
     loop_terminator_combinator = LoopTerminationCombinator(
         workflow=workflow, name=step_name + "-loop-termination-combinator"
     )
     loop_terminator_step = workflow.create_step(
         cls=CombinatorStep,
         name=step_name + "-loop-terminator",
@@ -488,151 +529,21 @@
     loop_terminator_combinator.add_output_item(port_name)
     loop_terminator_combinator.add_item(port_name)
 
     list_token = [
         ListToken([Token("a"), Token("b")], tag="0.0"),
         ListToken([Token("c"), Token("d")], tag="0.1"),
     ]
-    await _put_tokens(list_token, in_port, context)
+    await put_tokens(list_token, in_port, context)
 
     await workflow.save(context)
     executor = StreamFlowExecutor(workflow)
     await executor.run()
 
     assert len(out_port.token_list) == 3
     for out_token, in_token in zip(out_port.token_list[:-1], list_token):
-        await verify_dependency_tokens(out_token, out_port, [], [in_token], context)
-
-
-@pytest.mark.asyncio
-async def test_nested_crossproduct_combinator(context: StreamFlowContext):
-    """ """
-    workflow, in_port_1, in_port_2, out_port_1, out_port_2 = await _create_workflow(
-        context, num_port=4
-    )
-    port_name_1 = "echo_in1"
-    port_name_2 = "echo_in2"
-    prefix_name = "/step1-scatter"
-    step_name = prefix_name + "-combinator"
-    combinator = DotProductCombinator(
-        workflow=workflow, name=prefix_name + "-dot-product-combinator"
-    )
-    c1 = CartesianProductCombinator(name=step_name, workflow=workflow)
-    c1.add_item(port_name_1)
-    c1.add_item(port_name_2)
-    items = c1.get_items(False)
-    combinator.add_combinator(
-        c1,
-        items,
-    )
-
-    step = workflow.create_step(
-        cls=CombinatorStep,
-        name=step_name,
-        combinator=combinator,
-    )
-
-    step.add_input_port(port_name_1, in_port_1)
-    step.add_input_port(port_name_2, in_port_2)
-    step.add_output_port(port_name_1, out_port_1)
-    step.add_output_port(port_name_2, out_port_2)
-
-    list_token_1 = [
-        ListToken([Token("a"), Token("b")], tag="0.0"),
-        ListToken([Token("c"), Token("d")], tag="0.1"),
-    ]
-    await _put_tokens(list_token_1, in_port_1, context)
-
-    list_token_2 = [
-        ListToken([Token("1"), Token("2")], tag="0.0"),
-        ListToken([Token("3"), Token("4")], tag="0.1"),
-    ]
-    await _put_tokens(list_token_2, in_port_2, context)
-
-    await workflow.save(context)
-    executor = StreamFlowExecutor(workflow)
-    await executor.run()
-
-    nested_crossproduct_1 = [(t1, t2) for t2 in list_token_2 for t1 in list_token_1]
-    nested_crossproduct_2 = [(t1, t2) for t1 in list_token_1 for t2 in list_token_2]
-
-    for t in list_token_1:
-        print(f"{t.persistent_id}, {t.tag}, {[tt.value for tt in t.value]}")
-
-    for t in list_token_2:
-        print(f"{t.persistent_id}, {t.tag}, {[tt.value for tt in t.value]}")
-    print()
-
-    for out_token in out_port_1.token_list[:-1]:
-        print(
-            f"{out_token.persistent_id}, {out_token.tag}, {[tt.value for tt in out_token.value]}"
-        )
-    for out_token in out_port_2.token_list[:-1]:
-        print(
-            f"{out_token.persistent_id}, {out_token.tag}, {[tt.value for tt in out_token.value]}"
-        )
-    print()
-    # The tokens id produced by combinators depend on the order of input tokens.
-    # The use of the alternative_expected_dependee parameter is necessary
-    # For example:
-    # input port_1 token: (id, tag, value)
-    #   (  3, 0.0, ['a', 'b'] )
-    #   (  6, 0.1, ['c', 'd'] )
-    # input port_2 token: (id, tag, value)
-    #   (  9, 0.0, ['1', '2'] )
-    #   ( 12, 0.1, ['3', '4'] )
-
-    # case #1: port_1 input tokens arrive first
-    # - output port_1 token: (id, tag, value)
-    #   ( 13, 0.0.0, ['a', 'b'] )
-    #   ( 15, 0.0.1, ['a', 'b'] )
-    #   ( 17, 0.1.0, ['c', 'd'] )
-    #   ( 19, 0.1.1, ['c', 'd'] )
-    # - output port_2 token: (id, tag, value)
-    #   ( 14, 0.0.0, ['1', '2'] )
-    #   ( 16, 0.0.1, ['3', '4'] )
-    #   ( 18, 0.1.0, ['1', '2'] )
-    #   ( 20, 0.1.1, ['3', '4'] )
-    # - provenance token in port_1: { output token id : input token id list }
-    #   { 13 : [3, 9], 15 : [3, 12], 17 : [6, 9], 19 : [6, 12] }
-    # - provenance token in port_2: { output token id : input token id list }
-    #   { 14 : [3, 9], 16 : [3, 12], 18 : [6, 9], 20 : [6, 12] }
-
-    # case #2: port_2 input tokens arrive first
-    # - output port_1 token: (id, tag, value)
-    #   ( 13, 0.0.0, ['a', 'b'] )
-    #   ( 15, 0.1.0, ['c', 'd'] )
-    #   ( 17, 0.0.1, ['a', 'b'] )
-    #   ( 19, 0.1.1, ['c', 'd'] )
-    # - output port_2 token: (id, tag, value)
-    #   ( 14, 0.0.0, ['1', '2'] )
-    #   ( 16, 0.1.0, ['1', '2'] )
-    #   ( 18, 0.0.1, ['3', '4'] )
-    #   ( 20, 0.1.1, ['3', '4'] )
-    # - provenance token in port_1: { output token id : input token id list }
-    #   { 13 : [3, 9], 15 : [6, 9], 17 : [3, 12], 19 : [6, 12] }
-    # - provenance token in port_2: { output token id : input token id list }
-    #   { 14 : [3, 9], 16 : [6, 9], 18 : [3, 12], 20 : [6, 12] }
-
-    # check port_1 outputs
-    assert len(out_port_1.token_list) == 5
-    for i, out_token in enumerate(out_port_1.token_list[:-1]):
-        await verify_dependency_tokens(
-            out_token,
-            out_port_1,
-            [],
-            nested_crossproduct_1[i],
-            context,
-            alternative_expected_dependee=nested_crossproduct_2[i],
-        )
-
-    # check port_2 outputs
-    assert len(out_port_2.token_list) == 5
-    for i, out_token in enumerate(out_port_2.token_list[:-1]):
         await verify_dependency_tokens(
-            out_token,
-            out_port_2,
-            [],
-            nested_crossproduct_1[i],
-            context,
-            alternative_expected_dependee=nested_crossproduct_2[i],
+            token=out_token,
+            port=out_port,
+            context=context,
+            expected_dependee=[in_token],
         )
```

### Comparing `streamflow-0.2.0.dev6/tests/test_remotepath.py` & `streamflow-0.2.0.dev7/tests/test_remotepath.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/tests/test_scheduler.py` & `streamflow-0.2.0.dev7/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev6/tests/test_transfer.py` & `streamflow-0.2.0.dev7/tests/test_transfer.py`

 * *Files identical despite different names*

