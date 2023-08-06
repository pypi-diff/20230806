# Comparing `tmp/cfgparser-1.0.3.tar.gz` & `tmp/cfgparser-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cfgparser-1.0.3.tar", last modified: Sat Jul 30 20:45:34 2022, max compression
+gzip compressed data, was "cfgparser-1.0.4.tar", last modified: Sun Aug  6 02:14:40 2023, max compression
```

## Comparing `cfgparser-1.0.3.tar` & `cfgparser-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-07-30 20:45:34.116729 cfgparser-1.0.3/
--rw-rw-rw-   0        0        0     1215 2022-07-30 20:45:34.115729 cfgparser-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       83 2022-07-29 11:24:17.000000 cfgparser-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2022-07-30 20:45:34.116729 cfgparser-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     7522 2022-07-30 20:43:37.000000 cfgparser-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-30 20:45:34.096750 cfgparser-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2022-07-30 20:45:34.100729 cfgparser-1.0.3/src/cfgparser/
-drwxrwxrwx   0        0        0        0 2022-07-30 20:45:34.111732 cfgparser-1.0.3/src/cfgparser/io/
--rw-rw-rw-   0        0        0        0 2021-10-26 10:16:56.000000 cfgparser-1.0.3/src/cfgparser/io/__init__.py
--rw-rw-rw-   0        0        0      491 2021-10-26 08:47:16.000000 cfgparser-1.0.3/src/cfgparser/io/fileloader.py
--rw-rw-rw-   0        0        0      303 2021-11-29 17:48:46.000000 cfgparser-1.0.3/src/cfgparser/io/jsonfileloader.py
--rw-rw-rw-   0        0        0     3640 2022-07-29 10:45:25.000000 cfgparser-1.0.3/src/cfgparser/json_config_parser.py
-drwxrwxrwx   0        0        0        0 2022-07-30 20:45:34.114729 cfgparser-1.0.3/src/cfgparser/utils/
--rw-rw-rw-   0        0        0        0 2022-07-30 20:09:12.000000 cfgparser-1.0.3/src/cfgparser/utils/__init__.py
--rw-rw-rw-   0        0        0      611 2021-12-14 21:51:47.000000 cfgparser-1.0.3/src/cfgparser/utils/dynamic_type_loader.py
--rw-rw-rw-   0        0        0      462 2022-03-01 17:21:36.000000 cfgparser-1.0.3/src/cfgparser/utils/execution_timer.py
-drwxrwxrwx   0        0        0        0 2022-07-30 20:45:34.107731 cfgparser-1.0.3/src/cfgparser.egg-info/
--rw-rw-rw-   0        0        0     1215 2022-07-30 20:45:33.000000 cfgparser-1.0.3/src/cfgparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2022-07-30 20:45:33.000000 cfgparser-1.0.3/src/cfgparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-30 20:45:33.000000 cfgparser-1.0.3/src/cfgparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-07-30 20:45:33.000000 cfgparser-1.0.3/src/cfgparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-06 02:14:29.000000 cfgparser-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-06 02:14:40.026437 cfgparser-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-06 02:14:29.000000 cfgparser-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 02:14:40.026437 cfgparser-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-08-06 02:14:29.000000 cfgparser-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/cfgparser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/cfgparser/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/io/fileloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/io/jsonfileloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/json_config_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/cfgparser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/utils/dynamic_type_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/utils/execution_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/cfgparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-06 02:14:39.000000 cfgparser-1.0.4/src/cfgparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-06 02:14:39.000000 cfgparser-1.0.4/src/cfgparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 02:14:39.000000 cfgparser-1.0.4/src/cfgparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 02:14:39.000000 cfgparser-1.0.4/src/cfgparser.egg-info/top_level.txt
```

### Comparing `cfgparser-1.0.3/setup.py` & `cfgparser-1.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,150 +1,149 @@
-"""A setuptools based setup module.
-See:
-https://packaging.python.org/guides/distributing-packages-using-setuptools/
-https://github.com/pypa/sampleproject
-"""
-
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-
-# Get the long description from the README file
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-# Arguments marked as "Required" below must be included for upload to PyPI.
-# Fields marked as "Optional" may be commented out.
-
-setup(
-    # This is the name of your project. The first time you publish this
-    # package, this name will be registered for you. It will determine how
-    # users can install this project, e.g.:
-    #
-    # $ pip install sampleproject
-    #
-    # And where it will live on PyPI: https://pypi.org/project/sampleproject/
-    #
-    # There are some restrictions on what makes a valid project name
-    # specification here:
-    # https://packaging.python.org/specifications/core-metadata/#name
-    name="cfgparser",  # Required
-    # Versions should comply with PEP 440:
-    # https://www.python.org/dev/peps/pep-0440/
-    #
-    # For a discussion on single-sourcing the version across setup.py and the
-    # project code, see
-    # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.3",  # Required
-    # This is a one-line description or tagline of what your project does. This
-    # corresponds to the "Summary" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#summary
-    description="Python package that allows to parse typed JSON configs defined by python dataclasses",  # Optional
-    # This is an optional longer description of your project that represents
-    # the body of text which users will see when they visit PyPI.
-    #
-    # Often, this is the same as your README, so you can just read it in from
-    # that file directly (as we have already done above)
-    #
-    # This field corresponds to the "Description" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#description-optional
-    long_description=long_description,  # Optional
-    # Denotes that our long_description is in Markdown; valid values are
-    # text/plain, text/x-rst, and text/markdown
-    #
-    # Optional if long_description is written in reStructuredText (rst) but
-    # required for plain-text or Markdown; if unspecified, "applications should
-    # attempt to render [the long_description] as text/x-rst; charset=UTF-8 and
-    # fall back to text/plain if it is not valid rst" (see link below)
-    #
-    # This field corresponds to the "Description-Content-Type" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
-    long_description_content_type="text/markdown",  # Optional (see note above)
-    # This should be a valid link to your project's main homepage.
-    #
-    # This field corresponds to the "Home-Page" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url="https://github.com/CaRniFeXeR/PythonConfigParser",  # Optional
-    # This should be your name or the name of the organization which owns the
-    # project.
-    author="Florian Kowarsch",  # Optional
-    # This should be a valid email address corresponding to the author listed
-    # above.
-    author_email="flo.kowarsch@yahoo.de",  # Optional
-    # Classifiers help users find your project by categorizing it.
-    #
-    # For a list of valid classifiers, see https://pypi.org/classifiers/
-    classifiers=[  # Optional
-        # How mature is this project? Common values are
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
-        "Development Status :: 3 - Alpha",
-        # Indicate who your project is intended for
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Build Tools",
-        # Pick your license as you wish
-        "License :: OSI Approved :: MIT License",
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate you support Python 3. These classifiers are *not*
-        # checked by 'pip install'. See instead 'python_requires' below.
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3 :: Only",
-    ],
-    # This field adds keywords for your project which will appear on the
-    # project page. What does your project relate to?
-    #
-    # Note that this is a list of additional keywords, separated
-    # by commas, to be used to assist searching for the distribution in a
-    # larger catalog.
-    keywords="config, praser, JSON, typed-parsing, dataclass",  # Optional
-    # When your source code is in a subdirectory under the project root, e.g.
-    # `src/`, it is necessary to specify the `package_dir` argument.
-    package_dir={"": "src"},  # Optional
-    # You can just specify package directories manually here if your project is
-    # simple. Or you can use find_packages().
-    #
-    # Alternatively, if you just want to distribute a single Python file, use
-    # the `py_modules` argument instead as follows, which will expect a file
-    # called `my_module.py` to exist:
-    #
-    #   py_modules=["cfgparser"],
-    #
-    # packages=find_packages(),  # Required
-    packages = ["cfgparser", "cfgparser.io","cfgparser.utils"],
-    # Specify which Python versions you support. In contrast to the
-    # 'Programming Language' classifiers above, 'pip install' will check this
-    # and refuse to install the project if the version does not match. See
-    # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires=">=3.7, <4",
-    # This field lists other packages that your project depends on to run.
-    # Any package you put here will be installed by pip when your project is
-    # installed, so they must be valid existing projects.
-    #
-    # For an analysis of "install_requires" vs pip's requirements files see:
-    # https://packaging.python.org/discussions/install-requires-vs-requirements/
-    install_requires=[],  # Optional
-    # List additional groups of dependencies here (e.g. development
-    # dependencies). Users will be able to install these using the "extras"
-    # syntax, for example:
-    #
-    #   $ pip install sampleproject[dev]
-    #
-    # If there are data files included in your packages that need to be
-    # installed, specify them here.
-    # This field corresponds to the "Project-URL" metadata fields:
-    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
-    #
-    # Examples listed include a pattern for specifying where the package tracks
-    # issues, where the source is hosted, where to say thanks to the package
-    # maintainers, and where to support the project financially. The key is
-    # what's used to render the link text on PyPI.
-    project_urls={  # Optional
-        "Bug Reports": "https://github.com/CaRniFeXeR/PythonConfigParser/issues",
-        "Source": "https://github.com/CaRniFeXeR/PythonConfigParser/",
-    },
+"""A setuptools based setup module.
+See:
+https://packaging.python.org/guides/distributing-packages-using-setuptools/
+https://github.com/pypa/sampleproject
+"""
+
+# Always prefer setuptools over distutils
+from setuptools import setup, find_packages
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+
+# Get the long description from the README file
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+# Arguments marked as "Required" below must be included for upload to PyPI.
+# Fields marked as "Optional" may be commented out.
+
+setup(
+    # This is the name of your project. The first time you publish this
+    # package, this name will be registered for you. It will determine how
+    # users can install this project, e.g.:
+    #
+    # $ pip install sampleproject
+    #
+    # And where it will live on PyPI: https://pypi.org/project/sampleproject/
+    #
+    # There are some restrictions on what makes a valid project name
+    # specification here:
+    # https://packaging.python.org/specifications/core-metadata/#name
+    name="cfgparser",  # Required
+    # Versions should comply with PEP 440:
+    # https://www.python.org/dev/peps/pep-0440/
+    #
+    # For a discussion on single-sourcing the version across setup.py and the
+    # project code, see
+    # https://packaging.python.org/guides/single-sourcing-package-version/
+    version="1.0.4",  # Required
+    # This is a one-line description or tagline of what your project does. This
+    # corresponds to the "Summary" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#summary
+    description="Python package that allows to parse typed JSON configs defined by python dataclasses",  # Optional
+    # This is an optional longer description of your project that represents
+    # the body of text which users will see when they visit PyPI.
+    #
+    # Often, this is the same as your README, so you can just read it in from
+    # that file directly (as we have already done above)
+    #
+    # This field corresponds to the "Description" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#description-optional
+    long_description=long_description,  # Optional
+    # Denotes that our long_description is in Markdown; valid values are
+    # text/plain, text/x-rst, and text/markdown
+    #
+    # Optional if long_description is written in reStructuredText (rst) but
+    # required for plain-text or Markdown; if unspecified, "applications should
+    # attempt to render [the long_description] as text/x-rst; charset=UTF-8 and
+    # fall back to text/plain if it is not valid rst" (see link below)
+    #
+    # This field corresponds to the "Description-Content-Type" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
+    long_description_content_type="text/markdown",  # Optional (see note above)
+    # This should be a valid link to your project's main homepage.
+    #
+    # This field corresponds to the "Home-Page" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#home-page-optional
+    url="https://github.com/CaRniFeXeR/PythonConfigParser",  # Optional
+    # This should be your name or the name of the organization which owns the
+    # project.
+    author="Florian Kowarsch",  # Optional
+    # This should be a valid email address corresponding to the author listed
+    # above.
+    author_email="flo.kowarsch@yahoo.de",  # Optional
+    # Classifiers help users find your project by categorizing it.
+    #
+    # For a list of valid classifiers, see https://pypi.org/classifiers/
+    classifiers=[  # Optional
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        "Development Status :: 3 - Alpha",
+        # Indicate who your project is intended for
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        # Pick your license as you wish
+        "License :: OSI Approved :: MIT License",
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate you support Python 3. These classifiers are *not*
+        # checked by 'pip install'. See instead 'python_requires' below.
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+    ],
+    # This field adds keywords for your project which will appear on the
+    # project page. What does your project relate to?
+    #
+    # Note that this is a list of additional keywords, separated
+    # by commas, to be used to assist searching for the distribution in a
+    # larger catalog.
+    keywords="config, praser, JSON, typed-parsing, dataclass",  # Optional
+    # When your source code is in a subdirectory under the project root, e.g.
+    # `src/`, it is necessary to specify the `package_dir` argument.
+    package_dir={"": "src"},  # Optional
+    # You can just specify package directories manually here if your project is
+    # simple. Or you can use find_packages().
+    #
+    # Alternatively, if you just want to distribute a single Python file, use
+    # the `py_modules` argument instead as follows, which will expect a file
+    # called `my_module.py` to exist:
+    #
+    #   py_modules=["cfgparser"],
+    #
+    packages = ["cfgparser", "cfgparser.io","cfgparser.utils"],   # Required
+    # Specify which Python versions you support. In contrast to the
+    # 'Programming Language' classifiers above, 'pip install' will check this
+    # and refuse to install the project if the version does not match. See
+    # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
+    python_requires=">=3.7, <4",
+    # This field lists other packages that your project depends on to run.
+    # Any package you put here will be installed by pip when your project is
+    # installed, so they must be valid existing projects.
+    #
+    # For an analysis of "install_requires" vs pip's requirements files see:
+    # https://packaging.python.org/discussions/install-requires-vs-requirements/
+    install_requires=[],  # Optional
+    # List additional groups of dependencies here (e.g. development
+    # dependencies). Users will be able to install these using the "extras"
+    # syntax, for example:
+    #
+    #   $ pip install sampleproject[dev]
+    #
+    # If there are data files included in your packages that need to be
+    # installed, specify them here.
+    # This field corresponds to the "Project-URL" metadata fields:
+    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
+    #
+    # Examples listed include a pattern for specifying where the package tracks
+    # issues, where the source is hosted, where to say thanks to the package
+    # maintainers, and where to support the project financially. The key is
+    # what's used to render the link text on PyPI.
+    project_urls={  # Optional
+        "Bug Reports": "https://github.com/CaRniFeXeR/PythonConfigParser/issues",
+        "Source": "https://github.com/CaRniFeXeR/PythonConfigParser/",
+    },
 )
```

