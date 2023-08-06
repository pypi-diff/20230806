# Comparing `tmp/beet-0.90.0.tar.gz` & `tmp/beet-0.91.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beet-0.90.0.tar", max compression
+gzip compressed data, was "beet-0.91.0.tar", max compression
```

## Comparing `beet-0.90.0.tar` & `beet-0.91.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     1073 2023-08-06 11:17:07.932692 beet-0.90.0/LICENSE
--rw-r--r--   0        0        0     6048 2023-08-06 11:17:07.932692 beet-0.90.0/README.md
--rw-r--r--   0        0        0      584 2023-08-06 11:17:40.085051 beet-0.90.0/beet/__init__.py
--rw-r--r--   0        0        0       44 2023-08-06 11:17:07.932692 beet-0.90.0/beet/__main__.py
--rw-r--r--   0        0        0        0 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/__init__.py
--rw-r--r--   0        0        0     3265 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/auto_yaml.py
--rw-r--r--   0        0        0     1369 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/autosave.py
--rw-r--r--   0        0        0     2480 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/babelbox.py
--rw-r--r--   0        0        0      574 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/clear.py
--rw-r--r--   0        0        0     3005 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/copy_files.py
--rw-r--r--   0        0        0     8040 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/dbg.py
--rw-r--r--   0        0        0      187 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/default.py
--rw-r--r--   0        0        0     1605 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/dundervar.py
--rw-r--r--   0        0        0     1046 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/extra_files.py
--rw-r--r--   0        0        0     3967 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/find_replace.py
--rw-r--r--   0        0        0     1472 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/format_json.py
--rw-r--r--   0        0        0      909 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/function_header.py
--rw-r--r--   0        0        0     5701 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/hangman.py
--rw-r--r--   0        0        0     1932 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/inline_function.py
--rw-r--r--   0        0        0     1090 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/inline_function_tag.py
--rw-r--r--   0        0        0     3811 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/installation_advancement.py
--rw-r--r--   0        0        0     1771 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/json_log.py
--rw-r--r--   0        0        0     5360 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/json_reporter.py
--rw-r--r--   0        0        0     2871 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/lantern_load.py
--rw-r--r--   0        0        0      816 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/line_endings.py
--rw-r--r--   0        0        0     5916 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/link.py
--rw-r--r--   0        0        0     6740 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/livereload.py
--rw-r--r--   0        0        0     1742 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/load.py
--rw-r--r--   0        0        0     4228 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/load_yaml.py
--rw-r--r--   0        0        0      512 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/log_level.py
--rw-r--r--   0        0        0     1587 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/messages.py
--rw-r--r--   0        0        0      338 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/minify_function.py
--rw-r--r--   0        0        0      235 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/minify_json.py
--rw-r--r--   0        0        0     1590 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/model_merging.py
--rw-r--r--   0        0        0     1591 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/optifine.py
--rw-r--r--   0        0        0      960 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/output.py
--rw-r--r--   0        0        0      959 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/relative_function_path.py
--rw-r--r--   0        0        0     5219 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/rename_files.py
--rw-r--r--   0        0        0     1503 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/render.py
--rw-r--r--   0        0        0      882 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/sandstone.py
--rw-r--r--   0        0        0      889 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/scoreboard.py
--rw-r--r--   0        0        0      811 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/stdin.py
--rw-r--r--   0        0        0     1357 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/strip_final_newlines.py
--rw-r--r--   0        0        0      155 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/template_context.py
--rw-r--r--   0        0        0      229 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/template_sandbox.py
--rw-r--r--   0        0        0      897 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/text_encoding.py
--rw-r--r--   0        0        0      775 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/unknown_files.py
--rw-r--r--   0        0        0     7395 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/vanilla.py
--rw-r--r--   0        0        0     5719 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/worldgen.py
--rw-r--r--   0        0        0     2436 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/yellow_shulker_box.py
--rw-r--r--   0        0        0        0 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/__init__.py
--rw-r--r--   0        0        0    11434 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/cache.py
--rw-r--r--   0        0        0     5906 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/container.py
--rw-r--r--   0        0        0      565 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/error.py
--rw-r--r--   0        0        0    20025 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/file.py
--rw-r--r--   0        0        0     8241 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/utils.py
--rw-r--r--   0        0        0     3711 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/watch.py
--rw-r--r--   0        0        0        0 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/__init__.py
--rw-r--r--   0        0        0    40084 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/base.py
--rw-r--r--   0        0        0    11711 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/data_pack.py
--rw-r--r--   0        0        0    11939 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/resource_pack.py
--rw-r--r--   0        0        0      529 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/test_utils.py
--rw-r--r--   0        0        0      660 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/utils.py
--rw-r--r--   0        0        0       33 2023-08-06 11:17:07.936693 beet-0.90.0/beet/preset_stdin.yml
--rw-r--r--   0        0        0        0 2023-08-06 11:17:07.936693 beet-0.90.0/beet/py.typed
--rw-r--r--   0        0        0     4266 2023-08-06 11:17:07.936693 beet-0.90.0/beet/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/__init__.py
--rw-r--r--   0        0        0     8017 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/cli.py
--rw-r--r--   0        0        0     4600 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/commands.py
--rw-r--r--   0        0        0    14000 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/config.py
--rw-r--r--   0        0        0    11226 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/context.py
--rw-r--r--   0        0        0    11080 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/generator.py
--rw-r--r--   0        0        0     3484 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/helpers.py
--rw-r--r--   0        0        0     4355 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/pipeline.py
--rw-r--r--   0        0        0    13374 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/project.py
--rw-r--r--   0        0        0     6812 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/select.py
--rw-r--r--   0        0        0     6457 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/template.py
--rw-r--r--   0        0        0     3694 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/tree.py
--rw-r--r--   0        0        0     4636 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/utils.py
--rw-r--r--   0        0        0     9695 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/worker.py
--rw-r--r--   0        0        0     2277 2023-08-06 11:17:40.149052 beet-0.90.0/pyproject.toml
--rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 beet-0.90.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-06 12:25:17.397406 beet-0.91.0/LICENSE
+-rw-r--r--   0        0        0     6048 2023-08-06 12:25:17.397406 beet-0.91.0/README.md
+-rw-r--r--   0        0        0      584 2023-08-06 12:25:48.701705 beet-0.91.0/beet/__init__.py
+-rw-r--r--   0        0        0       44 2023-08-06 12:25:17.397406 beet-0.91.0/beet/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/__init__.py
+-rw-r--r--   0        0        0     3265 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/auto_yaml.py
+-rw-r--r--   0        0        0     1369 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/autosave.py
+-rw-r--r--   0        0        0     2480 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/babelbox.py
+-rw-r--r--   0        0        0      574 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/clear.py
+-rw-r--r--   0        0        0     3005 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/copy_files.py
+-rw-r--r--   0        0        0     8040 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/dbg.py
+-rw-r--r--   0        0        0      187 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/default.py
+-rw-r--r--   0        0        0     1605 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/dundervar.py
+-rw-r--r--   0        0        0     1046 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/extra_files.py
+-rw-r--r--   0        0        0     3967 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/find_replace.py
+-rw-r--r--   0        0        0     1472 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/format_json.py
+-rw-r--r--   0        0        0      909 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/function_header.py
+-rw-r--r--   0        0        0     5701 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/hangman.py
+-rw-r--r--   0        0        0     1932 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/inline_function.py
+-rw-r--r--   0        0        0     1090 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/inline_function_tag.py
+-rw-r--r--   0        0        0     3811 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/installation_advancement.py
+-rw-r--r--   0        0        0     1771 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/json_log.py
+-rw-r--r--   0        0        0     5360 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/json_reporter.py
+-rw-r--r--   0        0        0     2871 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/lantern_load.py
+-rw-r--r--   0        0        0      816 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/line_endings.py
+-rw-r--r--   0        0        0     5916 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/link.py
+-rw-r--r--   0        0        0     6740 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/livereload.py
+-rw-r--r--   0        0        0     1742 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/load.py
+-rw-r--r--   0        0        0     4228 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/load_yaml.py
+-rw-r--r--   0        0        0      512 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/log_level.py
+-rw-r--r--   0        0        0     1587 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/messages.py
+-rw-r--r--   0        0        0      338 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/minify_function.py
+-rw-r--r--   0        0        0      235 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/minify_json.py
+-rw-r--r--   0        0        0     1590 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/model_merging.py
+-rw-r--r--   0        0        0     1591 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/optifine.py
+-rw-r--r--   0        0        0      960 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/output.py
+-rw-r--r--   0        0        0      959 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/relative_function_path.py
+-rw-r--r--   0        0        0     5219 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/rename_files.py
+-rw-r--r--   0        0        0     1675 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/render.py
+-rw-r--r--   0        0        0      882 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/sandstone.py
+-rw-r--r--   0        0        0      889 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/scoreboard.py
+-rw-r--r--   0        0        0      811 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/stdin.py
+-rw-r--r--   0        0        0     1357 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/strip_final_newlines.py
+-rw-r--r--   0        0        0      155 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/template_context.py
+-rw-r--r--   0        0        0      229 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/template_sandbox.py
+-rw-r--r--   0        0        0      897 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/text_encoding.py
+-rw-r--r--   0        0        0      775 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/unknown_files.py
+-rw-r--r--   0        0        0     7395 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/vanilla.py
+-rw-r--r--   0        0        0     5719 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/worldgen.py
+-rw-r--r--   0        0        0     2436 2023-08-06 12:25:17.397406 beet-0.91.0/beet/contrib/yellow_shulker_box.py
+-rw-r--r--   0        0        0        0 2023-08-06 12:25:17.397406 beet-0.91.0/beet/core/__init__.py
+-rw-r--r--   0        0        0    11434 2023-08-06 12:25:17.397406 beet-0.91.0/beet/core/cache.py
+-rw-r--r--   0        0        0     5906 2023-08-06 12:25:17.401406 beet-0.91.0/beet/core/container.py
+-rw-r--r--   0        0        0      565 2023-08-06 12:25:17.401406 beet-0.91.0/beet/core/error.py
+-rw-r--r--   0        0        0    20025 2023-08-06 12:25:17.401406 beet-0.91.0/beet/core/file.py
+-rw-r--r--   0        0        0     8241 2023-08-06 12:25:17.401406 beet-0.91.0/beet/core/utils.py
+-rw-r--r--   0        0        0     3711 2023-08-06 12:25:17.401406 beet-0.91.0/beet/core/watch.py
+-rw-r--r--   0        0        0        0 2023-08-06 12:25:17.401406 beet-0.91.0/beet/library/__init__.py
+-rw-r--r--   0        0        0    40084 2023-08-06 12:25:17.401406 beet-0.91.0/beet/library/base.py
+-rw-r--r--   0        0        0    11711 2023-08-06 12:25:17.401406 beet-0.91.0/beet/library/data_pack.py
+-rw-r--r--   0        0        0    11939 2023-08-06 12:25:17.401406 beet-0.91.0/beet/library/resource_pack.py
+-rw-r--r--   0        0        0      529 2023-08-06 12:25:17.401406 beet-0.91.0/beet/library/test_utils.py
+-rw-r--r--   0        0        0      660 2023-08-06 12:25:17.401406 beet-0.91.0/beet/library/utils.py
+-rw-r--r--   0        0        0       33 2023-08-06 12:25:17.401406 beet-0.91.0/beet/preset_stdin.yml
+-rw-r--r--   0        0        0        0 2023-08-06 12:25:17.401406 beet-0.91.0/beet/py.typed
+-rw-r--r--   0        0        0     4266 2023-08-06 12:25:17.401406 beet-0.91.0/beet/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/__init__.py
+-rw-r--r--   0        0        0     8017 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/cli.py
+-rw-r--r--   0        0        0     4600 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/commands.py
+-rw-r--r--   0        0        0    14000 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/config.py
+-rw-r--r--   0        0        0    11226 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/context.py
+-rw-r--r--   0        0        0    11080 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/generator.py
+-rw-r--r--   0        0        0     3484 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/helpers.py
+-rw-r--r--   0        0        0     4355 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/pipeline.py
+-rw-r--r--   0        0        0    13374 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/project.py
+-rw-r--r--   0        0        0     6812 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/select.py
+-rw-r--r--   0        0        0     6457 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/template.py
+-rw-r--r--   0        0        0     3694 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/tree.py
+-rw-r--r--   0        0        0     4636 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/utils.py
+-rw-r--r--   0        0        0     9695 2023-08-06 12:25:17.401406 beet-0.91.0/beet/toolchain/worker.py
+-rw-r--r--   0        0        0     2277 2023-08-06 12:25:48.753705 beet-0.91.0/pyproject.toml
+-rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 beet-0.91.0/PKG-INFO
```

### Comparing `beet-0.90.0/LICENSE` & `beet-0.91.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/README.md` & `beet-0.91.0/README.md`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/__init__.py` & `beet-0.91.0/beet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.90.0"
+__version__ = "0.91.0"
 
 
 from .core.cache import *
 from .core.container import *
 from .core.error import *
 from .core.file import *
 from .core.watch import *
```

