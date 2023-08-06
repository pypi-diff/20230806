# Comparing `tmp/garth-0.4.3.tar.gz` & `tmp/garth-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.4.3.tar", last modified: Sat Aug  5 00:08:26 2023, max compression
+gzip compressed data, was "garth-0.4.4.tar", last modified: Sun Aug  6 14:32:18 2023, max compression
```

## Comparing `garth-0.4.3.tar` & `garth-0.4.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.3/LICENSE
--rw-r--r--   0        0        0    13213 2023-08-04 23:00:34.696055 garth-0.4.3/README.md
--rw-r--r--   0        0        0      679 2023-08-01 00:53:18.694307 garth-0.4.3/garth/__init__.py
--rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.3/garth/auth_tokens.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.4.3/garth/exc.py
--rw-r--r--   0        0        0     4879 2023-08-05 00:07:40.543783 garth-0.4.3/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.3/garth/py.typed
--rw-r--r--   0        0        0     4623 2023-08-04 23:41:52.190544 garth-0.4.3/garth/sso.py
--rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.3/garth/stats/__init__.py
--rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.3/garth/stats/_base.py
--rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.3/garth/stats/hrv.py
--rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.3/garth/stats/intensity_minutes.py
--rw-r--r--   0        0        0     3523 2023-08-01 01:10:51.104099 garth-0.4.3/garth/stats/sleep.py
--rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.3/garth/stats/steps.py
--rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.3/garth/stats/stress.py
--rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.3/garth/utils.py
--rw-r--r--   0        0        0       22 2023-08-05 00:03:06.948877 garth-0.4.3/garth/version.py
--rw-r--r--   0        0        0     1221 2023-08-05 00:08:26.429274 garth-0.4.3/pyproject.toml
--rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.3/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.3/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.3/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    50890 2023-08-04 23:53:42.180823 garth-0.4.3/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    54154 2023-08-04 23:59:00.720080 garth-0.4.3/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0    71602 2023-08-04 23:53:07.635030 garth-0.4.3/tests/cassettes/test_login_success_mfa.yaml
--rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.3/tests/cassettes/test_username.yaml
--rw-r--r--   0        0        0     3605 2023-08-04 15:10:55.580644 garth-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.3/tests/stats/cassettes/test_daily_hrv.yaml
--rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.3/tests/stats/cassettes/test_daily_hrv_no_results.yaml
--rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.3/tests/stats/cassettes/test_daily_hrv_paginate.yaml
--rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.3/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
--rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.3/tests/stats/cassettes/test_daily_intensity_minutes.yaml
--rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.3/tests/stats/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.3/tests/stats/cassettes/test_daily_steps.yaml
--rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.3/tests/stats/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.3/tests/stats/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.3/tests/stats/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.3/tests/stats/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.3/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
--rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.3/tests/stats/cassettes/test_weekly_steps.yaml
--rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.3/tests/stats/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.3/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.3/tests/stats/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.3/tests/stats/test_hrv.py
--rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.3/tests/stats/test_intensity_minutes.py
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.3/tests/stats/test_sleep.py
--rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.3/tests/stats/test_steps.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.3/tests/stats/test_stress.py
--rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.3/tests/test_auth_tokens.py
--rw-r--r--   0        0        0     3691 2023-08-04 21:49:04.237670 garth-0.4.3/tests/test_http.py
--rw-r--r--   0        0        0     2684 2023-08-04 23:59:13.586158 garth-0.4.3/tests/test_sso.py
--rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.3/tests/test_utils.py
--rw-r--r--   0        0        0    13665 1970-01-01 00:00:00.000000 garth-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.4/LICENSE
+-rw-r--r--   0        0        0    13296 2023-08-06 14:31:51.031646 garth-0.4.4/README.md
+-rw-r--r--   0        0        0      679 2023-08-01 00:53:18.694307 garth-0.4.4/garth/__init__.py
+-rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.4/garth/auth_tokens.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.4.4/garth/exc.py
+-rw-r--r--   0        0        0     5342 2023-08-06 14:26:25.502817 garth-0.4.4/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.4/garth/py.typed
+-rw-r--r--   0        0        0     4629 2023-08-06 14:15:24.095875 garth-0.4.4/garth/sso.py
+-rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.4/garth/stats/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.4/garth/stats/_base.py
+-rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.4/garth/stats/hrv.py
+-rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.4/garth/stats/intensity_minutes.py
+-rw-r--r--   0        0        0     3523 2023-08-01 01:10:51.104099 garth-0.4.4/garth/stats/sleep.py
+-rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.4/garth/stats/steps.py
+-rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.4/garth/stats/stress.py
+-rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.4/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-08-06 14:31:10.719525 garth-0.4.4/garth/version.py
+-rw-r--r--   0        0        0     1221 2023-08-06 14:32:18.760877 garth-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.4/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.4/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.4/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    50890 2023-08-04 23:53:42.180823 garth-0.4.4/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    54154 2023-08-04 23:59:00.720080 garth-0.4.4/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0    71602 2023-08-04 23:53:07.635030 garth-0.4.4/tests/cassettes/test_login_success_mfa.yaml
+-rw-r--r--   0        0        0     8025 2023-08-06 14:28:03.018233 garth-0.4.4/tests/cassettes/test_refresh_oauth2_token.yaml
+-rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.4/tests/cassettes/test_username.yaml
+-rw-r--r--   0        0        0     3687 2023-08-06 14:29:54.601729 garth-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.4/tests/stats/cassettes/test_daily_hrv.yaml
+-rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.4/tests/stats/cassettes/test_daily_hrv_no_results.yaml
+-rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.4/tests/stats/cassettes/test_daily_hrv_paginate.yaml
+-rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.4/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
+-rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.4/tests/stats/cassettes/test_daily_intensity_minutes.yaml
+-rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.4/tests/stats/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.4/tests/stats/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.4/tests/stats/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.4/tests/stats/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.4/tests/stats/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.4/tests/stats/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.4/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
+-rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.4/tests/stats/cassettes/test_weekly_steps.yaml
+-rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.4/tests/stats/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.4/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.4/tests/stats/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.4/tests/stats/test_hrv.py
+-rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.4/tests/stats/test_intensity_minutes.py
+-rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.4/tests/stats/test_sleep.py
+-rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.4/tests/stats/test_steps.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.4/tests/stats/test_stress.py
+-rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.4/tests/test_auth_tokens.py
+-rw-r--r--   0        0        0     4139 2023-08-06 14:30:50.849184 garth-0.4.4/tests/test_http.py
+-rw-r--r--   0        0        0     2684 2023-08-04 23:59:13.586158 garth-0.4.4/tests/test_sso.py
+-rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.4/tests/test_utils.py
+-rw-r--r--   0        0        0    13748 1970-01-01 00:00:00.000000 garth-0.4.4/PKG-INFO
```

### Comparing `garth-0.4.3/LICENSE` & `garth-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/README.md` & `garth-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 The most important reasoning is to build a library with authentication that
 works on [Google Colab](https://colab.research.google.com/) and doesn't require
 tools like Cloudscraper. Garth, in comparison:
 
 1. Uses OAuth1 and OAuth2 token authentication after initial login
 1. OAuth tokens survive for a year
 1. Supports MFA
+1. Auto-refresh of OAuth2 token when expired
+1. OAuth1 token is valid for one year
 1. Works on Google Colab
 1. Uses Pydantic dataclasses to validate and simplify use of data
 1. Full test coverage
 
 ### Python 3.10+
 
 Google Colab, currently, uses 3.10. We should take advantage of all the goodies
```

### Comparing `garth-0.4.3/garth/__init__.py` & `garth-0.4.4/garth/__init__.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/garth/auth_tokens.py` & `garth-0.4.4/garth/auth_tokens.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/garth/http.py` & `garth-0.4.4/garth/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,17 +78,17 @@
         )
         adapter = HTTPAdapter(max_retries=retry)
         self.sess.mount("https://", adapter)
 
     @property
     def username(self):
         if not self._username:
