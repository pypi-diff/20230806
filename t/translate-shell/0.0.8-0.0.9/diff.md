# Comparing `tmp/translate-shell-0.0.8.tar.gz` & `tmp/translate-shell-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translate-shell-0.0.8.tar", last modified: Sun Jan  8 07:34:11 2023, max compression
+gzip compressed data, was "translate-shell-0.0.9.tar", last modified: Mon Jan  9 05:47:52 2023, max compression
```

## Comparing `translate-shell-0.0.8.tar` & `translate-shell-0.0.9.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.148898 translate-shell-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.120898 translate-shell-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-08 07:33:52.000000 translate-shell-0.0.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.120898 translate-shell-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-01-08 07:33:52.000000 translate-shell-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-01-08 07:33:52.000000 translate-shell-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-08 07:33:52.000000 translate-shell-0.0.8/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-01-08 07:33:52.000000 translate-shell-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-08 07:33:52.000000 translate-shell-0.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-08 07:33:52.000000 translate-shell-0.0.8/.yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-08 07:33:52.000000 translate-shell-0.0.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-08 07:33:52.000000 translate-shell-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-01-08 07:33:52.000000 translate-shell-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-01-08 07:34:11.148898 translate-shell-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-01-08 07:33:52.000000 translate-shell-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-08 07:33:52.000000 translate-shell-0.0.8/addon-info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.112898 translate-shell-0.0.8/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.120898 translate-shell-0.0.8/assets/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-08 07:33:52.000000 translate-shell-0.0.8/assets/desktop/translate-shell.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.120898 translate-shell-0.0.8/autoload/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.120898 translate-shell-0.0.8/autoload/translate_shell/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-08 07:33:52.000000 translate-shell-0.0.8/autoload/translate_shell/utils.vim
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-08 07:33:52.000000 translate-shell-0.0.8/autoload/translate_shell.vim
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.120898 translate-shell-0.0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-01-08 07:33:52.000000 translate-shell-0.0.8/doc/translate-shell.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.120898 translate-shell-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.124898 translate-shell-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/api/external.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/api/translate_shell.md
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/api/translators.md
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/api/ui.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/api/utils.md
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.124898 translate-shell-0.0.8/docs/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/misc/acknowledgements.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/misc/todo.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.124898 translate-shell-0.0.8/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/gui.md
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/make.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/man.md
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/readline.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/translator.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-08 07:33:52.000000 translate-shell-0.0.8/docs/resources/vim.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.124898 translate-shell-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-08 07:33:52.000000 translate-shell-0.0.8/examples/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-08 07:33:52.000000 translate-shell-0.0.8/examples/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.124898 translate-shell-0.0.8/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-08 07:33:52.000000 translate-shell-0.0.8/plugin/translate_shell.vim
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-01-08 07:33:52.000000 translate-shell-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.128898 translate-shell-0.0.8/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-01-08 07:33:52.000000 translate-shell-0.0.8/requirements/color.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-01-08 07:33:52.000000 translate-shell-0.0.8/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-01-08 07:33:52.000000 translate-shell-0.0.8/requirements/keyring.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-01-08 07:33:52.000000 translate-shell-0.0.8/requirements/langdetect.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-01-08 07:33:52.000000 translate-shell-0.0.8/requirements/notification.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-01-08 07:33:52.000000 translate-shell-0.0.8/requirements/rich.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      160 2023-01-08 07:33:52.000000 translate-shell-0.0.8/requirements/stardict.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-01-08 07:33:52.000000 translate-shell-0.0.8/requirements/yaml.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.128898 translate-shell-0.0.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-CITATION.cff.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      154 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-__init__.py.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      259 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-acknowledgements.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-addon-info.json.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-pyproject.toml.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-repl-screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-requirements.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-todo.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-translator.md.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-01-08 07:33:52.000000 translate-shell-0.0.8/scripts/generate-vim.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 07:34:11.148898 translate-shell-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.112898 translate-shell-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.128898 translate-shell-0.0.8/src/translate_shell/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4629 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-08 07:34:10.000000 translate-shell-0.0.8/src/translate_shell/_metainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-08 07:34:10.000000 translate-shell-0.0.8/src/translate_shell/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.116898 translate-shell-0.0.8/src/translate_shell/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/assets/bash/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/assets/bash/preamble.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/assets/images/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/assets/json/lang.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/assets/json/number.json
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/assets/json/youdaozhiyun-error.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/assets/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/assets/zsh/preamble.zsh
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/external/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/external/colorama/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/colorama/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      601 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/colorama/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/external/keyring/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/keyring/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      728 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/keyring/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/external/langdetect/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/langdetect/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/langdetect/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell/external/platformdirs/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/platformdirs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/platformdirs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/external/pynotifier/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/pynotifier/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/pynotifier/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/external/pystardict/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/pystardict/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      748 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/pystardict/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/external/readline/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/readline/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      656 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/readline/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/external/rich/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/rich/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/rich/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/external/rich/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/rich/logging/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/rich/logging/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/external/rich/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/rich/traceback/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/rich/traceback/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/external/shtab/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/shtab/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/shtab/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/external/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/yaml/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/external/yaml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.136898 translate-shell-0.0.8/src/translate_shell/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.140898 translate-shell-0.0.8/src/translate_shell/translators/online/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/online/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/online/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/online/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/online/haici.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/online/yandex.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/online/youdao.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/online/youdaozhiyun.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/speaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.140898 translate-shell-0.0.8/src/translate_shell/translators/stardict/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/stardict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/stardict/jmdict_en_ja.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/stardict/jmdict_ja_en.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/stardict/langdao_ce_gb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/translators/stardict/langdao_ec_gb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.140898 translate-shell-0.0.8/src/translate_shell/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/ui/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/ui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/ui/repl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.144898 translate-shell-0.0.8/src/translate_shell/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/clippers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/speakers.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-08 07:33:52.000000 translate-shell-0.0.8/src/translate_shell/utils/youdaozhiyun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.132898 translate-shell-0.0.8/src/translate_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-01-08 07:34:11.000000 translate-shell-0.0.8/src/translate_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-01-08 07:34:11.000000 translate-shell-0.0.8/src/translate_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 07:34:11.000000 translate-shell-0.0.8/src/translate_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-08 07:34:11.000000 translate-shell-0.0.8/src/translate_shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-01-08 07:34:11.000000 translate-shell-0.0.8/src/translate_shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-08 07:34:11.000000 translate-shell-0.0.8/src/translate_shell.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.144898 translate-shell-0.0.8/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-08 07:33:52.000000 translate-shell-0.0.8/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-08 07:33:52.000000 translate-shell-0.0.8/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-01-08 07:33:52.000000 translate-shell-0.0.8/templates/metainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-08 07:33:52.000000 translate-shell-0.0.8/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.144898 translate-shell-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-08 07:33:52.000000 translate-shell-0.0.8/test/.themisrc
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-08 07:33:52.000000 translate-shell-0.0.8/test/syntax_test.vimspec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.144898 translate-shell-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-08 07:33:52.000000 translate-shell-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-08 07:33:52.000000 translate-shell-0.0.8/tests/cmd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.144898 translate-shell-0.0.8/tests/json/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-08 07:33:52.000000 translate-shell-0.0.8/tests/json/google.json
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-01-08 07:33:52.000000 translate-shell-0.0.8/tests/translate_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.144898 translate-shell-0.0.8/tests/txt/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-01-08 07:33:52.000000 translate-shell-0.0.8/tests/txt/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-08 07:33:52.000000 translate-shell-0.0.8/tests/txt/usage.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:34:11.144898 translate-shell-0.0.8/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-08 07:33:52.000000 translate-shell-0.0.8/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-08 07:33:52.000000 translate-shell-0.0.8/tests/utils/output_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.015431 translate-shell-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-09 05:47:38.000000 translate-shell-0.0.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-01-09 05:47:38.000000 translate-shell-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-01-09 05:47:38.000000 translate-shell-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 05:47:38.000000 translate-shell-0.0.9/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-01-09 05:47:38.000000 translate-shell-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-09 05:47:38.000000 translate-shell-0.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-09 05:47:38.000000 translate-shell-0.0.9/.yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-09 05:47:38.000000 translate-shell-0.0.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-09 05:47:38.000000 translate-shell-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-01-09 05:47:38.000000 translate-shell-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-01-09 05:47:52.015431 translate-shell-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-01-09 05:47:38.000000 translate-shell-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-09 05:47:38.000000 translate-shell-0.0.9/addon-info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.995431 translate-shell-0.0.9/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/assets/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-09 05:47:38.000000 translate-shell-0.0.9/assets/desktop/translate-shell.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/autoload/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/autoload/translate_shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-09 05:47:38.000000 translate-shell-0.0.9/autoload/translate_shell/utils.vim
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-09 05:47:38.000000 translate-shell-0.0.9/autoload/translate_shell.vim
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-01-09 05:47:38.000000 translate-shell-0.0.9/doc/translate-shell.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/api/external.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/api/translate_shell.md
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/api/translators.md
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/api/ui.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/api/utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.999431 translate-shell-0.0.9/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/misc/acknowledgements.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/misc/todo.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.003431 translate-shell-0.0.9/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/gui.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/make.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/man.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/readline.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/translator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-09 05:47:38.000000 translate-shell-0.0.9/docs/resources/vim.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.003431 translate-shell-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-09 05:47:38.000000 translate-shell-0.0.9/examples/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-09 05:47:38.000000 translate-shell-0.0.9/examples/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.003431 translate-shell-0.0.9/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-09 05:47:38.000000 translate-shell-0.0.9/plugin/translate_shell.vim
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-01-09 05:47:38.000000 translate-shell-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.003431 translate-shell-0.0.9/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-01-09 05:47:38.000000 translate-shell-0.0.9/requirements/color.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-01-09 05:47:38.000000 translate-shell-0.0.9/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-01-09 05:47:38.000000 translate-shell-0.0.9/requirements/keyring.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-01-09 05:47:38.000000 translate-shell-0.0.9/requirements/langdetect.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-01-09 05:47:38.000000 translate-shell-0.0.9/requirements/notification.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-01-09 05:47:38.000000 translate-shell-0.0.9/requirements/rich.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      160 2023-01-09 05:47:38.000000 translate-shell-0.0.9/requirements/stardict.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-01-09 05:47:38.000000 translate-shell-0.0.9/requirements/yaml.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.003431 translate-shell-0.0.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-CITATION.cff.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      154 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-__init__.py.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      259 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-acknowledgements.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-addon-info.json.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-pyproject.toml.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-repl-screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-requirements.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-todo.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-translator.md.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-01-09 05:47:38.000000 translate-shell-0.0.9/scripts/generate-vim.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 05:47:52.015431 translate-shell-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.995431 translate-shell-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.003431 translate-shell-0.0.9/src/translate_shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4629 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-09 05:47:51.000000 translate-shell-0.0.9/src/translate_shell/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-09 05:47:51.000000 translate-shell-0.0.9/src/translate_shell/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:51.995431 translate-shell-0.0.9/src/translate_shell/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/assets/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/assets/bash/preamble.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/assets/images/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/assets/json/lang.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/assets/json/number.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/assets/json/youdaozhiyun-error.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/assets/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/assets/zsh/preamble.zsh
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/colorama/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/colorama/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      601 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/colorama/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/keyring/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/keyring/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      728 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/keyring/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/langdetect/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/langdetect/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/langdetect/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/platformdirs/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/platformdirs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/platformdirs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/pynotifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/pynotifier/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/pynotifier/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/pystardict/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/pystardict/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      748 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/pystardict/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/readline/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/readline/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      656 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/readline/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/rich/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/rich/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/rich/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/rich/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/rich/logging/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/rich/logging/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/rich/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/rich/traceback/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/rich/traceback/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/shtab/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/shtab/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/shtab/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/external/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/yaml/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/external/yaml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.007431 translate-shell-0.0.9/src/translate_shell/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.011431 translate-shell-0.0.9/src/translate_shell/translators/online/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/online/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/online/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/online/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/online/haici.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/online/yandex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/online/youdao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/online/youdaozhiyun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/speaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.011431 translate-shell-0.0.9/src/translate_shell/translators/stardict/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/stardict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/stardict/jmdict_en_ja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/stardict/jmdict_ja_en.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/stardict/langdao_ce_gb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/translators/stardict/langdao_ec_gb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.011431 translate-shell-0.0.9/src/translate_shell/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/ui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/ui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/ui/repl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.011431 translate-shell-0.0.9/src/translate_shell/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/clippers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/speakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-09 05:47:38.000000 translate-shell-0.0.9/src/translate_shell/utils/youdaozhiyun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.003431 translate-shell-0.0.9/src/translate_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-01-09 05:47:51.000000 translate-shell-0.0.9/src/translate_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-01-09 05:47:51.000000 translate-shell-0.0.9/src/translate_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 05:47:51.000000 translate-shell-0.0.9/src/translate_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-09 05:47:51.000000 translate-shell-0.0.9/src/translate_shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-01-09 05:47:51.000000 translate-shell-0.0.9/src/translate_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-09 05:47:51.000000 translate-shell-0.0.9/src/translate_shell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.011431 translate-shell-0.0.9/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-09 05:47:38.000000 translate-shell-0.0.9/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-09 05:47:38.000000 translate-shell-0.0.9/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-01-09 05:47:38.000000 translate-shell-0.0.9/templates/metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-09 05:47:38.000000 translate-shell-0.0.9/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.011431 translate-shell-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-09 05:47:38.000000 translate-shell-0.0.9/test/.themisrc
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-09 05:47:38.000000 translate-shell-0.0.9/test/syntax_test.vimspec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.011431 translate-shell-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-09 05:47:38.000000 translate-shell-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-09 05:47:38.000000 translate-shell-0.0.9/tests/cmd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.011431 translate-shell-0.0.9/tests/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-09 05:47:38.000000 translate-shell-0.0.9/tests/json/google.json
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-01-09 05:47:38.000000 translate-shell-0.0.9/tests/translate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.015431 translate-shell-0.0.9/tests/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-01-09 05:47:38.000000 translate-shell-0.0.9/tests/txt/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-09 05:47:38.000000 translate-shell-0.0.9/tests/txt/usage.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 05:47:52.015431 translate-shell-0.0.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-09 05:47:38.000000 translate-shell-0.0.9/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-09 05:47:38.000000 translate-shell-0.0.9/tests/utils/output_test.py
```

### Comparing `translate-shell-0.0.8/.github/workflows/main.yml` & `translate-shell-0.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/.gitignore` & `translate-shell-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/.pre-commit-config.yaml` & `translate-shell-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/LICENSE` & `translate-shell-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/Makefile` & `translate-shell-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/PKG-INFO` & `translate-shell-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-shell
-Version: 0.0.8
+Version: 0.0.9
 Summary: Translate text by google, bing, youdaozhiyun, haici, stardict, etc at same time from CLI, GUI (GNU/Linux, Android, macOS and Windows), REPL, python, shell and vim.
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://translate-shell.readthedocs.org
 Project-URL: Download, https://github.com/Freed-Wu/translate-shell/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/translate-shell/issues
 Project-URL: Source, https://github.com/Freed-Wu/translate-shell
