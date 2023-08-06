# Comparing `tmp/remotior_sensus-0.0.8.tar.gz` & `tmp/remotior_sensus-0.0.9.tar.gz`

## Comparing `remotior_sensus-0.0.8.tar` & `remotior_sensus-0.0.9.tar`

### file list

```diff
@@ -1,180 +1,179 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/.readthedocs.yaml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/environment.yml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/*.
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/api.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/api_core.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/api_tools.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/basic_tutorials.rst
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/conf.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/index.rst
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/installation.rst
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/introduction.rst
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/modules.rst
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/quickstart.rst
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.bandset.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.bandset_catalog.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.configurations.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.log.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.messages.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.multiprocess_manager.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.output_manager.rst
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.processor.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.processor_functions.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.progress.rst
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.rst
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.session.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.spectral_signatures.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.table_manager.rst
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.core.temporary.rst
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_calc.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_classification.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_combination.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_dilation.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_erosion.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_mosaic.rst
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_neighbor_pixels.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_pca.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.band_sieve.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.cross_classification.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.download_products.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.preprocess_products.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.raster_reclassification.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.raster_report.rst
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.raster_to_vector.rst
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.dates_times.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.download_tools.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.files_directories.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.pytorch_tools.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.raster_vector.rst
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.read_write_files.rst
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.shared_tools.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/remotior_sensus.util.system_tools.rst
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/_static/fromGIStoRS.png
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/docs/source/_static/logo.png
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/COPYING
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/__init__.py
--rw-r--r--   0        0        0    32386 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/bandset.py
--rw-r--r--   0        0        0    49035 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/bandset_catalog.py
--rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/configurations.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/log.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/messages.py
--rw-r--r--   0        0        0    95512 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/multiprocess_manager.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/output_manager.py
--rw-r--r--   0        0        0    50342 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/processor.py
--rw-r--r--   0        0        0    51581 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/processor_functions.py
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/progress.py
--rw-r--r--   0        0        0    15609 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/session.py
--rw-r--r--   0        0        0    15273 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/spectral_signatures.py
--rw-r--r--   0        0        0    44472 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/table_manager.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/core/temporary.py
--rw-r--r--   0        0        0    82391 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/logo/remotior_sensus.svg
--rw-r--r--   0        0        0    82465 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/logo/remotior_sensus_bw.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/__init__.py
--rw-r--r--   0        0        0    69394 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_calc.py
--rw-r--r--   0        0        0    77922 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_classification.py
--rw-r--r--   0        0        0    15946 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_combination.py
--rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_dilation.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_erosion.py
--rw-r--r--   0        0        0     9544 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_mosaic.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_neighbor_pixels.py
--rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_pca.py
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/band_sieve.py
--rw-r--r--   0        0        0    24587 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/cross_classification.py
--rw-r--r--   0        0        0    46053 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/download_products.py
--rw-r--r--   0        0        0    39708 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/preprocess_products.py
--rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/raster_reclassification.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/raster_report.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/tools/raster_to_vector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/__init__.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/dates_times.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/download_tools.py
--rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/files_directories.py
--rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/pytorch_tools.py
--rw-r--r--   0        0        0    74959 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/raster_vector.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/read_write_files.py
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/shared_tools.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/src/remotior_sensus/util/system_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/run_tests.py
--rw-r--r--   0        0        0    20816 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_calc.py
--rw-r--r--   0        0        0     8110 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_classification.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_combination.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_dilation.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_erosion.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_mosaic.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_neighbor_pixels.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_pca.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_band_sieve.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_bandset.py
--rw-r--r--   0        0        0     9223 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_bandset_catalog.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_cross_classification.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_download_products.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_download_tools.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_files_directories.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_log.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_output_manager.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_preprocess_products.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_progress.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_raster_reclassification.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_raster_report.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_raster_to_vector.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_raster_vector.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_spectral_signatures.py
--rw-r--r--   0        0        0     6643 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_table_manager.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/test_temporary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B1.tif
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B10.tif
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B2.tif
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B3.tif
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B4.tif
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B5.tif
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B6.tif
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B7.tif
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/L8_2020-01-01/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B01.tif
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B02.tif
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B03.tif
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B04.tif
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B05.tif
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B06.tif
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B07.tif
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B08.tif
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B09.tif
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B11.tif
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B12.tif
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B8A.tif
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-01/__init__.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-02/S2_B02.tif
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-02/S2_B03.tif
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-02/S2_B04.tif
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-02/__init__.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-03/S2_B02.tif
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-03/S2_B03.tif
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-03/S2_B04.tif
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/S2_2020-01-03/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/file1.csv
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/file1.dbf
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/file2.csv
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/landsat_5_metadata_mtl.xml
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/landsat_8_metadata_mtl.xml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/reclass.csv
--rw-r--r--   0        0        0    98304 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/roi.gpkg
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/sentinel_2_metadata_test_l1c.xml
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/sentinel_2_metadata_test_l2a.xml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/spectral_signature_1.csv
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/tests/data/files/spectral_signature_2.csv
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/COPYING
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/LICENSE
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/README.rst
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 remotior_sensus-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/environment.yml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/api.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/api_core.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/api_tools.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/basic_tutorials.rst
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/conf.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/index.rst
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/installation.rst
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/introduction.rst
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/modules.rst
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/quickstart.rst
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.bandset.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.bandset_catalog.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.configurations.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.log.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.messages.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.multiprocess_manager.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.output_manager.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.processor.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.processor_functions.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.progress.rst
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.rst
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.session.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.spectral_signatures.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.table_manager.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.core.temporary.rst
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_calc.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_classification.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_combination.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_dilation.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_erosion.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_mosaic.rst
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_neighbor_pixels.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_pca.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.band_sieve.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.cross_classification.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.download_products.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.preprocess_products.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.raster_reclassification.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.raster_report.rst
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.raster_to_vector.rst
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.dates_times.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.download_tools.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.files_directories.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.pytorch_tools.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.raster_vector.rst
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.read_write_files.rst
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.shared_tools.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/remotior_sensus.util.system_tools.rst
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/_static/fromGIStoRS.png
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/docs/source/_static/logo.png
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/COPYING
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/__init__.py
+-rw-r--r--   0        0        0    32386 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/bandset.py
+-rw-r--r--   0        0        0    49035 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/bandset_catalog.py
+-rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/configurations.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/log.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/messages.py
+-rw-r--r--   0        0        0    95512 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/multiprocess_manager.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/output_manager.py
+-rw-r--r--   0        0        0    50342 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/processor.py
+-rw-r--r--   0        0        0    51581 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/processor_functions.py
+-rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/progress.py
+-rw-r--r--   0        0        0    15609 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/session.py
+-rw-r--r--   0        0        0    15273 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/spectral_signatures.py
+-rw-r--r--   0        0        0    44472 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/table_manager.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/core/temporary.py
+-rw-r--r--   0        0        0    82391 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/logo/remotior_sensus.svg
+-rw-r--r--   0        0        0    82465 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/logo/remotior_sensus_bw.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/__init__.py
+-rw-r--r--   0        0        0    69394 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_calc.py
+-rw-r--r--   0        0        0    77922 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_classification.py
+-rw-r--r--   0        0        0    15946 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_combination.py
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_dilation.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_erosion.py
+-rw-r--r--   0        0        0     9544 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_mosaic.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_neighbor_pixels.py
+-rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_pca.py
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/band_sieve.py
+-rw-r--r--   0        0        0    24587 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/cross_classification.py
+-rw-r--r--   0        0        0    46053 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/download_products.py
+-rw-r--r--   0        0        0    39708 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/preprocess_products.py
+-rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/raster_reclassification.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/raster_report.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/tools/raster_to_vector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/__init__.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/dates_times.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/download_tools.py
+-rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/files_directories.py
+-rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/pytorch_tools.py
+-rw-r--r--   0        0        0    74959 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/raster_vector.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/read_write_files.py
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/shared_tools.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/src/remotior_sensus/util/system_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/run_tests.py
+-rw-r--r--   0        0        0    20816 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_calc.py
+-rw-r--r--   0        0        0     8110 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_classification.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_combination.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_dilation.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_erosion.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_mosaic.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_neighbor_pixels.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_pca.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_band_sieve.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_bandset.py
+-rw-r--r--   0        0        0     9223 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_bandset_catalog.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_cross_classification.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_download_products.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_download_tools.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_files_directories.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_log.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_output_manager.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_preprocess_products.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_progress.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_raster_reclassification.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_raster_report.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_raster_to_vector.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_raster_vector.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_spectral_signatures.py
+-rw-r--r--   0        0        0     6643 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_table_manager.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/test_temporary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B1.tif
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B10.tif
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B2.tif
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B3.tif
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B4.tif
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B5.tif
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B6.tif
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B7.tif
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/L8_2020-01-01/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B01.tif
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B02.tif
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B03.tif
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B04.tif
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B05.tif
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B06.tif
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B07.tif
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B08.tif
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B09.tif
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B11.tif
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B12.tif
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B8A.tif
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-01/__init__.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-02/S2_B02.tif
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-02/S2_B03.tif
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-02/S2_B04.tif
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-02/__init__.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-03/S2_B02.tif
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-03/S2_B03.tif
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-03/S2_B04.tif
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/S2_2020-01-03/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/file1.csv
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/file1.dbf
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/file2.csv
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/landsat_5_metadata_mtl.xml
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/landsat_8_metadata_mtl.xml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/reclass.csv
+-rw-r--r--   0        0        0    98304 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/roi.gpkg
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/sentinel_2_metadata_test_l1c.xml
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/sentinel_2_metadata_test_l2a.xml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/spectral_signature_1.csv
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/tests/data/files/spectral_signature_2.csv
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/COPYING
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/README.rst
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 remotior_sensus-0.0.9/PKG-INFO
```

