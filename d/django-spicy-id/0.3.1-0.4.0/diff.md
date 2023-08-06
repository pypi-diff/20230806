# Comparing `tmp/django-spicy-id-0.3.1.tar.gz` & `tmp/django-spicy-id-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-spicy-id-0.3.1.tar", last modified: Wed Dec 14 20:51:34 2022, max compression
+gzip compressed data, was "django-spicy-id-0.4.0.tar", last modified: Fri Jun 23 18:04:57 2023, max compression
```

## Comparing `django-spicy-id-0.3.1.tar` & `django-spicy-id-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:51:34.116984 django-spicy-id-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-12-14 20:51:30.000000 django-spicy-id-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2022-12-14 20:51:34.116984 django-spicy-id-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2022-12-14 20:51:30.000000 django-spicy-id-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:51:34.112984 django-spicy-id-0.3.1/django_spicy_id/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2022-12-14 20:51:30.000000 django-spicy-id-0.3.1/django_spicy_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2022-12-14 20:51:30.000000 django-spicy-id-0.3.1/django_spicy_id/baseconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-14 20:51:30.000000 django-spicy-id-0.3.1/django_spicy_id/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2022-12-14 20:51:30.000000 django-spicy-id-0.3.1/django_spicy_id/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:51:34.116984 django-spicy-id-0.3.1/django_spicy_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2022-12-14 20:51:34.000000 django-spicy-id-0.3.1/django_spicy_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-14 20:51:34.000000 django-spicy-id-0.3.1/django_spicy_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 20:51:34.000000 django-spicy-id-0.3.1/django_spicy_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-14 20:51:34.000000 django-spicy-id-0.3.1/django_spicy_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-14 20:51:34.000000 django-spicy-id-0.3.1/django_spicy_id.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      614 2022-12-14 20:51:30.000000 django-spicy-id-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2022-12-14 20:51:34.116984 django-spicy-id-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-14 20:51:30.000000 django-spicy-id-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:04:57.986354 django-spicy-id-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-06-23 18:04:57.986354 django-spicy-id-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:04:57.986354 django-spicy-id-0.4.0/django_spicy_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/django_spicy_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/django_spicy_id/baseconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/django_spicy_id/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/django_spicy_id/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/django_spicy_id/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:04:57.986354 django-spicy-id-0.4.0/django_spicy_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-06-23 18:04:57.000000 django-spicy-id-0.4.0/django_spicy_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 18:04:57.000000 django-spicy-id-0.4.0/django_spicy_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:04:57.000000 django-spicy-id-0.4.0/django_spicy_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 18:04:57.000000 django-spicy-id-0.4.0/django_spicy_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 18:04:57.000000 django-spicy-id-0.4.0/django_spicy_id.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-23 18:04:57.990354 django-spicy-id-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 18:04:54.000000 django-spicy-id-0.4.0/setup.py
```

### Comparing `django-spicy-id-0.3.1/LICENSE.txt` & `django-spicy-id-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-spicy-id-0.3.1/PKG-INFO` & `django-spicy-id-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: django-spicy-id
-Version: 0.3.1
-Summary: Fancy ID fields for django models.
-Home-page: https://github.com/mik3y/django-spicy-id
-Author: mik3y
-Author-email: opensource@hoho.com
-License: MIT
-Keywords: django timeseries
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8.1
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # django-spicy-id
 
 A drop-in replacement for Django's `AutoField` that gives you "Stripe-style" self-identifying string object IDs, like `user_1234`.
 
 **Status:** Experimental! No warranty. See `LICENSE.txt`.
 
 [![PyPI version](https://badge.fury.io/py/django-spicy-id.svg)](https://badge.fury.io/py/django-spicy-id)
@@ -46,17 +17,21 @@
 - [Installation](#installation)
   - [Requirements](#requirements)
   - [Instructions](#instructions)
 - [Usage](#usage)
   - [Field types](#field-types)
   - [Required Parameters](#required-parameters)
   - [Optional Parameters](#optional-parameters)
+  - [Registering URLs](#registering-urls)
   - [Field Attributes](#field-attributes)
     - [`.validate_string(strval)`](#validate_stringstrval)
     - [`.re`](#re)
+    - [`.re_pattern`](#re_pattern)
+  - [Utility methods](#utility-methods)
+    - [`get_url_converter(model_class, field_name)`](#get_url_convertermodel_class-field_name)
   - [Errors](#errors)
     - [`django.db.utils.ProgrammingError`](#djangodbutilsprogrammingerror)
     - [`django_spicy_id.MalformedSpicyIdError`](#django_spicy_idmalformedspicyiderror)
 - [Tips and tricks](#tips-and-tricks)
   - [Don't change field configuration](#dont-change-field-configuration)
 - [Changelog](#changelog)
 
@@ -161,27 +136,81 @@
 - **`pad`**: Whether the encoded portion of the id should be zero-padded so that all values are the same string length. Either `False` (default) or `True`.
   - Example without padding: `user_8M0kX`
   - Example with padding: `user_0000008M0kX`
 - **`randomize`**: If `True`, the default value of a new record will be generated randomly using `secrets.randbelow()`. If `False` (the default), works just like a normal `AutoField` i.e. the default value comes from the database upon `INSERT`.
   - When `randomize` is set, an error will be thrown if `default` is also set, since `randomize` is essentially a special and built-in `default` function.
   - If you use this feature, be aware of its hazards: 
       - The generated ID may conflict with an existing row, with probability [determined by the birthday problem](https://en.wikipedia.org/wiki/Birthday_problem#Probability_table) (i.e. the column size and the size of the existing dataset).
-      - A conflict can also arise if two processes generate the same value for `secrets.randbelow()` (i.e. if system entropy is identical or misconfigured for some reason),
+      - A conflict can also arise if two processes generate the same value for `secrets.randbelow()` (i.e. if system entropy is identical or misconfigured for some reason).
+
+### Registering URLs
+
+When installing routes that must match a specific spicy id, you can use the `get_url_converter()` helper method to install a Django [custom path converter](https://docs.djangoproject.com/en/3.2/topics/http/urls/#registering-custom-path-converters).
+
+Using this method will ensure that _only_ valid spicy ID strings for that field will be presented to your view.
+
+Example:
+
+```py
+# models.py
+class User(models.model):
+    id = SpicyBigAutoField(primary_key=True, prefix='usr')
+```
+
+```py
+# urls.py
+from . import models
+from django.urls import path, register_converter
+from django_spicy_id import get_url_converter
+
+# Register the pattern for `User.id` as "spicy_user_id". You should do this
+# once for each unique spicy ID field.
+register_converter(get_url_converter(models.User, 'id'), 'spicy_user_id')
+
+urlpatterns = [
+    path('users/<spicy_user_id:id>', views.user_detail),
+    ...
+]
+```
+
+```py
+# views.py
+
+def user_detail(request, id):
+  user = models.User.objects.get(id=id)
+  ...
+```
 
 ### Field Attributes
 
 The following attributes are available on the field once constructed
 
 #### `.validate_string(strval)`
 
 Checks whether `strval` is a legal value for the field, throwing `django_spicy_id.errors.MalformedSpicyIdError` if not.
 
 #### `.re`
 
-A compiled regex which can be used to validate a string, e.g. in Django `urlpatterns`.
+A compiled regex which can be used to validate a string.
+
+#### `.re_pattern`
+
+A string regex pattern which can be used to validate a string. Unlike the pattern used in `re`, this pattern does not include the leading `^` and trailing `$` boundary characters, making it easier to use in things like Django url patterns.
+
+You probably don't need to use this directly, instead see `get_url_converter()`.
+
+### Utility methods
+
+These utility methods are provided on the top-level `django_spicy_id` module.
+
+#### `get_url_converter(model_class, field_name)`
+
+Returns a Django [custom path converter](https://docs.djangoproject.com/en/3.2/topics/http/urls/#registering-custom-path-converters) for `field_name` on `model_class`.
+
+See [Registering URLs](#registering-urls) for example usage.
 
 ### Errors
 
 #### `django.db.utils.ProgrammingError`
 
 Thrown when attempting to access or query this field using an illegal value. Some examples of this situation:
 
@@ -208,8 +237,8 @@
 
 Although the stored row IDs are never changed, any spicy IDs generated previously, with a different encoding configuration, may now be invalid or (potentially catastrophically) resolve to a different object.
 
 For just one example, `user_10` would naturally refer to a different numeric row id if parsed as `hex` versus `base62` or `base58`. You should avoid changing the field configuration.
 
 ## Changelog
 
-See [`CHANGELOG.md`](https://github.com/mik3y/django-spicy-id/blob/main/CHANGELOG.md) for a summary of changes.
+See [`CHANGELOG.md`](https://github.com/mik3y/django-spicy-id/blob/main/CHANGELOG.md) for a summary of changes.
```

### Comparing `django-spicy-id-0.3.1/README.md` & `django-spicy-id-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: django-spicy-id
+Version: 0.4.0
+Summary: Fancy ID fields for django models.
+Home-page: https://github.com/mik3y/django-spicy-id
+Author: mik3y
+Author-email: opensource@hoho.com
+License: MIT
+Keywords: django timeseries
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8.1
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # django-spicy-id
 
 A drop-in replacement for Django's `AutoField` that gives you "Stripe-style" self-identifying string object IDs, like `user_1234`.
 
 **Status:** Experimental! No warranty. See `LICENSE.txt`.
 
 [![PyPI version](https://badge.fury.io/py/django-spicy-id.svg)](https://badge.fury.io/py/django-spicy-id)
@@ -17,17 +46,21 @@
 - [Installation](#installation)
   - [Requirements](#requirements)
   - [Instructions](#instructions)
 - [Usage](#usage)
   - [Field types](#field-types)
   - [Required Parameters](#required-parameters)
   - [Optional Parameters](#optional-parameters)
+  - [Registering URLs](#registering-urls)
   - [Field Attributes](#field-attributes)
     - [`.validate_string(strval)`](#validate_stringstrval)
     - [`.re`](#re)
+    - [`.re_pattern`](#re_pattern)
+  - [Utility methods](#utility-methods)
+    - [`get_url_converter(model_class, field_name)`](#get_url_convertermodel_class-field_name)
   - [Errors](#errors)
     - [`django.db.utils.ProgrammingError`](#djangodbutilsprogrammingerror)
     - [`django_spicy_id.MalformedSpicyIdError`](#django_spicy_idmalformedspicyiderror)
 - [Tips and tricks](#tips-and-tricks)
   - [Don't change field configuration](#dont-change-field-configuration)
 - [Changelog](#changelog)
 
@@ -132,27 +165,81 @@
 - **`pad`**: Whether the encoded portion of the id should be zero-padded so that all values are the same string length. Either `False` (default) or `True`.
   - Example without padding: `user_8M0kX`
   - Example with padding: `user_0000008M0kX`
 - **`randomize`**: If `True`, the default value of a new record will be generated randomly using `secrets.randbelow()`. If `False` (the default), works just like a normal `AutoField` i.e. the default value comes from the database upon `INSERT`.
   - When `randomize` is set, an error will be thrown if `default` is also set, since `randomize` is essentially a special and built-in `default` function.
   - If you use this feature, be aware of its hazards: 
       - The generated ID may conflict with an existing row, with probability [determined by the birthday problem](https://en.wikipedia.org/wiki/Birthday_problem#Probability_table) (i.e. the column size and the size of the existing dataset).
-      - A conflict can also arise if two processes generate the same value for `secrets.randbelow()` (i.e. if system entropy is identical or misconfigured for some reason),
+      - A conflict can also arise if two processes generate the same value for `secrets.randbelow()` (i.e. if system entropy is identical or misconfigured for some reason).
+
+### Registering URLs
+
+When installing routes that must match a specific spicy id, you can use the `get_url_converter()` helper method to install a Django [custom path converter](https://docs.djangoproject.com/en/3.2/topics/http/urls/#registering-custom-path-converters).
+
+Using this method will ensure that _only_ valid spicy ID strings for that field will be presented to your view.
+
+Example:
+
+```py
+# models.py
+class User(models.model):
+    id = SpicyBigAutoField(primary_key=True, prefix='usr')
+```
+
+```py
+# urls.py
+from . import models
+from django.urls import path, register_converter
+from django_spicy_id import get_url_converter
+
+# Register the pattern for `User.id` as "spicy_user_id". You should do this
+# once for each unique spicy ID field.
+register_converter(get_url_converter(models.User, 'id'), 'spicy_user_id')
+
+urlpatterns = [
+    path('users/<spicy_user_id:id>', views.user_detail),
+    ...
+]
+```
+
+```py
+# views.py
+
+def user_detail(request, id):
+  user = models.User.objects.get(id=id)
+  ...
+```
 
 ### Field Attributes
 
 The following attributes are available on the field once constructed
 
 #### `.validate_string(strval)`
 
 Checks whether `strval` is a legal value for the field, throwing `django_spicy_id.errors.MalformedSpicyIdError` if not.
 
 #### `.re`
 
-A compiled regex which can be used to validate a string, e.g. in Django `urlpatterns`.
+A compiled regex which can be used to validate a string.
+
+#### `.re_pattern`
+
+A string regex pattern which can be used to validate a string. Unlike the pattern used in `re`, this pattern does not include the leading `^` and trailing `$` boundary characters, making it easier to use in things like Django url patterns.
+
+You probably don't need to use this directly, instead see `get_url_converter()`.
+
+### Utility methods
+
+These utility methods are provided on the top-level `django_spicy_id` module.
+
+#### `get_url_converter(model_class, field_name)`
+
+Returns a Django [custom path converter](https://docs.djangoproject.com/en/3.2/topics/http/urls/#registering-custom-path-converters) for `field_name` on `model_class`.
+
+See [Registering URLs](#registering-urls) for example usage.
 
 ### Errors
 
 #### `django.db.utils.ProgrammingError`
 
 Thrown when attempting to access or query this field using an illegal value. Some examples of this situation:
 
@@ -179,8 +266,8 @@
 
 Although the stored row IDs are never changed, any spicy IDs generated previously, with a different encoding configuration, may now be invalid or (potentially catastrophically) resolve to a different object.
 
 For just one example, `user_10` would naturally refer to a different numeric row id if parsed as `hex` versus `base62` or `base58`. You should avoid changing the field configuration.
 
 ## Changelog
 
-See [`CHANGELOG.md`](https://github.com/mik3y/django-spicy-id/blob/main/CHANGELOG.md) for a summary of changes.
+See [`CHANGELOG.md`](https://github.com/mik3y/django-spicy-id/blob/main/CHANGELOG.md) for a summary of changes.
```

### Comparing `django-spicy-id-0.3.1/django_spicy_id/baseconv.py` & `django-spicy-id-0.4.0/django_spicy_id/baseconv.py`

 * *Files identical despite different names*

### Comparing `django-spicy-id-0.3.1/django_spicy_id/fields.py` & `django-spicy-id-0.4.0/django_spicy_id/fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,28 +41,32 @@
             f"^({escaped_preamble})([{digits_without_pad_char}][{digits}]{{,{trailer_len}}})$"
         )
     else:
         return re.compile(f"^({escaped_preamble})([{digits}]{{{char_len}}})$")
 
 
 class BaseSpicyAutoField(models.BigAutoField):
-    """An auto field that is rendered as a prefixed string."""
+    """An AutoField that is rendered as a prefixed string."""
 
     NUM_BITS = None  # Must be defined in subclasses.
 
     def __init__(
         self,
         prefix,
         sep="_",
         encoding=ENCODING_BASE_62,
         randomize=False,
         pad=False,
         *args,
         **kwargs,
     ):
+        if not self.NUM_BITS:
+            raise NotImplemented(
+                "attempt to init abstract base class, or subclass has failed to set NUM_BITS"
+            )
         if encoding not in CODECS_BY_ENCODING:
             raise ImproperlyConfigured(f'unknown encoding "{encoding}"')
         if not isinstance(prefix, str):
             raise ImproperlyConfigured("prefix must be a string")
         if not isinstance(sep, str):
             raise ImproperlyConfigured("sep must be a string")
         if not sep.isascii():
@@ -81,14 +85,22 @@
 
         self.encoding = encoding
         self.codec = CODECS_BY_ENCODING[self.encoding]
         self.max_value = 2 ** (self.NUM_BITS - 1) - 1
         self.max_characters = math.ceil(math.log(self.max_value, len(self.codec.digits)))
         self.re = get_regex(f"{self.prefix}{self.sep}", self.codec, self.pad, self.max_characters)
 
+        # Expose the re pattern without word boundaries, for use in places where they
+        # would interfere (like urlpatterns).
+        #
+        # TODO(mikey): Expose `.as_converter()`, generating a Django URLpatterns converter
+        # class, as a further convenience.
+        # Ref: https://docs.djangoproject.com/en/4.1/topics/http/urls/#registering-custom-path-converters
+        self.re_pattern = self.re.pattern[1:-1]
+
         super().__init__(*args, **kwargs)
 
     def _to_string(self, intvalue):
         encoded = self.codec.encode(intvalue)
         unpadded_len = len(encoded)
         if self.pad and unpadded_len < self.max_characters:
             pad_char = self.codec.digits[0]
@@ -167,16 +179,22 @@
         kwargs["encoding"] = self.encoding
         kwargs["randomize"] = self.randomize
         kwargs["pad"] = self.pad
         return name, path, args, kwargs
 
 
 class SpicyBigAutoField(BaseSpicyAutoField, models.BigAutoField):
+    """A Spicy ID field that is backed by a standard 64-bit Django BigAutoField."""
+
     NUM_BITS = 64
 
 
 class SpicyAutoField(BaseSpicyAutoField, models.AutoField):
+    """A Spicy ID field that is backed by a standard 32-bit Django AutoField."""
+
     NUM_BITS = 32
 
 
 class SpicySmallAutoField(BaseSpicyAutoField, models.SmallAutoField):
+    """A Spicy ID field that is backed by a standard 16-bit Django SmallAutoField."""
+
     NUM_BITS = 16
```

### Comparing `django-spicy-id-0.3.1/django_spicy_id.egg-info/PKG-INFO` & `django-spicy-id-0.4.0/django_spicy_id.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-spicy-id
-Version: 0.3.1
+Version: 0.4.0
 Summary: Fancy ID fields for django models.
 Home-page: https://github.com/mik3y/django-spicy-id
 Author: mik3y
 Author-email: opensource@hoho.com
 License: MIT
 Keywords: django timeseries
 Platform: any
@@ -46,17 +46,21 @@
 - [Installation](#installation)
   - [Requirements](#requirements)
   - [Instructions](#instructions)
 - [Usage](#usage)
   - [Field types](#field-types)
   - [Required Parameters](#required-parameters)
   - [Optional Parameters](#optional-parameters)
+  - [Registering URLs](#registering-urls)
   - [Field Attributes](#field-attributes)
     - [`.validate_string(strval)`](#validate_stringstrval)
     - [`.re`](#re)
+    - [`.re_pattern`](#re_pattern)
+  - [Utility methods](#utility-methods)
+    - [`get_url_converter(model_class, field_name)`](#get_url_convertermodel_class-field_name)
   - [Errors](#errors)
     - [`django.db.utils.ProgrammingError`](#djangodbutilsprogrammingerror)
     - [`django_spicy_id.MalformedSpicyIdError`](#django_spicy_idmalformedspicyiderror)
 - [Tips and tricks](#tips-and-tricks)
   - [Don't change field configuration](#dont-change-field-configuration)
 - [Changelog](#changelog)
 
@@ -161,27 +165,81 @@
 - **`pad`**: Whether the encoded portion of the id should be zero-padded so that all values are the same string length. Either `False` (default) or `True`.
   - Example without padding: `user_8M0kX`
   - Example with padding: `user_0000008M0kX`
 - **`randomize`**: If `True`, the default value of a new record will be generated randomly using `secrets.randbelow()`. If `False` (the default), works just like a normal `AutoField` i.e. the default value comes from the database upon `INSERT`.
   - When `randomize` is set, an error will be thrown if `default` is also set, since `randomize` is essentially a special and built-in `default` function.
   - If you use this feature, be aware of its hazards: 
       - The generated ID may conflict with an existing row, with probability [determined by the birthday problem](https://en.wikipedia.org/wiki/Birthday_problem#Probability_table) (i.e. the column size and the size of the existing dataset).
-      - A conflict can also arise if two processes generate the same value for `secrets.randbelow()` (i.e. if system entropy is identical or misconfigured for some reason),
+      - A conflict can also arise if two processes generate the same value for `secrets.randbelow()` (i.e. if system entropy is identical or misconfigured for some reason).
+
+### Registering URLs
+
+When installing routes that must match a specific spicy id, you can use the `get_url_converter()` helper method to install a Django [custom path converter](https://docs.djangoproject.com/en/3.2/topics/http/urls/#registering-custom-path-converters).
+
+Using this method will ensure that _only_ valid spicy ID strings for that field will be presented to your view.
+
+Example:
+
+```py
+# models.py
+class User(models.model):
+    id = SpicyBigAutoField(primary_key=True, prefix='usr')
+```
+
+```py
+# urls.py
+from . import models
+from django.urls import path, register_converter
+from django_spicy_id import get_url_converter
+
+# Register the pattern for `User.id` as "spicy_user_id". You should do this
+# once for each unique spicy ID field.
+register_converter(get_url_converter(models.User, 'id'), 'spicy_user_id')
+
+urlpatterns = [
+    path('users/<spicy_user_id:id>', views.user_detail),
+    ...
+]
+```
+
+```py
+# views.py
+
+def user_detail(request, id):
+  user = models.User.objects.get(id=id)
+  ...
+```
 
 ### Field Attributes
 
 The following attributes are available on the field once constructed
 
 #### `.validate_string(strval)`
 
 Checks whether `strval` is a legal value for the field, throwing `django_spicy_id.errors.MalformedSpicyIdError` if not.
 
 #### `.re`
 
-A compiled regex which can be used to validate a string, e.g. in Django `urlpatterns`.
+A compiled regex which can be used to validate a string.
+
+#### `.re_pattern`
+
+A string regex pattern which can be used to validate a string. Unlike the pattern used in `re`, this pattern does not include the leading `^` and trailing `$` boundary characters, making it easier to use in things like Django url patterns.
+
+You probably don't need to use this directly, instead see `get_url_converter()`.
+
+### Utility methods
+
+These utility methods are provided on the top-level `django_spicy_id` module.
+
+#### `get_url_converter(model_class, field_name)`
+
+Returns a Django [custom path converter](https://docs.djangoproject.com/en/3.2/topics/http/urls/#registering-custom-path-converters) for `field_name` on `model_class`.
+
+See [Registering URLs](#registering-urls) for example usage.
 
 ### Errors
 
 #### `django.db.utils.ProgrammingError`
 
 Thrown when attempting to access or query this field using an illegal value. Some examples of this situation:
```

### Comparing `django-spicy-id-0.3.1/setup.cfg` & `django-spicy-id-0.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-spicy-id
-version = 0.3.1
+version = 0.4.0
 description = Fancy ID fields for django models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mik3y/django-spicy-id
 author = mik3y
 author_email = opensource@hoho.com
 license = MIT
```

