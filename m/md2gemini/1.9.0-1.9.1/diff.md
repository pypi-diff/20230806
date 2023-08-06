# Comparing `tmp/md2gemini-1.9.0.tar.gz` & `tmp/md2gemini-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2gemini-1.9.0.tar", last modified: Wed Dec  8 18:15:04 2021, max compression
+gzip compressed data, was "md2gemini-1.9.1.tar", last modified: Sun Aug  6 19:25:57 2023, max compression
```

## Comparing `md2gemini-1.9.0.tar` & `md2gemini-1.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 makeworld  (1000) makeworld  (1000)        0 2021-12-08 18:15:04.900165 md2gemini-1.9.0/
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)     7652 2020-05-26 15:51:58.000000 md2gemini-1.9.0/LICENSE
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)     9753 2021-12-08 18:15:04.900165 md2gemini-1.9.0/PKG-INFO
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)     9091 2021-12-08 17:59:34.000000 md2gemini-1.9.0/README.md
-drwxr-xr-x   0 makeworld  (1000) makeworld  (1000)        0 2021-12-08 18:15:04.900165 md2gemini-1.9.0/md2gemini/
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)    12621 2021-12-08 18:02:41.000000 md2gemini-1.9.0/md2gemini/__init__.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)       90 2020-05-17 03:08:53.000000 md2gemini-1.9.0/md2gemini/__main__.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)    15723 2021-12-08 17:57:14.000000 md2gemini-1.9.0/md2gemini/renderers.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)    38753 2020-09-09 20:00:40.000000 md2gemini-1.9.0/md2gemini/unitable.py
-drwxr-xr-x   0 makeworld  (1000) makeworld  (1000)        0 2021-12-08 18:15:04.900165 md2gemini-1.9.0/md2gemini.egg-info/
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)     9753 2021-12-08 18:15:04.000000 md2gemini-1.9.0/md2gemini.egg-info/PKG-INFO
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      595 2021-12-08 18:15:04.000000 md2gemini-1.9.0/md2gemini.egg-info/SOURCES.txt
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)        1 2021-12-08 18:15:04.000000 md2gemini-1.9.0/md2gemini.egg-info/dependency_links.txt
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)       46 2021-12-08 18:15:04.000000 md2gemini-1.9.0/md2gemini.egg-info/entry_points.txt
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)       34 2021-12-08 18:15:04.000000 md2gemini-1.9.0/md2gemini.egg-info/requires.txt
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)       16 2021-12-08 18:15:04.000000 md2gemini-1.9.0/md2gemini.egg-info/top_level.txt
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)       38 2021-12-08 18:15:04.900165 md2gemini-1.9.0/setup.cfg
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)     1077 2021-12-08 17:39:01.000000 md2gemini-1.9.0/setup.py
-drwxr-xr-x   0 makeworld  (1000) makeworld  (1000)        0 2021-12-08 18:15:04.900165 md2gemini-1.9.0/tests/
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)        0 2020-09-08 18:01:50.000000 md2gemini-1.9.0/tests/__init__.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      391 2020-09-09 20:00:29.000000 md2gemini-1.9.0/tests/test_base_url.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      668 2020-09-09 20:00:29.000000 md2gemini-1.9.0/tests/test_codeblock.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      686 2020-09-09 20:00:29.000000 md2gemini-1.9.0/tests/test_frontmatter.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      359 2020-12-05 14:42:37.000000 md2gemini-1.9.0/tests/test_link_func.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      787 2021-12-08 16:27:57.000000 md2gemini-1.9.0/tests/test_links.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      608 2020-09-23 02:10:09.000000 md2gemini-1.9.0/tests/test_list.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      347 2021-12-08 15:10:04.000000 md2gemini-1.9.0/tests/test_markdown_link.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)     1142 2020-11-02 14:15:46.000000 md2gemini-1.9.0/tests/test_plain.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      964 2021-12-08 16:52:58.000000 md2gemini-1.9.0/tests/test_quote.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      977 2020-09-09 20:00:29.000000 md2gemini-1.9.0/tests/test_strip_html.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)     1429 2020-10-16 23:19:44.000000 md2gemini-1.9.0/tests/test_tags.py
--rw-r--r--   0 makeworld  (1000) makeworld  (1000)      104 2020-09-08 18:01:50.000000 md2gemini-1.9.0/tests/util.py
+drwxr-xr-x   0 makeworld  (1000) makeworld  (1000)        0 2023-08-06 19:25:57.839471 md2gemini-1.9.1/
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     7652 2020-05-26 15:51:58.000000 md2gemini-1.9.1/LICENSE
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     9934 2023-08-06 19:25:57.839471 md2gemini-1.9.1/PKG-INFO
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     9309 2023-08-06 00:46:30.000000 md2gemini-1.9.1/README.md
+drwxr-xr-x   0 makeworld  (1000) makeworld  (1000)        0 2023-08-06 19:25:57.839471 md2gemini-1.9.1/md2gemini/
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)    12260 2023-08-06 19:23:01.000000 md2gemini-1.9.1/md2gemini/__init__.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)       90 2020-05-17 03:08:53.000000 md2gemini-1.9.1/md2gemini/__main__.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)    16820 2022-12-31 03:43:04.000000 md2gemini-1.9.1/md2gemini/renderers.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)    38753 2020-09-09 20:00:40.000000 md2gemini-1.9.1/md2gemini/unitable.py
+drwxr-xr-x   0 makeworld  (1000) makeworld  (1000)        0 2023-08-06 19:25:57.839471 md2gemini-1.9.1/md2gemini.egg-info/
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     9934 2023-08-06 19:25:57.000000 md2gemini-1.9.1/md2gemini.egg-info/PKG-INFO
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      595 2023-08-06 19:25:57.000000 md2gemini-1.9.1/md2gemini.egg-info/SOURCES.txt
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)        1 2023-08-06 19:25:57.000000 md2gemini-1.9.1/md2gemini.egg-info/dependency_links.txt
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)       45 2023-08-06 19:25:57.000000 md2gemini-1.9.1/md2gemini.egg-info/entry_points.txt
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)       34 2023-08-06 19:25:57.000000 md2gemini-1.9.1/md2gemini.egg-info/requires.txt
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)       10 2023-08-06 19:25:57.000000 md2gemini-1.9.1/md2gemini.egg-info/top_level.txt
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)       38 2023-08-06 19:25:57.839471 md2gemini-1.9.1/setup.cfg
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     1064 2022-12-31 00:38:02.000000 md2gemini-1.9.1/setup.py
+drwxr-xr-x   0 makeworld  (1000) makeworld  (1000)        0 2023-08-06 19:25:57.839471 md2gemini-1.9.1/tests/
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)        0 2020-09-08 18:01:50.000000 md2gemini-1.9.1/tests/__init__.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      391 2020-09-09 20:00:29.000000 md2gemini-1.9.1/tests/test_base_url.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     2358 2022-12-31 01:12:43.000000 md2gemini-1.9.1/tests/test_codeblock.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      686 2020-09-09 20:00:29.000000 md2gemini-1.9.1/tests/test_frontmatter.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      359 2020-12-05 14:42:37.000000 md2gemini-1.9.1/tests/test_link_func.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     1947 2022-12-31 03:39:42.000000 md2gemini-1.9.1/tests/test_links.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      608 2020-09-23 02:10:09.000000 md2gemini-1.9.1/tests/test_list.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      347 2021-12-08 15:10:04.000000 md2gemini-1.9.1/tests/test_markdown_link.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     1142 2020-11-02 14:15:46.000000 md2gemini-1.9.1/tests/test_plain.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      964 2022-12-31 01:52:30.000000 md2gemini-1.9.1/tests/test_quote.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      977 2020-09-09 20:00:29.000000 md2gemini-1.9.1/tests/test_strip_html.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)     1429 2020-10-16 23:19:44.000000 md2gemini-1.9.1/tests/test_tags.py
+-rw-r--r--   0 makeworld  (1000) makeworld  (1000)      104 2020-09-08 18:01:50.000000 md2gemini-1.9.1/tests/util.py
```

### Comparing `md2gemini-1.9.0/LICENSE` & `md2gemini-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `md2gemini-1.9.0/PKG-INFO` & `md2gemini-1.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: md2gemini
-Version: 1.9.0
+Version: 1.9.1
 Summary: Convert Markdown to the Gemini text format
 Home-page: https://github.com/makeworld-the-better-one/md2gemini
 Author: makeworld
 Author-email: makeworld@protonmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Markup
 Requires-Python: >=3.7
@@ -24,14 +22,18 @@
 
 Converter from Markdown to the [Gemini](https://gemini.circumlunar.space/) text format. It works as a Python module, or a command line application.
 
 One of its key features is that it can convert inline links into footnotes. It also supports tables, and will convert them into Unicode (or ASCII) tables.
 
 Anything else that it doesn't understand will remain the same as when you wrote it, like strikethrough for example.
 
+## Project Status
+
+md2gemini is now archived. It’s always been a pile of hacks, and now I’m not that invested in continuing it. See my [blog post](https://www.makeworld.space/2023/08/bye_gemini.html) for details.
+
 ## Link modes
 
 md2gemini has several link modes, because text/gemini doesn't support inline links. These modes can be set by passing different strings to the `-l` or `--links` flags on the command line, or the `links=` argument in Python.
 
 Here is some example markdown, to show what each link mode does:
 ```markdown
 This is a paragraph with an [inline](https://example.com) link.
@@ -230,9 +232,7 @@
     URL as parameter, and should return the new link.
 
     table_tag: "The default alt text for table blocks."
 
     checklist: whether to support GitHub-style checklist list items: [ ] and [x]
     """
 ```
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `md2gemini-1.9.0/README.md` & `md2gemini-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 Converter from Markdown to the [Gemini](https://gemini.circumlunar.space/) text format. It works as a Python module, or a command line application.
 
 One of its key features is that it can convert inline links into footnotes. It also supports tables, and will convert them into Unicode (or ASCII) tables.
 
 Anything else that it doesn't understand will remain the same as when you wrote it, like strikethrough for example.
 
+## Project Status
+
+md2gemini is now archived. It’s always been a pile of hacks, and now I’m not that invested in continuing it. See my [blog post](https://www.makeworld.space/2023/08/bye_gemini.html) for details.
+
 ## Link modes
 
 md2gemini has several link modes, because text/gemini doesn't support inline links. These modes can be set by passing different strings to the `-l` or `--links` flags on the command line, or the `links=` argument in Python.
 
 Here is some example markdown, to show what each link mode does:
 ```markdown
 This is a paragraph with an [inline](https://example.com) link.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `md2gemini-1.9.0/md2gemini/__init__.py` & `md2gemini-1.9.1/md2gemini/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         pg += NEWLINE * 2  # Add a blank line between paragraphs
         gemtext = __replace_between(gemtext, PARAGRAPH_DELIM, pg)
 
     # Add in hard linebreaks
     gemtext = gemtext.replace(LINEBREAK, NEWLINE)
 
     # Add remaining footnotes at and of file
-    gemtext += NEWLINE + renderer._render_footnotes() + NEWLINE
+    gemtext += renderer._render_footnotes()
 
     # Remove double link delims, which are produced by multiple footnotes
     gemtext = gemtext.replace(LINK_DELIM + LINK_DELIM, LINK_DELIM)
     # Remove all the link delims that are next to newlines,
     # so that when link delims are replaced with newlines later in the code,
     # we don't end up with double newlines.
     gemtext = re.sub(
@@ -171,21 +171,14 @@
             continue
         if i + 1 < length - 1 and line.startswith("=>") and not pre:
             # It's a link, fix the next line by removing left whitespace
             gemlines[i + 1] = gemlines[i + 1].lstrip()
     gemtext = NEWLINE.join(gemlines)
     gemtext = gemtext.rstrip().lstrip("\r\n")
 
-    # Remove more than two newlines in a row, as there's no way to induce that in valid markdown
-    # So any time there's more than two newlines in output that's a bug with md2gemini
-    # So it gets fixed here. Hacky, but it works.
-    gemtext = re.sub(
-        r"(?:" + NEWLINE + r"){3}(?:" + NEWLINE + r")*", NEWLINE * 2, gemtext
-    )
-
     return gemtext
 
 
 # Main functions, for running as a script
 
 
 def __convert_file(file, args):
@@ -366,8 +359,8 @@
         if not os.path.isfile(file):
             print("File", file, "cannot be found.", file=sys.stderr)
             sys.exit(1)
         __convert_file(file, args)
 
 
 __all__ = ["GeminiRenderer", "md2gemini", "main", "NEWLINE", "__version__"]
-__version__ = "1.9.0"
+__version__ = "1.9.1"
```

### Comparing `md2gemini-1.9.0/md2gemini/renderers.py` & `md2gemini-1.9.1/md2gemini/renderers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 All the renderers that convert markdown to gemini.
 """
 
+import re
 import mistune
-import functools
 from .unitable import UniTable, ArraySizeError
 
 
 NEWLINE = "\r\n"  # For Windows support
 PARAGRAPH_DELIM = "\x02"  # The marker for paragraph start and end, for post processing
 LINK_DELIM = "\x03"
 LINEBREAK = "\x01"  # Represents a hard linebreak that should not be changed
 
+FENCE_EXPR = re.compile(r"^( *)```")
+
 
 class GeminiRenderer(
     mistune.HTMLRenderer
 ):  # Actually BaseRenderer should be used but this isn't available
 
     # NAME = "gemini"
 
@@ -304,19 +306,25 @@
 
         lines = (
             text.replace(PARAGRAPH_DELIM, "\n")
             .replace(LINEBREAK, "\n")
             .strip()
             .splitlines()
         )
+
         ret = ""
-        for line in lines:
-            ret += (
-                "> " + line.strip() + LINEBREAK
-            )  # Linebreak used to prevent removal later
+        for i, line in enumerate(lines):
+            line = line.strip()
+            link = line and line[0] == LINK_DELIM
+            ret += LINEBREAK if link else "> "
+            ret += line
+            if i < len(lines) - 1:
+                # Linebreak used to prevent removal later
+                ret += LINEBREAK
+
         return PARAGRAPH_DELIM + ret + PARAGRAPH_DELIM
 
     def block_html(self, html):
         if self.strip_html:
             return NEWLINE
         return self.block_code(html, "html")
 
@@ -325,17 +333,39 @@
 
     def list_item(self, text, level):
         # It is necessary to split the text on newline, since markdown
         # allows for list items to be split across multiple lines.
         # We need to strip whitespace from these items and add it ourselves,
         # since the text doesn't guarantee any particular formatting for
         # these items.
-        items = [item.strip() for item in text.splitlines()]
-        text = functools.reduce(lambda x, y: x + " " + y, items)
-        return text + NEWLINE
+        new_text = ""
+        last_offset = 0
+        in_fence = False
+        text = text.replace(PARAGRAPH_DELIM, PARAGRAPH_DELIM + "\r\n")
+        for item in text.splitlines():
+            was_in_fence = in_fence
+            m = FENCE_EXPR.match(item)
+            if m:
+                this_offset = len(m.groups()[0])
+                in_fence = (
+                    not in_fence if m and this_offset == last_offset else in_fence
+                )
+                if in_fence and not was_in_fence:
+                    last_offset = this_offset
+            if in_fence:
+                new_text += LINEBREAK + item
+            else:
+                if was_in_fence:
+                    new_text += LINEBREAK + item + LINEBREAK
+                else:
+                    if new_text:
+                        new_text += " " + item.lstrip()
+                    else:
+                        new_text = item
+        return new_text + NEWLINE
 
     def list(self, text, ordered, level, start=None):
         """Gemini only defines single-level unordered lists.
 
         This uses indenting to do sub-levels.
         Ordered list items just use 1. 2. etc, as plain text.
         """
@@ -372,15 +402,20 @@
             for item in items:
                 if item.startswith(self.indent):
                     # See the comment above for why this check is required.
                     ret_items.append(item)
                 else:
                     ret_items.append(self.indent * (level - 1) + "* " + item.strip())
 
-        return NEWLINE.join(ret_items) + NEWLINE * 2
+        return (
+            PARAGRAPH_DELIM
+            + LINEBREAK.join(ret_items)
+            + self._end_of_paragraph()
+            + PARAGRAPH_DELIM
+        )
 
     # Elements that rely on plugins:
 
     # Tables
     # Most of the funcs just return the text unchanged because the actual text processing
     # is done at the end, using the UniTable class.
```

### Comparing `md2gemini-1.9.0/md2gemini/unitable.py` & `md2gemini-1.9.1/md2gemini/unitable.py`

 * *Files identical despite different names*

### Comparing `md2gemini-1.9.0/md2gemini.egg-info/PKG-INFO` & `md2gemini-1.9.1/md2gemini.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: md2gemini
-Version: 1.9.0
+Version: 1.9.1
 Summary: Convert Markdown to the Gemini text format
 Home-page: https://github.com/makeworld-the-better-one/md2gemini
 Author: makeworld
 Author-email: makeworld@protonmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Markup
 Requires-Python: >=3.7
@@ -24,14 +22,18 @@
 
 Converter from Markdown to the [Gemini](https://gemini.circumlunar.space/) text format. It works as a Python module, or a command line application.
 
 One of its key features is that it can convert inline links into footnotes. It also supports tables, and will convert them into Unicode (or ASCII) tables.
 
 Anything else that it doesn't understand will remain the same as when you wrote it, like strikethrough for example.
 
+## Project Status
+
+md2gemini is now archived. It’s always been a pile of hacks, and now I’m not that invested in continuing it. See my [blog post](https://www.makeworld.space/2023/08/bye_gemini.html) for details.
+
 ## Link modes
 
 md2gemini has several link modes, because text/gemini doesn't support inline links. These modes can be set by passing different strings to the `-l` or `--links` flags on the command line, or the `links=` argument in Python.
 
 Here is some example markdown, to show what each link mode does:
 ```markdown
 This is a paragraph with an [inline](https://example.com) link.
@@ -230,9 +232,7 @@
     URL as parameter, and should return the new link.
 
     table_tag: "The default alt text for table blocks."
 
     checklist: whether to support GitHub-style checklist list items: [ ] and [x]
     """
 ```
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `md2gemini-1.9.0/md2gemini.egg-info/SOURCES.txt` & `md2gemini-1.9.1/md2gemini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `md2gemini-1.9.0/setup.py` & `md2gemini-1.9.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     version=__version__,
     author="makeworld",
     author_email="makeworld@protonmail.com",
     description="Convert Markdown to the Gemini text format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/makeworld-the-better-one/md2gemini",
-    packages=setuptools.find_packages(),
+    packages=["md2gemini"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
         "Topic :: Text Processing",
         "Topic :: Text Processing :: General",
         "Topic :: Text Processing :: Markup",
```

### Comparing `md2gemini-1.9.0/tests/test_frontmatter.py` & `md2gemini-1.9.1/tests/test_frontmatter.py`

 * *Files identical despite different names*

### Comparing `md2gemini-1.9.0/tests/test_list.py` & `md2gemini-1.9.1/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `md2gemini-1.9.0/tests/test_plain.py` & `md2gemini-1.9.1/tests/test_plain.py`

 * *Files identical despite different names*

### Comparing `md2gemini-1.9.0/tests/test_quote.py` & `md2gemini-1.9.1/tests/test_quote.py`

 * *Files identical despite different names*

### Comparing `md2gemini-1.9.0/tests/test_strip_html.py` & `md2gemini-1.9.1/tests/test_strip_html.py`

 * *Files identical despite different names*

### Comparing `md2gemini-1.9.0/tests/test_tags.py` & `md2gemini-1.9.1/tests/test_tags.py`

 * *Files identical despite different names*

