# Comparing `tmp/tiktok-dlpy-1.3.1.tar.gz` & `tmp/tiktok-dlpy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok-dlpy-1.3.1.tar", last modified: Mon Jul 31 21:45:39 2023, max compression
+gzip compressed data, was "tiktok-dlpy-1.4.0.tar", last modified: Sat Aug  5 22:53:09 2023, max compression
```

## Comparing `tiktok-dlpy-1.3.1.tar` & `tiktok-dlpy-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 21:45:39.106501 tiktok-dlpy-1.3.1/
--rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.3.1/LICENSE
--rw-r--r--   0 becky      (501) staff       (20)      545 2023-07-31 21:45:39.106554 tiktok-dlpy-1.3.1/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      539 2023-07-31 21:43:57.000000 tiktok-dlpy-1.3.1/README.md
--rw-r--r--   0 becky      (501) staff       (20)       79 2023-07-31 21:45:39.106751 tiktok-dlpy-1.3.1/setup.cfg
--rw-r--r--   0 becky      (501) staff       (20)      805 2023-07-31 21:44:43.000000 tiktok-dlpy-1.3.1/setup.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 21:45:39.105862 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/
--rw-r--r--   0 becky      (501) staff       (20)      545 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      331 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/SOURCES.txt
--rw-r--r--   0 becky      (501) staff       (20)        1 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/dependency_links.txt
--rw-r--r--   0 becky      (501) staff       (20)       40 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/requires.txt
--rw-r--r--   0 becky      (501) staff       (20)        9 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/top_level.txt
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 21:45:39.106411 tiktok-dlpy-1.3.1/tiktokdl/
--rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.3.1/tiktokdl/__init__.py
--rw-r--r--   0 becky      (501) staff       (20)    14813 2023-07-31 21:44:03.000000 tiktok-dlpy-1.3.1/tiktokdl/download_post.py
--rw-r--r--   0 becky      (501) staff       (20)      434 2023-07-19 23:43:36.000000 tiktok-dlpy-1.3.1/tiktokdl/exceptions.py
--rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.3.1/tiktokdl/image_processing.py
--rw-r--r--   0 becky      (501) staff       (20)      560 2023-07-31 21:43:57.000000 tiktok-dlpy-1.3.1/tiktokdl/post_data.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-08-05 22:53:09.593004 tiktok-dlpy-1.4.0/
+-rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.4.0/LICENSE
+-rw-r--r--   0 becky      (501) staff       (20)      545 2023-08-05 22:53:09.593093 tiktok-dlpy-1.4.0/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      577 2023-08-05 22:33:17.000000 tiktok-dlpy-1.4.0/README.md
+-rw-r--r--   0 becky      (501) staff       (20)       79 2023-08-05 22:53:09.593327 tiktok-dlpy-1.4.0/setup.cfg
+-rw-r--r--   0 becky      (501) staff       (20)      805 2023-08-05 17:03:30.000000 tiktok-dlpy-1.4.0/setup.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-08-05 22:53:09.590541 tiktok-dlpy-1.4.0/tests/
+-rw-r--r--   0 becky      (501) staff       (20)     4690 2023-08-04 17:22:47.000000 tiktok-dlpy-1.4.0/tests/test_dataclasses.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-08-05 22:53:09.591387 tiktok-dlpy-1.4.0/tiktok_dlpy.egg-info/
+-rw-r--r--   0 becky      (501) staff       (20)      545 2023-08-05 22:53:09.000000 tiktok-dlpy-1.4.0/tiktok_dlpy.egg-info/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      357 2023-08-05 22:53:09.000000 tiktok-dlpy-1.4.0/tiktok_dlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 becky      (501) staff       (20)        1 2023-08-05 22:53:09.000000 tiktok-dlpy-1.4.0/tiktok_dlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 becky      (501) staff       (20)       40 2023-08-05 22:53:09.000000 tiktok-dlpy-1.4.0/tiktok_dlpy.egg-info/requires.txt
+-rw-r--r--   0 becky      (501) staff       (20)        9 2023-08-05 22:53:09.000000 tiktok-dlpy-1.4.0/tiktok_dlpy.egg-info/top_level.txt
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-08-05 22:53:09.592754 tiktok-dlpy-1.4.0/tiktokdl/
+-rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.4.0/tiktokdl/__init__.py
+-rw-r--r--   0 becky      (501) staff       (20)    17418 2023-08-05 17:06:55.000000 tiktok-dlpy-1.4.0/tiktokdl/download_post.py
+-rw-r--r--   0 becky      (501) staff       (20)      563 2023-08-05 15:45:38.000000 tiktok-dlpy-1.4.0/tiktokdl/exceptions.py
+-rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.4.0/tiktokdl/image_processing.py
+-rw-r--r--   0 becky      (501) staff       (20)      560 2023-07-31 21:43:57.000000 tiktok-dlpy-1.4.0/tiktokdl/post_data.py
```

### Comparing `tiktok-dlpy-1.3.1/LICENSE` & `tiktok-dlpy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.3.1/PKG-INFO` & `tiktok-dlpy-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tiktok-dlpy
-Version: 1.3.1
+Version: 1.4.0
 Summary: A package to download TikTok videos or slideshows by URL without needing to login
 Home-page: https://github.com/Fluxticks/TikTokDL
-Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v1.3.1.tar.gz
+Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v1.4.0.tar.gz
 Author: Fluxticks
 Keywords: tiktok,playwright,async
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
```

### Comparing `tiktok-dlpy-1.3.1/README.md` & `tiktok-dlpy-1.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # TikTokDL
 
 A python package to download TikTok videos or slideshows by URL without needing to login.
 
+## TODO
+
+- Cleanup `download_post.py`
+
 ## Usage
 
 1. Install the package
 
 ```bash
 $ pip install tiktok-dlpy
 ```
@@ -24,13 +28,13 @@
 ```
 
 3. Run the function in an async context
 
 ```python
 video_or_slide_url = ""
 
-video_info = asyncio.run(
+post_info = asyncio.run(
     get_post(
         video_or_slide_url
     )
 )
 ```
```

### Comparing `tiktok-dlpy-1.3.1/setup.py` & `tiktok-dlpy-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tiktok-dlpy",
-    version="1.3.1",
+    version="1.4.0",
     url="https://github.com/Fluxticks/TikTokDL",
-    download_url="https://github.com/Fluxticks/TikTokDL/archive/v1.3.1.tar.gz",
+    download_url="https://github.com/Fluxticks/TikTokDL/archive/v1.4.0.tar.gz",
     author="Fluxticks",
     packages=find_packages(),
     install_requires=[
         "bs4",
         "lxml",
         "playwright",
         "numpy",
```

### Comparing `tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/PKG-INFO` & `tiktok-dlpy-1.4.0/tiktok_dlpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tiktok-dlpy
-Version: 1.3.1
+Version: 1.4.0
 Summary: A package to download TikTok videos or slideshows by URL without needing to login
 Home-page: https://github.com/Fluxticks/TikTokDL
-Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v1.3.1.tar.gz
+Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v1.4.0.tar.gz
 Author: Fluxticks
 Keywords: tiktok,playwright,async
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
```

### Comparing `tiktok-dlpy-1.3.1/tiktokdl/download_post.py` & `tiktok-dlpy-1.4.0/tiktokdl/download_post.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 import inspect
 import json
-from datetime import datetime
 import random
 import time
+from asyncio import sleep as async_sleep
+from datetime import datetime
+from os.path import curdir
+from os.path import sep as PATH_SEP
 from typing import Literal
 from urllib.parse import parse_qs, urlparse
 from urllib.request import urlretrieve
 
 from bs4 import BeautifulSoup
+from playwright.async_api import BrowserContext
 from playwright.async_api import Error as PlaywrightError
-from playwright.async_api import Page, Request, BrowserContext
+from playwright.async_api import Page, Request
 from playwright.async_api import TimeoutError as PlaywrightTimeoutError
 from playwright.async_api import async_playwright
 
-from tiktokdl.exceptions import CaptchaFailedException, DownloadFailedException, ResponseParseException
+from tiktokdl.exceptions import (CaptchaFailedException, DownloadFailedException, ResponseParseException, TikTokBaseException)
 from tiktokdl.image_processing import find_position, image_from_url
-from tiktokdl.post_data import TikTokVideo, TikTokSlide, TikTokPost
+from tiktokdl.post_data import TikTokPost, TikTokSlide, TikTokVideo
 
 __all__ = ["get_post"]
 
 
+def __validate_download_path(download_path: str | None):
+    if download_path is None:
+        download_path = f"{curdir}{PATH_SEP}"
+
+    if not download_path.endswith(PATH_SEP):
+        download_path += PATH_SEP
+
+    return download_path
+
+
 def __parse_captcha_params_from_url(url: str) -> dict:
     parsed_url = urlparse(url, allow_fragments=False)
     params = parse_qs(parsed_url.query)
     out = {}
     for key, value in params.items():
         out[key] = value[0]
     return out
@@ -66,41 +80,35 @@
     timestamp = datetime.fromtimestamp(int(post_data.get("createTime")))
     like_count = post_data.get("stats").get("diggCount")
     share_count = post_data.get("stats").get("shareCount")
     comment_count = post_data.get("stats").get("commentCount")
     view_count = post_data.get("stats").get("playCount")
 
     post = TikTokPost(
-            url=post_url,
-            post_id=post_id,
-            author_username=username,
-            author_display_name=display_name,
-            author_avatar=avatar,
-            author_url=author_url,
-            post_download_setting=post_download_setting,
-            post_description=post_description,
-            timestamp=timestamp,
-            like_count=like_count,
-            share_count=share_count,
-            comment_count=comment_count,
-            view_count=view_count
+        url=post_url,
+        post_id=post_id,
+        author_username=username,
+        author_display_name=display_name,
+        author_avatar=avatar,
+        author_url=author_url,
+        post_download_setting=post_download_setting,
+        post_description=post_description,
+        timestamp=timestamp,
+        like_count=like_count,
+        share_count=share_count,
+        comment_count=comment_count,
+        view_count=view_count
     )
 
     if __is_image_post(post_data):
         images = post_data.get("imagePost").get("images")
-        return TikTokSlide(
-            **post.__dict__,
-            images=images
-        )
+        return TikTokSlide(**post.__dict__, images=images)
     else:
         video_thumbnail = post_data.get("video").get("originCover")
-        return TikTokVideo(
-             **post.__dict__,
-            video_thumbnail=video_thumbnail
-        )
+        return TikTokVideo(**post.__dict__, video_thumbnail=video_thumbnail)
 
 
 def __generate_random_captcha_steps(piece_position: tuple[int, int], tip_y_value: int):
     x_position = piece_position[0]
 
     steps = []
     current_distance = 0
@@ -135,21 +143,21 @@
         "reply": __generate_random_captcha_steps(position,
                                                  tip_value)
     }
 
     return body
 
 
-async def __handle_captcha(playwright_page: Page, retries: int = 3) -> bool:
+async def __handle_captcha(playwright_page: Page, attempts: int = 3, timeout: float | None = 5000) -> bool:
     captcha_success_status = False
-    retry_count = 0
+    attempt_count = 0
 
-    while not captcha_success_status and retry_count < retries:
+    while not captcha_success_status and attempt_count < attempts:
         try:
-            async with playwright_page.expect_request(lambda x: "/captcha/get?" in x.url) as request:
+            async with playwright_page.expect_request(lambda x: "/captcha/get?" in x.url, timeout=timeout) as request:
                 await playwright_page.wait_for_load_state("networkidle")
                 request_value = await request.value
                 response = await request_value.response()
                 response_data = await response.json()
 
                 captcha_solution = __calculate_captcha_solution(response_data)
                 post_url_query_params = __get_captcha_response_params(request_value.url)
@@ -166,15 +174,15 @@
                 )
 
                 if captcha_status.status != 200:
                     return False
 
                 captcha_status_data = await captcha_status.json()
                 captcha_success_status = captcha_status_data.get("message") == "Verification complete"
