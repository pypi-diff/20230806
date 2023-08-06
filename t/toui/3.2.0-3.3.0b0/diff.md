# Comparing `tmp/toui-3.2.0.tar.gz` & `tmp/toui-3.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-3.2.0.tar", last modified: Wed Aug  2 10:48:01 2023, max compression
+gzip compressed data, was "toui-3.3.0b0.tar", last modified: Sun Aug  6 07:56:16 2023, max compression
```

## Comparing `toui-3.2.0.tar` & `toui-3.3.0b0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.587409 toui-3.2.0/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.2.0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4263 2023-08-02 10:48:01.587409 toui-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.495270 toui-3.2.0/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.2.0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.2.0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.2.0/examples/advanced_example_2_toui_with_javascript.py
--rw-rw-rw-   0        0        0     2119 2023-07-30 07:47:07.000000 toui-3.2.0/examples/advanced_example_3_toui_with_google_sign_in.py
--rw-rw-rw-   0        0        0     3663 2023-07-31 16:08:00.000000 toui-3.2.0/examples/advanced_example_4_toui_with_firebase.py
--rw-rw-rw-   0        0        0     2806 2023-08-02 09:47:46.000000 toui-3.2.0/examples/advanced_example_5_toui_with_sql_user_database.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-08-02 09:47:39.000000 toui-3.2.0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.506632 toui-3.2.0/images/
--rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.2.0/images/icon.png
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.2.0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-08-02 10:48:01.588934 toui-3.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.510161 toui-3.2.0/tests/
--rw-rw-rw-   0        0        0      484 2023-05-15 13:04:45.000000 toui-3.2.0/tests/test_examples.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.567290 toui-3.2.0/toui/
--rw-rw-rw-   0        0        0      283 2023-08-02 09:40:36.000000 toui-3.2.0/toui/__init__.py
--rw-rw-rw-   0        0        0     2511 2023-07-29 20:14:41.000000 toui-3.2.0/toui/_cmd.py
--rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.2.0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.2.0/toui/_helpers.py
--rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.2.0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.2.0/toui/_signals.py
--rw-rw-rw-   0        0        0    50682 2023-07-31 18:08:02.000000 toui-3.2.0/toui/apps.py
--rw-rw-rw-   0        0        0    25891 2023-08-02 09:51:19.000000 toui-3.2.0/toui/elements.py
--rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.2.0/toui/exceptions.py
--rw-rw-rw-   0        0        0    21832 2023-08-02 09:51:30.000000 toui-3.2.0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.2.0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.585411 toui-3.2.0/toui.egg-info/
--rw-rw-rw-   0        0        0     4263 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      217 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 07:56:16.948124 toui-3.3.0b0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.3.0b0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.3.0b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4265 2023-08-06 07:56:16.947127 toui-3.3.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.3.0b0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 07:56:16.538586 toui-3.3.0b0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.3.0b0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.3.0b0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.3.0b0/examples/advanced_example_2_toui_with_javascript.py
+-rw-rw-rw-   0        0        0     2119 2023-07-30 07:47:07.000000 toui-3.3.0b0/examples/advanced_example_3_toui_with_google_sign_in.py
+-rw-rw-rw-   0        0        0     3663 2023-07-31 16:08:00.000000 toui-3.3.0b0/examples/advanced_example_4_toui_with_firebase.py
+-rw-rw-rw-   0        0        0     2806 2023-08-02 09:47:46.000000 toui-3.3.0b0/examples/advanced_example_5_toui_with_sql_user_database.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.3.0b0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.3.0b0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-08-02 09:47:39.000000 toui-3.3.0b0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.3.0b0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.3.0b0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.3.0b0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.3.0b0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:56:16.547595 toui-3.3.0b0/images/
+-rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.3.0b0/images/icon.png
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.3.0b0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-08-06 07:56:16.949122 toui-3.3.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.3.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:56:16.550603 toui-3.3.0b0/tests/
+-rw-rw-rw-   0        0        0      484 2023-05-15 13:04:45.000000 toui-3.3.0b0/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:56:16.923126 toui-3.3.0b0/toui/
+-rw-rw-rw-   0        0        0      288 2023-08-06 07:47:16.000000 toui-3.3.0b0/toui/__init__.py
+-rw-rw-rw-   0        0        0     2511 2023-07-29 20:14:41.000000 toui-3.3.0b0/toui/_cmd.py
+-rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.3.0b0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.3.0b0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.3.0b0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.3.0b0/toui/_signals.py
+-rw-rw-rw-   0        0        0    52054 2023-08-05 06:36:31.000000 toui-3.3.0b0/toui/apps.py
+-rw-rw-rw-   0        0        0    25891 2023-08-02 09:51:19.000000 toui-3.3.0b0/toui/elements.py
+-rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.3.0b0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    21871 2023-08-05 07:05:37.000000 toui-3.3.0b0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.3.0b0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:56:16.945135 toui-3.3.0b0/toui.egg-info/
+-rw-rw-rw-   0        0        0     4265 2023-08-06 07:56:16.000000 toui-3.3.0b0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-08-06 07:56:16.000000 toui-3.3.0b0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 07:56:16.000000 toui-3.3.0b0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-06 07:56:16.000000 toui-3.3.0b0/toui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      217 2023-08-06 07:56:16.000000 toui-3.3.0b0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-06 07:56:16.000000 toui-3.3.0b0/toui.egg-info/top_level.txt
```

### Comparing `toui-3.2.0/LICENSE` & `toui-3.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/PKG-INFO` & `toui-3.3.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.2.0
+Version: 3.3.0b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-3.2.0/README.md` & `toui-3.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/advanced_example_1_toui_blueprint.py` & `toui-3.3.0b0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/advanced_example_2_toui_with_javascript.py` & `toui-3.3.0b0/examples/advanced_example_2_toui_with_javascript.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/advanced_example_3_toui_with_google_sign_in.py` & `toui-3.3.0b0/examples/advanced_example_3_toui_with_google_sign_in.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/advanced_example_4_toui_with_firebase.py` & `toui-3.3.0b0/examples/advanced_example_4_toui_with_firebase.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/advanced_example_5_toui_with_sql_user_database.py` & `toui-3.3.0b0/examples/advanced_example_5_toui_with_sql_user_database.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/example_1_simple_website.py` & `toui-3.3.0b0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/example_2_simple_desktop_app.py` & `toui-3.3.0b0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/example_3_updating_page.py` & `toui-3.3.0b0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/example_4_function_with_arg.py` & `toui-3.3.0b0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/examples/example_5_user_variables.py` & `toui-3.3.0b0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/images/icon.png` & `toui-3.3.0b0/images/icon.png`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/images/logo.png` & `toui-3.3.0b0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/setup.py` & `toui-3.3.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/toui/_cmd.py` & `toui-3.3.0b0/toui/_cmd.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/toui/_helpers.py` & `toui-3.3.0b0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/toui/_javascript_templates.py` & `toui-3.3.0b0/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/toui/_signals.py` & `toui-3.3.0b0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/toui/apps.py` & `toui-3.3.0b0/toui/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -548,24 +548,37 @@
             ``True`` if the user is signed in, and ``False`` if it is not signed in.
 
         """
         self._confirm_user_database_created()
         if not self.username_exists(username) and not self.email_exists(email):
             return False
         if self._user_db_type == "sql":
-            user = self._user_cls.query.filter_by(username=username, password=password, email=email, **other_info).first()
+            filter = {"username": username, **other_info}
+            if email is not None:
+                filter["email"] = email
+            if password is not None:
+                filter["password"] = password
+            user = self._user_cls.query.filter_by(**filter).first()
             if user:
                 login_user(user)
                 self._user_vars._set("user-id", user.id)
                 return True
             else:
                 return False
         elif self._user_db_type == "firebase":
-            user_id = self._firebase_db.where("username", "==", username).get()[0].id
-            return self.signin_user_from_id(user_id)
+            users = self._firebase_db.where("username", "==", username).get()
+            if email is not None:
+                users = users[0].where("email", "==", email).get()
+                if len(users) == 0:
+                    return False
+            if password is not None:
+                users = users[0].where("password", "==", password).get()
+                if len(users) == 0:
+                    return False
+            return self.signin_user_from_id(users[0].id, **other_info)
         
     def signin_user_from_id(self, user_id, **other_info):
         """
         Loads the data of a user from database using the user's ID.
 
         Parameters
         ----------
@@ -587,15 +600,20 @@
                 login_user(user)
                 self._user_vars._set("user-id", user_id)
                 return True
             else:
                 return False
         elif self._user_db_type == "firebase":
             user = firebase_admin.auth.get_user(user_id)
+
             if user:
+                user_dict = user.to_dict()
+                for key, value in other_info.items():
+                    if user_dict.get(key) != value:
+                        return False
                 self._user_vars._set("user-id", user_id)
                 return True
             else:
                 return False
             
     def get_current_user_data(self, key):
         """
@@ -753,15 +771,16 @@
         if self.user_vars._get('user-id'):
             if self._user_db_type == "sql":
                 login_user(self._user_cls.query.filter_by(id=self._user_vars._get("user-id")).first())
             return True
         else:
             return False
         
-    def sign_in_using_google(self, client_id, client_secret, after_auth_url, additional_scopes=None, custom_username=None, **other_params):
+    def sign_in_using_google(self, client_id, client_secret, after_auth_url, additional_scopes=None, custom_username=None, custom_host=None,
+                             **other_params):
         """
         Signs in a user using Google (Experimental).
 
         Make sure to create a Google app first. Also, add the following as an authorized redirect URI to your Google app:
         ``https://<your-domain>/toui-google-sign-in``
         
         Parameters
@@ -779,25 +798,34 @@
         additional_scopes: list, default=None (optional)
             By default, the user allows the app to only access non-sensitive information such as the user's name and email. If you
             want to access more information, you can pass a list of scopes. For more information, see `Google's documentation <https://developers.google.com/identity/protocols/oauth2/scopes>`_.
 
         custom_username: str, default=None (optional)
             If you want to use a custom username instead of the user's email, you can pass it here.
 
