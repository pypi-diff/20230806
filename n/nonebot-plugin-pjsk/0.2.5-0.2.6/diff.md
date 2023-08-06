# Comparing `tmp/nonebot_plugin_pjsk-0.2.5.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.2.5.tar", last modified: Fri Aug  4 14:22:46 2023, max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.6.tar", last modified: Sun Aug  6 08:46:16 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.2.5.tar` & `nonebot_plugin_pjsk-0.2.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-08-04 14:22:25.249375 nonebot_plugin_pjsk-0.2.5/LICENSE
--rw-r--r--   0        0        0     4381 2023-08-04 14:22:25.249375 nonebot_plugin_pjsk-0.2.5/README.md
--rw-r--r--   0        0        0      795 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     8728 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/__main__.py
--rw-r--r--   0        0        0     1216 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0    11191 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     3962 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/resource.py
--rw-r--r--   0        0        0     2351 2023-08-04 14:22:25.301376 nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1787 2023-08-04 14:22:46.189397 nonebot_plugin_pjsk-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5372 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-06 08:45:58.454255 nonebot_plugin_pjsk-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4800 2023-08-06 08:45:58.454255 nonebot_plugin_pjsk-0.2.6/README.md
+-rw-r--r--   0        0        0      795 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     8728 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0     1216 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0    11391 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     4150 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2351 2023-08-06 08:45:58.506255 nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1787 2023-08-06 08:46:16.752144 nonebot_plugin_pjsk-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     5791 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.6/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.2.5/LICENSE` & `nonebot_plugin_pjsk-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.5/README.md` & `nonebot_plugin_pjsk-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-pjsk">
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-pjsk" alt="pypi download">
 </a>
 
 </div>
 
