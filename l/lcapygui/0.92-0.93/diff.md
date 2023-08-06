# Comparing `tmp/lcapygui-0.92.tar.gz` & `tmp/lcapygui-0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcapygui-0.92.tar", last modified: Tue Jul 18 02:35:34 2023, max compression
+gzip compressed data, was "lcapygui-0.93.tar", last modified: Sun Aug  6 20:22:05 2023, max compression
```

## Comparing `lcapygui-0.92.tar` & `lcapygui-0.93.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/
--rw-rw-r--   0 mph       (1000) mph       (1000)      934 2023-07-18 02:35:34.188850 lcapygui-0.92/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)      361 2023-07-18 02:35:33.000000 lcapygui-0.92/README.md
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.184850 lcapygui-0.92/lcapygui/
--rw-rw-r--   0 mph       (1000) mph       (1000)      567 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      443 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/annotation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      246 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/annotations.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/lcapygui/components/
--rw-rw-r--   0 mph       (1000) mph       (1000)       99 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       89 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/admittance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      620 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/annotation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      341 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/bipole.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      641 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/bjt.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      315 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/capacitor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/cccs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/ccvs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    13524 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/component.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3762 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/connection.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      177 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/controlledcomponent.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      107 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/cpe.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3368 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/cpt_maker.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/current_source.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      510 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/diode.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      136 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/ferritebead.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/impedance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      283 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/inductor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      215 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/jfet.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1610 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/mosfet.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3962 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/opamp.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      188 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/opencircuit.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      132 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/port.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      216 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/resistor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4522 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/sketch.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3342 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/svgparse.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1401 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/transistor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/vccs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/vcvs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/voltage_source.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      365 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/wire.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1237 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/node.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1842 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/nodes.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/lcapygui/scripts/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/scripts/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1878 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/scripts/lcapytk.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/lcapygui/ui/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1825 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/preferences.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/lcapygui/ui/tk/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1220 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/approximate_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2939 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/cpt_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4980 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/cpt_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1800 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/drawing.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      768 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/edit_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2693 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/edit_values_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1390 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/equations_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      716 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/expr_attributes_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      425 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/expr_calc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    13041 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/expr_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      187 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/exprimage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1760 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/help_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1206 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/inspect_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2373 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/labelentries.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      846 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/lateximage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    23079 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/lcapytk.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9431 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/lcapytkm.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1174 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/limit_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2342 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/menu.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      251 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/message_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1631 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/multiplot_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      907 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/node_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      788 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/plot_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2323 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/plot_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4324 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/preferences_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1679 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/python_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4078 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/sketcher.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2490 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/state_space_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1189 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/subs_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      892 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/transfer_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2011 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/transfer_function_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1448 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/twoport_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3864 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/twoport_select_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      435 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/working_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    20476 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/uimodelbase.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    17327 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/uimodelmph.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.184850 lcapygui-0.92/lcapygui.egg-info/
--rw-rw-r--   0 mph       (1000) mph       (1000)      934 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)     2628 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/SOURCES.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        1 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/dependency_links.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)       60 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/entry_points.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      150 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/requires.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        9 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/top_level.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      103 2023-07-18 02:35:33.000000 lcapygui-0.92/pyproject.toml
--rw-rw-r--   0 mph       (1000) mph       (1000)      287 2023-07-18 02:35:34.188850 lcapygui-0.92/setup.cfg
--rw-rw-r--   0 mph       (1000) mph       (1000)     1349 2023-07-18 02:35:33.000000 lcapygui-0.92/setup.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.699840 lcapygui-0.93/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      934 2023-08-06 20:22:05.699840 lcapygui-0.93/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)      361 2023-08-06 20:22:05.000000 lcapygui-0.93/README.md
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.691840 lcapygui-0.93/lcapygui/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      567 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      443 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/annotation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      246 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/annotations.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.695840 lcapygui-0.93/lcapygui/components/
+-rw-rw-r--   0 mph       (1000) mph       (1000)       99 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       89 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/admittance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      620 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/annotation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      341 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/bipole.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      641 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/bjt.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      315 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/capacitor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/cccs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/ccvs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    14491 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/component.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3814 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/connection.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      177 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/controlledcomponent.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      107 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/cpe.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2852 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/cpt_maker.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/current_source.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      510 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/diode.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4298 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/fdopamp.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      136 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/ferritebead.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/impedance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      283 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/inductor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      215 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/jfet.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1610 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/mosfet.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3977 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/opamp.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      177 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/opencircuit.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      132 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/port.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      216 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/resistor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5074 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/sketch.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3342 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/svgparse.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2963 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/transformer.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1401 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/transistor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/vccs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/vcvs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/voltage_source.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      391 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/components/wire.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1237 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/node.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1842 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/nodes.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.695840 lcapygui-0.93/lcapygui/scripts/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/scripts/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1878 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/scripts/lcapytk.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      761 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/sketch_library.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.695840 lcapygui-0.93/lcapygui/ui/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2335 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/preferences.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.699840 lcapygui-0.93/lcapygui/ui/tk/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1240 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/approximate_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2939 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/cpt_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5311 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/cpt_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1800 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/drawing.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      768 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/edit_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2693 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/edit_values_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1390 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/equations_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      716 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/expr_attributes_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      425 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/expr_calc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    13041 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/expr_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      187 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/exprimage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1920 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/help_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      614 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/image_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1206 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/inspect_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2373 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/labelentries.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      846 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/lateximage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    24327 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/lcapytk.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9431 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/lcapytkm.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1174 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/limit_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2461 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/menu.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      251 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/message_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1631 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/multiplot_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      907 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/node_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      788 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/plot_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2323 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/plot_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4495 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/preferences_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1679 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/python_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4000 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/sketcher.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2490 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/state_space_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1209 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/subs_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      892 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/transfer_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2011 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/transfer_function_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1448 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/twoport_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3864 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/twoport_select_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      435 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/tk/working_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    21586 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/uimodelbase.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    18281 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui/ui/uimodelmph.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-08-06 20:22:05.691840 lcapygui-0.93/lcapygui.egg-info/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      934 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui.egg-info/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2752 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui.egg-info/SOURCES.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        1 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui.egg-info/dependency_links.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)       60 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui.egg-info/entry_points.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      150 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui.egg-info/requires.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        9 2023-08-06 20:22:05.000000 lcapygui-0.93/lcapygui.egg-info/top_level.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      103 2023-08-06 20:22:05.000000 lcapygui-0.93/pyproject.toml
+-rw-rw-r--   0 mph       (1000) mph       (1000)      287 2023-08-06 20:22:05.699840 lcapygui-0.93/setup.cfg
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1353 2023-08-06 20:22:05.000000 lcapygui-0.93/setup.py
```

### Comparing `lcapygui-0.92/PKG-INFO` & `lcapygui-0.93/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapygui
-Version: 0.92
+Version: 0.93
 Summary: A GUI for lcapy
 Home-page: https://github.com/mph-/lcapy-gui
 Author: Michael Hayes, Jordan Hay
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mph-/lcapy-gui
 Description: # lcapy-gui
```

### Comparing `lcapygui-0.92/lcapygui/__init__.py` & `lcapygui-0.93/lcapygui/__init__.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/components/annotation.py` & `lcapygui-0.93/lcapygui/components/annotation.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/components/bjt.py` & `lcapygui-0.93/lcapygui/components/bjt.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/components/component.py` & `lcapygui-0.93/lcapygui/components/component.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     current_keys = ('i', 'i_', 'i^', 'i_>',  'i_<', 'i^>', 'i^<',
                     'i>_', 'i<_', 'i>^', 'i<^', 'i>', 'i<', 'ir')
     flow_keys = ('f', 'f_', 'f^', 'f_>',  'f_<', 'f^>', 'f^<',
                  'f>_', 'f<_', 'f>^', 'f<^', 'f>', 'f<')
     label_keys = ('l', 'l_', 'l^')
     annotation_keys = ('a', 'a_', 'a^')
 