```

### Comparing `translate-shell-0.0.8/README.md` & `translate-shell-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/autoload/translate_shell.vim` & `translate-shell-0.0.9/autoload/translate_shell.vim`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/doc/translate-shell.txt` & `translate-shell-0.0.9/doc/translate-shell.txt`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/docs/conf.py` & `translate-shell-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/docs/resources/config.md` & `translate-shell-0.0.9/docs/resources/config.md`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/docs/resources/gui.md` & `translate-shell-0.0.9/docs/resources/gui.md`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/docs/resources/install.md` & `translate-shell-0.0.9/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/docs/resources/translator.md` & `translate-shell-0.0.9/docs/resources/translator.md`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/pyproject.toml` & `translate-shell-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/scripts/generate-addon-info.json.pl` & `translate-shell-0.0.9/scripts/generate-addon-info.json.pl`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/scripts/generate-repl-screenshot.py` & `translate-shell-0.0.9/scripts/generate-repl-screenshot.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/__init__.py` & `translate-shell-0.0.9/src/translate_shell/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/__main__.py` & `translate-shell-0.0.9/src/translate_shell/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/_metainfo.py` & `translate-shell-0.0.9/src/translate_shell/_metainfo.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/assets/images/icon.png` & `translate-shell-0.0.9/src/translate_shell/assets/images/icon.png`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/assets/json/lang.json` & `translate-shell-0.0.9/src/translate_shell/assets/json/lang.json`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/assets/json/youdaozhiyun-error.json` & `translate-shell-0.0.9/src/translate_shell/assets/json/youdaozhiyun-error.json`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/config.py` & `translate-shell-0.0.9/src/translate_shell/config.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/colorama/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/colorama/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/keyring/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/keyring/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/langdetect/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/langdetect/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/platformdirs/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/pynotifier/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/pynotifier/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/pystardict/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/pystardict/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/readline/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/readline/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/rich/logging/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/rich/logging/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/shtab/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/shtab/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/external/yaml/__main__.py` & `translate-shell-0.0.9/src/translate_shell/external/yaml/__main__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translate.py` & `translate-shell-0.0.9/src/translate_shell/translate.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/__init__.py` & `translate-shell-0.0.9/src/translate_shell/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/online/__init__.py` & `translate-shell-0.0.9/src/translate_shell/translators/online/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/online/bing.py` & `translate-shell-0.0.9/src/translate_shell/translators/online/bing.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/online/google.py` & `translate-shell-0.0.9/src/translate_shell/translators/online/google.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/online/haici.py` & `translate-shell-0.0.9/src/translate_shell/translators/online/haici.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/online/youdaozhiyun.py` & `translate-shell-0.0.9/src/translate_shell/translators/online/youdaozhiyun.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/speaker.py` & `translate-shell-0.0.9/src/translate_shell/translators/speaker.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/stardict/__init__.py` & `translate-shell-0.0.9/src/translate_shell/translators/stardict/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/stardict/jmdict_en_ja.py` & `translate-shell-0.0.9/src/translate_shell/translators/stardict/jmdict_en_ja.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/stardict/jmdict_ja_en.py` & `translate-shell-0.0.9/src/translate_shell/translators/stardict/jmdict_ja_en.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/stardict/langdao_ce_gb.py` & `translate-shell-0.0.9/src/translate_shell/translators/stardict/langdao_ce_gb.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/translators/stardict/langdao_ec_gb.py` & `translate-shell-0.0.9/src/translate_shell/translators/stardict/langdao_ec_gb.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/ui/__init__.py` & `translate-shell-0.0.9/src/translate_shell/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/ui/gui.py` & `translate-shell-0.0.9/src/translate_shell/ui/gui.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/ui/repl.py` & `translate-shell-0.0.9/src/translate_shell/ui/repl.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/utils/clippers.py` & `translate-shell-0.0.9/src/translate_shell/utils/clippers.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/utils/complete.py` & `translate-shell-0.0.9/src/translate_shell/utils/complete.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,24 @@
     :type state: int
     :rtype: str
     """
     langs = list(LANGS.keys())
     volcab = ["=", "<", "!", ":"] + langs
     sl = text.split(":")[0]
     if text.startswith("="):
-        volcab = map(lambda x: "=" + x, TRANSLATORS)
+        length = len("=")
+        left, _, right = text[length:].rpartition(",")
+        if right in TRANSLATORS:
+            volcab = [text + ","]
+        else:
+            translators = left.split(",")
+            volcab = map(
+                lambda x: "=" + left + ("," if left else "") + x,
+                filter(lambda x: x not in translators, TRANSLATORS),
+            )
     elif text.startswith("<"):
         length = len("<")
         dirname = os.path.dirname(text[length:])
         if dirname:
             files = os.listdir(dirname)
         else:
             files = os.listdir()
@@ -47,10 +56,10 @@
                 if os.path.isdir(path):
                     files = os.listdir(path)
                     for file in files:
                         if os.path.isfile(os.path.join(path, file)):
                             bins += [file]
         volcab = map(lambda x: "!" + x, bins)
     elif sl in langs + [""] and len(text.split(":")) == 2:
-        volcab = map(lambda x: sl + ":" + x, langs + [""])
+        volcab = map(lambda x: sl + ":" + x, langs)
     results = [x for x in volcab if x.startswith(text)]
     return results[state]
```

