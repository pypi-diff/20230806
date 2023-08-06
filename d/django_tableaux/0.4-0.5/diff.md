# Comparing `tmp/django_tableaux-0.4.tar.gz` & `tmp/django_tableaux-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tableaux-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_tableaux-0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_tableaux-0.4.tar` & `django_tableaux-0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1809 2023-07-15 17:35:02.160341 django_tableaux-0.4/.gitignore
--rw-r--r--   0        0        0     1099 2023-07-15 17:10:11.497764 django_tableaux-0.4/LICENSE
--rw-r--r--   0        0        0     1177 2023-07-22 11:05:37.932487 django_tableaux-0.4/README.rst
--rw-r--r--   0        0        0     1170 2023-07-22 11:16:47.939966 django_tableaux-0.4/django_tableaux/__init__.py
--rw-r--r--   0        0        0      167 2023-07-15 11:12:22.980744 django_tableaux-0.4/django_tableaux/apps.py
--rw-r--r--   0        0        0      820 2023-07-15 11:12:22.980744 django_tableaux-0.4/django_tableaux/buttons.py
--rw-r--r--   0        0        0     2557 2023-07-15 11:12:22.981744 django_tableaux-0.4/django_tableaux/columns.py
--rw-r--r--   0        0        0     7871 2023-07-21 17:57:23.538305 django_tableaux-0.4/django_tableaux/static/django_tableaux/js/django_tableaux.js
--rw-r--r--   0        0        0      194 2023-07-15 11:12:22.982745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/_alert.html
--rw-r--r--   0        0        0      761 2023-07-22 07:33:55.960073 django_tableaux-0.4/django_tableaux/templates/django_tableaux/block_content.html
--rw-r--r--   0        0        0     1120 2023-07-22 07:20:37.370978 django_tableaux-0.4/django_tableaux/templates/django_tableaux/block_head.html
--rw-r--r--   0        0        0     3079 2023-07-22 07:37:36.360226 django_tableaux-0.4/django_tableaux/templates/django_tableaux/bootstrap4.html
--rw-r--r--   0        0        0     1103 2023-07-15 11:12:22.984745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/bootstrap5_base.html
--rw-r--r--   0        0        0       86 2023-07-15 11:12:22.984745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/button.html
--rw-r--r--   0        0        0      118 2023-07-15 11:12:22.984745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/cell_error.html
--rw-r--r--   0        0        0      512 2023-07-20 16:48:22.764631 django_tableaux-0.4/django_tableaux/templates/django_tableaux/cell_form.html
--rw-r--r--   0        0        0     1343 2023-07-21 07:21:05.700143 django_tableaux-0.4/django_tableaux/templates/django_tableaux/custom_bootstrap4.html
--rw-r--r--   0        0        0      331 2023-07-15 11:12:22.985745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/filter_settings.html
--rw-r--r--   0        0        0      890 2023-07-19 18:19:28.419384 django_tableaux-0.4/django_tableaux/templates/django_tableaux/filter_toolbar.html
--rw-r--r--   0        0        0     1348 2023-07-15 11:12:22.985745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/modal_base.html
--rw-r--r--   0        0        0      745 2023-07-15 11:12:22.986745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/modal_filter.html
--rw-r--r--   0        0        0      542 2023-07-15 11:12:22.986745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/modal_form.html
--rw-r--r--   0        0        0     1727 2023-07-15 11:12:22.986745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/paginator.html
--rw-r--r--   0        0        0     3041 2023-07-20 11:04:24.826254 django_tableaux-0.4/django_tableaux/templates/django_tableaux/render_rows.html
--rw-r--r--   0        0        0      105 2023-07-15 11:12:22.987744 django_tableaux-0.4/django_tableaux/templates/django_tableaux/render_table_data.html
--rw-r--r--   0        0        0      102 2023-07-15 11:12:22.987744 django_tableaux-0.4/django_tableaux/templates/django_tableaux/select_checkbox.html
--rw-r--r--   0        0        0     1427 2023-07-18 16:36:22.512989 django_tableaux-0.4/django_tableaux/templates/django_tableaux/tableaux.html
--rw-r--r--   0        0        0     1240 2023-07-20 12:33:33.463750 django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_actions.html
--rw-r--r--   0        0        0      181 2023-07-18 17:02:14.573795 django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_buttons.html
--rw-r--r--   0        0        0     1095 2023-07-15 11:12:22.988745 django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_columns.html
--rw-r--r--   0        0        0      607 2023-07-20 06:27:42.647795 django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_filter_field.html
--rw-r--r--   0        0        0      336 2023-07-19 16:09:11.116448 django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_filter_pills.html
--rw-r--r--   0        0        0      579 2023-07-15 11:12:22.989744 django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_rows.html
--rw-r--r--   0        0        0      469 2023-07-19 18:38:33.235037 django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/main.html
--rw-r--r--   0        0        0      317 2023-07-15 11:12:22.989744 django_tableaux-0.4/django_tableaux/templates/django_tableaux/width_request.html
--rw-r--r--   0        0        0        0 2023-07-15 11:12:22.989744 django_tableaux-0.4/django_tableaux/templatetags/__init__.py
--rw-r--r--   0        0        0     1161 2023-07-20 16:25:29.346745 django_tableaux-0.4/django_tableaux/templatetags/django_tableaux.py
--rw-r--r--   0        0        0     6529 2023-07-15 11:45:29.907566 django_tableaux-0.4/django_tableaux/tests.py
--rw-r--r--   0        0        0     3697 2023-07-17 18:44:03.199442 django_tableaux-0.4/django_tableaux/utils.py
--rw-r--r--   0        0        0    19866 2023-07-21 17:37:13.151709 django_tableaux-0.4/django_tableaux/views.py
--rw-r--r--   0        0        0      414 2023-07-15 17:10:11.497764 django_tableaux-0.4/pyproject.toml
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 django_tableaux-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1809 2023-07-15 17:35:02.160341 django_tableaux-0.5/.gitignore
+-rw-r--r--   0        0        0     1099 2023-07-15 17:10:11.497764 django_tableaux-0.5/LICENSE
+-rw-r--r--   0        0        0     1177 2023-07-22 11:05:37.932487 django_tableaux-0.5/README.rst
+-rw-r--r--   0        0        0     1170 2023-08-06 07:17:30.996420 django_tableaux-0.5/django_tableaux/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-15 11:12:22.980744 django_tableaux-0.5/django_tableaux/apps.py
+-rw-r--r--   0        0        0      820 2023-07-15 11:12:22.980744 django_tableaux-0.5/django_tableaux/buttons.py
+-rw-r--r--   0        0        0     2557 2023-07-15 11:12:22.981744 django_tableaux-0.5/django_tableaux/columns.py
+-rw-r--r--   0        0        0     8212 2023-07-22 13:26:17.974803 django_tableaux-0.5/django_tableaux/static/django_tableaux/js/django_tableaux.js
+-rw-r--r--   0        0        0      194 2023-07-15 11:12:22.982745 django_tableaux-0.5/django_tableaux/templates/django_tableaux/_alert.html
+-rw-r--r--   0        0        0      801 2023-07-22 15:04:16.261718 django_tableaux-0.5/django_tableaux/templates/django_tableaux/block_content.html
+-rw-r--r--   0        0        0     1120 2023-07-22 07:20:37.370978 django_tableaux-0.5/django_tableaux/templates/django_tableaux/block_head.html
+-rw-r--r--   0        0        0     3079 2023-07-22 07:37:36.360226 django_tableaux-0.5/django_tableaux/templates/django_tableaux/bootstrap4.html
+-rw-r--r--   0        0        0     1103 2023-07-15 11:12:22.984745 django_tableaux-0.5/django_tableaux/templates/django_tableaux/bootstrap5_base.html
+-rw-r--r--   0        0        0       86 2023-07-15 11:12:22.984745 django_tableaux-0.5/django_tableaux/templates/django_tableaux/button.html
+-rw-r--r--   0        0        0      118 2023-07-15 11:12:22.984745 django_tableaux-0.5/django_tableaux/templates/django_tableaux/cell_error.html
+-rw-r--r--   0        0        0      512 2023-07-20 16:48:22.764631 django_tableaux-0.5/django_tableaux/templates/django_tableaux/cell_form.html
+-rw-r--r--   0        0        0     1343 2023-07-21 07:21:05.700143 django_tableaux-0.5/django_tableaux/templates/django_tableaux/custom_bootstrap4.html
+-rw-r--r--   0        0        0      331 2023-07-15 11:12:22.985745 django_tableaux-0.5/django_tableaux/templates/django_tableaux/filter_settings.html
+-rw-r--r--   0        0        0      890 2023-07-19 18:19:28.419384 django_tableaux-0.5/django_tableaux/templates/django_tableaux/filter_toolbar.html
+-rw-r--r--   0        0        0     1303 2023-07-24 07:16:32.231168 django_tableaux-0.5/django_tableaux/templates/django_tableaux/modal_base.html
+-rw-r--r--   0        0        0      745 2023-07-15 11:12:22.986745 django_tableaux-0.5/django_tableaux/templates/django_tableaux/modal_filter.html
+-rw-r--r--   0        0        0      542 2023-07-15 11:12:22.986745 django_tableaux-0.5/django_tableaux/templates/django_tableaux/modal_form.html
+-rw-r--r--   0        0        0     1727 2023-07-15 11:12:22.986745 django_tableaux-0.5/django_tableaux/templates/django_tableaux/paginator.html
+-rw-r--r--   0        0        0     3041 2023-07-20 11:04:24.826254 django_tableaux-0.5/django_tableaux/templates/django_tableaux/render_rows.html
+-rw-r--r--   0        0        0      105 2023-07-15 11:12:22.987744 django_tableaux-0.5/django_tableaux/templates/django_tableaux/render_table_data.html
+-rw-r--r--   0        0        0      102 2023-07-15 11:12:22.987744 django_tableaux-0.5/django_tableaux/templates/django_tableaux/select_checkbox.html
+-rw-r--r--   0        0        0     1427 2023-07-18 16:36:22.512989 django_tableaux-0.5/django_tableaux/templates/django_tableaux/tableaux.html
+-rw-r--r--   0        0        0     1240 2023-07-20 12:33:33.463750 django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_actions.html
+-rw-r--r--   0        0        0      181 2023-07-18 17:02:14.573795 django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_buttons.html
+-rw-r--r--   0        0        0     1088 2023-08-06 07:17:30.991418 django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_columns.html
+-rw-r--r--   0        0        0      607 2023-07-20 06:27:42.647795 django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_filter_field.html
+-rw-r--r--   0        0        0      336 2023-07-19 16:09:11.116448 django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_filter_pills.html
+-rw-r--r--   0        0        0      572 2023-08-06 07:17:30.994420 django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_rows.html
+-rw-r--r--   0        0        0      528 2023-07-22 16:09:40.091704 django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/main.html
+-rw-r--r--   0        0        0      317 2023-07-15 11:12:22.989744 django_tableaux-0.5/django_tableaux/templates/django_tableaux/width_request.html
+-rw-r--r--   0        0        0        0 2023-07-15 11:12:22.989744 django_tableaux-0.5/django_tableaux/templatetags/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-20 16:25:29.346745 django_tableaux-0.5/django_tableaux/templatetags/django_tableaux.py
+-rw-r--r--   0        0        0     6529 2023-07-15 11:45:29.907566 django_tableaux-0.5/django_tableaux/tests.py
+-rw-r--r--   0        0        0     3841 2023-07-29 17:40:05.271279 django_tableaux-0.5/django_tableaux/utils.py
+-rw-r--r--   0        0        0    20154 2023-07-29 18:54:04.585254 django_tableaux-0.5/django_tableaux/views.py
+-rw-r--r--   0        0        0      414 2023-07-15 17:10:11.497764 django_tableaux-0.5/pyproject.toml
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 django_tableaux-0.5/PKG-INFO
```

### Comparing `django_tableaux-0.4/.gitignore` & `django_tableaux-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/LICENSE` & `django_tableaux-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/README.rst` & `django_tableaux-0.5/README.rst`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/__init__.py` & `django_tableaux-0.5/django_tableaux/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 * Edit specific fields directly inside the table
 * Easy integration with generic views for CRUD operations
 
 The project is still in beta but is fully usable.
 
 Full documentation to follow.
 """
-__version__ = "0.4"
+__version__ = "0.5"
```

