# Comparing `tmp/dotdrop-1.8.2.tar.gz` & `tmp/dotdrop-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotdrop-1.8.2.tar", last modified: Sat Nov 27 08:01:36 2021, max compression
+gzip compressed data, was "dotdrop-1.9.0.tar", last modified: Tue May 31 19:57:07 2022, max compression
```

## Comparing `dotdrop-1.8.2.tar` & `dotdrop-1.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 08:01:36.905181 dotdrop-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2021-11-27 08:01:26.000000 dotdrop-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-11-27 08:01:26.000000 dotdrop-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15093 2021-11-27 08:01:36.905181 dotdrop-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11517 2021-11-27 08:01:26.000000 dotdrop-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 08:01:36.905181 dotdrop-1.8.2/dotdrop/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5478 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/action.py
--rw-r--r--   0 runner    (1001) docker     (121)    14807 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/cfg_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (121)    61476 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/cfg_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     7356 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/comparator.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/dictparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    30817 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/dotdrop.py
--rw-r--r--   0 runner    (1001) docker     (121)     5348 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7942 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)    26432 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/installer.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/jhelpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/linktypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    13793 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     6094 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     9987 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/templategen.py
--rw-r--r--   0 runner    (1001) docker     (121)    17672 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/updater.py
--rw-r--r--   0 runner    (1001) docker     (121)    13892 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-11-27 08:01:26.000000 dotdrop-1.8.2/dotdrop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 08:01:36.905181 dotdrop-1.8.2/dotdrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15093 2021-11-27 08:01:36.000000 dotdrop-1.8.2/dotdrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      677 2021-11-27 08:01:36.000000 dotdrop-1.8.2/dotdrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-27 08:01:36.000000 dotdrop-1.8.2/dotdrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-11-27 08:01:36.000000 dotdrop-1.8.2/dotdrop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-11-27 08:01:36.000000 dotdrop-1.8.2/dotdrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-11-27 08:01:36.000000 dotdrop-1.8.2/dotdrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-11-27 08:01:26.000000 dotdrop-1.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-11-27 08:01:36.905181 dotdrop-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2021-11-27 08:01:26.000000 dotdrop-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 19:57:07.737910 dotdrop-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-05-31 19:56:55.000000 dotdrop-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-31 19:56:55.000000 dotdrop-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    13864 2022-05-31 19:57:07.737910 dotdrop-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10451 2022-05-31 19:56:55.000000 dotdrop-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 19:57:07.737910 dotdrop-1.9.0/dotdrop/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5478 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/action.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15037 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/cfg_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65516 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/cfg_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7613 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/dictparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30432 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/dotdrop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5348 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8013 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28490 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/installer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/jhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/linktypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13864 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6094 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9987 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/templategen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17672 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/updater.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13892 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-05-31 19:56:55.000000 dotdrop-1.9.0/dotdrop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 19:57:07.737910 dotdrop-1.9.0/dotdrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13864 2022-05-31 19:57:07.000000 dotdrop-1.9.0/dotdrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-05-31 19:57:07.000000 dotdrop-1.9.0/dotdrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 19:57:07.000000 dotdrop-1.9.0/dotdrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-31 19:57:07.000000 dotdrop-1.9.0/dotdrop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-05-31 19:57:07.000000 dotdrop-1.9.0/dotdrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-31 19:57:07.000000 dotdrop-1.9.0/dotdrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-31 19:56:55.000000 dotdrop-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-31 19:57:07.737910 dotdrop-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-05-31 19:56:55.000000 dotdrop-1.9.0/setup.py
```

### Comparing `dotdrop-1.8.2/LICENSE` & `dotdrop-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/PKG-INFO` & `dotdrop-1.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 Metadata-Version: 2.1
 Name: dotdrop
-Version: 1.8.2
+Version: 1.9.0
 Summary: Save your dotfiles once, deploy them everywhere
 Home-page: https://github.com/deadc0de6/dotdrop
 Author: deadc0de6
 Author-email: deadc0de6@foo.bar
 License: GPLv3
-Download-URL: https://github.com/deadc0de6/dotdrop/archive/v1.8.2.tar.gz
+Download-URL: https://github.com/deadc0de6/dotdrop/archive/v1.9.0.tar.gz
 Description: # <img src="https://raw.githubusercontent.com/deadc0de6/dotdrop/master/dotdrop.svg" width="100" height="100" align="left"> dotdrop
         <br/>
         <br/>
         