### Comparing `translate-shell-0.0.8/src/translate_shell/utils/input.py` & `translate-shell-0.0.9/src/translate_shell/utils/input.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/utils/output.py` & `translate-shell-0.0.9/src/translate_shell/utils/output.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/utils/prompt.py` & `translate-shell-0.0.9/src/translate_shell/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/utils/setting.py` & `translate-shell-0.0.9/src/translate_shell/utils/setting.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/utils/speakers.py` & `translate-shell-0.0.9/src/translate_shell/utils/speakers.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell/utils/youdaozhiyun.py` & `translate-shell-0.0.9/src/translate_shell/utils/youdaozhiyun.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/src/translate_shell.egg-info/PKG-INFO` & `translate-shell-0.0.9/src/translate_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-shell
-Version: 0.0.8
+Version: 0.0.9
 Summary: Translate text by google, bing, youdaozhiyun, haici, stardict, etc at same time from CLI, GUI (GNU/Linux, Android, macOS and Windows), REPL, python, shell and vim.
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://translate-shell.readthedocs.org
 Project-URL: Download, https://github.com/Freed-Wu/translate-shell/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/translate-shell/issues
 Project-URL: Source, https://github.com/Freed-Wu/translate-shell
```

### Comparing `translate-shell-0.0.8/src/translate_shell.egg-info/SOURCES.txt` & `translate-shell-0.0.9/src/translate_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/templates/metainfo.py` & `translate-shell-0.0.9/templates/metainfo.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/tests/cmd_test.py` & `translate-shell-0.0.9/tests/cmd_test.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/tests/translate_test.py` & `translate-shell-0.0.9/tests/translate_test.py`

 * *Files identical despite different names*

### Comparing `translate-shell-0.0.8/tests/txt/options.txt` & `translate-shell-0.0.9/tests/txt/options.txt`

 * *Files identical despite different names*