### Comparing `beet-0.90.0/beet/contrib/auto_yaml.py` & `beet-0.91.0/beet/contrib/auto_yaml.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/autosave.py` & `beet-0.91.0/beet/contrib/autosave.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/babelbox.py` & `beet-0.91.0/beet/contrib/babelbox.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/clear.py` & `beet-0.91.0/beet/contrib/clear.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/copy_files.py` & `beet-0.91.0/beet/contrib/copy_files.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/dbg.py` & `beet-0.91.0/beet/contrib/dbg.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/dundervar.py` & `beet-0.91.0/beet/contrib/dundervar.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/extra_files.py` & `beet-0.91.0/beet/contrib/extra_files.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/find_replace.py` & `beet-0.91.0/beet/contrib/find_replace.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/format_json.py` & `beet-0.91.0/beet/contrib/format_json.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/function_header.py` & `beet-0.91.0/beet/contrib/function_header.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/hangman.py` & `beet-0.91.0/beet/contrib/hangman.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/inline_function.py` & `beet-0.91.0/beet/contrib/inline_function.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/inline_function_tag.py` & `beet-0.91.0/beet/contrib/inline_function_tag.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/installation_advancement.py` & `beet-0.91.0/beet/contrib/installation_advancement.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/json_log.py` & `beet-0.91.0/beet/contrib/json_log.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/json_reporter.py` & `beet-0.91.0/beet/contrib/json_reporter.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/lantern_load.py` & `beet-0.91.0/beet/contrib/lantern_load.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/line_endings.py` & `beet-0.91.0/beet/contrib/line_endings.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/link.py` & `beet-0.91.0/beet/contrib/link.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/livereload.py` & `beet-0.91.0/beet/contrib/livereload.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/load.py` & `beet-0.91.0/beet/contrib/load.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/load_yaml.py` & `beet-0.91.0/beet/contrib/load_yaml.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/log_level.py` & `beet-0.91.0/beet/contrib/log_level.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/messages.py` & `beet-0.91.0/beet/contrib/messages.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/model_merging.py` & `beet-0.91.0/beet/contrib/model_merging.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/optifine.py` & `beet-0.91.0/beet/contrib/optifine.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/output.py` & `beet-0.91.0/beet/contrib/output.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/relative_function_path.py` & `beet-0.91.0/beet/contrib/relative_function_path.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/rename_files.py` & `beet-0.91.0/beet/contrib/rename_files.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/render.py` & `beet-0.91.0/beet/contrib/render.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 __all__ = [
     "RenderOptions",
     "render",
 ]
 
 
