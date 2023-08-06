# Comparing `tmp/devpi-server-6.9.1.tar.gz` & `tmp/devpi-server-6.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-server-6.9.1.tar", last modified: Sun Jul  2 12:02:56 2023, max compression
+gzip compressed data, was "devpi-server-6.9.2.tar", last modified: Sun Aug  6 10:33:47 2023, max compression
```

## Comparing `devpi-server-6.9.1.tar` & `devpi-server-6.9.2.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.395679 devpi-server-6.9.1/
--rw-r--r--   0 fschulze   (501) staff       (20)      138 2023-07-02 12:02:49.000000 devpi-server-6.9.1/AUTHORS
--rw-r--r--   0 fschulze   (501) staff       (20)    70990 2023-07-02 12:02:49.000000 devpi-server-6.9.1/CHANGELOG
--rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-07-02 12:02:49.000000 devpi-server-6.9.1/LICENSE
--rw-r--r--   0 fschulze   (501) staff       (20)      188 2023-07-02 12:02:49.000000 devpi-server-6.9.1/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     6008 2023-07-02 12:02:56.395806 devpi-server-6.9.1/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     2033 2023-07-02 12:02:49.000000 devpi-server-6.9.1/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.355997 devpi-server-6.9.1/devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       82 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/__main__.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7260 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1195 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/auth_basic.py
--rw-r--r--   0 fschulze   (501) staff       (20)      958 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/auth_devpi.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.362956 devpi-server-6.9.1/devpi_server/cfg/
--rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)      213 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/crontab.template
--rw-r--r--   0 fschulze   (501) staff       (20)      430 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/devpi.service.template
--rw-r--r--   0 fschulze   (501) staff       (20)      455 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/launchd-macos.txt.template
--rw-r--r--   0 fschulze   (501) staff       (20)      619 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-http.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      237 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-location.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      330 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-proxy.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      341 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-server.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)     2065 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/nginx-devpi.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      140 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/supervisor-devpi.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      283 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/supervisord.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)     1694 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/cfg/windows-service.txt.template
--rw-r--r--   0 fschulze   (501) staff       (20)    36622 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/config.py
--rw-r--r--   0 fschulze   (501) staff       (20)      643 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/exceptions.py
--rw-r--r--   0 fschulze   (501) staff       (20)    10069 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/filestore.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8841 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/fileutil.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3579 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/fsck.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6962 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/genconfig.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8555 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/hookspecs.py
--rw-r--r--   0 fschulze   (501) staff       (20)    28123 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/importexport.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1926 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/init.py
--rw-r--r--   0 fschulze   (501) staff       (20)     5921 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/interfaces.py
--rw-r--r--   0 fschulze   (501) staff       (20)    30210 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/keyfs.py
--rw-r--r--   0 fschulze   (501) staff       (20)    24464 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/keyfs_sqlite.py
--rw-r--r--   0 fschulze   (501) staff       (20)    11289 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/keyfs_sqlite_fs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2865 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/keyfs_types.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3751 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/log.py
--rw-r--r--   0 fschulze   (501) staff       (20)    26268 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/main.py
--rw-r--r--   0 fschulze   (501) staff       (20)      952 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/middleware.py
--rw-r--r--   0 fschulze   (501) staff       (20)    39630 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/mirror.py
--rw-r--r--   0 fschulze   (501) staff       (20)    74949 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/model.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3668 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/mythread.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1642 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/passwd.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7018 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/readonly.py
--rw-r--r--   0 fschulze   (501) staff       (20)    52150 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1589 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/sizeof.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.363385 devpi-server-6.9.1/devpi_server/vendor/
--rw-r--r--   0 fschulze   (501) staff       (20)     5030 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/vendor/_pip.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9110 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/view_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)    75592 2023-07-02 12:02:49.000000 devpi-server-6.9.1/devpi_server/views.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.358514 devpi-server-6.9.1/devpi_server.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)     6008 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     4838 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)     1007 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/not-zip-safe
--rw-r--r--   0 fschulze   (501) staff       (20)      235 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       51 2023-07-02 12:02:56.000000 devpi-server-6.9.1/devpi_server.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      549 2023-07-02 12:02:49.000000 devpi-server-6.9.1/pyproject.toml
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.364895 devpi-server-6.9.1/pytest_devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)      863 2023-07-02 12:02:49.000000 devpi-server-6.9.1/pytest_devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       86 2023-07-02 12:02:56.396309 devpi-server-6.9.1/setup.cfg
--rwxr-xr-x   0 fschulze   (501) staff       (20)     4518 2023-07-02 12:02:49.000000 devpi-server-6.9.1/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.386576 devpi-server-6.9.1/test_devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)    46442 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)      504 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/example.py
--rw-r--r--   0 fschulze   (501) staff       (20)    21873 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/functional.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.336688 devpi-server-6.9.1/test_devpi_server/importexportdata/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.386986 devpi-server-6.9.1/test_devpi_server/importexportdata/badindexname/
--rw-r--r--   0 fschulze   (501) staff       (20)      698 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/badindexname/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.387385 devpi-server-6.9.1/test_devpi_server/importexportdata/badusername/
--rw-r--r--   0 fschulze   (501) staff       (20)      719 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/badusername/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.387773 devpi-server-6.9.1/test_devpi_server/importexportdata/basescycle/
--rw-r--r--   0 fschulze   (501) staff       (20)      659 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/basescycle/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.388155 devpi-server-6.9.1/test_devpi_server/importexportdata/createdmodified/
--rw-r--r--   0 fschulze   (501) staff       (20)      423 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/createdmodified/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.388530 devpi-server-6.9.1/test_devpi_server/importexportdata/deletedbase/
--rw-r--r--   0 fschulze   (501) staff       (20)     1603 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/deletedbase/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.388903 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/
--rw-r--r--   0 fschulze   (501) staff       (20)     1413 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.328259 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.328394 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.328514 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.389292 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/
--rw-r--r--   0 fschulze   (501) staff       (20)      780 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.389682 devpi-server-6.9.1/test_devpi_server/importexportdata/modifiedpypi/
--rw-r--r--   0 fschulze   (501) staff       (20)      648 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/modifiedpypi/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.390067 devpi-server-6.9.1/test_devpi_server/importexportdata/nocreatedmodified/
--rw-r--r--   0 fschulze   (501) staff       (20)      485 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/nocreatedmodified/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.390443 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/
--rw-r--r--   0 fschulze   (501) staff       (20)     1610 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.329341 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.329468 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.390826 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.391214 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/
--rw-r--r--   0 fschulze   (501) staff       (20)     2299 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.329986 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.330742 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.391621 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/hello.pkg-1.1.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.392004 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.392385 devpi-server-6.9.1/test_devpi_server/importexportdata/norootpypi/
--rw-r--r--   0 fschulze   (501) staff       (20)      340 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/norootpypi/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.392767 devpi-server-6.9.1/test_devpi_server/importexportdata/nouser/
--rw-r--r--   0 fschulze   (501) staff       (20)      198 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/nouser/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.393201 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/
--rw-r--r--   0 fschulze   (501) staff       (20)     1581 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.334502 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/user/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.334731 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/user/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.393662 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.394066 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/
--rw-r--r--   0 fschulze   (501) staff       (20)     1538 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.335657 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.335869 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.336478 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.394471 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/hello-0.9.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.394926 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/
--rw-r--r--   0 fschulze   (501) staff       (20)        2 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/hello-0.9.tar.gz.toxresult0
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:02:56.395343 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_upload_default/
--rw-r--r--   0 fschulze   (501) staff       (20)      650 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json
--rw-r--r--   0 fschulze   (501) staff       (20)     3056 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/reqmock.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6149 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/simpypi.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9275 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2401 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_authcheck.py
--rw-r--r--   0 fschulze   (501) staff       (20)    17566 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_config.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1064 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)    16223 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_filestore.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4355 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_fileutil.py
--rw-r--r--   0 fschulze   (501) staff       (20)      623 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_genconfig.py
--rw-r--r--   0 fschulze   (501) staff       (20)    47791 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_importexport.py
--rw-r--r--   0 fschulze   (501) staff       (20)    31905 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_keyfs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2877 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_keyfs_sqlite_fs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3965 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_log.py
--rw-r--r--   0 fschulze   (501) staff       (20)    13794 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_main.py
--rw-r--r--   0 fschulze   (501) staff       (20)    51665 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_mirror.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8945 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_mirror_no_project_list.py
--rw-r--r--   0 fschulze   (501) staff       (20)    81466 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_model.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1711 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_mythread.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3112 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_nginx.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1210 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_nginx_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9617 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_permissions.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4527 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_readonly.py
--rw-r--r--   0 fschulze   (501) staff       (20)    56091 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3305 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_replica_functional.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1790 2023-07-02 12:02:49.000000 devpi-server-6.9.1/test_devpi_server/test_reqmock.py
--rw-r--r--   0 fschulze   (501) staff       (20)    16607 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_stage_customizer.py
--rw-r--r--   0 fschulze   (501) staff       (20)     5214 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_streaming.py
--rw-r--r--   0 fschulze   (501) staff       (20)      664 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_streaming_nginx.py
--rw-r--r--   0 fschulze   (501) staff       (20)      669 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_streaming_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)      681 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_streaming_replica_nginx.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4932 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_view_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)   105730 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_views.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3101 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_views_patch.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9465 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_views_push_external.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8899 2023-07-02 12:02:50.000000 devpi-server-6.9.1/test_devpi_server/test_views_status.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1514 2023-07-02 12:02:50.000000 devpi-server-6.9.1/tox.ini
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.419774 devpi-server-6.9.2/
+-rw-r--r--   0 fschulze   (501) staff       (20)      138 2023-08-06 10:33:41.000000 devpi-server-6.9.2/AUTHORS
+-rw-r--r--   0 fschulze   (501) staff       (20)    71146 2023-08-06 10:33:41.000000 devpi-server-6.9.2/CHANGELOG
+-rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-08-06 10:33:41.000000 devpi-server-6.9.2/LICENSE
+-rw-r--r--   0 fschulze   (501) staff       (20)      188 2023-08-06 10:33:41.000000 devpi-server-6.9.2/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)     5565 2023-08-06 10:33:47.419894 devpi-server-6.9.2/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     2033 2023-08-06 10:33:41.000000 devpi-server-6.9.2/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.381574 devpi-server-6.9.2/devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)       82 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/__main__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7260 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1195 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/auth_basic.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      958 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/auth_devpi.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.389174 devpi-server-6.9.2/devpi_server/cfg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      213 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/crontab.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      430 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/devpi.service.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      455 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/launchd-macos.txt.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      619 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/nginx-devpi-caching-http.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      237 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/nginx-devpi-caching-location.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      330 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/nginx-devpi-caching-proxy.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      341 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/nginx-devpi-caching-server.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)     2065 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/nginx-devpi.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      140 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/supervisor-devpi.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      283 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/supervisord.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)     1694 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/cfg/windows-service.txt.template
+-rw-r--r--   0 fschulze   (501) staff       (20)    36622 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      643 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/exceptions.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    10069 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/filestore.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8714 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/fileutil.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3579 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/fsck.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6962 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/genconfig.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8555 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/hookspecs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    28123 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/importexport.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1926 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/init.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     5921 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/interfaces.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    30210 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/keyfs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    24464 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/keyfs_sqlite.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    11289 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/keyfs_sqlite_fs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2865 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/keyfs_types.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3751 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/log.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    26268 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      952 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/middleware.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    39630 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/mirror.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    74949 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/model.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3668 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/mythread.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1642 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/passwd.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7018 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/readonly.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    52150 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1589 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/sizeof.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.389531 devpi-server-6.9.2/devpi_server/vendor/
+-rw-r--r--   0 fschulze   (501) staff       (20)     5030 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/vendor/_pip.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9110 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/view_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    75827 2023-08-06 10:33:41.000000 devpi-server-6.9.2/devpi_server/views.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.384409 devpi-server-6.9.2/devpi_server.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     5565 2023-08-06 10:33:47.000000 devpi-server-6.9.2/devpi_server.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     4838 2023-08-06 10:33:47.000000 devpi-server-6.9.2/devpi_server.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-08-06 10:33:47.000000 devpi-server-6.9.2/devpi_server.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1007 2023-08-06 10:33:47.000000 devpi-server-6.9.2/devpi_server.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-08-06 10:33:47.000000 devpi-server-6.9.2/devpi_server.egg-info/not-zip-safe
+-rw-r--r--   0 fschulze   (501) staff       (20)      235 2023-08-06 10:33:47.000000 devpi-server-6.9.2/devpi_server.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       51 2023-08-06 10:33:47.000000 devpi-server-6.9.2/devpi_server.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      549 2023-08-06 10:33:41.000000 devpi-server-6.9.2/pyproject.toml
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.389961 devpi-server-6.9.2/pytest_devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)      863 2023-08-06 10:33:41.000000 devpi-server-6.9.2/pytest_devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)       86 2023-08-06 10:33:47.420332 devpi-server-6.9.2/setup.cfg
+-rwxr-xr-x   0 fschulze   (501) staff       (20)     4518 2023-08-06 10:33:41.000000 devpi-server-6.9.2/setup.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.410161 devpi-server-6.9.2/test_devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    46442 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      504 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/example.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    21873 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/functional.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.361738 devpi-server-6.9.2/test_devpi_server/importexportdata/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.410554 devpi-server-6.9.2/test_devpi_server/importexportdata/badindexname/
+-rw-r--r--   0 fschulze   (501) staff       (20)      698 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/badindexname/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.410952 devpi-server-6.9.2/test_devpi_server/importexportdata/badusername/
+-rw-r--r--   0 fschulze   (501) staff       (20)      719 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/badusername/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.411338 devpi-server-6.9.2/test_devpi_server/importexportdata/basescycle/
+-rw-r--r--   0 fschulze   (501) staff       (20)      659 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/basescycle/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.411714 devpi-server-6.9.2/test_devpi_server/importexportdata/createdmodified/
+-rw-r--r--   0 fschulze   (501) staff       (20)      423 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/createdmodified/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.412106 devpi-server-6.9.2/test_devpi_server/importexportdata/deletedbase/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1603 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/deletedbase/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.412491 devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1413 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.357762 devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.357884 devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/root/pypi/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.358004 devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.413033 devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/
+-rw-r--r--   0 fschulze   (501) staff       (20)      780 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.413653 devpi-server-6.9.2/test_devpi_server/importexportdata/modifiedpypi/
+-rw-r--r--   0 fschulze   (501) staff       (20)      648 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/modifiedpypi/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.414062 devpi-server-6.9.2/test_devpi_server/importexportdata/nocreatedmodified/
+-rw-r--r--   0 fschulze   (501) staff       (20)      485 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/nocreatedmodified/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.414452 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1610 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.358808 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.358929 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.414848 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.415230 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/
+-rw-r--r--   0 fschulze   (501) staff       (20)     2299 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.359413 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.359706 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.415623 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/hello.pkg-1.1.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.416015 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.416436 devpi-server-6.9.2/test_devpi_server/importexportdata/norootpypi/
+-rw-r--r--   0 fschulze   (501) staff       (20)      340 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/norootpypi/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.416931 devpi-server-6.9.2/test_devpi_server/importexportdata/nouser/
+-rw-r--r--   0 fschulze   (501) staff       (20)      198 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/nouser/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.417478 devpi-server-6.9.2/test_devpi_server/importexportdata/removedindexplugin/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1581 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/removedindexplugin/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.360526 devpi-server-6.9.2/test_devpi_server/importexportdata/removedindexplugin/user/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.360648 devpi-server-6.9.2/test_devpi_server/importexportdata/removedindexplugin/user/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.417868 devpi-server-6.9.2/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.418250 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1538 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.361128 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.361255 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.361561 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.418659 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/hello-0.9.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.419053 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/
+-rw-r--r--   0 fschulze   (501) staff       (20)        2 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/hello-0.9.tar.gz.toxresult0
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-08-06 10:33:47.419446 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_upload_default/
+-rw-r--r--   0 fschulze   (501) staff       (20)      650 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json
+-rw-r--r--   0 fschulze   (501) staff       (20)     3056 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/reqmock.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6144 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/simpypi.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9275 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2401 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_authcheck.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    17566 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1064 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    16223 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_filestore.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4431 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_fileutil.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      623 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_genconfig.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    47791 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_importexport.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    31905 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_keyfs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2877 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_keyfs_sqlite_fs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3965 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_log.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    13794 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    51665 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_mirror.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8945 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_mirror_no_project_list.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    81466 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_model.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1711 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_mythread.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3112 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1210 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_nginx_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9617 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_permissions.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4527 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_readonly.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    56091 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3305 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_replica_functional.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1790 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_reqmock.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    16607 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_stage_customizer.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     5214 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_streaming.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      664 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_streaming_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      669 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_streaming_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      681 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_streaming_replica_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4932 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_view_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)   105730 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_views.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3531 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_views_patch.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9465 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_views_push_external.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8899 2023-08-06 10:33:41.000000 devpi-server-6.9.2/test_devpi_server/test_views_status.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1514 2023-08-06 10:33:41.000000 devpi-server-6.9.2/tox.ini
```

### Comparing `devpi-server-6.9.1/CHANGELOG` & `devpi-server-6.9.2/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 
 
 .. towncrier release notes start
 
