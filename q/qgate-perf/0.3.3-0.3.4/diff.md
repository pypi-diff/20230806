# Comparing `tmp/qgate_perf-0.3.3-py3-none-any.whl.zip` & `tmp/qgate_perf-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17792 bytes, number of entries: 17
+Zip file size: 17798 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1130 b- defN 23-Jun-12 17:32 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    15101 b- defN 23-Jun-12 17:30 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    15130 b- defN 23-Aug-06 18:24 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-Jun-05 18:34 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1824 b- defN 23-May-30 17:30 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-12 17:27 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-Aug-06 18:41 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
--rw-rw-rw-  2.0 fat      731 b- defN 23-May-26 14:21 tests/test_dir.py
+-rw-rw-rw-  2.0 fat      731 b- defN 23-Aug-06 18:25 tests/test_dir.py
 -rw-rw-rw-  2.0 fat     5367 b- defN 23-Jun-06 11:35 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-12 17:35 qgate_perf-0.3.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6995 b- defN 23-Jun-12 17:35 qgate_perf-0.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 17:35 qgate_perf-0.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-12 17:35 qgate_perf-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1359 b- defN 23-Jun-12 17:35 qgate_perf-0.3.3.dist-info/RECORD
-17 files, 56386 bytes uncompressed, 15568 bytes compressed:  72.4%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-06 18:41 qgate_perf-0.3.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6995 b- defN 23-Aug-06 18:41 qgate_perf-0.3.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-06 18:41 qgate_perf-0.3.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-06 18:41 qgate_perf-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1359 b- defN 23-Aug-06 18:41 qgate_perf-0.3.4.dist-info/RECORD
+17 files, 56415 bytes uncompressed, 15574 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: tests/test_dir.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.3.3.dist-info/LICENSE
+Filename: qgate_perf-0.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.3.3.dist-info/METADATA
+Filename: qgate_perf-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.3.3.dist-info/WHEEL
+Filename: qgate_perf-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.3.3.dist-info/top_level.txt
+Filename: qgate_perf-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.3.3.dist-info/RECORD
+Filename: qgate_perf-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -175,16 +175,17 @@
                 FileFormat.PRF_CORE_STD_DEVIATION: sum_deviation / count,
                 FileFormat.PRF_CORE_TIME_END: datetime.datetime.utcnow().isoformat(' ')
             }
             self._print(file, f"  {json.dumps(out)}")
 
     def _open_output(self):
         dirname = os.path.dirname(self._output_file)
-        if not os.path.exists(dirname):
-            os.makedirs(dirname)
+        if dirname:
+            if not os.path.exists(dirname):
+                os.makedirs(dirname)
         return open(self._output_file, 'a')
 
     def _executeCore(self, run_setup: RunSetup, return_dict, processes=2, threads=2):
 
         from qgate_perf.run_return import RunReturn
 
         proc = []
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.3.3'
+__version__ = '0.3.4'
```

## Comparing `qgate_perf-0.3.3.dist-info/LICENSE` & `qgate_perf-0.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.3.3.dist-info/METADATA` & `qgate_perf-0.3.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.3.3
+Version: 0.3.4
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.3.3.dist-info/RECORD` & `qgate_perf-0.3.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=kGCih4ZnCgdzYcTXuhAUbPt-_hHyMzE5f7OzB6L4HVQ,5714
 qgate_perf/file_format.py,sha256=12FCV1UuJopUE337c8V6iBOTqHvc_hUBY6p2Cumf4Ok,1130
-qgate_perf/parallel_executor.py,sha256=Bs63LHQCyi-y6oWeUUQ5dLvL-MNLoaJxZcT1-czMjBE,15101
+qgate_perf/parallel_executor.py,sha256=nWnp6-7LS19U2xkDcumqndP_pDITj2aqSuUzSQFpR40,15130
 qgate_perf/parallel_probe.py,sha256=D1TuHfYxoZxXa1xXhXk4uyRKmNOEoUtSc0dkZ6Yqe1U,5431
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
 qgate_perf/run_setup.py,sha256=hCpvZak-7VEyuDRgh_IqJx6VYcUDqTkXi1a27V8ddsI,1824
-qgate_perf/version.py,sha256=h9smI8UNpB1x9avY745e_zgAo2ehKcrUZc7KyxVsVpU,215
+qgate_perf/version.py,sha256=fXTgRu9DtldvJE-MKt_eFkoiBktc35QZOJ7a2x46rwc,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_dir.py,sha256=NFNu4S6gZhJ7F_wuiYfl_pAXlgx8bUbwNr6UYMKG7e8,731
 tests/test_run.py,sha256=H-F3LWXBdZr4ciSvmtDLVD4c__Ut3Dw2SLuctaklSho,5367
-qgate_perf-0.3.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.3.3.dist-info/METADATA,sha256=bojM8sDYGT0yR4Cabpnwd-i49dFmNJkkEvCgLmZkZnM,6995
-qgate_perf-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.3.3.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.3.3.dist-info/RECORD,,
+qgate_perf-0.3.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.3.4.dist-info/METADATA,sha256=7Yu_CBYBZWi7Ha1-j6edDsAPd4t1DVyJI-up4pr0YyI,6995
+qgate_perf-0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.3.4.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.3.4.dist-info/RECORD,,
```