+        custom_host: str, default=None (optional)
+            Only use this option if you need to change the scheme and host of the redirect uri. For example,
+            if you want to use ``http://127.0.0.1:5000`` instead of ``http://localhost:5000``, you can pass
+            ``http://127.0.0.1:5000`` here.
+
         other_params: kwargs (optional)
             Keyword arguments that can be passed as parameters to authorization url.For more information, see
             `Google's documentation <https://developers.google.com/identity/protocols/oauth2/web-server#httprest_1>`_.
         """
 
         self._google_data = {"client_id": client_id, "client_secret": client_secret}
         scope = "https://www.googleapis.com/auth/userinfo.email https://www.googleapis.com/auth/userinfo.profile"
         if additional_scopes:
             for s in additional_scopes:
                 scope += f" {s}"
         url = f"/toui-google-sign-in?scope={scope}"
+        if custom_username:
+            url += f"&username={custom_username}"
+        if custom_host:
+            url += f"&host={custom_host}"
         for key, value in other_params.items():
             url += f"&{key}={value}"
         self.user_vars._set('google-after-auth-url', after_auth_url)
         self.open_new_page(url=url)
 
     @_ReqsChecker(['flask-basicauth'])
     def add_restriction(self, username, password):
@@ -1015,15 +1043,18 @@
                     return self._get_user_details_from_google_token(r.json()['access_token'])
         raise Exception(f"Error getting user details from Google. Status code: {r.status_code}. Response: {r.text}")
     
     def _sign_in_using_google(self):
         client_id = self._google_data['client_id']
         client_secret = self._google_data['client_secret']
         scope = request.args.get("scope")
-        redirect_uri = request.base_url
+        if request.args.get("host"):
+            redirect_uri = request.args.get("host") + "/toui-google-sign-in"
+        else:
+            redirect_uri = request.base_url
         response_type = "code"
         access_type = request.args.get("access_type")
         state = request.args.get("state")
         include_granted_scopes = request.args.get("include_granted_scopes")
         enable_granular_consent = request.args.get("enable_granular_consent")
         login_hint = request.args.get("login_hint")
         prompt = request.args.get("prompt")
```

### Comparing `toui-3.2.0/toui/elements.py` & `toui-3.3.0b0/toui/elements.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/toui/pages.py` & `toui-3.3.0b0/toui/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,14 +544,21 @@
             if window.uid == self._uid:
                 return window
             
     def _on_url_request(self, func=None, display_return_value=False):
         self._app._user_vars._gen_sid()
         session['user page'] = copy(self)
         try:
+            pg = session['user page']
+            body_element = pg.get_body_element()
+            if body_element:
+                body_element.set_content(pg._navigation_bar + body_element.to_str()) 
+                body_element.add_content(pg._footer)
+            else:
+                pg.from_str(pg._navigation_bar + pg.to_str() + pg._footer)
             if func:
                 new_return = func()
                 if display_return_value:
                     del session['user page']
                     if "toui-response" in session:
                         response = session['toui-response']
                         if isinstance(new_return, Response):
@@ -559,20 +566,14 @@
                         else:
                             response.set_data(new_return)
                         del session['toui-response']
                         return response
                     else:   
                         return new_return
             pg = session['user page']
-            body_element = pg.get_body_element()
-            if body_element:
-                body_element.set_content(pg._navigation_bar + body_element.to_str()) 
-                body_element.add_content(pg._footer)
-            else:
-                pg.from_str(pg._navigation_bar + pg.to_str() + pg._footer)
             del session['user page']
             if "toui-response" in session:
                 response = session['toui-response']
                 response.set_data(pg.to_str())
                 del session['toui-response']
                 return response
             else:
```

### Comparing `toui-3.2.0/toui/structure.py` & `toui-3.3.0b0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-3.2.0/toui.egg-info/PKG-INFO` & `toui-3.3.0b0/toui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.2.0
+Version: 3.3.0b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-3.2.0/toui.egg-info/SOURCES.txt` & `toui-3.3.0b0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