+6.9.2 (2023-08-06)
+==================
+
+Bug Fixes
+---------
+
+- Prevent duplicates when adding values to lists in index configuration with ``+=`` operator.
+
+
 6.9.1 (2023-07-02)
 ==================
 
 Bug Fixes
 ---------
 
 - Prevent error in find_pre_existing_file in case of incomplete metadata.
```

### Comparing `devpi-server-6.9.1/LICENSE` & `devpi-server-6.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/PKG-INFO` & `devpi-server-6.9.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-server
-Version: 6.9.1
+Version: 6.9.2
 Summary: devpi-server: reliable private and pypi.org caching server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/server/CHANGELOG
@@ -98,14 +98,23 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+6.9.2 (2023-08-06)
+==================
+
+Bug Fixes
+---------
+
+- Prevent duplicates when adding values to lists in index configuration with ``+=`` operator.
+
+
 6.9.1 (2023-07-02)
 ==================
 
 Bug Fixes
 ---------
 
 - Prevent error in find_pre_existing_file in case of incomplete metadata.
@@ -171,22 +180,7 @@
 
 
 Bug Fixes
 ---------
 
 - Fix #840: Correct url scheme in config if nginx is behind another proxy.
 
-
-6.6.1 (2022-09-12)
-==================
-
-Bug Fixes
----------
-
-- Fix slowdown introduced in 6.6.0 when simple links for mirrors are requested more than once in the same thread.
-
-- Removed preservation of original server uuid during import. Imported state is different from the original server. Replicas could not detect the change and get into an inconsistent state.
-
-- Prevent cache trashing when updating simple links on mirrors for projects with huge number of releases.
-
-- Preserve toxresult filenames during import to keep them being accessible on the same URLs after the fix for #686 in 5.2.0.
-
```

### Comparing `devpi-server-6.9.1/README.rst` & `devpi-server-6.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/auth.py` & `devpi-server-6.9.2/devpi_server/auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/auth_basic.py` & `devpi-server-6.9.2/devpi_server/auth_basic.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/auth_devpi.py` & `devpi-server-6.9.2/devpi_server/auth_devpi.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/cfg/nginx-devpi-caching-http.conf.template` & `devpi-server-6.9.2/devpi_server/cfg/nginx-devpi-caching-http.conf.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/cfg/nginx-devpi.conf.template` & `devpi-server-6.9.2/devpi_server/cfg/nginx-devpi.conf.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/cfg/windows-service.txt.template` & `devpi-server-6.9.2/devpi_server/cfg/windows-service.txt.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/config.py` & `devpi-server-6.9.2/devpi_server/config.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/exceptions.py` & `devpi-server-6.9.2/devpi_server/exceptions.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/filestore.py` & `devpi-server-6.9.2/devpi_server/filestore.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/fileutil.py` & `devpi-server-6.9.2/devpi_server/fileutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,18 +97,16 @@
             stopped = True
             break
         elif opcode == b'R':  # True
             stack_append(True)
         elif opcode == b'T':  # complex
             stack_append(complex(_unpack("!d", read(8))[0], _unpack("!d", read(8))[0]))
         else:
-            # the typo is also in execnet and we compare execnet output directly
-            # in tests, so it needs to be here
             raise LoadError(
-                "unkown opcode %r - wire protocol corruption?" % opcode)
+                "unknown opcode %r - wire protocol corruption?" % opcode)
     if not stopped:
         raise LoadError("didn't get STOP")
     if len(stack) != 1:
         raise LoadError("internal unserialization error")
     return stack_pop(0)
```

### Comparing `devpi-server-6.9.1/devpi_server/fsck.py` & `devpi-server-6.9.2/devpi_server/fsck.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/genconfig.py` & `devpi-server-6.9.2/devpi_server/genconfig.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/hookspecs.py` & `devpi-server-6.9.2/devpi_server/hookspecs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/importexport.py` & `devpi-server-6.9.2/devpi_server/importexport.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/init.py` & `devpi-server-6.9.2/devpi_server/init.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/interfaces.py` & `devpi-server-6.9.2/devpi_server/interfaces.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/keyfs.py` & `devpi-server-6.9.2/devpi_server/keyfs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/keyfs_sqlite.py` & `devpi-server-6.9.2/devpi_server/keyfs_sqlite.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/keyfs_sqlite_fs.py` & `devpi-server-6.9.2/devpi_server/keyfs_sqlite_fs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/keyfs_types.py` & `devpi-server-6.9.2/devpi_server/keyfs_types.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/log.py` & `devpi-server-6.9.2/devpi_server/log.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/main.py` & `devpi-server-6.9.2/devpi_server/main.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/middleware.py` & `devpi-server-6.9.2/devpi_server/middleware.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/mirror.py` & `devpi-server-6.9.2/devpi_server/mirror.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/model.py` & `devpi-server-6.9.2/devpi_server/model.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/mythread.py` & `devpi-server-6.9.2/devpi_server/mythread.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/passwd.py` & `devpi-server-6.9.2/devpi_server/passwd.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/readonly.py` & `devpi-server-6.9.2/devpi_server/readonly.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/replica.py` & `devpi-server-6.9.2/devpi_server/replica.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/sizeof.py` & `devpi-server-6.9.2/devpi_server/sizeof.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/vendor/_pip.py` & `devpi-server-6.9.2/devpi_server/vendor/_pip.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/view_auth.py` & `devpi-server-6.9.2/devpi_server/view_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server/views.py` & `devpi-server-6.9.2/devpi_server/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,15 +412,15 @@
 def version_in_filename(version, filename):
     if version is None:
         # no version set, so skip check
         return True
     if version in filename:
         return True
     # PEP 427 escaped wheels
