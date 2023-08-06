# Comparing `tmp/ogl-0.70.52.tar.gz` & `tmp/ogl-0.85.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogl-0.70.52.tar", last modified: Fri Jun  9 21:30:57 2023, max compression
+gzip compressed data, was "ogl-0.85.0.tar", last modified: Sun Aug  6 03:15:47 2023, max compression
```

## Comparing `ogl-0.70.52.tar` & `ogl-0.85.0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.377038 ogl-0.70.52/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.52/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-06-09 21:30:57.376918 ogl-0.70.52/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1999 2023-04-12 19:50:00.000000 ogl-0.70.52/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.369367 ogl-0.70.52/miniogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.52/miniogl/AnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.52/miniogl/AttachmentSide.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3100 2023-06-09 19:44:45.000000 ogl-0.70.52/miniogl/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/Constants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/ControlPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-05-15 20:23:59.000000 ogl-0.70.52/miniogl/Diagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-05-16 01:00:55.000000 ogl-0.70.52/miniogl/DiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.52/miniogl/DlgDebugDiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/LinePoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.52/miniogl/LineShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.52/miniogl/LollipopLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.52/miniogl/MiniOglColorEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/MiniOglPenStyle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/MiniOglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/PointShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-05-16 01:00:24.000000 ogl-0.70.52/miniogl/RectangleShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/RectangleShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.52/miniogl/RotatableShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.52/miniogl/SelectAnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-05-15 20:23:15.000000 ogl-0.70.52/miniogl/Shape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2336 2023-05-16 16:52:43.000000 ogl-0.70.52/miniogl/ShapeEventHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.52/miniogl/ShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2023-05-16 00:57:28.000000 ogl-0.70.52/miniogl/SizerShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.52/miniogl/TextShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/TextShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.52/miniogl/VShapes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.52/miniogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.52/miniogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.372237 ogl-0.70.52/ogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/IllegalOperationException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4646 2023-05-16 01:11:07.000000 ogl-0.70.52/ogl/OglActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.52/ogl/OglAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.52/ogl/OglAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      328 2023-06-09 20:08:20.000000 ogl-0.70.52/ogl/OglAssociationLabel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-05-16 00:59:29.000000 ogl-0.70.52/ogl/OglClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.52/ogl/OglComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/OglConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/OglDimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.52/ogl/OglInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.70.52/ogl/OglInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.52/ogl/OglInterface2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.52/ogl/OglLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.52/ogl/OglLinkFactory.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.52/ogl/OglNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.52/ogl/OglNoteLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5529 2023-05-16 16:51:16.000000 ogl-0.70.52/ogl/OglObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      474 2023-06-09 20:04:54.000000 ogl-0.70.52/ogl/OglPosition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8683 2023-05-15 20:22:45.000000 ogl-0.70.52/ogl/OglText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/OglTextFontFamily.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.52/ogl/OglUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/OglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-05-14 21:20:56.000000 ogl-0.70.52/ogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       24 2023-06-09 21:21:11.000000 ogl-0.70.52/ogl/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.373562 ogl-0.70.52/ogl/events/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.52/ogl/events/IOglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/events/InvalidKeywordException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.52/ogl/events/OglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.52/ogl/events/OglEvents.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/events/ShapeSelectedEventData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/events/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.52/ogl/events/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.373862 ogl-0.70.52/ogl/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21282 2023-05-14 20:59:24.000000 ogl-0.70.52/ogl/preferences/OglPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.52/ogl/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.52/ogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.373946 ogl-0.70.52/ogl/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.374477 ogl-0.70.52/ogl/resources/img/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/resources/img/Display.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/resources/img/DoNotDisplay.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/resources/img/UnSpecified.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/resources/img/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.52/ogl/resources/img/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.374898 ogl-0.70.52/ogl/resources/img/textdetails/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/resources/img/textdetails/DecreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/resources/img/textdetails/IncreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/resources/img/textdetails/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.52/ogl/resources/img/textdetails/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.375385 ogl-0.70.52/ogl/sd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      904 2023-05-12 20:37:54.000000 ogl-0.70.52/ogl/sd/OglInstanceName.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-05-16 01:17:51.000000 ogl-0.70.52/ogl/sd/OglSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6874 2023-05-14 21:08:57.000000 ogl-0.70.52/ogl/sd/OglSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.52/ogl/sd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.52/ogl/sd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.375883 ogl-0.70.52/ogl/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-05-16 00:59:48.000000 ogl-0.70.52/ogl/ui/BaseOglPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.52/ogl/ui/DefaultValuesPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.52/ogl/ui/DiagramPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.52/ogl/ui/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.52/ogl/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.376753 ogl-0.70.52/ogl/ui/valuecontrols/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.52/ogl/ui/valuecontrols/AssociationAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.52/ogl/ui/valuecontrols/ClassAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.52/ogl/ui/valuecontrols/DefaultNamesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.52/ogl/ui/valuecontrols/NoteAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.52/ogl/ui/valuecontrols/SDAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5284 2023-05-14 22:17:09.000000 ogl-0.70.52/ogl/ui/valuecontrols/TextAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.52/ogl/ui/valuecontrols/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:30:57.372764 ogl-0.70.52/ogl.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-06-09 21:30:57.000000 ogl-0.70.52/ogl.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2516 2023-06-09 21:30:57.000000 ogl-0.70.52/ogl.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 21:30:57.000000 ogl-0.70.52/ogl.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-06-09 21:30:57.000000 ogl-0.70.52/ogl.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-06-09 21:30:57.000000 ogl-0.70.52/ogl.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 21:30:57.377069 ogl-0.70.52/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1565 2023-06-09 21:21:38.000000 ogl-0.70.52/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.021572 ogl-0.85.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-07-05 13:40:50.000000 ogl-0.85.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    42076 2023-08-06 03:15:47.021438 ogl-0.85.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1898 2023-08-06 03:13:18.000000 ogl-0.85.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.008373 ogl-0.85.0/miniogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.85.0/miniogl/AnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.85.0/miniogl/AttachmentSide.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3100 2023-06-09 19:44:45.000000 ogl-0.85.0/miniogl/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/Constants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/ControlPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-05-15 20:23:59.000000 ogl-0.85.0/miniogl/Diagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-05-16 01:00:55.000000 ogl-0.85.0/miniogl/DiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.85.0/miniogl/DlgDebugDiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/LinePoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.85.0/miniogl/LineShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.85.0/miniogl/LollipopLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.85.0/miniogl/MiniOglColorEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/MiniOglPenStyle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/MiniOglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/PointShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-05-16 01:00:24.000000 ogl-0.85.0/miniogl/RectangleShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/RectangleShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.85.0/miniogl/RotatableShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.85.0/miniogl/SelectAnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-05-15 20:23:15.000000 ogl-0.85.0/miniogl/Shape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2336 2023-05-16 16:52:43.000000 ogl-0.85.0/miniogl/ShapeEventHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.85.0/miniogl/ShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2023-05-16 00:57:28.000000 ogl-0.85.0/miniogl/SizerShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.85.0/miniogl/TextShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/TextShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.85.0/miniogl/VShapes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.85.0/miniogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.85.0/miniogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.014387 ogl-0.85.0/ogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/IllegalOperationException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4646 2023-05-16 01:11:07.000000 ogl-0.85.0/ogl/OglActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.85.0/ogl/OglAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13187 2023-08-06 03:13:18.000000 ogl-0.85.0/ogl/OglAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      448 2023-08-06 03:13:18.000000 ogl-0.85.0/ogl/OglAssociationLabel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-05-16 00:59:29.000000 ogl-0.85.0/ogl/OglClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.85.0/ogl/OglComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/OglConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/OglDimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.85.0/ogl/OglInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.85.0/ogl/OglInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.85.0/ogl/OglInterface2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.85.0/ogl/OglLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.85.0/ogl/OglLinkFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.85.0/ogl/OglNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.85.0/ogl/OglNoteLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5529 2023-05-16 16:51:16.000000 ogl-0.85.0/ogl/OglObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      474 2023-06-09 20:04:54.000000 ogl-0.85.0/ogl/OglPosition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8683 2023-05-15 20:22:45.000000 ogl-0.85.0/ogl/OglText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/OglTextFontFamily.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.85.0/ogl/OglUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/OglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-05-14 21:20:56.000000 ogl-0.85.0/ogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       23 2023-08-06 03:13:18.000000 ogl-0.85.0/ogl/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.016140 ogl-0.85.0/ogl/events/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.85.0/ogl/events/IOglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/events/InvalidKeywordException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.85.0/ogl/events/OglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.85.0/ogl/events/OglEvents.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/events/ShapeSelectedEventData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/events/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.85.0/ogl/events/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.016697 ogl-0.85.0/ogl/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21282 2023-05-14 20:59:24.000000 ogl-0.85.0/ogl/preferences/OglPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.85.0/ogl/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.85.0/ogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.016781 ogl-0.85.0/ogl/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.017335 ogl-0.85.0/ogl/resources/img/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/resources/img/Display.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/resources/img/DoNotDisplay.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/resources/img/UnSpecified.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/resources/img/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.85.0/ogl/resources/img/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.017763 ogl-0.85.0/ogl/resources/img/textdetails/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/resources/img/textdetails/DecreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/resources/img/textdetails/IncreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/resources/img/textdetails/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.85.0/ogl/resources/img/textdetails/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.018636 ogl-0.85.0/ogl/sd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      904 2023-05-12 20:37:54.000000 ogl-0.85.0/ogl/sd/OglInstanceName.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-05-16 01:17:51.000000 ogl-0.85.0/ogl/sd/OglSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6874 2023-05-14 21:08:57.000000 ogl-0.85.0/ogl/sd/OglSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.85.0/ogl/sd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.85.0/ogl/sd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.019496 ogl-0.85.0/ogl/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-05-16 00:59:48.000000 ogl-0.85.0/ogl/ui/BaseOglPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.85.0/ogl/ui/DefaultValuesPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.85.0/ogl/ui/DiagramPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.85.0/ogl/ui/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.85.0/ogl/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.021219 ogl-0.85.0/ogl/ui/valuecontrols/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.85.0/ogl/ui/valuecontrols/AssociationAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.85.0/ogl/ui/valuecontrols/ClassAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.85.0/ogl/ui/valuecontrols/DefaultNamesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.85.0/ogl/ui/valuecontrols/NoteAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.85.0/ogl/ui/valuecontrols/SDAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5284 2023-05-14 22:17:09.000000 ogl-0.85.0/ogl/ui/valuecontrols/TextAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.85.0/ogl/ui/valuecontrols/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-08-06 03:15:47.014955 ogl-0.85.0/ogl.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    42076 2023-08-06 03:15:46.000000 ogl-0.85.0/ogl.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2516 2023-08-06 03:15:46.000000 ogl-0.85.0/ogl.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-08-06 03:15:46.000000 ogl-0.85.0/ogl.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-08-06 03:15:46.000000 ogl-0.85.0/ogl.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-08-06 03:15:46.000000 ogl-0.85.0/ogl.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-08-06 03:15:47.021603 ogl-0.85.0/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1586 2023-08-06 03:13:18.000000 ogl-0.85.0/setup.py
```

### Comparing `ogl-0.70.52/LICENSE` & `ogl-0.85.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/PKG-INFO` & `ogl-0.85.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: ogl
-Version: 0.70.52
-Summary: External Pyut Graphical Shapes
-Home-page: https://github.com/hasii2011/ogl
-Author: Humberto A. Sanchez II
-Author-email: Humberto.A.Sanchez.II@gmail.com
-Maintainer: Humberto A. Sanchez II
-Maintainer-email: humberto.a.sanchez.ii@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img src="./developer/agpl-license-web-badge-version-2-256x48.png"/> 
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/ogl/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/ogl/tree/master)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
@@ -47,11 +35,7 @@
 
 While I do not advocate for all the issues listed there I do not like that a company like Microsoft may profit from open source projects.
 
 I continue to use GitHub because it offers the services I need for free.  But, I continue to monitor their terms of service.
 
 Any use of this project's code by GitHub Copilot, past or present, is done without my permission.  I do not consent to GitHub's use of this project's
 code in Copilot.
