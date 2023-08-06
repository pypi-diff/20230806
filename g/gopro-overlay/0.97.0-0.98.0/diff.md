# Comparing `tmp/gopro-overlay-0.97.0.tar.gz` & `tmp/gopro-overlay-0.98.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopro-overlay-0.97.0.tar", last modified: Mon May 29 08:59:07 2023, max compression
+gzip compressed data, was "gopro-overlay-0.98.0.tar", last modified: Mon May 29 13:54:54 2023, max compression
```

## Comparing `gopro-overlay-0.97.0.tar` & `gopro-overlay-0.98.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.038049 gopro-overlay-0.97.0/
--rw-rw-r--   0 richja    (1000) richja    (1000)    35691 2023-05-22 13:30:42.000000 gopro-overlay-0.97.0/LICENSE.md
--rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.97.0/MANIFEST.in
--rw-rw-r--   0 richja    (1000) richja    (1000)    12013 2023-05-29 08:59:07.038049 gopro-overlay-0.97.0/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)    11220 2023-05-29 08:57:30.000000 gopro-overlay-0.97.0/README.md
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.026049 gopro-overlay-0.97.0/bin/
--rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.97.0/bin/gopro-contrib-data-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.97.0/bin/gopro-cut.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    15098 2023-05-29 08:34:54.000000 gopro-overlay-0.97.0/bin/gopro-dashboard.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/bin/gopro-debug.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.97.0/bin/gopro-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/bin/gopro-join.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)     5603 2023-05-29 08:34:54.000000 gopro-overlay-0.97.0/bin/gopro-layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3702 2023-05-23 10:54:25.000000 gopro-overlay-0.97.0/bin/gopro-rename.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/bin/gopro-to-csv.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/bin/gopro-to-gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.030049 gopro-overlay-0.97.0/gopro_overlay/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.97.0/gopro_overlay/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-29 08:55:36.000000 gopro-overlay-0.97.0/gopro_overlay/__version__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     7063 2023-05-22 08:55:54.000000 gopro-overlay-0.97.0/gopro_overlay/arguments.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5447 2023-05-08 10:30:40.000000 gopro-overlay-0.97.0/gopro_overlay/buffering.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.97.0/gopro_overlay/common.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      846 2023-05-27 14:18:06.000000 gopro-overlay-0.97.0/gopro_overlay/config.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/counter.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/date_overlap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.97.0/gopro_overlay/dimensions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/entry.py
--rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.97.0/gopro_overlay/exceptions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.97.0/gopro_overlay/execution.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/fake.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10025 2023-05-22 09:32:45.000000 gopro-overlay-0.97.0/gopro_overlay/ffmpeg.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1206 2023-05-27 14:12:20.000000 gopro-overlay-0.97.0/gopro_overlay/ffmpeg_profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1958 2023-05-26 14:53:43.000000 gopro-overlay-0.97.0/gopro_overlay/filenaming.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.97.0/gopro_overlay/fit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.97.0/gopro_overlay/font.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/framemeta.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/framemeta_gpx.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.97.0/gopro_overlay/functional.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6859 2023-05-29 08:34:54.000000 gopro-overlay-0.97.0/gopro_overlay/geo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.97.0/gopro_overlay/geo_render.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-05-23 10:54:25.000000 gopro-overlay-0.97.0/gopro_overlay/geocode.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_calculate.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_cori.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_debug.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_grav.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_xyz.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.034049 gopro-overlay-0.97.0/gopro_overlay/icons/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.97.0/gopro_overlay/icons/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.97.0/gopro_overlay/icons/bicycle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.97.0/gopro_overlay/icons/car.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/faq.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/forbidden.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gauge-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gauge.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_2d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_3d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_none.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_unknown.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.97.0/gopro_overlay/icons/heartbeat.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.97.0/gopro_overlay/icons/ice-cream-van.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.97.0/gopro_overlay/icons/mountain-range.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.97.0/gopro_overlay/icons/mountain.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.97.0/gopro_overlay/icons/power.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.97.0/gopro_overlay/icons/ruler.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.97.0/gopro_overlay/icons/slope-triangle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.97.0/gopro_overlay/icons/slope.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.97.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/thermometer-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.97.0/gopro_overlay/icons/thermometer.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.97.0/gopro_overlay/icons/user.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.97.0/gopro_overlay/icons/van-black-side-view.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/journey.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.97.0/gopro_overlay/layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layout_components.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layout_xml.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layout_xml_attribute.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layout_xml_cairo.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.034049 gopro-overlay-0.97.0/gopro_overlay/layouts/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/default-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/default-2704x1520.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/default-3840x2160.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/example-2.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/example.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/power-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/log.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.97.0/gopro_overlay/models.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.97.0/gopro_overlay/parsing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/point.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.97.0/gopro_overlay/privacy.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.97.0/gopro_overlay/progress_frames.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/rdp.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/smoothing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/timeseries.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/timeseries_process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.97.0/gopro_overlay/timeunits.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/timing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.97.0/gopro_overlay/units.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.034049 gopro-overlay-0.97.0/gopro_overlay/widgets/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/asi.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/bar.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.038049 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/angle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/annotation.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/background.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/bordered.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/box.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/cairo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/cap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/circuit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/colour.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/ellipse.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/face.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/gauge_marker.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/gauge_round_254.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/line.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/needle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/reading.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/scale.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/tick.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/chart.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/compass.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/compass_arrow.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/gradient_bar.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/info.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/map.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/text.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8038 2023-05-06 09:06:40.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/widgets.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/widgets_experimental.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.030049 gopro-overlay-0.97.0/gopro_overlay.egg-info/
--rw-rw-r--   0 richja    (1000) richja    (1000)    12013 2023-05-29 08:59:06.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)     4216 2023-05-29 08:59:07.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/SOURCES.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-29 08:59:06.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/dependency_links.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-29 08:59:06.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/requires.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-29 08:59:06.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/top_level.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-29 08:59:07.038049 gopro-overlay-0.97.0/setup.cfg
--rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-29 08:55:36.000000 gopro-overlay-0.97.0/setup.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 13:54:54.969264 gopro-overlay-0.98.0/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    35691 2023-05-22 13:30:42.000000 gopro-overlay-0.98.0/LICENSE.md
+-rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.98.0/MANIFEST.in
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12140 2023-05-29 13:54:54.969264 gopro-overlay-0.98.0/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11347 2023-05-29 13:54:28.000000 gopro-overlay-0.98.0/README.md
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 13:54:54.957265 gopro-overlay-0.98.0/bin/
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.98.0/bin/gopro-contrib-data-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.98.0/bin/gopro-cut.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15116 2023-05-29 11:59:42.000000 gopro-overlay-0.98.0/bin/gopro-dashboard.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/bin/gopro-debug.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.98.0/bin/gopro-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/bin/gopro-join.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)     5603 2023-05-29 13:43:14.000000 gopro-overlay-0.98.0/bin/gopro-layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3702 2023-05-23 10:54:25.000000 gopro-overlay-0.98.0/bin/gopro-rename.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/bin/gopro-to-csv.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/bin/gopro-to-gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 13:54:54.961264 gopro-overlay-0.98.0/gopro_overlay/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.98.0/gopro_overlay/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-29 13:53:11.000000 gopro-overlay-0.98.0/gopro_overlay/__version__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7500 2023-05-29 13:51:53.000000 gopro-overlay-0.98.0/gopro_overlay/arguments.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5947 2023-05-29 13:36:09.000000 gopro-overlay-0.98.0/gopro_overlay/buffering.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.98.0/gopro_overlay/common.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      846 2023-05-29 09:00:59.000000 gopro-overlay-0.98.0/gopro_overlay/config.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/counter.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/date_overlap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.98.0/gopro_overlay/dimensions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/entry.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.98.0/gopro_overlay/exceptions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.98.0/gopro_overlay/execution.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/fake.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10025 2023-05-22 09:32:45.000000 gopro-overlay-0.98.0/gopro_overlay/ffmpeg.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1206 2023-05-29 09:00:59.000000 gopro-overlay-0.98.0/gopro_overlay/ffmpeg_profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1958 2023-05-26 14:53:43.000000 gopro-overlay-0.98.0/gopro_overlay/filenaming.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.98.0/gopro_overlay/fit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.98.0/gopro_overlay/font.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/framemeta.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/framemeta_gpx.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.98.0/gopro_overlay/functional.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6892 2023-05-29 09:13:04.000000 gopro-overlay-0.98.0/gopro_overlay/geo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.98.0/gopro_overlay/geo_render.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-05-23 10:54:25.000000 gopro-overlay-0.98.0/gopro_overlay/geocode.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.98.0/gopro_overlay/gpmd.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/gpmd_calculate.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_cori.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_debug.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_grav.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_xyz.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 13:54:54.965264 gopro-overlay-0.98.0/gopro_overlay/icons/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.98.0/gopro_overlay/icons/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.98.0/gopro_overlay/icons/bicycle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.98.0/gopro_overlay/icons/car.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/icons/faq.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/icons/forbidden.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.98.0/gopro_overlay/icons/gauge-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.98.0/gopro_overlay/icons/gauge.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/icons/gps_lock_2d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/icons/gps_lock_3d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/icons/gps_lock_none.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/icons/gps_lock_unknown.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.98.0/gopro_overlay/icons/heartbeat.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.98.0/gopro_overlay/icons/ice-cream-van.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.98.0/gopro_overlay/icons/mountain-range.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.98.0/gopro_overlay/icons/mountain.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.98.0/gopro_overlay/icons/power.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.98.0/gopro_overlay/icons/ruler.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.98.0/gopro_overlay/icons/slope-triangle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.98.0/gopro_overlay/icons/slope.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.98.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.98.0/gopro_overlay/icons/thermometer-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.98.0/gopro_overlay/icons/thermometer.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.98.0/gopro_overlay/icons/user.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.98.0/gopro_overlay/icons/van-black-side-view.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/journey.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.98.0/gopro_overlay/layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layout_components.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layout_xml.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layout_xml_attribute.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layout_xml_cairo.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 13:54:54.965264 gopro-overlay-0.98.0/gopro_overlay/layouts/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.98.0/gopro_overlay/layouts/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layouts/default-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layouts/default-2704x1520.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layouts/default-3840x2160.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layouts/example-2.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layouts/example.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/layouts/power-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/log.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.98.0/gopro_overlay/models.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.98.0/gopro_overlay/parsing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/point.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.98.0/gopro_overlay/privacy.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.98.0/gopro_overlay/progress_frames.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/rdp.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/smoothing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/timeseries.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/timeseries_process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.98.0/gopro_overlay/timeunits.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/timing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.98.0/gopro_overlay/units.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 13:54:54.969264 gopro-overlay-0.98.0/gopro_overlay/widgets/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/asi.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/bar.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 13:54:54.969264 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/angle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/annotation.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/background.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/bordered.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/box.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/cairo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/cap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/circuit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/colour.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/ellipse.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/face.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/gauge_marker.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/gauge_round_254.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/line.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/needle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/reading.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/scale.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/tick.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/chart.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/compass.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/compass_arrow.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/gradient_bar.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/info.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/map.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/text.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8111 2023-05-29 11:59:42.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/widgets.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.98.0/gopro_overlay/widgets/widgets_experimental.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 13:54:54.965264 gopro-overlay-0.98.0/gopro_overlay.egg-info/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12140 2023-05-29 13:54:54.000000 gopro-overlay-0.98.0/gopro_overlay.egg-info/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4216 2023-05-29 13:54:54.000000 gopro-overlay-0.98.0/gopro_overlay.egg-info/SOURCES.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-29 13:54:54.000000 gopro-overlay-0.98.0/gopro_overlay.egg-info/dependency_links.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-29 13:54:54.000000 gopro-overlay-0.98.0/gopro_overlay.egg-info/requires.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-29 13:54:54.000000 gopro-overlay-0.98.0/gopro_overlay.egg-info/top_level.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-29 13:54:54.969264 gopro-overlay-0.98.0/setup.cfg
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-29 13:53:11.000000 gopro-overlay-0.98.0/setup.py
```

### Comparing `gopro-overlay-0.97.0/LICENSE.md` & `gopro-overlay-0.98.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/PKG-INFO` & `gopro-overlay-0.98.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.97.0
+Version: 0.98.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Classifier: Development Status :: 5 - Production/Stable
@@ -234,14 +234,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.98.0 [Feature] Add configurable background colour with `--bg rgba` thanks to @mishuha in discussion #120 for the concept. 
 - 0.97.0 [Feature] Add new map style "local" - which will connect to a tileserver running locally on port 8000. This may be useful if you want to use a completely custom map - like a hand drawn one.
   - For more details see: https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to @mattghub1 for the concept. 
 - 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.97.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.98.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -100,45 +100,47 @@
 Â© [Thunderforest](http://www.thunderforest.com/) ## References https://
 github.com/juanmcasillas/gopro2gpx https://github.com/JuanIrache/gopro-
 telemetry https://github.com/gopro/gpmf-parser https://coderunner.io/how-to-
 compress-gopro-movies-and-keep-metadata/ ## Other Related Software https://
 github.com/progweb/gpx2video https://github.com/JuanIrache/gopro-telemetry ##
 Latest Changes If you find any issues with new releases, please discuss in
 [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/
-discussions) - 0.97.0 [Feature] Add new map style "local" - which will connect
-to a tileserver running locally on port 8000. This may be useful if you want to
-use a completely custom map - like a hand drawn one. - For more details see:
-https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to
-@mattghub1 for the concept. - 0.96.0 [Feature] Hopefully add support for older
-gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-
-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for
-raising and some example code. - 0.95.0 [Feature] Add api key support for
-geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
-issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
-[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
-Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
-now possible. It takes a bit of work, but now can render at 12x realtime. See
-[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
-Remove support for `--output-size` as it didn't really work properly anyway. -
-0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
-much faster rendering, but may not work on all architectures. Speed
-improvements highly dependent on `ffmpeg` performance. Likely much faster when
-using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
-items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
-patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
-quickly. - [Change] Map rendering caches tile images more efficiently, so draws
-more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
-A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
-[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
-Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
-Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
-instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
-gauge-marker` - a nice clean gauge component, with a marker for the current
-value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
-06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
-attributes in layout files. This may cause some custom layouts to break! - But
-they wouldn't have been working as intended. - [Change/Breaking] Change some
-`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
-Change some `cairo-circuit-map` attribute names, aiming for standardisation
-Older changes are in [CHANGELOG.md](CHANGELOG.md)
+discussions) - 0.98.0 [Feature] Add configurable background colour with `--bg
+rgba` thanks to @mishuha in discussion #120 for the concept. - 0.97.0 [Feature]
+Add new map style "local" - which will connect to a tileserver running locally
+on port 8000. This may be useful if you want to use a completely custom map -
+like a hand drawn one. - For more details see: https://github.com/time4tea/
+gopro-dashboard-overlay/discussions/132 Thanks to @mattghub1 for the concept. -
+0.96.0 [Feature] Hopefully add support for older gopro files when joining.
+[#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks
+[@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example
+code. - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://
+github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha]
+(https://github.com/mishuha) for raising. - 0.94.0 [Change] Update docker image
+to python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully gpu* decoding/
+overlay/encoding. Huge performance increase now possible. It takes a bit of
+work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md]
+(docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove support for `--output-size`
+as it didn't really work properly anyway. - 0.92.0 [Feature] `--double-buffer`
+- EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not
+work on all architectures. Speed improvements highly dependent on `ffmpeg`
+performance. Likely much faster when using `--generate overlay`. Feedback
+welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location.
+[#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks
+[@patkoscsaba](https://github.com/patkoscsaba) for raising. - 0.90.0 [Change]
+`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
+tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
+component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
+docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
+cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
+were no locked GPS points in the movie. - Thanks [@shahargli](https://
+github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
+discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
+colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
+gauge component, with a marker for the current value.. See docs [docs/xml/
+examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
+0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
+files. This may cause some custom layouts to break! - But they wouldn't have
+been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
+names, aiming for standardisation - [Change/Breaking] Change some `cairo-
+circuit-map` attribute names, aiming for standardisation Older changes are in
+[CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.97.0/README.md` & `gopro-overlay-0.98.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -213,14 +213,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.98.0 [Feature] Add configurable background colour with `--bg rgba` thanks to @mishuha in discussion #120 for the concept. 
 - 0.97.0 [Feature] Add new map style "local" - which will connect to a tileserver running locally on port 8000. This may be useful if you want to use a completely custom map - like a hand drawn one.
   - For more details see: https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to @mattghub1 for the concept. 
 - 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway.
```

#### html2text {}

```diff
@@ -89,46 +89,47 @@
 copyright) Some Maps Â© [Thunderforest](http://www.thunderforest.com/) ##
 References https://github.com/juanmcasillas/gopro2gpx https://github.com/
 JuanIrache/gopro-telemetry https://github.com/gopro/gpmf-parser https://
 coderunner.io/how-to-compress-gopro-movies-and-keep-metadata/ ## Other Related
 Software https://github.com/progweb/gpx2video https://github.com/JuanIrache/
 gopro-telemetry ## Latest Changes If you find any issues with new releases,
 please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-
-dashboard-overlay/discussions) - 0.97.0 [Feature] Add new map style "local" -
-which will connect to a tileserver running locally on port 8000. This may be
-useful if you want to use a completely custom map - like a hand drawn one. -
-For more details see: https://github.com/time4tea/gopro-dashboard-overlay/
-discussions/132 Thanks to @mattghub1 for the concept. - 0.96.0 [Feature]
-Hopefully add support for older gopro files when joining. [#129](https://
-github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle]
-(https://github.com/FFMbyBicycle) for raising and some example code. - 0.95.0
-[Feature] Add api key support for geocode.xyz - [#117](https://github.com/
-time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://
-github.com/mishuha) for raising. - 0.94.0 [Change] Update docker image to
-python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully gpu* decoding/
-overlay/encoding. Huge performance increase now possible. It takes a bit of
-work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md]
-(docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove support for `--output-size`
-as it didn't really work properly anyway. - 0.92.0 [Feature] `--double-buffer`
-- EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not
-work on all architectures. Speed improvements highly dependent on `ffmpeg`
-performance. Likely much faster when using `--generate overlay`. Feedback
-welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location.
-[#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks
-[@patkoscsaba](https://github.com/patkoscsaba) for raising. - 0.90.0 [Change]
-`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
-tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
-component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
-docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
-cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
-were no locked GPS points in the movie. - Thanks [@shahargli](https://
-github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
-discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
-colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
-gauge component, with a marker for the current value.. See docs [docs/xml/
-examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
-0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
-files. This may cause some custom layouts to break! - But they wouldn't have
-been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
-names, aiming for standardisation - [Change/Breaking] Change some `cairo-
-circuit-map` attribute names, aiming for standardisation Older changes are in
-[CHANGELOG.md](CHANGELOG.md)
+dashboard-overlay/discussions) - 0.98.0 [Feature] Add configurable background
+colour with `--bg rgba` thanks to @mishuha in discussion #120 for the concept.
+- 0.97.0 [Feature] Add new map style "local" - which will connect to a
+tileserver running locally on port 8000. This may be useful if you want to use
+a completely custom map - like a hand drawn one. - For more details see: https:
+//github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to
+@mattghub1 for the concept. - 0.96.0 [Feature] Hopefully add support for older
+gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for
+raising and some example code. - 0.95.0 [Feature] Add api key support for
+geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
+issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
+[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
+Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
+now possible. It takes a bit of work, but now can render at 12x realtime. See
+[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
+Remove support for `--output-size` as it didn't really work properly anyway. -
+0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
+much faster rendering, but may not work on all architectures. Speed
+improvements highly dependent on `ffmpeg` performance. Likely much faster when
+using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
+items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
+dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
+patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
+quickly. - [Change] Map rendering caches tile images more efficiently, so draws
+more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
+A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
+round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
+[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
+Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
+Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
+instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
+gauge-marker` - a nice clean gauge component, with a marker for the current
+value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
+06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
+attributes in layout files. This may cause some custom layouts to break! - But
+they wouldn't have been working as intended. - [Change/Breaking] Change some
+`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
+Change some `cairo-circuit-map` attribute names, aiming for standardisation
+Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.97.0/bin/gopro-contrib-data-extract.py` & `gopro-overlay-0.98.0/bin/gopro-contrib-data-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/bin/gopro-cut.py` & `gopro-overlay-0.98.0/bin/gopro-cut.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/bin/gopro-dashboard.py` & `gopro-overlay-0.98.0/bin/gopro-dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,17 +324,17 @@
             overlay = Overlay(framemeta=frame_meta, create_widgets=layout_creator)
 
             try:
                 with ffmpeg.generate() as writer:
 
                     if args.double_buffer:
                         log("*** NOTE: Double Buffer mode is experimental. It is believed to work fine on Linux. Please raise issues if you see it working or not-working. Thanks ***")
-                        buffer = DoubleBuffer(dimensions, writer)
+                        buffer = DoubleBuffer(dimensions, args.bg, writer)
                     else:
-                        buffer = SingleBuffer(dimensions, writer)
+                        buffer = SingleBuffer(dimensions, args.bg, writer)
 
                     with buffer:
                         for index, dt in enumerate(stepper.steps()):
                             progress.update(index)
                             draw_timer.time(lambda: buffer.draw(lambda frame: overlay.draw(dt, frame)))
 
                 log("Finished drawing frames. waiting for ffmpeg to catch up")
```

### Comparing `gopro-overlay-0.97.0/bin/gopro-debug.py` & `gopro-overlay-0.98.0/bin/gopro-debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/bin/gopro-extract.py` & `gopro-overlay-0.98.0/bin/gopro-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/bin/gopro-join.py` & `gopro-overlay-0.98.0/bin/gopro-join.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/bin/gopro-layout.py` & `gopro-overlay-0.98.0/bin/gopro-layout.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/bin/gopro-rename.py` & `gopro-overlay-0.98.0/bin/gopro-rename.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/bin/gopro-to-csv.py` & `gopro-overlay-0.98.0/bin/gopro-to-csv.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/bin/gopro-to-gpx.py` & `gopro-overlay-0.98.0/bin/gopro-to-gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/arguments.py` & `gopro-overlay-0.98.0/gopro_overlay/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,22 @@
         if len(bbox) != 4:
             raise ValueError("Bounding Box requires 4 values - minlon,minlat,maxlon,maxlat")
         extent_min = Point(lon=bbox[0], lat=bbox[1])
         extent_max = Point(lon=bbox[2], lat=bbox[3])
         setattr(namespace, self.dest, BoundingBox(min=extent_min, max=extent_max))
 
 
+class ColourArgs(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        colour = tuple(map(int, values.split(",")))
+        if len(colour) != 4:
+            raise ValueError("Colour Requires 4 values - r,g,b,a")
+        setattr(namespace, self.dest, colour)
+
+
 default_config_location = pathlib.Path.home() / ".gopro-graphics"
 
 
 def gopro_dashboard_arguments(args=None):
     parser = argparse.ArgumentParser(
         description="Overlay gadgets on to GoPro MP4",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
@@ -46,14 +54,16 @@
     parser.add_argument("--privacy", help="Set privacy zone (lat,lon,km)")
 
     parser.add_argument("--generate", choices=["default", "overlay", "none"], default="default",
                         help="Type of output to generate")
     parser.add_argument("--overlay-size",
                         help="<XxY> e.g. 1920x1080 Force size of overlay. "
                              "Use if video differs from supported bundled overlay sizes (1920x1080, 3840x2160), Required if --use-gpx-only")
+    parser.add_argument("--bg", help="Background Colour - R,G,B,A - each 0-255, no spaces!", default=(0, 0, 0, 0), action=ColourArgs)
+
     parser.add_argument("--profile",
                         help="Use ffmpeg options profile <name> from ~/gopro-graphics/ffmpeg-profiles.json")
 
     parser.add_argument("--config-dir", help="Location of config files (api keys, profiles, ...)", type=pathlib.Path,
                         default=default_config_location)
     parser.add_argument("--cache-dir", help="Location of caches (map tiles, ...)", type=pathlib.Path,
                         default=default_config_location)
```

### Comparing `gopro-overlay-0.97.0/gopro_overlay/buffering.py` & `gopro-overlay-0.98.0/gopro_overlay/buffering.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import ctypes
 import io
 import multiprocessing
 import os
 from io import BufferedWriter
 from multiprocessing.shared_memory import SharedMemory
-from typing import Callable, Any
+from typing import Callable, Any, Tuple
 
-from PIL import Image
+from PIL import Image, ImageDraw
 
 from gopro_overlay.dimensions import Dimension
 from gopro_overlay.widgets.widgets import SimpleFrameSupplier
 
 
 class DrawBuffer:
     def draw(self, f: Callable[[Image.Image], Any]):
         raise NotImplementedError()
 
 
 class SingleBuffer(DrawBuffer):
-    def __init__(self, size: Dimension, writer: BufferedWriter):
-        self.supplier = SimpleFrameSupplier(size)
+    def __init__(self, size: Dimension, background: Tuple, writer: BufferedWriter):
+        self.supplier = SimpleFrameSupplier(size, background)
         self.writer = writer
 
     def draw(self, f: Callable[[Image.Image], Any]):
         image = self.supplier.drawing_frame()
         f(image)
         self.writer.write(image.tobytes())
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
+
 class SerialisedWriter(io.BufferedWriter):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.lock = multiprocessing.Lock()
 
     def write(self, __buffer) -> int:
         with self.lock:
@@ -51,53 +52,54 @@
 
 def raw_image(dimensions: Dimension, buffer) -> Image.Image:
     image = Image.frombuffer("RGBA", (dimensions.x, dimensions.y), buffer, "raw", "RGBA", 0, 1)
     image.readonly = 0
     return image
 
 
-def clear_buffer(buffer, l):
-    ctypes.memset(ctypes.byref(buffer), 0x00, l)
-
-
 class Frame:
-    def __init__(self, shm: SharedMemory, quit: multiprocessing.Value, size: Dimension, count: int):
+    def __init__(self, shm: SharedMemory, quit: multiprocessing.Value, size: Dimension, background: Tuple, count: int):
         self.shm = shm
         self.size = size
         self.count = count
         self.quit = quit
-
+        self.background = background
         self.buffer_size = (size.x * size.y * 4)
 
         self.memory = shm.buf[self.buffer_size * self.count:self.buffer_size * (self.count + 1)]
 
         self.image = raw_image(size, self.memory)
+        self.im_draw = ImageDraw.ImageDraw(self.image)
 
         self.active = multiprocessing.Lock()
         self.can_draw = multiprocessing.Condition(self.active)
         self.can_write = multiprocessing.Condition(self.active)
 
         self.ctypes_buffer = ctypes.c_char.from_buffer(self.memory)
 
         self.drawn_frame_number = multiprocessing.Value(ctypes.c_long)
         self.drawn_frame_number.value = -1
 
         self.written_frame_number = multiprocessing.Value(ctypes.c_long)
         self.written_frame_number.value = -1
 
+        self.clear()
+
     def wake(self):
         with self.can_draw:
             self.can_draw.notify()
         with self.can_write:
             self.can_write.notify()
 
     def clear(self):
-        clear_buffer(self.ctypes_buffer, self.buffer_size)
+        ctypes.memset(ctypes.byref(self.ctypes_buffer), 0x00, self.buffer_size)
+        if self.background != (0, 0, 0, 0):
+            self.im_draw.rectangle((0, 0, self.size.x, self.size.y), self.background)
 
-    def draw(self, f: Callable[[Image.Image], None]):
+    def draw(self, f: Callable[[Image.Image], None]) -> bool:
         with self.can_draw:
             while not self.can_draw.wait_for(predicate=lambda: self.quit.value == 1 or self.written_frame_number.value == self.drawn_frame_number.value, timeout=cond_timeout):
                 pass
 
         if self.drawn_frame_number.value == self.written_frame_number.value:
             f(self.image)
 
@@ -105,14 +107,20 @@
         with self.can_write:
             self.can_write.notify()
 
         if self.quit.value == 1:
             return False
         return True
 
+    def copy(self) -> Image.Image:
+        """Return a copy of this image, not from shared memory"""
+        c = Image.new("RGBA", self.size.tuple())
+        c.paste(self.image)
+        return c
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.wake()
         del self.ctypes_buffer
         self.image.close()
@@ -139,23 +147,23 @@
 def p_writer(frame: Frame, writer: io.BytesIO):
     while True:
         if not frame.write(writer):
             break
 
 
 class DoubleBuffer(DrawBuffer):
-    def __init__(self, size: Dimension, writer: BufferedWriter):
+    def __init__(self, size: Dimension, background: Tuple, writer: BufferedWriter):
         shm_name = f"gopro.{os.getpid()}"
         buffer_size = (size.x * size.y * 4)
         shm_size = buffer_size * 2
         self.shm = SharedMemory(create=True, name=shm_name, size=shm_size)
         self.quit = multiprocessing.Value(ctypes.c_int)
 
-        self.frame0 = Frame(self.shm, self.quit, size, 0)
-        self.frame1 = Frame(self.shm, self.quit, size, 1)
+        self.frame0 = Frame(self.shm, self.quit, size, background, 0)
+        self.frame1 = Frame(self.shm, self.quit, size, background, 1)
 
         writer = SerialisedWriter(writer)
 
         self.worker1 = multiprocessing.Process(target=p_writer, args=(self.frame0, writer))
         self.worker1.start()
         self.worker2 = multiprocessing.Process(target=p_writer, args=(self.frame1, writer))
         self.worker2.start()
```

### Comparing `gopro-overlay-0.97.0/gopro_overlay/common.py` & `gopro-overlay-0.98.0/gopro_overlay/common.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/config.py` & `gopro-overlay-0.98.0/gopro_overlay/config.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/dimensions.py` & `gopro-overlay-0.98.0/gopro_overlay/dimensions.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/entry.py` & `gopro-overlay-0.98.0/gopro_overlay/entry.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/execution.py` & `gopro-overlay-0.98.0/gopro_overlay/execution.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/fake.py` & `gopro-overlay-0.98.0/gopro_overlay/fake.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/ffmpeg.py` & `gopro-overlay-0.98.0/gopro_overlay/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/ffmpeg_profile.py` & `gopro-overlay-0.98.0/gopro_overlay/ffmpeg_profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/filenaming.py` & `gopro-overlay-0.98.0/gopro_overlay/filenaming.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/fit.py` & `gopro-overlay-0.98.0/gopro_overlay/fit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/framemeta.py` & `gopro-overlay-0.98.0/gopro_overlay/framemeta.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/framemeta_gpx.py` & `gopro-overlay-0.98.0/gopro_overlay/framemeta_gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/geo.py` & `gopro-overlay-0.98.0/gopro_overlay/geo.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         "api-key-ref": "thunderforest",
         "limit": 2,
     }
 
 
 def local_attrs(style):
     return {
+        "attribution": "Custom",
         "name": "Local",
         "url": "http://localhost:8000/{z}/{x}/{y}.{ext}",
         "cache": False,
         "limit": 2
     }
```

### Comparing `gopro-overlay-0.97.0/gopro_overlay/geo_render.py` & `gopro-overlay-0.98.0/gopro_overlay/geo_render.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/geocode.py` & `gopro-overlay-0.98.0/gopro_overlay/geocode.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpmd.py` & `gopro-overlay-0.98.0/gopro_overlay/gpmd.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpmd_calculate.py` & `gopro-overlay-0.98.0/gopro_overlay/gpmd_calculate.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors.py` & `gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_cori.py` & `gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_cori.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_debug.py` & `gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_gps.py` & `gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_grav.py` & `gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_grav.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_xyz.py` & `gopro-overlay-0.98.0/gopro_overlay/gpmd_visitors_xyz.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/gpx.py` & `gopro-overlay-0.98.0/gopro_overlay/gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/bicycle.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/car.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/car.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/faq.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/faq.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/forbidden.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/forbidden.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/gauge-1.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/gauge-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/gauge.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/gauge.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_2d.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/gps_lock_2d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_3d.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/gps_lock_3d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_none.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/gps_lock_none.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_unknown.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/gps_lock_unknown.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/heartbeat.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/heartbeat.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/ice-cream-van.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/ice-cream-van.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/mountain-range.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/mountain-range.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/mountain.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/mountain.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/power.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/power.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/ruler.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/ruler.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/slope-triangle.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/slope-triangle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/slope.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/slope.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/thermometer-1.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/thermometer-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/thermometer.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/thermometer.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/user.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/user.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/icons/van-black-side-view.png` & `gopro-overlay-0.98.0/gopro_overlay/icons/van-black-side-view.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/journey.py` & `gopro-overlay-0.98.0/gopro_overlay/journey.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layout.py` & `gopro-overlay-0.98.0/gopro_overlay/layout.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layout_components.py` & `gopro-overlay-0.98.0/gopro_overlay/layout_components.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layout_xml.py` & `gopro-overlay-0.98.0/gopro_overlay/layout_xml.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layout_xml_attribute.py` & `gopro-overlay-0.98.0/gopro_overlay/layout_xml_attribute.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layout_xml_cairo.py` & `gopro-overlay-0.98.0/gopro_overlay/layout_xml_cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layouts/default-1920x1080.xml` & `gopro-overlay-0.98.0/gopro_overlay/layouts/default-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layouts/default-2704x1520.xml` & `gopro-overlay-0.98.0/gopro_overlay/layouts/default-2704x1520.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layouts/default-3840x2160.xml` & `gopro-overlay-0.98.0/gopro_overlay/layouts/default-3840x2160.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layouts/example-2.xml` & `gopro-overlay-0.98.0/gopro_overlay/layouts/example-2.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layouts/example.xml` & `gopro-overlay-0.98.0/gopro_overlay/layouts/example.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/layouts/power-1920x1080.xml` & `gopro-overlay-0.98.0/gopro_overlay/layouts/power-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/models.py` & `gopro-overlay-0.98.0/gopro_overlay/models.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/point.py` & `gopro-overlay-0.98.0/gopro_overlay/point.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/privacy.py` & `gopro-overlay-0.98.0/gopro_overlay/privacy.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/progress_frames.py` & `gopro-overlay-0.98.0/gopro_overlay/progress_frames.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/rdp.py` & `gopro-overlay-0.98.0/gopro_overlay/rdp.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/smoothing.py` & `gopro-overlay-0.98.0/gopro_overlay/smoothing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/timeseries.py` & `gopro-overlay-0.98.0/gopro_overlay/timeseries.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/timeseries_process.py` & `gopro-overlay-0.98.0/gopro_overlay/timeseries_process.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/timeunits.py` & `gopro-overlay-0.98.0/gopro_overlay/timeunits.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/timing.py` & `gopro-overlay-0.98.0/gopro_overlay/timing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/asi.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/asi.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/bar.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/angle.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/angle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/annotation.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/annotation.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/background.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/background.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/bordered.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/bordered.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/cairo.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/cap.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/cap.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/circuit.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/circuit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/colour.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/colour.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/ellipse.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/ellipse.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/face.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/face.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/gauge_marker.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/gauge_marker.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/gauge_round_254.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/gauge_round_254.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/needle.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/needle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/reading.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/reading.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/scale.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/cairo/scale.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/chart.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/chart.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/compass.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/compass.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/compass_arrow.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/compass_arrow.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/gps.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/gradient_bar.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/gradient_bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/info.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/info.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/map.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/map.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/profile.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/text.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/text.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/widgets.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,19 +225,20 @@
 class FrameSupplier:
     def drawing_frame(self) -> Image:
         raise NotImplementedError()
 
 
 class SimpleFrameSupplier(FrameSupplier):
 
-    def __init__(self, dimensions: Dimension):
+    def __init__(self, dimensions: Dimension, background: Tuple = (0,0,0,0)):
         self._dimensions = dimensions
+        self._background = background
 
     def drawing_frame(self) -> Image:
-        return Image.new("RGBA", (self._dimensions.x, self._dimensions.y), (0, 0, 0, 0))
+        return Image.new("RGBA", (self._dimensions.x, self._dimensions.y), self._background)
 
 
 class Scene:
 
     def __init__(self, widgets: List[Widget]):
         self._widgets = widgets
```

### Comparing `gopro-overlay-0.97.0/gopro_overlay/widgets/widgets_experimental.py` & `gopro-overlay-0.98.0/gopro_overlay/widgets/widgets_experimental.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/gopro_overlay.egg-info/PKG-INFO` & `gopro-overlay-0.98.0/gopro_overlay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.97.0
+Version: 0.98.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Classifier: Development Status :: 5 - Production/Stable
@@ -234,14 +234,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.98.0 [Feature] Add configurable background colour with `--bg rgba` thanks to @mishuha in discussion #120 for the concept. 
 - 0.97.0 [Feature] Add new map style "local" - which will connect to a tileserver running locally on port 8000. This may be useful if you want to use a completely custom map - like a hand drawn one.
   - For more details see: https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to @mattghub1 for the concept. 
 - 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.97.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.98.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -100,45 +100,47 @@
 Â© [Thunderforest](http://www.thunderforest.com/) ## References https://
 github.com/juanmcasillas/gopro2gpx https://github.com/JuanIrache/gopro-
 telemetry https://github.com/gopro/gpmf-parser https://coderunner.io/how-to-
 compress-gopro-movies-and-keep-metadata/ ## Other Related Software https://
 github.com/progweb/gpx2video https://github.com/JuanIrache/gopro-telemetry ##
 Latest Changes If you find any issues with new releases, please discuss in
 [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/
-discussions) - 0.97.0 [Feature] Add new map style "local" - which will connect
-to a tileserver running locally on port 8000. This may be useful if you want to
-use a completely custom map - like a hand drawn one. - For more details see:
-https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to
-@mattghub1 for the concept. - 0.96.0 [Feature] Hopefully add support for older
-gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-
-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for
-raising and some example code. - 0.95.0 [Feature] Add api key support for
-geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
-issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
-[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
-Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
-now possible. It takes a bit of work, but now can render at 12x realtime. See
-[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
-Remove support for `--output-size` as it didn't really work properly anyway. -
-0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
-much faster rendering, but may not work on all architectures. Speed
-improvements highly dependent on `ffmpeg` performance. Likely much faster when
-using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
-items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
-patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
-quickly. - [Change] Map rendering caches tile images more efficiently, so draws
-more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
-A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
-[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
-Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
-Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
-instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
-gauge-marker` - a nice clean gauge component, with a marker for the current
-value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
-06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
-attributes in layout files. This may cause some custom layouts to break! - But
-they wouldn't have been working as intended. - [Change/Breaking] Change some
-`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
-Change some `cairo-circuit-map` attribute names, aiming for standardisation
-Older changes are in [CHANGELOG.md](CHANGELOG.md)
+discussions) - 0.98.0 [Feature] Add configurable background colour with `--bg
+rgba` thanks to @mishuha in discussion #120 for the concept. - 0.97.0 [Feature]
+Add new map style "local" - which will connect to a tileserver running locally
+on port 8000. This may be useful if you want to use a completely custom map -
+like a hand drawn one. - For more details see: https://github.com/time4tea/
+gopro-dashboard-overlay/discussions/132 Thanks to @mattghub1 for the concept. -
+0.96.0 [Feature] Hopefully add support for older gopro files when joining.
+[#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks
+[@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example
+code. - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://
+github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha]
+(https://github.com/mishuha) for raising. - 0.94.0 [Change] Update docker image
+to python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully gpu* decoding/
+overlay/encoding. Huge performance increase now possible. It takes a bit of
+work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md]
+(docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove support for `--output-size`
+as it didn't really work properly anyway. - 0.92.0 [Feature] `--double-buffer`
+- EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not
+work on all architectures. Speed improvements highly dependent on `ffmpeg`
+performance. Likely much faster when using `--generate overlay`. Feedback
+welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location.
+[#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks
+[@patkoscsaba](https://github.com/patkoscsaba) for raising. - 0.90.0 [Change]
+`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
+tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
+component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
+docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
+cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
+were no locked GPS points in the movie. - Thanks [@shahargli](https://
+github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
+discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
+colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
+gauge component, with a marker for the current value.. See docs [docs/xml/
+examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
+0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
+files. This may cause some custom layouts to break! - But they wouldn't have
+been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
+names, aiming for standardisation - [Change/Breaking] Change some `cairo-
+circuit-map` attribute names, aiming for standardisation Older changes are in
+[CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.97.0/gopro_overlay.egg-info/SOURCES.txt` & `gopro-overlay-0.98.0/gopro_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.97.0/setup.py` & `gopro-overlay-0.98.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 test_requirements = [
     "pytest"
 ]
 
 setup(
     name="gopro-overlay",
-    version="0.97.0",
+    version="0.98.0",
     description="Overlay graphics dashboards onto GoPro footage",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/time4tea/gopro-dashboard-overlay",
     author="James Richardson",
     author_email="james+gopro@time4tea.net",
     license="MIT",
```

