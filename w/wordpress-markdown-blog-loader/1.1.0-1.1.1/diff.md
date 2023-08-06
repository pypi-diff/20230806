# Comparing `tmp/wordpress-markdown-blog-loader-1.1.0.tar.gz` & `tmp/wordpress-markdown-blog-loader-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordpress-markdown-blog-loader-1.1.0.tar", last modified: Wed Apr 12 12:24:00 2023, max compression
+gzip compressed data, was "wordpress-markdown-blog-loader-1.1.1.tar", last modified: Sun Aug  6 18:22:01 2023, max compression
```

## Comparing `wordpress-markdown-blog-loader-1.1.0.tar` & `wordpress-markdown-blog-loader-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.846010 wordpress-markdown-blog-loader-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/check_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/name_to_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/remove_newlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:23:39.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/tests/test_blog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:22:01.452165 wordpress-markdown-blog-loader-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-06 18:22:01.452165 wordpress-markdown-blog-loader-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 18:22:01.452165 wordpress-markdown-blog-loader-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:22:01.448165 wordpress-markdown-blog-loader-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:22:01.452165 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/check_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/name_to_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/remove_newlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:22:01.452165 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-06 18:22:01.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-06 18:22:01.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:22:01.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 18:22:01.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:21:34.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-06 18:22:01.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-06 18:22:01.000000 wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:22:01.452165 wordpress-markdown-blog-loader-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-06 18:21:19.000000 wordpress-markdown-blog-loader-1.1.1/tests/test_blog.py
```

### Comparing `wordpress-markdown-blog-loader-1.1.0/PKG-INFO` & `wordpress-markdown-blog-loader-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,22 @@
-Metadata-Version: 2.1
-Name: wordpress-markdown-blog-loader
-Version: 1.1.0
-Summary: load markdown blogs into wordpress
-Home-page: https://github.com/binxio/wordpress-markdown-blog-loader
-Author: Mark van Holsteijn
-Author-email: markvanholsteijn@binx.io
-License: APL2
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-
 # wordpress-markdown-blog-loader
 This utility loads markdown blogs into Wordpress as a post. It allows you to work on your blog
 in your favorite editor and keeps all your blogs in git.
 
 ## features
 - converts markdown into plain html, with syntax hightlighting support
 - uploads and synchronizes any locally referenced images
 - generates an opengraph image including the title, subtitle and author in Binx.io or xebia.com style
 - sets the Yoast focus keywords
 - sets the canonical url, if specified
 
 ## caveats
 - changing the slug may orphan images
 - removing images from the markdown, will leave dangling images in Wordpress