### Comparing `django_tableaux-0.4/django_tableaux/buttons.py` & `django_tableaux-0.5/django_tableaux/buttons.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/columns.py` & `django_tableaux-0.5/django_tableaux/columns.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/static/django_tableaux/js/django_tableaux.js` & `django_tableaux-0.5/django_tableaux/static/django_tableaux/js/django_tableaux.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,146 +1,126 @@
 // Handle checkboxes in tables, and modal forms
 'use strict';
 let tablesPro = (function() {
-            let tb = {};
-            let lastChecked = null
-            let selAll = null
-            let selAllPage = null
-            tb.init = function() {
-                let url = new URL(window.location.href)
-                const w = url.searchParams.get("_width")
-                if (w !== null) {
-                    if (parseInt(w) !== window.outerWidth) {
-                        window.location.href = window.location.href.replace(`_width=${w}`, `_width=${window.outerWidth}`)
-                    }
-                }
-                selAll = document.getElementById('select_all')
-                selAllPage = document.getElementById('select_all_page')
-                if (selAllPage) {
-                    selAllPage.addEventListener("click", selectAllPage)
-                    selectAllPage()
-                }
-                if (selAll) {
-                    selAll.addEventListener("click", selectAll)
-                    selectAll()
-                }
-                Array.from(document.querySelectorAll(".select-checkbox")).forEach(e => e.addEventListener("click", chkBoxClick));
-                Array.from(document.querySelectorAll("td")).forEach(e => e.addEventListener("click", tdClick));
-                Array.from(document.querySelectorAll(".auto-submit")).forEach(e => e.addEventListener("change", function() {
-                    document.getElementById("id_filter_form").submit()
-                }));
-                Array.from(document.querySelectorAll(".filter-clear")).forEach(e => e.addEventListener("click", filterClear))
-                Array.from(document.querySelectorAll(".form-group.hx-get")).forEach(e => e.addEventListener("change", filterChanged))
-                document.body.addEventListener("trigger", function(evt) {
-                    window.htmx.ajax('GET', evt.detail.url, {
-                        source: '#table_data',
-                        'target': '#table_data'
-                    });
-                })
-                // When editing a cell inline enter key triggers blur
-                if (document.querySelector(".td_editing")) {
-                    this.addEventListener("keypress", loseFocus)
-                }
-                countChecked()
+        let tb = {};
+        let lastChecked = null
+        let selAll = null
+        let selAllPage = null
+        tb.init = function() {
+            let url = new URL(window.location.href)
+            const w = url.searchParams.get("_width")
+            if (w !== null) {
+                if (parseInt(w) !== window.outerWidth) {
+                    window.location.href = window.location.href.replace(`_width=${w}`, `_width=${window.outerWidth}`)
+                }
+            }
+            selAll = document.getElementById('select_all')
+            selAllPage = document.getElementById('select_all_page')
+            if (selAllPage) {
+                selAllPage.addEventListener("click", selectAllPage)
+                selectAllPage()
+            }
+            if (selAll) {
+                selAll.addEventListener("click", selectAll)
+                selectAll()
+            }
+            Array.from(document.querySelectorAll("table")).forEach(e => e.addEventListener("click", tableClick));
+            Array.from(document.querySelectorAll(".auto-submit")).forEach(e => e.addEventListener("change", function() {
+                document.getElementById("id_filter_form").submit()
+            }));
+            Array.from(document.querySelectorAll(".filter-clear")).forEach(e => e.addEventListener("click", filterClear))
+            Array.from(document.querySelectorAll(".form-group.hx-get")).forEach(e => e.addEventListener("change", filterChanged))
+            document.body.addEventListener("trigger", function(evt) {
+                window.htmx.ajax('GET', evt.detail.url, {
+                    source: '#table_data',
+                    'target': '#table_data'
+                });
+            })
+            // When editing a cell inline enter key triggers blur
+            if (document.querySelector(".td_editing")) {
+                this.addEventListener("keypress", loseFocus)
             }
+            countChecked()
+        }
 
-            function loseFocus(e) {
-                if (e.key == "Enter") {
-                    document.activeElement.blur();
-                }
+        function loseFocus(e) {
+            if (e.key == "Enter") {
+                document.activeElement.blur();
             }
+        }
 
-            function filterChanged() {
-                // filter within header changed
-                window.htmx.ajax('GET', '', {
-                    source: '#' + this.firstChild.getAttribute("for"),
-                    target: '#table_data'
-                });
-            }
+        function filterChanged() {
+            // filter within header changed
+            window.htmx.ajax('GET', '', {
+                source: '#' + this.firstChild.getAttribute("for"),
+                target: '#table_data'
+            });
+        }
 
-            function filterClear(e) {
-                let input = window.htmx.closest(e.target, ".input-group").firstChild
-                window.htmx.ajax('GET', '', {
-                    source: input,
-                    target: input
-                });
-            }
+        function filterClear(e) {
+            let input = window.htmx.closest(e.target, ".input-group").firstChild
+            window.htmx.ajax('GET', '', {
+                source: input,
+                target: input
+            });
+        }
 
-            function selectAllPage() {
-                // Click on 'Select all on page' highlights all rows
-                if (selAllPage) {
-                    let checked = selAllPage.checked
-                    if (selAll) {
-                        if (checked) {
-                            selAll.parentElement.style.display = 'block';
-                        } else {
-                            selAll.parentElement.style.display = 'none';
-                        }
+        function selectAllPage() {
+            // Click on 'Select all on page' highlights all rows
+            if (selAllPage) {
+                let checked = selAllPage.checked
+                if (selAll) {
+                    if (checked) {
+                        selAll.parentElement.style.display = 'block';
+                    } else {
+                        selAll.parentElement.style.display = 'none';
                     }
-                    Array.from(document.getElementsByClassName("select-checkbox")).forEach(function(box) {
-                        box.checked = checked
-                        //box.disabled = false;
-                        highlightRow(box)
-                    })
-                    countChecked()
-                    lastChecked = null
-                }
-            }
-
-            function selectAll() {
-                // Click on Select all highlights all rows and disables checkboxes
-                let checked = selAll.checked
-                if (checked) {
-                    document.getElementById('count').innerText = 'All';
-                    if (selAllPage) {
-                        selAllPage.disabled = true
-                    };
-                } else {
-                    if (selAllPage) {
-                        selAllPage.disabled = false
-                    };
-                    //sslAllPage.checked = false;
                 }
                 Array.from(document.getElementsByClassName("select-checkbox")).forEach(function(box) {
-                    box.disabled = checked;
+                    box.checked = checked
+                    //box.disabled = false;
+                    highlightRow(box)
                 })
-                countChecked();
-                lastChecked = null;
+                countChecked()
+                lastChecked = null
             }
+        }
 
-            function chkBoxClick(e) {
-                // Click on row's select checkbox - handle using shift to select multiple rows
+        function selectAll() {
+            // Click on Select all highlights all rows and disables checkboxes
+            let checked = selAll.checked
+            if (checked) {
+                document.getElementById('count').innerText = 'All';
                 if (selAllPage) {
-                    selAllPage.checked = false
-                }
-                let chkBox = e.target
-                highlightRow(chkBox)
-                if (!lastChecked) {
-                    lastChecked = chkBox
-                } else if (e.shiftKey) {
-                    let chkBoxes = Array.from(document.getElementsByClassName("select-checkbox"))
-                    let start = chkBoxes.indexOf(chkBox)
-                    let end = chkBoxes.indexOf(lastChecked)
-                    chkBoxes.slice(Math.min(start, end), Math.max(start, end) + 1).forEach(function(box) {
-                        box.checked = chkBox.checked;
-                    });
-                    lastChecked = chkBox;
-                } else {
-                    lastChecked = chkBox;
-                }
-                countChecked();
-            }
+                    selAllPage.disabled = true
+                };
+            } else {
+                if (selAllPage) {
+                    selAllPage.disabled = false
+                };
+                //sslAllPage.checked = false;
+            }
+            Array.from(document.getElementsByClassName("select-checkbox")).forEach(function(box) {
+                box.disabled = checked;
+            })
+            countChecked();
+            lastChecked = null;
+        }
 
-            function tdClick(e) {
+        function tableClick(e) {
+            // Handle any clicks within the table.
+            // This catches clicks on elements that are added dynamically e.g. after infinite scroll
+            if (e.target.tagName === 'TD') {
+                // Ignore clicks in td holding select checkbox to handle near misses of checkbox
+                if (e.target.innerHTML.search('select-checkbox') >= 0) {
+                    return
+                }
                 let editing = document.getElementsByClassName("td-editing");
                 if (editing.length > 0) {
-                    if (e.target === editing[0]) {
-                        return
-                    }
-                    // click on a cell when editing another causes Put
+                    // clicking on a cell when already editing causes a put
                     let el = editing[0].parentNode
                     window.htmx.ajax('PUT', "", {
                         source: "#" + el.id,
                         target: "#" + el.id,
                         values: window.htmx.closest(el, 'tr')
                     })
                 } else {
@@ -179,53 +159,73 @@
                         e.target.setAttribute("id", "td" + idSuffix);
                         window.htmx.ajax('GET', "", {
                             source: '#td' + idSuffix,
                             target: '#td' + idSuffix,
                         });
                     }
                 }
-            }
-
-            function highlightRow(box) {
-                let row = box.parentElement.parentElement;
-                let cls = (("selected" in row.dataset) ? row.dataset.selected : "table-active");
-                if (box.checked) {
-                    row.classList.add(cls)
+            } else if (e.target.name === 'select-checkbox') {
+                // Click on row's select checkbox - handle using shift to select multiple rows
+                if (selAllPage) {
+                    selAllPage.checked = false
+                }
+                let chkBox = e.target
+                highlightRow(chkBox)
+                if (!lastChecked) {
+                    lastChecked = chkBox
+                } else if (e.shiftKey) {
+                    let chkBoxes = checkBoxes()
+                    let start = chkBoxes.indexOf(chkBox)
+                    let end = chkBoxes.indexOf(lastChecked)
+                    chkBoxes.slice(Math.min(start, end), Math.max(start, end) + 1).forEach(function(box) {
+                        box.checked = chkBox.checked;
+                    });
+                    lastChecked = chkBox;
                 } else {
-                    row.classList.remove(cls)
+                    lastChecked = chkBox;
                 }
+                countChecked();
             }
+        }
 
-            // Count the number of checked rows and nake sure they are highlighted
-            function countChecked() {
-                if (selAll && selAll.checked) {
-                    return
-                }
-                let checked = Array.from(document.querySelectorAll(".select-checkbox:checked"));
-                let ids = []
-                checked.forEach(function(el) {
-                    let row = el.parentElement.parentElement
-                    row.classList.add((("selected" in row.dataset) ? row.dataset.selected : "table-active"))
-                    ids.push(el.value)
-                });
-                let hiddenInput = document.querySelector("input[name='selected_ids']")
-                if (hiddenInput) {
-                    hiddenInput.value = ids.toString();
-                }
-                let count = checked.length;
-                let countField = document.getElementById('count');
-                if (countField) {
-                    countField.innerText = count.toString();
-                }
-                let actionMenu = document.getElementById('selectActionMenu');
-                if (actionMenu) {
-                    actionMenu.disabled = (count === 0);
-                    actionMenu.enabled = (count > 0 || selAll.checked);
-                }
+        function highlightRow(box) {
+            let row = box.parentElement.parentElement;
+            let cls = (("selected" in row.dataset) ? row.dataset.selected : "table-active");
+            if (box.checked) {
+                row.classList.add(cls)
+            } else {
+                row.classList.remove(cls)
             }
-
-            return tb
         }
 
-    )
+        // Count the number of checked rows and nake sure they are highlighted
+        // update hidden input with associated ids
+        function countChecked() {
+            if (selAll && selAll.checked) {
+                return
+            }
+            let checked = Array.from(document.querySelectorAll(".select-checkbox:checked"));
+            let ids = []
+            checked.forEach(function(el) {
+                let row = el.parentElement.parentElement
+                row.classList.add((("selected" in row.dataset) ? row.dataset.selected : "table-active"))
+                ids.push(el.value)
+            });
+            let hiddenInput = document.querySelector("input[name='selected_ids']")
+            if (hiddenInput) {
+                hiddenInput.value = ids.toString();
+            }
+            let count = checked.length;
+            let countField = document.getElementById('count');
+            if (countField) {
+                countField.innerText = count.toString();
+            }
+            let actionMenu = document.getElementById('selectActionMenu');
+            if (actionMenu) {
+                actionMenu.disabled = (count === 0);
+                actionMenu.enabled = (count > 0 || selAll.checked);
+            }
+        }
+        return tb
+    })
     ();
 window.addEventListener("load", tablesPro.init)
```

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/block_content.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/block_content.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% load static django_tableaux %}
 <div id="block_content">
   {% if view.filterset_class and view.filter_style == 1 %}
     <div class="{{ css_toolbar }}">
       {% include "django_tableaux/filter_toolbar.html" %}
     </div>
   {% endif %}
-  {% if filters %}
-    <div class="d-flex">
+  {% if view.filter_pills and filters %}
+    <div class="{{ css_toolbar }} d-flex">
       {% include "django_tableaux/toolbar/_filter_pills.html" %}
     </div>
   {% endif %}
   {% if actions or buttons or table.column_states or view.filterset_class and view.filter_modal %}
     <div class="{{ css_toolbar }}">
       {% include "django_tableaux/toolbar/main.html" %}
     </div>
```

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/block_head.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/block_head.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/bootstrap4.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/bootstrap5_base.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/bootstrap5_base.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/cell_form.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/cell_form.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/custom_bootstrap4.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/custom_bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/filter_toolbar.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/filter_toolbar.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/modal_base.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/modal_base.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load bootstrap4 %}
 <div id="modal-backdrop" class="modal-backdrop fade show" style="display:block;"></div>
 <div id="modal" class="modal fade show" tabindex="-1" style="display:block;">
-  <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable {{ view.modal_size }}">
+  <div class="modal-dialog {{ view.modal_class }}">
     <div class="modal-content">
       {% block modal_content %}
         {% block modal_header %}
           <div class="modal-header ">
             <div class="modal-title">{% block modal_title %}<h4 class="my-0">{{ view.title }}</h4>{% endblock %}</div>
             <button type="button" class="close" name="close_modal" onclick="closeModal()" aria-label="Close"><span
                 aria-hidden="true">&times;</span></button>
```

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/modal_filter.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/modal_filter.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/modal_form.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/modal_form.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/paginator.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/paginator.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/render_rows.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/render_rows.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/tableaux.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/tableaux.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_actions.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_actions.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_columns.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_columns.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {# Code for toggle and margin is compatible with bootstrap4 and bootstrap5 #}
 {% if view.column_settings %}
 <div class="dropdown">
-  <button class="btn btn-sm btn-outline-secondary dropdown-toggle mr-1" type="button" id="dropdownColumnButton"
+  <button class="btn btn-outline-secondary dropdown-toggle mr-1" type="button" id="dropdownColumnButton"
           data-toggle="dropdown" data-bs-toggle="dropdown"
           aria-haspopup="true" aria-expanded="false">
     Columns
   </button>
   <div class="dropdown-menu" aria-labelledby="dropdownColumnButton" hx-target="#table_data">
     {% if default %}
       <a class="dropdown-item py-0" href="#" hx-get="" id="id_col_reset">Reset columns</a>
```

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_filter_field.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_filter_field.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/templates/django_tableaux/toolbar/_rows.html` & `django_tableaux-0.5/django_tableaux/templates/django_tableaux/toolbar/_rows.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% if view.row_settings %}
 <div class="dropdown">
-  <button class="btn btn-sm btn-outline-secondary dropdown-toggle mr-1" type="button" id="dropdownRowsButton"
+  <button class="btn btn-outline-secondary dropdown-toggle mr-1" type="button" id="dropdownRowsButton"
           data-toggle="dropdown" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
     {{ per_page }} rows
   </button>
   <div class="dropdown-menu" aria-labelledby="dropdownRowsButton"  hx-target="#table_data">
     {% for row in rows %}
     <div class="dropdown-item pl-2" name="{{ row }}" id="id_row_{{ row }}" hx-get="">{{ row }} rows</div>
     {% endfor %}
```

### Comparing `django_tableaux-0.4/django_tableaux/templatetags/django_tableaux.py` & `django_tableaux-0.5/django_tableaux/templatetags/django_tableaux.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/tests.py` & `django_tableaux-0.5/django_tableaux/tests.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.4/django_tableaux/utils.py` & `django_tableaux-0.5/django_tableaux/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,18 @@
     table.columns_default = table.sequence
     table.columns_editable = []
     if table.Meta:
         col_dict = {}
         if hasattr(table.Meta, "editable"):
             table.columns_editable = table.Meta.editable
         if hasattr(table.Meta, "columns"):
-            col_dict = table.Meta.columns
+            if type(table.Meta.columns) == dict:
+                col_dict = table.Meta.columns
+            else:
+                raise ValueError("Meta.columns must be a dictionary")
         if hasattr(table.Meta, "responsive"):
             table.responsive = True
             key = 0
             for breakpoint in table.Meta.responsive.keys():
                 if width >= breakpoint:
                     key = breakpoint
             col_dict = table.Meta.responsive.get(key, {})
```

### Comparing `django_tableaux-0.4/django_tableaux/views.py` & `django_tableaux-0.5/django_tableaux/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 logger = logging.getLogger(__name__)
 
 
 class ConfigurationError(Exception):
     pass
 
 
-class DjangoTableauxView(SingleTableMixin, FilterView):
+class TableauxView(SingleTableMixin, FilterView):
     class FilterStyle(IntEnum):
         NONE = 0
         TOOLBAR = 1
         MODAL = 2
         HEADER = 3
 
     class ClickAction(IntEnum):
@@ -60,14 +60,15 @@
 
     table_pagination = {"per_page": 10}
     infinite_scroll = False
     infinite_load = False
     #
     context_filter_name = "filter"
     filter_style = FilterStyle.TOOLBAR
+    filter_pills = False
     filter_button = False  # only relevant for TOOLBAR style
     #
     column_settings = False
     row_settings = False
 
     click_action = ClickAction.NONE
     click_url_name = ""
@@ -261,23 +262,24 @@
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         self.table = context["table"]
         self.preprocess_table(self.table, context["filter"])
         context.update(
             title=self.title,
             filter_button=self.filter_button,
+            filter_pills=self.filter_pills,
+            filters=[],
             buttons=self.get_buttons(),
             actions=self.get_actions(),
             rows=self.rows_list(),
             per_page=self.request.GET.get(
                 "per_page", self.table_pagination.get("per_page", 25)
             ),
             breakpoints=breakpoints(self.table),
             width=self.width,
-            filters=[],
         )
         if "_width" in self.request.GET:
             context["breakpoints"] = None
 
         for key, value in self.request.GET.items():
             if key not in self.ALLOWED_PARAMS and value:
                 context["filters"].append((key, value))
@@ -359,15 +361,14 @@
         bits = request.htmx.current_url.split("?")
         if len(bits) == 2:
             return QueryDict(bits[1]).copy()
         return QueryDict().copy()
 
     def handle_action(self, request, action):
         """
-        The action is also in the request.POST dictionary.
         self.selected_objects is a queryset that contains the objects to be processed.
         self.selected_ids is a list of model ids that were selected, empty for 'All rows'
         Possible return values:
         - None: (default) - reloads the last path
         - HttpResponse to be returned
         """
         return None
@@ -439,14 +440,19 @@
         # set visible columns according to saved setting
         table.columns_visible = load_columns(self.request, width=self.width)
         if not table.columns_visible:
             table.columns_visible = table.columns_default
             save_columns(
                 self.request, width=self.width, column_list=table.columns_visible
             )
+        else:
+            # ensure all fixed columns are in the visible list in case table definitions have been changed
+            for entry in table.columns_fixed:
+                if entry not in table.columns_visible:
+                    table.columns_visible.append(entry)
 
         set_column_states(table)
 
         if table.filter:
             table.filter.style = self.filter_style
             # If filter is in header, build list of filters in same sequence as columns
             if self.filter_style == self.FilterStyle.HEADER:
```

### Comparing `django_tableaux-0.4/PKG-INFO` & `django_tableaux-0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tableaux
-Version: 0.4
+Version: 0.5
 Summary: Django tables with Advanced User eXperience
 Author-email: Ian Stewart <is@iskt.co.uk>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/ianastewart/django_tableaux/
 
 ===============
```

