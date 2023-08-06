# Comparing `tmp/nonebot_plugin_impact-0.6.114514.tar.gz` & `tmp/nonebot_plugin_impact-0.7.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_impact-0.6.114514.tar", last modified: Fri Jul 28 16:38:32 2023, max compression
+gzip compressed data, was "nonebot_plugin_impact-0.7.114514.tar", last modified: Sun Aug  6 21:47:16 2023, max compression
```

## Comparing `nonebot_plugin_impact-0.6.114514.tar` & `nonebot_plugin_impact-0.7.114514.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 16:38:32.777642 nonebot_plugin_impact-0.6.114514/
--rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.6.114514/LICENSE
--rw-rw-rw-   0        0        0      306 2023-07-28 16:38:32.776641 nonebot_plugin_impact-0.6.114514/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 16:38:32.759642 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/
--rw-rw-rw-   0        0        0     2093 2023-07-28 16:37:24.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/__init__.py
--rw-rw-rw-   0        0        0     9180 2023-07-28 16:31:58.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/draw_img.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:38:32.766642 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/fonts/
--rw-rw-rw-   0        0        0  6700204 2023-07-28 16:31:58.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
--rw-rw-rw-   0        0        0    20206 2023-07-28 16:31:58.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/handle.py
--rw-rw-rw-   0        0        0     2205 2023-07-28 16:31:58.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/txt2img.py
--rw-rw-rw-   0        0        0     8687 2023-07-28 16:35:21.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:38:32.765641 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/
--rw-rw-rw-   0        0        0      306 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 16:38:32.777642 nonebot_plugin_impact-0.6.114514/setup.cfg
--rw-rw-rw-   0        0        0      543 2023-07-28 16:38:14.000000 nonebot_plugin_impact-0.6.114514/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 21:47:16.210519 nonebot_plugin_impact-0.7.114514/
+-rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.7.114514/LICENSE
+-rw-rw-rw-   0        0        0      306 2023-08-06 21:47:16.209519 nonebot_plugin_impact-0.7.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-06 21:47:16.190519 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/
+-rw-rw-rw-   0        0        0     2309 2023-08-06 21:16:41.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/__init__.py
+-rw-rw-rw-   0        0        0     7368 2023-08-06 21:30:13.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/data_sheet.py
+-rw-rw-rw-   0        0        0     9107 2023-08-06 21:21:24.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/draw_img.py
+drwxrwxrwx   0        0        0        0 2023-08-06 21:47:16.199519 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/fonts/
+-rw-rw-rw-   0        0        0  6700204 2023-08-06 17:56:52.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
+-rw-rw-rw-   0        0        0    19004 2023-08-06 21:21:50.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/handle.py
+-rw-rw-rw-   0        0        0     2286 2023-08-06 21:21:54.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/txt2img.py
+-rw-rw-rw-   0        0        0     4876 2023-08-06 21:14:30.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 21:47:16.198518 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact.egg-info/
+-rw-rw-rw-   0        0        0      306 2023-08-06 21:47:15.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-08-06 21:47:16.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 21:47:15.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-08-06 21:47:15.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-06 21:47:15.000000 nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 21:47:16.210519 nonebot_plugin_impact-0.7.114514/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-08-06 21:46:55.000000 nonebot_plugin_impact-0.7.114514/setup.py
```

### Comparing `nonebot_plugin_impact-0.6.114514/LICENSE` & `nonebot_plugin_impact-0.7.114514/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/__init__.py` & `nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+"""插件入口"""
 import contextlib
 from re import I
 
-from nonebot import on_command, on_regex
+from nonebot import on_command, on_regex, require
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
 from nonebot.permission import SUPERUSER
 
 from .handle import impart
 from .utils import utils
 
+require("nonebot_plugin_apscheduler")
+
+from nonebot_plugin_apscheduler import scheduler
+
+scheduler.add_job(impart.penalties_and_resets, "cron", hour = 0, misfire_grace_time = 600)
+
 on_command(
     "pk",
     aliases={"对决"},
     rule=utils.rule,
     priority=20,
     block=False,
     handlers=[impart.pk],
@@ -85,11 +92,11 @@
         description="让群友们眼前一黑的nonebot2淫趴插件",
         usage=utils.usage,
         type="application",
         homepage="https://github.com/Special-Week/nonebot_plugin_impact",
         supported_adapters={"~onebot.v11"},
         extra={
             "author": "Special-Week",
-            "version": "0.06.114514",
+            "version": "0.07.114514",
             "priority": 20,
         },
     )