-            self._username = self.connectapi(
-                "/userprofile-service/socialProfile"
-            )["userName"]
+            profile = self.connectapi("/userprofile-service/socialProfile")
+            assert isinstance(profile, dict)
+            self._username = profile["userName"]
         return self._username
 
     def request(
         self,
         method: str,
         subdomain: str,
         path: str,
@@ -98,14 +98,17 @@
         headers: dict = {},
         **kwargs,
     ) -> Response:
         url = f"https://{subdomain}.{self.domain}{path}"
         if referrer is True and self.last_resp:
             headers["referer"] = self.last_resp.url
         if api:
+            assert self.oauth1_token and self.oauth2_token
+            if self.oauth2_token.expired:
+                self.refresh_oauth2()
             headers["Authorization"] = str(self.oauth2_token)
         self.last_resp = self.sess.request(
             method,
             url,
             headers=headers,
             timeout=self.timeout,
             **kwargs,
@@ -118,14 +121,20 @@
 
     def post(self, *args, **kwargs) -> Response:
         return self.request("POST", *args, **kwargs)
 
     def login(self, *args):
         self.oauth1_token, self.oauth2_token = sso.login(*args, client=self)
 
+    def refresh_oauth2(self):
+        assert self.oauth1_token
+        # There is a way to perform a refresh of an OAuth2 token, but it
+        # appears even Garmin uses this approach when the OAuth2 is expired
+        self.oauth2_token = sso.exchange(self.oauth1_token, self)
+
     def connectapi(self, path: str, **kwargs):
         resp = self.get("connectapi", path, api=True, **kwargs)
         if resp.status_code == 204:
             rv = None
         else:
             rv = resp.json()
         return rv
```

### Comparing `garth-0.4.3/garth/sso.py` & `garth-0.4.4/garth/sso.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 def exchange(oauth1: OAuth1Token, client: "http.Client") -> OAuth2Token:
     sess = GarminOAuth1Session(
         resource_owner_key=oauth1.oauth_token,
         resource_owner_secret=oauth1.oauth_token_secret,
     )
     data = dict(mfa_token=oauth1.mfa_token) if oauth1.mfa_token else {}
     token = sess.post(
-        "https://connectapi.garmin.com/oauth-service/oauth/exchange/user/2.0",
+        f"https://connectapi.{client.domain}/oauth-service/oauth/exchange/user/2.0",
         headers=USER_AGENT
         | {"Content-Type": "application/x-www-form-urlencoded"},
         data=data,
     ).json()
 
     return OAuth2Token(**set_expirations(token))
```

### Comparing `garth-0.4.3/garth/stats/_base.py` & `garth-0.4.4/garth/stats/_base.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/garth/stats/hrv.py` & `garth-0.4.4/garth/stats/hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/garth/stats/intensity_minutes.py` & `garth-0.4.4/garth/stats/intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/garth/stats/sleep.py` & `garth-0.4.4/garth/stats/sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/garth/stats/steps.py` & `garth-0.4.4/garth/stats/steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/garth/stats/stress.py` & `garth-0.4.4/garth/stats/stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/garth/utils.py` & `garth-0.4.4/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/pyproject.toml` & `garth-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
 packages = [
     { include = "garth" },
 ]
-version = "0.4.3"
+version = "0.4.4"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `garth-0.4.3/tests/cassettes/test_client_request.yaml` & `garth-0.4.4/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/cassettes/test_connectapi.yaml` & `garth-0.4.4/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/cassettes/test_exchange.yaml` & `garth-0.4.4/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.4.4/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/cassettes/test_login_success.yaml` & `garth-0.4.4/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/cassettes/test_login_success_mfa.yaml` & `garth-0.4.4/tests/cassettes/test_login_success_mfa.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/cassettes/test_username.yaml` & `garth-0.4.4/tests/cassettes/test_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/conftest.py` & `garth-0.4.4/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 @pytest.fixture
 def authed_client(
     oauth1_token: OAuth1Token, oauth2_token: OAuth2Token
 ) -> Client:
     client = Client()
     try:
         client.load(os.environ["GARTH_HOME"])
+        assert client.oauth2_token
+        assert not client.oauth2_token.expired
     except KeyError:
         client.configure(oauth1_token=oauth1_token, oauth2_token=oauth2_token)
     return client
 
 
 @pytest.fixture
 def vcr(vcr):
```

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_hrv.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_hrv.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_hrv_no_results.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_hrv_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_hrv_paginate.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_hrv_paginate.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_intensity_minutes.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_sleep.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_sleep.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_steps.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_stress.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_daily_stress_pagination.yaml` & `garth-0.4.4/tests/stats/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_sleep_data_get.yaml` & `garth-0.4.4/tests/stats/cassettes/test_sleep_data_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_sleep_data_list.yaml` & `garth-0.4.4/tests/stats/cassettes/test_sleep_data_list.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_weekly_intensity_minutes.yaml` & `garth-0.4.4/tests/stats/cassettes/test_weekly_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_weekly_steps.yaml` & `garth-0.4.4/tests/stats/cassettes/test_weekly_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_weekly_stress.yaml` & `garth-0.4.4/tests/stats/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.4.4/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.4.4/tests/stats/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/test_hrv.py` & `garth-0.4.4/tests/stats/test_hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/test_intensity_minutes.py` & `garth-0.4.4/tests/stats/test_intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/test_sleep.py` & `garth-0.4.4/tests/stats/test_sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/test_steps.py` & `garth-0.4.4/tests/stats/test_steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/stats/test_stress.py` & `garth-0.4.4/tests/stats/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/test_http.py` & `garth-0.4.4/tests/test_http.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import tempfile
+import time
 
 import pytest
 from requests import HTTPError
 
 from garth.auth_tokens import OAuth2Token
 from garth.http import Client
 
@@ -112,16 +113,29 @@
 
 
 @pytest.mark.vcr
 def test_connectapi(authed_client: Client):
     stress = authed_client.connectapi(
         "/usersummary-service/stats/stress/daily/2023-07-21/2023-07-21"
     )
+    assert stress
+    assert isinstance(stress, list)
     assert len(stress) == 1
     assert stress[0]["calendarDate"] == "2023-07-21"
     assert list(stress[0]["values"].keys()) == [
         "highStressDuration",
         "lowStressDuration",
         "overallStressLevel",
         "restStressDuration",
         "mediumStressDuration",
     ]
+
+
+@pytest.mark.vcr
+def test_refresh_oauth2_token(authed_client: Client):
+    assert authed_client.oauth2_token
+    authed_client.oauth2_token.expires_at = int(time.time())
+    assert authed_client.oauth2_token.expired
+    profile = authed_client.connectapi("/userprofile-service/socialProfile")
+    assert profile
+    assert isinstance(profile, dict)
+    assert profile["userName"]
```

### Comparing `garth-0.4.3/tests/test_sso.py` & `garth-0.4.4/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/tests/test_utils.py` & `garth-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.3/PKG-INFO` & `garth-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.4.3
+Version: 0.4.4
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
@@ -57,14 +57,16 @@
 The most important reasoning is to build a library with authentication that
 works on [Google Colab](https://colab.research.google.com/) and doesn't require
 tools like Cloudscraper. Garth, in comparison:
 
 1. Uses OAuth1 and OAuth2 token authentication after initial login
 1. OAuth tokens survive for a year
 1. Supports MFA
+1. Auto-refresh of OAuth2 token when expired
+1. OAuth1 token is valid for one year
 1. Works on Google Colab
 1. Uses Pydantic dataclasses to validate and simplify use of data
 1. Full test coverage
 
 ### Python 3.10+
 
 Google Colab, currently, uses 3.10. We should take advantage of all the goodies
```