-    if re.sub(r"[^\w\d.]+", "_", version, re.UNICODE) in filename:
+    if re.sub(r"[^\w\d.]+", "_", version, flags=re.UNICODE) in filename:
         return True
     return False
 
 
 class PyPIView:
     def __init__(self, request):
         self.request = request
@@ -875,28 +875,31 @@
                             400, "The '%s' setting doesn't have value '%s'" % (key, value))
                     if isinstance(ixconfig[key], tuple):
                         ixconfig[key] = tuple(
                             x for x in ixconfig[key] if x != value)
                     else:
                         ixconfig[key].remove(value)
                 elif op == 'add':
-                    if isinstance(ixconfig[key], tuple):
-                        ixconfig[key] += (value,)
-                    else:
-                        ixconfig[key].append(value)
+                    if value not in ixconfig[key]:
+                        if isinstance(ixconfig[key], tuple):
+                            ixconfig[key] += (value,)
+                        else:
+                            ixconfig[key].append(value)
                 elif op == 'set':
                     ixconfig[key] = value
                 elif op == 'drop':
                     ixconfig[key] = RemoveValue
                 else:
                     raise ValueError("Unknown operator '%s'." % op)
             json = ixconfig
         if json.get('type') == 'indexconfig' and 'result' in json:
             json = json['result']
         oldconfig = dict(stage.ixconfig)