-    # These are not passed to the sktecher.
+    # These are not passed to the sketcher.
     ignore_keys = ('left', 'right', 'up', 'down', 'size', 'rotate',
                    'pinnodes', 'pinnames', 'pins', 'pinlabels',
                    'mirrorinputs', 'free', 'ignore', 'nosim', 'arrow',
                    'startarrow', 'endarrow', 'bus', 'anchor', 'fixed')
 
     all_keys = voltage_keys + current_keys + flow_keys + \
         label_keys + annotation_keys + ignore_keys
@@ -191,65 +191,76 @@
         return self.nodes
 
     @property
     def drawn_nodes(self):
 
         return self.nodes
 
-    def draw(self, editor, sketcher, **kwargs):
+    def _sketch_lookup(self, model):
+
+        ui = model.ui
+        style = model.preferences.style
+
+        sketch = ui.sketchlib.lookup(self.sketch_key, style)
+        return sketch
+
+    def draw(self, model, **kwargs):
         """
         Handles drawing specific features of components.
         """
 
+        sketch = self._sketch_lookup(model)
+
         # Handle ports where nothing is drawn.
-        if self.sketch is None:
+        if sketch is None:
             return
 
         x1, y1 = self.node1.x, self.node1.y
         x2, y2 = self.node2.x, self.node2.y
         dx = x2 - x1
         dy = y2 - y1
 
         r = self.length
         if r == 0:
-            editor.ui.show_warning_dialog(
+            model.ui.show_warning_dialog(
                 'Ignoring zero size component ' + self.name)
             return
 
         angle = self.angle
 
         # Width in cm
-        w = self.sketch.width / 72 * 2.54
+        w = sketch.width / 72 * 2.54
 
         p1 = array((x1, y1))
         if r != 0:
             dw = array((dx, dy)) / r * (r - w) / 2
             p1p = p1 + dw
         else:
             # For zero length wires
             p1p = p1
 
-        kwargs = self.make_kwargs(editor, **kwargs)
+        kwargs = self.make_kwargs(model, **kwargs)
 
         if 'invisible' in kwargs or 'nodraw' in kwargs or 'ignore' in kwargs:
             return
 
-        sketcher.sketch(self.sketch, offset=p1p, angle=angle,
-                        snap=True, **kwargs)
+        sketch.draw(model, offset=p1p, angle=angle,
+                    snap=True, **kwargs)
 
         # Add stretchable wires
         if self.can_stretch:
 
             p2 = array((x2, y2))
             p2p = p2 - dw
 
             # TODO: generalize
             kwargs.pop('mirror', False)
             kwargs.pop('invert', False)
 
+            sketcher = model.ui.sketcher
             sketcher.stroke_line(*p1, *p1p, **kwargs)
             sketcher.stroke_line(*p2p, *p2, **kwargs)
 
             # For transistors.
             if len(self.nodes) == 3:
 
                 x3, y3 = self.nodes[1].x, self.nodes[1].y
@@ -259,32 +270,52 @@
                 dx = mx - x3
                 dy = my - y3
                 r = sqrt(dx**2 + dy**2)
 
                 p3 = array((x3, y3))
 
                 # Height in cm
-                h = self.sketch.height / 72 * 2.54
+                h = sketch.height / 72 * 2.54
                 dh = array((dx, dy)) / r * (r - h)
                 p3p = p3 + dh
                 sketcher.stroke_line(*p3, *p3p, **kwargs)
 
         # TODO, add label, voltage_label, current_label, flow_label
 
-    def make_kwargs(self, editor, **kwargs):
+    def _line_width_to_lw(self, model, line_width):
+        """Return line width as a float for use with matplotlib."""
+
+        # TODO, handle other units?
+        if line_width.endswith('pt'):
+            line_width = float(line_width[0:-2])
+        elif line_width.endswith('mm'):
+            line_width = float(line_width[0:-2]) * 72 / 25.4
+        else:
+            model.ui.show_warning_dialog('Assuming points for line width')
+            line_width = float(line_width)
+
+        return line_width * model.preferences.line_width_scale
+
+    def make_kwargs(self, model, **kwargs):
 
         opts = Opts(self.attrs)
 
-        kwargs['lw'] = kwargs.pop('lw', editor.preferences.lw)
+        line_width = model.preferences.line_width
+        lw = self._line_width_to_lw(model, line_width)
+
+        kwargs['lw'] = kwargs.pop('lw', lw)
 
         for k, v in opts.items():
             if k in ('bodydiode', ):
                 continue
             if v == '':
                 v = True
+            if k == 'line width':
+                k = 'lw'
+                v = self._line_width_to_lw(model, v)
             kwargs[k] = v
 
         if kwargs.pop('thick', False):
             kwargs['lw'] = kwargs['lw'] * 2
 
         if self.color != '':
             kwargs['color'] = self.color
@@ -302,22 +333,22 @@
             kwargs['linestyle'] = ':'
 
         return kwargs
 
     @property
     def length(self) -> float:
         """
-        Computes the length of the component.
+        Returns the length of the component.
         """
         return (self.node2.pos - self.node1.pos).norm()
 
     @property
     def midpoint(self):
         """
-        Computes the midpoint of the component.
+        Returns the midpoint of the component.
         """
 
         return (self.node1.pos + self.node2.pos) * 0.5
 
     @property
     def vertical(self) -> bool:
         """
```

### Comparing `lcapygui-0.92/lcapygui/components/connection.py` & `lcapygui-0.93/lcapygui/components/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,39 +11,42 @@
 
     kinds = {'-0V': '0V',
              '-ground': 'Ground', '-sground': 'Signal ground',
              '-rground': 'Rail ground', '-cground': 'Chassis ground',
              '-vcc': 'VCC', '-vdd': 'VDD', '-vee': 'VEE', '-vss': 'VSS',
              '-input': 'Input', '-output': 'Output', '-bidir': 'Bidirectional'}
 
-    def draw(self, editor, sketcher, **kwargs):
+    def draw(self, model, **kwargs):
+
+        sketch = self._sketch_lookup(model)
 
         x1, y1 = self.node1.x, self.node1.y
         x2, y2 = self.node2.x, self.node2.y
 
-        kwargs = self.make_kwargs(editor, **kwargs)
+        kwargs = self.make_kwargs(model, **kwargs)
 
         if self.symbol_kind in ('vcc', 'vdd'):
-            x1, y1, angle = self.split_node_pos(x2, y2, editor.STEP, True)
+            x1, y1, angle = self.split_node_pos(x2, y2, model.STEP, True)
             offset = x1, y1
             angle = angle + 90
         elif self.symbol_kind in ('vee', 'vss'):
-            x2, y2, angle = self.split_node_pos(x1, y1, editor.STEP)
+            x2, y2, angle = self.split_node_pos(x1, y1, model.STEP)
             offset = x2, y2
             angle = angle + 90
         elif self.symbol_kind in ('input', ):
-            x2, y2, angle = self.split_node_pos(x1, y1, editor.STEP)
+            x2, y2, angle = self.split_node_pos(x1, y1, model.STEP)
             offset = x2, y2
         else:
-            x2, y2, angle = self.split_node_pos(x1, y1, editor.STEP)
+            x2, y2, angle = self.split_node_pos(x1, y1, model.STEP)
             offset = x2, y2
 
-        sketcher.sketch(self.sketch, offset=offset,
-                        angle=angle, snap=False, **kwargs)
+        sketch.draw(model, offset=offset,
+                    angle=angle, snap=False, **kwargs)
 
+        sketcher = model.ui.sketcher
         sketcher.stroke_line(x1, y1, x2, y2, **kwargs)
 
     def split_node_pos(self, x, y, step=1, flip=False):
 
         def get_value(direction):
 
             val = self.opts[direction]
```

### Comparing `lcapygui-0.92/lcapygui/components/mosfet.py` & `lcapygui-0.93/lcapygui/components/mosfet.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/components/opamp.py` & `lcapygui-0.93/lcapygui/components/opamp.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,34 +85,36 @@
         diff = (pos - self.nodes[0].pos) * 0.5
         return diff.norm()
 
     def attr_dir_string(self, x1, y1, x2, y2, step=1):
 
         # TODO: Handle rotation
         dy = abs(y2 - y1)
-        size = dy * 5 / 4
+        size = dy / 2
 
         attr = 'right=%s' % size
         return attr
 
-    def draw(self, editor, sketcher, **kwargs):
+    def draw(self, model, **kwargs):
+
+        sketch = self._sketch_lookup(model)
 
         x1, y1 = self.nodes[2].pos.x, self.nodes[2].pos.y
         x2, y2 = self.nodes[3].pos.x, self.nodes[3].pos.y
 
         xc = (x1 + x2) / 2
         yc = (y1 + y2) / 2
 
         dy = abs(self.nodes[3].y - self.nodes[2].y)
         size = dy * 5 / 4
 
-        kwargs = self.make_kwargs(editor, **kwargs)
+        kwargs = self.make_kwargs(model, **kwargs)
 
-        sketcher.sketch(self.sketch, offset=(xc, yc), angle=0, scale=size / 2.5,
-                        **kwargs)
+        sketch.draw(model, offset=(xc, yc), angle=0, scale=size / 2.5,
+                    **kwargs)
 
     def netitem_nodes(self, node_names):
 
         parts = []
         for node_name in node_names[0:2]:
             parts.append(node_name)
         parts.append('opamp')
```

### Comparing `lcapygui-0.92/lcapygui/components/sketch.py` & `lcapygui-0.93/lcapygui/components/sketch.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,22 +38,26 @@
 
     @property
     def color(self):
 
         return self.kwargs.get('color', 'black')
 
     @classmethod
-    def load(cls, sketch_key):
+    def load(cls, sketch_key, style='american', complain=True):
 
         from lcapygui import __datadir__
 
-        dirname = __datadir__ / 'svg'
+        dirname = __datadir__ / 'svg' / style
         svg_filename = dirname / (sketch_key + '.svg')
 
         if not svg_filename.exists():
+
+            if complain:
+                raise FileNotFoundError('Could not find data file %s for %s' %
+                                        (svg_filename, sketch_key))
             return None
 
         svg = SVGParse(str(svg_filename))
 
         sketch_paths = []
         for svga_path in svg.paths:
             sketch_path = SketchPath(
@@ -61,36 +65,38 @@
             sketch_path = sketch_path.transform(Affine2D(svga_path.transform))
             sketch_paths.append(sketch_path)
 
         sketch = cls(sketch_paths, svg.width, svg.height).align(sketch_key)
         return sketch
 
     @classmethod
-    def create(cls, sketch_key, sketch_net):
+    def create(cls, sketch_key, sketch_net, style='american'):
 
-        dirname = join('lcapygui', 'data', 'svg')
+        dirname = join('lcapygui', 'data', 'svg', style)
         svg_filename = join(dirname, sketch_key + '.svg')
 
         a = Circuit()
 
         net = sketch_net
         if net is None:
             return None
         if ';' not in net:
             net += '; right'
 
         a.add(net)
 
         a.draw(str(svg_filename), label_values=False, label_ids=False,
-               label_nodes=False, draw_nodes=False)
+               label_nodes=False, draw_nodes=False, style=style)
 
     def offsets1(self, sketch_key):
 
-        if sketch_key == 'opamp':
+        if sketch_key in ('opamp', 'fdopamp'):
             return 0, self.height / 2
+        elif sketch_key.startswith('TF'):
+            return self.width / 2 - 4.2, self.height / 2
 
         # TODO, use sketch_key to help find offset.
 
         xoffset = None
         yoffset = None
 
         # Look for pair of horizontal wires
@@ -138,20 +144,26 @@
 
     def offsets(self, sketch_key):
 
         xoffset, yoffset = self.offsets1(sketch_key)
         return xoffset, yoffset
 
     def align(self, sketch_key):
-        """Remove yoffset from component."""
+        """Remove xoffset, yoffset from component."""
 
         xoffset, yoffset = self.offsets(sketch_key)
 
         if xoffset is None:
             return self
 
         paths = []
         for path in self.paths:
             paths.append(path.transform(
                 Affine2D().translate(-xoffset, -yoffset)))
 
         return self.__class__(paths, self.width, self.height, **self.kwargs)
+
+    def draw(self, model, offset=(0, 0), scale=1, angle=0, **kwargs):
+
+        sketcher = model.ui.sketcher
+
+        return sketcher.sketch(self, offset, scale, angle, **kwargs)
```

### Comparing `lcapygui-0.92/lcapygui/components/svgparse.py` & `lcapygui-0.93/lcapygui/components/svgparse.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/components/transistor.py` & `lcapygui-0.93/lcapygui/components/transistor.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/node.py` & `lcapygui-0.93/lcapygui/node.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/nodes.py` & `lcapygui-0.93/lcapygui/nodes.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/scripts/lcapytk.py` & `lcapygui-0.93/lcapygui/scripts/lcapytk.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/preferences.py` & `lcapygui-0.93/lcapygui/ui/tk/drawing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,76 @@
-from pathlib import Path
-import json
+from numpy import arange
 
 
-# Perhaps make a dict?
-class Preferences:
+class Drawing():
 
-    def __init__(self):
+    def __init__(self, ui, fig, model, debug=0):
 
-        self.version = 1
-        self.label_nodes = 'none'
-        self.draw_nodes = 'connections'
-        self.label_cpts = 'name'
-        self.style = 'american'
-        self.node_size = 0.1
-        self.node_color = 'black'
-        self.grid = 'on'
-        self.lw = 1.2
-        self.show_units = 'false'
-        self.xsize = 36
-        self.ysize = 22
-        self.snap_grid = 'true'
-        self.voltage_dir = 'RP'
+        self.ui = ui
+        self.fig = fig
+        self.debug = debug
+        self.xsize = model.preferences.xsize
+        self.ysize = model.preferences.ysize
 
-        self.load()
+        self.ax = self.fig.add_subplot(111)
 
-    @property
-    def _dirname(self):
+        self.draw_grid('on')
+        self.set_default_view()
 
-        return Path('~/.lcapy/').expanduser()
+    def draw_grid(self, grid):
 
-    @property
-    def _filename(self):
+        if self.debug:
+            print('draw grid')
 
-        return self._dirname / 'preferences.json'
+        # Enlarge grid by factor of 2 in each direction.
+        # Only xsize by ysize is visible.
+        xticks = arange(self.xsize * 2)
+        yticks = arange(self.ysize * 2)
 
-    def load(self):
+        self.ax.axis('equal')
+        self.ax.set_xticks(xticks)
+        self.ax.set_yticks(yticks)
+        self.ax.set_xticklabels([])
+        self.ax.set_yticklabels([])
+        if grid == 'on':
+            self.ax.grid(color='lightblue')
 
-        dirname = self._dirname
-        if not dirname.exists():
-            return
+        self.ax.tick_params(which='both', left=False, bottom=False,
+                            top=False, labelbottom=False)
 
-        s = self._filename.read_text()
-        d = json.loads(s)
-        for k, v in d.items():
-            setattr(self, k, v)
+        self.ax.set_axisbelow(True)
 
-    def save(self):
+    def savefig(self, filename):
 
-        dirname = self._dirname
-        if not dirname.exists():
-            dirname.mkdir()
-        s = json.dumps(self, default=lambda o: o.__dict__,
-                       sort_keys=True, indent=4)
+        self.fig.savefig(filename, bbox_inches='tight', pad_inches=0)
 
-        self._filename.write_text(s)
+    def set_view(self, xmin, ymin, xmax, ymax):
 
-    def schematic_preferences(self):
+        if self.debug:
+            print('view', xmin, ymin, xmax, ymax)
 
-        opts = ('draw_nodes', 'label_nodes', 'style', 'voltage_dir')
+        self.ax.set_xlim(xmin, xmax)
+        self.ax.set_ylim(ymin, ymax)
 
-        foo = []
-        for opt in opts:
-            foo.append(opt + '=' + getattr(self, opt))
-        s = ', '.join(foo)
+    def set_default_view(self):
 
-        if self.label_cpts == 'name':
-            s += ', label_ids=true'
-            s += ', label_values=false'
-        elif self.label_cpts == 'value':
-            s += ', label_ids=false'
-            s += ', label_values=true'
-        elif self.label_cpts == 'value+name':
-            s += ', label_ids=true'
-            s += ', label_values=true'
+        self.set_view(0, 0, self.xsize, self.ysize)
 
-        return s
+    def clear(self, grid='on'):
+
+        if self.debug:
+            print('clear')
+
+        xmin, xmax = self.ax.get_xlim()
+        ymin, ymax = self.ax.get_ylim()
+
+        self.ax.clear()
+
+        self.draw_grid(grid)
+
+        self.set_view(xmin, ymin, xmax, ymax)
+
+    def refresh(self):
+
+        if self.debug:
+            print('refresh')
+        self.fig.canvas.draw()
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/approximate_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/approximate_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.window.title(title)
 
         entries = []
 
         self.symbols = []
         for key in expr.symbols:
             # Ignore domain variable
-            if key != expr.var.name:
+            if expr.var is None or key != expr.var.name:
                 entries.append(LabelEntry(key, key, 0.0))
                 self.symbols.append(key)
 
         self.labelentries = LabelEntries(self.window, ui, entries)
 
         button = Button(self.window, text="Approximate",
                         command=self.on_update)
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/cpt_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/cpt_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/cpt_properties_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/cpt_properties_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from tkinter import Tk, Button
+from tkinter import Toplevel, Button
 from .labelentries import LabelEntry, LabelEntries
 
 
 class CptPropertiesDialog:
 
     def __init__(self, ui, cpt, update=None, title=''):
 
         self.cpt = cpt
         self.gcpt = cpt.gcpt
         self.update = update
         self.ui = ui
 
-        self.window = Tk()
+        self.window = Toplevel()
         self.window.title(title)
 
         entries = []
         if self.gcpt.kinds != {}:
             kind_name = self.gcpt.kinds[self.gcpt.kind]
             entries.append(LabelEntry(
                 'kind', 'Kind', kind_name, list(self.gcpt.kinds.values()),
@@ -58,14 +58,28 @@
             entries.append(LabelEntry(k, v, getattr(self.gcpt, k),
                                       command=self.on_update))
 
         self.labelentries = LabelEntries(self.window, ui, entries)
 
         button = Button(self.window, text="OK", command=self.on_ok)
         button.grid(row=self.labelentries.row)
+        self.window.focus()
+
+        self.window.protocol('WM_DELETE_WINDOW', self.on_close)
+
+    def focus(self):
+
+        # Put window on top
+        self.window.attributes('-topmost', True)
+        self.window.focus()
+
+    def on_close(self):
+
+        self.ui.dialogs.pop(self.cpt.name)
+        self.window.destroy()
 
     def on_update(self, arg=None):
 
         if self.gcpt.kinds != {}:
             kind = self.gcpt.inv_kinds[self.labelentries.get('kind')]
             if self.gcpt.kind != kind:
                 self.gcpt.kind = kind
@@ -135,9 +149,8 @@
 
         if self.update:
             self.update(self.cpt)
 
     def on_ok(self):
 
         self.on_update()
-
         self.window.destroy()
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/edit_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/edit_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/edit_values_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/edit_values_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/equations_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/equations_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/expr_attributes_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/expr_attributes_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/expr_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/expr_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/help_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/help_dialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,45 +4,48 @@
 
 class HelpDialog:
 
     message = r"""
 
 <h1>Editing</h1>
 
-Click on the grid to place a red positive node then click elsewhere
-to place a blue negative node.  Then enter c for a capacitor, i for
+<p>Click on the grid to place a red positive cursor then click elsewhere
+to place a blue negative cursor.  Then enter c for a capacitor, i for
 a current source, l for an inductor, r for a resistor, v for a voltage
-source, etc.  Alternatively, use the Components menu.  The escape key
-will remove both the positive and negative nodes.
+source, etc.  Alternatively, use the Components menu.</p>
 
-The attributes of a component (name, value, etc.) can be edited by
+<p>By default, the cursors snap to the grid and align with the other
+cursor.  The escape key removes both the positive and negative
+cursors.  ctrl+t exchanges the cursors.</p>
+
+<p>The attributes of a component (name, value, etc.) can be edited by
 right clicking on a component.  Note, voltage and current sources
 default to DC.  Select kind as step for transient analysis or specify
-the value as a time domain function.
+the value as a time domain function.</p>
 
-The attributes of a node can be edited by right clicking on a
-node.  This is useful for defining a ground node.
+<p>The attributes of a node can be edited by right clicking on a
+node.  This is useful for defining a ground node.</p>
 
 <h1>Analysis</h1>
 
-Select a component and use Inspect (ctrl+i) to find the voltage across
+<p>Select a component and use Inspect (ctrl+i) to find the voltage across
 a component or the current through a component.  Note the polarity is
-defined by the red (plus) and blue (minus) highlighted nodes.
+defined by the red (plus) and blue (minus) highlighted cursors.</p>
 
-Note, voltage and current sources default to DC.  This can be changed
+<p>Note, voltage and current sources default to DC.  This can be changed
 by right clicking on the source and selecting `DC`, `AC`, `step`, or
 `arbitrary`.  With `arbitrary`, the value can be an arbitrary
 time-domain expression, for example, `4 * H(t) + 2`, where `H(t)` is
-the Heaviside step.
+the Heaviside step.</p>
 
 <h1>Documentation</h1>
 
-For further information about Lcapy, see
+<p>For further information about Lcapy, see
  <a href="https://lcapy-gui.readthedocs.io"> https://lcapy-gui.readthedocs.io </a>
-and  <a href="https://lcapy.readthedocs.io"> https://lcapy.readthedocs.io </a>
+and  <a href="https://lcapy.readthedocs.io"> https://lcapy.readthedocs.io </a> </p>
 """
 
     def __init__(self):
 
         window = Tk()
         window.title('Help!')
         html_label = HTMLLabel(window, html=self.message)
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/inspect_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/inspect_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/labelentries.py` & `lcapygui-0.93/lcapygui/ui/tk/labelentries.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/lateximage.py` & `lcapygui-0.93/lcapygui/ui/tk/lateximage.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/lcapytk.py` & `lcapygui-0.93/lcapygui/ui/tk/lcapytk.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.backends.backend_tkagg import NavigationToolbar2Tk
 from os.path import basename
 from ..uimodelmph import UIModelMPH
 from .sketcher import Sketcher
 from .drawing import Drawing
 from .menu import MenuBar, MenuDropdown, MenuItem
+from ...sketch_library import SketchLibrary
 
 
 class LcapyTk(Tk):
 
     SCALE = 0.01
 
     GEOMETRY = '1200x800'
@@ -26,36 +27,38 @@
 
         super().__init__()
 
         self.debug = debug
         self.version = __version__
         self.model = None
         self.canvas = None
+        self.sketchlib = SketchLibrary()
+        self.dialogs = {}
 
         if uimodel_class is None:
             uimodel_class = UIModelMPH
         self.uimodel_class = uimodel_class
 
         # Title and size of the window
         self.title('Lcapy-tk ' + __version__)
         self.geometry(self.GEOMETRY)
 
         items = []
         for key, val in self.uimodel_class.component_map.items():
             acc = key if len(key) == 1 else ''
-            items.append(MenuItem(val[1], lambda foo=key: self.on_add_cpt(foo),
+            items.append(MenuItem(val[1], command=self.on_add_cpt, arg=key,
                          accelerator=acc))
 
         component_menu_dropdown = MenuDropdown('Components', 0, items)
 
         items = []
 
         for key, val in self.uimodel_class.connection_map.items():
             acc = key if len(key) == 1 else ''
-            items.append(MenuItem(val[1], lambda foo=key: self.on_add_con(foo),
+            items.append(MenuItem(val[1], command=self.on_add_con, arg=key,
                          accelerator=acc))
 
         connection_menu_dropdown = MenuDropdown('Connections', 0, items)
 
         menudropdowns = [
             MenuDropdown('File', 0,
                          [
@@ -108,15 +111,17 @@
                              MenuItem('Nodal equations',
                                       self.on_nodal_equations),
                              MenuItem('Mesh equations',
                                       self.on_mesh_equations),
                              MenuItem('Best fit', self.on_best_fit),
                              MenuItem('Default fit', self.on_default_fit),
                              MenuItem('Plots', self.on_plots),
-                             MenuItem('Description', self.on_description)
+                             MenuItem('Description', self.on_description),
+                             MenuItem('Annotation', self.on_annotation),
+                             MenuItem('Circuit graph ', self.on_circuitgraph)
                          ]),
 
             MenuDropdown('Create', 0,
                          [
                              MenuItem('State space',
                                       self.on_create_state_space),
                              MenuItem('Transfer function',
@@ -179,15 +184,18 @@
 
         self.canvas = None
 
         if pathnames is None:
             pathnames = []
 
         for pathname in pathnames:
-            self.load(pathname)
+            try:
+                self.load(pathname)
+            except FileNotFoundError:
+                self.new(pathname)
 
         if pathnames == []:
             model = self.new()
 
     def clear(self, grid='on'):
 
         self.canvas.drawing.clear(grid)
@@ -235,27 +243,31 @@
         fig.subplots_adjust(left=0, bottom=0, right=1,
                             top=1, wspace=0, hspace=0)
 
         graph = FigureCanvasTkAgg(fig, canvas)
         graph.draw()
         graph.get_tk_widget().pack(fill='both', expand=True)
 
-        toolbar = NavigationToolbar2Tk(graph, canvas, pack_toolbar=False)
-        toolbar.update()
-        toolbar.pack(side=BOTTOM, fill=X)
-
         drawing = Drawing(self, fig, model, self.debug)
         canvas.drawing = drawing
         canvas.tab = tab
         canvas.sketcher = Sketcher(canvas.drawing.ax, self.debug)
 
         tab.canvas = canvas
 
         self.canvases.append(canvas)
 
+        # Display x, y position of cursor
+        drawing.ax.format_coord = lambda x, y: "x:{0:.1f}, y:{1:.1f}".format(
+            x, y)
+
+        toolbar = NavigationToolbar2Tk(graph, canvas, pack_toolbar=False)
+        toolbar.update()
+        toolbar.pack(side=BOTTOM, fill=X)
+
         self.notebook.select(len(self.canvases) - 1)
 
         self.notebook.bind('<<NotebookTabChanged>>', self.on_tab_selected)
 
         canvas.model = model
 
         figure = canvas.drawing.fig
@@ -265,18 +277,19 @@
         canvas.kp_id = figure.canvas.mpl_connect('key_press_event',
                                                  self.on_key_press_event)
 
         self.enter(canvas)
 
         return canvas
 
-    def new(self):
+    def new(self, name='untitled.sch'):
 
         model = self.uimodel_class(self)
-        canvas = self.create_canvas('Untitled', model)
+        model.pathname = name
+        canvas = self.create_canvas(name, model)
         self.model = model
         return model
 
     def on_add_con(self, conname):
 
         if self.debug:
             print('Adding connection ' + conname)
@@ -286,14 +299,21 @@
     def on_add_cpt(self, cptname):
 
         if self.debug:
             print('Adding component ' + cptname)
 
         self.model.on_add_cpt(cptname)
 
+    def on_annotation(self, *args):
+
+        # TODO: add args
+        # TODO: need to support voltage and current labels
+        cct = self.model.circuit.annotate_voltages(None)
+        self.model.on_show_new_circuit(cct)
+
     def on_best_fit(self, *args):
 
         self.model.on_best_fit()
 
     def on_click_event(self, event):
 
         if self.debug:
@@ -345,14 +365,21 @@
         self.canvas.drawing.set_default_view()
         self.refresh()
 
     def on_description(self, *args):
 
         self.show_message_dialog(self.model.circuit.description())
 
+    def on_circuitgraph(self, *args):
+
+        # TODO, save to png file and then display file
+        self.model.circuit.cg.draw('/tmp/cg.png')
+        self.show_image_dialog(
+            '/tmp/cg.png', title='Circuit graph ' + self.model.pathname)
+
     def report_callback_exception(self, exc, val, tb):
 
         # This catches exceptions but only for this window.
         # Each class needs to hook into this.
         from tkinter.messagebox import showerror
 
         showerror("Error", message=str(val))
@@ -601,26 +628,36 @@
 
     def show_help_dialog(self):
 
         from .help_dialog import HelpDialog
 
         self.help_dialog = HelpDialog()
 
+    def show_image_dialog(self, filename, title=''):
+
+        from .image_dialog import ImageDialog
+
+        self.image_dialog = ImageDialog(self, filename, title)
+
     def show_inspect_dialog(self, cpt, title=''):
 
         from .inspect_dialog import InspectDialog
 
         self.inspect_dialog = InspectDialog(self.model, cpt, title)
 
     def inspect_properties_dialog(self, cpt, on_changed=None, title=''):
 
         from .cpt_properties_dialog import CptPropertiesDialog
 
-        self.cpt_properties_dialog = CptPropertiesDialog(self, cpt,
-                                                         on_changed, title)
+        name = cpt.name
+        if name in self.dialogs:
+            self.dialogs[name].focus()
+        else:
+            dialog = CptPropertiesDialog(self, cpt, on_changed, title)
+            self.dialogs[name] = dialog
 
     def show_info_dialog(self, message):
 
         from tkinter.messagebox import showinfo
 
         showinfo('', message)
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/lcapytkm.py` & `lcapygui-0.93/lcapygui/ui/tk/lcapytkm.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/limit_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/limit_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         if len(symbols) == 0:
             raise ValueError('Constant expression')
 
         entries = []
         entries.append(LabelEntry('symbol', 'symbol',
                                   symbols[0], symbols))
 
-        entries.append(LabelEntry('limit', 'Limit', 0.0))
+        entries.append(LabelEntry('limit', 'Limit', '0'))
 
         entries.append(LabelEntry('dir', 'Direction',
                                   '+', ('+', '-')))
 
         self.labelentries = LabelEntries(self.window, ui, entries)
 
         button = Button(self.window, text="OK", command=self.on_ok)
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/menu.py` & `lcapygui-0.93/lcapygui/ui/tk/menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from tkinter import Menu
 
 
 class MenuItem:
 
-    def __init__(self, label, command=None, underline=0, accelerator=None):
+    def __init__(self, label, command=None, arg=None, underline=0, accelerator=None):
 
         self.label = label
         self.command = command
+        self.arg = arg
         self.underline = underline
         self.accelerator = accelerator
 
 
 class MenuDropdown:
 
     def __init__(self, label, underline=0, menuitems=None):
@@ -26,15 +27,19 @@
 
         self.menudropdowns = menudropdowns
 
     def make(self, window):
 
         def doit(menuitem):
 
-            menuitem.command(menuitem.label)
+            arg = menuitem.arg
+            if arg is None:
+                arg = menuitem.label
+
+            menuitem.command(arg)
 
         # Create the drop down menus
         self.menubar = Menu(window, bg='lightgrey', fg='black')
 
         self.menus = []
 
         for menudropdown in self.menudropdowns:
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/multiplot_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/multiplot_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/node_properties_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/node_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/plot_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/plot_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/plot_properties_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/plot_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/preferences_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/preferences_dialog.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,16 +32,16 @@
                               self.model.preferences.voltage_dir,
                               ('RP', 'EF'),
                               command=self.on_update),
                    LabelEntry('grid', 'Grid',
                               self.model.preferences.grid,
                               ('on', 'off'),
                               command=self.on_update),
-                   LabelEntry('lw', 'Line width',
-                              self.model.preferences.lw,
+                   LabelEntry('line_width', 'Line width',
+                              self.model.preferences.line_width,
                               command=self.on_update),
                    LabelEntry('node_size', 'Node size',
                               self.model.preferences.node_size,
                               command=self.on_update),
                    LabelEntry('show_units', 'Show units',
                               self.model.preferences.show_units,
                               ('true', 'false'),
@@ -69,15 +69,18 @@
             'label_nodes')
         self.model.preferences.draw_nodes = self.labelentries.get('draw_nodes')
         self.model.preferences.label_cpts = self.labelentries.get('label_cpts')
         self.model.preferences.style = self.labelentries.get('style')
         self.model.preferences.voltage_dir = self.labelentries.get(
             'voltage_dir')
         self.model.preferences.grid = self.labelentries.get('grid')
-        self.model.preferences.lw = self.labelentries.get('lw')
+        line_width = self.labelentries.get('line_width')
+        if not line_width.endswith('pt') and not line_width.endswith('mm'):
+            line_width += 'pt'
+        self.model.preferences.line_width = line_width
         self.model.preferences.node_size = self.labelentries.get('node_size')
         self.model.preferences.show_units = self.labelentries.get('show_units')
         self.model.preferences.xsize = self.labelentries.get('xsize')
         self.model.preferences.ysize = self.labelentries.get('ysize')
         self.model.preferences.snap_grid = self.labelentries.get('snap_grid')
 
         # Do not set show_units; this needs fixing in Lcapy since
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/python_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/python_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/sketcher.py` & `lcapygui-0.93/lcapygui/ui/tk/sketcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,14 @@
                 path = Path(vertices, path.codes)
             if invert:
                 vertices = path.vertices * (-1, 1)
                 path = Path(vertices, path.codes)
 
             path = path.transformed(gtransform)
 
-            if False and patches == []:
-                print(path.vertices)
-
             fill = kwargs.pop('fill', fill)
 
             if self.debug:
                 color = ['red', 'yellow', 'orange',
                          'green', 'blue', 'violet'][m % 6]
 
             patch = PathPatch(path, fill=fill, color=color, **kwargs)
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/state_space_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/state_space_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/subs_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/subs_dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         self.window.title(title)
 
         entries = []
 
         self.symbols = []
         for key in expr.symbols:
             # Ignore domain variable
-            if key != expr.var.name:
-                entries.append(LabelEntry(key, key, 0.0))
+            if expr.var is None or key != expr.var.name:
+                entries.append(LabelEntry(key, key, key))
                 self.symbols.append(key)
 
         self.labelentries = LabelEntries(self.window, ui, entries)
 
         button = Button(self.window, text="Subs",
                         command=self.on_update)
         button.grid(row=self.labelentries.row)
```

### Comparing `lcapygui-0.92/lcapygui/ui/tk/transfer_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/transfer_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/transfer_function_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/transfer_function_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/twoport_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/twoport_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/tk/twoport_select_dialog.py` & `lcapygui-0.93/lcapygui/ui/tk/twoport_select_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.92/lcapygui/ui/uimodelbase.py` & `lcapygui-0.93/lcapygui/ui/uimodelbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..annotation import Annotation
 from ..annotations import Annotations
 from .preferences import Preferences
 from ..components.opamp import Opamp
-from ..components.cpt_maker import cpt_make_from_cpt, cpt_make_from_type, cpt_remake
+from ..components.cpt_maker import cpt_make_from_cpt, cpt_make_from_type
 
 from copy import copy
 from math import atan2, degrees, sqrt
 from numpy import nan, isnan
 from lcapy import Circuit, expr
 from lcapy.mnacpts import Cpt
 from lcapy.nodes import parse_nodes
@@ -18,36 +18,38 @@
 
     STEP = 2
     SNAP = 1
     SCALE = 0.25
 
     # Short-cut key, name, type, kind
     component_map = {
+        'y': ('y', 'Admittance', 'Y', ''),
         'c': ('c', 'Capacitor', 'C', ''),
+        'cpe': ('', 'Constant phase element (CPE)', 'CPE', ''),
+        'f': ('f', 'Current controlled current source', 'F', ''),
+        'h': ('h', 'Current controlled voltage source', 'H', ''),
+        'i': ('i', 'Current source', 'I', ''),
         'd': ('d', 'Diode', 'D', ''),
         'fb': ('', 'Ferrite bead', 'FB', ''),
-        'i': ('i', 'Current source', 'I', ''),
-        'j': ('j', 'JFET', 'J', ''),
+        'z': ('z', 'Impedance', 'Z', ''),
         'l': ('l', 'Inductor', 'L', ''),
-        'm': ('m', 'MOSFET', 'M', ''),
-        'q': ('q', 'BJT', 'Q', ''),
+        'opamp': ('', 'Opamp', 'opamp', ''),
+        'fdopamp': ('', 'Opamp (fully differential)', 'fdopamp', ''),
+        'o': ('o', 'Open circuit', 'O', ''),
+        'p': ('p', 'Port', 'P', ''),
         'r': ('r', 'Resistor', 'R', ''),
-        'nr': ('', 'Noiseless resistor', 'R', ''),
+        'nr': ('', 'Resistor (noiseless)', 'R', ''),
+        'tf': ('tf', 'Transformer', 'TF', ''),
+        'q': ('q', 'Transistor BJT', 'Q', ''),
+        'j': ('j', 'Transistor JFET', 'J', ''),
+        'm': ('m', 'Transistor MOSFET', 'M', ''),
         'v': ('v', 'Voltage source', 'V', ''),
+        'g': ('g', 'Voltage controlled current source', 'G', ''),
+        'e': ('e', 'Voltage controlled voltage source', 'E', ''),
         'w': ('w', 'Wire', 'W', ''),
-        'e': ('e', 'VCVS', 'E', ''),
-        'f': ('f', 'CCCS', 'F', ''),
-        'g': ('g', 'VCCS', 'G', ''),
-        'h': ('h', 'CCVS', 'H', ''),
-        'o': ('o', 'Open circuit', 'O', ''),
-        'opamp': ('', 'Opamp', 'opamp', ''),
-        'p': ('p', 'Port', 'P', ''),
-        'y': ('y', 'Admittance', 'Y', ''),
-        'z': ('z', 'Impedance', 'Z', ''),
-        'cpe': ('', 'CPE', 'CPE', ''),
     }
 
     connection_map = {
         '0': ('0', '0V', 'W', ''),
         '0V': ('', '0V', 'W', '0V'),
         'ground': ('', 'Ground', 'W', ''),
         'sground': ('', 'Signal ground', 'W', 'sground'),
@@ -123,15 +125,15 @@
                 ymin = node.y
             if node.y > ymax:
                 ymax = node.y
         return xmin, ymin, xmax, ymax
 
     def choose_cpt_name(self, cpt_type):
 
-        if cpt_type == 'opamp':
+        if cpt_type in ('opamp', 'fdopamp'):
             cpt_type = 'E'
 
         num = 1
         while True:
             name = cpt_type + str(num)
             if name not in self.circuit.elements:
                 return name
@@ -198,15 +200,15 @@
 
     def cpt_draw(self, cpt):
 
         gcpt = cpt.gcpt
         if gcpt is None:
             return
 
-        gcpt.draw(self, self.ui.sketcher)
+        gcpt.draw(self)
 
         label_cpts = self.preferences.label_cpts
 
         if gcpt.type in ('A', 'O', 'W'):
             label_cpts = 'none'
 
         name = cpt.name
@@ -291,24 +293,24 @@
                 'Cannot find a component with nodes %s and %s' % (node_name1, node_name2))
         return fcpt
 
     def cpt_remake(self, cpt):
 
         gcpt = cpt.gcpt
 
-        if cpt.is_dependent_source and gcpt.type != 'Eopamp':
+        if cpt.is_dependent_source and gcpt.type not in ('Eopamp', 'Efdopamp'):
             try:
                 newcpt = cpt._change_control(gcpt.control)
             except Exception:
                 self.exception('Control component %s for %s deleted' %
                                (gcpt.control, cpt.name))
                 return
         elif gcpt.cpt_kind == cpt._kind:
             newcpt = cpt
-        elif gcpt.type != 'Eopamp':
+        elif gcpt.type not in ('Eopamp', 'Efdopamp'):
             try:
                 newcpt = cpt._change_kind(gcpt.cpt_kind)
             except Exception:
                 self.exception('Cannot change kind for %s' % cpt.name)
                 return
         else:
             newcpt = cpt
@@ -320,24 +322,25 @@
                 self.exception('Cannot change name for %s' % cpt.name)
                 return
 
         if gcpt.mirror ^ ('mirror' in newcpt.opts):
             # TODO, add mirror method...
             if gcpt.type == 'Eopamp':
                 newcpt.nodes[2], newcpt.nodes[3] = newcpt.nodes[3], newcpt.nodes[2]
+            elif gcpt.type == 'Efdopamp':
+                newcpt.nodes[2], newcpt.nodes[3] = newcpt.nodes[3], newcpt.nodes[2]
             elif gcpt.type in ('J', 'M', 'Q'):
                 newcpt.nodes[2], newcpt.nodes[0] = newcpt.nodes[0], newcpt.nodes[2]
             else:
                 print('Trying to change mirror for ' + str(newcpt))
 
         newcpt.opts.clear()
         newcpt.opts.add(gcpt.attr_string_update(self.STEP))
 
         newcpt.gcpt = gcpt
-        cpt_remake(newcpt.gcpt)
 
     def cut(self, cpt):
 
         self.delete(cpt)
         self.clipboard = cpt
 
     def delete(self, cpt):
@@ -410,16 +413,16 @@
                 return
 
             width, height = sch.width * self.STEP, sch.height * self.STEP
 
             # Centre the schematic.
             xsize = self.ui.canvas.drawing.xsize
             ysize = self.ui.canvas.drawing.ysize
-            offsetx, offsety = self.snap((xsize - width) / 2,
-                                         (ysize - height) / 2)
+            offsetx, offsety = self.snap_to_grid((xsize - width) / 2,
+                                                 (ysize - height) / 2)
             for node in sch.nodes.values():
                 node.pos.x += offsetx
                 node.pos.y += offsety
                 # May have split nodes...
                 if node.name in circuit.nodes:
                     circuit.nodes[node.name].pos = node.pos
 
@@ -494,28 +497,30 @@
 
     def schematic(self):
 
         s = '# Created by ' + self.ui.NAME + ' V' + self.ui.version + '\n'
 
         # Define node positions
         foo = [str(node) for node in self.circuit.nodes.values()
-               if not isnan(node.pos.x)]
+               if node.pos is not None and not isnan(node.pos.x)]
 
         s += '; nodes={' + ', '.join(foo) + '}' + '\n'
 
         for cpt in self.circuit.elements.values():
             s += str(cpt) + '\n'
 
         # FIXME, remove other preference string
         # Note, need a newline so string treated as a netlist string
         s += '; ' + self.preferences.schematic_preferences() + '\n'
         return s
 
     def thing_create(self, cpt_type, x1, y1, x2, y2, kind=''):
 
+        from lcapy.mnacpts import Cpt
+
         cpt_name = self.choose_cpt_name(cpt_type)
         gcpt = cpt_make_from_type(cpt_type, cpt_name, kind=kind)
         if gcpt is None:
             return
 
         all_node_names = list(self.circuit.nodes)
         node_names = []
@@ -534,17 +539,20 @@
             node_names.append(node_name)
 
         netitem = gcpt.netitem(node_names, x1, y1, x2, y2, self.STEP)
 
         if self.ui.debug:
             print('Adding ' + netitem)
 
-        cct = self.circuit.add(netitem)
+        cpt = self.circuit.add(netitem)
         self.invalidate()
-        cpt = cct[cpt_name]
+
+        if not isinstance(cpt, Cpt):
+            # Support older versions of Lcapy
+            cpt = self.circuit[cpt_name]
 
         for m, position in enumerate(positions):
             cpt.nodes[m].pos = Pos(position)
 
         attr_string = netitem.split(';', 1)[1]
         gcpt.update(nodes=cpt.nodes, opts=Opts(attr_string))
 
@@ -621,20 +629,47 @@
         except (AttributeError, ValueError, RuntimeError) as e:
             self.exception(e)
 
     def select(self, thing):
 
         self.selected = thing
 
-    def snap(self, x, y):
+    def is_close_to(self, x, xc):
+
+        return abs(x - xc) < 0.3
+
+    def is_on_grid_x(self, x):
+
+        xs = self.snap_to_grid_x(x)
+        return x == xs
+
+    def is_on_grid_y(self, y):
+
+        ys = self.snap_to_grid_y(y)
+        return y == ys
+
+    def is_on_grid(self, x, y):
+
+        return self.is_on_grid_x(x) and self.is_on_grid_y(y)
+
+    def snap_to_grid_x(self, x):
 
         snap = self.SNAP
         x = (x + 0.5 * snap) // snap * snap
+        return x
+
+    def snap_to_grid_y(self, y):
+
+        snap = self.SNAP
         y = (y + 0.5 * snap) // snap * snap
-        return x, y
+        return y
+
+    def snap_to_grid(self, x, y):
+
+        return self.snap_to_grid_x(x), self.snap_to_grid_y(y)
 
     def unselect(self):
         pass
 
     def view(self):
 
         cct = Circuit(self.schematic())
```

### Comparing `lcapygui-0.92/lcapygui/ui/uimodelmph.py` & `lcapygui-0.93/lcapygui/ui/uimodelmph.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             'ctrl+e': self.on_export,
             'ctrl+h': self.on_help,
             'ctrl+i': self.on_inspect,
             'ctrl+n': self.on_new,
             'ctrl+o': self.on_load,
             'ctrl+s': self.on_save,
             'alt+s': self.on_save_as,
+            'ctrl+t': self.on_exchange_cursors,
             'ctrl+u': self.on_view,
             'ctrl+v': self.on_paste,
             'ctrl+w': self.on_quit,
             'ctrl+x': self.on_cut,
             'ctrl+y': self.on_redo,
             'ctrl+z': self.on_undo,
             'ctrl+9': self.on_pdb,
@@ -87,14 +88,17 @@
         for k, v in self.component_map.items():
             self.key_bindings_with_key[k] = self.on_add_cpt
         for k, v in self.connection_map.items():
             self.key_bindings_with_key[k] = self.on_add_con
 
     def add_cursor(self, x, y):
 
+        # cursors[0] is the positive cursor
+        # cursors[1] is the negative cursor
+
         cursor = Cursor(self.ui, x, y)
 
         if len(self.cursors) == 0:
             cursor.draw('red')
             self.cursors.append(cursor)
 
         elif len(self.cursors) == 1:
@@ -164,14 +168,15 @@
         self.ui.show_transfer_function_dialog(cpt)
 
     def create_twoport(self, cpt, kind):
 
         self.ui.show_twoport_dialog(cpt, kind)
 
     def exception(self, e):
+
         message = str(e)
         if self.pathname != '':
             message += ' in ' + self.pathname
         self.ui.show_error_dialog(message)
         if self.ui.debug:
             import pdb
             pdb.set_trace()
@@ -190,20 +195,34 @@
                 base = '_'.join(parts[0:-1])
             except ValueError:
                 suffix = '1'
         return base + '_' + suffix + ext
 
     def on_add_node(self, x, y):
 
-        # Snap to known node then snap to grid.
+        # Snap to closest known node then snap to grid.
         node = self.closest_node(x, y)
         if node is None:
+
             if self.preferences.snap_grid == 'true':
-                x, y = self.snap(x, y)
-            # Could be smarter and try to align with nearby node.
+
+                if len(self.cursors) > 0:
+                    xc = self.cursors[0].x
+                    yc = self.cursors[0].y
+                    if self.is_close_to(x, xc):
+                        x = xc
+                    else:
+                        x = self.snap_to_grid_x(x)
+                    if self.is_close_to(y, yc):
+                        y = yc
+                    else:
+                        y = self.snap_to_grid_y(y)
+                else:
+                    x, y = self.snap_to_grid(x, y)
+
         else:
             x, y = node.x, node.y
 
         self.add_cursor(x, y)
 
     def on_add_cpt(self, cpt_key):
 
@@ -358,14 +377,18 @@
         self.ui.refresh()
 
     def on_describe(self):
 
         self.ui.show_message_dialog(self.circuit.description(),
                                     title='Description')
 
+    def on_exchange_cursors(self):
+
+        self.exchange_cursors()
+
     def on_expand(self):
 
         cct = self.circuit.expand()
         self.on_show_new_circuit(cct)
 
     def on_export(self):
 
@@ -679,11 +702,22 @@
 
         with open(schtex_filename) as f:
             content = f.read()
         remove(schtex_filename)
 
         self.ui.show_message_dialog(content)
 
+    def exchange_cursors(self):
+
+        if len(self.cursors) < 2:
+            return
+        self.cursors[0], self.cursors[1] = self.cursors[1], self.cursors[0]
+        self.cursors[0].remove()
+        self.cursors[1].remove()
+        self.cursors[0].draw('red')
+        self.cursors[1].draw('blue')
+        self.ui.refresh()
+
     def unselect(self):
 
         self.cursors.remove()
         self.ui.refresh()
```

### Comparing `lcapygui-0.92/lcapygui.egg-info/PKG-INFO` & `lcapygui-0.93/lcapygui.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapygui
-Version: 0.92
+Version: 0.93
 Summary: A GUI for lcapy
 Home-page: https://github.com/mph-/lcapy-gui
 Author: Michael Hayes, Jordan Hay
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mph-/lcapy-gui
 Description: # lcapy-gui
```

### Comparing `lcapygui-0.92/lcapygui.egg-info/SOURCES.txt` & `lcapygui-0.93/lcapygui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.cfg
 setup.py
 lcapygui/__init__.py
 lcapygui/annotation.py
 lcapygui/annotations.py
 lcapygui/node.py
 lcapygui/nodes.py
+lcapygui/sketch_library.py
 lcapygui.egg-info/PKG-INFO
 lcapygui.egg-info/SOURCES.txt
 lcapygui.egg-info/dependency_links.txt
 lcapygui.egg-info/entry_points.txt
 lcapygui.egg-info/requires.txt
 lcapygui.egg-info/top_level.txt
 lcapygui/components/__init__.py
@@ -24,25 +25,27 @@
 lcapygui/components/component.py
 lcapygui/components/connection.py
 lcapygui/components/controlledcomponent.py
 lcapygui/components/cpe.py
 lcapygui/components/cpt_maker.py
 lcapygui/components/current_source.py
 lcapygui/components/diode.py
+lcapygui/components/fdopamp.py
 lcapygui/components/ferritebead.py
 lcapygui/components/impedance.py
 lcapygui/components/inductor.py
 lcapygui/components/jfet.py
 lcapygui/components/mosfet.py
 lcapygui/components/opamp.py
 lcapygui/components/opencircuit.py
 lcapygui/components/port.py
 lcapygui/components/resistor.py
 lcapygui/components/sketch.py
 lcapygui/components/svgparse.py
+lcapygui/components/transformer.py
 lcapygui/components/transistor.py
 lcapygui/components/vccs.py
 lcapygui/components/vcvs.py
 lcapygui/components/voltage_source.py
 lcapygui/components/wire.py
 lcapygui/scripts/__init__.py
 lcapygui/scripts/lcapytk.py
@@ -59,14 +62,15 @@
 lcapygui/ui/tk/edit_values_dialog.py
 lcapygui/ui/tk/equations_dialog.py
 lcapygui/ui/tk/expr_attributes_dialog.py
 lcapygui/ui/tk/expr_calc.py
 lcapygui/ui/tk/expr_dialog.py
 lcapygui/ui/tk/exprimage.py
 lcapygui/ui/tk/help_dialog.py
+lcapygui/ui/tk/image_dialog.py
 lcapygui/ui/tk/inspect_dialog.py
 lcapygui/ui/tk/labelentries.py
 lcapygui/ui/tk/lateximage.py
 lcapygui/ui/tk/lcapytk.py
 lcapygui/ui/tk/lcapytkm.py
 lcapygui/ui/tk/limit_dialog.py
 lcapygui/ui/tk/menu.py
```

### Comparing `lcapygui-0.92/setup.py` & `lcapygui-0.93/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name='lcapygui',
     packages=find_packages(include=[
         "lcapygui",
         "lcapygui.*"
     ]),
-    version="0.92",
+    version="0.93",
     description="A GUI for lcapy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Michael Hayes, Jordan Hay",
     license="MIT",
     url="https://github.com/mph-/lcapy-gui",
     project_urls={
@@ -42,10 +42,10 @@
     ],
     entry_points={
         'console_scripts': [
             'lcapy-tk=lcapygui.scripts.lcapytk:main',
         ],
     },
     include_package_data=True,
-    package_data={'': ['data/svg/*.svg', 'data/lib/*.sch']},
+    package_data={'': ['data/svg/*/*.svg', 'data/lib/*/*.sch']},
     python_requires=">=3.7"  # matched with lcapy
 )
```