+- you cannot edit via WP and via the uploader, without confusing yourself
 
 ## required Wordpress Plugins
 
 - [Yoast SEO](https://wordpress.org/plugins/wordpress-seo/)
 - [REST API Meta Support](https://wordpress.org/plugins/rest-api-meta-support/)
 
 Furthermore, you have to enable the Rest API for the [Custom Field Group](https://www.advancedcustomfields.com/resources/wp-rest-api-integration/#enabling-the-rest-api-for-your-acf-fields) for the field `show_header_image`.
@@ -47,20 +27,26 @@
 
 ```
 [DEFAULT]
 host = xebia.com
 
 [xebia.com]
 username = <your wordpress username>
-password = <your application passwoird>
+password = <your application password>
 ```
 Note that the application password is different from the password you use to login to your WordPress installation.
 
 If the site is served through a CDN, you can also set the `api_host` which will be used as the hostname to invoke the WP REST API. 
 
+## Never touch the WP editor again
+
+Once you start to manage your blogs via this uploader, *do not edit* the blog via one of the WP editors. The editors are weird,
+because it appears to make a copy of the content on which you get a WYSIWIG viewer. Unfortunately, it does not detect changes
+in the actual blog content. It will look like your uploaded changes are not applied (but they are).
+
 ## Using the image
 To use the docker image, you have to login using a GitHub container registry access token:
 
 1. Browse to https://github.com/settings/tokens
 2. Create new token with 'read:packages' permission
 3. Copy the token
 4. login to  ghcr.io with Docker.
@@ -68,15 +54,15 @@
    `pbpaste | docker login ghcr.io -u <github username> --password-stdin`
 
 
 ## set an alias
 To use the docker image as a command line utility, create the following alias:
 
 ```bash
-alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:main'
+alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.1
 ```
 
 ## start a new blog
 To start a new blog, type:
 
 ```bash
 $ wp-md posts new \
```

### Comparing `wordpress-markdown-blog-loader-1.1.0/setup.py` & `wordpress-markdown-blog-loader-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="wordpress-markdown-blog-loader",
-    version="1.1.0",
+    version="1.1.1",
     url="https://github.com/binxio/wordpress-markdown-blog-loader",
     license="APL2",
     author="Mark van Holsteijn",
     author_email="markvanholsteijn@binx.io",
     description="load markdown blogs into wordpress",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/__main__.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/__main__.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/api.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/api.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/blog.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/blog.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/check_links.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/check_links.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/download.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/download.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/name_to_email.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/name_to_email.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/new.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/new.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/remove_newlines.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/remove_newlines.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/upload.py` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader/upload.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO` & `wordpress-markdown-blog-loader-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-markdown-blog-loader
-Version: 1.1.0
+Version: 1.1.1
 Summary: load markdown blogs into wordpress
 Home-page: https://github.com/binxio/wordpress-markdown-blog-loader
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: APL2
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -29,14 +29,15 @@
 - generates an opengraph image including the title, subtitle and author in Binx.io or xebia.com style
 - sets the Yoast focus keywords
 - sets the canonical url, if specified
 
 ## caveats
 - changing the slug may orphan images
 - removing images from the markdown, will leave dangling images in Wordpress
+- you cannot edit via WP and via the uploader, without confusing yourself
 
 ## required Wordpress Plugins
 
 - [Yoast SEO](https://wordpress.org/plugins/wordpress-seo/)
 - [REST API Meta Support](https://wordpress.org/plugins/rest-api-meta-support/)
 
 Furthermore, you have to enable the Rest API for the [Custom Field Group](https://www.advancedcustomfields.com/resources/wp-rest-api-integration/#enabling-the-rest-api-for-your-acf-fields) for the field `show_header_image`.
@@ -47,20 +48,26 @@
 
 ```
 [DEFAULT]
 host = xebia.com
 
 [xebia.com]
 username = <your wordpress username>
-password = <your application passwoird>
+password = <your application password>
 ```
 Note that the application password is different from the password you use to login to your WordPress installation.
 
 If the site is served through a CDN, you can also set the `api_host` which will be used as the hostname to invoke the WP REST API. 
 
+## Never touch the WP editor again
+
+Once you start to manage your blogs via this uploader, *do not edit* the blog via one of the WP editors. The editors are weird,
+because it appears to make a copy of the content on which you get a WYSIWIG viewer. Unfortunately, it does not detect changes
+in the actual blog content. It will look like your uploaded changes are not applied (but they are).
+
 ## Using the image
 To use the docker image, you have to login using a GitHub container registry access token:
 
 1. Browse to https://github.com/settings/tokens
 2. Create new token with 'read:packages' permission
 3. Copy the token
 4. login to  ghcr.io with Docker.
@@ -68,15 +75,15 @@
    `pbpaste | docker login ghcr.io -u <github username> --password-stdin`
 
 
 ## set an alias
 To use the docker image as a command line utility, create the following alias:
 
 ```bash
-alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:main'
+alias wp-md='docker run -v $HOME:$HOME -v $HOME/.wordpress.ini:/root/.wordpress.ini -v $PWD:/$PWD -w $PWD ghcr.io/binxio/wordpress-markdown-blog-loader:1.1.1
 ```
 
 ## start a new blog
 To start a new blog, type:
 
 ```bash
 $ wp-md posts new \
```

### Comparing `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt` & `wordpress-markdown-blog-loader-1.1.1/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.1.0/tests/test_blog.py` & `wordpress-markdown-blog-loader-1.1.1/tests/test_blog.py`

 * *Files identical despite different names*