-from typing import Dict
+from typing import Dict, Union
 
 from beet import Context, ListOption, PluginOptions, configurable
 from beet.core.utils import snake_case
 
 
 class RenderOptions(PluginOptions):
-    resource_pack: Dict[str, ListOption[str]] = {}
-    data_pack: Dict[str, ListOption[str]] = {}
+    resource_pack: Union[Dict[str, ListOption[str]], ListOption[str]] = {}
+    data_pack: Union[Dict[str, ListOption[str]], ListOption[str]] = {}
 
 
 def beet_default(ctx: Context):
     ctx.require(render)
 
 
 @configurable(validator=RenderOptions)
@@ -27,16 +27,19 @@
     """Plugin that processes the data pack and the resource pack with Jinja."""
     for groups, pack in zip([opts.resource_pack, opts.data_pack], ctx.packs):
         file_types = set(pack.resolve_scope_map().values())
         group_map = {
             snake_case(file_type.__name__): file_type for file_type in file_types
         }
 
-        for singular in list(group_map):
-            group_map.setdefault(f"{singular}s", group_map[singular])
+        if isinstance(groups, ListOption):
+            groups = {k: groups for k in group_map}
+        else:
+            for singular in list(group_map):
+                group_map.setdefault(f"{singular}s", group_map[singular])
 
         for group, render_options in groups.items():
             try:
                 file_type = group_map[group]
                 proxy = pack[file_type]
                 file_paths = proxy.match(*render_options.entries())
             except:
```

### Comparing `beet-0.90.0/beet/contrib/sandstone.py` & `beet-0.91.0/beet/contrib/sandstone.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/scoreboard.py` & `beet-0.91.0/beet/contrib/scoreboard.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/stdin.py` & `beet-0.91.0/beet/contrib/stdin.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/strip_final_newlines.py` & `beet-0.91.0/beet/contrib/strip_final_newlines.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/text_encoding.py` & `beet-0.91.0/beet/contrib/text_encoding.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/unknown_files.py` & `beet-0.91.0/beet/contrib/unknown_files.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/vanilla.py` & `beet-0.91.0/beet/contrib/vanilla.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/worldgen.py` & `beet-0.91.0/beet/contrib/worldgen.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/contrib/yellow_shulker_box.py` & `beet-0.91.0/beet/contrib/yellow_shulker_box.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/core/cache.py` & `beet-0.91.0/beet/core/cache.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/core/container.py` & `beet-0.91.0/beet/core/container.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/core/error.py` & `beet-0.91.0/beet/core/error.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/core/file.py` & `beet-0.91.0/beet/core/file.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/core/utils.py` & `beet-0.91.0/beet/core/utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/core/watch.py` & `beet-0.91.0/beet/core/watch.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/library/base.py` & `beet-0.91.0/beet/library/base.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/library/data_pack.py` & `beet-0.91.0/beet/library/data_pack.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/library/resource_pack.py` & `beet-0.91.0/beet/library/resource_pack.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/library/test_utils.py` & `beet-0.91.0/beet/library/test_utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/library/utils.py` & `beet-0.91.0/beet/library/utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/pytest_plugin.py` & `beet-0.91.0/beet/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/cli.py` & `beet-0.91.0/beet/toolchain/cli.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/commands.py` & `beet-0.91.0/beet/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/config.py` & `beet-0.91.0/beet/toolchain/config.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/context.py` & `beet-0.91.0/beet/toolchain/context.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/generator.py` & `beet-0.91.0/beet/toolchain/generator.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/helpers.py` & `beet-0.91.0/beet/toolchain/helpers.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/pipeline.py` & `beet-0.91.0/beet/toolchain/pipeline.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/project.py` & `beet-0.91.0/beet/toolchain/project.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/select.py` & `beet-0.91.0/beet/toolchain/select.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/template.py` & `beet-0.91.0/beet/toolchain/template.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/tree.py` & `beet-0.91.0/beet/toolchain/tree.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/utils.py` & `beet-0.91.0/beet/toolchain/utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/beet/toolchain/worker.py` & `beet-0.91.0/beet/toolchain/worker.py`

 * *Files identical despite different names*

### Comparing `beet-0.90.0/pyproject.toml` & `beet-0.91.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beet"
-version = "0.90.0"
+version = "0.91.0"
 description = "The Minecraft pack development kit"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/beet"
 repository = "https://github.com/mcbeet/beet"
 documentation = "https://github.com/mcbeet/beet"
```

### Comparing `beet-0.90.0/PKG-INFO` & `beet-0.91.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beet
-Version: 0.90.0
+Version: 0.91.0
 Summary: The Minecraft pack development kit
 Home-page: https://github.com/mcbeet/beet
 License: MIT
 Keywords: beet,minecraft,datapack,resourcepack,mcfunction
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.10,<4.0
```