-
-A repository owner may opt out of Copilot by changing Settings --> GitHub Copilot.
-
-I have done so.
```

#### html2text {}

```diff
@@ -1,30 +1,25 @@
-Metadata-Version: 2.1 Name: ogl Version: 0.70.52 Summary: External Pyut
-Graphical Shapes Home-page: https://github.com/hasii2011/ogl Author: Humberto
-A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com Maintainer:
-Humberto A. Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com
-Description-Content-Type: text/markdown License-File: LICENSE [./developer/
-agpl-license-web-badge-version-2-256x48.png] [![Maintenance](https://
-img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/
-StrapDown.js/graphs/commit-activity) [![CircleCI](https://dl.circleci.com/
-status-badge/img/gh/hasii2011/ogl/tree/master.svg?style=shield)](https://
-dl.circleci.com/status-badge/redirect/gh/hasii2011/ogl/tree/master) [![macOS]
-(https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg) [!
-[forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) ð ð¨ ð¤ ð£ stands for Python UML
-Tool. This is the external graphical shapes module for Pyut that allows for
-external plugin development; This project depends on pyutmodel and wxPython ___
-## Developer Notes This project uses [buildlackey](https://github.com/
-hasii2011/buildlackey) for day to day development builds ___ Written by
-Humberto_A._Sanchez_II (C) 2023 ## Note For all kind of problems, requests,
-enhancements, bug reports, etc., please drop me an e-mail. ![Humberto's
-Modified Logo](https://raw.githubusercontent.com/wiki/hasii2011/
-gittodoistclone/images/SillyGitHub.png) I am concerned about GitHub's Copilot
-project I urge you to read about the [Give up GitHub](https://GiveUpGitHub.org)
-campaign from [the Software Freedom Conservancy](https://sfconservancy.org).
-While I do not advocate for all the issues listed there I do not like that a
-company like Microsoft may profit from open source projects. I continue to use
-GitHub because it offers the services I need for free. But, I continue to
-monitor their terms of service. Any use of this project's code by GitHub
-Copilot, past or present, is done without my permission. I do not consent to
-GitHub's use of this project's code in Copilot. A repository owner may opt out
-of Copilot by changing Settings --> GitHub Copilot. I have done so.
+[./developer/agpl-license-web-badge-version-2-256x48.png] [![Maintenance]
+(https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/
+Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
+dl.circleci.com/status-badge/img/gh/hasii2011/ogl/tree/
+master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/
+hasii2011/ogl/tree/master) [![macOS](https://svgshare.com/i/ZjP.svg)](https://
+svgshare.com/i/ZjP.svg) [![forthebadge made-with-python](http://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
+) ð ð¨ ð¤ ð£ stands for Python UML Tool. This is the external
+graphical shapes module for Pyut that allows for external plugin development;
+This project depends on pyutmodel and wxPython ___ ## Developer Notes This
+project uses [buildlackey](https://github.com/hasii2011/buildlackey) for day to
+day development builds ___ Written by Humberto_A._Sanchez_II (C) 2023 ## Note
+For all kind of problems, requests, enhancements, bug reports, etc., please
+drop me an e-mail. ![Humberto's Modified Logo](https://
+raw.githubusercontent.com/wiki/hasii2011/gittodoistclone/images/
+SillyGitHub.png) I am concerned about GitHub's Copilot project I urge you to
+read about the [Give up GitHub](https://GiveUpGitHub.org) campaign from [the
+Software Freedom Conservancy](https://sfconservancy.org). While I do not
+advocate for all the issues listed there I do not like that a company like
+Microsoft may profit from open source projects. I continue to use GitHub
+because it offers the services I need for free. But, I continue to monitor
+their terms of service. Any use of this project's code by GitHub Copilot, past
+or present, is done without my permission. I do not consent to GitHub's use of
+this project's code in Copilot.
```

### Comparing `ogl-0.70.52/miniogl/AnchorPoint.py` & `ogl-0.85.0/miniogl/AnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/AttachmentSide.py` & `ogl-0.85.0/miniogl/AttachmentSide.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/Common.py` & `ogl-0.85.0/miniogl/Common.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/ControlPoint.py` & `ogl-0.85.0/miniogl/ControlPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/Diagram.py` & `ogl-0.85.0/miniogl/Diagram.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/DiagramFrame.py` & `ogl-0.85.0/miniogl/DiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/DlgDebugDiagramFrame.py` & `ogl-0.85.0/miniogl/DlgDebugDiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/LinePoint.py` & `ogl-0.85.0/miniogl/LinePoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/LineShape.py` & `ogl-0.85.0/miniogl/LineShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/LollipopLine.py` & `ogl-0.85.0/miniogl/LollipopLine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/MiniOglColorEnum.py` & `ogl-0.85.0/miniogl/MiniOglColorEnum.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/MiniOglPenStyle.py` & `ogl-0.85.0/miniogl/MiniOglPenStyle.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/PointShape.py` & `ogl-0.85.0/miniogl/PointShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/RectangleShape.py` & `ogl-0.85.0/miniogl/RectangleShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/RectangleShapeModel.py` & `ogl-0.85.0/miniogl/RectangleShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/RotatableShape.py` & `ogl-0.85.0/miniogl/RotatableShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/SelectAnchorPoint.py` & `ogl-0.85.0/miniogl/SelectAnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/Shape.py` & `ogl-0.85.0/miniogl/Shape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/ShapeEventHandler.py` & `ogl-0.85.0/miniogl/ShapeEventHandler.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/ShapeModel.py` & `ogl-0.85.0/miniogl/ShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/SizerShape.py` & `ogl-0.85.0/miniogl/SizerShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/TextShape.py` & `ogl-0.85.0/miniogl/TextShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/TextShapeModel.py` & `ogl-0.85.0/miniogl/TextShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/miniogl/VShapes.py` & `ogl-0.85.0/miniogl/VShapes.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglActor.py` & `ogl-0.85.0/ogl/OglActor.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglAggregation.py` & `ogl-0.85.0/ogl/OglAggregation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglAssociation.py` & `ogl-0.85.0/ogl/OglAssociation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from typing import Callable
 from typing import cast
 from typing import List
 from typing import NewType
 from typing import Tuple
 
 from logging import Logger
@@ -21,16 +22,16 @@
 from wx import FONTWEIGHT_NORMAL
 from wx import WHITE_BRUSH
 
 from wx import Font
 
 from pyutmodel.PyutLink import PyutLink
 
+from miniogl.Diagram import Diagram
 from miniogl.LineShape import Segments
-from miniogl.TextShape import TextShape
 
 from ogl.OglAssociationLabel import OglAssociationLabel
 from ogl.OglLink import OglLink
 from ogl.OglPosition import OglPosition
 
 from ogl.preferences.OglPreferences import OglPreferences
 
@@ -65,25 +66,22 @@
             dstPos:     Position of destination Override location of input destination
         """
         self.oglAssociationLogger: Logger         = getLogger(__name__)
         self._preferences:         OglPreferences = OglPreferences()
 
         super().__init__(srcShape, pyutLink, dstShape, srcPos=srcPos, dstPos=dstPos)
 
-        self._associationNameLabel:   OglAssociationLabel = OglAssociationLabel(text=self._link.name, oglPosition=OglPosition(x=0, y=0))
-        self._sourceCardinality:      OglAssociationLabel = OglAssociationLabel()
-        self._destinationCardinality: OglAssociationLabel = OglAssociationLabel()
-
         self._defaultFont: Font = Font(self._preferences.associationTextFontSize, FONTFAMILY_DEFAULT, FONTSTYLE_NORMAL, FONTWEIGHT_NORMAL)
 
-        self._associationNameTextShape:        TextShape = cast(TextShape, None)
-        self._sourceCardinalityTextShape:      TextShape = cast(TextShape, None)
-        self._destinationCardinalityTextShape: TextShape = cast(TextShape, None)
+        self._associationName:        OglAssociationLabel = cast(OglAssociationLabel, None)
+        self._sourceCardinality:      OglAssociationLabel = cast(OglAssociationLabel, None)
+        self._destinationCardinality: OglAssociationLabel = cast(OglAssociationLabel, None)
 
         self.SetDrawArrow(False)
+        self._labelsAdded: bool = False
 
     @property
     def pyutObject(self) -> PyutLink:
         """
         Override
         Returns:  The data model
         """
@@ -102,19 +100,19 @@
         self.sourceCardinality.text      = pyutLink.sourceCardinality
         self.destinationCardinality.text = pyutLink.destinationCardinality
 
         self.oglAssociationLogger.debug(f'{self.centerLabel=}')
 
     @property
     def centerLabel(self) -> OglAssociationLabel:
-        return self._associationNameLabel
+        return self._associationName
 
     @centerLabel.setter
     def centerLabel(self, newValue: OglAssociationLabel):
-        self._associationNameLabel = newValue
+        self._associationName = newValue
 
     @property
     def sourceCardinality(self) -> OglAssociationLabel:
         return self._sourceCardinality
 
     @sourceCardinality.setter
     def sourceCardinality(self, newValue: OglAssociationLabel):
@@ -124,44 +122,63 @@
     def destinationCardinality(self) -> OglAssociationLabel:
         return self._destinationCardinality
 
     @destinationCardinality.setter
     def destinationCardinality(self, newValue: OglAssociationLabel):
         self._destinationCardinality = newValue
 
+    def addLabelsToDiagram(self):
+        """
+        This method should only be called once.   It should only
+        be called once the OglAssociation shape itself has been
+        added to the diagram
+        """
+        assert self._labelsAdded is False, 'Developer error:  Labels should only be added once'
+        diagram: Diagram = self._diagram
+        if self.centerLabel is not None:
+            diagram.AddShape(self.centerLabel, withModelUpdate=True)
+        if self._sourceCardinality is not None:
+            diagram.AddShape(self.sourceCardinality, withModelUpdate=True)
+        if self._destinationCardinality is not None:
+            diagram.AddShape(self._destinationCardinality, withModelUpdate=True)
+
+        self._labelsAdded = True
+
     def Draw(self, dc: DC, withChildren: bool = True):
         """
         Called to draw the link content.
         We are going to draw all of our stuff, cardinality, Link name, etc.
 
         Args:
             dc:     Device context
             withChildren:   draw the children or not
         """
         OglLink.Draw(self, dc, withChildren)
+
+        if self._associationName is not None:
+            self._associationName.text = self._link.name
+
+        if self._sourceCardinality is not None:
+            self._sourceCardinality.text = self._link.sourceCardinality
+            self.oglAssociationLogger.debug(f'{self._sourceCardinality.GetPosition()=}')
+
+        if self._destinationCardinality is not None:
+            self._destinationCardinality.text = self._link.destinationCardinality
+            self.oglAssociationLogger.debug(f'{self._destinationCardinality.GetPosition()=}')
+
+    def createDefaultAssociationLabels(self):
         sp: Tuple[int, int] = self._srcAnchor.GetPosition()
         dp: Tuple[int, int] = self._dstAnchor.GetPosition()
+        oglDp: OglPosition = self._computeDestinationPosition(sp=OglPosition.tupleToOglPosition(sp), dp=OglPosition.tupleToOglPosition(dp))
 
         oglSp: OglPosition = OglPosition(x=sp[0], y=sp[1])
-        oglDp: OglPosition = self._computeDestinationPosition(sp=OglPosition.tupleToOglPosition(sp), dp=OglPosition.tupleToOglPosition(dp))
 
-        if self._link.name != '' and self._associationNameTextShape is None:
-            self._createAssociationName()
-        elif self._associationNameTextShape is not None:
-            self._updateAssociationState()
-
-        if self._link.sourceCardinality != '' and self._sourceCardinalityTextShape is None:
-            self._createSourceCardinality(sp=oglSp)
-        elif self._sourceCardinalityTextShape is not None:
-            self._updateSourceCardinalityState()
-
-        if self._link.destinationCardinality != '' and self._destinationCardinalityTextShape is None:
-            self._createDestinationCardinality(dp=oglDp)
-        elif self._destinationCardinalityTextShape is not None:
-            self._updateDestinationCardinalityState()
+        self._createAssociationName()
+        self._createSourceCardinality(sp=oglSp)
+        self._createDestinationCardinality(dp=oglDp)
 
     def drawDiamond(self, dc: DC, filled: bool = False):
         """
         Draw an arrow at the beginning of the line.
 
         Args:
             dc:         The device context
@@ -182,58 +199,34 @@
         dc.DrawPolygon(points)
         dc.SetBrush(WHITE_BRUSH)
 
     def _createAssociationName(self):
         """
         Create association name text shape;
         """
-        self._associationNameTextShape = self._createTextShapeFromAssociationLabel(associationLabel=self._associationNameLabel)
+        if self._link.name is None:
+            self._link.name = ''
+        self._associationName = self._createAssociationLabel(x=0, y=0, text=self._link.name, font=self._defaultFont)
 
     def _createSourceCardinality(self, sp: OglPosition):
 
-        self._sourceCardinalityTextShape = self._createTextShapeFromAssociationLabel(associationLabel=self._sourceCardinality)
+        if self._link.sourceCardinality is None:
+            self._link.sourceCardinality = ''
+        self._sourceCardinality = self._createAssociationLabel(x=sp.x, y=sp.y, text=self._link.sourceCardinality, font=self._defaultFont)
 
-        srcX, srcY = self._sourceCardinalityTextShape.ConvertCoordToRelative(x=sp.x, y=sp.y)
-        self._sourceCardinalityTextShape.SetRelativePosition(x=srcX, y=srcY)
-        self._sourceCardinality.oglPosition = OglPosition(x=srcX, y=srcY)
+        srcX, srcY = self._sourceCardinality.ConvertCoordToRelative(x=sp.x, y=sp.y)
+        self._sourceCardinality.SetRelativePosition(x=srcX, y=srcY)
 
     def _createDestinationCardinality(self, dp: OglPosition):
-        self._destinationCardinalityTextShape = self._createTextShapeFromAssociationLabel(associationLabel=self._destinationCardinality)
-
-        dstX, dstY = self._destinationCardinalityTextShape.ConvertCoordToRelative(x=dp.x, y=dp.y)
-        self._destinationCardinalityTextShape.SetRelativePosition(x=dstX, y=dstY)
-        self._destinationCardinality.oglPosition = OglPosition(x=dstX, y=dstY)
-
-    def _createTextShapeFromAssociationLabel(self, associationLabel: OglAssociationLabel) -> TextShape:
-
-        oglPosition:    OglPosition = associationLabel.oglPosition
-        labelTextShape: TextShape   = self._createTextShape(x=oglPosition.x, y=oglPosition.y, text=associationLabel.text, font=self._defaultFont)
+        if self._link.destinationCardinality is None:
+            self._link.destinationCardinality = ''
+        self._destinationCardinality = self._createAssociationLabel(x=dp.x, y=dp.y, text=self._link.destinationCardinality, font=self._defaultFont)
 
-        labelTextShape.draggable = True
-
-        return labelTextShape
-
-    def _updateAssociationState(self):
-
-        x, y = self._associationNameTextShape.GetRelativePosition()
-
-        self._associationNameLabel.oglPosition = OglPosition(x=x, y=y)
-        self._associationNameTextShape.text = self._link.name
-
-    def _updateSourceCardinalityState(self):
-        x, y = self._sourceCardinalityTextShape.GetRelativePosition()
-
-        self._sourceCardinality.oglPosition = OglPosition(x=x, y=y)
-        self._sourceCardinalityTextShape.text = self._link.sourceCardinality
-
-    def _updateDestinationCardinalityState(self):
-        x, y = self._sourceCardinalityTextShape.GetRelativePosition()
-
-        self.destinationCardinality.oglPosition = OglPosition(x=x, y=y)
-        self._destinationCardinalityTextShape.text = self._link.destinationCardinality
+        dstX, dstY = self._destinationCardinality.ConvertCoordToRelative(x=dp.x, y=dp.y)
+        self._destinationCardinality.SetRelativePosition(x=dstX, y=dstY)
 
     def _computeDestinationPosition(self, sp: OglPosition, dp: OglPosition) -> OglPosition:
 
         def computeDestination(dx, dy, linkLength) -> OglPosition:
             x: int = round((-20 * dx / linkLength + dx * 5 / linkLength) + dp.x)
             y: int = round((-20 * dy / linkLength - dy * 5 / linkLength) + dp.y)
 
@@ -266,14 +259,34 @@
                 f'{dy=} '
                 f'linkLength={linkLength:.2f} '
                 f'{oglPosition=}'
             )
             self.oglAssociationLogger.debug(info)
         return oglPosition
 
+    def _createAssociationLabel(self, x: int, y: int, text: str, font: Font = None) -> OglAssociationLabel:
+        """
+        Create an association label and add it to the diagram.
+
+        Args:
+            x,: position of the text, relative to the origin of the shape
+            y : position of the text, relative to the origin of the shape
+            text: text to add
+            font: font to use
+
+        Returns:  AssociationLabel : the created shape
+        """
+        oglAssociationLabel: OglAssociationLabel = OglAssociationLabel(x, y, text, parent=self, font=font)
+        if self._diagram is not None:
+            self._diagram.AddShape(oglAssociationLabel)
+        self.oglAssociationLogger.info(f'_createAssociationLabel - {oglAssociationLabel=} added at {x=} {y=}')
+
+        oglAssociationLabel.draggable = True
+        return oglAssociationLabel
+
     @staticmethod
     def calculateDiamondPoints(lineSegments: Segments) -> DiamondPoints:
         """
         Made static so that we can unit test it;  Please the only instance variables needed
         are passed in
 
         Args:
```

### Comparing `ogl-0.70.52/ogl/OglClass.py` & `ogl-0.85.0/ogl/OglClass.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglComposition.py` & `ogl-0.85.0/ogl/OglComposition.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglConstants.py` & `ogl-0.85.0/ogl/OglConstants.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglDimensions.py` & `ogl-0.85.0/ogl/OglDimensions.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglInheritance.py` & `ogl-0.85.0/ogl/OglInheritance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglInterface.py` & `ogl-0.85.0/ogl/OglInterface.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglInterface2.py` & `ogl-0.85.0/ogl/OglInterface2.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglLink.py` & `ogl-0.85.0/ogl/OglLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglLinkFactory.py` & `ogl-0.85.0/ogl/OglLinkFactory.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglNote.py` & `ogl-0.85.0/ogl/OglNote.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglNoteLink.py` & `ogl-0.85.0/ogl/OglNoteLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglObject.py` & `ogl-0.85.0/ogl/OglObject.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglText.py` & `ogl-0.85.0/ogl/OglText.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglUseCase.py` & `ogl-0.85.0/ogl/OglUseCase.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/OglUtils.py` & `ogl-0.85.0/ogl/OglUtils.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/events/IOglEventEngine.py` & `ogl-0.85.0/ogl/events/IOglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/events/OglEventEngine.py` & `ogl-0.85.0/ogl/events/OglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/events/OglEvents.py` & `ogl-0.85.0/ogl/events/OglEvents.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/preferences/OglPreferences.py` & `ogl-0.85.0/ogl/preferences/OglPreferences.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/resources/img/Display.py` & `ogl-0.85.0/ogl/resources/img/Display.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/resources/img/DoNotDisplay.py` & `ogl-0.85.0/ogl/resources/img/DoNotDisplay.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/resources/img/UnSpecified.py` & `ogl-0.85.0/ogl/resources/img/UnSpecified.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/resources/img/textdetails/DecreaseTextSize.py` & `ogl-0.85.0/ogl/resources/img/textdetails/DecreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/resources/img/textdetails/IncreaseTextSize.py` & `ogl-0.85.0/ogl/resources/img/textdetails/IncreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/sd/OglInstanceName.py` & `ogl-0.85.0/ogl/sd/OglInstanceName.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/sd/OglSDInstance.py` & `ogl-0.85.0/ogl/sd/OglSDInstance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/sd/OglSDMessage.py` & `ogl-0.85.0/ogl/sd/OglSDMessage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/BaseOglPreferencesPage.py` & `ogl-0.85.0/ogl/ui/BaseOglPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/DefaultValuesPreferencesPage.py` & `ogl-0.85.0/ogl/ui/DefaultValuesPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/DiagramPreferencesPage.py` & `ogl-0.85.0/ogl/ui/DiagramPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/valuecontrols/AssociationAttributesControl.py` & `ogl-0.85.0/ogl/ui/valuecontrols/AssociationAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/valuecontrols/ClassAttributesControl.py` & `ogl-0.85.0/ogl/ui/valuecontrols/ClassAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/valuecontrols/DefaultNamesControl.py` & `ogl-0.85.0/ogl/ui/valuecontrols/DefaultNamesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/valuecontrols/NoteAttributesControl.py` & `ogl-0.85.0/ogl/ui/valuecontrols/NoteAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/valuecontrols/SDAttributesControl.py` & `ogl-0.85.0/ogl/ui/valuecontrols/SDAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl/ui/valuecontrols/TextAttributesControl.py` & `ogl-0.85.0/ogl/ui/valuecontrols/TextAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/ogl.egg-info/SOURCES.txt` & `ogl-0.85.0/ogl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogl-0.70.52/setup.py` & `ogl-0.85.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,17 @@
     version=oglVersion,
     author='Humberto A. Sanchez II',
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='External Pyut Graphical Shapes',
     long_description=README,
-    long_description_content_type="text/markdown",
-    url="https://github.com/hasii2011/ogl",
+    long_description_content_type='text/markdown',
+    license=LICENSE,
+    url='https://github.com/hasii2011/ogl',
     package_data={
         'miniogl':              ['py.typed'],
         'ogl':                  ['py.typed'],
         'ogl.events':           ['py.typed'],
         'ogl.preferences':      ['py.typed'],
         'ogl.resources':        ['py.typed'],
         'ogl.resources.img':             ['py.typed'],
```