+        if 'error_on_noop' in self.request.params and oldconfig == json:
+            apireturn(400, message="The requested modifications resulted in no changes")
         try:
             ixconfig = stage.modify(**json)
         except InvalidIndexconfig as e:
             apireturn(400, message=", ".join(e.messages))
         try:
             stage.customizer.on_modified(self.request, oldconfig)
         except InvalidIndexconfig as e:
```

### Comparing `devpi-server-6.9.1/devpi_server.egg-info/PKG-INFO` & `devpi-server-6.9.2/devpi_server.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-server
-Version: 6.9.1
+Version: 6.9.2
 Summary: devpi-server: reliable private and pypi.org caching server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/server/CHANGELOG
@@ -98,14 +98,23 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+6.9.2 (2023-08-06)
+==================
+
+Bug Fixes
+---------
+
+- Prevent duplicates when adding values to lists in index configuration with ``+=`` operator.
+
+
 6.9.1 (2023-07-02)
 ==================
 
 Bug Fixes
 ---------
 
 - Prevent error in find_pre_existing_file in case of incomplete metadata.
@@ -171,22 +180,7 @@
 
 
 Bug Fixes
 ---------
 
 - Fix #840: Correct url scheme in config if nginx is behind another proxy.
 
-
-6.6.1 (2022-09-12)
-==================
-
-Bug Fixes
----------
-
-- Fix slowdown introduced in 6.6.0 when simple links for mirrors are requested more than once in the same thread.
-
-- Removed preservation of original server uuid during import. Imported state is different from the original server. Replicas could not detect the change and get into an inconsistent state.
-
-- Prevent cache trashing when updating simple links on mirrors for projects with huge number of releases.
-
-- Preserve toxresult filenames during import to keep them being accessible on the same URLs after the fix for #686 in 5.2.0.
-
```

### Comparing `devpi-server-6.9.1/devpi_server.egg-info/SOURCES.txt` & `devpi-server-6.9.2/devpi_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/devpi_server.egg-info/entry_points.txt` & `devpi-server-6.9.2/devpi_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/pyproject.toml` & `devpi-server-6.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/pytest_devpi_server/__init__.py` & `devpi-server-6.9.2/pytest_devpi_server/__init__.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/setup.py` & `devpi-server-6.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
       url="https://devpi.net",
       project_urls={
         'Bug Tracker': 'https://github.com/devpi/devpi/issues',
         'Changelog': 'https://github.com/devpi/devpi/blob/main/server/CHANGELOG',
         'Documentation': 'https://doc.devpi.net',
         'Source Code': 'https://github.com/devpi/devpi'
       },