### Comparing `remotior_sensus-0.0.8/.github/workflows/publish-to-pypi.yml` & `remotior_sensus-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/Makefile` & `remotior_sensus-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/make.bat` & `remotior_sensus-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/source/conf.py` & `remotior_sensus-0.0.9/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 sys.path.insert(0, os.path.abspath('../../src/'))
 
 # -- Project information -----------------------------------------------------
 
 project = 'Remotior Sensus'
 copyright = '2022-2023, Luca Congedo'
 author = 'Luca Congedo'
-release = '0.0.5'
-version = '0.0.5.1'
+release = '0.0.9'
+version = '0.0.9.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 master_doc = 'index'
 locale_dirs = ['locale/']
 gettext_compact = False
```

### Comparing `remotior_sensus-0.0.8/docs/source/index.rst` & `remotior_sensus-0.0.9/docs/source/index.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 .. toctree::
    :maxdepth: 3
    :titlesonly:
 
    introduction.rst
    installation.rst
    quickstart.rst
-   basic_tutorials.rst
    api_tools.rst
    api_core.rst
    api.rst
+   basic_tutorials.rst
 
 `Except where otherwise noted, content of this work is licensed under a`
 `Creative Commons Attribution-ShareAlike 4.0 International License
 <http://creativecommons.org/licenses/by-sa/4.0/>`_.
