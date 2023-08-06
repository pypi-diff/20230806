# Comparing `tmp/aiogram_widgets-1.2.3.tar.gz` & `tmp/aiogram_widgets-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_widgets-1.2.3.tar", max compression
+gzip compressed data, was "aiogram_widgets-1.2.4.tar", max compression
```

## Comparing `aiogram_widgets-1.2.3.tar` & `aiogram_widgets-1.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       23 2023-08-03 19:27:06.733984 aiogram_widgets-1.2.3/aiogram_widgets/__meta__.py
--rw-r--r--   0        0        0      121 2023-08-03 20:33:55.339887 aiogram_widgets-1.2.3/aiogram_widgets/enums.py
--rw-r--r--   0        0        0       74 2023-08-02 11:45:02.390573 aiogram_widgets-1.2.3/aiogram_widgets/pagination/__init__.py
--rw-r--r--   0        0        0     5228 2023-08-04 08:47:21.672288 aiogram_widgets-1.2.3/aiogram_widgets/pagination/_base.py
--rw-r--r--   0        0        0     3063 2023-08-04 08:47:10.595891 aiogram_widgets-1.2.3/aiogram_widgets/pagination/keyboard.py
--rw-r--r--   0        0        0     3437 2023-08-04 08:47:58.099543 aiogram_widgets-1.2.3/aiogram_widgets/pagination/text.py
--rw-r--r--   0        0        0      885 2023-08-04 08:39:34.265847 aiogram_widgets-1.2.3/aiogram_widgets/types.py
--rw-r--r--   0        0        0     1088 2023-08-02 14:37:27.882686 aiogram_widgets-1.2.3/LICENSE
--rw-r--r--   0        0        0      810 2023-08-04 09:26:19.727895 aiogram_widgets-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     4614 2023-08-04 09:26:06.489775 aiogram_widgets-1.2.3/README.md
--rw-r--r--   0        0        0     5089 1970-01-01 00:00:00.000000 aiogram_widgets-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-08-03 19:27:06.733984 aiogram_widgets-1.2.4/aiogram_widgets/__meta__.py
+-rw-r--r--   0        0        0      121 2023-08-03 20:33:55.339887 aiogram_widgets-1.2.4/aiogram_widgets/enums.py
+-rw-r--r--   0        0        0       74 2023-08-02 11:45:02.390573 aiogram_widgets-1.2.4/aiogram_widgets/pagination/__init__.py
+-rw-r--r--   0        0        0     5228 2023-08-04 08:47:21.672288 aiogram_widgets-1.2.4/aiogram_widgets/pagination/_base.py
+-rw-r--r--   0        0        0     3041 2023-08-04 09:48:09.372743 aiogram_widgets-1.2.4/aiogram_widgets/pagination/keyboard.py
+-rw-r--r--   0        0        0     3415 2023-08-04 09:48:15.293581 aiogram_widgets-1.2.4/aiogram_widgets/pagination/text.py
+-rw-r--r--   0        0        0      885 2023-08-04 08:39:34.265847 aiogram_widgets-1.2.4/aiogram_widgets/types.py
+-rw-r--r--   0        0        0     1088 2023-08-02 14:37:27.882686 aiogram_widgets-1.2.4/LICENSE
+-rw-r--r--   0        0        0      812 2023-08-06 19:27:13.617851 aiogram_widgets-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4613 2023-08-04 09:29:18.622244 aiogram_widgets-1.2.4/README.md
+-rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 aiogram_widgets-1.2.4/PKG-INFO
```

### Comparing `aiogram_widgets-1.2.3/aiogram_widgets/pagination/_base.py` & `aiogram_widgets-1.2.4/aiogram_widgets/pagination/_base.py`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-1.2.3/aiogram_widgets/pagination/keyboard.py` & `aiogram_widgets-1.2.4/aiogram_widgets/pagination/keyboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 "text": "Button name 999",
                 "callback_data": "callback_data_999",
             },
         ]
 
         :param router: pagination automatization. (`required`)
         :param additional_buttons: provide additional buttons, that will be inserted after pagination panel. `(default=None)`
-        :param pagination_key: callback data, which will be attached to the callback of each pagination button `(default="text_paginated")`
+        :param pagination_key: custom callback data, which will be attached to the callback of each pagination button
         :param pagination_buttons: list of `four` buttons, where each is a string or None (if you don't want to add this button) `(default=["⏪", "⬅️", "➡️", "⏩"])`
         :param per_row: amount of items per row `(default=2)`
         :param per_page: amount of items per page `(default=10)`
         """
         self.per_row = per_row
         super().__init__(
             data=data,
```

### Comparing `aiogram_widgets-1.2.3/aiogram_widgets/pagination/text.py` & `aiogram_widgets-1.2.4/aiogram_widgets/pagination/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                         "Text number 999",
             ],
         ]
 
         :param router: pagination automatization. (`required`)
         :param join_symbol: string, which will `join` current text chunk to one text `(default=new string)`
         :param additional_buttons: provide additional buttons, that will be inserted after pagination panel. `(default=None)`