-                retry_count += 1
+                attempt_count += 1
                 await playwright_page.locator("#verify-bar-close").click()
 
         except PlaywrightTimeoutError:
             return True
         except PlaywrightError:
             return False
 
@@ -204,50 +212,33 @@
     for key, value in all_kwargs.items():
         if key in allowed_args:
             valid_kwargs[key] = value
 
     return valid_kwargs
 
 
-async def get_post(
+async def __get_post(
     url: str,
     download: bool = True,
     force_download_strategy: Literal["primary",
                                      "secondary"] | None = None,
     proxy: dict | None = None,
     download_timeout: float = 5000,
+    download_path: str | None = None,
+    captcha_timeout: float = 5000,
+    captcha_attempts: int = 3,
     browser: Literal["firefox",
                      "chromium",
                      "chrome",
                      "safari",
                      "webkit"] = "firefox",
     headless: bool | None = None,
     slow_mo: float | None = None,
     **kwargs: dict
 ) -> TikTokVideo | TikTokSlide:
-    """Get the information about a given video URL. If the `download` param is set to True, also download the video as an mp4 file.
-
-    Args:
-        url (str): The URL to get the information of.
-        download (bool, optional): If the video should be downloaded locally. Defaults to True.
-        force_download_strategy (Literal[&quot;primary&quot;, &quot;secondary&quot;] | None, optional): Force a specific download strategy to use. Defaults to None which will auto-select the strategy to use.
-        proxy (dict | None, optional): The proxy settings to use for the request. Defaults to None.
-        download_timeout (float, optional): The number of ms the download will wait to start before timing out.
-        browser (Literal[&quot;firefox&quot;, &quot;chromium&quot;, &quot;chrome&quot;, &quot;safari&quot;, &quot;webkit&quot;], optional): The browser to use to scrape the content. Defaults to "firefox".
-        headless (bool | None, optional): If the browser should be headless. Defaults to None.
-        slow_mo (float | None, optional): Slow the browser down, useful when not headless. Defaults to None.
-
-    Raises:
-        TypeError: If the given browser is not a valid browser.
-        CaptchaFailedException: If the captcha was not able to be solved.
-        DownloadFailedException: If the video could not be downloaded.
-
-    Returns:
-        TikTokVideo: The data for the given URL as a TikTokVideo dataclass.
-    """
     async with async_playwright() as playwright:
         match browser:
             case "firefox":
                 browser_instance = playwright.firefox
             case "chrome":
                 browser_instance = playwright.chromium
             case "chromium":
@@ -275,106 +266,183 @@
             video_info = __parse_post_info(page_source)
         except:
             raise ResponseParseException(url)
 
         if not download:
             return video_info
 
-        captcha_success_result = await __handle_captcha(video_page)
+        captcha_success_result = await __handle_captcha(video_page, captcha_attempts, captcha_timeout)
         if not captcha_success_result:
             raise CaptchaFailedException(url)
 
         await __close_popups(video_page)
 
         if isinstance(video_info, TikTokSlide):
-            await download_slideshow(video_info)
+            await download_slideshow(video_info, download_path)
             return video_info
 
         if force_download_strategy:
-            try:
-                match force_download_strategy:
-                    case "primary":
-                        await primary_download_strategy(browser_context, video_page, video_info, download_timeout)
-                    case "secondary":
-                        await alternate_download_strategy(video_page, video_info, download_timeout)
-                    case _:
-                        raise ValueError(
-                            "Invalid download strategy provided. Strategy must be \"primary\", \"secondary\" or None."
-                        )
-            except:
-                raise DownloadFailedException(url=url)
-
-            return video_info
+            match force_download_strategy:
+                case "primary":
+                    video_info.post_download_setting = 0
+                case "secondary":
+                    video_info.post_download_setting = 1
+                case _:
+                    raise ValueError(
+                        "Invalid download strategy provided. Strategy must be \"primary\", \"secondary\" or None."
+                    )
 
         try:
             if video_info.post_download_setting == 0:
-                await primary_download_strategy(browser_context, video_page, video_info, download_timeout)
+                await primary_download_strategy(browser_context, video_page, video_info, download_timeout, download_path)
             else:
-                await alternate_download_strategy(video_page, video_info, download_timeout)
+                await alternate_download_strategy(video_page, video_info, download_timeout, download_path)
         except PlaywrightTimeoutError:
             raise DownloadFailedException(url=url)
 
         return video_info
 
 
+async def get_post(
+    url: str,
+    download: bool = True,
+    force_download_strategy: Literal["primary",
+                                     "secondary"] | None = None,
+    proxy: dict | None = None,
+    retries: int = 3,
+    retry_delay: float = 500,
+    download_timeout: float = 5000,
+    download_path: str | None = None,
+    browser: Literal["firefox",
+                     "chromium",
+                     "chrome",
+                     "safari",
+                     "webkit"] = "firefox",
+    headless: bool | None = None,
+    slow_mo: float | None = None,
+    **kwargs: dict
+) -> TikTokVideo | TikTokSlide:
+    """Get the information about a given video URL. If the `download` param is set to True, also download the video as an mp4 file.
+
+    Args:
+        url (str): The URL to get the information of.
+        download (bool, optional): If the video should be downloaded locally. Defaults to True.
+        force_download_strategy (Literal[&quot;primary&quot;, &quot;secondary&quot;] | None, optional): Force a specific download strategy to use. Defaults to None which will auto-select the strategy to use.
+        proxy (dict | None, optional): The proxy settings to use for the request. Defaults to None.
+        retries (int, optional): The number of times to retry upon failure. Defaults to 3.
+        retry_delay (float, optional): The number of ms to wait before retrying. Defaults to 500.
+        download_timeout (float, optional): The number of ms the download will wait to start before timing out.
+        download_path (str | None, optional): The path to download vidoes or images to. Defaults to None, the current directory.
+        browser (Literal[&quot;firefox&quot;, &quot;chromium&quot;, &quot;chrome&quot;, &quot;safari&quot;, &quot;webkit&quot;], optional): The browser to use to scrape the content. Defaults to "firefox".
+        headless (bool | None, optional): If the browser should be headless. Defaults to None.
+        slow_mo (float | None, optional): Slow the browser down, useful when not headless. Defaults to None.
+
+    Raises:
+        TypeError: If the given browser is not a valid browser.
+        CaptchaFailedException: If the captcha was not able to be solved.
+        DownloadFailedException: If the video could not be downloaded.
+
+    Returns:
+        TikTokVideo | TikTokSlide: The data for the given URL as a TikTokVideo or TikTokSlide dataclass.
+    """
+
+    for x in range(retries + 1):
+        try:
+            result = await __get_post(
+                url=url,
+                download=download,
+                force_download_strategy=force_download_strategy,
+                proxy=proxy,
+                download_timeout=download_timeout,
+                download_path=download_path,
+                browser=browser,
+                headless=headless,
+                slow_mo=slow_mo,
+                **kwargs
+            )
+            return result
+        except TikTokBaseException as e:
+            if x < retries:
+                await async_sleep(retry_delay / 1000.0)
+                continue
+
+            raise e
+
+        except Exception as e:
+            raise e
+
+
 async def primary_download_strategy(
     browser_context: BrowserContext,
     playwright_page: Page,
     video_info: TikTokVideo,
-    timeout: float
+    timeout: float,
+    download_path: str | None
 ):
     """Downloads the TikTok video using the UI download button that appears on a video. Only valid for videos with download setting 0.
 
     Args:
         browser_context (BrowserContext): The current browser context.
         playwright_page (Page): The current page.
         video_info (TikTokVideo): The video data of the TikTok video.
         timeout (float): The number of ms to wait for the download to start before timing out.
+        download_path (str | None): The path to download the video to. If None, uses current directory.
     """
+    download_path = __validate_download_path(download_path)
     browser_context.set_default_timeout(timeout)
     page_video_tag = playwright_page.locator("video").first
     await page_video_tag.click(button="right")
     await __random_timeout_duration(playwright_page, 100, 500)
     download_video_li = playwright_page.locator("li", has_text="Download video")
     async with playwright_page.expect_download() as download_info:
         await download_video_li.click()
         download = await download_info.value
-        save_path = f"{video_info.post_id}.mp4"
+        save_path = f"{download_path}{video_info.post_id}.mp4"
         await download.save_as(save_path)
         video_info.file_path = save_path
 
 
-async def alternate_download_strategy(playwright_page: Page, video_info: TikTokVideo, timeout: float):
+async def alternate_download_strategy(
+    playwright_page: Page,
+    video_info: TikTokVideo,
+    timeout: float,
+    download_path: str | None
+):
     """Uses the the browser request for the video to download the video. Valid for any download setting but less reliable.
 
     Args:
         playwright_page (Page): The current page.
         video_info (TikTokVideo): The video data of the TikTok video.
         timeout (float): THe number of ms to wait for the request to occur before timing out.
+        download_path (str | None): The path to download the video to. If None, uses current directory.
     """
+    download_path = __validate_download_path(download_path)
     page_video_tag = playwright_page.locator("video").first
     video_source = await page_video_tag.get_attribute("src")
 
     response_base_url = video_source.split("?")[0]
     async with playwright_page.expect_response(lambda x: response_base_url in x.url, timeout=timeout) as response_info:
         await playwright_page.reload()
         response = await response_info.value
-        save_path = f"{video_info.post_id}.mp4"
+        save_path = f"{download_path}{video_info.post_id}.mp4"
         with open(save_path, "wb") as f:
             f.write(await response.body())
         video_info.file_path = save_path
 
 
-async def download_slideshow(video_info: TikTokSlide):
+async def download_slideshow(video_info: TikTokSlide, download_path: str | None):
     """For a given Slideshow post, download the images associated with it.
 
     Args:
         video_info (TikTokSlide): The Slideshow post data.
+        download_path (str | None): The path to download the images to. If None, uses current directory.
     """
+    download_path = __validate_download_path(download_path)
+
     images = []
     for idx, image_info in enumerate(video_info.images):
         image_url = image_info.get("imageURL").get("urlList")[-1]
-        file = f"{idx+1}.jpeg"
+        file = f"{download_path}{idx+1}.jpeg"
         urlretrieve(image_url, file)
         images.append(file)
 
     video_info.images = images
```

### Comparing `tiktok-dlpy-1.3.1/tiktokdl/image_processing.py` & `tiktok-dlpy-1.4.0/tiktokdl/image_processing.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.3.1/tiktokdl/post_data.py` & `tiktok-dlpy-1.4.0/tiktokdl/post_data.py`

 * *Files identical despite different names*