```

### Comparing `remotior_sensus-0.0.8/docs/source/installation.rst` & `remotior_sensus-0.0.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/source/introduction.rst` & `remotior_sensus-0.0.9/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/source/remotior_sensus.core.rst` & `remotior_sensus-0.0.9/docs/source/remotior_sensus.core.rst`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/source/remotior_sensus.tools.rst` & `remotior_sensus-0.0.9/docs/source/remotior_sensus.tools.rst`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/source/remotior_sensus.util.rst` & `remotior_sensus-0.0.9/docs/source/remotior_sensus.util.rst`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/source/_static/favicon.ico` & `remotior_sensus-0.0.9/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/source/_static/fromGIStoRS.png` & `remotior_sensus-0.0.9/docs/source/_static/fromGIStoRS.png`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/docs/source/_static/logo.png` & `remotior_sensus-0.0.9/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/COPYING` & `remotior_sensus-0.0.9/src/remotior_sensus/COPYING`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/__init__.py` & `remotior_sensus-0.0.9/src/remotior_sensus/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License
 # along with Remotior Sensus. If not, see <https://www.gnu.org/licenses/>.
 
 from remotior_sensus.core.session import Session
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
```

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/bandset.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/bandset.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/bandset_catalog.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/bandset_catalog.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/configurations.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/configurations.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/log.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/log.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/messages.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/messages.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/multiprocess_manager.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/multiprocess_manager.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/output_manager.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/output_manager.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/processor.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/processor.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/processor_functions.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/processor_functions.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/progress.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/progress.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/session.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/session.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/spectral_signatures.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/spectral_signatures.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/table_manager.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/table_manager.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/core/temporary.py` & `remotior_sensus-0.0.9/src/remotior_sensus/core/temporary.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/logo/remotior_sensus.svg` & `remotior_sensus-0.0.9/src/remotior_sensus/logo/remotior_sensus.svg`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/logo/remotior_sensus_bw.svg` & `remotior_sensus-0.0.9/src/remotior_sensus/logo/remotior_sensus_bw.svg`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_calc.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_calc.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_classification.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_classification.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_combination.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_combination.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_dilation.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_dilation.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_erosion.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_erosion.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_mosaic.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_mosaic.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_neighbor_pixels.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_neighbor_pixels.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_pca.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_pca.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/band_sieve.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/band_sieve.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/cross_classification.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/cross_classification.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/download_products.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/download_products.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/preprocess_products.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/preprocess_products.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/raster_reclassification.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/raster_reclassification.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/raster_report.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/raster_report.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/tools/raster_to_vector.py` & `remotior_sensus-0.0.9/src/remotior_sensus/tools/raster_to_vector.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/util/dates_times.py` & `remotior_sensus-0.0.9/src/remotior_sensus/util/dates_times.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/util/download_tools.py` & `remotior_sensus-0.0.9/src/remotior_sensus/util/download_tools.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/util/files_directories.py` & `remotior_sensus-0.0.9/src/remotior_sensus/util/files_directories.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/util/pytorch_tools.py` & `remotior_sensus-0.0.9/src/remotior_sensus/util/pytorch_tools.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/util/raster_vector.py` & `remotior_sensus-0.0.9/src/remotior_sensus/util/raster_vector.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/util/read_write_files.py` & `remotior_sensus-0.0.9/src/remotior_sensus/util/read_write_files.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/util/shared_tools.py` & `remotior_sensus-0.0.9/src/remotior_sensus/util/shared_tools.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/src/remotior_sensus/util/system_tools.py` & `remotior_sensus-0.0.9/src/remotior_sensus/util/system_tools.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/run_tests.py` & `remotior_sensus-0.0.9/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_calc.py` & `remotior_sensus-0.0.9/tests/test_band_calc.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_classification.py` & `remotior_sensus-0.0.9/tests/test_band_classification.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_combination.py` & `remotior_sensus-0.0.9/tests/test_band_combination.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_dilation.py` & `remotior_sensus-0.0.9/tests/test_band_dilation.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_erosion.py` & `remotior_sensus-0.0.9/tests/test_band_erosion.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_mosaic.py` & `remotior_sensus-0.0.9/tests/test_band_mosaic.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_neighbor_pixels.py` & `remotior_sensus-0.0.9/tests/test_band_neighbor_pixels.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_pca.py` & `remotior_sensus-0.0.9/tests/test_band_pca.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_band_sieve.py` & `remotior_sensus-0.0.9/tests/test_band_sieve.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_bandset.py` & `remotior_sensus-0.0.9/tests/test_bandset.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_bandset_catalog.py` & `remotior_sensus-0.0.9/tests/test_bandset_catalog.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_cross_classification.py` & `remotior_sensus-0.0.9/tests/test_cross_classification.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_download_products.py` & `remotior_sensus-0.0.9/tests/test_download_products.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_download_tools.py` & `remotior_sensus-0.0.9/tests/test_download_tools.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_files_directories.py` & `remotior_sensus-0.0.9/tests/test_files_directories.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_output_manager.py` & `remotior_sensus-0.0.9/tests/test_output_manager.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_preprocess_products.py` & `remotior_sensus-0.0.9/tests/test_preprocess_products.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_progress.py` & `remotior_sensus-0.0.9/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_raster_reclassification.py` & `remotior_sensus-0.0.9/tests/test_raster_reclassification.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_raster_report.py` & `remotior_sensus-0.0.9/tests/test_raster_report.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_raster_to_vector.py` & `remotior_sensus-0.0.9/tests/test_raster_to_vector.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_raster_vector.py` & `remotior_sensus-0.0.9/tests/test_raster_vector.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_spectral_signatures.py` & `remotior_sensus-0.0.9/tests/test_spectral_signatures.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_table_manager.py` & `remotior_sensus-0.0.9/tests/test_table_manager.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/test_temporary.py` & `remotior_sensus-0.0.9/tests/test_temporary.py`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B1.tif` & `remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B1.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B10.tif` & `remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B10.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B2.tif` & `remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B2.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B3.tif` & `remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B3.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B4.tif` & `remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B4.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B5.tif` & `remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B5.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B6.tif` & `remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B6.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/L8_2020-01-01/L8_B7.tif` & `remotior_sensus-0.0.9/tests/data/L8_2020-01-01/L8_B7.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B01.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B01.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B02.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B02.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B03.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B03.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B04.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B04.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B05.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B05.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B06.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B06.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B07.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B07.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B08.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B08.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B09.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B09.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B11.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B11.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B12.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B12.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-01/S2_B8A.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-01/S2_B8A.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-02/S2_B02.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-02/S2_B02.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-02/S2_B03.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-02/S2_B03.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-02/S2_B04.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-02/S2_B04.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-03/S2_B02.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-03/S2_B02.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-03/S2_B03.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-03/S2_B03.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/S2_2020-01-03/S2_B04.tif` & `remotior_sensus-0.0.9/tests/data/S2_2020-01-03/S2_B04.tif`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/files/landsat_5_metadata_mtl.xml` & `remotior_sensus-0.0.9/tests/data/files/landsat_5_metadata_mtl.xml`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/files/landsat_8_metadata_mtl.xml` & `remotior_sensus-0.0.9/tests/data/files/landsat_8_metadata_mtl.xml`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/files/roi.gpkg` & `remotior_sensus-0.0.9/tests/data/files/roi.gpkg`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/files/sentinel_2_metadata_test_l1c.xml` & `remotior_sensus-0.0.9/tests/data/files/sentinel_2_metadata_test_l1c.xml`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/tests/data/files/sentinel_2_metadata_test_l2a.xml` & `remotior_sensus-0.0.9/tests/data/files/sentinel_2_metadata_test_l2a.xml`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/.gitignore` & `remotior_sensus-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/COPYING` & `remotior_sensus-0.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/LICENSE` & `remotior_sensus-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/README.rst` & `remotior_sensus-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/pyproject.toml` & `remotior_sensus-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `remotior_sensus-0.0.8/PKG-INFO` & `remotior_sensus-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotior_sensus
-Version: 0.0.8
+Version: 0.0.9
 Summary: Remotior Sensus is software to process remote sensing and GIS data
 Project-URL: Homepage, https://github.com/semiautomaticgit/remotior_sensus
 Project-URL: Bug Tracker, https://github.com/semiautomaticgit/remotior_sensus/issues
 Author-email: Luca Congedo <ing.congedoluca@gmail.com>
 License-File: COPYING
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