+## 💬 前言
+
+- 如遇字体大小不协调问题，请更新插件到最新版本，并且删除 `data/pjsk/fonts` 文件夹下的所有文件
+- 如果遇到资源文件下载失败的情况，请参考 [这个 issue](https://github.com/Agnes4m/nonebot_plugin_pjsk/issues/15)
+
 ## 📖 介绍
 
 ### Wonderhoy!
 
 ![Wonderhoy](./readme/wonderhoy.png)
 
 ## 💿 安装
@@ -147,14 +152,19 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.6
+
+- 插件会按角色名重新排序表情列表与表情 ID，以防数据源表情 ID 冲突
+- 角色列表名称展示优化
+
 ### 0.2.5
 
 - 使用自己合并的字体文件避免某些字不显示的问题
 
 ### 0.2.4
 
 - 在交互模式中提供的参数会去掉指令前缀，以防 Adapter 删掉参数开头的 Bot 昵称，导致参数不对的情况
```

#### html2text {}

```diff
@@ -1,15 +1,20 @@
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-PJSK _â¨ Project Sekai è¡¨æåå¶ä½ â¨_ [python] [pdm-
                            managed] [QQ_Chat_Group]
                        [license] [pypi] [pypi_download]
-## ð ä»ç» ### Wonderhoy! ![Wonderhoy](./readme/wonderhoy.png) ## ð¿
-å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
-å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+## ð¬ åè¨ -
+å¦éå­ä½å¤§å°ä¸åè°é®é¢ï¼è¯·æ´æ°æä»¶å°ææ°çæ¬ï¼å¹¶ä¸å é¤
+`data/pjsk/fonts` æä»¶å¤¹ä¸çæææä»¶ -
+å¦æéå°èµæºæä»¶ä¸è½½å¤±è´¥çæåµï¼è¯·åè [è¿ä¸ª issue](https:
+//github.com/Agnes4m/nonebot_plugin_pjsk/issues/15) ## ð ä»ç» ###
+Wonderhoy! ![Wonderhoy](./readme/wonderhoy.png) ## ð¿ å®è£
+ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
+å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-pjsk
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
 ```bash conda install nonebot-plugin-pjsk ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
@@ -26,15 +31,17 @@
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.5
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.6
+- æä»¶ä¼æè§è²åéæ°æåºè¡¨æåè¡¨ä¸è¡¨æ
+IDï¼ä»¥é²æ°æ®æºè¡¨æ ID å²çª - è§è²åè¡¨åç§°å±ç¤ºä¼å ### 0.2.5
 - ä½¿ç¨èªå·±åå¹¶çå­ä½æä»¶é¿åæäºå­ä¸æ¾ç¤ºçé®é¢ ### 0.2.4
 - å¨äº¤äºæ¨¡å¼ä¸­æä¾çåæ°ä¼å»ææä»¤åç¼ï¼ä»¥é² Adapter
 å æåæ°å¼å¤´ç Bot æµç§°ï¼å¯¼è´åæ°ä¸å¯¹çæåµ -
 éåå¸®å©å¾ççæ¸²æï¼ä¸ªäººæè§ææè¿ä¸æ¯å¾å¥½â¦â¦ï¼ ###
 0.2.3 - éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
 æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
 nonebot_plugin_pjsk/issues/14)) - åæ° `--rotate`
```

### Comparing `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __plugin_meta__ = PluginMetadata(
     name="Sekai Stickers",
     description="基于 NoneBot2 的 Project Sekai 表情包制作插件",
     usage="使用指令 `pjsk -h` 查看帮助",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/__main__.py` & `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/draw.py`

 * *Files 9% similar despite different names*

```diff
@@ -372,20 +372,27 @@
         await path.write_bytes(image)
         return image
 
     return wrapper
 
 
 async def render_all_characters() -> Image.Image:
-    characters: Dict[str, StickerInfo] = {}
+    character_dict: Dict[str, StickerInfo] = {}
     for info in LOADED_STICKER_INFO:
-        if info.character not in characters:
-            characters[info.character] = info
+        character = info.character
+        if character not in character_dict:
+            character = (
+                character
+                if character[0].isupper()
+                else character[0].upper() + character[1:]
+            )
+            character_dict[character] = info
+
     return await render_summary_from_tasks(
-        draw_sticker(info, info.character.capitalize()) for info in characters.values()
+        draw_sticker(info, character) for character, info in character_dict.items()
     )
 
 
 async def get_all_characters() -> bytes:
     return await use_image_cache(render_all_characters, "all_characters")()
```

### Comparing `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/resource.py` & `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,20 @@
     color: str
     default_text: StickerText = Field(..., alias="defaultText")
 
 
 LOADED_STICKER_INFO: List[StickerInfo] = []
 
 
+def sort_stickers():
+    LOADED_STICKER_INFO.sort(key=lambda x: x.character.lower())
+    for i, x in enumerate(LOADED_STICKER_INFO, 1):
+        x.sticker_id = str(i)
+
+
 @overload
 def select_or_get_random(sticker_id: None = None) -> StickerInfo:
     ...
 
 
 @overload
 def select_or_get_random(sticker_id: str) -> Optional[StickerInfo]:
@@ -89,19 +95,20 @@
     path = anyio.Path(STICKER_INFO_CACHE)
     try:
         loaded_text = await async_request("src/characters.json", ResponseType.TEXT)
         await path.write_text(loaded_text, encoding="u8")
     except Exception as e:
         if not (await path.exists()):
             raise
-        logger.warning(f"Failed to load sticker information, using cached data\n{e!r}")
+        logger.warning(f"Failed to load sticker information, using cached data: {e!r}")
         loaded_text = await path.read_text(encoding="u8")
 
     LOADED_STICKER_INFO.clear()
     LOADED_STICKER_INFO.extend(parse_raw_as(List[StickerInfo], loaded_text))
+    sort_stickers()
 
 
 async def check_and_download_stickers():
     semaphore = asyncio.Semaphore(10)
 
     @with_semaphore(semaphore)
     async def download(path_str: str):
```

### Comparing `nonebot_plugin_pjsk-0.2.5/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.2.6/nonebot_plugin_pjsk/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.5/pyproject.toml` & `nonebot_plugin_pjsk-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pjsk"
-version = "0.2.5"
+version = "0.2.6"
 description = "Project Sekai Sticker Creator for NoneBot2."
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
```

### Comparing `nonebot_plugin_pjsk-0.2.5/PKG-INFO` & `nonebot_plugin_pjsk-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.2.5
+Version: 0.2.6
 Summary: Project Sekai Sticker Creator for NoneBot2.
 Keywords: pjsk nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 Author-Email: Agnes_Digital <Z735803792@163.com>, student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -57,14 +57,19 @@
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-pjsk">
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-pjsk" alt="pypi download">
 </a>
 
 </div>
 
+## 💬 前言
+
+- 如遇字体大小不协调问题，请更新插件到最新版本，并且删除 `data/pjsk/fonts` 文件夹下的所有文件
+- 如果遇到资源文件下载失败的情况，请参考 [这个 issue](https://github.com/Agnes4m/nonebot_plugin_pjsk/issues/15)
+
 ## 📖 介绍
 
 ### Wonderhoy!
 
 ![Wonderhoy](./readme/wonderhoy.png)
 
 ## 💿 安装
@@ -172,14 +177,19 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
+### 0.2.6
+
+- 插件会按角色名重新排序表情列表与表情 ID，以防数据源表情 ID 冲突
+- 角色列表名称展示优化
+
 ### 0.2.5
 
 - 使用自己合并的字体文件避免某些字不显示的问题
 
 ### 0.2.4
 
 - 在交互模式中提供的参数会去掉指令前缀，以防 Adapter 删掉参数开头的 Bot 昵称，导致参数不对的情况
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.5 Summary: Project
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.6 Summary: Project
 Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin Home-page:
 https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email: Agnes_Digital
 163.com>, student_2333
 126.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -13,17 +13,22 @@
 httpx>=0.24.1 Requires-Dist: numpy>=1.25.1 Requires-Dist: anyio>=3.7.1
 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-PJSK _â¨ Project Sekai è¡¨æåå¶ä½ â¨_ [python] [pdm-
                            managed] [QQ_Chat_Group]
                        [license] [pypi] [pypi_download]
-## ð ä»ç» ### Wonderhoy! ![Wonderhoy](./readme/wonderhoy.png) ## ð¿
-å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
-å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+## ð¬ åè¨ -
+å¦éå­ä½å¤§å°ä¸åè°é®é¢ï¼è¯·æ´æ°æä»¶å°ææ°çæ¬ï¼å¹¶ä¸å é¤
+`data/pjsk/fonts` æä»¶å¤¹ä¸çæææä»¶ -
+å¦æéå°èµæºæä»¶ä¸è½½å¤±è´¥çæåµï¼è¯·åè [è¿ä¸ª issue](https:
+//github.com/Agnes4m/nonebot_plugin_pjsk/issues/15) ## ð ä»ç» ###
+Wonderhoy! ![Wonderhoy](./readme/wonderhoy.png) ## ð¿ å®è£
+ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
+å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-pjsk
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
 ```bash conda install nonebot-plugin-pjsk ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
@@ -40,15 +45,17 @@
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.5
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.6
+- æä»¶ä¼æè§è²åéæ°æåºè¡¨æåè¡¨ä¸è¡¨æ
+IDï¼ä»¥é²æ°æ®æºè¡¨æ ID å²çª - è§è²åè¡¨åç§°å±ç¤ºä¼å ### 0.2.5
 - ä½¿ç¨èªå·±åå¹¶çå­ä½æä»¶é¿åæäºå­ä¸æ¾ç¤ºçé®é¢ ### 0.2.4
 - å¨äº¤äºæ¨¡å¼ä¸­æä¾çåæ°ä¼å»ææä»¤åç¼ï¼ä»¥é² Adapter
 å æåæ°å¼å¤´ç Bot æµç§°ï¼å¯¼è´åæ°ä¸å¯¹çæåµ -
 éåå¸®å©å¾ççæ¸²æï¼ä¸ªäººæè§ææè¿ä¸æ¯å¾å¥½â¦â¦ï¼ ###
 0.2.3 - éå¶äºè´´çº¸ææ¬å¤§å°ï¼ä»¥å Bot ç¬é´çç¸ -
 æªæä¾å­ä½å¤§å°æ¶éåºæ§è°è ([#14](https://github.com/Agnes4m/
 nonebot_plugin_pjsk/issues/14)) - åæ° `--rotate`
```