```

### Comparing `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/draw_img.py` & `nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/draw_img.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""绘画图表模块"""
 import random
 from io import BytesIO
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 from PIL import Image, ImageDraw, ImageFilter, ImageFont
 
@@ -20,14 +21,15 @@
             (255, 99, 71),  # 红橙色
             (255, 215, 0),  # 金色
         ]
         self.module_path: Path = Path(__file__).parent
         self.font = str(self.module_path / "fonts" / "SIMYOU.TTF")
 
     async def draw_bar_chart(self, data: Dict[str, float]) -> bytes:
+        """画柱状图, 传入一个字典, key是str类型的用户名字, value是对应用户的注入量"""
         values = list(data.values())
         keys = list(data.keys())
         image = Image.new("RGBA", (1920, 1080), (255, 255, 255, 255))
         draw = ImageDraw.Draw(image)
 
         # ------------------------ 画一个框框 ------------------------
 
@@ -84,15 +86,14 @@
         # ------------------------ 画柱状图 ------------------------
 
         columns = Image.new("RGBA", (1920, 1080), (255, 255, 255, 0))
         draw = ImageDraw.Draw(columns)
         random.shuffle(self.colors)
         for i, value in enumerate(values):
             color = self.colors[i]
-            # 在左边依次画出颜色的方块, 并且写上名字, 间隔20像素, 方块边长为50像素
             draw.rectangle((50, 50 + 70 * i, 100, 100 + 70 * i), fill=color + (250,))
             draw.text(
                 (120, 60 + 70 * i),
                 keys[i] if len(keys[i]) < 8 else f"{keys[i][:8]}...",
                 fill="black",
                 font=ImageFont.truetype(self.font, 28),
             )
@@ -102,47 +103,46 @@
                         540 + 120 * i,
                         770 - 78 * (value / maxnum_scale),
                         635 + 120 * i,
                         770,
                     ),
                     fill=color + (200,),
                 )
-                # 在柱子上方写上值, 居中
                 draw.text(
                     (540 + 120 * i, 770 - 78 * (value / maxnum_scale) - 30),
                     str(value),
                     fill="black",
-                    font=ImageFont.truetype(self.font, 32),
+                    font=ImageFont.truetype(self.font, 26),
                 )
             else:
                 draw.rectangle(
                     (
                         540 + 120 * i,
                         770,
                         635 + 120 * i,
                         770 - 78 * (value / minnum_scale),
                     ),
                     fill=color + (200,),
                 )
-                # 在柱子下方写上值, 居中
                 draw.text(
                     (540 + 120 * i, 770 - 78 * (value / minnum_scale) + 10),
                     str(value),
                     fill="black",
-                    font=ImageFont.truetype(self.font, 32),
+                    font=ImageFont.truetype(self.font, 26),
                 )
 
         # ------------------------ 粘贴上来 ------------------------
         image.paste(columns, (0, 0), columns)
         img_byte = BytesIO()
         image.save(img_byte, format="PNG")
         return img_byte.getvalue()
 
+
     async def draw_line_chart(self, data: Dict[str, float]):
-        # 画折线图
+        """画折线图, 传入一个字典, key是str类型的用户名字, value是对应用户的注入量"""
         values = list(data.values())
         keys = list(data.keys())
         image = Image.new("RGBA", (1920, 1080), (255, 255, 255, 255))
         draw = ImageDraw.Draw(image)
 
         # ------------------------ 画一个框框 ------------------------
 
@@ -199,22 +199,20 @@
                 font=ImageFont.truetype(self.font, 32),
             )
             for i in range(1, len(values)):
                 x_new = x_start + x_gap * i
                 y_new = 1000 - 95 * (values[i] / maxnum_scale)
                 draw.line((x, y, x_new, y_new), fill="black", width=2)
                 x, y = x_new, y_new
-                # 给每个点画个圆圈
                 draw.ellipse((x - 5, y - 5, x + 5, y + 5), fill="black", width=2)
-                # 在每个点上写上值
                 draw.text(
                     (x - 20, y - 30),
                     str(values[i]),
                     fill="black",
-                    font=ImageFont.truetype(self.font, 32),
+                    font=ImageFont.truetype(self.font, 26),
                 )
 
         draw_line_chart()
         if len(values) > 18:
             keys = keys[:9] + keys[-9:]
         position = 0
         for i in range(len(values)):
```

### Comparing `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF` & `nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/handle.py` & `nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/handle.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,268 +1,270 @@
+"""matcher的handle模块"""
 import asyncio
 import random
 import time
 from random import choice
-from typing import Tuple
+from typing import Dict, List, Tuple
 
+from nonebot import get_driver
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, Message, MessageSegment
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, RegexGroup
 
+from .data_sheet import (
+    add_new_user,
+    check_group_allow,
+    get_ejaculation_data,
+    get_jj_length,
+    get_sorted,
+    get_today_ejaculation_data,
+    insert_ejaculation,
+    is_in_table,
+    punish_all_inactive_users,
+    set_group_allow,
+    set_jj_length,
+    update_activity,
+)
 from .draw_img import draw_bar_chart
 from .utils import utils
 
 
 class Impart:
+    penalties_impact: bool = getattr(get_driver().config, "isalive", False)  # 重置每日活跃度
+
+    @staticmethod
+    def penalties_and_resets() -> None:
+        """重置每日活跃度"""
+        if Impart.penalties_impact:
+            punish_all_inactive_users()
+
     @staticmethod
     async def pk(matcher: Matcher, event: GroupMessageEvent) -> None:
         """pk的响应器"""
-        if not (await utils.check_group_allow(str(event.group_id))):
+        if not check_group_allow(event.group_id):
             await matcher.finish(utils.not_allow, at_sender=True)
         uid: str = event.get_user_id()
         allow: bool = await utils.pkcd_check(uid)  # CD是否允许pk
         if not allow:  # 如果不允许pk, 则返回
             await matcher.finish(
                 f"你已经pk不动了喵, 请等待{round(utils.pk_cd_time-(time.time() - utils.pk_cd_data[uid]),3)}秒后再pk喵",
                 at_sender=True,
             )
         utils.pk_cd_data.update({uid: time.time()})  # 更新CD时间
         at = await utils.get_at(event)  # 获取at的id, 类型为str
         if at == uid:  # 如果at的id和uid相同, 则返回
             await matcher.finish("你不能pk自己喵", at_sender=True)
         # rule规定了必须有at, 所以不用判断at是否为寄
-        if uid in utils.userdata and at in utils.userdata:  # 如果两个都在userdata里面
+        if is_in_table(userid=int(uid)) and is_in_table(int(at)):  # 如果两个都在userdata里面
             random_num = random.random()  # 生成一个随机数
             # 如果random_num大于0.5, 则胜利, 否则失败
             if random_num > 0.5:
                 random_num: float = utils.get_random_num()  # 重新生成一个随机数
-                utils.userdata.update(
-                    {uid: round(utils.userdata[uid] + (random_num / 2), 3)}
-                )  # 更新userdata
-                # 更新userdata
-                utils.userdata.update({at: round(utils.userdata[at] - random_num, 3)})
-                utils.write_user_data()  # 写入文件
+                set_jj_length(int(uid), random_num / 2)
+                set_jj_length(int(at), -random_num)
                 await matcher.finish(
                     f"对决胜利喵, 你的{choice(utils.jj_variable)}增加了{round(random_num/2,3)}cm喵, 对面则在你的阴影笼罩下减小了{random_num}cm喵",
                     at_sender=True,
                 )
             else:
                 random_num: float = utils.get_random_num()  # 重新生成一个随机数
-                utils.userdata.update(
-                    {uid: round(utils.userdata[uid] - random_num, 3)}
-                )  # 更新userdata
-                # 更新userdata
-                utils.userdata.update(
-                    {at: round(utils.userdata[at] + random_num / 2, 3)}
-                )
-                utils.write_user_data()  # 写入文件
+                set_jj_length(int(uid), -random_num)
+                set_jj_length(int(at), random_num / 2)
                 await matcher.finish(
                     f"对决失败喵, 在对面牛子的阴影笼罩下你的{choice(utils.jj_variable)}减小了{random_num}cm喵, 对面增加了{round(random_num/2,3)}cm喵",
                     at_sender=True,
                 )
         else:
             # 谁不在userdata里面, 就创建谁
-            if uid not in utils.userdata:
-                utils.userdata.update({uid: 10})  # 创建用户
-            if at not in utils.userdata:
-                utils.userdata.update({at: 10})  # 创建用户
-            utils.write_user_data()  # 写入文件
+            if is_in_table(userid=int(uid)):
+                add_new_user(int(at))
+            if is_in_table(userid=int(at)):
+                add_new_user(int(uid))
             del utils.pk_cd_data[uid]  # 删除CD时间
             await matcher.finish(
                 f"你或对面还没有创建{choice(utils.jj_variable)}喵, 咱全帮你创建了喵, 你们的{choice(utils.jj_variable)}长度都是10cm喵",
                 at_sender=True,
             )
 
     @staticmethod
     async def dajiao(matcher: Matcher, event: GroupMessageEvent) -> None:
         """打胶的响应器"""
-        if not (await utils.check_group_allow(str(event.group_id))):
+        if not check_group_allow(event.group_id):
             await matcher.finish(utils.not_allow, at_sender=True)
         uid: str = event.get_user_id()
         allow = await utils.cd_check(uid)  # CD是否允许打胶
         if not allow:  # 如果不允许打胶, 则返回
             await matcher.finish(
                 f"你已经打不动了喵, 请等待{round(utils.dj_cd_time-(time.time() - utils.cd_data[uid]),3)}秒后再打喵",
                 at_sender=True,
             )
         utils.cd_data.update({uid: time.time()})  # 更新CD时间
-        if uid in utils.userdata:  # 如果在userdata里面
+        if is_in_table(userid=int(uid)):  # 如果在userdata里面
             random_num = utils.get_random_num()  # 生成一个随机数
-            utils.userdata.update(
-                {uid: round(utils.userdata[uid] + random_num, 3)}
-            )  # 更新userdata
-            utils.write_user_data()  # 写入文件
+            set_jj_length(int(uid), random_num)  # 更新userdata
             await matcher.finish(
-                f"打胶结束喵, 你的{choice(utils.jj_variable)}很满意喵, 长了{random_num}cm喵, 目前长度为{utils.userdata[uid]}cm喵",
+                f"打胶结束喵, 你的{choice(utils.jj_variable)}很满意喵, 长了{random_num}cm喵, 目前长度为{get_jj_length(int(uid))}cm喵",
                 at_sender=True,
             )
         else:
-            utils.userdata.update({uid: 10})  # 创建用户
-            utils.write_user_data()  # 写入文件
-            del utils.cd_data[uid]  # 删除CD时间
+            add_new_user(int(uid))  # 创建用户
             await matcher.finish(
                 f"你还没有创建{choice(utils.jj_variable)}, 咱帮你创建了喵, 目前长度是10cm喵",
                 at_sender=True,
             )
 
     @staticmethod
     async def suo(matcher: Matcher, event: GroupMessageEvent) -> None:
         """嗦牛子的响应器"""
-        if not (await utils.check_group_allow(str(event.group_id))):
+        if not check_group_allow(event.group_id):
             await matcher.finish(utils.not_allow, at_sender=True)
         uid: str = event.get_user_id()
         allow = await utils.suo_cd_check(uid)  # CD是否允许嗦
         if not allow:  # 如果不允许嗦, 则返回
             await matcher.finish(
                 f"你已经嗦不动了喵, 请等待{round(utils.suo_cd_time-(time.time() - utils.suo_cd_data[uid]),3)}秒后再嗦喵",
                 at_sender=True,
             )
         utils.suo_cd_data.update({uid: time.time()})  # 更新CD时间
         at: str = await utils.get_at(event)  # 获取at的用户id, 类型为str
         if at == "寄":  # 如果没有at
-            if uid in utils.userdata:  # 如果在userdata里面
+            if is_in_table(userid=int(uid)):  # 如果在userdata里面
                 random_num = utils.get_random_num()  # 生成一个随机数
-                utils.userdata.update(
-                    {uid: round(utils.userdata[uid] + random_num, 3)}
-                )  # 更新userdata
-                utils.write_user_data()  # 写入文件
+                set_jj_length(int(uid), random_num)
                 await matcher.finish(
-                    f"你的{choice(utils.jj_variable)}很满意喵, 嗦长了{random_num}cm喵, 目前长度为{utils.userdata[uid]}cm喵",
+                    f"你的{choice(utils.jj_variable)}很满意喵, 嗦长了{random_num}cm喵, 目前长度为{get_jj_length(int(uid))}cm喵",
                     at_sender=True,
                 )
             else:  # 如果不在userdata里面
-                utils.userdata.update({uid: 10})  # 创建用户
-                utils.write_user_data()  # 写入文件
+                add_new_user(int(uid))  # 创建用户
                 del utils.suo_cd_data[uid]  # 删除CD时间
                 await matcher.finish(
                     f"你还没有创建{choice(utils.jj_variable)}喵, 咱帮你创建了喵, 目前长度是10cm喵",
                     at_sender=True,
                 )
-        elif at in utils.userdata:  # 如果在userdata里面
+        elif is_in_table(userid=int(at)):  # 如果在userdata里面
             random_num = utils.get_random_num()  # 生成一个随机数
             # 更新userdata
-            utils.userdata.update({at: round(utils.userdata[at] + random_num, 3)})
-            utils.write_user_data()  # 写入文件
+            set_jj_length(int(at), random_num)
             await matcher.finish(
-                f"对方的{choice(utils.jj_variable)}很满意喵, 嗦长了{random_num}cm喵, 目前长度为{utils.userdata[at]}cm喵",
+                f"对方的{choice(utils.jj_variable)}很满意喵, 嗦长了{random_num}cm喵, 目前长度为{get_jj_length(int(at))}cm喵",
                 at_sender=True,
             )
         else:
-            utils.userdata.update({at: 10})  # 创建用户
-            utils.write_user_data()  # 写入文件
+            add_new_user(int(at))  # 创建用户
             del utils.suo_cd_data[uid]  # 删除CD时间
             await matcher.finish(
-                f"他还没有创建{choice(utils.jj_variable)}喵, 咱帮他创建了喵, 目前长度是10cm喵",
+                f"TA还没有创建{choice(utils.jj_variable)}喵, 咱帮TA创建了喵, 目前长度是10cm喵",
                 at_sender=True,
             )
 
     @staticmethod
     async def queryjj(matcher: Matcher, event: GroupMessageEvent) -> None:
         """查询某人jj的响应器"""
-        if not (await utils.check_group_allow(str(event.group_id))):
+        if not check_group_allow(event.group_id):
             await matcher.finish(utils.not_allow, at_sender=True)
         uid: str = event.get_user_id()  # 获取用户id, 类型为str
         at: str = await utils.get_at(event)  # 获取at的用户id, 类型为str
         if at == "寄":  # 如果没有at
-            if uid in utils.userdata:  # 如果在userdata里面
+            if is_in_table(userid=int(uid)):  # 如果在userdata里面
                 await matcher.finish(
-                    f"你的{choice(utils.jj_variable)}目前长度为{utils.userdata[uid]}cm喵",
+                    f"你的{choice(utils.jj_variable)}目前长度为{get_jj_length(int(uid))}cm喵",
                     at_sender=True,
                 )
             else:
-                utils.userdata.update({uid: 10})  # 创建用户
-                utils.write_user_data()  # 写入文件
+                add_new_user(int(uid))  # 创建用户
                 await matcher.finish(
                     f"你还没有创建{choice(utils.jj_variable)}喵, 咱帮你创建了喵, 目前长度是10cm喵",
                     at_sender=True,
                 )
-        elif at in utils.userdata:  # 如果在userdata里面
+        elif is_in_table(userid=int(at)):  # 如果在userdata里面
             await matcher.finish(
-                f"他的{choice(utils.jj_variable)}目前长度为{utils.userdata[at]}cm喵",
+                f"TA的{choice(utils.jj_variable)}目前长度为{get_jj_length(int(at))}cm喵",
                 at_sender=True,
             )
         else:
-            utils.userdata.update({at: 10})  # 创建用户
-            utils.write_user_data()  # 写入文件
+            add_new_user(int(at))  # 创建用户
             await matcher.finish(
-                f"他还没有创建{choice(utils.jj_variable)}喵, 咱帮他创建了喵, 目前长度是10cm喵",
+                f"TA还没有创建{choice(utils.jj_variable)}喵, 咱帮他创建了喵, 目前长度是10cm喵",
                 at_sender=True,
             )
 
     @staticmethod
     async def jjrank(bot: Bot, matcher: Matcher, event: GroupMessageEvent) -> None:
         """输出前五后五和自己的排名"""
-        if not (await utils.check_group_allow(str(event.group_id))):
+        if not check_group_allow(event.group_id):
             await matcher.finish(utils.not_allow, at_sender=True)
-        uid: str = event.get_user_id()
-        rankdata: list = sorted(
-            utils.userdata.items(), key=lambda x: x[1], reverse=True
-        )  # 排序
+        uid: int = event.user_id
+        rankdata: List[Dict] = get_sorted()
         if len(rankdata) < 5:
             await matcher.finish("目前记录的数据量小于5, 无法显示rank喵")
-        top5: list = rankdata[:5]  # 取前5
-        last5: list = rankdata[-5:]  # 取后5
-        index = [i for i, x in enumerate(rankdata) if x[0] == uid]  # 获取用户排名
+        top5: List = rankdata[:5]  # 取前5
+        last5: List = rankdata[-5:]  # 取后5
+        # 获取自己的排名
+        index: List = [i for i in range(len(rankdata)) if rankdata[i]["userid"] == uid]
         if not index:  # 如果用户没有创建JJ
-            utils.userdata.update({uid: 10})  # 创建用户
-            utils.write_user_data()  # 写入文件
+            add_new_user(uid)
             await matcher.finish(
                 f"你还没有创建{choice(utils.jj_variable)}看不到rank喵, 咱帮你创建了喵, 目前长度是10cm喵",
                 at_sender=True,
             )
         # top5和end5的信息，然后获取其网名
-        top5info = [await bot.get_stranger_info(user_id=int(name[0])) for name in top5]
+        top5info = [
+            await bot.get_stranger_info(user_id=name["userid"]) for name in top5
+        ]
         last5info = [
-            await bot.get_stranger_info(user_id=int(name[0])) for name in last5
+            await bot.get_stranger_info(user_id=name["userid"]) for name in last5
         ]
+
         top5names = [name["nickname"] for name in top5info]
         last5names = [name["nickname"] for name in last5info]
-        data = {top5names[i]: top5[i][1] for i in range(len(top5))}
+
+        data = {top5names[i]: top5[i]["jj_length"] for i in range(len(top5))}
         for i in range(len(last5)):
-            data[last5names[i]] = last5[i][1]
+            data[last5names[i]] = last5[i]["jj_length"]
         img_bytes = await draw_bar_chart.draw_bar_chart(data)
         reply2 = f"你的排名为{index[0]+1}喵"
         await matcher.finish(MessageSegment.image(img_bytes) + reply2, at_sender=True)
 
     @staticmethod
     async def yinpa_prehandle(
         bot: Bot,
         args: Tuple,
         matcher: Matcher,
         event: GroupMessageEvent,
-    ) -> Tuple[int, int, str, str, list]:
+    ) -> Tuple[int, str, str, list]:
         """透群员的预处理环节"""
         gid, uid = event.group_id, event.user_id
-        if not (await utils.check_group_allow(str(gid))):
+        if not check_group_allow(event.group_id):
             await matcher.finish(utils.not_allow, at_sender=True)
         allow = await utils.fuck_cd_check(event)  # CD检查是否允许
         if not allow:
             await matcher.finish(
                 f"你已经榨不出来任何东西了, 请先休息{round(utils.fuck_cd_time-(time.time() - utils.ejaculation_cd[str(uid)]),3)}秒",
                 at_sender=True,
             )
         utils.ejaculation_cd.update({str(uid): time.time()})  # 记录时间
-        req_user_card = await utils.get_user_card(bot, group_id=int(gid), qid=int(uid))
+        req_user_card = str(await utils.get_user_card(event))
         prep_list = await bot.get_group_member_list(group_id=gid)
-        return gid, uid, req_user_card, args[0], prep_list
+        return uid, req_user_card, args[0], prep_list
 
     @staticmethod
     async def yinpa_member_handle(
         prep_list: list,
         req_user_card: str,
         matcher: Matcher,
         event: GroupMessageEvent,
     ) -> str:
         prep_list = [prep.get("user_id", 114514) for prep in prep_list]  # 群友列表
         target = await utils.get_at(event)  # 获取消息有没有at
         if target == "寄":  # 没有的话
             # 随机抽取幸运成员
             prep_list.remove(event.user_id)
             lucky_user = choice(prep_list)
-            await matcher.send(f"现在咱将随机抽取一位幸运裙友\n送给{req_user_card}色色！")
+            await matcher.send(f"现在咱将随机抽取一位幸运群友\n送给{req_user_card}色色！")
         else:  # 有的话lucky user就是at的人
             lucky_user = target
         return lucky_user
 
     @staticmethod
     async def yinpa_owner_handle(
         uid: int,
@@ -320,103 +322,93 @@
     async def yinpa(
         self,
         bot: Bot,
         matcher: Matcher,
         event: GroupMessageEvent,
         args: Tuple = RegexGroup(),
     ) -> None:
-        gid, uid, req_user_card, command, prep_list = await self.yinpa_prehandle(
+        if not check_group_allow(event.group_id):
+            await matcher.finish(utils.not_allow, at_sender=True)
+        uid, req_user_card, command, prep_list = await self.yinpa_prehandle(
             matcher=matcher, bot=bot, args=args, event=event
         )
         lucky_user: str = await self.yinpa_identity_handle(
             command=command,
             prep_list=prep_list,
             req_user_card=req_user_card,
             matcher=matcher,
             event=event,
         )
         # 获取群名片或者网名
-        lucky_user_card = await utils.get_user_card(bot, gid, int(lucky_user))
+        lucky_user_card = str(await utils.get_user_card(event))
         # 1--100的随机数， 保留三位
         ejaculation = round(random.uniform(1, 100), 3)
-        try:
-            temp = (
-                utils.ejaculation_data[lucky_user][utils.get_today()]["ejaculation"]
-                + ejaculation
-            )
-            await utils.update_ejaculation(round(temp, 3), lucky_user)
-        except Exception:
-            await utils.update_ejaculation(ejaculation, lucky_user)
+        insert_ejaculation(int(lucky_user), ejaculation)
         await asyncio.sleep(2)  # 休眠2秒, 更有效果
+        update_activity(int(lucky_user))  # 更新活跃度
+        update_activity(uid)  # 更新活跃度
         # 准备调用api, 用来获取头像
-        repo_1 = f"好欸！{req_user_card}({uid})用时{random.randint(1, 20)}秒 \n给 {lucky_user_card}({lucky_user}) 注入了{ejaculation}毫升的脱氧核糖核酸, 当日总注入量为：{utils.get_today_ejaculation(lucky_user)}"
+        repo_1 = f"好欸！{req_user_card}({uid})用时{random.randint(1, 20)}秒 \n给 {lucky_user_card}({lucky_user}) 注入了{ejaculation}毫升的脱氧核糖核酸, 当日总注入量为：{get_today_ejaculation_data(int(lucky_user))}毫升\n"
         await matcher.send(
             repo_1
-            + MessageSegment.image(f"http://q1.qlogo.cn/g?b=qq&nk={lucky_user}&s=640")
+            + MessageSegment.image(f"https://q1.qlogo.cn/g?b=qq&nk={lucky_user}&s=640")
         )  # 结束
 
     @staticmethod
     async def open_module(
         matcher: Matcher, event: GroupMessageEvent, args: Tuple = RegexGroup()
     ) -> None:
         """开关"""
-        gid = str(event.group_id)
+        gid: int = event.group_id
         command: str = args[0]
         if "开启" in command or "开始" in command:
-            if gid in utils.groupdata:
-                utils.groupdata[gid]["allow"] = True
-            else:
-                utils.groupdata.update({gid: {"allow": True}})
-            utils.write_group_data()
+            set_group_allow(gid, True)
             await matcher.finish("功能已开启喵")
         elif "禁止" in command or "关闭" in command:
-            if gid in utils.groupdata:
-                utils.groupdata[gid]["allow"] = False
-            else:
-                utils.groupdata.update({gid: {"allow": False}})
-            utils.write_group_data()
+            set_group_allow(gid, False)
             await matcher.finish("功能已禁用喵")
 
     @staticmethod
     async def query_injection(
         matcher: Matcher, event: GroupMessageEvent, args: Message = CommandArg()
     ) -> None:
         """查询某人的注入量"""
-        if not (await utils.check_group_allow(str(event.group_id))):
+        if not check_group_allow(event.group_id):
             await matcher.finish(utils.not_allow, at_sender=True)
         target = args.extract_plain_text()  # 获取命令参数
         user_id: str = event.get_user_id()
         # 判断带不带at
         [object_id, replay1] = (
             [await utils.get_at(event), "该用户"]
             if await utils.get_at(event) != "寄"
             else [user_id, "您"]
         )
+        #  获取用户的所有注入数据
+        data: List[Dict] = get_ejaculation_data(int(object_id))
         ejaculation = 0  # 先初始化0
         if "历史" in target or "全部" in target:
-            try:
-                date = utils.ejaculation_data[object_id]  # 对象不存在直接输出0
-            except Exception:
+            if not data:
                 await matcher.finish(f"{replay1}历史总被注射量为0ml")
             inject_data = {}
-            for key in date:  # 遍历所有的日期
-                temp = date[key]["ejaculation"]
+            for item in data:  # 遍历所有的日期
+                temp: float = item["volume"]  # 获取注入量
                 ejaculation += temp  # 注入量求和
-                inject_data[key] = temp
+                date: str = item["date"]  # 获取日期
+                inject_data[date] = temp
             if len(inject_data) < 2:
                 await matcher.finish(f"{replay1}历史总被注射量为{ejaculation}ml")
 
             await matcher.finish(
                 MessageSegment.text(f"{replay1}历史总被注射量为{ejaculation}ml")
                 + MessageSegment.image(
                     await draw_bar_chart.draw_line_chart(inject_data)
                 )
             )
         else:
-            ejaculation = utils.get_today_ejaculation(object_id)  # 获取对象当天的注入量
+            ejaculation: float = get_today_ejaculation_data(int(object_id))
             await matcher.finish(f"{replay1}当日总被注射量为{ejaculation}ml")
 
     @staticmethod
     async def yinpa_introduce(matcher: Matcher) -> None:
         """输出用法"""
         await matcher.send(MessageSegment.image(await utils.plugin_usage()))
```

### Comparing `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/txt2img.py` & `nonebot_plugin_impact-0.7.114514/nonebot_plugin_impact/txt2img.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+"""一个工具类, 将文本转换为图片, 根据文本长度自动换行"""
 from io import BytesIO
+from pathlib import Path
 
 from PIL import Image, ImageDraw, ImageFont
-from pathlib import Path
 
 
 class TxtToImg:
     def __init__(self) -> None:
         self.LINE_CHAR_COUNT = 30 * 2
         self.CHAR_SIZE = 30
         self.TABLE_WIDTH = 4
```

### Comparing `nonebot_plugin_impact-0.6.114514/setup.py` & `nonebot_plugin_impact-0.7.114514/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name="nonebot_plugin_impact",
-    version="0.06.114514",
+    version="0.07.114514",
     author="Special-Week",
     author_email="HuaMing27499@gmail.com",
     description="让群友们眼前一黑的nonebot2淫趴插件",
     python_requires=">=3.8.0",
     packages=find_packages(),
     url="https://github.com/Special-Week/nonebot_plugin_impact",
     package_data={"nonebot_plugin_impact": ["fonts/*"]},
     # 设置依赖包
-    install_requires=["pillow", "nonebot2", "nonebot-adapter-onebot"],
+    install_requires=["pillow", "nonebot2", "nonebot-adapter-onebot","sqlalchemy"],
 )
```