-      version='6.9.1',
+      version='6.9.2',
       maintainer="Florian Schulze",
       maintainer_email="mail@pyfidelity.com",
       packages=[
         'devpi_server',
         'devpi_server.cfg',
         'devpi_server.vendor',
         'pytest_devpi_server',
```

### Comparing `devpi-server-6.9.1/test_devpi_server/conftest.py` & `devpi-server-6.9.2/test_devpi_server/conftest.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/functional.py` & `devpi-server-6.9.2/test_devpi_server/functional.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/badindexname/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/badindexname/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/badusername/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/badusername/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/basescycle/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/basescycle/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/deletedbase/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/deletedbase/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz` & `devpi-server-6.9.2/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/modifiedpypi/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/modifiedpypi/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/normalization/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/normalization/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/normalization_merge/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/normalization_merge/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/removedindexplugin/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/removedindexplugin/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json` & `devpi-server-6.9.2/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/reqmock.py` & `devpi-server-6.9.2/test_devpi_server/reqmock.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/simpypi.py` & `devpi-server-6.9.2/test_devpi_server/simpypi.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 releases = project['releases']
                 simpypi.add_log(
                     "do_GET", self.path, "found",
                     project['title'], "with", list(releases))
                 start_response(200, headers)
                 self.wfile.write(b'\n'.join(releases))
                 return
-        elif p == ['', 'simple', ''] or p == ['', 'simple']:
+        elif p in (['', 'simple', ''], ['', 'simple']):
             # root listing
             projects = [
                 '<a href="/simple/%s/">%s</a>' % (k, v['title'])
                 for k, v in simpypi.projects.items()]
             simpypi.add_log("do_GET", self.path, "found", list(simpypi.projects))
             start_response(200, headers)
             self.wfile.write(b'\n'.join(x.encode('utf-8') for x in projects))
```

### Comparing `devpi-server-6.9.1/test_devpi_server/test_auth.py` & `devpi-server-6.9.2/test_devpi_server/test_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_authcheck.py` & `devpi-server-6.9.2/test_devpi_server/test_authcheck.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_config.py` & `devpi-server-6.9.2/test_devpi_server/test_config.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_conftest.py` & `devpi-server-6.9.2/test_devpi_server/test_conftest.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_filestore.py` & `devpi-server-6.9.2/test_devpi_server/test_filestore.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_fileutil.py` & `devpi-server-6.9.2/test_devpi_server/test_fileutil.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 def _dumps(obj):
     return _Serializer().save(obj, versioned=False)
 
 
 def test_execnet_opcodes():
     # we need to make sure execnet doesn't change
-    assert list(Unserializer.num2func.keys()) == [
+    assert set(Unserializer.num2func.keys()) == {
         b'@', b'A', b'B', b'C', b'D', b'E', b'F', b'G', b'H', b'I', b'J', b'K',
-        b'L', b'M', b'N', b'O', b'P', b'Q', b'R', b'S', b'T']
+        b'L', b'M', b'N', b'O', b'P', b'Q', b'R', b'S', b'T'}
 
 
 @pytest.mark.parametrize('data, expected', [
     (b'@\x00\x00\x00\x00Q', ()),
     (b'F\x00\x00\x00\x01@\x00\x00\x00\x01Q', (1,)),
     (b'F\x00\x00\x00\x01F\x00\x00\x00\x02@\x00\x00\x00\x02Q', (1, 2)),
     (b'A\x00\x00\x00\x01aQ', b'a'),
@@ -104,15 +104,16 @@
         dumps(object())
     assert msg == str(e.value)
 
 
 def test_loads_bad_data():
     with pytest.raises(_LoadError) as e:
         _loads(b'foo')
-    msg = str(e.value)
+    # fix typo from execnet < 2.x
+    msg = str(e.value).replace('unkown opcode', 'unknown opcode')
     with pytest.raises(LoadError) as e:
         loads(b'foo')
     assert msg == str(e.value)
     with pytest.raises(_LoadError) as e:
         _loads(b'LCQ')
     msg = str(e.value)
     with pytest.raises(LoadError) as e:
```

### Comparing `devpi-server-6.9.1/test_devpi_server/test_genconfig.py` & `devpi-server-6.9.2/test_devpi_server/test_genconfig.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_importexport.py` & `devpi-server-6.9.2/test_devpi_server/test_importexport.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_keyfs.py` & `devpi-server-6.9.2/test_devpi_server/test_keyfs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_keyfs_sqlite_fs.py` & `devpi-server-6.9.2/test_devpi_server/test_keyfs_sqlite_fs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_log.py` & `devpi-server-6.9.2/test_devpi_server/test_log.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_main.py` & `devpi-server-6.9.2/test_devpi_server/test_main.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_mirror.py` & `devpi-server-6.9.2/test_devpi_server/test_mirror.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_mirror_no_project_list.py` & `devpi-server-6.9.2/test_devpi_server/test_mirror_no_project_list.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_model.py` & `devpi-server-6.9.2/test_devpi_server/test_model.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_mythread.py` & `devpi-server-6.9.2/test_devpi_server/test_mythread.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_nginx.py` & `devpi-server-6.9.2/test_devpi_server/test_nginx.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_nginx_replica.py` & `devpi-server-6.9.2/test_devpi_server/test_nginx_replica.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_permissions.py` & `devpi-server-6.9.2/test_devpi_server/test_permissions.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_readonly.py` & `devpi-server-6.9.2/test_devpi_server/test_readonly.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_replica.py` & `devpi-server-6.9.2/test_devpi_server/test_replica.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_replica_functional.py` & `devpi-server-6.9.2/test_devpi_server/test_replica_functional.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_reqmock.py` & `devpi-server-6.9.2/test_devpi_server/test_reqmock.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_stage_customizer.py` & `devpi-server-6.9.2/test_devpi_server/test_stage_customizer.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_streaming.py` & `devpi-server-6.9.2/test_devpi_server/test_streaming.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_streaming_nginx.py` & `devpi-server-6.9.2/test_devpi_server/test_streaming_nginx.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_streaming_replica.py` & `devpi-server-6.9.2/test_devpi_server/test_streaming_replica.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_streaming_replica_nginx.py` & `devpi-server-6.9.2/test_devpi_server/test_streaming_replica_nginx.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_view_auth.py` & `devpi-server-6.9.2/test_devpi_server/test_view_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_views.py` & `devpi-server-6.9.2/test_devpi_server/test_views.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_views_patch.py` & `devpi-server-6.9.2/test_devpi_server/test_views_patch.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,22 @@
         'projects': [],
         'type': 'stage',
         'volatile': True}
     # add to acl_upload
     testapp.patch_json("/foo/dev", ["acl_upload+=bar"])
     r = testapp.get("/foo/dev")
     assert r.json['result']['acl_upload'] == ['foo', 'bar']
+    # add again to acl_upload
+    testapp.patch_json("/foo/dev", ["acl_upload+=bar"])
+    r = testapp.get("/foo/dev")
+    assert r.json['result']['acl_upload'] == ['foo', 'bar']
+    # add again to acl_upload with error
+    r = testapp.patch_json("/foo/dev?error_on_noop", ["acl_upload+=bar"], expect_errors=True)
+    assert r.status_code == 400
+    assert r.json['message'] == "The requested modifications resulted in no changes"
     # remove from acl_upload
     testapp.patch_json("/foo/dev", ["acl_upload-=bar"])
     r = testapp.get("/foo/dev")
     assert r.json['result']['acl_upload'] == ['foo']
     # add to bases
     testapp.patch_json("/foo/dev", ["bases+=root/pypi"])
     r = testapp.get("/foo/dev")
```

### Comparing `devpi-server-6.9.1/test_devpi_server/test_views_push_external.py` & `devpi-server-6.9.2/test_devpi_server/test_views_push_external.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/test_devpi_server/test_views_status.py` & `devpi-server-6.9.2/test_devpi_server/test_views_status.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.9.1/tox.ini` & `devpi-server-6.9.2/tox.ini`

 * *Files identical despite different names*