+        [![GitHub release (latest by date)](https://img.shields.io/github/v/release/deadc0de6/dotdrop)](https://github.com/deadc0de6/dotdrop/releases/latest)
+        [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
+        [![GitHub Repo stars](https://img.shields.io/github/stars/deadc0de6/dotdrop?style=social)](https://github.com/deadc0de6/dotdrop/)
+        
         [![Tests Status](https://github.com/deadc0de6/dotdrop/workflows/tests/badge.svg)](https://github.com/deadc0de6/dotdrop/actions)
         [![Doc Status](https://readthedocs.org/projects/dotdrop/badge/?version=latest)](https://dotdrop.readthedocs.io/en/latest/?badge=latest)
-        [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
-        [![Coverage Status](https://coveralls.io/repos/github/deadc0de6/dotdrop/badge.svg?branch=master)](https://coveralls.io/github/deadc0de6/dotdrop?branch=master)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/deadc0de6/dotdrop.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/deadc0de6/dotdrop/context:python)
+        [![Coveralls](https://img.shields.io/coveralls/github/deadc0de6/dotdrop)](https://coveralls.io/github/deadc0de6/dotdrop?branch=master)
+        [![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/deadc0de6/dotdrop?label=code%20quality)](https://lgtm.com/projects/g/deadc0de6/dotdrop/context:python)
         
-        [![PyPI version](https://badge.fury.io/py/dotdrop.svg)](https://badge.fury.io/py/dotdrop)
-        [![AUR](https://img.shields.io/aur/version/dotdrop.svg)](https://aur.archlinux.org/packages/dotdrop)
         [![Python](https://img.shields.io/pypi/pyversions/dotdrop.svg)](https://pypi.python.org/pypi/dotdrop)
         
+        [![PyPI](https://img.shields.io/pypi/v/dotdrop)](https://badge.fury.io/py/dotdrop)
+        [![Homebrew version](https://img.shields.io/homebrew/v/dotdrop)](https://formulae.brew.sh/formula/dotdrop)
+        [![AUR](https://img.shields.io/aur/version/dotdrop.svg)](https://aur.archlinux.org/packages/dotdrop)
+        
         [![Donate](https://img.shields.io/badge/donate-KoFi-blue.svg)](https://ko-fi.com/deadc0de6)
         
         *Save your dotfiles once, deploy them everywhere*
         
         [Dotdrop](https://github.com/deadc0de6/dotdrop) makes the management of dotfiles between different hosts easy.
         It allows you to store your dotfiles in Git and automagically deploy
         different versions of the same file on different setups.
         
-        It also allows you to manage different *sets* of dotfiles.
+        It also allows to manage different *sets* of dotfiles.
         For example, you can have a set of dotfiles for your home laptop and
         a different set for your office desktop. Those sets may overlap, and different
         versions of the same dotfiles can be deployed using different predefined *profiles*.
         Or you may have a main set of dotfiles for your
         everyday host and a subset you only need to deploy to temporary
         hosts (cloud VM etc.) that may be using
         a slightly different version of some of the dotfiles.
         
         Features:
         
         * Sync once every dotfile in Git for different usages
-        * Allow dotfile templating by leveraging [Jinja2](https://palletsprojects.com/p/jinja/)
+        * Allow dotfile templating
         * Dynamically generated dotfile contents with pre-defined variables
         * Comparison between deployed and stored dotfiles
         * Handling multiple profiles with different sets of dotfiles
         * Easily import and update dotfiles
         * Handle files and directories
         * Support symlinking of dotfiles
         * Associate actions to the deployment of specific dotfiles
@@ -55,29 +60,30 @@
         Also check out the [blog post](https://deadc0de.re/articles/dotfiles.html),
         the [example](#getting-started), the [documentation](https://dotdrop.readthedocs.io/) or
         how [people are using dotdrop](https://dotdrop.readthedocs.io/en/latest/misc/people-using-dotdrop/)
         for more.
         
         Quick start:
         ```bash
+        ## using dotdrop as a submodule
         mkdir dotfiles && cd dotfiles
         git init
         git submodule add https://github.com/deadc0de6/dotdrop.git
         pip3 install -r dotdrop/requirements.txt --user
         ./dotdrop/bootstrap.sh
         ./dotdrop.sh --help
         ```
         
         A mirror of this repository is available on GitLab under <https://gitlab.com/deadc0de6/dotdrop>.
         
         ## Why dotdrop?
         
         There exist many tools to manage dotfiles; however, not
-        many allow you to deploy different versions of the same dotfile
-        on different hosts. Moreover, dotdrop allows you to specify the
+        many allow to deploy different versions of the same dotfile
+        on different hosts. Moreover, dotdrop allows to specify the
         set of dotfiles that need to be deployed for a specific profile.
         
         See the [example](#getting-started) for a concrete example of
         why [dotdrop](https://github.com/deadc0de6/dotdrop) rocks.
         
         ---
         
@@ -86,69 +92,30 @@
         * [Installation](#installation)
         * [Getting started](#getting-started)
         * [Documentation](#documentation)
         * [Thank you](#thank-you)
         
         # Installation
         
-        There are multiple ways to install and use dotdrop.
-        It is recommended to install dotdrop [as a submodule](#as-a-submodule)
-        to your dotfiles Git tree. Having dotdrop as a submodule guarantees that anywhere
-        you are cloning your dotfiles Git tree from you'll have dotdrop shipped with it.
-        
-        The below instructions show how to install dotdrop as a submodule. For alternative
-        installation instructions, see the
-        [installation documentation](https://dotdrop.readthedocs.io/en/latest/installation/).
-        
-        Dotdrop is also available on:
-        * pypi: https://pypi.org/project/dotdrop/
-        * aur (stable): https://aur.archlinux.org/packages/dotdrop/
-        * aur (git version): https://aur.archlinux.org/packages/dotdrop-git/
-        * snapcraft: https://snapcraft.io/dotdrop
-        
-        ## As a submodule
-        
-        The following will create a git repository for your dotfiles and
-        keep dotdrop as a submodule:
-        ```bash
-        ## create the repository
-        $ mkdir dotfiles; cd dotfiles
-        $ git init
-        
-        ## install dotdrop as a submodule
-        $ git submodule add https://github.com/deadc0de6/dotdrop.git
-        $ pip3 install -r dotdrop/requirements.txt --user
-        $ ./dotdrop/bootstrap.sh
-        
-        ## use dotdrop
-        $ ./dotdrop.sh --help
-        ```
+        See the [installation instructions](https://dotdrop.readthedocs.io/en/latest/installation/).
         
-        For macOS users, make sure to install `realpath` through Homebrew
-        (part of *coreutils*).
-        
-        Using dotdrop as a submodule will require you to work with dotdrop by
-        using the generated script `dotdrop.sh` at the root
-        of your dotfiles repository. Note that this script updates the submodule
-        automatically unless called with the environment variable `DOTDROP_AUTOUPDATE`
-        set to `no`.
-        
-        To ease the use of dotdrop, it is recommended to add an alias to it in your
-        shell (*~/.bashrc*, *~/.zshrc*, etc.) with the config file path, for example:
-        ```
-        alias dotdrop='<absolute-path-to-dotdrop.sh> --cfg=<path-to-your-config.yaml>'
-        ```
+        Dotdrop is available on:
         
-        Completion scripts exist for `bash`, `zsh` and `fish`; see [the related doc](completion/README.md).
+        * [PyPI](https://pypi.org/project/dotdrop/)
+        * [Homebrew](https://formulae.brew.sh/formula/dotdrop)
+        * [AUR (stable)](https://aur.archlinux.org/packages/dotdrop/)
+        * [AUR (git version)](https://aur.archlinux.org/packages/dotdrop-git/)
+        * [Snapcraft](https://snapcraft.io/dotdrop)
+        * [Pacstall](https://github.com/pacstall/pacstall-programs/blob/master/packages/dotdrop/dotdrop.pacscript)
         
         # Getting started
         
         [Create a new repository](https://dotdrop.readthedocs.io/en/latest/repository-setup/)
         to store your dotfiles with dotdrop. *Init* or *clone* that new repository and
-        [install dotdrop](https://dotdrop.readthedocs.io/en/latest/installation/#as-a-submodule).
+        [install dotdrop](https://dotdrop.readthedocs.io/en/latest/installation).
         
         Then import any dotfiles (files or directories) you want to manage with dotdrop.
         You can either use the default profile (which resolves to the *hostname* of the host
         you are running dotdrop on) or provide it explicitly using the switch `-p`/`--profile`.
         
         Import dotfiles on host *home*:
         ```bash
@@ -358,12 +325,14 @@
 Keywords: dotfiles jinja2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3
 Description-Content-Type: text/markdown; variant=GFM
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `dotdrop-1.8.2/README.md` & `dotdrop-1.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 # <img src="https://raw.githubusercontent.com/deadc0de6/dotdrop/master/dotdrop.svg" width="100" height="100" align="left"> dotdrop
 <br/>
 <br/>
 
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/deadc0de6/dotdrop)](https://github.com/deadc0de6/dotdrop/releases/latest)
+[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
+[![GitHub Repo stars](https://img.shields.io/github/stars/deadc0de6/dotdrop?style=social)](https://github.com/deadc0de6/dotdrop/)
+
 [![Tests Status](https://github.com/deadc0de6/dotdrop/workflows/tests/badge.svg)](https://github.com/deadc0de6/dotdrop/actions)
 [![Doc Status](https://readthedocs.org/projects/dotdrop/badge/?version=latest)](https://dotdrop.readthedocs.io/en/latest/?badge=latest)
-[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
-[![Coverage Status](https://coveralls.io/repos/github/deadc0de6/dotdrop/badge.svg?branch=master)](https://coveralls.io/github/deadc0de6/dotdrop?branch=master)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/deadc0de6/dotdrop.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/deadc0de6/dotdrop/context:python)
+[![Coveralls](https://img.shields.io/coveralls/github/deadc0de6/dotdrop)](https://coveralls.io/github/deadc0de6/dotdrop?branch=master)
+[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/deadc0de6/dotdrop?label=code%20quality)](https://lgtm.com/projects/g/deadc0de6/dotdrop/context:python)
 
-[![PyPI version](https://badge.fury.io/py/dotdrop.svg)](https://badge.fury.io/py/dotdrop)
-[![AUR](https://img.shields.io/aur/version/dotdrop.svg)](https://aur.archlinux.org/packages/dotdrop)
 [![Python](https://img.shields.io/pypi/pyversions/dotdrop.svg)](https://pypi.python.org/pypi/dotdrop)
 
+[![PyPI](https://img.shields.io/pypi/v/dotdrop)](https://badge.fury.io/py/dotdrop)
+[![Homebrew version](https://img.shields.io/homebrew/v/dotdrop)](https://formulae.brew.sh/formula/dotdrop)
+[![AUR](https://img.shields.io/aur/version/dotdrop.svg)](https://aur.archlinux.org/packages/dotdrop)
+
 [![Donate](https://img.shields.io/badge/donate-KoFi-blue.svg)](https://ko-fi.com/deadc0de6)
 
 *Save your dotfiles once, deploy them everywhere*
 
 [Dotdrop](https://github.com/deadc0de6/dotdrop) makes the management of dotfiles between different hosts easy.
 It allows you to store your dotfiles in Git and automagically deploy
 different versions of the same file on different setups.
 
-It also allows you to manage different *sets* of dotfiles.
+It also allows to manage different *sets* of dotfiles.
 For example, you can have a set of dotfiles for your home laptop and
 a different set for your office desktop. Those sets may overlap, and different
 versions of the same dotfiles can be deployed using different predefined *profiles*.
 Or you may have a main set of dotfiles for your
 everyday host and a subset you only need to deploy to temporary
 hosts (cloud VM etc.) that may be using
 a slightly different version of some of the dotfiles.
 
 Features:
 
 * Sync once every dotfile in Git for different usages
-* Allow dotfile templating by leveraging [Jinja2](https://palletsprojects.com/p/jinja/)
+* Allow dotfile templating
 * Dynamically generated dotfile contents with pre-defined variables
 * Comparison between deployed and stored dotfiles
 * Handling multiple profiles with different sets of dotfiles
 * Easily import and update dotfiles
 * Handle files and directories
 * Support symlinking of dotfiles
 * Associate actions to the deployment of specific dotfiles
@@ -46,29 +51,30 @@
 Also check out the [blog post](https://deadc0de.re/articles/dotfiles.html),
 the [example](#getting-started), the [documentation](https://dotdrop.readthedocs.io/) or
 how [people are using dotdrop](https://dotdrop.readthedocs.io/en/latest/misc/people-using-dotdrop/)
 for more.
 
 Quick start:
 ```bash
+## using dotdrop as a submodule
 mkdir dotfiles && cd dotfiles
 git init
 git submodule add https://github.com/deadc0de6/dotdrop.git
 pip3 install -r dotdrop/requirements.txt --user
 ./dotdrop/bootstrap.sh
 ./dotdrop.sh --help
 ```
 
 A mirror of this repository is available on GitLab under <https://gitlab.com/deadc0de6/dotdrop>.
 
 ## Why dotdrop?
 
 There exist many tools to manage dotfiles; however, not
-many allow you to deploy different versions of the same dotfile
-on different hosts. Moreover, dotdrop allows you to specify the
+many allow to deploy different versions of the same dotfile
+on different hosts. Moreover, dotdrop allows to specify the
 set of dotfiles that need to be deployed for a specific profile.
 
 See the [example](#getting-started) for a concrete example of
 why [dotdrop](https://github.com/deadc0de6/dotdrop) rocks.
 
 ---
 
@@ -77,69 +83,30 @@
 * [Installation](#installation)
 * [Getting started](#getting-started)
 * [Documentation](#documentation)
 * [Thank you](#thank-you)
 
 # Installation
 
-There are multiple ways to install and use dotdrop.
-It is recommended to install dotdrop [as a submodule](#as-a-submodule)
-to your dotfiles Git tree. Having dotdrop as a submodule guarantees that anywhere
-you are cloning your dotfiles Git tree from you'll have dotdrop shipped with it.
-
-The below instructions show how to install dotdrop as a submodule. For alternative
-installation instructions, see the
-[installation documentation](https://dotdrop.readthedocs.io/en/latest/installation/).
-
-Dotdrop is also available on:
-* pypi: https://pypi.org/project/dotdrop/
-* aur (stable): https://aur.archlinux.org/packages/dotdrop/
-* aur (git version): https://aur.archlinux.org/packages/dotdrop-git/
-* snapcraft: https://snapcraft.io/dotdrop
+See the [installation instructions](https://dotdrop.readthedocs.io/en/latest/installation/).
 
-## As a submodule
-
-The following will create a git repository for your dotfiles and
-keep dotdrop as a submodule:
-```bash
-## create the repository
-$ mkdir dotfiles; cd dotfiles
-$ git init
-
-## install dotdrop as a submodule
-$ git submodule add https://github.com/deadc0de6/dotdrop.git
-$ pip3 install -r dotdrop/requirements.txt --user
-$ ./dotdrop/bootstrap.sh
-
-## use dotdrop
-$ ./dotdrop.sh --help
-```
-
-For macOS users, make sure to install `realpath` through Homebrew
-(part of *coreutils*).
-
-Using dotdrop as a submodule will require you to work with dotdrop by
-using the generated script `dotdrop.sh` at the root
-of your dotfiles repository. Note that this script updates the submodule
-automatically unless called with the environment variable `DOTDROP_AUTOUPDATE`
-set to `no`.
-
-To ease the use of dotdrop, it is recommended to add an alias to it in your
-shell (*~/.bashrc*, *~/.zshrc*, etc.) with the config file path, for example:
-```
-alias dotdrop='<absolute-path-to-dotdrop.sh> --cfg=<path-to-your-config.yaml>'
-```
+Dotdrop is available on:
 
-Completion scripts exist for `bash`, `zsh` and `fish`; see [the related doc](completion/README.md).
+* [PyPI](https://pypi.org/project/dotdrop/)
+* [Homebrew](https://formulae.brew.sh/formula/dotdrop)
+* [AUR (stable)](https://aur.archlinux.org/packages/dotdrop/)
+* [AUR (git version)](https://aur.archlinux.org/packages/dotdrop-git/)
+* [Snapcraft](https://snapcraft.io/dotdrop)
+* [Pacstall](https://github.com/pacstall/pacstall-programs/blob/master/packages/dotdrop/dotdrop.pacscript)
 
 # Getting started
 
 [Create a new repository](https://dotdrop.readthedocs.io/en/latest/repository-setup/)
 to store your dotfiles with dotdrop. *Init* or *clone* that new repository and
-[install dotdrop](https://dotdrop.readthedocs.io/en/latest/installation/#as-a-submodule).
+[install dotdrop](https://dotdrop.readthedocs.io/en/latest/installation).
 
 Then import any dotfiles (files or directories) you want to manage with dotdrop.
 You can either use the default profile (which resolves to the *hostname* of the host
 you are running dotdrop on) or provide it explicitly using the switch `-p`/`--profile`.
 
 Import dotfiles on host *home*:
 ```bash
```

### Comparing `dotdrop-1.8.2/dotdrop/action.py` & `dotdrop-1.9.0/dotdrop/action.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/cfg_aggregator.py` & `dotdrop-1.9.0/dotdrop/cfg_aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         """
         self.path = path
         self.profile_key = profile_key
         self.debug = debug
         self.dry = dry
         self.log = Logger(debug=self.debug)
         self._load()
+        self._validate()
 
     ########################################################
     # public methods
     ########################################################
 
     def del_dotfile(self, dotfile):
         """remove this dotfile from the config"""
@@ -214,14 +215,20 @@
             return None
         return Dotfile(key, dst, src)
 
     ########################################################
     # parsing
     ########################################################
 
+    def _validate(self):
+        """validate fields on top level view of config"""
+        val = self.settings.workdir
+        if not val:
+            raise UndefinedException('\"workdir\" is undefined')
+
     def _load(self, reloading=False):
         """load lower level config"""
         self.cfgyaml = CfgYaml(self.path,
                                self.profile_key,
                                reloading=reloading,
                                debug=self.debug)
```

### Comparing `dotdrop-1.8.2/dotdrop/cfg_yaml.py` & `dotdrop-1.9.0/dotdrop/cfg_yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 import os
 import glob
 import io
 from copy import deepcopy
 from itertools import chain
 from ruamel.yaml import YAML as yaml
+import toml
 
 # local imports
 from dotdrop.version import __version__ as VERSION
 from dotdrop.settings import Settings
 from dotdrop.logger import Logger
 from dotdrop.templategen import Templategen
 from dotdrop.linktypes import LinkTypes
@@ -92,42 +93,50 @@
     key_imp_link = Settings.key_link_on_import
     key_settings_template = Settings.key_template_dotfile_default
 
     # link values
     lnk_nolink = LinkTypes.NOLINK.name.lower()
     lnk_link = LinkTypes.LINK.name.lower()
     lnk_children = LinkTypes.LINK_CHILDREN.name.lower()
+    lnk_absolute = LinkTypes.ABSOLUTE.name.lower()
+    lnk_relative = LinkTypes.RELATIVE.name.lower()
 
     # checks
-    allowed_link_val = [lnk_nolink, lnk_link, lnk_children]
+    allowed_link_val = [lnk_nolink, lnk_link, lnk_children,
+                        lnk_absolute, lnk_relative]
     top_entries = [key_dotfiles, key_settings, key_profiles]
 
     def __init__(self, path, profile=None, addprofiles=None,
-                 reloading=False, debug=False):
+                 reloading=False, debug=False, imported_configs=None):
         """
         config parser
         @path: config file path
         @profile: the selected profile names
         @addprofiles: included profiles names (list)
         @reloading: true when reloading
+        @imported_configs: paths of config files that have been imported so far
         @debug: debug flag
         """
         self._path = os.path.abspath(path)
         self._profile = profile
         self._reloading = reloading
         self._debug = debug
         self._log = Logger(debug=self._debug)
+        # config format
+        self._config_format = 'yaml'
         # config needs to be written
         self._dirty = False
         # indicates the config has been updated
         self._dirty_deprecated = False
         # profile variables
         self._profilevarskeys = []
         # included profiles
         self._inc_profiles = addprofiles or []
+        # imported configs
+        self.imported_configs = imported_configs or []
 
         # init the dictionaries
         self.settings = {}
         self.dotfiles = {}
         self.profiles = {}
         self.actions = {}
         self.trans_r = {}
@@ -213,14 +222,21 @@
 
         self._template_include_entry()
         if self._debug:
             title = 'variables defined (after template include)'
             self._debug_dict(title, self.variables)
 
         ##################################################
+        # template config entries
+        ##################################################
+        entry = self.settings[self.key_settings_dotpath]
+        val = self._template_item(entry)
+        self.settings[self.key_settings_dotpath] = val
+
+        ##################################################
         # parse the other blocks
         ##################################################
 
         # parse the "dotfiles" block
         self.dotfiles = self._parse_blk_dotfiles(self._yaml_dict)
         # parse the "actions" block
         self.actions = self._parse_blk_actions(self._yaml_dict)
@@ -280,16 +296,17 @@
     ########################################################
 
     def _resolve_dotfile_link(self, link):
         """resolve dotfile link entry"""
         newlink = self._template_item(link)
         # check link value
         if newlink not in self.allowed_link_val:
-            err = 'bad value: {}'.format(newlink)
+            err = 'bad link value: {}'.format(newlink)
             self._log.err(err)
+            self._log.err('allowed: {}'.format(self.allowed_link_val))
             raise YamlException('config content error: {}'.format(err))
         return newlink
 
     def resolve_dotfile_src(self, src, templater=None):
         """resolve dotfile src path"""
         newsrc = ''
         if src:
@@ -316,24 +333,37 @@
                 msg = 'dotfile dst: \"{}\" -> \"{}\"'.format(dst, new)
                 self._dbg(msg)
             dst = new
             newdst = self._norm_path(dst)
         return newdst
 
     def add_dotfile_to_profile(self, dotfile_key, profile_key):
-        """add an existing dotfile key to a profile_key"""
+        """
+        add an existing dotfile key to a profile_key
+        we test using profiles variable since it merges
+        imported ones (include, etc) but insert in main
+        yaml only
+        """
+        # create the profile if it doesn't exist
         self._new_profile(profile_key)
-        profile = self._yaml_dict[self.key_profiles][profile_key]
+        profile = self.profiles[profile_key]
+
+        # ensure profile dotfiles list is not None
         if self.key_profile_dotfiles not in profile or \
                 profile[self.key_profile_dotfiles] is None:
             profile[self.key_profile_dotfiles] = []
+            self._yaml_dict[self.key_profiles][profile_key] = []
+
+        # add to the profile
         pdfs = profile[self.key_profile_dotfiles]
         if self.key_all not in pdfs and \
                 dotfile_key not in pdfs:
-            profile[self.key_profile_dotfiles].append(dotfile_key)
+            # append dotfile
+            pro = self._yaml_dict[self.key_profiles][profile_key]
+            pro[self.key_profile_dotfiles].append(dotfile_key)
             if self._debug:
                 msg = 'add \"{}\" to profile \"{}\"'.format(dotfile_key,
                                                             profile_key)
                 msg.format(dotfile_key, profile_key)
                 self._dbg(msg)
             self._dirty = True
         return self._dirty
@@ -447,15 +477,15 @@
             settings[self.key_settings_minversion] = VERSION
 
         # save to file
         if self._debug:
             self._dbg('saving to {}'.format(self._path))
         try:
             with open(self._path, 'w', encoding='utf8') as file:
-                self._yaml_dump(content, file)
+                self._yaml_dump(content, file, fmt=self._config_format)
         except Exception as exc:
             self._log.err(exc)
             err = 'error saving config: {}'.format(self._path)
             raise YamlException(err) from exc
 
         if self._dirty_deprecated:
             warn = 'your config contained deprecated entries'
@@ -465,15 +495,15 @@
         self._dirty = False
         return True
 
     def dump(self):
         """dump the config dictionary"""
         output = io.StringIO()
         content = self._prepare_to_save(self._yaml_dict.copy())
-        self._yaml_dump(content, output)
+        self._yaml_dump(content, output, fmt=self._config_format)
         return output.getvalue()
 
     ########################################################
     # block parsing
     ########################################################
 
     def _parse_blk_settings(self, dic):
@@ -977,15 +1007,16 @@
         """import config from path"""
         if self._debug:
             self._dbg('import config from {}'.format(path))
             self._dbg('profile: {}'.format(self._profile))
             self._dbg('included profiles: {}'.format(self._inc_profiles))
         sub = CfgYaml(path, profile=self._profile,
                       addprofiles=self._inc_profiles,
-                      debug=self._debug)
+                      debug=self._debug,
+                      imported_configs=self.imported_configs)
 
         # settings are ignored from external file
         # except for filter_file and func_file
         self.settings[Settings.key_func_file] += [
             self._norm_path(func_file)
             for func_file in sub.settings[Settings.key_func_file]
         ]
@@ -999,26 +1030,33 @@
         self.profiles = self._merge_dict(self.profiles, sub.profiles,
                                          deep=True)
         self.actions = self._merge_dict(self.actions, sub.actions)
         self.trans_r = self._merge_dict(self.trans_r, sub.trans_r)
         self.trans_w = self._merge_dict(self.trans_w, sub.trans_w)
         self._clear_profile_vars(sub.variables)
 
+        self.imported_configs.append(path)
+        self.imported_configs += sub.imported_configs
+
         if self._debug:
             self._debug_dict('add import_configs var', sub.variables)
         self._add_variables(sub.variables, prio=True)
 
     def _import_configs(self):
         """import configs from external files"""
         # settings -> import_configs
         imp = self.settings.get(self.key_import_configs, None)
         if not imp:
             return
         paths = self._resolve_paths(imp)
         for path in paths:
+            if path in self.imported_configs:
+                err = '{} imported more than once in {}'.format(path,
+                                                                self._path)
+                raise YamlException(err)
             self._import_config(path)
 
     def _import_sub(self, path, key, mandatory=False, patch_func=None):
         """
         import the block "key" from "path"
         patch_func is applied to each element if defined
         """
@@ -1045,14 +1083,17 @@
     def _new_profile(self, key):
         """add a new profile if it doesn't exist"""
         if key not in self.profiles.keys():
             # update yaml_dict
             self._yaml_dict[self.key_profiles][key] = {
                 self.key_profile_dotfiles: []
             }
+            self.profiles[key] = {
+                self.key_profile_dotfiles: []
+            }
             if self._debug:
                 self._dbg('adding new profile: {}'.format(key))
             self._dirty = True
 
     ########################################################
     # handle deprecated entries
     ########################################################
@@ -1098,28 +1139,44 @@
                 cur = dotfile[self.key_dotfile_link]
                 new = self.lnk_nolink
                 if cur:
                     new = self.lnk_link
                 dotfile[self.key_dotfile_link] = new
                 self._dirty = True
                 self._dirty_deprecated = True
-                self._log.warn('deprecated \"link\" value')
+                warn = 'deprecated \"link: <boolean>\"'
+                warn += ', updated to \"link: {}\"'.format(new)
+                self._log.warn(warn)
 
-            elif old_key in dotfile and \
+            if self.key_dotfile_link in dotfile and \
+                    dotfile[self.key_dotfile_link] == self.lnk_link:
+                # patch "link: link"
+                # to "link: absolute"
+                new = self.lnk_absolute
+                dotfile[self.key_dotfile_link] = new
+                self._dirty = True
+                self._dirty_deprecated = True
+                warn = 'deprecated \"link: link\"'
+                warn += ', updated to \"link: {}\"'.format(new)
+                self._log.warn(warn)
+
+            if old_key in dotfile and \
                     isinstance(dotfile[old_key], bool):
                 # patch link_children: <bool>
                 cur = dotfile[old_key]
                 new = self.lnk_nolink
                 if cur:
                     new = self.lnk_children
                 del dotfile[old_key]
                 dotfile[self.key_dotfile_link] = new
                 self._dirty = True
                 self._dirty_deprecated = True
-                self._log.warn('deprecated \"link_children\" value')
+                warn = 'deprecated \"link_children\" value'
+                warn += ', updated to \"{}\"'.format(new)
+                self._log.warn(warn)
 
     ########################################################
     # yaml utils
     ########################################################
 
     def _prepare_to_save(self, content):
         content = self._clear_none(content)
@@ -1141,20 +1198,22 @@
             cfg = '\n'
             with open(path, 'r', encoding='utf8') as file:
                 for line in file:
                     cfg += line
             self._dbg(cfg.rstrip())
             self._dbg('----------end:{}----------'.format(path))
         try:
-            content = self._yaml_load(path)
+            content, fmt = self._yaml_load(path)
+            self._config_format = fmt
         except Exception as exc:
             self._log.err(exc)
             err = 'config yaml error: {}'.format(path)
             raise YamlException(err) from exc
-
+        if self._debug:
+            self._dbg('format: {}'.format(self._config_format))
         return content
 
     def _validate(self, yamldict):
         """validate entries"""
         if not yamldict:
             return
 
@@ -1168,49 +1227,92 @@
         # check link_dotfile_default
         if self.key_settings not in yamldict:
             # no configs top entry
             return
         if not yamldict[self.key_settings]:
             # configs empty
             return
+
+        # check settings values
         settings = yamldict[self.key_settings]
         if self.key_settings_link_dotfile_default not in settings:
             return
         val = settings[self.key_settings_link_dotfile_default]
         if val not in self.allowed_link_val:
-            err = 'bad value: {}'.format(val)
+            err = 'bad link value: {}'.format(val)
             self._log.err(err)
+            self._log.err('allowed: {}'.format(self.allowed_link_val))
             raise YamlException('config content error: {}'.format(err))
 
     @classmethod
     def _yaml_load(cls, path):
+        """load config file"""
+        is_toml = path.lower().endswith(".toml")
+        if is_toml:
+            return cls.__toml_load(path), 'toml'
+        return cls.__yaml_load(path), 'yaml'
+
+    @classmethod
+    def __yaml_load(cls, path):
         """load from yaml"""
         with open(path, 'r', encoding='utf8') as file:
             data = yaml()
             data.typ = 'rt'
             content = data.load(file)
         return content
 
     @classmethod
-    def _yaml_dump(cls, content, where):
+    def __toml_load(cls, path):
+        """load from toml"""
+        with open(path, 'r', encoding='utf8') as file:
+            data = file.read()
+        content = toml.loads(data)
+        # handle inexistent dotfiles/profiles
+        # since toml doesn't have a nul/nil/null/none
+        if cls.key_dotfiles not in content:
+            content[cls.key_dotfiles] = None
+        if cls.key_profiles not in content:
+            content[cls.key_profiles] = None
+        return content
+
+    @classmethod
+    def _yaml_dump(cls, content, file, fmt='yaml'):
+        """dump config file"""
+        if fmt == 'toml':
+            return cls.__toml_dump(content, file)
+        if fmt == 'yaml':
+            return cls.__yaml_dump(content, file)
+        raise YamlException("unsupported format")
+
+    @classmethod
+    def __yaml_dump(cls, content, file):
         """dump to yaml"""
         data = yaml()
         data.default_flow_style = False
         data.indent = 2
         data.typ = 'rt'
-        data.dump(content, where)
+        data.dump(content, file)
+
+    @classmethod
+    def __toml_dump(cls, content, file):
+        """dump to toml"""
+        toml.dump(content, file)
 
     ########################################################
     # templating
     ########################################################
 
     def _redefine_templater(self):
         """create templater based on current variables"""
-        fufile = self.settings[Settings.key_func_file]
-        fifile = self.settings[Settings.key_filter_file]
+        fufile = None
+        fifile = None
+        if Settings.key_func_file in self.settings:
+            fufile = self.settings[Settings.key_func_file]
+        if Settings.key_filter_file in self.settings:
+            fifile = self.settings[Settings.key_filter_file]
         self._tmpl = Templategen(variables=self.variables,
                                  func_file=fufile,
                                  filter_file=fifile)
 
     def _template_item(self, item, exc_if_fail=True):
         """
         template an item using the templategen
@@ -1629,14 +1731,14 @@
 
         # save the config
         content = {'variables': uvars}
         try:
             if self._debug:
                 self._dbg('saving uservariables values to {}'.format(path))
             with open(path, 'w', encoding='utf8') as file:
-                self._yaml_dump(content, file)
+                self._yaml_dump(content, file, fmt=self._config_format)
         except Exception as exc:
             # self._log.err(exc)
             err = 'error saving uservariables to {}'.format(path)
             self._log.err(err)
             raise YamlException(err) from exc
         self._log.log('uservariables values saved to {}'.format(path))
```

### Comparing `dotdrop-1.8.2/dotdrop/comparator.py` & `dotdrop-1.9.0/dotdrop/comparator.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,20 @@
         @debug: enable debug
         """
         self.diff_cmd = diff_cmd
         self.debug = debug
         self.log = Logger(debug=self.debug)
         self.ignore_missing_in_dotdrop = ignore_missing_in_dotdrop
 
-    def compare(self, local_path, deployed_path, ignore=None):
-        """diff local_path (dotdrop dotfile) and
-        deployed_path (destination file)"""
+    def compare(self, local_path, deployed_path, ignore=None, mode=None):
+        """
+        diff local_path (dotdrop dotfile) and
+        deployed_path (destination file)
+        If mode is None, rights will be read from local_path
+        """
         if not ignore:
             ignore = []
         local_path = os.path.expanduser(local_path)
         deployed_path = os.path.expanduser(deployed_path)
         self.log.dbg('comparing {} and {}'.format(
             local_path,
             deployed_path,
@@ -54,27 +57,32 @@
             )
 
         # test content
         if not os.path.isdir(local_path):
             self.log.dbg('{} is a file'.format(local_path))
             ret = self._comp_file(local_path, deployed_path, ignore)
             if not ret:
-                ret = self._comp_mode(local_path, deployed_path)
+                ret = self._comp_mode(local_path, deployed_path, mode=mode)
             return ret
 
         self.log.dbg('{} is a directory'.format(local_path))
 
         ret = self._comp_dir(local_path, deployed_path, ignore)
         if not ret:
-            ret = self._comp_mode(local_path, deployed_path)
+            ret = self._comp_mode(local_path, deployed_path, mode=mode)
         return ret
 
-    def _comp_mode(self, local_path, deployed_path):
-        """compare mode"""
-        local_mode = get_file_perm(local_path)
+    def _comp_mode(self, local_path, deployed_path, mode=None):
+        """
+        compare mode
+        If mode is None, rights will be read on local_path
+        """
+        local_mode = mode
+        if not local_mode:
+            local_mode = get_file_perm(local_path)
         deployed_mode = get_file_perm(deployed_path)
         if local_mode == deployed_mode:
             return ''
         msg = 'mode differ {} ({:o}) and {} ({:o})'
         self.log.dbg(msg.format(local_path, local_mode, deployed_path,
                                 deployed_mode))
         ret = 'modes differ for {} ({:o}) vs {:o}\n'
```

### Comparing `dotdrop-1.8.2/dotdrop/dictparser.py` & `dotdrop-1.9.0/dotdrop/dictparser.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/dotdrop.py` & `dotdrop-1.9.0/dotdrop/dotdrop.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             LOG.log(line.format(dotfile.key, err))
             LOG.err(err)
             return False
         src = insttmp
 
     # compare
     # need to be executed before cleaning
-    diff = comp.compare(src, dotfile.dst, ignore=ignores)
+    diff = comp.compare(src, dotfile.dst, ignore=ignores, mode=dotfile.chmod)
 
     # clean tmp transformed dotfile if any
     if tmpsrc:
         tmpsrc = os.path.join(opts.dotpath, tmpsrc)
         if os.path.exists(tmpsrc):
             removepath(tmpsrc, LOG)
 
@@ -216,33 +216,26 @@
     ignores = list(set(opts.install_ignore + dotfile.instignore))
     ignores = patch_ignores(ignores, dotfile.dst, debug=opts.debug)
 
     is_template = dotfile.template and Templategen.is_template(
         dotfile.src,
         ignore=ignores,
     )
-    if hasattr(dotfile, 'link') and dotfile.link == LinkTypes.LINK:
-        # link
+    if hasattr(dotfile, 'link') and dotfile.link in (
+        LinkTypes.LINK, LinkTypes.LINK_CHILDREN,
+        LinkTypes.RELATIVE, LinkTypes.ABSOLUTE
+    ):
+        # nolink|relative|absolute|link_children
         ret, err = inst.install(templ, dotfile.src, dotfile.dst,
                                 dotfile.link,
                                 actionexec=pre_actions_exec,
                                 is_template=is_template,
                                 ignore=ignores,
                                 chmod=dotfile.chmod,
                                 force_chmod=opts.install_force_chmod)
-    elif hasattr(dotfile, 'link') and \
-            dotfile.link == LinkTypes.LINK_CHILDREN:
-        # link_children
-        ret, err = inst.install(templ, dotfile.src, dotfile.dst,
-                                dotfile.link,
-                                actionexec=pre_actions_exec,
-                                is_template=is_template,
-                                chmod=dotfile.chmod,
-                                ignore=ignores,
-                                force_chmod=opts.install_force_chmod)
     else:
         # nolink
         src = dotfile.src
         tmp = None
         if dotfile.trans_r:
             tmp = apply_trans(opts.dotpath, dotfile, templ, debug=opts.debug)
             if not tmp:
@@ -648,15 +641,15 @@
                 continue
             dotfiles = [dotfile]
 
         for dotfile in dotfiles:
             k = dotfile.key
             # ignore if uses any type of link
             if dotfile.link != LinkTypes.NOLINK:
-                msg = '{} uses link/link_children, remove manually'
+                msg = '{} uses symlink, remove manually'
                 LOG.warn(msg.format(k))
                 continue
 
             LOG.dbg('removing {}'.format(key))
 
             # make sure is part of the profile
             if dotfile.key not in [d.key for d in opts.dotfiles]:
```

### Comparing `dotdrop-1.8.2/dotdrop/dotfile.py` & `dotdrop-1.9.0/dotdrop/dotfile.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/importer.py` & `dotdrop-1.9.0/dotdrop/importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         """
         import a dotfile pointed by path
         returns:
             1: 1 dotfile imported
             0: ignored
             -1: error
         """
+        path = os.path.abspath(path)
         self.log.dbg('import {}'.format(path))
         if not os.path.exists(path):
             self.log.err('\"{}\" does not exist, ignored!'.format(path))
             return -1
 
         return self._import(path, import_as=import_as,
                             import_link=import_link, import_mode=import_mode)
@@ -131,15 +132,15 @@
             1: 1 dotfile imported
             0: ignored
         """
 
         # handle file mode
         chmod = None
         dflperm = get_default_file_perms(dst, self.umask)
-        self.log.dbg('import mode: {}'.format(import_mode))
+        self.log.dbg('import chmod: {}'.format(import_mode))
         if import_mode or perm != dflperm:
             msg = 'adopt mode {:o} (umask {:o})'
             self.log.dbg(msg.format(perm, dflperm))
             chmod = perm
 
         # add file to config file
         retconf = self.conf.new_dotfile(src, dst, linktype, chmod=chmod)
@@ -230,15 +231,16 @@
         for dotfile in dfs:
             profiles = self.conf.get_profiles_by_dotfile_key(dotfile.key)
             profiles = [x.key for x in profiles]
             if self.profile in profiles and \
                     not self.conf.get_dotfile_by_src_dst(src, dst):
                 # same profile
                 # different src
-                self.log.err('duplicate dotfile for this profile')
+                msg = 'duplicate dotfile: {}'
+                self.log.err(msg.format(dotfile.key))
                 return True
         return False
 
     def _ignore(self, path):
         if must_ignore([path], self.ignore, debug=self.debug):
             self.log.dbg('ignoring import of {}'.format(path))
             self.log.warn('{} ignored'.format(path))
```

### Comparing `dotdrop-1.8.2/dotdrop/installer.py` & `dotdrop-1.9.0/dotdrop/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,20 +129,26 @@
                                           noempty=noempty, ignore=ignore,
                                           is_template=is_template)
             else:
                 ret, err = self._copy_file(templater, src, dst,
                                            actionexec=actionexec,
                                            noempty=noempty, ignore=ignore,
                                            is_template=is_template)
-        elif linktype == LinkTypes.LINK:
+        elif linktype in (LinkTypes.LINK, LinkTypes.ABSOLUTE):
             # symlink
-            ret, err = self._link(templater, src, dst,
-                                  actionexec=actionexec,
-                                  is_template=is_template,
-                                  ignore=ignore)
+            ret, err = self._link_absolute(templater, src, dst,
+                                           actionexec=actionexec,
+                                           is_template=is_template,
+                                           ignore=ignore)
+        elif linktype == LinkTypes.RELATIVE:
+            # symlink
+            ret, err = self._link_relative(templater, src, dst,
+                                           actionexec=actionexec,
+                                           is_template=is_template,
+                                           ignore=ignore)
         elif linktype == LinkTypes.LINK_CHILDREN:
             # symlink direct children
             if not isdir:
                 msg = 'symlink children of {} to {}'
                 self.log.dbg(msg.format(src, dst))
                 err = 'source dotfile is not a directory: {}'.format(src)
                 ret = False
@@ -242,18 +248,56 @@
 
         return ret, err, tmpdst
 
     ########################################################
     # low level accessors for public methods
     ########################################################
 
-    def _link(self, templater, src, dst, actionexec=None,
-              is_template=True, ignore=None):
+    def _link_absolute(self, templater, src, dst,
+                       actionexec=None,
+                       is_template=True,
+                       ignore=None):
+        """
+        install link:absolute|link
+
+        return
+        - True, None        : success
+        - False, error_msg  : error
+        - False, None       : ignored
+        - False, 'aborted'    : user aborted
+        """
+        return self._link_dotfile(templater, src, dst,
+                                  actionexec=actionexec,
+                                  is_template=is_template,
+                                  ignore=ignore,
+                                  absolute=True)
+
+    def _link_relative(self, templater, src, dst,
+                       actionexec=None,
+                       is_template=True,
+                       ignore=None):
+        """
+        install link:relative
+
+        return
+        - True, None        : success
+        - False, error_msg  : error
+        - False, None       : ignored
+        - False, 'aborted'    : user aborted
+        """
+        return self._link_dotfile(templater, src, dst,
+                                  actionexec=actionexec,
+                                  is_template=is_template,
+                                  ignore=ignore,
+                                  absolute=False)
+
+    def _link_dotfile(self, templater, src, dst, actionexec=None,
+                      is_template=True, ignore=None, absolute=True):
         """
-        install link:link
+        symlink
 
         return
         - True, None        : success
         - False, error_msg  : error
         - False, None       : ignored
         - False, 'aborted'    : user aborted
         """
@@ -266,15 +310,16 @@
                                     LinkTypes.NOLINK,
                                     actionexec=actionexec,
                                     is_template=is_template,
                                     ignore=ignore)
             if not ret and not os.path.exists(tmp):
                 return ret, err
             src = tmp
-        ret, err = self._symlink(src, dst, actionexec=actionexec)
+        ret, err = self._symlink(src, dst, actionexec=actionexec,
+                                 absolute=absolute)
         return ret, err
 
     def _link_children(self, templater, src, dst,
                        actionexec=None, is_template=True, ignore=None):
         """
         install link:link_children
 
@@ -350,15 +395,15 @@
 
         return installed > 0, None
 
     ########################################################
     # file operations
     ########################################################
 
-    def _symlink(self, src, dst, actionexec=None):
+    def _symlink(self, src, dst, actionexec=None, absolute=True):
         """
         set src as a link target of dst
 
         return
         - True, None        : success
         - False, error_msg  : error
         - False, None       : ignored
@@ -411,17 +456,24 @@
             try:
                 utils.removepath(dst)
             except OSError as exc:
                 err = 'something went wrong with {}: {}'.format(src, exc)
                 return False, err
 
         # create symlink
-        os.symlink(src, dst)
+        lnk_src = src
+        if not absolute:
+            # relative symlink
+            dstrel = dst
+            if not os.path.isdir(dstrel):
+                dstrel = os.path.dirname(dstrel)
+            lnk_src = os.path.relpath(src, dstrel)
+        os.symlink(lnk_src, dst)
         if not self.comparing:
-            self.log.sub('linked {} to {}'.format(dst, src))
+            self.log.sub('linked {} to {}'.format(dst, lnk_src))
         return True, None
 
     def _copy_file(self, templater, src, dst,
                    actionexec=None, noempty=False,
                    ignore=None, is_template=True):
         """
         install src to dst when is a file
```

### Comparing `dotdrop-1.8.2/dotdrop/jhelpers.py` & `dotdrop-1.9.0/dotdrop/jhelpers.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/linktypes.py` & `dotdrop-1.9.0/dotdrop/linktypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 
 class LinkTypes(IntEnum):
     """a type of link"""
     NOLINK = 0
     LINK = 1
     LINK_CHILDREN = 2
+    ABSOLUTE = 3
+    RELATIVE = 4
 
     @classmethod
     def get(cls, key, default=None):
         """get the linktype"""
         try:
             return key if isinstance(key, cls) else cls[key.upper()]
         except KeyError as exc:
```

### Comparing `dotdrop-1.8.2/dotdrop/logger.py` & `dotdrop-1.9.0/dotdrop/logger.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/options.py` & `dotdrop-1.9.0/dotdrop/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 CONFIG = 'config.yaml'
 HOMECFG = '~/.config/{}'.format(NAME)
 ETCXDGCFG = '/etc/xdg/{}'.format(NAME)
 ETCCFG = '/etc/{}'.format(NAME)
 
 OPT_LINK = {
     LinkTypes.NOLINK.name.lower(): LinkTypes.NOLINK,
-    LinkTypes.LINK.name.lower(): LinkTypes.LINK,
+    LinkTypes.ABSOLUTE.name.lower(): LinkTypes.ABSOLUTE,
+    LinkTypes.RELATIVE.name.lower(): LinkTypes.RELATIVE,
     LinkTypes.LINK_CHILDREN.name.lower(): LinkTypes.LINK_CHILDREN}
 
 BANNER = r"""     _       _      _
   __| | ___ | |_ __| |_ __ ___  _ __
  / _` |/ _ \| __/ _` | '__/ _ \| '_ |
  \__,_|\___/ \__\__,_|_|  \___/| .__/  v{}
                                |_|""".format(VERSION)
@@ -78,15 +79,15 @@
   -C --file=<path>        Path of dotfile to compare.
   -d --dry                Dry run.
   -D --showdiff           Show a diff before overwriting.
   -f --force              Do not ask user confirmation for anything.
   -G --grepable           Grepable output.
   -i --ignore=<pattern>   Pattern to ignore.
   -k --key                Treat <path> as a dotfile key.
-  -l --link=<link>        Link option (nolink|link|link_children).
+  -l --link=<link>        Link option (nolink|absolute|relative|link_children).
   -L --file-only          Do not show diff but only the files that differ.
   -m --preserve-mode      Insert a chmod entry in the dotfile with its mode.
   -n --nodiff             Do not diff when installing.
   -p --profile=<profile>  Specify the profile to use [default: {}].
   -P --show-patch         Provide a one-liner to manually patch template.
   -s --as=<path>          Import as a different path from actual path.
   -t --temp               Install to a temporary directory for review.
@@ -322,15 +323,15 @@
             sys.exit(USAGE)
 
         # import link default value
         self.import_link = self.link_on_import
         if self.args['--link']:
             # overwrite default import link with cli switch
             link = self.args['--link']
-            if link not in OPT_LINK.keys():
+            if link not in OPT_LINK:
                 self.log.err('bad option for --link: {}'.format(link))
                 sys.exit(USAGE)
             self.import_link = OPT_LINK[link]
 
         # "files" specifics
         self._apply_args_files()
```

### Comparing `dotdrop-1.8.2/dotdrop/profile.py` & `dotdrop-1.9.0/dotdrop/profile.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/settings.py` & `dotdrop-1.9.0/dotdrop/settings.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/templategen.py` & `dotdrop-1.9.0/dotdrop/templategen.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/updater.py` & `dotdrop-1.9.0/dotdrop/updater.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop/utils.py` & `dotdrop-1.9.0/dotdrop/utils.py`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/dotdrop.egg-info/PKG-INFO` & `dotdrop-1.9.0/dotdrop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 Metadata-Version: 2.1
 Name: dotdrop
-Version: 1.8.2
+Version: 1.9.0
 Summary: Save your dotfiles once, deploy them everywhere
 Home-page: https://github.com/deadc0de6/dotdrop
 Author: deadc0de6
 Author-email: deadc0de6@foo.bar
 License: GPLv3
-Download-URL: https://github.com/deadc0de6/dotdrop/archive/v1.8.2.tar.gz
+Download-URL: https://github.com/deadc0de6/dotdrop/archive/v1.9.0.tar.gz
 Description: # <img src="https://raw.githubusercontent.com/deadc0de6/dotdrop/master/dotdrop.svg" width="100" height="100" align="left"> dotdrop
         <br/>
         <br/>
         
+        [![GitHub release (latest by date)](https://img.shields.io/github/v/release/deadc0de6/dotdrop)](https://github.com/deadc0de6/dotdrop/releases/latest)
+        [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
+        [![GitHub Repo stars](https://img.shields.io/github/stars/deadc0de6/dotdrop?style=social)](https://github.com/deadc0de6/dotdrop/)
+        
         [![Tests Status](https://github.com/deadc0de6/dotdrop/workflows/tests/badge.svg)](https://github.com/deadc0de6/dotdrop/actions)
         [![Doc Status](https://readthedocs.org/projects/dotdrop/badge/?version=latest)](https://dotdrop.readthedocs.io/en/latest/?badge=latest)
-        [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
-        [![Coverage Status](https://coveralls.io/repos/github/deadc0de6/dotdrop/badge.svg?branch=master)](https://coveralls.io/github/deadc0de6/dotdrop?branch=master)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/deadc0de6/dotdrop.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/deadc0de6/dotdrop/context:python)
+        [![Coveralls](https://img.shields.io/coveralls/github/deadc0de6/dotdrop)](https://coveralls.io/github/deadc0de6/dotdrop?branch=master)
+        [![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/deadc0de6/dotdrop?label=code%20quality)](https://lgtm.com/projects/g/deadc0de6/dotdrop/context:python)
         
-        [![PyPI version](https://badge.fury.io/py/dotdrop.svg)](https://badge.fury.io/py/dotdrop)
-        [![AUR](https://img.shields.io/aur/version/dotdrop.svg)](https://aur.archlinux.org/packages/dotdrop)
         [![Python](https://img.shields.io/pypi/pyversions/dotdrop.svg)](https://pypi.python.org/pypi/dotdrop)
         
+        [![PyPI](https://img.shields.io/pypi/v/dotdrop)](https://badge.fury.io/py/dotdrop)
+        [![Homebrew version](https://img.shields.io/homebrew/v/dotdrop)](https://formulae.brew.sh/formula/dotdrop)
+        [![AUR](https://img.shields.io/aur/version/dotdrop.svg)](https://aur.archlinux.org/packages/dotdrop)
+        
         [![Donate](https://img.shields.io/badge/donate-KoFi-blue.svg)](https://ko-fi.com/deadc0de6)
         
         *Save your dotfiles once, deploy them everywhere*
         
         [Dotdrop](https://github.com/deadc0de6/dotdrop) makes the management of dotfiles between different hosts easy.
         It allows you to store your dotfiles in Git and automagically deploy
         different versions of the same file on different setups.
         
-        It also allows you to manage different *sets* of dotfiles.
+        It also allows to manage different *sets* of dotfiles.
         For example, you can have a set of dotfiles for your home laptop and
         a different set for your office desktop. Those sets may overlap, and different
         versions of the same dotfiles can be deployed using different predefined *profiles*.
         Or you may have a main set of dotfiles for your
         everyday host and a subset you only need to deploy to temporary
         hosts (cloud VM etc.) that may be using
         a slightly different version of some of the dotfiles.
         
         Features:
         
         * Sync once every dotfile in Git for different usages
-        * Allow dotfile templating by leveraging [Jinja2](https://palletsprojects.com/p/jinja/)
+        * Allow dotfile templating
         * Dynamically generated dotfile contents with pre-defined variables
         * Comparison between deployed and stored dotfiles
         * Handling multiple profiles with different sets of dotfiles
         * Easily import and update dotfiles
         * Handle files and directories
         * Support symlinking of dotfiles
         * Associate actions to the deployment of specific dotfiles
@@ -55,29 +60,30 @@
         Also check out the [blog post](https://deadc0de.re/articles/dotfiles.html),
         the [example](#getting-started), the [documentation](https://dotdrop.readthedocs.io/) or
         how [people are using dotdrop](https://dotdrop.readthedocs.io/en/latest/misc/people-using-dotdrop/)
         for more.
         
         Quick start:
         ```bash
+        ## using dotdrop as a submodule
         mkdir dotfiles && cd dotfiles
         git init
         git submodule add https://github.com/deadc0de6/dotdrop.git
         pip3 install -r dotdrop/requirements.txt --user
         ./dotdrop/bootstrap.sh
         ./dotdrop.sh --help
         ```
         
         A mirror of this repository is available on GitLab under <https://gitlab.com/deadc0de6/dotdrop>.
         
         ## Why dotdrop?
         
         There exist many tools to manage dotfiles; however, not
-        many allow you to deploy different versions of the same dotfile
-        on different hosts. Moreover, dotdrop allows you to specify the
+        many allow to deploy different versions of the same dotfile
+        on different hosts. Moreover, dotdrop allows to specify the
         set of dotfiles that need to be deployed for a specific profile.
         
         See the [example](#getting-started) for a concrete example of
         why [dotdrop](https://github.com/deadc0de6/dotdrop) rocks.
         
         ---
         
@@ -86,69 +92,30 @@
         * [Installation](#installation)
         * [Getting started](#getting-started)
         * [Documentation](#documentation)
         * [Thank you](#thank-you)
         
         # Installation
         
-        There are multiple ways to install and use dotdrop.
-        It is recommended to install dotdrop [as a submodule](#as-a-submodule)
-        to your dotfiles Git tree. Having dotdrop as a submodule guarantees that anywhere
-        you are cloning your dotfiles Git tree from you'll have dotdrop shipped with it.
-        
-        The below instructions show how to install dotdrop as a submodule. For alternative
-        installation instructions, see the
-        [installation documentation](https://dotdrop.readthedocs.io/en/latest/installation/).
-        
-        Dotdrop is also available on:
-        * pypi: https://pypi.org/project/dotdrop/
-        * aur (stable): https://aur.archlinux.org/packages/dotdrop/
-        * aur (git version): https://aur.archlinux.org/packages/dotdrop-git/
-        * snapcraft: https://snapcraft.io/dotdrop
-        
-        ## As a submodule
-        
-        The following will create a git repository for your dotfiles and
-        keep dotdrop as a submodule:
-        ```bash
-        ## create the repository
-        $ mkdir dotfiles; cd dotfiles
-        $ git init
-        
-        ## install dotdrop as a submodule
-        $ git submodule add https://github.com/deadc0de6/dotdrop.git
-        $ pip3 install -r dotdrop/requirements.txt --user
-        $ ./dotdrop/bootstrap.sh
-        
-        ## use dotdrop
-        $ ./dotdrop.sh --help
-        ```
+        See the [installation instructions](https://dotdrop.readthedocs.io/en/latest/installation/).
         
-        For macOS users, make sure to install `realpath` through Homebrew
-        (part of *coreutils*).
-        
-        Using dotdrop as a submodule will require you to work with dotdrop by
-        using the generated script `dotdrop.sh` at the root
-        of your dotfiles repository. Note that this script updates the submodule
-        automatically unless called with the environment variable `DOTDROP_AUTOUPDATE`
-        set to `no`.
-        
-        To ease the use of dotdrop, it is recommended to add an alias to it in your
-        shell (*~/.bashrc*, *~/.zshrc*, etc.) with the config file path, for example:
-        ```
-        alias dotdrop='<absolute-path-to-dotdrop.sh> --cfg=<path-to-your-config.yaml>'
-        ```
+        Dotdrop is available on:
         
-        Completion scripts exist for `bash`, `zsh` and `fish`; see [the related doc](completion/README.md).
+        * [PyPI](https://pypi.org/project/dotdrop/)
+        * [Homebrew](https://formulae.brew.sh/formula/dotdrop)
+        * [AUR (stable)](https://aur.archlinux.org/packages/dotdrop/)
+        * [AUR (git version)](https://aur.archlinux.org/packages/dotdrop-git/)
+        * [Snapcraft](https://snapcraft.io/dotdrop)
+        * [Pacstall](https://github.com/pacstall/pacstall-programs/blob/master/packages/dotdrop/dotdrop.pacscript)
         
         # Getting started
         
         [Create a new repository](https://dotdrop.readthedocs.io/en/latest/repository-setup/)
         to store your dotfiles with dotdrop. *Init* or *clone* that new repository and
-        [install dotdrop](https://dotdrop.readthedocs.io/en/latest/installation/#as-a-submodule).
+        [install dotdrop](https://dotdrop.readthedocs.io/en/latest/installation).
         
         Then import any dotfiles (files or directories) you want to manage with dotdrop.
         You can either use the default profile (which resolves to the *hostname* of the host
         you are running dotdrop on) or provide it explicitly using the switch `-p`/`--profile`.
         
         Import dotfiles on host *home*:
         ```bash
@@ -358,12 +325,14 @@
 Keywords: dotfiles jinja2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3
 Description-Content-Type: text/markdown; variant=GFM
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `dotdrop-1.8.2/dotdrop.egg-info/SOURCES.txt` & `dotdrop-1.9.0/dotdrop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotdrop-1.8.2/setup.py` & `dotdrop-1.9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,20 +28,22 @@
     python_requires=REQUIRES_PYTHON,
     classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Programming Language :: Python :: 3.5',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
             'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
           ],
 
     keywords='dotfiles jinja2',
     packages=find_packages(exclude=['tests*']),
-    install_requires=['docopt', 'Jinja2', 'ruamel.yaml', 'python-magic', 'packaging', 'requests'],
+    install_requires=['docopt', 'Jinja2', 'ruamel.yaml', 'python-magic', 'packaging', 'requests', 'toml'],
 
     extras_require={
         'dev': ['check-manifest'],
         'test': ['coverage', 'pytest', 'pytest-cov'],
     },
 
     entry_points={
```