-        :param pagination_key: callback data, which will be attached to the callback of each pagination button `(default="text_paginated")`
+        :param pagination_key: custom callback data, which will be attached to the callback of each pagination button
         :param pagination_buttons: list of `four` buttons, where each is a string or None (if you don't want to add this button) `(default=["⏪", "⬅️", "➡️", "⏩"])`
         :param per_page: amount of items per page `(default=10)`
         """
         super().__init__(
             data=data,
             router=router,
             additional_buttons=additional_buttons,
```

### Comparing `aiogram_widgets-1.2.3/aiogram_widgets/types.py` & `aiogram_widgets-1.2.4/aiogram_widgets/types.py`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-1.2.3/LICENSE` & `aiogram_widgets-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_widgets-1.2.3/pyproject.toml` & `aiogram_widgets-1.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiogram-widgets"
-version = "1.2.3"
+version = "1.2.4"
 readme = "README.md"
 description = "Create most popular widgets for aiogram 3 in few code lines "
 keywords = ["aiogram", "telegram api", "pagination", "calendar", "checkbox", "multiselect", "templates"]
 authors = ["ggindinson"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -15,13 +15,13 @@
 
 [project.urls]
 "Homepage" = "https://github.com/ggindinson/aiogram-widgets"
 "PyPI" = "https://pypi.python.org/pypi/aiogram_widgets/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aiogram = "3.0.0b7"
+aiogram = ">=3.0.0b1"
 pydantic = ">=1.10.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aiogram_widgets-1.2.3/README.md` & `aiogram_widgets-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,219 +71,219 @@
 00000460: 5069 703a 0d0a 0d0a 6060 6062 6173 680d  Pip:....```bash.
 00000470: 0a70 6970 2069 6e73 7461 6c6c 2061 696f  .pip install aio
 00000480: 6772 616d 5f77 6964 6765 7473 0d0a 6060  gram_widgets..``
 00000490: 600d 0a0d 0a50 6f65 7472 793a 0d0a 0d0a  `....Poetry:....
 000004a0: 6060 6062 6173 680d 0a70 6f65 7472 7920  ```bash..poetry 
 000004b0: 6164 6420 6169 6f67 7261 6d5f 7769 6467  add aiogram_widg
 000004c0: 6574 730d 0a60 6060 0d0a 0d0a 0d0a 2320  ets..```......# 
-000004d0: 215b 5d28 6874 7470 733a 2f2f 7261 772e  ![](https://raw.
-000004e0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000004f0: 742e 636f 6d2f 6767 696e 6469 6e73 6f6e  t.com/ggindinson
-00000500: 2f61 696f 6772 616d 5f77 6964 6765 7473  /aiogram_widgets
-00000510: 2f6d 6169 6e2f 6465 6d6f 2e67 6966 2920  /main/demo.gif) 
-00000520: f09f a496 205b 426f 7420 6578 616d 706c  .... [Bot exampl
-00000530: 655d 2868 7474 7073 3a2f 2f74 2e6d 652f  e](https://t.me/
-00000540: 6169 6f67 7261 6d5f 7769 6467 6574 735f  aiogram_widgets_
-00000550: 6465 6d6f 5f62 6f74 2920 7c20 5b42 6f74  demo_bot) | [Bot
-00000560: 2073 6f75 7263 6520 636f 6465 5d28 6874   source code](ht
-00000570: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000580: 2f67 6769 6e64 696e 736f 6e2f 6169 6f67  /ggindinson/aiog
-00000590: 7261 6d5f 7769 6467 6574 732f 626c 6f62  ram_widgets/blob
-000005a0: 2f6d 6169 6e2f 6578 616d 706c 652e 7079  /main/example.py
-000005b0: 2920 e29a 99ef b88f 0d0a 0d0a 0d0a 0d0a  ) ..............
-000005c0: 0d0a 0d0a 2320 5573 6167 652f 4578 616d  ....# Usage/Exam
-000005d0: 706c 6573 0d0a 0d0a 0d0a 0d0a 2323 2053  ples........## S
-000005e0: 696d 706c 6520 6b65 7962 6f61 7264 2070  imple keyboard p
-000005f0: 6167 696e 6174 696f 6e0d 0a0d 0a60 6060  agination....```
-00000600: 7079 7468 6f6e 0d0a 6672 6f6d 2061 696f  python..from aio
-00000610: 6772 616d 5f77 6964 6765 7473 2e70 6167  gram_widgets.pag
-00000620: 696e 6174 696f 6e20 696d 706f 7274 204b  ination import K
-00000630: 6579 626f 6172 6450 6167 696e 6174 6f72  eyboardPaginator
-00000640: 0d0a 0d0a 4072 6f75 7465 722e 6d65 7373  ....@router.mess
-00000650: 6167 6528 462e 7465 7874 203d 3d20 222f  age(F.text == "/
-00000660: 6b65 7962 6f61 7264 5f70 6167 696e 6174  keyboard_paginat
-00000670: 696f 6e22 290d 0a61 7379 6e63 2064 6566  ion")..async def
-00000680: 206b 6579 626f 6172 645f 7061 6769 6e61   keyboard_pagina
-00000690: 7469 6f6e 286d 6573 7361 6765 3a20 4d65  tion(message: Me
-000006a0: 7373 6167 6529 3a0d 0a20 2020 2062 7574  ssage):..    but
-000006b0: 746f 6e73 203d 205b 0d0a 2020 2020 2020  tons = [..      
-000006c0: 2020 496e 6c69 6e65 4b65 7962 6f61 7264    InlineKeyboard
-000006d0: 4275 7474 6f6e 2874 6578 743d 6622 4275  Button(text=f"Bu
-000006e0: 7474 6f6e 207b 697d 222c 2063 616c 6c62  tton {i}", callb
-000006f0: 6163 6b5f 6461 7461 3d66 2262 7574 746f  ack_data=f"butto
-00000700: 6e5f 7b69 7d22 290d 0a20 2020 2020 2020  n_{i}")..       
-00000710: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00000720: 312c 2031 3030 3129 0d0a 2020 2020 5d0d  1, 1001)..    ].
-00000730: 0a20 2020 2070 6167 696e 6174 6f72 203d  .    paginator =
-00000740: 204b 6579 626f 6172 6450 6167 696e 6174   KeyboardPaginat
-00000750: 6f72 280d 0a20 2020 2020 2020 2064 6174  or(..        dat
-00000760: 613d 6275 7474 6f6e 732c 0d0a 2020 2020  a=buttons,..    
-00000770: 2020 2020 7065 725f 7061 6765 3d32 302c      per_page=20,
-00000780: 0d0a 2020 2020 2020 2020 7065 725f 726f  ..        per_ro
-00000790: 773d 320d 0a20 2020 2029 0d0a 0d0a 0d0a  w=2..    )......
-000007a0: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-000007b0: 652e 616e 7377 6572 2874 6578 743d 224b  e.answer(text="K
-000007c0: 6579 626f 6172 6420 7061 6769 6e61 7469  eyboard paginati
-000007d0: 6f6e 222c 2072 6570 6c79 5f6d 6172 6b75  on", reply_marku
-000007e0: 703d 7061 6769 6e61 746f 722e 6173 5f6d  p=paginator.as_m
-000007f0: 6172 6b75 7028 2929 0d0a 0d0a 6060 600d  arkup())....```.
-00000800: 0a23 2320 4b65 7962 6f61 7264 2070 6167  .## Keyboard pag
-00000810: 696e 6174 696f 6e20 7769 7468 2061 6464  ination with add
-00000820: 6974 696f 6e61 6c20 6275 7474 6f6e 7320  itional buttons 
-00000830: 2853 616d 6520 7769 7468 2074 6578 7420  (Same with text 
-00000840: 7061 6769 6e61 7469 6f6e 290d 0a60 6060  pagination)..```
-00000850: 7079 7468 6f6e 0d0a 6672 6f6d 2061 696f  python..from aio
-00000860: 6772 616d 5f77 6964 6765 7473 2e70 6167  gram_widgets.pag
-00000870: 696e 6174 696f 6e20 696d 706f 7274 204b  ination import K
-00000880: 6579 626f 6172 6450 6167 696e 6174 6f72  eyboardPaginator
-00000890: 0d0a 0d0a 4072 6f75 7465 722e 6d65 7373  ....@router.mess
-000008a0: 6167 6528 462e 7465 7874 203d 3d20 222f  age(F.text == "/
-000008b0: 6b62 5f61 6464 6974 696f 6e61 6c5f 6275  kb_additional_bu
-000008c0: 7474 6f6e 7322 290d 0a61 7379 6e63 2064  ttons")..async d
-000008d0: 6566 206b 625f 6164 6469 7469 6f6e 616c  ef kb_additional
-000008e0: 5f62 7574 746f 6e73 286d 6573 7361 6765  _buttons(message
-000008f0: 3a20 4d65 7373 6167 6529 3a0d 0a20 2020  : Message):..   
-00000900: 2062 7574 746f 6e73 203d 205b 0d0a 2020   buttons = [..  
-00000910: 2020 2020 2020 496e 6c69 6e65 4b65 7962        InlineKeyb
-00000920: 6f61 7264 4275 7474 6f6e 2874 6578 743d  oardButton(text=
-00000930: 6622 4275 7474 6f6e 207b 697d 222c 2063  f"Button {i}", c
-00000940: 616c 6c62 6163 6b5f 6461 7461 3d66 2262  allback_data=f"b
-00000950: 7574 746f 6e5f 7b69 7d22 290d 0a20 2020  utton_{i}")..   
-00000960: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00000970: 6e67 6528 312c 2031 3030 3129 0d0a 2020  nge(1, 1001)..  
-00000980: 2020 5d0d 0a20 2020 2061 6464 6974 696f    ]..    additio
-00000990: 6e61 6c5f 6275 7474 6f6e 7320 3d20 5b0d  nal_buttons = [.
-000009a0: 0a20 2020 2020 2020 205b 0d0a 2020 2020  .        [..    
-000009b0: 2020 2020 2020 2020 496e 6c69 6e65 4b65          InlineKe
-000009c0: 7962 6f61 7264 4275 7474 6f6e 2874 6578  yboardButton(tex
-000009d0: 743d 2247 6f20 6261 636b 20f0 9f94 9922  t="Go back ...."
-000009e0: 2c20 6361 6c6c 6261 636b 5f64 6174 613d  , callback_data=
-000009f0: 2267 6f5f 6261 636b 2229 2c0d 0a20 2020  "go_back"),..   
-00000a00: 2020 2020 205d 0d0a 2020 2020 5d0d 0a20       ]..    ].. 
-00000a10: 2020 200d 0a20 2020 2070 6167 696e 6174     ..    paginat
-00000a20: 6f72 203d 204b 6579 626f 6172 6450 6167  or = KeyboardPag
-00000a30: 696e 6174 6f72 280d 0a20 2020 2020 2020  inator(..       
-00000a40: 2064 6174 613d 6275 7474 6f6e 732c 0d0a   data=buttons,..
-00000a50: 2020 2020 2020 2020 6164 6469 7469 6f6e          addition
-00000a60: 616c 5f62 7574 746f 6e73 3d61 6464 6974  al_buttons=addit
-00000a70: 696f 6e61 6c5f 6275 7474 6f6e 732c 2020  ional_buttons,  
-00000a80: 2020 0d0a 2020 2020 2020 2020 7065 725f    ..        per_
-00000a90: 7061 6765 3d32 302c 200d 0a20 2020 2020  page=20, ..     
-00000aa0: 2020 2070 6572 5f72 6f77 3d32 0d0a 2020     per_row=2..  
-00000ab0: 2020 290d 0a0d 0a20 2020 2061 7761 6974    )....    await
-00000ac0: 206d 6573 7361 6765 2e61 6e73 7765 7228   message.answer(
-00000ad0: 0d0a 2020 2020 2020 2020 7465 7874 3d22  ..        text="
-00000ae0: 4b65 7962 6f61 7264 2070 6167 696e 6174  Keyboard paginat
-00000af0: 696f 6e20 7769 7468 2061 6464 6974 696f  ion with additio
-00000b00: 6e61 6c20 6275 7474 6f6e 7322 2c0d 0a20  nal buttons",.. 
-00000b10: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-00000b20: 6b75 703d 7061 6769 6e61 746f 722e 6173  kup=paginator.as
-00000b30: 5f6d 6172 6b75 7028 292c 0d0a 2020 2020  _markup(),..    
-00000b40: 290d 0a0d 0a60 6060 0d0a 2323 204b 6579  )....```..## Key
-00000b50: 626f 6172 6420 7061 6769 6e61 7469 6f6e  board pagination
-00000b60: 2077 6974 6820 6375 7374 6f6d 2070 6167   with custom pag
-00000b70: 696e 6174 696f 6e20 6275 7474 6f6e 7320  ination buttons 
-00000b80: 2853 616d 6520 7769 7468 2074 6578 7420  (Same with text 
-00000b90: 7061 6769 6e61 7469 6f6e 290d 0a60 6060  pagination)..```
-00000ba0: 2070 7974 686f 6e0d 0a40 726f 7574 6572   python..@router
-00000bb0: 2e6d 6573 7361 6765 2846 2e74 6578 7420  .message(F.text 
-00000bc0: 3d3d 2022 2f6b 625f 6375 7374 6f6d 5f70  == "/kb_custom_p
-00000bd0: 6167 696e 6174 696f 6e22 290d 0a61 7379  agination")..asy
-00000be0: 6e63 2064 6566 206b 625f 6375 7374 6f6d  nc def kb_custom
-00000bf0: 5f70 6167 696e 6174 696f 6e28 6d65 7373  _pagination(mess
-00000c00: 6167 653a 204d 6573 7361 6765 293a 0d0a  age: Message):..
-00000c10: 2020 2020 7465 7874 5f64 6174 6120 3d20      text_data = 
-00000c20: 5b66 2249 2061 6d20 7374 7269 6e67 206e  [f"I am string n
-00000c30: 756d 6265 7220 7b69 7d22 2066 6f72 2069  umber {i}" for i
-00000c40: 2069 6e20 7261 6e67 6528 312c 2031 3030   in range(1, 100
-00000c50: 3129 5d0d 0a20 2020 2070 6167 696e 6174  1)]..    paginat
-00000c60: 696f 6e5f 6275 7474 6f6e 7320 3d20 5b0d  ion_buttons = [.
-00000c70: 0a20 2020 2020 2020 204e 6f6e 652c 2022  .        None, "
-00000c80: 3c2d 222c 2022 2d3e 222c 204e 6f6e 650d  <-", "->", None.
-00000c90: 0a20 2020 205d 0d0a 0d0a 2020 2020 7061  .    ]....    pa
-00000ca0: 6769 6e61 746f 7220 3d20 5465 7874 5061  ginator = TextPa
-00000cb0: 6769 6e61 746f 7228 0d0a 2020 2020 2020  ginator(..      
-00000cc0: 2020 6461 7461 3d74 6578 745f 6461 7461    data=text_data
-00000cd0: 2c0d 0a20 2020 2020 2020 2070 6167 696e  ,..        pagin
-00000ce0: 6174 696f 6e5f 6275 7474 6f6e 733d 7061  ation_buttons=pa
-00000cf0: 6769 6e61 7469 6f6e 5f62 7574 746f 6e73  gination_buttons
-00000d00: 2c0d 0a20 2020 2029 0d0a 0d0a 2020 2020  ,..    )....    
-00000d10: 6375 7272 656e 745f 7465 7874 5f63 6875  current_text_chu
-00000d20: 6e6b 2c20 7265 706c 795f 6d61 726b 7570  nk, reply_markup
-00000d30: 203d 2070 6167 696e 6174 6f72 2e63 7572   = paginator.cur
-00000d40: 7265 6e74 5f6d 6573 7361 6765 5f64 6174  rent_message_dat
-00000d50: 610d 0a0d 0a20 2020 2061 7761 6974 206d  a....    await m
-00000d60: 6573 7361 6765 2e61 6e73 7765 7228 0d0a  essage.answer(..
-00000d70: 2020 2020 2020 2020 7465 7874 3d63 7572          text=cur
-00000d80: 7265 6e74 5f74 6578 745f 6368 756e 6b2c  rent_text_chunk,
-00000d90: 0d0a 2020 2020 2020 2020 7265 706c 795f  ..        reply_
-00000da0: 6d61 726b 7570 3d72 6570 6c79 5f6d 6172  markup=reply_mar
-00000db0: 6b75 702c 0d0a 2020 2020 290d 0a0d 0a60  kup,..    )....`
-00000dc0: 6060 0d0a 0d0a 2323 2053 696d 706c 6520  ``....## Simple 
-00000dd0: 7465 7874 2070 6167 696e 6174 696f 6e0d  text pagination.
-00000de0: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00000df0: 2061 696f 6772 616d 5f77 6964 6765 7473   aiogram_widgets
-00000e00: 2e70 6167 696e 6174 696f 6e20 696d 706f  .pagination impo
-00000e10: 7274 2054 6578 7450 6167 696e 6174 6f72  rt TextPaginator
-00000e20: 0d0a 0d0a 0d0a 4072 6f75 7465 722e 6d65  ......@router.me
-00000e30: 7373 6167 6528 462e 7465 7874 203d 3d20  ssage(F.text == 
-00000e40: 222f 7465 7874 5f70 6167 696e 6174 696f  "/text_paginatio
-00000e50: 6e22 290d 0a61 7379 6e63 2064 6566 2074  n")..async def t
-00000e60: 6578 745f 7061 6769 6e61 7469 6f6e 286d  ext_pagination(m
-00000e70: 6573 7361 6765 3a20 4d65 7373 6167 6529  essage: Message)
-00000e80: 3a0d 0a20 2020 2074 6578 745f 6461 7461  :..    text_data
-00000e90: 203d 205b 0d0a 2020 2020 2020 2020 6622   = [..        f"
-00000ea0: 4920 616d 2073 7472 696e 6720 6e75 6d62  I am string numb
-00000eb0: 6572 207b 697d 220d 0a20 2020 2020 2020  er {i}"..       
-00000ec0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00000ed0: 312c 2031 3030 3129 0d0a 2020 2020 5d0d  1, 1001)..    ].
-00000ee0: 0a20 2020 200d 0a20 2020 2070 6167 696e  .    ..    pagin
-00000ef0: 6174 6f72 203d 2054 6578 7450 6167 696e  ator = TextPagin
-00000f00: 6174 6f72 280d 0a20 2020 2020 2020 2064  ator(..        d
-00000f10: 6174 613d 7465 7874 5f64 6174 612c 0d0a  ata=text_data,..
-00000f20: 2020 2020 290d 0a0d 0a20 2020 2063 7572      )....    cur
-00000f30: 7265 6e74 5f74 6578 745f 6368 756e 6b2c  rent_text_chunk,
-00000f40: 2072 6570 6c79 5f6d 6172 6b75 7020 3d20   reply_markup = 
-00000f50: 7061 6769 6e61 746f 722e 6375 7272 656e  paginator.curren
-00000f60: 745f 6d65 7373 6167 655f 6461 7461 0d0a  t_message_data..
-00000f70: 0d0a 2020 2020 6177 6169 7420 6d65 7373  ..    await mess
-00000f80: 6167 652e 616e 7377 6572 280d 0a20 2020  age.answer(..   
-00000f90: 2020 2020 2074 6578 743d 6375 7272 656e       text=curren
-00000fa0: 745f 7465 7874 5f63 6875 6e6b 2c0d 0a20  t_text_chunk,.. 
-00000fb0: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-00000fc0: 6b75 703d 7265 706c 795f 6d61 726b 7570  kup=reply_markup
-00000fd0: 2c0d 0a20 2020 2029 0d0a 0d0a 6060 600d  ,..    )....```.
-00000fe0: 0a0d 0a0d 0a23 2320 5465 7874 2070 6167  .....## Text pag
-00000ff0: 696e 6174 696f 6e20 7769 7468 2063 7573  ination with cus
-00001000: 746f 6d20 6a6f 696e 0d0a 0d0a 6060 6070  tom join....```p
-00001010: 7974 686f 6e0d 0a40 726f 7574 6572 2e6d  ython..@router.m
-00001020: 6573 7361 6765 2846 2e74 6578 7420 3d3d  essage(F.text ==
-00001030: 2022 2f74 6578 745f 6a6f 696e 2229 0d0a   "/text_join")..
-00001040: 6173 796e 6320 6465 6620 7465 7874 5f63  async def text_c
-00001050: 7573 746f 6d5f 6a6f 696e 286d 6573 7361  ustom_join(messa
-00001060: 6765 3a20 4d65 7373 6167 6529 3a0d 0a20  ge: Message):.. 
-00001070: 2020 2074 6578 745f 6461 7461 203d 205b     text_data = [
-00001080: 6622 4920 616d 2073 7472 696e 6720 6e75  f"I am string nu
-00001090: 6d62 6572 207b 697d 2220 666f 7220 6920  mber {i}" for i 
-000010a0: 696e 2072 616e 6765 2831 2c20 3130 3031  in range(1, 1001
-000010b0: 295d 0d0a 0d0a 2020 2020 7061 6769 6e61  )]....    pagina
-000010c0: 746f 7220 3d20 5465 7874 5061 6769 6e61  tor = TextPagina
-000010d0: 746f 7228 0d0a 2020 2020 2020 2020 6461  tor(..        da
-000010e0: 7461 3d74 6578 745f 6461 7461 2c0d 0a20  ta=text_data,.. 
-000010f0: 2020 2020 2020 206a 6f69 6e5f 7379 6d62         join_symb
-00001100: 6f6c 3d22 5c6e 5c6e 222c 0d0a 2020 2020  ol="\n\n",..    
-00001110: 290d 0a20 2020 2063 7572 7265 6e74 5f74  )..    current_t
-00001120: 6578 745f 6368 756e 6b2c 2072 6570 6c79  ext_chunk, reply
-00001130: 5f6d 6172 6b75 7020 3d20 7061 6769 6e61  _markup = pagina
-00001140: 746f 722e 6375 7272 656e 745f 6d65 7373  tor.current_mess
-00001150: 6167 655f 6461 7461 0d0a 0d0a 2020 2020  age_data....    
-00001160: 6177 6169 7420 6d65 7373 6167 652e 616e  await message.an
-00001170: 7377 6572 280d 0a20 2020 2020 2020 2074  swer(..        t
-00001180: 6578 743d 6375 7272 656e 745f 7465 7874  ext=current_text
-00001190: 5f63 6875 6e6b 2c0d 0a20 2020 2020 2020  _chunk,..       
-000011a0: 2072 6570 6c79 5f6d 6172 6b75 703d 7265   reply_markup=re
-000011b0: 706c 795f 6d61 726b 7570 2c0d 0a20 2020  ply_markup,..   
-000011c0: 2029 0d0a 0d0a 6060 600d 0a0d 0a23 2046   )....```....# F
-000011d0: 6565 6462 6163 6b0d 0a0d 0a49 2077 6f75  eedback....I wou
-000011e0: 6c64 2062 6520 7665 7279 2070 6c65 6173  ld be very pleas
-000011f0: 6564 2066 6f72 2061 2073 7461 7220 e2ad  ed for a star ..
-00001200: 90ef b88f 0d0a                           ......
+000004d0: f09f a496 205b 426f 7420 6578 616d 706c  .... [Bot exampl
+000004e0: 655d 2868 7474 7073 3a2f 2f74 2e6d 652f  e](https://t.me/
+000004f0: 6169 6f67 7261 6d5f 7769 6467 6574 735f  aiogram_widgets_
+00000500: 6465 6d6f 5f62 6f74 2920 7c20 5b42 6f74  demo_bot) | [Bot
+00000510: 2073 6f75 7263 6520 636f 6465 5d28 6874   source code](ht
+00000520: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000530: 2f67 6769 6e64 696e 736f 6e2f 6169 6f67  /ggindinson/aiog
+00000540: 7261 6d5f 7769 6467 6574 732f 626c 6f62  ram_widgets/blob
+00000550: 2f6d 6169 6e2f 6578 616d 706c 652e 7079  /main/example.py
+00000560: 2920 e29a 99ef b88f 0d0a 215b 5d28 6874  ) ........![](ht
+00000570: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000580: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000590: 6767 696e 6469 6e73 6f6e 2f61 696f 6772  ggindinson/aiogr
+000005a0: 616d 5f77 6964 6765 7473 2f6d 6169 6e2f  am_widgets/main/
+000005b0: 6465 6d6f 2e67 6966 290d 0a0d 0a0d 0a0d  demo.gif).......
+000005c0: 0a0d 0a23 2055 7361 6765 2f45 7861 6d70  ...# Usage/Examp
+000005d0: 6c65 730d 0a0d 0a0d 0a0d 0a23 2320 5369  les........## Si
+000005e0: 6d70 6c65 206b 6579 626f 6172 6420 7061  mple keyboard pa
+000005f0: 6769 6e61 7469 6f6e 0d0a 0d0a 6060 6070  gination....```p
+00000600: 7974 686f 6e0d 0a66 726f 6d20 6169 6f67  ython..from aiog
+00000610: 7261 6d5f 7769 6467 6574 732e 7061 6769  ram_widgets.pagi
+00000620: 6e61 7469 6f6e 2069 6d70 6f72 7420 4b65  nation import Ke
+00000630: 7962 6f61 7264 5061 6769 6e61 746f 720d  yboardPaginator.
+00000640: 0a0d 0a40 726f 7574 6572 2e6d 6573 7361  ...@router.messa
+00000650: 6765 2846 2e74 6578 7420 3d3d 2022 2f6b  ge(F.text == "/k
+00000660: 6579 626f 6172 645f 7061 6769 6e61 7469  eyboard_paginati
+00000670: 6f6e 2229 0d0a 6173 796e 6320 6465 6620  on")..async def 
+00000680: 6b65 7962 6f61 7264 5f70 6167 696e 6174  keyboard_paginat
+00000690: 696f 6e28 6d65 7373 6167 653a 204d 6573  ion(message: Mes
+000006a0: 7361 6765 293a 0d0a 2020 2020 6275 7474  sage):..    butt
+000006b0: 6f6e 7320 3d20 5b0d 0a20 2020 2020 2020  ons = [..       
+000006c0: 2049 6e6c 696e 654b 6579 626f 6172 6442   InlineKeyboardB
+000006d0: 7574 746f 6e28 7465 7874 3d66 2242 7574  utton(text=f"But
+000006e0: 746f 6e20 7b69 7d22 2c20 6361 6c6c 6261  ton {i}", callba
+000006f0: 636b 5f64 6174 613d 6622 6275 7474 6f6e  ck_data=f"button
+00000700: 5f7b 697d 2229 0d0a 2020 2020 2020 2020  _{i}")..        
+00000710: 666f 7220 6920 696e 2072 616e 6765 2831  for i in range(1
+00000720: 2c20 3130 3031 290d 0a20 2020 205d 0d0a  , 1001)..    ]..
+00000730: 2020 2020 7061 6769 6e61 746f 7220 3d20      paginator = 
+00000740: 4b65 7962 6f61 7264 5061 6769 6e61 746f  KeyboardPaginato
+00000750: 7228 0d0a 2020 2020 2020 2020 6461 7461  r(..        data
+00000760: 3d62 7574 746f 6e73 2c0d 0a20 2020 2020  =buttons,..     
+00000770: 2020 2070 6572 5f70 6167 653d 3230 2c0d     per_page=20,.
+00000780: 0a20 2020 2020 2020 2070 6572 5f72 6f77  .        per_row
+00000790: 3d32 0d0a 2020 2020 290d 0a0d 0a0d 0a20  =2..    )...... 
+000007a0: 2020 2061 7761 6974 206d 6573 7361 6765     await message
+000007b0: 2e61 6e73 7765 7228 7465 7874 3d22 4b65  .answer(text="Ke
+000007c0: 7962 6f61 7264 2070 6167 696e 6174 696f  yboard paginatio
+000007d0: 6e22 2c20 7265 706c 795f 6d61 726b 7570  n", reply_markup
+000007e0: 3d70 6167 696e 6174 6f72 2e61 735f 6d61  =paginator.as_ma
+000007f0: 726b 7570 2829 290d 0a0d 0a60 6060 0d0a  rkup())....```..
+00000800: 2323 204b 6579 626f 6172 6420 7061 6769  ## Keyboard pagi
+00000810: 6e61 7469 6f6e 2077 6974 6820 6164 6469  nation with addi
+00000820: 7469 6f6e 616c 2062 7574 746f 6e73 2028  tional buttons (
+00000830: 5361 6d65 2077 6974 6820 7465 7874 2070  Same with text p
+00000840: 6167 696e 6174 696f 6e29 0d0a 6060 6070  agination)..```p
+00000850: 7974 686f 6e0d 0a66 726f 6d20 6169 6f67  ython..from aiog
+00000860: 7261 6d5f 7769 6467 6574 732e 7061 6769  ram_widgets.pagi
+00000870: 6e61 7469 6f6e 2069 6d70 6f72 7420 4b65  nation import Ke
+00000880: 7962 6f61 7264 5061 6769 6e61 746f 720d  yboardPaginator.
+00000890: 0a0d 0a40 726f 7574 6572 2e6d 6573 7361  ...@router.messa
+000008a0: 6765 2846 2e74 6578 7420 3d3d 2022 2f6b  ge(F.text == "/k
+000008b0: 625f 6164 6469 7469 6f6e 616c 5f62 7574  b_additional_but
+000008c0: 746f 6e73 2229 0d0a 6173 796e 6320 6465  tons")..async de
+000008d0: 6620 6b62 5f61 6464 6974 696f 6e61 6c5f  f kb_additional_
+000008e0: 6275 7474 6f6e 7328 6d65 7373 6167 653a  buttons(message:
+000008f0: 204d 6573 7361 6765 293a 0d0a 2020 2020   Message):..    
+00000900: 6275 7474 6f6e 7320 3d20 5b0d 0a20 2020  buttons = [..   
+00000910: 2020 2020 2049 6e6c 696e 654b 6579 626f       InlineKeybo
+00000920: 6172 6442 7574 746f 6e28 7465 7874 3d66  ardButton(text=f
+00000930: 2242 7574 746f 6e20 7b69 7d22 2c20 6361  "Button {i}", ca
+00000940: 6c6c 6261 636b 5f64 6174 613d 6622 6275  llback_data=f"bu
+00000950: 7474 6f6e 5f7b 697d 2229 0d0a 2020 2020  tton_{i}")..    
+00000960: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00000970: 6765 2831 2c20 3130 3031 290d 0a20 2020  ge(1, 1001)..   
+00000980: 205d 0d0a 2020 2020 6164 6469 7469 6f6e   ]..    addition
+00000990: 616c 5f62 7574 746f 6e73 203d 205b 0d0a  al_buttons = [..
+000009a0: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
+000009b0: 2020 2020 2020 2049 6e6c 696e 654b 6579         InlineKey
+000009c0: 626f 6172 6442 7574 746f 6e28 7465 7874  boardButton(text
+000009d0: 3d22 476f 2062 6163 6b20 f09f 9499 222c  ="Go back ....",
+000009e0: 2063 616c 6c62 6163 6b5f 6461 7461 3d22   callback_data="
+000009f0: 676f 5f62 6163 6b22 292c 0d0a 2020 2020  go_back"),..    
+00000a00: 2020 2020 5d0d 0a20 2020 205d 0d0a 2020      ]..    ]..  
+00000a10: 2020 0d0a 2020 2020 7061 6769 6e61 746f    ..    paginato
+00000a20: 7220 3d20 4b65 7962 6f61 7264 5061 6769  r = KeyboardPagi
+00000a30: 6e61 746f 7228 0d0a 2020 2020 2020 2020  nator(..        
+00000a40: 6461 7461 3d62 7574 746f 6e73 2c0d 0a20  data=buttons,.. 
+00000a50: 2020 2020 2020 2061 6464 6974 696f 6e61         additiona
+00000a60: 6c5f 6275 7474 6f6e 733d 6164 6469 7469  l_buttons=additi
+00000a70: 6f6e 616c 5f62 7574 746f 6e73 2c20 2020  onal_buttons,   
+00000a80: 200d 0a20 2020 2020 2020 2070 6572 5f70   ..        per_p
+00000a90: 6167 653d 3230 2c20 0d0a 2020 2020 2020  age=20, ..      
+00000aa0: 2020 7065 725f 726f 773d 320d 0a20 2020    per_row=2..   
+00000ab0: 2029 0d0a 0d0a 2020 2020 6177 6169 7420   )....    await 
+00000ac0: 6d65 7373 6167 652e 616e 7377 6572 280d  message.answer(.
+00000ad0: 0a20 2020 2020 2020 2074 6578 743d 224b  .        text="K
+00000ae0: 6579 626f 6172 6420 7061 6769 6e61 7469  eyboard paginati
+00000af0: 6f6e 2077 6974 6820 6164 6469 7469 6f6e  on with addition
+00000b00: 616c 2062 7574 746f 6e73 222c 0d0a 2020  al buttons",..  
+00000b10: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+00000b20: 7570 3d70 6167 696e 6174 6f72 2e61 735f  up=paginator.as_
+00000b30: 6d61 726b 7570 2829 2c0d 0a20 2020 2029  markup(),..    )
+00000b40: 0d0a 0d0a 6060 600d 0a23 2320 4b65 7962  ....```..## Keyb
+00000b50: 6f61 7264 2070 6167 696e 6174 696f 6e20  oard pagination 
+00000b60: 7769 7468 2063 7573 746f 6d20 7061 6769  with custom pagi
+00000b70: 6e61 7469 6f6e 2062 7574 746f 6e73 2028  nation buttons (
+00000b80: 5361 6d65 2077 6974 6820 7465 7874 2070  Same with text p
+00000b90: 6167 696e 6174 696f 6e29 0d0a 6060 6020  agination)..``` 
+00000ba0: 7079 7468 6f6e 0d0a 4072 6f75 7465 722e  python..@router.
+00000bb0: 6d65 7373 6167 6528 462e 7465 7874 203d  message(F.text =
+00000bc0: 3d20 222f 6b62 5f63 7573 746f 6d5f 7061  = "/kb_custom_pa
+00000bd0: 6769 6e61 7469 6f6e 2229 0d0a 6173 796e  gination")..asyn
+00000be0: 6320 6465 6620 6b62 5f63 7573 746f 6d5f  c def kb_custom_
+00000bf0: 7061 6769 6e61 7469 6f6e 286d 6573 7361  pagination(messa
+00000c00: 6765 3a20 4d65 7373 6167 6529 3a0d 0a20  ge: Message):.. 
+00000c10: 2020 2074 6578 745f 6461 7461 203d 205b     text_data = [
+00000c20: 6622 4920 616d 2073 7472 696e 6720 6e75  f"I am string nu
+00000c30: 6d62 6572 207b 697d 2220 666f 7220 6920  mber {i}" for i 
+00000c40: 696e 2072 616e 6765 2831 2c20 3130 3031  in range(1, 1001
+00000c50: 295d 0d0a 2020 2020 7061 6769 6e61 7469  )]..    paginati
+00000c60: 6f6e 5f62 7574 746f 6e73 203d 205b 0d0a  on_buttons = [..
+00000c70: 2020 2020 2020 2020 4e6f 6e65 2c20 223c          None, "<
+00000c80: 2d22 2c20 222d 3e22 2c20 4e6f 6e65 0d0a  -", "->", None..
+00000c90: 2020 2020 5d0d 0a0d 0a20 2020 2070 6167      ]....    pag
+00000ca0: 696e 6174 6f72 203d 2054 6578 7450 6167  inator = TextPag
+00000cb0: 696e 6174 6f72 280d 0a20 2020 2020 2020  inator(..       
+00000cc0: 2064 6174 613d 7465 7874 5f64 6174 612c   data=text_data,
+00000cd0: 0d0a 2020 2020 2020 2020 7061 6769 6e61  ..        pagina
+00000ce0: 7469 6f6e 5f62 7574 746f 6e73 3d70 6167  tion_buttons=pag
+00000cf0: 696e 6174 696f 6e5f 6275 7474 6f6e 732c  ination_buttons,
+00000d00: 0d0a 2020 2020 290d 0a0d 0a20 2020 2063  ..    )....    c
+00000d10: 7572 7265 6e74 5f74 6578 745f 6368 756e  urrent_text_chun
+00000d20: 6b2c 2072 6570 6c79 5f6d 6172 6b75 7020  k, reply_markup 
+00000d30: 3d20 7061 6769 6e61 746f 722e 6375 7272  = paginator.curr
+00000d40: 656e 745f 6d65 7373 6167 655f 6461 7461  ent_message_data
+00000d50: 0d0a 0d0a 2020 2020 6177 6169 7420 6d65  ....    await me
+00000d60: 7373 6167 652e 616e 7377 6572 280d 0a20  ssage.answer(.. 
+00000d70: 2020 2020 2020 2074 6578 743d 6375 7272         text=curr
+00000d80: 656e 745f 7465 7874 5f63 6875 6e6b 2c0d  ent_text_chunk,.
+00000d90: 0a20 2020 2020 2020 2072 6570 6c79 5f6d  .        reply_m
+00000da0: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
+00000db0: 7570 2c0d 0a20 2020 2029 0d0a 0d0a 6060  up,..    )....``
+00000dc0: 600d 0a0d 0a23 2320 5369 6d70 6c65 2074  `....## Simple t
+00000dd0: 6578 7420 7061 6769 6e61 7469 6f6e 0d0a  ext pagination..
+00000de0: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00000df0: 6169 6f67 7261 6d5f 7769 6467 6574 732e  aiogram_widgets.
+00000e00: 7061 6769 6e61 7469 6f6e 2069 6d70 6f72  pagination impor
+00000e10: 7420 5465 7874 5061 6769 6e61 746f 720d  t TextPaginator.
+00000e20: 0a0d 0a0d 0a40 726f 7574 6572 2e6d 6573  .....@router.mes
+00000e30: 7361 6765 2846 2e74 6578 7420 3d3d 2022  sage(F.text == "
+00000e40: 2f74 6578 745f 7061 6769 6e61 7469 6f6e  /text_pagination
+00000e50: 2229 0d0a 6173 796e 6320 6465 6620 7465  ")..async def te
+00000e60: 7874 5f70 6167 696e 6174 696f 6e28 6d65  xt_pagination(me
+00000e70: 7373 6167 653a 204d 6573 7361 6765 293a  ssage: Message):
+00000e80: 0d0a 2020 2020 7465 7874 5f64 6174 6120  ..    text_data 
+00000e90: 3d20 5b0d 0a20 2020 2020 2020 2066 2249  = [..        f"I
+00000ea0: 2061 6d20 7374 7269 6e67 206e 756d 6265   am string numbe
+00000eb0: 7220 7b69 7d22 0d0a 2020 2020 2020 2020  r {i}"..        
+00000ec0: 666f 7220 6920 696e 2072 616e 6765 2831  for i in range(1
+00000ed0: 2c20 3130 3031 290d 0a20 2020 205d 0d0a  , 1001)..    ]..
+00000ee0: 2020 2020 0d0a 2020 2020 7061 6769 6e61      ..    pagina
+00000ef0: 746f 7220 3d20 5465 7874 5061 6769 6e61  tor = TextPagina
+00000f00: 746f 7228 0d0a 2020 2020 2020 2020 6461  tor(..        da
+00000f10: 7461 3d74 6578 745f 6461 7461 2c0d 0a20  ta=text_data,.. 
+00000f20: 2020 2029 0d0a 0d0a 2020 2020 6375 7272     )....    curr
+00000f30: 656e 745f 7465 7874 5f63 6875 6e6b 2c20  ent_text_chunk, 
+00000f40: 7265 706c 795f 6d61 726b 7570 203d 2070  reply_markup = p
+00000f50: 6167 696e 6174 6f72 2e63 7572 7265 6e74  aginator.current
+00000f60: 5f6d 6573 7361 6765 5f64 6174 610d 0a0d  _message_data...
+00000f70: 0a20 2020 2061 7761 6974 206d 6573 7361  .    await messa
+00000f80: 6765 2e61 6e73 7765 7228 0d0a 2020 2020  ge.answer(..    
+00000f90: 2020 2020 7465 7874 3d63 7572 7265 6e74      text=current
+00000fa0: 5f74 6578 745f 6368 756e 6b2c 0d0a 2020  _text_chunk,..  
+00000fb0: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+00000fc0: 7570 3d72 6570 6c79 5f6d 6172 6b75 702c  up=reply_markup,
+00000fd0: 0d0a 2020 2020 290d 0a0d 0a60 6060 0d0a  ..    )....```..
+00000fe0: 0d0a 0d0a 2323 2054 6578 7420 7061 6769  ....## Text pagi
+00000ff0: 6e61 7469 6f6e 2077 6974 6820 6375 7374  nation with cust
+00001000: 6f6d 206a 6f69 6e0d 0a0d 0a60 6060 7079  om join....```py
+00001010: 7468 6f6e 0d0a 4072 6f75 7465 722e 6d65  thon..@router.me
+00001020: 7373 6167 6528 462e 7465 7874 203d 3d20  ssage(F.text == 
+00001030: 222f 7465 7874 5f6a 6f69 6e22 290d 0a61  "/text_join")..a
+00001040: 7379 6e63 2064 6566 2074 6578 745f 6375  sync def text_cu
+00001050: 7374 6f6d 5f6a 6f69 6e28 6d65 7373 6167  stom_join(messag
+00001060: 653a 204d 6573 7361 6765 293a 0d0a 2020  e: Message):..  
+00001070: 2020 7465 7874 5f64 6174 6120 3d20 5b66    text_data = [f
+00001080: 2249 2061 6d20 7374 7269 6e67 206e 756d  "I am string num
+00001090: 6265 7220 7b69 7d22 2066 6f72 2069 2069  ber {i}" for i i
+000010a0: 6e20 7261 6e67 6528 312c 2031 3030 3129  n range(1, 1001)
+000010b0: 5d0d 0a0d 0a20 2020 2070 6167 696e 6174  ]....    paginat
+000010c0: 6f72 203d 2054 6578 7450 6167 696e 6174  or = TextPaginat
+000010d0: 6f72 280d 0a20 2020 2020 2020 2064 6174  or(..        dat
+000010e0: 613d 7465 7874 5f64 6174 612c 0d0a 2020  a=text_data,..  
+000010f0: 2020 2020 2020 6a6f 696e 5f73 796d 626f        join_symbo
+00001100: 6c3d 225c 6e5c 6e22 2c0d 0a20 2020 2029  l="\n\n",..    )
+00001110: 0d0a 2020 2020 6375 7272 656e 745f 7465  ..    current_te
+00001120: 7874 5f63 6875 6e6b 2c20 7265 706c 795f  xt_chunk, reply_
+00001130: 6d61 726b 7570 203d 2070 6167 696e 6174  markup = paginat
+00001140: 6f72 2e63 7572 7265 6e74 5f6d 6573 7361  or.current_messa
+00001150: 6765 5f64 6174 610d 0a0d 0a20 2020 2061  ge_data....    a
+00001160: 7761 6974 206d 6573 7361 6765 2e61 6e73  wait message.ans
+00001170: 7765 7228 0d0a 2020 2020 2020 2020 7465  wer(..        te
+00001180: 7874 3d63 7572 7265 6e74 5f74 6578 745f  xt=current_text_
+00001190: 6368 756e 6b2c 0d0a 2020 2020 2020 2020  chunk,..        
+000011a0: 7265 706c 795f 6d61 726b 7570 3d72 6570  reply_markup=rep
+000011b0: 6c79 5f6d 6172 6b75 702c 0d0a 2020 2020  ly_markup,..    
+000011c0: 290d 0a0d 0a60 6060 0d0a 0d0a 2320 4665  )....```....# Fe
+000011d0: 6564 6261 636b 0d0a 0d0a 4920 776f 756c  edback....I woul
+000011e0: 6420 6265 2076 6572 7920 706c 6561 7365  d be very please
+000011f0: 6420 666f 7220 6120 7374 6172 20e2 ad90  d for a star ...
+00001200: efb8 8f0d 0a                             .....
```

### Comparing `aiogram_widgets-1.2.3/PKG-INFO` & `aiogram_widgets-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aiogram-widgets
-Version: 1.2.3
+Version: 1.2.4
 Summary: Create most popular widgets for aiogram 3 in few code lines 
 Keywords: aiogram,telegram api,pagination,calendar,checkbox,multiselect,templates
 Author: ggindinson
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiogram (==3.0.0b7)
+Requires-Dist: aiogram (>=3.0.0b1)
 Requires-Dist: pydantic (>=1.10.4)
 Description-Content-Type: text/markdown
 
 
 
 ## aiogram_widgets
 
@@ -72,16 +72,16 @@
 Poetry:
 
 ```bash
 poetry add aiogram_widgets
 ```
 
 
-# ![](https://raw.githubusercontent.com/ggindinson/aiogram_widgets/main/demo.gif) 🤖 [Bot example](https://t.me/aiogram_widgets_demo_bot) | [Bot source code](https://github.com/ggindinson/aiogram_widgets/blob/main/example.py) ⚙️
-
+# 🤖 [Bot example](https://t.me/aiogram_widgets_demo_bot) | [Bot source code](https://github.com/ggindinson/aiogram_widgets/blob/main/example.py) ⚙️
+![](https://raw.githubusercontent.com/ggindinson/aiogram_widgets/main/demo.gif)
 
 
 
 
 # Usage/Examples
```

