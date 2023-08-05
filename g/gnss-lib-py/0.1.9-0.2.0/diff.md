# Comparing `tmp/gnss_lib_py-0.1.9.tar.gz` & `tmp/gnss_lib_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnss_lib_py-0.1.9.tar", max compression
+gzip compressed data, was "gnss_lib_py-0.2.0.tar", max compression
```

## Comparing `gnss_lib_py-0.1.9.tar` & `gnss_lib_py-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-05-05 22:56:56.120860 gnss_lib_py-0.1.9/LICENSE
--rw-r--r--   0        0        0     6739 2023-05-05 22:56:56.120860 gnss_lib_py-0.1.9/README.md
--rw-r--r--   0        0        0      796 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/__init__.py
--rw-r--r--   0        0        0     9603 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/algorithms/gnss_filters.py
--rw-r--r--   0        0        0     3314 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/algorithms/residuals.py
--rw-r--r--   0        0        0     9890 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/algorithms/snapshot.py
--rw-r--r--   0        0        0    23478 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/android.py
--rw-r--r--   0        0        0    21479 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/ephemeris.py
--rw-r--r--   0        0        0    56305 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/navdata.py
--rw-r--r--   0        0        0    31911 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/precise_ephemerides.py
--rw-r--r--   0        0        0     9291 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/smart_loc.py
--rw-r--r--   0        0        0     2658 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/constants.py
--rw-r--r--   0        0        0    19067 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/coordinates.py
--rw-r--r--   0        0        0      888 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/file_operations.py
--rw-r--r--   0        0        0    11986 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/filters.py
--rw-r--r--   0        0        0    25777 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/sim_gnss.py
--rw-r--r--   0        0        0    13571 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/time_conversions.py
--rw-r--r--   0        0        0    32216 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/visualizations.py
--rw-r--r--   0        0        0     1389 2023-05-05 22:56:56.204865 gnss_lib_py-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     8295 1970-01-01 00:00:00.000000 gnss_lib_py-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-05 23:23:22.024667 gnss_lib_py-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7135 2023-08-05 23:23:22.024667 gnss_lib_py-0.2.0/README.md
+-rw-r--r--   0        0        0     1042 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/__init__.py
+-rw-r--r--   0        0        0     9601 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/algorithms/gnss_filters.py
+-rw-r--r--   0        0        0     3314 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/algorithms/residuals.py
+-rw-r--r--   0        0        0    12652 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/algorithms/snapshot.py
+-rw-r--r--   0        0        0    25598 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/parsers/android.py
+-rw-r--r--   0        0        0     6188 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/parsers/clk.py
+-rw-r--r--   0        0        0    56783 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/parsers/navdata.py
+-rw-r--r--   0        0        0     7727 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/parsers/nmea.py
+-rw-r--r--   0        0        0    21697 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/parsers/rinex_nav.py
+-rw-r--r--   0        0        0     6901 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/parsers/rinex_obs.py
+-rw-r--r--   0        0        0     9304 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/parsers/smartloc.py
+-rw-r--r--   0        0        0     7470 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/parsers/sp3.py
+-rw-r--r--   0        0        0     2910 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/utils/constants.py
+-rw-r--r--   0        0        0    19067 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/utils/coordinates.py
+-rw-r--r--   0        0        0    30887 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/utils/ephemeris_downloader.py
+-rw-r--r--   0        0        0      888 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/utils/file_operations.py
+-rw-r--r--   0        0        0    11986 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/utils/filters.py
+-rw-r--r--   0        0        0    25277 2023-08-05 23:23:22.052668 gnss_lib_py-0.2.0/gnss_lib_py/utils/gnss_models.py
+-rw-r--r--   0        0        0    36652 2023-08-05 23:23:22.056668 gnss_lib_py-0.2.0/gnss_lib_py/utils/sv_models.py
+-rw-r--r--   0        0        0    19604 2023-08-05 23:23:22.056668 gnss_lib_py-0.2.0/gnss_lib_py/utils/time_conversions.py
+-rw-r--r--   0        0        0    32363 2023-08-05 23:23:22.056668 gnss_lib_py-0.2.0/gnss_lib_py/utils/visualizations.py
+-rw-r--r--   0        0        0     1389 2023-08-05 23:23:22.056668 gnss_lib_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8643 1970-01-01 00:00:00.000000 gnss_lib_py-0.2.0/PKG-INFO
```

### Comparing `gnss_lib_py-0.1.9/LICENSE` & `gnss_lib_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.9/README.md` & `gnss_lib_py-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 measurements into state estimates and visualization tools for measurements
 and state estimates.
 The modularity of `gnss_lib_py` is made possibly by the unifying
 `NavData` class, which contains methods to add, remove and modify
 numeric and string data consistently.
 We provide standard row names for `NavData` elements on the
 [reference page](https://gnss-lib-py.readthedocs.io/en/latest/reference/reference.html).
-These names ensure cross compatability between different datasets and
+These names ensure cross compatibility between different datasets and
 algorithms.
 
 Documentation
 -------------
 Full documentation is available on our [readthedocs website](https://gnss-lib-py.readthedocs.io/en/latest/index.html).
 
 
@@ -76,15 +76,19 @@
   * The data parsers in the `parsers` directory allow for either loading
     GNSS data into `gnss_lib_py`'s unifying `NavData` class or parsing
     precise ephemerides data.
     Currently, the following datasets and types are supported:
 
       * [2021 Google Android Derived Dataset](https://www.kaggle.com/c/google-smartphone-decimeter-challenge)
       * [2022 Google Android Derived Dataset](https://www.kaggle.com/competitions/smartphone-decimeter-2022)
-      * [Precise Ephemeris Data](https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/gnss_mgex.html)
+      * [TU Chemnitz smartLoc Dataset](https://www.tu-chemnitz.de/projekt/smartLoc/gnss_dataset.html.en#Datasets)
+      * [NMEA](https://www.sparkfun.com/datasheets/GPS/NMEA%20Reference%20Manual-Rev2.1-Dec07.pdf)
+      * [RINEX .o and .n](https://files.igs.org/pub/data/format/rinex305.pdf)
+      * [SP3 precise orbits](https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/orbit_products.html)
+      * [CLK clock products](https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/clock_products.html)
 
   * The `utils` directory contains utilities used to handle
     GNSS measurements, time conversions, visualizations, satellite
     simulation, file operations, etc.
 
 Installation
 ------------
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/__init__.py` & `gnss_lib_py-0.2.0/gnss_lib_py/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 
 # import submodules into gnss_lib_py namespace
 from gnss_lib_py.algorithms.gnss_filters import *
 from gnss_lib_py.algorithms.residuals import *
 from gnss_lib_py.algorithms.snapshot import *
 
 from gnss_lib_py.parsers.android import *
-from gnss_lib_py.parsers.ephemeris import *
+from gnss_lib_py.parsers.clk import *
 from gnss_lib_py.parsers.navdata import *
-from gnss_lib_py.parsers.precise_ephemerides import *
+from gnss_lib_py.parsers.nmea import *
+from gnss_lib_py.parsers.rinex_nav import *
+from gnss_lib_py.parsers.rinex_obs import *
+from gnss_lib_py.parsers.smartloc import *
+from gnss_lib_py.parsers.sp3 import *
 
 from gnss_lib_py.utils.coordinates import *
+from gnss_lib_py.utils.ephemeris_downloader import *
 from gnss_lib_py.utils.filters import *
-from gnss_lib_py.utils.sim_gnss import *
+from gnss_lib_py.utils.gnss_models import *
+from gnss_lib_py.utils.sv_models import *
 from gnss_lib_py.utils.time_conversions import *
 from gnss_lib_py.utils.visualizations import *
 
 # single location of version exists in pyproject.toml
 __version__ = metadata.version("gnss-lib-py")
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/algorithms/gnss_filters.py` & `gnss_lib_py-0.2.0/gnss_lib_py/algorithms/gnss_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     state_estimate["b_rx_ekf_m"] = states[:,7]
 
     lat,lon,alt = ecef_to_geodetic(state_estimate[["x_rx_ekf_m",
                                                    "y_rx_ekf_m",
                                                    "z_rx_ekf_m"]].reshape(3,-1))
     state_estimate["lat_rx_ekf_deg"] = lat
     state_estimate["lon_rx_ekf_deg"] = lon
-    state_estimate["alt_rx_ekf_deg"] = alt
+    state_estimate["alt_rx_ekf_m"] = alt
 
     return state_estimate
 
 class GNSSEKF(BaseExtendedKalmanFilter):
     """GNSS-only EKF implementation.
 
     States: 3D position, 3D velocity and clock bias (in m).
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/algorithms/residuals.py` & `gnss_lib_py-0.2.0/gnss_lib_py/algorithms/residuals.py`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/algorithms/snapshot.py` & `gnss_lib_py-0.2.0/gnss_lib_py/algorithms/snapshot.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,36 +10,31 @@
 __date__ = "25 Jan 2022"
 
 import warnings
 
 import numpy as np
 
 from gnss_lib_py.parsers.navdata import NavData
+from gnss_lib_py.utils import constants as consts
 from gnss_lib_py.utils.coordinates import ecef_to_geodetic
 
 def solve_wls(measurements, weight_type = None, only_bias = False,
               receiver_state=None, tol = 1e-7, max_count = 20,
-              delta_t_decimals=-2):
+              sv_rx_time=False, delta_t_decimals=-2):
     """Runs weighted least squares across each timestep.
 
     Runs weighted least squares across each timestep and adds a new
     row for the receiver's position and clock bias.
 
     The option for only_bias allows the user to only calculate the clock
     bias if the receiver position is already known. Only the bias term
     in rx_est_m will be updated if only_bias is set to True.
 
     If only_bias is set to True, then the receiver position must also
-    be passed in as the receiver_state
-
-    receiver_state : gnss_lib_py.parsers.navdata.NavData
-        Either estimated or ground truth receiver position in ECEF frame
-        in meters as an instance of the NavData class with the
-        following rows: ``x_rx*_m``, `y_rx*_m``, ``z_rx*_m``,
-        ``gps_millis``.
+    be passed in as the receiver_state.
 
     Parameters
     ----------
     measurements : gnss_lib_py.parsers.navdata.NavData
         Instance of the NavData class
     weight_type : string
         Must either be None or the name of a row in measurements
@@ -52,26 +47,34 @@
         NavData class with at least the following rows: ``x_rx*_m``,
         ``y_rx*_m``, ``z_rx*_m``, ``gps_millis``.
     tol : float
         Tolerance used for the convergence check.
     max_count : int
         Number of maximum iterations before process is aborted and
         solution returned.
+    sv_rx_time : bool
+        Flag that specifies whether the input SV positions are in the ECEF
+        frame of reference corresponding to when the measurements were
+        received. If set to `True`, the satellite positions are used as
+        is. The default value is `False`, in which case the ECEF positions
+        are assumed to in the ECEF frame at the time of signal transmission
+        and are converted to the ECEF frame at the time of signal reception,
+        while solving the WLS problem.
     delta_t_decimals : int
             Decimal places after which times are considered equal.
 
     Returns
     -------
     state_estimate : gnss_lib_py.parsers.navdata.NavData
         Estimated receiver position in ECEF frame in meters and the
         estimated receiver clock bias also in meters as an instance of
         the NavData class with shape (4 x # unique timesteps) and
         the following rows: gps_millis, x_rx_wls_m, y_rx_wls_m,
         z_rx_wls_m, b_rx_wls_m, lat_rx_wls_deg, lon_rx_wls_deg,
-        alt_rx_wls_deg.
+        alt_rx_wls_m.
 
     """
 
     # check that all necessary rows exist
     measurements.in_rows(["x_sv_m","y_sv_m","z_sv_m","gps_millis"])
 
     if only_bias:
@@ -98,14 +101,15 @@
         not_nan_indexes = ~np.isnan(pos_sv_m).any(axis=1)
         pos_sv_m = pos_sv_m[not_nan_indexes]
         corr_pr_m = corr_pr_m[not_nan_indexes]
 
         if weight_type is not None:
             if isinstance(weight_type,str) and weight_type in measurements.rows:
                 weights = measurement_subset[weight_type].reshape(-1,1)
+                weights = weights[not_nan_indexes]
             else:
                 raise TypeError("WLS weights must be None or row"\
                                 +" in NavData")
         else:
             weights = None
 
         try:
@@ -114,15 +118,15 @@
                                   receiver_state.where("gps_millis",
                                   timestamp)[[rx_idxs["x_rx*_m"][0],
                                               rx_idxs["y_rx*_m"][0],
                                               rx_idxs["z_rx*_m"][0]]
                                               ,0].reshape(-1,1),
                                              position[3])) # clock bias
             position = wls(position, pos_sv_m, corr_pr_m, weights,
-                           only_bias, tol, max_count)
+                           only_bias, tol, max_count, sv_rx_time=sv_rx_time)
             states.append([timestamp] + np.squeeze(position).tolist())
         except RuntimeError as error:
             if str(error) not in runtime_error_idxs:
                 runtime_error_idxs[str(error)] = [str(int(timestamp))]
             else:
                 runtime_error_idxs[str(error)].append(str(int(timestamp)))
             states.append([timestamp, np.nan, np.nan, np.nan, np.nan])
@@ -146,35 +150,35 @@
                     + "returning NaNs.", RuntimeWarning)
         return state_estimate
 
     lat,lon,alt = ecef_to_geodetic(state_estimate[["x_rx_wls_m","y_rx_wls_m",
                                    "z_rx_wls_m"]].reshape(3,-1))
     state_estimate["lat_rx_wls_deg"] = lat
     state_estimate["lon_rx_wls_deg"] = lon
-    state_estimate["alt_rx_wls_deg"] = alt
+    state_estimate["alt_rx_wls_m"] = alt
 
     return state_estimate
 
 def wls(rx_est_m, pos_sv_m, corr_pr_m, weights = None,
-        only_bias = False, tol = 1e-7, max_count = 20):
+        only_bias = False, tol = 1e-7, max_count = 20, sv_rx_time=False):
     """Weighted least squares solver for GNSS measurements.
 
     The option for only_bias allows the user to only calculate the clock
     bias if the receiver position is already known. Only the bias term
     in rx_est_m will be updated if only_bias is set to True.
 
     Parameters
     ----------
     rx_est_m : np.ndarray
         Estimated receiver position in ECEF frame in meters and the
         estimated receiver clock bias also in meters in an
         array with shape (4 x 1) and the following order:
         x_rx_m, y_rx_m, z_rx_m, b_rx_m.
     pos_sv_m : np.ndarray
-        Satellite positions as an array of shape [# svs x 3] where
+        Satellite ECEF positions as an array of shape [# svs x 3] where
         the columns contain in order x_sv_m, y_sv_m, and z_sv_m.
     corr_pr_m : np.ndarray
         Corrected pseudoranges for all satellites with shape of
         [# svs x 1]
     weights : np.array
         Weights as an array of shape [# svs x 1] where the column
         is in the same order as pos_sv_m and corr_pr_m
@@ -182,28 +186,63 @@
         If True, then only the receiver clock bias is estimated.
         Otherwise, both position and clock bias are estimated.
     tol : float
         Tolerance used for the convergence check.
     max_count : int
         Number of maximum iterations before process is aborted and
         solution returned.
+    sv_rx_time : bool
+        Flag to indicate if the satellite positions at the time of
+        transmission should be used as is or if they should be transformed
+        to the ECEF frame of reference at the time of reception. For real
+        measurements, use ``sv_rx_time=False`` to account for the Earth's
+        rotation and convert SV positions from the ECEF frame at the time
+        of signal transmission to the ECEF frame at the time of signal
+        reception. If the SV positions should be used as is, set
+        ``sv_rx_time=True`` to indicate that the given positions are in
+        the ECEF frame of reference for when the signals are received.
+        By default, ``sv_rx_time=False``.
 
     Returns
     -------
     rx_est_m : np.ndarray
         Estimated receiver position in ECEF frame in meters and the
         estimated receiver clock bias also in meters in an
         array with shape (4 x 1) and the following order:
         x_rx_m, y_rx_m, z_rx_m, b_rx_m.
 
+    Notes
+    -----
+    This function internally updates the used SV position to account for
+    the time taken for the signal to travel to the Earth from the GNSS
+    satellites.
+    Since the SV and receiver positions are calculated in an ECEF frame
+    of reference, which is moving with the Earth's rotation, the reference
+    frame is slightly (about 30 m along longitude) different when the
+    signals are received than when the signals were transmitted. Given
+    the receiver's position is estimated when the signal is received,
+    the SV positions need to be updated to reflect the change in the
+    frame of reference in which their position is calculated.
+
+    This update happens after every Gauss-Newton update step and is
+    adapted from [1]_.
+
+    References
+    ----------
+    .. [1] https://github.com/google/gps-measurement-tools/blob/master/opensource/FlightTimeCorrection.m
+
     """
 
     rx_est_m = rx_est_m.copy() # don't change referenced value
 
     count = 0
+    # Store the SV position at the original receiver time.
+    # This position will be modified by the time taken by the signal to
+    # travel to the receiver.
+    rx_time_pos_sv_m = pos_sv_m.copy()
     num_svs = pos_sv_m.shape[0]
     if num_svs < 4 and not only_bias:
         raise RuntimeError("Need at least four satellites for WLS.")
     pos_x_delta = np.inf*np.ones((4,1))
 
     # load weights
     if weights is None:
@@ -241,14 +280,24 @@
             break
 
         if only_bias:
             rx_est_m[3,0] += pos_x_delta[0,0]
         else:
             rx_est_m += pos_x_delta
 
+        if not sv_rx_time:
+            # Update the satellite positions based on the time taken for
+            # the signal to reach the Earth and the satellite clock bias.
+            delta_t = (corr_pr_m.reshape(-1) - rx_est_m[3,0])/consts.C
+            dtheta = consts.OMEGA_E_DOT*delta_t
+            pos_sv_m[:, 0] = np.cos(dtheta)*rx_time_pos_sv_m[:,0] + \
+                             np.sin(dtheta)*rx_time_pos_sv_m[:,1]
+            pos_sv_m[:, 1] = -np.sin(dtheta)*rx_time_pos_sv_m[:,0] + \
+                              np.cos(dtheta)*rx_time_pos_sv_m[:,1]
+
         count += 1
 
         if count >= max_count:
             warnings.warn("Newton Raphson did not converge.", RuntimeWarning)
             break
 
     return rx_est_m
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/parsers/android.py` & `gnss_lib_py-0.2.0/gnss_lib_py/parsers/android.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Functions to process Android measurements.
 
 """
 
-__authors__ = "Ashwin Kanhere, Shubh Gupta, Adam Dai"
+__authors__ = "Ashwin Kanhere, Derek Knowles, Shubh Gupta, Adam Dai"
 __date__ = "02 Nov 2021"
 
 
 import os
 import csv
 import warnings
 
@@ -26,15 +26,15 @@
     Inherits from NavData().
     """
     def __init__(self, input_path, remove_timing_outliers=True):
         """Android specific loading and preprocessing
 
         Parameters
         ----------
-        input_path : string
+        input_path : string or path-like
             Path to measurement csv file
         remove_timing_outliers : bool
             Flag for whether to remove measures that are too close or
             too far away in time. Code from the competition hosts used
             to implement changes. See note.
 
         Notes
@@ -153,15 +153,15 @@
     """
 
     def __init__(self, input_path):
         """Android specific loading and preprocessing
 
         Parameters
         ----------
-        input_path : string
+        input_path : string or path-like
             Path to measurement csv file
         """
         super().__init__(csv_path=input_path)
 
     def postprocess(self):
         """Android derived specific postprocessing
 
@@ -203,14 +203,51 @@
                       "BDS_B2A" : "b2a",
                      }
         self.replace(signal_map, rows="signal_type", inplace=True)
 
         # add gps milliseconds
         self["gps_millis"] = unix_to_gps_millis(self["unix_millis"])
 
+    def get_state_estimate(self):
+        """Extract relevant rows in a separate NavData for state estimate.
+
+        Returns
+        -------
+        state_estimate : gnss_lib_py.parsers.navdata.NavData
+            Instance of `NavData` containing state estimate rows present
+            in the instance of `AndroidDerived2022`.
+        """
+
+        rx_rows_to_find = ['x_rx*_m', 'y_rx*_m', 'z_rx*_m',
+                        'vx_rx*_mps', 'vy_rx*_mps', 'vz_rx*_mps',
+                        'b_rx*_m', 'b_dot_rx*_mps']
+        rx_rows_in_measure = ['gps_millis']
+        for row_wildcard in rx_rows_to_find:
+            try:
+                row_map = self.find_wildcard_indexes(row_wildcard, max_allow=1)
+                row = row_map[row_wildcard][0]
+                rx_rows_in_measure.append(row)
+            except KeyError:
+                warnings.warn(f"Row wildcard: {row_wildcard} not found", RuntimeWarning)
+                continue
+
+        state_estimate = NavData()
+        for _, _, measure_frame in self.loop_time('gps_millis', delta_t_decimals=-2):
+            temp_est = NavData()
+            for row_wildcard in rx_rows_in_measure:
+                temp_est[row_wildcard] = measure_frame[row_wildcard, 0]
+            if len(state_estimate)==0:
+                state_estimate = temp_est
+            else:
+                state_estimate.concat(temp_est, inplace=True)
+        return state_estimate
+
+
+
+
     @staticmethod
     def _row_map():
         """Map of row names from loaded to gnss_lib_py standard
 
         Returns
         -------
         row_map : Dict
@@ -251,15 +288,15 @@
     Inherits from NavData().
     """
     def __init__(self, input_path):
         """Android specific loading and preprocessing for NavData()
 
         Parameters
         ----------
-        input_path : string
+        input_path : string or path-like
             Path to measurement csv file
         """
 
         super().__init__(csv_path=input_path)
 
         self.postprocess()
 
@@ -365,25 +402,30 @@
 
 
     def preprocess(self, input_path):
         """Read Android raw file and produce IMU dataframe objects
 
         Parameters
         ----------
-        input_path : string
+        input_path : string or path-like
             File location of data file to read.
 
         Returns
         -------
-        accel : pd.DataFrame
-            Dataframe that contains the accel measurements from the log.
-        gyro : pd.DataFrame
-            Dataframe that contains the gyro measurements from the log.
+        measurements : pd.DataFrame
+            Dataframe that contains the accel and gyro measurements from
+            the log.
 
         """
+
+        if not isinstance(input_path, (str, os.PathLike)):
+            raise TypeError("input_path must be string or path-like")
+        if not os.path.exists(input_path):
+            raise FileNotFoundError("file not found")
+
         with open(input_path, encoding="utf8") as csvfile:
             reader = csv.reader(csvfile)
             for row in reader:
                 if row[0][0] == '#':
                     if 'Accel' in row[0]:
                         accel = [row[1:]]
                     elif 'Gyro' in row[0]:
@@ -431,23 +473,29 @@
 
 
     def preprocess(self, input_path):
         """Read Android raw file and produce location fix dataframe objects
 
         Parameters
         ----------
-        input_path : string
+        input_path : string or path-like
             File location of data file to read.
 
         Returns
         -------
         fix_df : pd.DataFrame
             Dataframe that contains the location fixes from the log.
 
         """
+
+        if not isinstance(input_path, (str, os.PathLike)):
+            raise TypeError("input_path must be string or path-like")
+        if not os.path.exists(input_path):
+            raise FileNotFoundError("file not found")
+
         with open(input_path, encoding="utf8") as csvfile:
             reader = csv.reader(csvfile)
             for row in reader:
                 if row[0][0] == '#':
                     if 'Fix' in row[0]:
                         android_fixes = [row[1:]]
                 else:
@@ -459,15 +507,15 @@
 
 
 def make_csv(input_path, output_directory, field, show_path=False):
     """Write specific data types from a GNSS android log to a CSV.
 
     Parameters
     ----------
-    input_path : string
+    input_path : string or path-like
         File location of data file to read.
     output_directory : string
         Directory where new csv file should be created
     fields : list of strings
         Type of data to extract. Valid options are either "Raw",
         "Accel", "Gyro", "Mag", or "Fix".
 
@@ -484,14 +532,20 @@
 
     """
     if not os.path.isdir(output_directory): #pragma: no cover
         os.makedirs(output_directory)
     output_path = os.path.join(output_directory, field + ".csv")
     with open(output_path, 'w', encoding="utf8") as out_csv:
         writer = csv.writer(out_csv)
+
+        if not isinstance(input_path, (str, os.PathLike)):
+            raise TypeError("input_path must be string or path-like")
+        if not os.path.exists(input_path):
+            raise FileNotFoundError("file not found")
+
         with open(input_path, 'r', encoding="utf8") as in_txt:
             for line in in_txt:
                 # Comments in the log file
                 if line[0] == '#':
                     # Remove initial '#', spaces, trailing newline
                     # and split using commas as delimiter
                     line_data = line[2:].rstrip('\n').replace(" ","").split(",")
@@ -539,15 +593,15 @@
                                                          ]].to_numpy()))
 
     state_estimate = NavData()
     state_estimate["gps_millis"] = unix_to_gps_millis(
                                      data_df["unix_millis"].to_numpy())
     state_estimate["lat_rx_deg"] = lat
     state_estimate["lon_rx_deg"] = lon
-    state_estimate["alt_rx_deg"] = alt
+    state_estimate["alt_rx_m"] = alt
 
     return state_estimate
 
 def prepare_kaggle_submission(state_estimate, trip_id="trace/phone"):
     """Converts from gnss_lib_py receiver state to Kaggle submission.
 
     Parameters
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/parsers/ephemeris.py` & `gnss_lib_py-0.2.0/gnss_lib_py/parsers/rinex_nav.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,529 +1,537 @@
-"""Functions to download, save and process satellite ephemeris files.
+"""Parses Rinex .n files.
 
-The Ephemeris Manager provides broadcast ephemeris for specific
-satellites at a specific timestep. The EphemerisManager class should be
-initialized and then the ``get_ephemeris`` function can be used to
-retrieve ephemeris for specific satellites. ``get_ephemeris`` returns
-the most recent broadcast ephemeris for the provided list of satellites
-that was broadcast BEFORE the provided timestamp. For example GPS daily
-ephemeris files contain data at a two hour frequency, so if the
-timestamp provided is 5am, then ``get_ephemeris`` will return the 4am
-data but not 6am. If provided a timestamp between midnight and 2am then
-the ephemeris from around midnight (might be the day before) will be
-provided. If no list of satellites is provided, then ``get_ephemeris``
-will return data for all satellites.
-
-When multiple observations are provided for the same satellite and same
-timestep, the Ephemeris Manager will only return the first instance.
-This is applicable when requesting ephemeris for multi-GNSS for the
-current day. Same-day multi GNSS data is pulled from  same day. For
-same-day multi-GNSS from https://igs.org/data/ which often has multiple
-observations.
+Loads rinex navigation files into a NavData object. Loading time can be
+sped up significantly by passing in the "satellites" parameter which in
+turn gets passed into the georinex library used to parse the rinex file.
+
+Rinex files can be downloaded with the load_ephemeris function in the
+utils/ephemeris_downloader.py file.
 
 """
 
-__authors__ = "Shubh Gupta, Ashwin Kanhere"
+
+__authors__ = "Ashwin Kanhere, Shubh Gupta"
 __date__ = "13 July 2021"
 
 import os
-import shutil
-import gzip
-import ftplib
-from ftplib import FTP_TLS, FTP
-from datetime import datetime, timezone
+import warnings
+from datetime import timezone
 
-import unlzw3
-import georinex
 import numpy as np
 import pandas as pd
+import georinex as gr
 
 import gnss_lib_py.utils.constants as consts
 from gnss_lib_py.parsers.navdata import NavData
-from gnss_lib_py.utils.time_conversions import datetime_to_gps_millis, tzinfo_to_utc
+from gnss_lib_py.utils.time_conversions import datetime_to_gps_millis, gps_millis_to_tow
+from gnss_lib_py.utils.ephemeris_downloader import load_ephemeris, DEFAULT_EPHEM_PATH
+
 
+class RinexNav(NavData):
+    """Class to parse Rinex navigation files containing SV parameters.
 
-class EphemerisManager():
-    """Download, store and process ephemeris files
+
+    Loads rinex navigation files into a NavData object. Loading time can
+    be sped up significantly by passing in the "satellites" parameter
+    which in turn gets passed into the georinex library used to parse
+    the rinex file.
+
+    Inherits from NavData().
 
     Attributes
     ----------
-    data_directory : string
-        Directory to store/read ephemeris files
-    data : pd.Dataframe
-        Ephemeris parameters
-    leapseconds : int
-        Leap seconds to add to UTC time to get GPS time
+    iono_params : dict
+        Dictionary of the ionosphere correction terms of the form
+        ``{gps_millis_at_day_start : {gnss_id : iono_array}}`` where
+        ``gps_millis_at_day_start`` is the time (in gps_millis) for the
+        beginning of the day corresponding to the ionosphere correction
+        parameters in ``iono_array``.
     verbose : bool
         If true, prints debugging statements.
 
-    Notes
-    -----
-    Class code taken from https://github.com/johnsonmitchelld/gnss-analysis/blob/main/gnssutils/ephemeris_manager.py
+    """
 
-    The associated license is copied below:
+    def __init__(self, input_paths, satellites=None, verbose=False):
+        """Rinex specific loading and preprocessing
 
-    BSD 3-Clause License
+        Parameters
+        ----------
+        input_paths : string or path-like or list of paths
+            Path to measurement Rinex file(s).
+        satellites : List
+            List of satellite IDs as a string, for example ['G01','E11',
+            'R06']. Defaults to None which returns get_ephemeris for
+            all satellites.
 
-    Copyright (c) 2021, Mitchell D Johnson
-    All rights reserved.
+        """
+        self.iono_params = None
+        self.verbose = verbose
+        pd_df = self.preprocess(input_paths, satellites)
 
-    Redistribution and use in source and binary forms, with or without
-    modification, are permitted provided that the following conditions are met:
-
-    1. Redistributions of source code must retain the above copyright notice, this
-       list of conditions and the following disclaimer.
-
-    2. Redistributions in binary form must reproduce the above copyright notice,
-       this list of conditions and the following disclaimer in the documentation
-       and/or other materials provided with the distribution.
-
-    3. Neither the name of the copyright holder nor the names of its
-       contributors may be used to endorse or promote products derived from
-       this software without specific prior written permission.
-
-    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-    AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-    IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-    DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-    FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-    DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-    SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-    CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-    OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-    OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        super().__init__(pandas_df=pd_df)
 
-    """
-    def __init__(self, data_directory=os.path.join(os.getcwd(), 'data', 'ephemeris'),
-                 verbose=False):
-        self.data_directory = data_directory
-        nasa_dir = os.path.join(data_directory, 'nasa')
-        igs_dir = os.path.join(data_directory, 'igs')
-        os.makedirs(nasa_dir, exist_ok=True)
-        os.makedirs(igs_dir, exist_ok=True)
-        self.data = None
-        self.leapseconds = None
-        self.verbose = verbose
 
-    def get_ephemeris(self, timestamp, satellites=None):
-        """Return ephemeris DataFrame for satellites input.
+    def preprocess(self, rinex_paths, satellites):
+        """Combine Rinex files and create pandas frame if necessary.
 
-        The Ephemeris Manager provides broadcast ephemeris for specific
-        satellites at a specific timestep. The EphemerisManager class
-        should be initialized and then the ``get_ephemeris`` function
-        can be used to retrieve ephemeris for specific satellites.
-        ``get_ephemeris`` returns the most recent broadcast ephemeris
-        for the provided list of satellites that was broadcast BEFORE
-        the provided timestamp. For example GPS daily ephemeris files
-        contain data at a two hour frequency, so if the timestamp
-        provided is 5am, then ``get_ephemeris`` will return the 4am data
-        but not 6am. If provided a timestamp between midnight and 2am
-        then the ephemeris from around midnight (might be the day
-        before) will be provided. If no list of satellites is provided,
-        then ``get_ephemeris`` will return data for all satellites.
-
-        When multiple observations are provided for the same satellite
-        and same timestep, the Ephemeris Manager will only return the
-        first instance. This is applicable when requesting ephemeris for
-        multi-GNSS for the current day. Same-day multi GNSS data is
-        pulled from  same day. For same-day multi-GNSS from
-        https://igs.org/data/ which often has multiple observations.
+        Also loads the ionospheric correction parameters from the Rinex
+        file header and stores them in a dictionary while loading the
+        pandas dataframe.
 
         Parameters
         ----------
-        timestamp : datetime.datetime
-            Ephemeris data is returned for the timestamp day and
-            includes all broadcast ephemeris whose broadcast timestamps
-            happen before the given timestamp variable. Timezone should
-            be added manually and is interpreted as UTC if not added.
+        rinex_paths : string or path-like or list of paths
+            Path to measurement Rinex file(s).
         satellites : List
             List of satellite IDs as a string, for example ['G01','E11',
             'R06']. Defaults to None which returns get_ephemeris for
             all satellites.
 
         Returns
         -------
-        data : gnss_lib_py.parsers.navdata.NavData
-            ephemeris entries corresponding to timestamp
-
-        Notes
-        -----
-        The Galileo week ``GALWeek`` is identical to the GPS Week
-        ``GPSWeek``. See http://acc.igs.org/misc/rinex304.pdf page A26
+        data : pd.DataFrame
+            Combined rinex data from all files.
 
         """
-        systems = EphemerisManager.get_constellations(satellites)
-        # add UTC timezone if datatime os offset-naive
-        timestamp = tzinfo_to_utc(timestamp)
-        if not isinstance(self.data, pd.DataFrame):
-            same_day = (datetime.now(timezone.utc) - timestamp).days <= 0
-            self.load_data(timestamp, systems, same_day)
-        data = self.data
+
+        if satellites is not None and len(satellites) != 0:
+            constellations = set()
+            for sat in satellites:
+                constellations.add(sat[0])
+        else:
+            constellations = None
+
+        if isinstance(rinex_paths, (str, os.PathLike)):
+            rinex_paths = [rinex_paths]
+
+        data = pd.DataFrame()
+        self.iono_params = {}
+        for rinex_path in rinex_paths:
+            new_data, rinex_header = self._get_ephemeris_dataframe(rinex_path,
+                                                                   constellations)
+            data = pd.concat((data,new_data), ignore_index=True)
+            # The pandas dataframe is indexed by a (time, sv) tuple and
+            # the following line gets the date of the first entry and
+            # converts it to an equivalent time in gps_millis
+            first_time = new_data['time'][0]
+            day_start_time = first_time.replace(hour=0,
+                                                minute=0,
+                                                second=0,
+                                                tzinfo = timezone.utc)
+            start_gps_millis = float(datetime_to_gps_millis(day_start_time))
+            iono_params = self.get_iono_params(rinex_header,
+                                               constellations)
+
+            if start_gps_millis not in self.iono_params \
+                or self.iono_params[start_gps_millis] is None:
+                self.iono_params[start_gps_millis] = iono_params
+            else:
+                for constellation, value in self.iono_params.items():
+                    if constellation not in \
+                        self.iono_params[start_gps_millis].keys():
+                            self.iono_params[start_gps_millis][constellation] \
+                            = value
+            #TODO: Find a more pythonic way to do this^
+        data.reset_index(inplace=True, drop=True)
+        data.sort_values('time', inplace=True, ignore_index=True)
+
         if satellites is not None:
             data = data.loc[data['sv'].isin(satellites)]
-        time_cropped_data = data.loc[data['time'] < timestamp]
-        time_cropped_data = time_cropped_data.sort_values('time').groupby(
-            'sv').last().drop(labels = 'index', axis = 'columns')
-        if satellites is not None and len(time_cropped_data) < len(satellites):
-            # if no data available for the given day, try looking at the
-            # previous day, may occur when a time near to midnight
-            # is provided. For example, 12:01am
-            if len(time_cropped_data) != 0:
-                satellites = list(set(satellites) - set(time_cropped_data.index))
-            systems = EphemerisManager.get_constellations(satellites)
-            prev_day_timestamp = datetime(year=timestamp.year,
-                                          month=timestamp.month,
-                                          day=timestamp.day - 1,
-                                          hour=23,
-                                          minute=59,
-                                          second=59,
-                                          microsecond=999999,
-                                          tzinfo=timezone.utc,
-                                          )
-            self.load_data(prev_day_timestamp, systems, False)
-            prev_data = self.data
-            if satellites is not None:
-                prev_data = prev_data.loc[prev_data['sv'].isin(satellites)]
-            prev_data = prev_data.sort_values('time').groupby(
-                'sv').last().drop(labels = 'index', axis = 'columns')
-            data = pd.concat((time_cropped_data,prev_data))
-        else:
-            data = time_cropped_data
-        data['Leap Seconds'] = self.leapseconds
-        # Convert data DataFrame to NavData instance
+
         # Move sv to DataFrame columns, reset index
-        data = data.reset_index()
+        data = data.reset_index(drop=True)
         # Replace datetime with gps_millis
-        gps_millis = [datetime_to_gps_millis(df_row['time']) \
-                        for _, df_row in data.iterrows()]
+        # Use the vectorized version of datetime_to_gps_millis
+        gps_millis = datetime_to_gps_millis(data['time'])
+        # gps_millis = [np.float64(datetime_to_gps_millis(df_row['time'])) \
+        #                 for _, df_row in data.iterrows()]
         data['gps_millis'] = gps_millis
         data = data.drop(columns=['time'])
         data = data.rename(columns={"sv":"sv_id"})
         if "GPSWeek" in data.columns:
             data = data.rename(columns={"GPSWeek":"gps_week"})
             if "GALWeek" in data.columns:
                 data["gps_week"] = np.where(pd.isnull(data["gps_week"]),
                                                       data["GALWeek"],
                                                       data["gps_week"])
         elif "GALWeek" in data.columns:
             data = data.rename(columns={"GALWeek":"gps_week"})
         if len(data) == 0:
             raise RuntimeError("No ephemeris data available for the " \
                              + "given satellites")
-        data_navdata = NavData(pandas_df=data)
-        data_navdata['gnss_sv_id'] = data_navdata['sv_id']
-        gnss_chars = [sv_id[0] for sv_id in np.atleast_1d(data_navdata['sv_id'])]
-        gnss_nums = [sv_id[1:] for sv_id in np.atleast_1d(data_navdata['sv_id'])]
-        gnss_id = [consts.CONSTELLATION_CHARS[gnss_char] for gnss_char in gnss_chars]
-        data_navdata['gnss_id'] = np.asarray(gnss_id)
-        data_navdata['sv_id'] = np.asarray(gnss_nums, dtype=int)
-        return data_navdata
+        return data
 
-    def load_data(self, timestamp, constellations=None, same_day=False):
-        """Load ephemeris into class instance
+    def postprocess(self):
+        """Rinex specific post processing.
 
-        Parameters
-        ----------
-        timestamp : datetime.datetime
-            Ephemeris data is returned for the timestamp day and
-            includes all broadcast ephemeris whose broadcast timestamps
-            happen before the given timestamp variable. Timezone should
-            be added manually and is interpreted as UTC if not added.
-        constellations : Set
-            Set of satellites For example, set({"G","R","E"}).
-        same_day : bool
-            Whether or not ephemeris is for same-day aquisition.
+        This function breaks the input `sv` row containing the
+        standard `gnss_sv_id` data into `gnss_id` and `sv_id` rows and
+        also renames `sv` to `gnss_sv_id` to match the standard
+        nomenclature.
 
         """
-        filepaths = EphemerisManager.get_filepaths(timestamp)
-        data_list = []
-
-        if constellations == None:
-            for fileinfo in filepaths.values():
-                data = self.get_ephemeris_dataframe(fileinfo,
-                                                    constellations)
-                data_list.append(data)
-        else:
-            legacy_systems = set(['G', 'R'])
-            legacy_systems_only = len(constellations - legacy_systems) == 0
-            if not same_day:
-                if legacy_systems_only:
-                    if 'G' in constellations:
-                        data_list.append(self.get_ephemeris_dataframe(
-                            filepaths['nasa_daily_gps'],
-                            constellations=None))
-                    if 'R' in constellations:
-                        data_list.append(self.get_ephemeris_dataframe(
-                            filepaths['nasa_daily_glonass'],
-                            constellations=None))
-                else:
-                    data_list.append(self.get_ephemeris_dataframe(
-                        filepaths['nasa_daily_combined'],
-                        constellations))
-            else:
-                if legacy_systems_only and 'G' in constellations:
-                    data_list.append(self.get_ephemeris_dataframe(
-                        filepaths['nasa_daily_gps'],
-                        constellations=None))
-                else:
-                    data_list.append(self.get_ephemeris_dataframe(
-                        filepaths['bkg_daily_combined'],
-                        constellations))
 
-        data = pd.DataFrame()
-        for new_data in data_list:
-            data = pd.concat((data,new_data), ignore_index=True)
-
-        data.reset_index(inplace=True)
-        data.sort_values('time', inplace=True, ignore_index=True)
-        self.data = data
+        self['gnss_sv_id'] = self['sv_id']
+        gnss_chars = [sv_id[0] for sv_id in np.atleast_1d(self['sv_id'])]
+        gnss_nums = [sv_id[1:] for sv_id in np.atleast_1d(self['sv_id'])]
+        gnss_id = [consts.CONSTELLATION_CHARS[gnss_char] for gnss_char in gnss_chars]
+        self['gnss_id'] = np.asarray(gnss_id)
+        self['sv_id'] = np.asarray(gnss_nums, dtype=int)
 
-    def get_ephemeris_dataframe(self, fileinfo, constellations=None):
+    def _get_ephemeris_dataframe(self, rinex_path, constellations=None):
         """Load/download ephemeris files and process into DataFrame
 
         Parameters
         ----------
-        fileinfo : dict
-            Filenames for ephemeris with ftp server and constellation details
-
-        constellations : Set
+        rinex_path : string or path-like
+            Filepath to rinex file
+        constellations : set
             Set of satellites {"ConstIDSVID"}
 
         Returns
         -------
         data : pd.DataFrame
             Parsed ephemeris DataFrame
+        data_header : dict
+            Header information from Rinex file.
+
         """
-        filepath = fileinfo['filepath']
-        url = fileinfo['url']
-        directory = os.path.split(filepath)[0]
-        filename = os.path.split(filepath)[1]
-        if url == 'igs-ftp.bkg.bund.de':
-            dest_filepath = os.path.join(self.data_directory, 'igs', filename)
-        else:
-            dest_filepath = os.path.join(self.data_directory, 'nasa', filename)
-        decompressed_filename = os.path.splitext(dest_filepath)[0]
-        if not os.path.isfile(decompressed_filename): # pragma: no cover
-            self.retrieve_file(url, directory, filename,
-                               dest_filepath)
-        if not self.leapseconds:
-            self.leapseconds = EphemerisManager.load_leapseconds(
-                decompressed_filename)
+
         if constellations is not None:
-            data = georinex.load(decompressed_filename,
+            data = gr.load(rinex_path,
                                  use=constellations,
                                  verbose=self.verbose).to_dataframe()
         else:
-            data = georinex.load(decompressed_filename,
+            data = gr.load(rinex_path,
                                  verbose=self.verbose).to_dataframe()
+        data_header = gr.rinexheader(rinex_path)
+        leap_seconds = self.load_leapseconds(data_header)
+        data['leap_seconds'] = leap_seconds
         data.dropna(how='all', inplace=True)
         data.reset_index(inplace=True)
-        data['source'] = decompressed_filename
-        data['t_oc'] = pd.to_numeric(data['time'] - datetime(1980, 1, 6, 0, 0, 0))
-        #TODO: Use a constant for the time of GPS clock start
+        data['source'] = rinex_path
+        data['t_oc'] = pd.to_numeric(data['time'] - consts.GPS_EPOCH_0.replace(tzinfo=None))
         data['t_oc']  = 1e-9 * data['t_oc'] - consts.WEEKSEC * np.floor(1e-9 * data['t_oc'] / consts.WEEKSEC)
         data['time'] = data['time'].dt.tz_localize('UTC')
+        # Rename Keplerian orbital parameters to match a GLP standard
         data.rename(columns={'M0': 'M_0', 'Eccentricity': 'e', 'Toe': 't_oe', 'DeltaN': 'deltaN', 'Cuc': 'C_uc', 'Cus': 'C_us',
                              'Cic': 'C_ic', 'Crc': 'C_rc', 'Cis': 'C_is', 'Crs': 'C_rs', 'Io': 'i_0', 'Omega0': 'Omega_0'}, inplace=True)
-        return data
-
-
-    @staticmethod
-    def get_filetype(timestamp):
-        """Get file extension of IGS file based on timestamp
+        data.rename(columns={'X': 'sv_x_m', 'dX': 'sv_dx_mps', 'dX2': 'sv_dx2_mps2',
+                             'Y': 'sv_y_m', 'dY': 'sv_dy_mps', 'dY2': 'sv_dy2_mps2',
+                             'Z': 'sv_z_m', 'dZ': 'sv_dz_mps', 'dZ2': 'sv_dz2_mps2'}, )
+        return data, data_header
+
+    def get_iono_params(self, rinex_header, constellations=None):
+        """Gets ionosphere parameters from RINEX file header for calculation of
+        ionosphere delay.
+
+        There are different possible ways of the header containing
+        parameters for ionosphere delay parameters. This function tries
+        different keys to extract the pertinent parameters.
 
         Parameters
         ----------
-        timestamp : datetime.datetime
-            Time of clock
+        rinex_header : dict
+            Dictionary containing RINEX file header information
+        constellations : list
+            List of strings indicating which constellations ionosphere
+            correction parameters are required for. Set to `None` by
+            default, in which case the function gets all available
+            parameters.
 
         Returns
         -------
-        extension : string
-            Extension of compressed ephemeris file
+        iono_params : dict
+            Dictionary of the form ``{gnss_id : iono_array}``, where the
+            shape of the array containing the ionospheric corrections.
         """
-        # IGS switched from .Z to .gz compression format on December 1st, 2020
-        if timestamp >= datetime(2020, 12, 1, 0, 0, 0, tzinfo=timezone.utc):
-            extension = '.gz'
-        else:
-            extension = '.Z'
-        return extension
+        iono_params = {}
+        # If path ends in .n, then the file contains only GPS satellites
+        if rinex_header['filetype']=='N' and rinex_header['systems']=='G':
+            try:
+                ion_alpha_str = rinex_header['ION ALPHA'].replace('D', 'E')
+                ion_alpha = np.array(list(map(float, ion_alpha_str.split())))
+                ion_beta_str = rinex_header['ION BETA'].replace('D', 'E')
+                ion_beta = np.array(list(map(float, ion_beta_str.split())))
+            except KeyError:
+                ion_alpha = np.array([[np.nan]])
+                ion_beta = np.array([[np.nan]])
+            gps_iono_params = np.vstack((ion_alpha, ion_beta))
+            iono_params['gps'] = gps_iono_params
+        # If the path ends in .g, then the file constains GLONASS and no
+        # ionospheric parameters
+        if rinex_header['filetype']=='G':
+            iono_params = None
+        # If the path ends in .rnx, then the file contains multiple
+        # constellations, each with their own ionospheric parameters
+        if rinex_header['filetype']=='N' and rinex_header['systems']=='M':
+            try:
+                iono_corrs = rinex_header['IONOSPHERIC CORR']
+                iono_corr_key = self._iono_corr_key()
+                # If no constellations have been specified, then use all
+                # possible constellations.
+                if constellations is None:
+                    constellations = list(iono_corr_key.keys())
+                # Loop through each constellation and load the parameters
+                for constellation in constellations:
+                    try:
+                        # Load the relevant keys for the corrections
+                        const_keys = iono_corr_key[constellation]
+                        if len(const_keys) == 2:
+                            temp_iono_params = np.empty([len(const_keys), 4])
+                            # Loop through the two constellation specific
+                            #keys to load the parameters
+                            for idx, const_key in enumerate(const_keys):
+                                temp_iono_params[idx, :] = iono_corrs[const_key]
+                        else:
+                            temp_iono_params = np.asarray(iono_corrs[const_keys[0]])
+                        iono_params[constellation] = temp_iono_params
+                    except KeyError:
+                        # if no iono parameters are found for a particular
+                        # constellation, skip that constellation
+                        continue
+            except KeyError:
+                iono_params = None
+                warnings.warn("No ionospheric parameters found in RINEX file",
+                              RuntimeWarning)
+        return iono_params
 
     @staticmethod
-    def load_leapseconds(filename):
-        """Read leapseconds from ephemeris file
-
-        Parameters
-        ----------
-        filename : string
-            Ephemeris filename
+    def _iono_corr_key():
+        """Correlations between satellite name and iono param name.
 
         Returns
         -------
-        read_lp_sec : int or None
-            Leap seconds read from file
+        iono_corr_key : list
+            String names for ionospheric correction parameters within
+            the rinex navigation file.
 
         """
-        with open(filename) as f:
-            for line in f:
-                if 'LEAP SECONDS' in line:
-                    read_lp_sec = int(line.split()[0])
-                    return read_lp_sec
-                if 'END OF HEADER' in line:
-                    return None
+        iono_corr_key = {}
+        iono_corr_key['gps'] = ['GPSA', 'GPSB']
+        iono_corr_key['galileo'] = ['GAL']
+        iono_corr_key['beidou'] = ['BDSA', 'BDSB']
+        iono_corr_key['qzss'] = ['QZSA', 'QZSB']
+        iono_corr_key['irnss'] = ['IRNA', 'IRNB']
+        return iono_corr_key
 
-        return None
-
-    @staticmethod
-    def get_constellations(satellites):
-        """Convert list of satellites to set
+    def load_leapseconds(self, rinex_header):
+        """Read leapseconds from Rinex file
 
         Parameters
         ----------
-        satellites : List
-            List of satellites of form [ConstIDSVID]
+        rinex_header : dict
+            Header information from Rinex file.
 
         Returns
         -------
-        systems : Set or None
-            Set representation of satellites for which ephemeris is needed
-        """
-        if isinstance(satellites, list):
-            systems = set()
-            for sat in satellites:
-                systems.add(sat[0])
-            return systems
-
-        return None
-
-    def retrieve_file(self, url, directory, filename, dest_filepath):
-        """Copy ephemeris file from FTP filepath to local directory.
+        leap_seconds : int
+            Leap seconds read from file, return ``np.nan``  if not found.
 
-        Also decompresses file.
+        """
+        if rinex_header['systems']=='M':
+            try:
+                leap_seconds_line = rinex_header['LEAP SECONDS']
+                leap_seconds = int(leap_seconds_line[4]+leap_seconds_line[5])
+            except KeyError:
+                leap_seconds = np.nan
+        else:
+            try:
+                leap_seconds = int(rinex_header['LEAP SECONDS'].split()[0])
+            except KeyError:
+                leap_seconds = np.nan
+        return leap_seconds
 
-        Parameters
-        ----------
-        url : String
-            FTP server location
 
-        directory : String
-            Directory where ephemeris files are stored on the FTP server
+def _compute_eccentric_anomaly(gps_week, gps_tow, ephem, tol=1e-5, max_iter=10):
+    """Compute the eccentric anomaly from ephemeris parameters.
 
-        filename : String
-            Filename in which ephemeris files are stored (both locally and globally)
+    This function extracts relevant parameters from the broadcast navigation
+    ephemerides and then solves the equation `f(E) = M - E + e * sin(E) = 0`
+    using the Newton-Raphson method.
 
-        dest_filepath : String
-            Directory where downloaded ephemeris files are stored locally
+    In the above equation `M` is the corrected mean anomaly, `e` is the
+    orbit eccentricity and `E` is the eccentric anomaly, which is unknown.
 
-        """
+    Parameters
+    ----------
+    gps_week : int
+        Week of GPS calendar corresponding to time of clock.
+    gps_tow : np.ndarray
+        GPS time of the week at which positions are required [s].
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing ephemeris parameters of satellites
+        for which states are required.
+    tol : float
+        Tolerance for convergence of the Newton-Raphson.
+    max_iter : int
+        Maximum number of iterations for Newton-Raphson.
+
+    Returns
+    -------
+    ecc_anom : np.ndarray
+        Eccentric Anomaly of GNSS satellite orbits.
 
-        secure = bool(url == 'gdc.cddis.eosdis.nasa.gov')
+    """
+    #Extract required parameters from ephemeris and GPS constants
+    delta_n   = ephem['deltaN']
+    mean_anom_0  = ephem['M_0']
+    sqrt_sma = ephem['sqrtA'] # sqrt of semi-major axis
+    sqrt_mu_a = np.sqrt(consts.MU_EARTH) * sqrt_sma**-3 # mean angular motion
+    ecc        = ephem['e']     # eccentricity
+    #Times for computing positions
+    gpsweek_diff = (np.mod(gps_week,1024) - np.mod(ephem['gps_week'],1024))*604800.
+    delta_t = gps_tow - ephem['t_oe'] + gpsweek_diff
+
+    # Calculate the mean anomaly with corrections
+    mean_anom_corr = delta_n * delta_t
+    mean_anom = mean_anom_0 + (sqrt_mu_a * delta_t) + mean_anom_corr
+
+    # Compute Eccentric Anomaly
+    ecc_anom = mean_anom
+    for _ in np.arange(0, max_iter):
+        fun = mean_anom - ecc_anom + ecc * np.sin(ecc_anom)
+        df_decc_anom = ecc*np.cos(ecc_anom) - 1.
+        delta_ecc_anom   = -fun / df_decc_anom
+        ecc_anom    = ecc_anom + delta_ecc_anom
+
+    if np.any(delta_ecc_anom > tol): #pragma: no cover
+        raise RuntimeWarning("Eccentric Anomaly may not have converged" \
+                            + f"after {max_iter} steps. : dE = {delta_ecc_anom}")
+
+    return ecc_anom
+
+
+def _estimate_sv_clock_corr(gps_millis, ephem):
+    """Calculate the modelled satellite clock delay
+
+    Parameters
+    ---------
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        Satellite ephemeris parameters for measurement SVs.
+
+    Returns
+    -------
+    clock_corr : np.ndarray
+        Satellite clock corrections containing all terms [m].
+    corr_polynomial : np.ndarray
+        Polynomial clock perturbation terms [m].
+    clock_relativistic : np.ndarray
+        Relativistic clock correction terms [m].
 
-        if self.verbose:
-            print('Retrieving ' + directory + '/' + filename + ' from ' + url)
-        ftp = self.connect(url, secure)
-        src_filepath = directory + '/' + filename
-        try:
-            with open(dest_filepath, 'wb') as handle:
-                ftp.retrbinary(
-                    'RETR ' + src_filepath, handle.write)
-        except ftplib.error_perm as err:
-            os.remove(dest_filepath)
-            raise ftplib.error_perm(str(err) + ' Failed to retrieve ' \
-                                  + src_filepath + ' from ' + url)
-
-        ftp.quit()
-        if ftp is not None: # try closing if still active
-            ftp.close()
-        self.decompress_file(dest_filepath)
+    """
+    # Extract required GPS constants
+    ecc        = ephem['e']     # eccentricity
+    sqrt_sma = ephem['sqrtA'] # sqrt of semi-major axis
+
+    # if np.abs(delta_t).any() > 302400:
+    #     delta_t = delta_t - np.sign(delta_t)*604800
+
+    gps_week, gps_tow = gps_millis_to_tow(gps_millis)
+
+    # Compute Eccentric Anomaly
+    ecc_anom = _compute_eccentric_anomaly(gps_week, gps_tow, ephem)
+
+    # Determine pseudorange corrections due to satellite clock corrections.
+    # Calculate time offset from satellite reference time
+    t_offset = gps_tow - ephem['t_oc']
+    if np.abs(t_offset).any() > 302400:  # pragma: no cover
+        t_offset = t_offset-np.sign(t_offset)*604800
+
+    # Calculate clock corrections from the polynomial corrections in
+    # broadcast message
+    corr_polynomial = (ephem['SVclockBias']
+                     + ephem['SVclockDrift']*t_offset
+                     + ephem['SVclockDriftRate']*t_offset**2)
+
+    # Calcualte the relativistic clock correction
+    corr_relativistic = consts.F * ecc * sqrt_sma * np.sin(ecc_anom)
+
+    # Calculate the total clock correction including the Tgd term
+    clk_corr = (corr_polynomial - ephem['TGD'] + corr_relativistic)
+
+    #Convert values to equivalent meters from seconds
+    clk_corr = np.array(consts.C*clk_corr, ndmin=1)
+    corr_polynomial = np.array(consts.C*corr_polynomial, ndmin=1)
+    corr_relativistic = np.array(consts.C*corr_relativistic, ndmin=1)
+
+    return clk_corr, corr_polynomial, corr_relativistic
+
+def get_time_cropped_rinex(gps_millis, satellites=None,
+                           ephemeris_directory=DEFAULT_EPHEM_PATH,
+                           verbose=False):
+    """Add SV states using Rinex file.
+
+    Provides broadcast ephemeris for specific
+    satellites at a specific timestep
+    ``add_sv_states_rinex`` returns the most recent broadcast ephemeris
+    for the provided list of satellites that was broadcast BEFORE
+    the provided timestamp. For example GPS daily ephemeris files
+    contain data at a two hour frequency, so if the timestamp
+    provided is 5am, then ``add_sv_states_rinex`` will return the 4am data
+    but not 6am. If provided a timestamp between midnight and 2am
+    then the ephemeris from around midnight (might be the day
+    before) will be provided. If no list of satellites is provided,
+    then ``add_sv_states_rinex`` will return data for all satellites.
+
+    When multiple observations are provided for the same satellite
+    and same timestep,  will only return the
+    first instance. This is applicable when requesting ephemeris for
+    multi-GNSS for the current day. Same-day multi GNSS data is
+    pulled from  same day. For same-day multi-GNSS from
+    https://igs.org/data/ which often has multiple observations.
 
-    def decompress_file(self, filepath):
-        """Decompress downloaded file ephemeris file in same destination location
+    Parameters
+    ----------
+    gps_millis : float
+        Ephemeris data is returned for the timestamp day and
+        includes all broadcast ephemeris whose broadcast timestamps
+        happen before the given timestamp variable. Timezone should
+        be added manually and is interpreted as UTC if not added.
+    satellites : List
+        List of satellite IDs as a string, for example ['G01','E11',
+        'R06']. Defaults to None which returns get_ephemeris for
+        all satellites.
+    ephemeris_directory : string or path-like
+        Directory where ephemeris files are downloaded if necessary.
+    verbose : bool
+        Prints extra debugging statements.
 
-        Parameters
-        ----------
-        filepath : String
-            Local filepath where the compressed ephemeris file is stored
+    Returns
+    -------
+    rinex_data : gnss_lib_py.parsers.navdata.NavData
+        ephemeris entries corresponding to timestamp
 
-        """
-        extension = os.path.splitext(filepath)[1]
-        decompressed_path = os.path.splitext(filepath)[0]
-        if extension == '.gz':
-            with gzip.open(filepath, 'rb') as f_in:
-                with open(decompressed_path, 'wb') as f_out:
-                    shutil.copyfileobj(f_in, f_out)
-        elif extension == '.Z':
-            with open(filepath, 'rb') as f_in:
-                with open(decompressed_path, 'wb') as f_out:
-                    f_out.write(unlzw3.unlzw(f_in.read()))
-        os.remove(filepath)
+    Notes
+    -----
+    The Galileo week ``GALWeek`` is identical to the GPS Week
+    ``GPSWeek``. See http://acc.igs.org/misc/rinex304.pdf page A26
 
-    def connect(self, url, secure):
-        """Connect to given FTP server
+    """
 
-        Parameters
-        ----------
-        url : String
-            URL of FTP server where ephemeris files are stored
+    constellations = set()
+    for sat in satellites:
+        constellations.add(consts.CONSTELLATION_CHARS[sat[0]])
+    constellations = list(constellations)
 
-        secure : Bool
-            Flag for secure FTP connection
+    rinex_paths = load_ephemeris("rinex_nav",gps_millis,constellations,
+                                 download_directory=ephemeris_directory,
+                                 verbose=verbose)
+    rinex_data = RinexNav(rinex_paths, satellites=satellites)
 
-        Returns
-        -------
-        ftp : FTP_TLS
-            FTP connection object
-        """
-        if secure:
-            ftp = FTP_TLS(url)
-            ftp.login()
-            ftp.prot_p()
-        else:
-            ftp = FTP(url)
-            ftp.login()
-        return ftp
+    time_cropped_data = rinex_data.where('gps_millis', gps_millis, "lesser")
 
-    @staticmethod
-    def get_filepaths(timestamp):
-        """Generate filepaths for all ephemeris files
+    time_cropped_data = time_cropped_data.pandas_df().sort_values(
+        'gps_millis').groupby('gnss_sv_id').last()
 
-        Parameters
-        ----------
-        timestamp : datetime.datetime
-            Time of clock
+    rinex_data_df = time_cropped_data
+    rinex_iono_params = rinex_data.iono_params
 
-        Returns
-        -------
-        filepaths : Dict
-            Dictionary of dictionaries containing filepath and directory for ephemeris files
-        """
-        timetuple = timestamp.timetuple()
-        extension = EphemerisManager.get_filetype(timestamp)
-        filepaths = {}
-
-        directory = 'gnss/data/daily/' + str(timetuple.tm_year) + '/brdc/'
-        filename = 'BRDC00IGS_R_' + \
-            str(timetuple.tm_year) + \
-            str(timetuple.tm_yday).zfill(3) + '0000_01D_MN.rnx.gz'
-        filepaths['nasa_daily_combined'] = {
-            'filepath': directory + filename, 'url': 'gdc.cddis.eosdis.nasa.gov'}
-
-        filename = 'brdc' + str(timetuple.tm_yday).zfill(3) + \
-            '0.' + str(timetuple.tm_year)[-2:] + 'n' + extension
-        filepaths['nasa_daily_gps'] = {
-            'filepath': directory + filename, 'url': 'gdc.cddis.eosdis.nasa.gov'}
-
-        filename = 'brdc' + str(timetuple.tm_yday).zfill(3) + \
-            '0.' + str(timetuple.tm_year)[-2:] + 'g' + extension
-        filepaths['nasa_daily_glonass'] = {
-            'filepath': directory + filename, 'url': 'gdc.cddis.eosdis.nasa.gov'}
-
-        directory = '/IGS/BRDC/' + \
-            str(timetuple.tm_year) + '/' + \
-            str(timetuple.tm_yday).zfill(3) + '/'
-        filename = 'BRDC00WRD_S_' + \
-            str(timetuple.tm_year) + \
-            str(timetuple.tm_yday).zfill(3) + '0000_01D_MN.rnx.gz'
-        filepaths['bkg_daily_combined'] = {
-            'filepath': directory + filename, 'url': 'igs-ftp.bkg.bund.de'}
+    rinex_data_df = rinex_data_df.reset_index()
+    rinex_data = NavData(pandas_df=rinex_data_df)
+    rinex_data.iono_params = rinex_iono_params
 
-        return filepaths
+    return rinex_data
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/parsers/navdata.py` & `gnss_lib_py-0.2.0/gnss_lib_py/parsers/navdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     Can either be initialized empty, with a csv file by setting
     ``csv_path``, a Pandas DataFrame by setting ``pandas_df`` or by a
     Numpy array by setting ``numpy_array``.
 
     Parameters
     ----------
-    csv_path : string
+    csv_path : string or path-like
         Path to csv file containing data
     pandas_df : pd.DataFrame
         Data used to initialize NavData instance.
     numpy_array : np.ndarray
         Numpy array containing data used to initialize NavData
         instance.
     **kwargs : args
@@ -89,25 +89,25 @@
         """
 
     def from_csv_path(self, csv_path, **kwargs):
         """Build attributes of NavData using csv file.
 
         Parameters
         ----------
-        csv_path : string
+        csv_path : string or path-like
             Path to csv file containing data
         header : string, int, or None
             "infer" uses the first row as column names, setting to
             None will add int names for the columns.
         sep : char
             Delimiter to use when reading in csv file.
 
         """
-        if not isinstance(csv_path, str):
-            raise TypeError("csv_path must be string")
+        if not isinstance(csv_path, (str, os.PathLike)):
+            raise TypeError("csv_path must be string or path-like")
         if not os.path.exists(csv_path):
             raise FileNotFoundError("file not found")
 
         self._build_navdata()
 
         pandas_df = pd.read_csv(csv_path, **kwargs)
         self.from_pandas_df(pandas_df)
@@ -238,14 +238,15 @@
                         new_row = np.atleast_1d(data[row])
                     elif len(data) == 0:
                         continue
                     else:
                         # add np.nan for missing values
                         new_row = np.empty((len(data),))
                         new_row.fill(np.nan)
+                    new_row = np.array(new_row, ndmin=1)
                     combined_row = np.concatenate((combined_row,
                                                    new_row))
                 new_navdata[row] = combined_row
 
             if len(self) > 0 and len(navdata) > 0:
                 new_navdata.orig_dtypes = navdata.orig_dtypes.copy()
                 new_navdata.orig_dtypes.update(self.orig_dtypes)
@@ -373,40 +374,42 @@
             elif np.isnan(value):
                 str_check = [str(np.nan)]
             else:
                 raise ValueError("Value must be string or array-like " \
                                + "for string condition checks")
             # Extract columns where condition holds true and return new NavData
             if condition == "eq":
-                new_cols = np.argwhere(np.isin(self[row, :],str_check))
+                new_cols = np.argwhere(np.atleast_1d(np.isin(self[row, :],
+                                                             str_check)))
             else:
                 # condition == "neq"
-                new_cols = np.argwhere(~np.isin(self[row, :],str_check))
+                new_cols = np.argwhere(np.atleast_1d(~np.isin(self[row, :],
+                                                              str_check)))
 
         else:
             # Values in row are numerical
             # Find columns where value can be found and return new NavData
             if condition=="eq":
                 if isinstance(value,(np.ndarray,list,tuple,set)):
                     # use numpy's isin() condition if list of values
-                    new_cols = np.argwhere(np.isin(self.array[row, :],
-                                           value))
+                    new_cols = np.argwhere(np.atleast_1d(np.isin(self.array[row, :],
+                                           value)))
                 elif not isinstance(value,str) and np.isnan(value):
                     # check isinstance b/c np.isnan can't handle strings
                     new_cols = np.argwhere(np.isnan(self.array[row, :]))
                 else:
                     new_cols = np.argwhere(self.array[row, :]==value)
             elif condition=="neq":
                 if isinstance(value,(np.ndarray,list,tuple,set)):
                     # use numpy's isin() condition if list of values
-                    new_cols = np.argwhere(~np.isin(self.array[row, :],
-                                           value))
+                    new_cols = np.argwhere(np.atleast_1d(~np.isin(self.array[row, :],
+                                           value)))
                 elif not isinstance(value,str) and np.isnan(value):
                     # check isinstance b/c np.isnan can't handle strings
-                    new_cols = np.argwhere(~np.isnan(self.array[row, :]))
+                    new_cols = np.argwhere(np.atleast_1d(~np.isnan(self.array[row, :])))
                 else:
                     new_cols = np.argwhere(self.array[row, :]!=value)
             elif condition == "leq":
                 new_cols = np.argwhere(self.array[row, :]<=value)
             elif condition == "geq":
                 new_cols = np.argwhere(self.array[row, :]>=value)
             elif condition == "greater":
@@ -443,14 +446,18 @@
         -------
         new_navdata : gnss_lib_py.parsers.navdata.NavData or None
             If inplace is False, returns NavData instance after renaming
             specified rows. If inplace is True, returns
             None.
 
         """
+        # check if there is only one column - no sorting needed
+        if self.shape[1] == 1:
+            return self
+
         if ind is None:
             assert order is not None, \
             "Provide 'order' arg as row on which NavData is sorted"
             if ascending:
                 ind = np.argsort(self[order])
             else:
                 ind = np.argsort(-self[order])
@@ -1396,15 +1403,16 @@
         cols : slice/list
             Columns to extract from the array
         """
         if isinstance(key_idx, str):
             self.in_rows(key_idx)
             rows = [self.map[key_idx]]
             cols = slice(None, None)
-        elif isinstance(key_idx, list) and isinstance(key_idx[0], str):
+        elif isinstance(key_idx, (list,tuple)) \
+            and all(isinstance(idx, str) for idx in key_idx):
             rows = [self.map[k] for k in key_idx]
             cols = slice(None, None)
         elif isinstance(key_idx, slice):
             rows = key_idx
             cols = slice(None, None)
         elif isinstance(key_idx, int):
             rows = [key_idx]
@@ -1417,15 +1425,15 @@
 
             rows = []
             if isinstance(key_idx[0], slice):
                 rows = key_idx[0]
             elif isinstance(key_idx[0], int):
                 rows = [key_idx[0]]
             else:
-                if not isinstance(key_idx[0],list):
+                if not isinstance(key_idx[0],(tuple,list)):
                     row_key = [key_idx[0]]
                 else:
                     row_key = key_idx[0]
                 for key in row_key:
                     rows.append(self.map[key])
         return rows, cols
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/parsers/precise_ephemerides.py` & `gnss_lib_py-0.2.0/gnss_lib_py/utils/sv_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,774 +1,911 @@
-"""Functions to process precise ephemerides .sp3 and .clk files.
+"""Model GNSS SV states (positions and velocities).
 
+Functions to calculate GNSS SV positions and velocities for a given time.
 """
 
-__authors__ = "Sriramya Bhamidipati"
-__date__ = "09 June 2022"
+__authors__ = "Ashwin Kanhere, Bradley Collicott"
+__date__ = "17 Jan, 2023"
 
-import os
 import warnings
 
-from datetime import datetime, timedelta, timezone
-
 import numpy as np
-from scipy import interpolate
 
-from gnss_lib_py.parsers.ephemeris import EphemerisManager
+from gnss_lib_py.parsers.sp3 import Sp3
+from gnss_lib_py.parsers.clk import Clk
 from gnss_lib_py.parsers.navdata import NavData
-from gnss_lib_py.utils.sim_gnss import find_sat
-from gnss_lib_py.utils.time_conversions import gps_millis_to_tow
-from gnss_lib_py.utils.time_conversions import datetime_to_gps_millis
+from gnss_lib_py.parsers.rinex_nav import get_time_cropped_rinex, RinexNav
+from gnss_lib_py.parsers.rinex_nav import _compute_eccentric_anomaly
+from gnss_lib_py.parsers.rinex_nav import _estimate_sv_clock_corr
 import gnss_lib_py.utils.constants as consts
+from gnss_lib_py.utils.coordinates import ecef_to_el_az
+from gnss_lib_py.utils.time_conversions import gps_millis_to_tow
+from gnss_lib_py.utils.ephemeris_downloader import DEFAULT_EPHEM_PATH, load_ephemeris
+
+
+def add_sv_states(navdata, source = 'precise', file_paths = None,
+                  download_directory = DEFAULT_EPHEM_PATH,
+                  verbose = True):
+    """Add SV states to measurements using SP3 and CLK or Rinex files.
 
-# Define the number of sats to create arrays for
-NUMSATS = {'gps': (32, 'G'),
-           'galileo': (36, 'E'),
-           'beidou': (46, 'C'),
-           'glonass': (26, 'R'), # 26 total GLONASS satellites in orbit
-           'qzss': (3, 'J')}
-
-class Sp3:
-    """Class handling satellite position data from precise ephemerides
-
-    """
-    def __init__(self):
-        self.const = None
-        self.xpos = []
-        self.ypos = []
-        self.zpos = []
-        self.tym = []
-        self.utc_time = []
-
-    def __eq__(self, other):
-        """Checks if two Sp3() classes are equal to each other
-
-        Parameters
-        ----------
-        other : gnss_lib_py.parsers.precise_ephemerides.Sp3
-            Sp3 object that stores .sp3 parsed information
-
-        Returns
-        ----------
-        bool_check : bool
-            Flag (True/False) that indicates if Sp3 classes are equal
-        """
-        bool_check = (self.const == other.const) & \
-                     (self.xpos == other.xpos) & \
-                     (self.ypos == other.ypos) & \
-                     (self.zpos == other.zpos) & \
-                     (self.tym == other.tym) & \
-                     (self.utc_time == other.utc_time)
-
-        return bool_check
-
-def parse_sp3(input_path, constellation = 'gps'):
-    """sp3 specific loading and preprocessing for any GNSS constellation
+    If source is 'precise' then will use SP3 and CLK files.
 
     Parameters
     ----------
-    input_path : string
-        Path to sp3 file
-    constellation : string
-        Key from among {gps, galileo, glonass, beidou, qzss, etc} that
-        specifies which GNSS constellation to be parsed from .sp3 file
-        (the default is 'gps')
+    navdata : gnss_lib_py.parsers.navdata.NavData
+        Instance of the NavData class that must include rows for
+        ``gps_millis``, ``gnss_id``, ``sv_id``, and ``raw_pr_m``.
+    source : string
+        The method used to compute SV states. If 'precise', then will
+        use SP3 and CLK precise files.
+    file_paths : list, string or path-like
+        Paths to existing ephemeris files if they exist.
+    download_directory : string or path-like
+        Directory where ephemeris files are downloaded if necessary.
+    verbose : bool
+        Prints extra debugging statements if true.
 
     Returns
     -------
-    sp3data : list
-        List of gnss_lib_py.parsers.precise_ephemerides.Sp3 with len = NUMSATS,
-        where each element corresponds to a satellite with specified constellation
-        and is populated with parsed sp3 information
+    navdata_w_sv_states : gnss_lib_py.parsers.navdata.NavData
+        Updated NavData class with satellite information computed.
 
-    Notes
-    -----
-    The format for .sp3 files can be viewed in [1]_.
+    """
+    if source == 'precise':
+        navdata_w_sv_states = add_sv_states_precise(navdata,
+                                file_paths = file_paths,
+                                download_directory = download_directory,
+                                verbose = verbose)
+    else:
+        raise RuntimeError('Only Precise SV state estimation supported')
+    return navdata_w_sv_states
 
-    This parser function does not process all available GNSS constellations
-    at once, i.e., needs to be independently called for each desired one
 
-    0th array of the Clk class is always empty since PRN=0 does not exist
+def add_sv_states_precise(navdata, file_paths = None,
+                          download_directory = DEFAULT_EPHEM_PATH,
+                          verbose=True):
+    """Add SV states to measurements using SP3 and CLK files.
 
-    Based on code written by J. Makela.
-    AE 456, Global Navigation Sat Systems, University of Illinois
-    Urbana-Champaign. Fall 2015
+    Parameters
+    ----------
+    navdata : gnss_lib_py.parsers.navdata.NavData
+        Instance of the NavData class that must include rows for
+        ``gps_millis``, ``gnss_id``, ``sv_id``, and ``raw_pr_m``.
+    file_paths : list, string or path-like
+        Paths to existing SP3 or CLK files if they exist.
+    download_directory : string or path-like
+        Directory where ephemeris files are downloaded if necessary.
+    verbose : bool
+        Prints extra debugging statements if true.
 
-    References
+    Returns
+    -------
+    navdata_w_sv_states : gnss_lib_py.parsers.navdata.NavData
+        Updated NavData class with satellite information computed.
+
+    """
+
+    # get unique gps_millis and constellations for ephemeris loader
+    unique_gps_millis = np.unique(navdata["gps_millis"])
+    constellations = np.unique(navdata["gnss_id"])
+
+    # load sp3 files
+    sp3_paths = load_ephemeris("sp3", gps_millis = unique_gps_millis,
+                               constellations=constellations,
+                               file_paths = file_paths,
+                               download_directory=download_directory,
+                               verbose=verbose
+                              )
+    sp3 = Sp3(sp3_paths)
+
+    # load clk files
+    clk_paths = load_ephemeris("clk", gps_millis = unique_gps_millis,
+                               constellations=constellations,
+                               file_paths = file_paths,
+                               download_directory=download_directory,
+                               verbose=verbose
+                              )
+    clk = Clk(clk_paths)
+
+    # add SV states using sp3 and clk
+    navdata_w_sv_states = single_gnss_from_precise_eph(navdata,
+                                                       sp3,
+                                                       clk,
+                                                       verbose=verbose)
+
+    return navdata_w_sv_states
+
+def add_sv_states_rinex(measurements, ephemeris_path= DEFAULT_EPHEM_PATH,
+                  constellations=['gps'], delta_t_dec = -2):
+    """
+    Add SV states (ECEF position and velocities) to measurements.
+
+    Given received measurements, add SV states for measurements corresponding
+    to received time and SV ID. If receiver position is given, that
+    position is used to calculate the delay between signal transmission
+    and reception, which is used to update the time at which the SV
+    states are calculated.
+
+    Columns for SV calculation: `gps_millis`, `gnss_id` and `sv_id`.
+    Columns for Rx based correction: x_rx*_m, y_rx*_m and z_rx*_m
+
+    Parameters
     ----------
-    .. [1]  https://files.igs.org/pub/data/format/sp3d.pdf
-            Accessed as of August 20, 2022
+    measurements : gnss_lib_py.parsers.navdata.NavData
+        Recorded measurements with time of recpetion, GNSS ID and SV ID,
+        corresponding to which SV states are calculated
+    ephemeris_path : string or path-like
+        Location where ephemeris files are stored. Files will be
+        downloaded if they don't exist for the given date and constellation.
+        If not given, default from
+    constellations : list
+        List of GNSS IDs for constellations are to be used. Others will
+        be removed while processing the measurements
+    delta_t_dec : int
+        Decimal places after which times are considered as belonging to
+        the same discrete time interval.
+
+    Returns
+    -------
+    sv_states_all_time : gnss_lib_py.parsers.navdata.NavData
+        Input measurements with rows containing SV states appended.
     """
-    # Initial checks for loading sp3_path
-    if not isinstance(input_path, str):
-        raise TypeError("input_path must be string")
-    if not os.path.exists(input_path):
-        raise FileNotFoundError("file not found")
-
-    # Load in the file
-    with open(input_path, 'r', encoding="utf-8") as infile:
-        data = [line.strip() for line in infile]
-
-    # Poll the total no. of satellites based on constellation specified
-    if constellation in NUMSATS.keys():
-        nsvs = NUMSATS[constellation][0]
-    else:
-        raise RuntimeError("No support exists for specified constellation")
+    measurements_subset, ephem, _ = \
+        _filter_ephemeris_measurements(measurements, constellations, ephemeris_path)
+    sv_states_all_time = NavData()
+    # Loop through the measurement file per time step
+    for _, _, measure_frame in measurements_subset.loop_time('gps_millis', \
+                                                             delta_t_decimals=delta_t_dec):
+        # measure_frame = measure_frame.sort('sv_id', order="descending")
+        # Sort the satellites
+        rx_ephem, _, inv_sort_order = _sort_ephem_measures(measure_frame, ephem)
+        if rx_ephem.shape[1] != measure_frame.shape[1]: #pragma: no cover
+            raise RuntimeError('Some ephemeris data is missing')
+        try:
+            # The following statement raises a KeyError if rows don't exist
+            rx_rows_to_find = ['x_rx*_m', 'y_rx*_m', 'z_rx*_m']
+            rx_idxs = measure_frame.find_wildcard_indexes(
+                                                   rx_rows_to_find,
+                                                   max_allow=1)
+            rx_ecef = measure_frame[[rx_idxs["x_rx*_m"][0],
+                                     rx_idxs["y_rx*_m"][0],
+                                     rx_idxs["z_rx*_m"][0]]
+                                     ,0]
+            sv_states, _, _ = find_sv_location(measure_frame['gps_millis'], rx_ecef, rx_ephem)
+        except KeyError:
+            sv_states = find_sv_states(measure_frame['gps_millis'], rx_ephem)
+        # Reverse the sorting
+        sv_states = sv_states.sort(ind=inv_sort_order)
+        # Add them to new rows
+        for row in sv_states.rows:
+            if row not in ('gps_millis','gnss_id','sv_id'):
+                measure_frame[row] = sv_states[row]
+        if len(sv_states_all_time)==0:
+            sv_states_all_time = measure_frame
+        else:
+            sv_states_all_time.concat(measure_frame, inplace=True)
+    return sv_states_all_time
 
-    # Create a sp3 class for each expected satellite
-    sp3data = []
-    for _ in np.arange(0, nsvs+1):
-        sp3data.append(Sp3())
-        sp3data[-1].const = constellation
-
-    # Loop through each line
-    for dval in data:
-        if len(dval) == 0:
-            # No data
-            continue
-
-        if dval[0] == '*':
-            # A new record
-            # Get the date
-            temp = dval.split()
-            curr_time = datetime( int(temp[1]), int(temp[2]), \
-                                  int(temp[3]), int(temp[4]), \
-                                  int(temp[5]),int(float(temp[6])), \
-                                  tzinfo=timezone.utc )
-            gps_millis = datetime_to_gps_millis(curr_time, add_leap_secs = False)
-
-        if 'P' in dval[0]:
-            # A satellite record.  Get the satellite number, and coordinate (X,Y,Z) info
-            temp = dval.split()
-
-            if temp[0][1] == NUMSATS[constellation][1]:
-                prn = int(temp[0][2:])
-                sp3data[prn].utc_time.append(curr_time)
-                sp3data[prn].tym.append(gps_millis)
-                sp3data[prn].xpos.append(float(temp[1])*1e3)
-                sp3data[prn].ypos.append(float(temp[2])*1e3)
-                sp3data[prn].zpos.append(float(temp[3])*1e3)
-
-    # Add warning in case any satellite PRN does not have data
-    no_data_arrays = []
-    for prn in np.arange(1, nsvs+1):
-        if len(sp3data[prn].tym) == 0:
-            no_data_arrays.append(prn)
-    if len(no_data_arrays) == nsvs:
-        warnings.warn("No sp3 data found for PRNs: "+str(no_data_arrays), RuntimeWarning)
-
-    return sp3data
-
-class Clk:
-    """Class handling satellite clock bias data from precise ephemerides
-
-    """
-    def __init__(self):
-        self.const = None
-        self.clk_bias = []
-        self.utc_time = []
-        self.tym = []
-
-    def __eq__(self, other):
-        """Checks if two Clk() classes are equal to each other
-
-        Parameters
-        ----------
-        other : gnss_lib_py.parsers.precise_ephemerides.Clk
-            Clk object that stores .clk parsed information
-
-        Returns
-        ----------
-        bool_check : bool
-            Flag (True/False) indicating if Clk classes are equal
-        """
-        return (self.const == other.const) & \
-               (self.clk_bias == other.clk_bias) & \
-               (self.tym == other.tym) & \
-               (self.utc_time == other.utc_time)
-
-def parse_clockfile(input_path, constellation = 'gps'):
-    """Clk specific loading and preprocessing for any GNSS constellation
-
-    Parameters
-    ----------
-    input_path : string
-        Path to clk file
-    constellation : string
-        Key from among {gps, galileo, glonass, beidou, qzss, etc} that
-        specifies which GNSS constellation to be parsed from .clk file
-        (the default is 'gps')
-
-    Returns
-    -------
-    clkdata : list
-        List of gnss_lib_py.parsers.precise_ephemerides.Clk with len = NUMSATS,
-        where each element corresponds to a satellite with specified constellation
-        and is populated with parsed clk information
 
-    Notes
-    -----
-    The format for .sp3 files can be viewed in [2]_.
+def add_visible_svs_for_trajectory(rx_states,
+                                   ephemeris_path=DEFAULT_EPHEM_PATH,
+                                   constellations=['gps'], el_mask = 5.):
+    """Wrapper to add visible satellite states for given times and positions.
+
+    Given a sequence of times and rx points in ECEF, along with desired
+    constellations, give SV states for satellites that are visible along
+    trajectory at given times (assuming open sky conditions).
+
+    rx_states must contain the following rows in order of increasing time:
+    * :code:`gps_millis`
+    * :code:`x_rx*_m`
+    * :code:`y_rx*_m`
+    * :code:`z_rx*_m`
 
-    This parser function does not process all available GNSS constellations
-    at once, i.e., needs to be independently called for each desired one
+    Parameters
+    ----------
+    rx_states : gnss_lib_py.parsers.navdata.NavData
+        NavData containing position states of receiver at which SV states
+        are needed.
+    ephemeris_path : string
+        Path at which ephemeris files are to be stored. Uses directory
+        default if not given.
+    constellations : list
+        List of constellations for which states are to be estimated.
+        Default is :code:`['gps']`. If :code:`None` is given, will estimate
+        states for all available constellations.
+    el_mask : float
+        Elevation value above which satellites are considered visible.
 
-    0th array of the Clk class is always empty since PRN=0 does not exist
+    Returns
+    -------
+    sv_posvel_trajectory : gnss_lib_py.parsers.navdata.Navdata
+        NavData instance containing
 
-    Based on code written by J. Makela.
-    AE 456, Global Navigation Sat Systems, University of Illinois
-    Urbana-Champaign. Fall 2015
 
-    References
-    -----
-    .. [2]  https://files.igs.org/pub/data/format/rinex_clock300.txt
-            Accessed as of August 24, 2022
     """
+    # Checks to ensure that the same number of times and states are given
+    gps_millis = rx_states['gps_millis']
+    assert len(gps_millis) == len(rx_states), \
+        "Please give same number of times and ECEF points"
+    assert isinstance(rx_states, NavData), \
+        "rx_states must be a NavData instance"
+
+
+    # Find starting time to download broadcast ephemeris file
+    start_millis = gps_millis[0]
+
+    # Initialize file with broadcast ephemeris parameters
+    rinex_paths = load_ephemeris("rinex_nav",start_millis,constellations,
+                                 download_directory=ephemeris_path,
+                                 )
+    ephem_all_sats = RinexNav(rinex_paths)
+
+    # Find rows that correspond to receiver positions
+    rx_rows_to_find = ['x_rx*_m', 'y_rx*_m', 'z_rx*_m']
+    rx_idxs = rx_states.find_wildcard_indexes(rx_rows_to_find,
+                                              max_allow=1)
+
+    # Loop through all times and positions, estimated SV states and adding
+    # them to a NavData instance that is returned
+    sv_posvel_trajectory = NavData()
+    for idx, milli in enumerate(gps_millis):
+        rx_ecef = rx_states[[rx_idxs["x_rx*_m"][0],
+                                rx_idxs["y_rx*_m"][0],
+                                rx_idxs["z_rx*_m"][0]],
+                                idx]
+        ephem_viz = find_visible_ephem(milli, rx_ecef, ephem_all_sats, el_mask=el_mask)
+        sv_posvel, _, _ = find_sv_location(milli, rx_ecef, ephem_viz)
+        sv_posvel['gps_millis'] = milli
+        if len(sv_posvel_trajectory) == 0:
+            sv_posvel_trajectory = sv_posvel
+        else:
+            sv_posvel_trajectory.concat(sv_posvel, inplace=True)
 
-    # Initial checks for loading sp3_path
-    if not isinstance(input_path, str):
-        raise TypeError("input_path must be string")
-    if not os.path.exists(input_path):
-        raise FileNotFoundError("file not found")
-
-    # Poll the total no. of satellites based on constellation specified
-    if constellation in NUMSATS.keys():
-        nsvs = NUMSATS[constellation][0]
-    else:
-        raise RuntimeError("No support exists for specified constellation")
+    return sv_posvel_trajectory
 
-    # Create a CLK class for each expected satellite
-    clkdata = []
-    for _ in np.arange(0, nsvs+1):
-        clkdata.append(Clk())
-        clkdata[-1].const = constellation
-
-    # Read Clock file
-    with open(input_path, 'r', encoding="utf-8") as infile:
-        clk = infile.readlines()
-
-    line = 0
-    while True:
-        if 'OF SOLN SATS' not in clk[line]:
-            del clk[line]
-        else:
-            line +=1
-            break
+def svs_from_el_az(elaz_deg):
+    """Generate NED satellite positions for given elevation and azimuth.
 
-    line = 0
-    while True:
-        if 'END OF HEADER' not in clk[line]:
-            line +=1
-        else:
-            del clk[0:line+1]
-            break
+    Given elevation and azimuth angles, with respect to the receiver,
+    generate satellites in the NED frame of reference with the receiver
+    position as the origin. Satellites are assumed to have a nominal
+    distance of 20,200 km from the receiver (height of GNSS satellite orbit)
+
+    Parameters
+    ----------
+    elaz_deg : np.ndarray
+        Nx2 array of elevation and azimuth angles [degrees]
+
+    Returns
+    -------
+    svs_ned : np.ndarray
+        Nx3 satellite NED positions, simulated at a distance of 20,200 km
+    """
+    assert np.shape(elaz_deg)[0] == 2, "elaz_deg should be a 2xN array"
+    el_deg = np.deg2rad(elaz_deg[0, :])
+    az_deg = np.deg2rad(elaz_deg[1, :])
+    unit_vect = np.zeros([3, np.shape(elaz_deg)[1]])
+    unit_vect[0, :] = np.sin(az_deg)*np.cos(el_deg)
+    unit_vect[1, :] = np.cos(az_deg)*np.cos(el_deg)
+    unit_vect[2, :] = np.sin(el_deg)
+    svs_ned = 20200000*unit_vect
+    return svs_ned
+
+
+def find_sv_states(gps_millis, ephem):
+    """Compute position and velocities for all satellites in ephemeris file
+    given time of clock.
+
+    `ephem` contains broadcast ephemeris parameters (similar in form to GPS
+    broadcast parameters).
+
+    Must contain the following rows (description in [1]_):
+    * :code:`gnss_id`
+    * :code:`sv_id`
+    * :code:`gps_week`
+    * :code:`t_oe`
+    * :code:`e`
+    * :code:`omega`
+    * :code:`Omega_0`
+    * :code:`OmegaDot`
+    * :code:`sqrtA`
+    * :code:`deltaN`
+    * :code:`IDOT`
+    * :code:`i_0`
+    * :code:`C_is`
+    * :code:`C_ic`
+    * :code:`C_rs`
+    * :code:`C_rc`
+    * :code:`C_uc`
+    * :code:`C_us`
+
+    Parameters
+    ----------
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing ephemeris parameters of satellites
+        for which states are required.
 
-    timelist = []
-    for _, clk_val in enumerate(clk):
-        if clk_val[0:2]=='AS':
-            timelist.append(clk_val.split())
+    Returns
+    -------
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        NavData containing satellite positions, velocities, corresponding
+        time with GNSS ID and SV number.
 
-    for _, timelist_val in enumerate(timelist):
-        dval = timelist_val[1]
+    Notes
+    -----
+    Based on code written by J. Makela.
+    AE 456, Global Navigation Sat Systems, University of Illinois
+    Urbana-Champaign. Fall 2017
+
+    More details on the algorithm used to compute satellite positions
+    from broadcast navigation message can be found in [1]_.
 
-        if dval[0] == NUMSATS[constellation][1]:
-            prn = int(dval[1:])
-            curr_time = datetime(year = int(timelist_val[2]), \
-                                 month = int(timelist_val[3]), \
-                                 day = int(timelist_val[4]), \
-                                 hour = int(timelist_val[5]), \
-                                 minute = int(timelist_val[6]), \
-                                 second = int(float(timelist_val[7])), \
-                                 tzinfo=timezone.utc)
-            clkdata[prn].utc_time.append(curr_time)
-            gps_millis = datetime_to_gps_millis(curr_time, add_leap_secs = False)
-            clkdata[prn].tym.append(gps_millis)
-            clkdata[prn].clk_bias.append(float(timelist_val[9]))
+    Satellite velocity calculations based on algorithms introduced in [2]_.
+
+    References
+    ----------
+    ..  [1] Misra, P. and Enge, P,
+        "Global Positioning System: Signals, Measurements, and Performance."
+        2nd Edition, Ganga-Jamuna Press, 2006.
+    ..  [2] B. F. Thompson, S. W. Lewis, S. A. Brown, and T. M. Scott,
+        “Computing GPS satellite velocity and acceleration from the broadcast
+        navigation message,” NAVIGATION, vol. 66, no. 4, pp. 769–779, Dec. 2019,
+        doi: 10.1002/navi.342.
+
+    """
+
+    # Convert time from GPS millis to TOW
+    gps_week, gps_tow = gps_millis_to_tow(gps_millis)
+    # Extract parameters
+
+    c_is = ephem['C_is']
+    c_ic = ephem['C_ic']
+    c_rs = ephem['C_rs']
+    c_rc = ephem['C_rc']
+    c_uc = ephem['C_uc']
+    c_us = ephem['C_us']
+    delta_n   = ephem['deltaN']
+
+    ecc        = ephem['e']     # eccentricity
+    omega    = ephem['omega'] # argument of perigee
+    omega_0  = ephem['Omega_0']
+    sqrt_sma = ephem['sqrtA'] # sqrt of semi-major axis
+    sma      = sqrt_sma**2      # semi-major axis
+
+    sqrt_mu_a = np.sqrt(consts.MU_EARTH) * sqrt_sma**-3 # mean angular motion
+    gpsweek_diff = (np.mod(gps_week,1024) - np.mod(ephem['gps_week'],1024))*604800.
+    sv_posvel = NavData()
+    sv_posvel['gnss_id'] = ephem['gnss_id']
+    sv_posvel['sv_id'] = ephem['sv_id']
+    # Deal with times being a single value or a vector with the same
+    # length as the ephemeris
+    sv_posvel['gps_millis'] = gps_millis
+
+    delta_t = gps_tow - ephem['t_oe'] + gpsweek_diff
+
+    # Calculate the mean anomaly with corrections
+    ecc_anom = _compute_eccentric_anomaly(gps_week, gps_tow, ephem)
+
+    cos_e   = np.cos(ecc_anom)
+    sin_e   = np.sin(ecc_anom)
+    e_cos_e = (1 - ecc*cos_e)
+
+    # Calculate the true anomaly from the eccentric anomaly
+    sin_nu = np.sqrt(1 - ecc**2) * (sin_e/e_cos_e)
+    cos_nu = (cos_e-ecc) / e_cos_e
+    nu_rad     = np.arctan2(sin_nu, cos_nu)
+
+    # Calcualte the argument of latitude iteratively
+    phi_0 = nu_rad + omega
+    phi   = phi_0
+    for incl in range(5):
+        cos_to_phi = np.cos(2.*phi)
+        sin_to_phi = np.sin(2.*phi)
+        phi_corr = c_uc * cos_to_phi + c_us * sin_to_phi
+        phi = phi_0 + phi_corr
+
+    # Calculate the longitude of ascending node with correction
+    omega_corr = ephem['OmegaDot'] * delta_t
+
+    # Also correct for the rotation since the beginning of the GPS week for which the Omega0 is
+    # defined.  Correct for GPS week rollovers.
+
+    # Also correct for the rotation since the beginning of the GPS week for
+    # which the Omega0 is defined.  Correct for GPS week rollovers.
+    omega = omega_0 - (consts.OMEGA_E_DOT*(gps_tow + gpsweek_diff)) + omega_corr
+
+    # Calculate orbital radius with correction
+    r_corr = c_rc * cos_to_phi + c_rs * sin_to_phi
+    orb_radius      = sma*e_cos_e + r_corr
+
+    ############################################
+    ######  Lines added for velocity (1)  ######
+    ############################################
+    delta_e   = (sqrt_mu_a + delta_n) / e_cos_e
+    dphi = np.sqrt(1 - ecc**2)*delta_e / e_cos_e
+    # Changed from the paper
+    delta_r   = (sma * ecc * delta_e * sin_e) + 2*(c_rs*cos_to_phi - c_rc*sin_to_phi)*dphi
+
+    # Calculate the inclination with correction
+    i_corr = c_ic*cos_to_phi + c_is*sin_to_phi + ephem['IDOT']*delta_t
+    incl = ephem['i_0'] + i_corr
+
+    ############################################
+    ######  Lines added for velocity (2)  ######
+    ############################################
+    delta_i = 2*(c_is*cos_to_phi - c_ic*sin_to_phi)*dphi + ephem['IDOT']
+
+    # Find the position in the orbital plane
+    x_plane = orb_radius*np.cos(phi)
+    y_plane = orb_radius*np.sin(phi)
+
+    ############################################
+    ######  Lines added for velocity (3)  ######
+    ############################################
+    delta_u = (1 + 2*(c_us * cos_to_phi - c_uc*sin_to_phi))*dphi
+    dxp = delta_r*np.cos(phi) - orb_radius*np.sin(phi)*delta_u
+    dyp = delta_r*np.sin(phi) + orb_radius*np.cos(phi)*delta_u
+    # Find satellite position in ECEF coordinates
+    cos_omega = np.cos(omega)
+    sin_omega = np.sin(omega)
+    cos_i = np.cos(incl)
+    sin_i = np.sin(incl)
+
+    sv_posvel['x_sv_m'] = x_plane*cos_omega - y_plane*cos_i*sin_omega
+    sv_posvel['y_sv_m'] = x_plane*sin_omega + y_plane*cos_i*cos_omega
+    sv_posvel['z_sv_m'] = y_plane*sin_i
+
+    ############################################
+    ######  Lines added for velocity (4)  ######
+    ############################################
+    omega_dot = ephem['OmegaDot'] - consts.OMEGA_E_DOT
+    sv_posvel['vx_sv_mps'] = (dxp * cos_omega
+                         - dyp * cos_i*sin_omega
+                         + y_plane  * sin_omega*sin_i*delta_i
+                         - (x_plane * sin_omega + y_plane*cos_i*cos_omega)*omega_dot)
+
+    sv_posvel['vy_sv_mps'] = (dxp * sin_omega
+                         + dyp * cos_i * cos_omega
+                         - y_plane  * sin_i * cos_omega * delta_i
+                         + (x_plane * cos_omega - (y_plane*cos_i*sin_omega)) * omega_dot)
+
+    sv_posvel['vz_sv_mps'] = dyp*sin_i + y_plane*cos_i*delta_i
+
+    # Estimate SV clock corrections, including polynomial and relativistic
+    # clock corrections
+    clock_corr, _, _ = _estimate_sv_clock_corr(gps_millis, ephem)
 
-    infile.close() # close the file
+    sv_posvel['b_sv_m'] = clock_corr
 
-    # Add warning in case any satellite PRN does not have data
-    no_data_arrays = []
-    for prn in np.arange(1, nsvs+1):
-        if len(clkdata[prn].tym) == 0:
-            no_data_arrays.append(prn)
-    if len(no_data_arrays) == nsvs:
-        warnings.warn("No clk data found for PRNs: " + str(no_data_arrays), RuntimeWarning)
+    return sv_posvel
 
-    return clkdata
 
-def extract_sp3(sp3data, sidx, ipos = 10, \
-                     method = 'CubicSpline', verbose = False):
-    """Computing interpolated function over sp3 data for any GNSS
+def find_visible_ephem(gps_millis, rx_ecef, ephem, el_mask=5.):
+    """Trim input ephemeris to keep only visible SVs.
 
     Parameters
     ----------
-    sp3data : list
-        Instance of GPS-only Sp3 class list with len == # sats
-    sidx : int
-        Nearest index within sp3 time series around which interpolated
-        function needs to be centered
-    ipos : int
-        No. of data points from sp3 data on either side of sidx
-        that will be used for computing interpolated function
-    method : string
-        Type of interpolation method used for sp3 data (the default is
-        CubicSpline, which depicts third-order polynomial)
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    rx_ecef : np.ndarray
+        3x1 row rx_pos ECEF position vector [m].
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing satellite ephemeris parameters
+        including gps_week and gps_tow for the ephemeris
+    el_mask : float
+        Minimum elevation of satellites considered visible.
 
     Returns
     -------
-    func_satpos : np.ndarray
-        Instance with 3-D array of scipy.interpolate.interpolate.interp1d
-        that is loaded with .sp3 data
+    eph : gnss_lib_py.parsers.navdata.NavData
+        Ephemeris parameters of visible satellites
+
     """
+    # Find positions and velocities of all satellites
+    approx_posvel = find_sv_states(gps_millis - 1000.*consts.T_TRANS, ephem)
+    # Find elevation and azimuth angles for all satellites
+    approx_pos, _ = _extract_pos_vel_arr(approx_posvel)
+    approx_el_az = ecef_to_el_az(np.reshape(rx_ecef, [3, 1]), approx_pos)
+    # Keep attributes of only those satellites which are visible
+    keep_ind = approx_el_az[0,:] > el_mask
+    eph = ephem.copy(cols=np.nonzero(keep_ind))
+    return eph
 
-    func_satpos = np.empty((3,), dtype=object)
-    func_satpos[:] = np.nan
 
-    if method=='CubicSpline':
-        low_i = (sidx - ipos) if (sidx - ipos) >= 0 else 0
-        high_i = (sidx + ipos) if (sidx + ipos) <= len(sp3data.tym) else -1
+def find_visible_sv_posvel(rx_ecef, sv_posvel, el_mask=5.):
+    """Trim input SV state NavData to keep only visible SVs.
 
-        if verbose:
-            print('Nearest sp3: ', sidx, sp3data.tym[sidx], \
-                                   sp3data.xpos[sidx], sp3data.ypos[sidx], sp3data.zpos[sidx])
+    Parameters
+    ----------
+    rx_ecef : np.ndarray
+        3x1 row rx_pos ECEF position vector [m].
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing satellite positions and velocities
+        at the time at which visible satellites are needed.
+    el_mask : float
+        Minimum elevation of satellites considered visible.
 
-        func_satpos[0] = interpolate.CubicSpline(sp3data.tym[low_i:high_i], \
-                                                 sp3data.xpos[low_i:high_i])
-        func_satpos[1] = interpolate.CubicSpline(sp3data.tym[low_i:high_i], \
-                                                 sp3data.ypos[low_i:high_i])
-        func_satpos[2] = interpolate.CubicSpline(sp3data.tym[low_i:high_i], \
-                                                 sp3data.zpos[low_i:high_i])
+    Returns
+    -------
+    vis_posvel : gnss_lib_py.parsers.navdata.NavData
+        SV states of satellites that are visible
 
-    return func_satpos
+    """
+    # Find positions and velocities of all satellites
+    approx_posvel = sv_posvel.copy()
+    # Find elevation and azimuth angles for all satellites
+    approx_pos, _ = _extract_pos_vel_arr(approx_posvel)
+    approx_el_az = ecef_to_el_az(np.reshape(rx_ecef, [3, 1]), approx_pos)
+    # Keep attributes of only those satellites which are visible
+    keep_ind = approx_el_az[0,:] > el_mask
+    vis_posvel = sv_posvel.copy(cols=np.nonzero(keep_ind))
+    return vis_posvel
 
-def extract_clk(clkdata, sidx, ipos = 10, \
-                     method='CubicSpline', verbose = False):
-    """Computing interpolated function over clk data for any GNSS
+def find_sv_location(gps_millis, rx_ecef, ephem=None, sv_posvel=None, get_iono=False):
+    """Given time, return SV positions, difference from Rx, and ranges.
 
     Parameters
     ----------
-    clkdata : list
-        Instance of GPS-only Sp3 class list with len == # sats
-    sidx : int
-        Nearest index within sp3 time series around which interpolated
-        function needs to be centered
-    ipos : int
-        No. of data points from sp3 data on either side of sidx
-        that will be used for computing interpolated function
-    method : string
-        Type of interpolation method used for sp3 data (the default is
-        CubicSpline, which depicts third-order polynomial)
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    rx_ecef : np.ndarray
+        3x1 Receiver 3D ECEF position [m].
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        DataFrame containing all satellite ephemeris parameters ephemeris,
+        as indicated in :code:`find_sv_states`. Use None if using
+        precomputed satellite positions and velocities instead.
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Precomputed positions of satellites, use None if using broadcast
+        ephemeris parameters instead.
 
     Returns
     -------
-    func_satbias : np.ndarray
-        Instance with 1-D array of scipy.interpolate.interpolate.interp1d
-        that is loaded with .clk data
-    """
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Satellite position and velocities (same if input).
+    del_pos : np.ndarray
+        Difference between satellite positions and receiver position.
+    true_range : np.ndarray
+        Distance between satellite and receiver positions.
+
+    """
+    rx_ecef = np.reshape(rx_ecef, [3, 1])
+    if sv_posvel is None:
+        assert ephem is not None, "Must provide ephemeris or positions" \
+                                + " to find satellites states"
+        sv_posvel = find_sv_states(gps_millis - 1000.*consts.T_TRANS, ephem)
+        del_pos, true_range = _find_delxyz_range(sv_posvel, rx_ecef)
+        t_corr = true_range/consts.C
+
+        # Find satellite locations at (a more accurate) time of transmission
+        sv_posvel = find_sv_states(gps_millis-1000.*t_corr, ephem)
+    del_pos, true_range = _find_delxyz_range(sv_posvel, rx_ecef)
+    t_corr = true_range/consts.C
+
+    return sv_posvel, del_pos, true_range
+
+def _filter_ephemeris_measurements(measurements, constellations,
+                                   ephemeris_path = DEFAULT_EPHEM_PATH, get_iono=False):
+    """Return subset of input measurements and ephmeris containing
+    constellations and received SVs.
+
+    Measurements are filtered to contain the intersection of received and
+    desired constellations.
+    Ephemeris is extracted from the given path and a subset containing
+    SVs that are in measurements is returned.
 
-    if method=='CubicSpline':
-        low_i = (sidx - ipos) if (sidx - ipos) >= 0 else 0
-        high_i = (sidx + ipos) if (sidx + ipos) <= len(clkdata.tym) else -1
+    Parameters
+    ----------
+    measurements : gnss_lib_py.parsers.navdata.NavData
+        Received measurements, that are filtered based on constellations.
+    constellations : list
+        List of strings indicating constellations required in output.
+    ephemeris_path : string or path-like
+        Path where the ephermis files are stored or downloaded to.
 
-        if verbose:
-            print('Nearest clk: ', sidx, clkdata.tym[sidx], clkdata.clk_bias[sidx])
+    Returns
+    -------
+    measurements_subset : gnss_lib_py.parsers.navdata.NavData
+        Measurements containing desired constellations
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        Ephemeris parameters for received SVs and constellations
+    """
+    measurements.in_rows(['gnss_id', 'sv_id', 'gps_millis'])
+    # Check whether the rows are in the right format as needed.
+    isinstance(measurements['gnss_id'].dtype, object)
+    isinstance(measurements['sv_id'].dtype, int)
+    isinstance(measurements['gps_millis'].dtype, np.int64)
+    rx_const= np.unique(measurements['gnss_id'])
+    # Check if required constellations are available, keep only required
+    # constellations
+    if constellations is None:
+        constellations = list(consts.CONSTELLATION_CHARS.values())
+    for const in constellations:
+        if const not in rx_const:
+            warnings.warn(const + " not available in received constellations", RuntimeWarning)
+    rx_const_set = set(rx_const)
+    req_const_set = set(constellations)
+    keep_consts = req_const_set.intersection(rx_const_set)
+
+    measurements_subset = measurements.where('gnss_id', keep_consts, condition="eq")
+
+    # preprocessing of received quantities for downloading ephemeris file
+    eph_sv = _combine_gnss_sv_ids(measurements)
+    lookup_sats = list(np.unique(eph_sv))
+    start_gps_millis = np.min(measurements['gps_millis'])
+    # Download the ephemeris file for all the satellites in the measurement files
+    ephem = get_time_cropped_rinex(start_gps_millis, lookup_sats,
+                                   ephemeris_path)
+    if get_iono:
+        keys = list(ephem.iono_params.keys())
+        key = keys[np.argmin([(start_gps_millis - key) for key in keys \
+                            if (start_gps_millis - key) >= 0])]
+        iono_params = ephem.iono_params[key]
+    else:
+        iono_params = None
+    return measurements_subset, ephem, iono_params
 
-        func_satbias = interpolate.CubicSpline(clkdata.tym[low_i:high_i], \
-                                               clkdata.clk_bias[low_i:high_i])
 
-    return func_satbias
+def _combine_gnss_sv_ids(measurement_frame):
+    """Combine string `gnss_id` and integer `sv_id` into single `gnss_sv_id`.
 
-def sp3_snapshot(func_satpos, cxtime, hstep = 5e-1, method='CubicSpline'):
-    """Compute satellite 3-D position and velocity from sp3 interpolated function
+    `gnss_id` contains strings like 'gps' and 'glonass' and `sv_id` contains
+    integers. The newly returned `gnss_sv_id` is formatted as `Axx` where
+    `A` is a single letter denoting the `gnss_id` and `xx` denote the two
+    digit `sv_id` of the satellite.
 
     Parameters
     ----------
-    func_satpos : np.ndarray
-        Instance with 3-D array of scipy.interpolate.interpolate.interp1d
-        that is loaded with .sp3 data
-    cxtime : float
-        Time at which the satellite 3-D position and velocity needs to be
-        computed, given 3-D array of interpolated functions
-    hstep : float
-        Step size in milliseconds used to computing 3-D velocity of any
-        given satellite using central differencing the default is 5e-1)
-    method : string
-        Type of interpolation method used for sp3 data (the default is
-        CubicSpline, which depicts third-order polynomial)
+    measurement_frame : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing measurements including `gnss_id` and
+        `sv_id`.
 
     Returns
     -------
-    satpos_sp3 : 3-D array
-        Computed satellite position in ECEF frame (Earth's rotation not included)
-    satvel_sp3 : 3-D array
-        Computed satellite velocity in ECEF frame (Earth's rotation not included)
+    gnss_sv_id : np.ndarray
+	New row values that combine `gnss_id` and `sv_id` into a something
+	similar to 'R01' or 'G12' for example.
+
+    Notes
+    -----
+    For reference on strings and the contellation characters corresponding
+    to them, refer to :code:`CONSTELLATION_CHARS` in
+    `gnss_lib_py/utils/constants.py`.
+
     """
-    if method=='CubicSpline':
-        sat_x = func_satpos[0]([cxtime-0.5*hstep, cxtime, cxtime+0.5*hstep])
-        sat_y = func_satpos[1]([cxtime-0.5*hstep, cxtime, cxtime+0.5*hstep])
-        sat_z = func_satpos[2]([cxtime-0.5*hstep, cxtime, cxtime+0.5*hstep])
+    constellation_char_inv = {const : gnss_char for gnss_char, const in consts.CONSTELLATION_CHARS.items()}
+    gnss_chars = [constellation_char_inv[const] for const in np.array(measurement_frame['gnss_id'], ndmin=1)]
+    gnss_sv_id = np.asarray([gnss_chars[col_num] + f'{sv:02}' for col_num, sv in enumerate(np.array(measurement_frame['sv_id'], ndmin=1))])
+    return gnss_sv_id
+
 
-    satpos_sp3 = np.array([sat_x[1], sat_y[1], sat_z[1]])
-    satvel_sp3 = np.array([ (sat_x[2]-sat_x[0]) / hstep, \
-                            (sat_y[2]-sat_y[0]) / hstep, \
-                            (sat_z[2]-sat_z[0]) / hstep ])
+def _sort_ephem_measures(measure_frame, ephem):
+    """Sort measures and return indices for sorting and inverting sort.
 
-    return satpos_sp3, (satvel_sp3 * 1e3)
+    Parameters
+    ----------
+    measure_frame : gnss_lib_py.parsers.navdata.NavData
+        Measurements received for a single time instance, to be sorted.
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        Ephemeris parameters for all satellites for the closest time
+        before the measurements were received.
+
+    Returns
+    -------
+    rx_ephem : gnss_lib_py.parsers.navdata.NavData
+        Ephemeris parameters for satellites from which measurements were
+        received. Sorted by `gnss_sv_id`.
+    sorted_sats_ind : np.ndarray
+        Indices that sorts the original measurements by `gnss_sv_id`.
+    inv_sort_order : np.ndarray
+        Indices that invert the sort by `gnss_sv_id` to match the order
+        in the input measurements.
+
+    """
+    gnss_sv_id = _combine_gnss_sv_ids(measure_frame)
+    sorted_sats_ind = np.argsort(gnss_sv_id)
+    inv_sort_order = np.argsort(sorted_sats_ind)
+    sorted_sats = gnss_sv_id[sorted_sats_ind]
+    rx_ephem = ephem.where('gnss_sv_id', sorted_sats, condition="eq")
+    return rx_ephem, sorted_sats_ind, inv_sort_order
 
-def clk_snapshot(func_satbias, cxtime, hstep = 5e-1, method='CubicSpline'):
-    """Compute satellite clock bias and drift from clk interpolated function
+
+def _extract_pos_vel_arr(sv_posvel):
+    """Extract satellite positions and velocities into numpy arrays.
 
     Parameters
     ----------
-    func_satbias : scipy.interpolate._cubic.CubicSpline
-        Instance with interpolated function for satellite bias from .clk data
-    cxtime : float
-        Time at which satellite clock bias and drift is to be computed
-    hstep : float
-        Step size in milliseconds used to computing clock drift using
-        central differencing (the default is 5e-1)
-    method : string
-        Type of interpolation method used for sp3 data (the default is
-        CubicSpline, which depicts third-order polynomial)
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        NavData containing satellite position and velocity states.
 
     Returns
     -------
-    satbias_clk : float
-        Computed satellite clock bias (in seconds)
-    satdrift_clk : float
-        Computed satellite clock drift (in seconds/seconds)
-    """
+    sv_pos : np.ndarray
+        ECEF satellite x, y and z positions 3xN [m].
+    sv_vel : np.ndarray
+        ECEF satellite x, y and z velocities 3xN [m].
+    """
+    sv_pos = sv_posvel[['x_sv_m', 'y_sv_m', 'z_sv_m']]
+    sv_vel   = sv_posvel[['vx_sv_mps', 'vy_sv_mps', 'vz_sv_mps']]
+    return sv_pos, sv_vel
 
-    if method=='CubicSpline':
-        sat_t = func_satbias([cxtime-0.5*hstep, cxtime, cxtime+0.5*hstep])
 
-    satbias_clk = sat_t[1]
-    satdrift_clk = (sat_t[2]-sat_t[0]) / hstep
+def _find_delxyz_range(sv_posvel, rx_ecef):
+    """Return difference of satellite and rx_pos positions and distance between them.
 
-    return satbias_clk, (satdrift_clk * 1e3)
+    Parameters
+    ----------
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Satellite position and velocities.
+    rx_ecef : np.ndarray
+        3x1 Receiver 3D ECEF position [m].
 
-def single_gnss_from_precise_eph(navdata, sp3_parsed_file, \
-                                         clk_parsed_file, verbose = False):
+    Returns
+    -------
+    del_pos : np.ndarray
+        Difference between satellite positions and receiver position.
+    true_range : np.ndarray
+        Distance between satellite and receiver positions.
+    """
+    rx_ecef = np.reshape(rx_ecef, [3, 1])
+    satellites = len(sv_posvel)
+    sv_pos, _ = _extract_pos_vel_arr(sv_posvel)
+    sv_pos = sv_pos.reshape(rx_ecef.shape[0], satellites)
+    del_pos = sv_pos - np.tile(rx_ecef, (1, satellites))
+    true_range = np.linalg.norm(del_pos, axis=0)
+    return del_pos, true_range
+
+def single_gnss_from_precise_eph(navdata, sp3_parsed_file,
+                                 clk_parsed_file, inplace=False,
+                                 verbose = False):
     """Compute satellite information using .sp3 and .clk for any GNSS constellation
 
+    Either adds or replaces satellite ECEF position data and clock bias
+    for any satellite that exists in the provided sp3 file
+
     Parameters
     ----------
     navdata : gnss_lib_py.parsers.navdata.NavData
         Instance of the NavData class that depicts android derived dataset
-    sp3_parsed_file : list
-        Instance with list of gnss_lib_py.parsers.precise_ephemerides.Sp3
-    clk_parsed_file : list
-        Instance with list of gnss_lib_py.parsers.precise_ephemerides.Clk
+    sp3_parsed_file : gnss_lib_py.parsers.sp3.Sp3
+        SP3 data
+    clk_parsed_file : gnss_lib_py.parsers.clk.Clk
+        Clk data
+    inplace : bool
+        If true, adds satellite positions and clock bias to the input
+        navdata object, otherwise returns a new NavData object with the
+        satellite rows added.
     verbose : bool
         Flag (True/False) for whether to print intermediate steps useful
         for debugging/reviewing (the default is False)
 
     Returns
     -------
     navdata : gnss_lib_py.parsers.navdata.NavData
         Updated NavData class with satellite information computed using
         precise ephemerides from .sp3 and .clk files
     """
 
-    navdata_offset = 0 #1000 # Set this to zero, when android errors get fixed
-    unique_gnss_id = np.unique(navdata['gnss_id'])
-    if not len(unique_gnss_id)==1:
-        raise RuntimeError("Input error: Multiple constellations " + \
-                           "cannot be updated simultaneously")
-
-    if not len(sp3_parsed_file) == len(clk_parsed_file):
-        raise RuntimeError("Input error: Max no. of PRNs in sp3 and clk " + \
-                           "parsed files do not match")
-
-    if not sp3_parsed_file[0].const == clk_parsed_file[0].const:
-        raise RuntimeError("Input error: Constellations associated with " + \
-                           "sp3 and clk parsed files do not match")
-
-    # add another if condition here that checks if navdata, sp3, clk all same
-    # constellation -> after constellation flag changed in precise_ephemerides
-
-    interp_method = 'CubicSpline' # Currently only one functionality
-
     # Initialize the sp3 and clk iref arrays
-    sp3_iref_old = -1 * np.ones( (len(sp3_parsed_file),))
-    satfunc_xyz_old = np.empty( (len(sp3_parsed_file),), dtype=object)
-    satfunc_xyz_old[:] = np.nan
-
-    clk_iref_old = -1 * np.ones( (len(clk_parsed_file),))
-    satfunc_t_old = np.empty( (len(clk_parsed_file),), dtype=object)
-    satfunc_t_old[:] = np.nan
+    sp3_iref_old = {}
+    satfunc_xyz_old = {}
+    clk_iref_old = {}
+    satfunc_t_old = {}
+
 
-    # Compute satellite information for desired time steps
-    unique_timesteps = np.unique(navdata["gps_millis"])
+    # combine gnss_id and sv_id into gnss_sv_ids
+    if inplace:
+        navdata["gnss_sv_id"] = _combine_gnss_sv_ids(navdata)
+    else:
+        new_navdata = navdata.copy()
+        new_navdata["gnss_sv_id"] = _combine_gnss_sv_ids(new_navdata)
 
     # add satellite indexes if not present already.
     sv_idx_keys = ['x_sv_m', 'y_sv_m', 'z_sv_m', \
                 'vx_sv_mps','vy_sv_mps','vz_sv_mps', \
                 'b_sv_m', 'b_dot_sv_mps']
     for sv_idx_key in sv_idx_keys:
         if sv_idx_key not in navdata.rows:
-            navdata[sv_idx_key] = np.nan
-
-    for t_idx, timestep in enumerate(unique_timesteps):
+            if inplace:
+                navdata[sv_idx_key] = np.nan
+            else:
+                new_navdata[sv_idx_key] = np.nan
 
-        # Compute indices where gps_millis match, sort them
-        # sorting is done for consistency across all satellite pos. estimation
-        # algorithms as ephemerismanager inherently sorts based on prns
-        idxs = np.where(navdata["gps_millis"] == timestep)[0]
-        sorted_idxs = idxs[np.argsort(navdata["sv_id", idxs], axis = 0)]
-
-        if verbose:
-            print(t_idx, timestep, idxs, sorted_idxs)
-            print('misc: ', navdata['gps_millis', sorted_idxs], \
-                            navdata['gnss_id', sorted_idxs], \
-                            navdata['sv_id', sorted_idxs], \
-                            )
-
-        visible_sats = np.atleast_1d(navdata["sv_id", sorted_idxs])
-
-        for sv_idx, prn in enumerate(visible_sats):
-
-            prn = int(prn)
-
-            # continue if no sp3 or clk data availble
-            if len(sp3_parsed_file[prn].tym) == 0 \
-                or len(clk_parsed_file[prn].tym) == 0:
-                continue
-
-            # Perform nearest time step search to compute iref values for sp3 and clk
-            sp3_iref = np.argmin(abs(np.array(sp3_parsed_file[prn].tym) - \
-                                     (timestep - navdata_offset) ))
-            clk_iref = np.argmin(abs(np.array(clk_parsed_file[prn].tym) - \
-                                     (timestep - navdata_offset) ))
+    if inplace:
+        iterate_navdata = navdata
+    else:
+        iterate_navdata = new_navdata
 
+    for row_idx, row in enumerate(iterate_navdata):
+        gnss_sv_id = str(row["gnss_sv_id"])
+        # continue if no sp3 or clk data availble
+        if gnss_sv_id not in sp3_parsed_file["gnss_sv_id"] \
+          or gnss_sv_id not in clk_parsed_file["gnss_sv_id"] \
+          or len(sp3_parsed_file.where("gnss_sv_id",gnss_sv_id)) == 0 \
+          or len(clk_parsed_file.where("gnss_sv_id",gnss_sv_id)) == 0: continue
+
+        timestep = row["gps_millis"]
+
+        # Perform nearest time step search to compute iref values for sp3 and clk
+        sp3_iref = np.argmin(abs(np.array(sp3_parsed_file.where("gnss_sv_id",
+                            gnss_sv_id)["gps_millis"]) - timestep ))
+        clk_iref = np.argmin(abs(np.array(clk_parsed_file.where("gnss_sv_id",
+                            gnss_sv_id)["gps_millis"]) - timestep ))
+
+        # Carry out .sp3 processing by first checking if
+        # previous interpolated function holds
+        if gnss_sv_id in sp3_iref_old and sp3_iref == sp3_iref_old[gnss_sv_id]:
+            func_satpos = satfunc_xyz_old[gnss_sv_id]
+        else:
+            # if does not hold, recompute the interpolation function based on current iref
             if verbose:
-                print('Stats: ', t_idx, timestep, prn, idxs, sorted_idxs)
-                print('sp3 stats: ', sp3_iref, sp3_iref_old[prn])
-                print('clk stats: ', clk_iref, clk_iref_old[prn])
-
-            # Carry out .sp3 processing by first checking if
-            # previous interpolated function holds
-            if sp3_iref == sp3_iref_old[prn]:
-                func_satpos = satfunc_xyz_old[prn]
-            else:
-                # if does not hold, recompute the interpolation function based on current iref
-                if verbose:
-                    print('SP3: Computing new interpolation!')
-                func_satpos = extract_sp3(sp3_parsed_file[prn], \
-                                               sp3_iref, method = interp_method)
-                # Update the relevant interp function and iref values
-                satfunc_xyz_old[prn] = func_satpos
-                sp3_iref_old[prn] = sp3_iref
-
-            # Compute satellite position and velocity using interpolated function
-            satpos_sp3, satvel_sp3 = sp3_snapshot(func_satpos, \
-                                                          (timestep - navdata_offset), \
-                                                          method = interp_method)
-
-            # Adjust the satellite position based on Earth's rotation
-            trans_time = navdata["raw_pr_m", sorted_idxs[sv_idx]] / consts.C
-            del_x = (consts.OMEGA_E_DOT * satpos_sp3[1] * trans_time)
-            del_y = (-consts.OMEGA_E_DOT * satpos_sp3[0] * trans_time)
-            satpos_sp3[0] = satpos_sp3[0] + del_x
-            satpos_sp3[1] = satpos_sp3[1] + del_y
-
-            # Carry out .clk processing by first checking if previous interpolated
-            # function holds
-            if clk_iref == clk_iref_old[prn]:
-                func_satbias = satfunc_t_old[prn]
-            else:
-                # if does not hold, recompute the interpolation function based on current iref
-                if verbose:
-                    print('CLK: Computing new interpolation!')
-                func_satbias = extract_clk(clk_parsed_file[prn], \
-                                                clk_iref, method = interp_method)
-                # Update the relevant interp function and iref values
-                satfunc_t_old[prn] = func_satbias
-                clk_iref_old[prn] = clk_iref
-
-            # Compute satellite clock bias and drift using interpolated function
-            satbias_clk, \
-            satdrift_clk = clk_snapshot(func_satbias, \
-                                                (timestep - navdata_offset), \
-                                                method = interp_method)
+                print('SP3: Computing new interpolation for',gnss_sv_id)
+            func_satpos = sp3_parsed_file.extract_sp3(gnss_sv_id,
+                                                      sp3_iref)
+            # Update the relevant interp function and iref values
+            satfunc_xyz_old[gnss_sv_id] = func_satpos
+            sp3_iref_old[gnss_sv_id] = sp3_iref
+
+        # Compute satellite position and velocity using interpolated function
+        satpos_sp3, satvel_sp3 = sp3_parsed_file.sp3_snapshot(func_satpos, timestep)
+
+        # Adjust the satellite position based on Earth's rotation
+        trans_time = row["raw_pr_m"] / consts.C
+        del_x = consts.OMEGA_E_DOT * satpos_sp3[1] * trans_time
+        del_y = -consts.OMEGA_E_DOT * satpos_sp3[0] * trans_time
+        satpos_sp3[0] = satpos_sp3[0] + del_x
+        satpos_sp3[1] = satpos_sp3[1] + del_y
+
+        # Carry out .clk processing by first checking if previous interpolated
+        # function holds
+        if gnss_sv_id in clk_iref_old and clk_iref == clk_iref_old[gnss_sv_id]:
+            func_satbias = satfunc_t_old[gnss_sv_id]
+        else:
+            # if does not hold, recompute the interpolation function based on current iref
             if verbose:
-                print('after sp3:', satpos_sp3, \
-                                    satvel_sp3, \
-                                    consts.C * satbias_clk, \
-                                    consts.C * satdrift_clk)
-
-                satpos_android = np.transpose([ navdata["x_sv_m", sorted_idxs], \
-                                                navdata["y_sv_m", sorted_idxs], \
-                                                navdata["z_sv_m", sorted_idxs] ])
-                print( 'Android-sp3 Pos Error (m): ', \
-                          np.linalg.norm(satpos_android[sv_idx] - satpos_sp3), \
-                          navdata["x_sv_m", sorted_idxs[sv_idx]] - satpos_sp3[0], \
-                          navdata["y_sv_m", sorted_idxs[sv_idx]] - satpos_sp3[1], \
-                          navdata["z_sv_m", sorted_idxs[sv_idx]] - satpos_sp3[2] )
-
-                satvel_android = np.transpose([ navdata["vx_sv_mps", sorted_idxs], \
-                                                   navdata["vy_sv_mps", sorted_idxs], \
-                                                   navdata["vz_sv_mps", sorted_idxs] ])
-                print('android:', satpos_android[sv_idx], satvel_android[sv_idx])
-                print('Android-sp3 Vel Error (m): ', \
-                          np.linalg.norm(satvel_android[sv_idx] - satvel_sp3), \
-                          navdata["vx_sv_mps", sorted_idxs[sv_idx]] - satvel_sp3[0], \
-                          navdata["vy_sv_mps", sorted_idxs[sv_idx]] - satvel_sp3[1], \
-                          navdata["vz_sv_mps", sorted_idxs[sv_idx]] - satvel_sp3[2] )
-
-                print('Android-sp3 Clk Error (m): ', \
-                          navdata["b_sv_m", sorted_idxs[sv_idx]] - consts.C * satbias_clk, \
-                          navdata["b_dot_sv_mps", sorted_idxs[sv_idx]] - consts.C * satdrift_clk)
-                print(' ')
+                print('CLK: Computing new interpolation for',gnss_sv_id)
+            func_satbias = clk_parsed_file.extract_clk(gnss_sv_id,
+                                                       clk_iref)
+            # Update the relevant interp function and iref values
+            satfunc_t_old[gnss_sv_id] = func_satbias
+            clk_iref_old[gnss_sv_id] = clk_iref
+
+        # Compute satellite clock bias and drift using interpolated function
+        satbias_clk, satdrift_clk = clk_parsed_file.clk_snapshot(func_satbias, timestep)
 
+        if inplace:
             # update *_sv_m of navdata with the estimated values from .sp3 files
-            navdata['x_sv_m', sorted_idxs[sv_idx]] = np.array([satpos_sp3[0]])
-            navdata['y_sv_m', sorted_idxs[sv_idx]] = np.array([satpos_sp3[1]])
-            navdata['z_sv_m', sorted_idxs[sv_idx]] = np.array([satpos_sp3[2]])
+            navdata['x_sv_m', row_idx] = np.array([satpos_sp3[0]])
+            navdata['y_sv_m', row_idx] = np.array([satpos_sp3[1]])
+            navdata['z_sv_m', row_idx] = np.array([satpos_sp3[2]])
 
             # update v*_sv_mps of navdata with the estimated values from .sp3 files
-            navdata["vx_sv_mps", sorted_idxs[sv_idx]] = np.array([satvel_sp3[0]])
-            navdata["vy_sv_mps", sorted_idxs[sv_idx]] = np.array([satvel_sp3[1]])
-            navdata["vz_sv_mps", sorted_idxs[sv_idx]] = np.array([satvel_sp3[2]])
+            navdata["vx_sv_mps", row_idx] = np.array([satvel_sp3[0]])
+            navdata["vy_sv_mps", row_idx] = np.array([satvel_sp3[1]])
+            navdata["vz_sv_mps", row_idx] = np.array([satvel_sp3[2]])
 
             # update clock data of navdata with the estimated values from .clk files
-            navdata["b_sv_m", sorted_idxs[sv_idx]] = np.array([consts.C * satbias_clk])
-            navdata["b_dot_sv_mps", sorted_idxs[sv_idx]] = np.array([consts.C * satdrift_clk])
-
-    return navdata
-
-def multi_gnss_from_precise_eph(navdata, sp3_path, clk_path, \
-                                        constellations, verbose = False):
-    """Compute satellite information using .sp3 and .clk for multiple GNSS
-
-    Parameters
-    ----------
-    navdata : gnss_lib_py.parsers.navdata.NavData
-        Instance of the NavData class that depicts android derived dataset
-    sp3_path : path
-        File path for .sp3 file to extract precise ephemerides
-    clk_path : path
-        File path for .clk file to extract precise ephemerides
-    constellations : array-like
-        The GNSS constellations for which you want to extract precise
-        ephemeris, (e.g. ['gps','glonass'])
-    verbose : bool
-        Flag (True/False) for whether to print intermediate steps useful
-        for debugging/reviewing (the default is False)
-
-    Returns
-    -------
-    navdata : gnss_lib_py.parsers.navdata.NavData
-        Updated NavData class with satellite information computed using
-        precise ephemerides from .sp3 and .clk files
-    """
-
-    navdata_prcs_merged = NavData()
-    for sv in constellations:
-        navdata_prcs_gnss = navdata.where('gnss_id', sv)
-
-        sp3_parsed_gnss = parse_sp3(sp3_path, constellation = sv)
-        clk_parsed_gnss = parse_clockfile(clk_path, constellation = sv)
-        derived_prcs_gnss = single_gnss_from_precise_eph(navdata_prcs_gnss, \
-                                                                 sp3_parsed_gnss, \
-                                                                 clk_parsed_gnss, \
-                                                                 verbose = verbose)
-        navdata_prcs_merged.concat(navdata_prcs_gnss, inplace=True)
-
-    return navdata_prcs_merged
-
-def sv_gps_from_brdcst_eph(navdata, verbose = False):
-    """Compute satellite information using .n for any GNSS constellation
-
-    Parameters
-    ----------
-    navdata : gnss_lib_py.parsers.navdata.NavData
-        Instance of the NavData class that depicts android derived dataset
-    verbose : bool
-        Flag (True/False) for whether to print intermediate steps useful
-        for debugging/reviewing (the default is False)
-
-    Returns
-    -------
-    navdata : gnss_lib_py.parsers.navdata.NavData
-        Updated NavData class with satellite information computed using
-        broadcast ephemerides from .n files
-    """
-    navdata_offset = 0 #1000 # Set this to zero, when android errors get fixed
-    unique_gnss_id = np.unique(navdata['gnss_id'])
-    if len(unique_gnss_id)==1:
-        if unique_gnss_id == 'gps':
-            # Need this string to create sv_id strings for ephemeris manager
-            unique_gnss_id_str = 'G'
+            navdata["b_sv_m", row_idx] = np.array([satbias_clk])
+            navdata["b_dot_sv_mps", row_idx] = np.array([satdrift_clk])
         else:
-            raise RuntimeError("No non-GPS capability yet")
-    else:
-        raise RuntimeError("Multi-GNSS constellations cannot be updated simultaneously")
+            # update *_sv_m of navdata with the estimated values from .sp3 files
+            new_navdata['x_sv_m', row_idx] = np.array([satpos_sp3[0]])
+            new_navdata['y_sv_m', row_idx] = np.array([satpos_sp3[1]])
+            new_navdata['z_sv_m', row_idx] = np.array([satpos_sp3[2]])
 
-    repo = EphemerisManager()
-    unique_timesteps = np.unique(navdata["gps_millis"])
+            # update v*_sv_mps of navdata with the estimated values from .sp3 files
+            new_navdata["vx_sv_mps", row_idx] = np.array([satvel_sp3[0]])
+            new_navdata["vy_sv_mps", row_idx] = np.array([satvel_sp3[1]])
+            new_navdata["vz_sv_mps", row_idx] = np.array([satvel_sp3[2]])
 
-    for t_idx, timestep in enumerate(unique_timesteps):
-        # Compute indices where gps_millis match, sort them
-        # sorting is done for consistency across all satellite pos. estimation
-        # algorithms as ephemerismanager inherently sorts based on prns
-        idxs = np.where(navdata["gps_millis"] == timestep)[0]
-        sorted_idxs = idxs[np.argsort(navdata["sv_id", idxs], axis = 0)]
-
-        # compute ephem information using desired_sats, rxdatetime
-        desired_sats = [unique_gnss_id_str + str(int(i)).zfill(2) \
-                                           for i in navdata["sv_id", sorted_idxs]]
-        rxdatetime = datetime(1980, 1, 6, 0, 0, 0, tzinfo=timezone.utc) + \
-                     timedelta( seconds = (timestep - navdata_offset) * 1e-3 )
-        ephem = repo.get_ephemeris(rxdatetime, satellites = desired_sats)
-
-        if verbose:
-            print(t_idx, timestep, idxs, sorted_idxs)
-            print('misc: ', navdata['gps_millis', sorted_idxs], \
-                            navdata['gnss_id', sorted_idxs], \
-                            navdata['sv_id', sorted_idxs], \
-                            desired_sats, rxdatetime)
-
-            satpos_android = np.transpose([ navdata["x_sv_m", sorted_idxs], \
-                                            navdata["y_sv_m", sorted_idxs], \
-                                            navdata["z_sv_m", sorted_idxs] ])
-            satvel_android = np.transpose([ navdata["vx_sv_mps", sorted_idxs], \
-                                               navdata["vy_sv_mps", sorted_idxs], \
-                                               navdata["vz_sv_mps", sorted_idxs] ])
-            print('android:', satpos_android, satvel_android)
-
-        # compute satellite position and velocity based on ephem and gps_time
-        # Transform satellite position to account for earth's rotation
-        gps_week, gps_tow = gps_millis_to_tow(timestep - navdata_offset)
-        get_sat_from_ephem = find_sat(ephem, gps_tow, gps_week)
-        satpos_ephemeris = np.transpose([get_sat_from_ephem["x_sv_m"], \
-                                         get_sat_from_ephem["y_sv_m"], \
-                                         get_sat_from_ephem["z_sv_m"]])
-        satvel_ephemeris = np.transpose([get_sat_from_ephem["vx_sv_mps"], \
-                                         get_sat_from_ephem["vy_sv_mps"], \
-                                         get_sat_from_ephem["vz_sv_mps"]])
-        trans_time = navdata["raw_pr_m", sorted_idxs] / consts.C
-        del_x = (consts.OMEGA_E_DOT * satpos_ephemeris[:,1] * trans_time)
-        del_y = (-consts.OMEGA_E_DOT * satpos_ephemeris[:,0] * trans_time)
-        satpos_ephemeris[:,0] = satpos_ephemeris[:,0] + del_x
-        satpos_ephemeris[:,1] = satpos_ephemeris[:,1] + del_y
-
-        if verbose:
-            print('after ephemeris:', satpos_ephemeris, satvel_ephemeris)
-            print('nav-android Pos Error: ', \
-                      np.linalg.norm(satpos_ephemeris - satpos_android, axis=1) )
-            print('nav-android Vel Error: ', \
-                      np.linalg.norm(satvel_ephemeris - satvel_android, axis=1) )
-            print(' ')
-
-        # update *_sv_m of navdata with the estimated values from .n files
-        navdata["x_sv_m", sorted_idxs] = satpos_ephemeris[:,0]
-        navdata["y_sv_m", sorted_idxs] = satpos_ephemeris[:,1]
-        navdata["z_sv_m", sorted_idxs] = satpos_ephemeris[:,2]
-
-        # update v*_sv_mps of navdata with the estimated values from .n files
-        navdata["vx_sv_mps", sorted_idxs] = satvel_ephemeris[:,0]
-        navdata["vy_sv_mps", sorted_idxs] = satvel_ephemeris[:,1]
-        navdata["vz_sv_mps", sorted_idxs] = satvel_ephemeris[:,2]
+            # update clock data of navdata with the estimated values from .clk files
+            new_navdata["b_sv_m", row_idx] = np.array([satbias_clk])
+            new_navdata["b_dot_sv_mps", row_idx] = np.array([satdrift_clk])
 
-    return navdata
+    if inplace:
+        return None
+    return new_navdata
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/parsers/smart_loc.py` & `gnss_lib_py-0.2.0/gnss_lib_py/parsers/smartloc.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(self, input_path):
         """TU Chemnitz raw specific loading and preprocessing.
 
         Should input path to RXM-RAWX.csv file.
 
         Parameters
         ----------
-        input_path : string
+        input_path : string or path-like
             Path to measurement csv file
 
         """
 
         super().__init__(csv_path=input_path, sep=";")
 
     def postprocess(self):
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/utils/constants.py` & `gnss_lib_py-0.2.0/gnss_lib_py/utils/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 
 WEEKSEC = 604800
 """ int : Number of seconds in a week [s]."""
 
 GPS_EPOCH_0 = datetime(1980, 1, 6, 0, 0, 0, 0, tzinfo=timezone.utc)
 """ datetime.datetime: Starting time for GPS epoch"""
 
+MILLIS_PER_DAY = 86400000
+
 TROPO_DELAY_C1 = 2.47
 """float : First coefficient of simplified tropospheric delay model developed in [1]_."""
 
 TROPO_DELAY_C2 = 0.0121
 """float : Second coefficient of simplified tropospheric delay model developed in [1]_."""
 
 TROPO_DELAY_C3 = 1.33e-4
@@ -83,7 +85,14 @@
                        'S':'sbas',
                        'C':'beidou',
                        'E':'galileo',
                        'J':'qzss',
                        'I':'irnss',
                        }
 """dict : Satellite System identifier from Rinex specification p13 in [2]_."""
+
+NUMSATS = {'gps': (32),
+            'galileo': (36),
+            'beidou': (46),
+            'glonass': (24),
+            'qzss': (3)}
+"""dict : Number of satellites, for identifiers from Rinex specification p13 in [2]_."""
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/utils/coordinates.py` & `gnss_lib_py-0.2.0/gnss_lib_py/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/utils/file_operations.py` & `gnss_lib_py-0.2.0/gnss_lib_py/utils/file_operations.py`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/utils/filters.py` & `gnss_lib_py-0.2.0/gnss_lib_py/utils/filters.py`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/utils/sim_gnss.py` & `gnss_lib_py-0.2.0/gnss_lib_py/utils/gnss_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,761 +1,642 @@
-"""Generates expected measurements and simulates pseudoranges.
-
-Functions to generate expected measurements and to simulate pseudoranges
-and doppler for GPS satellites.
+"""Model GNSS measurements and measurement corrections.
 
+Functions to generate expected measurements, simulate noisy mesurements,
+and estimate pseudorange corrections (clock corrections, ionospheric and
+tropospheric delays) for given receiver states and time.
 """
 
 __authors__ = "Ashwin Kanhere, Bradley Collicott"
-__date__ = "16 July 2021"
+__date__ = "17 Jan, 2023"
+
+import warnings
 
 import numpy as np
-import pandas as pd
 from numpy.random import default_rng
 
 import gnss_lib_py.utils.constants as consts
-from gnss_lib_py.utils.coordinates import ecef_to_geodetic
-from gnss_lib_py.utils.time_conversions import gps_millis_to_tow
+from gnss_lib_py.utils.coordinates import ecef_to_geodetic, ecef_to_el_az
 from gnss_lib_py.parsers.navdata import NavData
-# TODO: Check if any of the functions are sorting the dataframe w.r.t SV while
-# processing the measurements
-
-
-def sats_from_el_az(elaz_deg):
-    """Generate NED satellite positions at given elevation and azimuth.
-
-    Given elevation and azimuth angles are with respect to the receiver.
-    Generated satellites are in the NED frame of reference with the receiver
-    position as the origin.
-
-    Parameters
-    ----------
-    elaz_deg : np.ndarray
-        Nx2 array of elevation and azimuth angles [degrees]
-
-    Returns
-    -------
-    sats_ned : np.ndarray
-        Nx3 satellite NED positions, simulated at a distance of 20,200 km
-    """
-    assert np.shape(elaz_deg)[1] == 2, "elaz_deg should be a Nx2 array"
-    el = np.deg2rad(elaz_deg[:, 0])
-    az = np.deg2rad(elaz_deg[:,1])
-    unit_vect = np.zeros([3, np.shape(elaz_deg)[0]])
-    unit_vect[0, :] = np.sin(az)*np.cos(el)
-    unit_vect[1, :] = np.cos(az)*np.cos(el)
-    unit_vect[2, :] = np.sin(el)
-    sats_ned = np.transpose(20200000*unit_vect)
-    return sats_ned
-
-
-def _extract_pos_vel_arr(sv_posvel):
-    """Extract satellite positions and velocities into numpy arrays.
-
-    Parameters
-    ----------
-    sv_posvel : pd.DataFrame
-        Dataframe with satellite states
+from gnss_lib_py.utils.time_conversions import gps_millis_to_tow
+from gnss_lib_py.utils.sv_models import find_visible_ephem, _extract_pos_vel_arr, \
+                        find_sv_location, find_sv_states, \
+                        find_visible_sv_posvel, _sort_ephem_measures, \
+                        _filter_ephemeris_measurements
+from gnss_lib_py.utils.ephemeris_downloader import DEFAULT_EPHEM_PATH
+
+
+def add_measures(measurements, state_estimate,
+                 ephemeris_path = DEFAULT_EPHEM_PATH, iono_params=None,
+                 pseudorange=True, doppler=True, corrections=True,
+                 delta_t_dec = -2):
+    """Estimate measurements and add to given navdata with rx measures.
+
+    Given measurements that were received, containing time, GNSS ID and
+    SV ID, computes estimated pseudorange and doppler measurements and
+    adds them to the input navdata.
+
+    If the input navdata does not contain SV positions and velocities,
+    which are required to estimate measurements, they are added to the
+    navdata as well.
+
+    Must contain rows:
+    * :code:`gps_millis`
+    * :code:`gnss_id`
+    * :code:`sv_id`
+
+    To use previously computed SV states, provide following rows:
+    * :code:`x_sv_m`
+    * :code:`y_sv_m`
+    * :code:`z_sv_m`
+    * :code:`vx_sv_mps`
+    * :code:`vy_sv_mps`
+    * :code:`vz_sv_mps`
+
+    To estimate the expected measurements, the receiver state is needed.
+    This state is stored in `state_estimate` and must contain the
+    following rows
+    * :code:`x_rx*_m`
+    * :code:`y_rx*_m`
+    * :code:`z_rx*_m`
+    * :code:`vx_rx*_mps`
+    * :code:`vy_rx*_mps`
+    * :code:`vz_rx*_mps`
+
+
+    Parameters
+    ----------
+    measurements : gnss_lib_py.parsers.navdata.NavData
+        Received measurements for which SV states are required. Must
+        contain `gps_millis`, `gnss_id`, and `sv_id` fields.
+    state_estimate : gnss_lib_py.parsers.navdata.NavData
+        Estimate for receiver states --- ECEF x, y, and z positions in meters,
+        ECEF x, y, and z velocities in meters, clock bias in meters, and
+        the clock drift in meters per second --- stored in a NavData instance.
+    ephemeris_path : string or path-like
+        Location where ephemeris files are stored. Files will be
+        downloaded if they don't exist for the given date and constellation.
+    iono_params : np.ndarray
+        Parameters to calculate the ionospheric delay in pseudoranges.
+    pseudorange : bool
+        Flag on whether pseudoranges are to be calculated and used or not.
+    doppler : bool
+        Flag on whether doppler measurements are to be calculated and
+        used or not.
+    corrections : bool
+        Flag on whether pseudorange corrections are to be calculated and
+        used or not.
+    delta_t_dec : int
+        Decimal places after which times are considered as belonging to
+        the same discrete time interval.
 
-    Returns
-    -------
-    prns : List
-        Satellite PRNs in input DataFrame
-    sv_pos : ndarray
-        ECEF satellite positions
-    sv_vel : ndarray
-        ECEF satellite x, y and z velocities
-    """
+    Notes
+    -----
+    In some cases, such as when using derived versions of the collected
+    data from the Google Decimeter Challenge, the measurements contain
+    state estimates in the same data structure as the received measurements.
+    In such a case, a separate `state_estimate` can be generated using
+    the particular class' method for generating a separate `state_estimate`.
+    """
+    constellations = np.unique(measurements['gnss_id'])
+    if iono_params is None:
+        measurements, ephem, iono_params = _filter_ephemeris_measurements(
+            measurements, constellations, ephemeris_path, get_iono=True)
+    else:
+        measurements, ephem, _ = _filter_ephemeris_measurements(
+            measurements, constellations, ephemeris_path, get_iono=False)
+    info_rows = ['gps_millis', 'gnss_id', 'sv_id']
+    sv_state_rows = ['x_sv_m', 'y_sv_m', 'z_sv_m',
+                     'vx_sv_mps', 'vy_sv_mps', 'vz_sv_mps',
+                     'b_sv_m']
+    rx_pos_rows_to_find = ['x_rx*_m', 'y_rx*_m', 'z_rx*_m']
+    rx_pos_rows_idxs = state_estimate.find_wildcard_indexes(
+                                            rx_pos_rows_to_find,
+                                            max_allow=1)
+    rx_pos_rows = [rx_pos_rows_idxs['x_rx*_m'][0],
+                   rx_pos_rows_idxs['y_rx*_m'][0],
+                   rx_pos_rows_idxs['z_rx*_m'][0]]
+    # velocity rows
+    rx_vel_rows_to_find = ['vx_rx*_mps', 'vy_rx*_mps', 'vz_rx*_mps']
+    # clock rows
+    rx_clk_rows_to_find = ['b_rx*_m', 'b_dot_rx*_mps']
+
+    est_measurements = NavData()
+    # Loop through the measurement file per time step
+    for gps_millis, _, measure_frame in measurements.loop_time('gps_millis',
+                                                        delta_t_decimals=delta_t_dec):
+        # Sort the satellites
+        rx_ephem, sorted_sats_ind, inv_sort_order = _sort_ephem_measures(measure_frame, ephem)
+        # Create new NavData with SV positions and velocities
+        # If they're not given, the SV states computed with measures will be used
+        try:
+            measure_frame.in_rows(sv_state_rows)
+            use_posvel = False
+            sv_posvel = NavData()
+            for row in sv_state_rows:
+                sv_posvel[row] = measure_frame[row]
+            for row in info_rows:
+                sv_posvel[row] = measure_frame[row]
+            # sv_posvel = sv_posvel.sort(ind=sorted_sats_ind)
+            sv_posvel = sv_posvel.sort(ind=sorted_sats_ind)
+        except KeyError:
+            sv_posvel = None
+            use_posvel = True
+
+        # Find the column of the state_estimate which best matches time
+        # from loop
+        state_col = np.argmin(np.abs(state_estimate['gps_millis'] - gps_millis))
+        # Extract RX states into State NavData
+        state = NavData()
+        for row in rx_pos_rows:
+            state[row] = state_estimate[row, state_col]
+        # velocity and clock rows
+        vel_clk_rows = rx_vel_rows_to_find + rx_clk_rows_to_find
+        for row in vel_clk_rows:
+            try:
+                row_idx = state_estimate.find_wildcard_indexes(row,max_allow=1)
+                state[row_idx[row][0]] = state_estimate[row_idx[row][0], state_col]
+            except KeyError:
+                warnings.warn("Assuming 0 "+ row + " for Rx", RuntimeWarning)
+                state[row] = 0
+
+        # Compute measurements
+        if pseudorange or doppler:
+            est_meas, sv_posvel = expected_measures(gps_millis, state,
+                                                    ephem=rx_ephem,
+                                                    sv_posvel=sv_posvel)
+            # Reverse the sorting to match the input measurements
+            est_meas = est_meas.sort(ind=inv_sort_order)
+        else:
+            est_meas = None
+        if corrections:
+            est_trp, est_iono = calculate_pseudorange_corr(gps_millis,
+                                    state=state, ephem=rx_ephem,
+                                    sv_posvel=sv_posvel, iono_params=iono_params)
+            # Reverse the sorting to match the input measurements
+            est_trp = est_trp[inv_sort_order]
+            est_iono = est_iono[inv_sort_order]
+        else:
+            est_trp = None
+            est_iono = None
+        # Add required values to new rows
+        if sv_posvel is not None:
+            # Reverse the sorting to match the input measurements
+            sv_posvel = sv_posvel.sort(ind=sorted_sats_ind)
+        est_frame = NavData()
+        if pseudorange:
+            est_frame['est_pr_m'] = est_meas['est_pr_m']
+        if doppler:
+            est_frame['est_doppler_hz'] = est_meas['est_doppler_hz']
+        if corrections:
+            est_frame['tropo_delay_m'] = est_trp
+            est_frame['iono_delay_m'] = est_iono
+        if use_posvel:
+            # Update the SV states with those estimated in this function
+            for row in sv_state_rows:
+                est_frame[row] = sv_posvel[row]
+        if len(est_measurements)==0:
+            est_measurements = est_frame
+        else:
+            est_measurements.concat(est_frame, inplace=True)
+    est_measurements = measurements.concat(est_measurements, axis=0, inplace=False)
+    return est_measurements
 
-    try:
-        prns   = [int(prn[1:]) for prn in sv_posvel.index]
-    except:
-        prns   = [int(prn) for prn in sv_posvel.index]
-    sv_pos = sv_posvel.filter(['x_sv_m', 'y_sv_m', 'z_sv_m'])
-    sv_vel   = sv_posvel.filter(['vx_sv_mps', 'vy_sv_mps', 'vz_sv_mps'])
-    sv_pos = sv_pos.to_numpy()
-    sv_vel   = sv_vel.to_numpy()
-    return prns, sv_pos, sv_vel
-    # TODO: Remove prns from function output if not needed
 
-def simulate_measures(gpsweek, gpstime, ephem, pos, bias, b_dot, vel,
-                      prange_sigma = 6., doppler_sigma=0.1, sv_posvel=None):
+def simulate_measures(gps_millis, state, noise_dict=None, ephem=None,
+                      sv_posvel=None, rng=None, el_mask=5.):
     """Simulate GNSS pseudoranges and doppler measurements given receiver state.
 
-    Measurements are simulated by adding Gaussian noise to measurements expected
-    based on the receiver states.
+    Measurements are simulated by finding satellites visible from the
+    given position (in state), computing the expected pseudorange and
+    doppler measurements for those satellites, corresponding to the given
+    state, and adding Gaussian noise to these expected measurements.
 
     Parameters
     ----------
-    gpsweek : int
-        Week in GPS calendar
-    gpstime : float
-        GPS time of the week for simulate measurements [s]
-    ephem : pd.DataFrame
-        DataFrame containing all satellite ephemeris parameters for gpsweek and
-        gpstime
-    pos : ndarray
-        1x3 Receiver 3D ECEF position [m]
-    bias : float
-        Receiver clock bais [m]
-    b_dot : float
-        Receiver clock drift [m/s]
-    vel : ndarray
-        1x3 Receiver 3D ECEF velocity
-    prange_sigma : float
-        Standard deviation of Gaussian error in simulated pseduranges
-    doppler_sigma : float
-        Standard deviation of Gaussian error in simulated doppler measurements
-    sv_posvel : pd.DataFrame
-        Precomputed positions of satellites (if available)
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    state : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing state i.e. 3D position, 3D velocity,
+        receiver clock bias and receiver clock drift rate at which
+        measurements have to be simulated.
+        Must be a single state (single column)
+    noise_dict : dict
+        Dictionary with pseudorange ('prange_sigma') and doppler noise
+        ('doppler_sigma') standard deviation values in [m] and [m/s].
+        If None, uses default values `prange_sigma=6` and
+        `doppler_sigma=1`.
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing satellite ephemeris parameters for a
+        particular time of ephemeris. Use None if not available and using
+        SV positions directly instead.
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Precomputed positions of satellites, set to None if not available.
+    rng : np.random.Generator
+        A random number generator for sampling random noise values.
+    el_mask: float
+        The elevation mask above which satellites are considered visible
+        from the given receiver position. Only visible sate.
 
     Returns
     -------
-    measurements : pd.DataFrame
-        Pseudorange and doppler measurements indexed by satellite SV with
-        Gaussian noise
-    sv_posvel : pd.DataFrame
-        Satellite positions and velocities (same as input if provided)
+    measurements : gnss_lib_py.parsers.navdata.NavData
+        Pseudorange (label: `prange`) and doppler (label: `doppler`)
+        measurements with satellite SV. Gaussian noise is added to
+        expected measurements to simulate stochasticity.
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Satellite positions and velocities (same as input if provided).
+
+    """
+    #TODO: Verify the default noise value for doppler range
+    #Handle default values
+    if rng is None:
+        rng = default_rng()
+
+    if noise_dict is None:
+        noise_dict = {}
+        noise_dict['prange_sigma'] = 6.
+        noise_dict['doppler_sigma'] = 1.
+
+    rx_ecef, _, _, _ = _extract_state_variables(state)
+
+    if ephem is not None:
+        ephem = find_visible_ephem(gps_millis, rx_ecef, ephem, el_mask=el_mask)
+        sv_posvel = None
+    else:
+        sv_posvel = find_visible_sv_posvel(rx_ecef, sv_posvel, el_mask=el_mask)
+        ephem = None
 
-    """
-    #TODO: Modify to work with input satellite positions
-    #TODO: Add assertions/error handling for sizes of position, bias, b_dot and
-    # velocity arrays
-    #TODO: Modify to use single state vector instead of multiple inputs
-    #TODO: Modify to use single dictionary with uncertainty values
-    ephem = _find_visible_sats(gpsweek, gpstime, pos, ephem)
-    measurements, sv_posvel = expected_measures(gpsweek, gpstime, ephem, pos,
-                                              bias, b_dot, vel, sv_posvel)
-    num_sats   = len(measurements.index)
-    rng = default_rng()
+    measurements, sv_posvel = expected_measures(gps_millis, state,
+                                                ephem, sv_posvel)
+    num_svs   = len(measurements)
+
+    # Create simulated measurements that match received naming convention
+    #TODO: Add clock and atmospheric delays here
+    measurements['raw_pr_m']  = (measurements['est_pr_m']
+        + noise_dict['prange_sigma'] *rng.standard_normal(num_svs))
 
-    measurements['prange']  = (measurements['prange']
-        + prange_sigma *rng.standard_normal(num_sats))
+    measurements['doppler_hz'] = (measurements['est_doppler_hz']
+        + noise_dict['doppler_sigma']*rng.standard_normal(num_svs))
 
-    measurements['doppler'] = (measurements['doppler']
-        + doppler_sigma*rng.standard_normal(num_sats))
+    # Remove expected measurements so they can be added later
+    measurements.remove(rows=['est_pr_m', 'est_doppler_hz'], inplace=True)
 
     return measurements, sv_posvel
 
-def expected_measures(gpsweek, gpstime, ephem, pos,
-                      bias, b_dot, vel, sv_posvel=None):
+
+def expected_measures(gps_millis, state, ephem=None, sv_posvel=None):
     """Compute expected pseudoranges and doppler measurements given receiver
     states.
 
     Parameters
     ----------
-    gpsweek : int
-        Week in GPS calendar
-    gpstime : float
-        GPS time of the week for simulate measurements [s]
-    ephem : pd.DataFrame
-        DataFrame containing all satellite ephemeris parameters for gpsweek and
-        gpstime
-    pos : ndarray
-        1x3 Receiver 3D ECEF position [m]
-    bias : float
-        Receiver clock bais [m]
-    b_dot : float
-        Receiver clock drift [m/s]
-    vel : ndarray
-        1x3 Receiver 3D ECEF velocity
-    sv_posvel : pd.DataFrame
-        Precomputed positions of satellites (if available)
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    state : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing state i.e. 3D position, 3D velocity,
+        receiver clock bias and receiver clock drift rate at which
+        measurements have to be simulated.
+        Must be a single state (single column)
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        NavData instance containing satellite ephemeris parameters for a
+        particular time of ephemeris, use None if not available and
+        using position directly.
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Precomputed positions of satellites (if available).
 
     Returns
     -------
-    measurements : pd.DataFrame
-        Expected pseudorange and doppler measurements indexed by satellite SV
-    sv_posvel : pd.DataFrame
-        Satellite positions and velocities (same as input if provided)
+    measurements : gnss_lib_py.parsers.navdata.NavData
+        Pseudorange (label: `prange`) and doppler (label: `doppler`)
+        measurements with satellite SV. Also contains SVs and gps_tow at
+        which the measurements are simulated.
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Satellite positions and velocities (same as input if provided).
     """
-    # NOTE: When using saved data, pass saved DataFrame with ephemeris in ephem
     # and satellite positions in sv_posvel
-    # TODO: Modify this function to use PRNS from measurement in addition to
-    # gpstime from measurement
-    pos = np.reshape(pos, [1, 3])
-    vel = np.reshape(vel, [1, 3])
-    sv_posvel, del_pos, true_range = _find_sv_location(gpsweek, gpstime,
-                                                         ephem, pos, sv_posvel)
+    rx_ecef, rx_v_ecef, clk_bias, clk_drift = _extract_state_variables(state)
+    sv_posvel, del_pos, true_range = find_sv_location(gps_millis,
+                                                         rx_ecef, ephem, sv_posvel)
     # sv_pos, sv_vel, del_pos are both Nx3
-    _, _, sv_vel = _extract_pos_vel_arr(sv_posvel)
+    _, sv_vel = _extract_pos_vel_arr(sv_posvel)
 
     # Obtain corrected pseudoranges and add receiver clock bias to them
-    prange = true_range + bias
-    # prange = (correct_pseudorange(gpstime, gpsweek, ephem, true_range,
-    #                              np.reshape(pos, [-1, 3])) + bias)
-    # TODO: Correction should be applied to the received pseudoranges, not
-    # modelled/expected pseudorange -- per discussion in meeting on 11/12
-    # TODO: Add corrections instead of returning corrected pseudoranges
-
-    # Obtain difference of velocity between satellite and receiver
+    prange = true_range
+    prange += clk_bias
 
-    del_vel = sv_vel - np.tile(np.reshape(vel, 3), [len(ephem), 1])
-    prange_rate = np.sum(del_vel*del_pos, axis=1)/true_range + b_dot
+    del_vel = sv_vel.reshape(3, -1) - np.tile(np.reshape(rx_v_ecef, [3,1]), [1, len(sv_posvel)])
+    prange_rate = np.sum(del_vel*del_pos, axis=0)/true_range
+    prange_rate += clk_drift
+    # Remove the hardcoded F1 below and change to frequency in measurements
     doppler = -(consts.F1/consts.C) * (prange_rate)
-
-    # doppler = pd.DataFrame(doppler, index=prange.index.copy())
-    measurements = pd.DataFrame(np.column_stack((prange, doppler)),
-                                index=sv_posvel.index,
-                                columns=['prange', 'doppler'])
+    measurements = NavData()
+    measurements['sv_id'] = sv_posvel['sv_id']
+    measurements['gnss_id'] = sv_posvel['gnss_id']
+    measurements['est_pr_m'] = prange
+    measurements['est_doppler_hz'] = doppler
     return measurements, sv_posvel
 
 
-def _find_visible_sats(gpsweek, gpstime, rx_ecef, ephem, el_mask=5.):
-    """Trim input ephemeris to keep only visible SVs.
-
-    Parameters
-    ----------
-    gpsweek : int
-        Week in GPS calendar
-    gpstime : float
-        GPS time of the week for simulate measurements [s]
-    rx_ecef : ndarray
-        1x3 row rx_pos ECEF position vector [m]
-    ephem  pd.DataFrame
-        DataFrame containing all satellite ephemeris parameters for gpsweek and
-        gpstime
-    el_mask : float
-        Minimum elevation of returned satellites
-
-    Returns
-    -------
-    eph : pd.DataFrame
-        Ephemeris parameters of visible satellites
-
-    """
-
-    # Find positions and velocities of all satellites
-    approx_posvel = find_sat(ephem, gpstime - consts.T_TRANS, gpsweek)
-
-    # Find elevation and azimuth angles for all satellites
-    _, approx_pos, _ = _extract_pos_vel_arr(approx_posvel)
-    approx_el_az = find_elaz(np.reshape(rx_ecef, [1, 3]), approx_pos)
-    # Keep attributes of only those satellites which are visible
-    keep_ind = approx_el_az[:,0] > el_mask
-    # prns = approx_posvel.index.to_numpy()[keep_ind]
-    # TODO: Remove above statement if superfluous
-    # TODO: Check that a copy of the ephemeris is being generated, also if it is
-    # needed
-    ephem_df = ephem.pandas_df()
-    eph = ephem_df.loc[keep_ind, :]
-    eph = NavData(pandas_df=eph)
-    return eph
-
-
-def _find_sv_location(gpsweek, gpstime, ephem, pos, sv_posvel=None):
-    """Return satellite positions, difference from rx_pos position and ranges.
+def _extract_state_variables(state):
+    """Extract position, velocity and clock bias terms from state.
 
     Parameters
     ----------
-    gpsweek : int
-        Week in GPS calendar
-    gpstime : float
-        GPS time of the week for simulate measurements [s]
-    ephem : pd.DataFrame
-        DataFrame containing all satellite ephemeris parameters for gpsweek and
-        gpstime
-    pos : ndarray
-        1x3 Receiver 3D ECEF position [m]
-    sv_posvel : pd.DataFrame
-        Precomputed positions of satellites (if available)
+    state : gnss_lib_py.parsers.navdata.NavData
+        NavData containing state values i.e. 3D position, 3D velocity,
+        receiver clock bias and receiver clock drift rate at which
+        measurements will be simulated.
 
     Returns
     -------
-    sv_posvel : pd.DataFrame
-        Satellite position and velocities (same if input)
-    del_pos : ndarray
-        Difference between satellite positions and receiver position
-    true_range : ndarray
-        Distance between satellite and receiver positions
-
-    """
-    pos = np.reshape(pos, [1, 3])
-    if sv_posvel is None:
-        satellites = len(ephem)
-        sv_posvel = find_sat(ephem, gpstime - consts.T_TRANS, gpsweek)
-        del_pos, true_range = _find_delxyz_range(sv_posvel, pos, satellites)
-        t_corr = true_range/consts.C
-
-        # Find satellite locations at (a more accurate) time of transmission
-        sv_posvel = find_sat(ephem, gpstime-t_corr, gpsweek)
-    else:
-        satellites = len(sv_posvel.index)
-    del_pos, true_range = _find_delxyz_range(sv_posvel, pos, satellites)
-    t_corr = true_range/consts.C
-    # Corrections for the rotation of the Earth during transmission
-    # _, sv_pos, sv_vel = _extract_pos_vel_arr(sv_posvel)
-    del_x = consts.OMEGA_E_DOT*sv_posvel['x_sv_m'] * t_corr
-    del_y = consts.OMEGA_E_DOT*sv_posvel['y_sv_m'] * t_corr
-    sv_posvel['x_sv_m'] = sv_posvel['x_sv_m'] + del_x
-    sv_posvel['y_sv_m'] = sv_posvel['y_sv_m'] + del_y
-    return sv_posvel, del_pos, true_range
+    rx_ecef : np.ndarray
+        3x1 Receiver 3D ECEF position [m].
+    rx_v_ecef : np.ndarray
+        3x1 Receiver 3D ECEF velocity.
+    clk_bias : float
+        Receiver clock bais [m].
+    clk_drift : float
+        Receiver clock drift [m/s].
+
+    """
+    assert len(state)==1, "Only single state accepted for GNSS simulation"
+
+    rx_idxs = state.find_wildcard_indexes(['x_rx*_m',
+                                           'y_rx*_m',
+                                           'z_rx*_m',
+                                           'vx_rx*_mps',
+                                           'vy_rx*_mps',
+                                           'vz_rx*_mps',
+                                           'b_rx*_m',
+                                           'b_dot_rx*_mps',
+                                           ],
+                                           max_allow=1)
+
+    rx_ecef = np.reshape(state[[rx_idxs['x_rx*_m'][0],
+                                rx_idxs['y_rx*_m'][0],
+                                rx_idxs['z_rx*_m'][0]]], [3,1])
+    rx_v_ecef = np.reshape(state[[rx_idxs['vx_rx*_mps'][0],
+                                  rx_idxs['vy_rx*_mps'][0],
+                                  rx_idxs['vz_rx*_mps'][0]]], [3,1])
+    clk_bias = state[rx_idxs['b_rx*_m'][0]]
+    clk_drift = state[rx_idxs['b_dot_rx*_mps'][0]]
+    return rx_ecef, rx_v_ecef, clk_bias, clk_drift
 
 
+def calculate_pseudorange_corr(gps_millis, state=None, ephem=None, sv_posvel=None,
+                                 iono_params=None):
+    """Incorporate corrections in measurements.
 
-def _find_delxyz_range(sv_posvel, pos, satellites):
-    """Return difference of satellite and rx_pos positions and range between them.
+    Incorporate clock corrections (relativistic and polynomial), tropospheric
+    and ionospheric atmospheric delay corrections.
 
     Parameters
     ----------
-    sv_posvel : pd.DataFrame
-        Satellite position and velocities
-    pos : ndarray
-        1x3 Receiver 3D ECEF position [m]
-    satellites : int
-        Number of satellites in sv_posvel
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    state : gnss_lib_py.parsers.navdata.NavData
+        NavData containing state values i.e. 3D position, 3D velocity,
+        receiver clock bias and receiver clock drift rate at which
+        measurements will be simulated.
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        Satellite ephemeris parameters for measurement SVs, use None if
+        using satellite positions instead.
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Precomputed positions of satellites corresponding to the input
+        `gps_millis`, set to None if not available.
+    iono_params : np.ndarray
+        Ionospheric atmospheric delay parameters for Klobuchar model,
+        passed in 2x4 array, use None if not available.
 
     Returns
     -------
-    del_pos : ndarray
-        Difference between satellite positions and receiver position
-    true_range : ndarray
-        Distance between satellite and receiver positions
-    """
-    # Repeating computation in find_sv_location
-    #NOTE: Input is from satellite finding in AE 456 code
-    pos = np.reshape(pos, [1, 3])
-    if np.size(pos)!=3:
-        raise ValueError('Position is not in XYZ')
-    _, sv_pos, _ = _extract_pos_vel_arr(sv_posvel)
-    del_pos = sv_pos - np.tile(np.reshape(pos, [-1, 3]), (satellites, 1))
-    true_range = np.linalg.norm(del_pos, axis=1)
-    return del_pos, true_range
+    tropo_delay : np.ndarray
+        Estimated delay caused by the troposhere [m].
+    iono_delay : np.ndarray
+        Estimated delay caused by the ionosphere [m].
 
 
-def find_sat(ephem, times, gpsweek):
-    """Compute position and velocities for all satellites in ephemeris file
-    given time of clock.
-
-    Parameters
-    ----------
-    ephem : pd.DataFrame
-        DataFrame containing ephemeris parameters of satellites for which states
-        are required
-    times : ndarray
-        GPS time of the week at which positions are required [s]
-    gpsweek : int
-        Week of GPS calendar corresponding to time of clock
-
-    Returns
-    -------
-    sv_posvel : pd.DataFrame
-        DataFrame indexed by satellite SV containing positions and velocities
-
     Notes
     -----
     Based on code written by J. Makela.
     AE 456, Global Navigation Sat Systems, University of Illinois
     Urbana-Champaign. Fall 2017
 
-    Satellite velocity calculations based on algorithms introduced in [1]_.
-
-    References
-    ----------
-    ..  [1] B. F. Thompson, S. W. Lewis, S. A. Brown, and T. M. Scott,
-        “Computing GPS satellite velocity and acceleration from the broadcast
-        navigation message,” NAVIGATION, vol. 66, no. 4, pp. 769–779, Dec. 2019,
-        doi: 10.1002/navi.342.
-
     """
-    # Satloc contains both positions and velocities.
-
-    # Extract parameters
-    c_is = ephem['C_is']
-    c_ic = ephem['C_ic']
-    c_rs = ephem['C_rs']
-    c_rc = ephem['C_rc']
-    c_uc = ephem['C_uc']
-    c_us = ephem['C_us']
-    M_0  = ephem['M_0']
-    dN   = ephem['deltaN']
-
-    ecc        = ephem['e']     # eccentricity
-    omega    = ephem['omega'] # argument of perigee
-    omega_0  = ephem['Omega_0']
-    sqrt_sma = ephem['sqrtA'] # sqrt of semi-major axis
-    sma      = sqrt_sma**2      # semi-major axis
-
-    ephem['GPSWeek'], ephem["tow"] = gps_millis_to_tow(ephem["gps_millis"])
-    sqrt_mu_A = np.sqrt(consts.MU_EARTH) * sqrt_sma**-3 # mean angular motion
-    gpsweek_diff = (np.mod(gpsweek,1024) - np.mod(ephem['GPSWeek'],1024))*604800.
-
-    # if np.size(times_all)==1:
-    #     times_all = times_all*np.ones(len(ephem))
-    # else:
-    #     times_all = np.reshape(times_all, len(ephem))
-    # times = times_all
-    sv_posvel = pd.DataFrame()
-    sv_posvel.loc[:,'sv'] = ephem["sv_id"]
-    sv_posvel.set_index('sv', inplace=True)
-    #TODO: Check if 'dt' or 'times' should be stored in the final DataFrame
-    sv_posvel.loc[:,'times'] = times
-
-    dt = times - ephem['t_oe'] + gpsweek_diff
-
-    # Calculate the mean anomaly with corrections
-    M_corr = dN * dt
-    M = M_0 + (sqrt_mu_A * dt) + M_corr
-
-    # Compute Eccentric Anomaly
-    E = _compute_eccentric_anomoly(M, ecc, tol=1e-5)
-
-    cos_E   = np.cos(E)
-    sin_E   = np.sin(E)
-    e_cos_E = (1 - ecc*cos_E)
-
-    # Calculate the true anomaly from the eccentric anomaly
-    sin_nu = np.sqrt(1 - ecc**2) * (sin_E/e_cos_E)
-    cos_nu = (cos_E-ecc) / e_cos_E
-    nu     = np.arctan2(sin_nu, cos_nu)
-
-    # Calcualte the argument of latitude iteratively
-    phi_0 = nu + omega
-    phi   = phi_0
-    for i in range(5):
-        cos_to_phi = np.cos(2.*phi)
-        sin_to_phi = np.sin(2.*phi)
-        phi_corr = c_uc * cos_to_phi + c_us * sin_to_phi
-        phi = phi_0 + phi_corr
-
-    # Calculate the longitude of ascending node with correction
-    omega_corr = ephem['OmegaDot'] * dt
-
-    # Also correct for the rotation since the beginning of the GPS week for which the Omega0 is
-    # defined.  Correct for GPS week rollovers.
-
-    # Also correct for the rotation since the beginning of the GPS week for
-    # which the Omega0 is defined.  Correct for GPS week rollovers.
-    omega = omega_0 - (consts.OMEGA_E_DOT*(times + gpsweek_diff)) + omega_corr
-
-    # Calculate orbital radius with correction
-    r_corr = c_rc * cos_to_phi + c_rs * sin_to_phi
-    r      = sma*e_cos_E + r_corr
-
-    ############################################
-    ######  Lines added for velocity (1)  ######
-    ############################################
-    dE   = (sqrt_mu_A + dN) / e_cos_E
-    dphi = np.sqrt(1 - ecc**2)*dE / e_cos_E
-    # Changed from the paper
-    dr   = (sma * ecc * dE * sin_E) + 2*(c_rs*cos_to_phi - c_rc*sin_to_phi)*dphi
-
-    # Calculate the inclination with correction
-    i_corr = c_ic*cos_to_phi + c_is*sin_to_phi + ephem['IDOT']*dt
-    i = ephem['i_0'] + i_corr
-
-    ############################################
-    ######  Lines added for velocity (2)  ######
-    ############################################
-    di = 2*(c_is*cos_to_phi - c_ic*sin_to_phi)*dphi + ephem['IDOT']
-
-    # Find the position in the orbital plane
-    xp = r*np.cos(phi)
-    yp = r*np.sin(phi)
-
-    ############################################
-    ######  Lines added for velocity (3)  ######
-    ############################################
-    du = (1 + 2*(c_us * cos_to_phi - c_uc*sin_to_phi))*dphi
-    dxp = dr*np.cos(phi) - r*np.sin(phi)*du
-    dyp = dr*np.sin(phi) + r*np.cos(phi)*du
-    # Find satellite position in ECEF coordinates
-    cos_omega = np.cos(omega)
-    sin_omega = np.sin(omega)
-    cos_i = np.cos(i)
-    sin_i = np.sin(i)
-
-    sv_posvel.loc[:,'x_sv_m'] = xp*cos_omega - yp*cos_i*sin_omega
-    sv_posvel.loc[:,'y_sv_m'] = xp*sin_omega + yp*cos_i*cos_omega
-    sv_posvel.loc[:,'z_sv_m'] = yp*sin_i
-    # TODO: Add satellite clock bias here using the 'clock corrections' not to
-    # be used but compared against SP3 and Android data
-
-    ############################################
-    ######  Lines added for velocity (4)  ######
-    ############################################
-    omega_dot = ephem['OmegaDot'] - consts.OMEGA_E_DOT
-    sv_posvel.loc[:,'vx_sv_mps'] = (dxp * cos_omega
-                         - dyp * cos_i*sin_omega
-                         + yp  * sin_omega*sin_i*di
-                         - (xp * sin_omega + yp*cos_i*cos_omega)*omega_dot)
-
-    sv_posvel.loc[:,'vy_sv_mps'] = (dxp * sin_omega
-                         + dyp * cos_i * cos_omega
-                         - yp  * sin_i * cos_omega * di
-                         + (xp * cos_omega - (yp*cos_i*sin_omega)) * omega_dot)
-
-    sv_posvel.loc[:,'vz_sv_mps'] = dyp*sin_i + yp*cos_i*di
-    return sv_posvel
-
-
-def correct_pseudorange(gpstime, gpsweek, ephem, pr_meas, rx_ecef=[[None]]):
-    """Incorporate corrections in measurements.
-
-    Incorporate clock corrections (relativistic, drift), tropospheric and
-    ionospheric clock corrections.
-
-    Parameters
-    ----------
-    gpstime : float
-        Time of clock in seconds of the week
-    gpsweek : int
-        GPS week for time of clock
-    ephem : pd.DataFrame
-        Satellite ephemeris parameters for measurement SVs
-    pr_meas : ndarray
-        Ranging measurements from satellites [m]
-    rx_ecef : ndarray
-        1x3 array of ECEF rx_pos position [m]
-
-    Returns
-    -------
-    pr_corr : ndarray
-        Array of corrected pseudorange measurements [m]
-
-    Notes
-    -----
-    Based on code written by J. Makela.
-    AE 456, Global Navigation Sat Systems, University of Illinois
-    Urbana-Champaign. Fall 2017
 
-    """
-    # TODO: Incorporate satellite clock rate changes into the doppler measurements
-    # TODO: Change default of rx to an array of None with size
-    # TODO: Change the sign for corrections to what will be added to expected measurements
-    # TODO: Return corrections instead of corrected measurements
-
-    # Extract parameters
-    # M_0  = ephem['M_0']
-    # dN   = ephem['deltaN']
-
-    e        = ephem['e']     # eccentricity
-    sqrt_sma = ephem['sqrtA'] # sqrt of semi-major axis
-
-    sqrt_mu_A = np.sqrt(consts.MU_EARTH) * sqrt_sma**-3 # mean angular motion
-
-    # Make sure gpstime and gpsweek are arrays
-    if not isinstance(gpstime, np.ndarray):
-        gpstime = np.array(gpstime)
-    if not isinstance(gpsweek, np.ndarray):
-        gpsweek = np.array(gpsweek)
-
-    # Initialize the correction array
-    pr_corr = pr_meas
-
-    dt = gpstime - ephem['t_oe']
-    if np.abs(dt).any() > 302400:
-        dt = dt - np.sign(dt)*604800
-
-    # Calculate the mean anomaly with corrections
-    M_corr = ephem['deltaN'] * dt
-    M      = ephem['M_0'] + (sqrt_mu_A * dt) + M_corr
-
-    # Compute Eccentric Anomaly
-    E = _compute_eccentric_anomoly(M, e, tol=1e-5)
-
-    # Determine pseudorange corrections due to satellite clock corrections.
-    # Calculate time offset from satellite reference time
-    t_offset = gpstime - ephem['t_oc']
-    if np.abs(t_offset).any() > 302400:
-        t_offset = t_offset-np.sign(t_offset)*604800
-
-    # Calculate clock corrections from the polynomial
-    # corr_polynomial = ephem.af0
-    #                 + ephem.af1*t_offset
-    #                 + ephem.af2*t_offset**2
-    corr_polynomial = (ephem['SVclockBias']
-                     + ephem['SVclockDrift']*t_offset
-                     + ephem['SVclockDriftRate']*t_offset**2)
-
-    # Calcualte the relativistic clock correction
-    corr_relativistic = consts.F * e * sqrt_sma * np.sin(E)
-
-    # Calculate the total clock correction including the Tgd term
-    clk_corr = (corr_polynomial - ephem['TGD'] + corr_relativistic)
+    if state is not None:
+        rx_ecef, _, _, _ = _extract_state_variables(state)
+    else:
+        rx_ecef = None
 
-    # NOTE: Removed ionospheric delay calculation here
 
-    # calculate clock pseudorange correction
-    pr_corr +=  clk_corr*consts.C
+    if ephem is not None:
+        satellites = len(ephem)
+    else:
+        assert sv_posvel is not None, \
+                "SV states must be given when ephemeris isn't"
+        satellites = len(sv_posvel)
 
-    if rx_ecef[0][0] is not None: # TODO: Reference using 2D array slicing
+    if rx_ecef is not None:
         # Calculate the tropospheric delays
-        tropo_delay = calculate_tropo_delay(gpstime, gpsweek, ephem, rx_ecef)
-        # Calculate total pseudorange correction
-        pr_corr -= tropo_delay*consts.C
-
-    if isinstance(pr_corr, pd.Series):
-        pr_corr = pr_corr.to_numpy(dtype=float)
-
-    # fill nans (fix for non-GPS satellites)
-    pr_corr = np.where(np.isnan(pr_corr), pr_meas, pr_corr)
+        tropo_delay = _calculate_tropo_delay(gps_millis, rx_ecef, ephem, sv_posvel)
+    else:
+        warnings.warn("Receiver position not given, returning 0 "\
+                    + "ionospheric delay", RuntimeWarning)
+        tropo_delay = np.zeros(satellites)
+
+    if iono_params is not None and rx_ecef is not None:
+        iono_delay = _calculate_iono_delay(gps_millis, iono_params,
+                                            rx_ecef, ephem, sv_posvel)
+    else:
+        warnings.warn("Ionospheric delay parameters or receiver position"\
+                    + "not given, returning 0 ionospheric delay", \
+                        RuntimeWarning)
+        iono_delay = np.zeros(satellites)
 
-    return pr_corr
+    return tropo_delay, iono_delay
 
 
-def calculate_tropo_delay(gpstime, gpsweek, ephem, rx_ecef):
+def _calculate_tropo_delay(gps_millis, rx_ecef, ephem=None, sv_posvel=None):
     """Calculate tropospheric delay
 
     Parameters
     ----------
-    gpstime : float
-        Time of clock in seconds of the week
-    gpsweek : int
-        GPS week for time of clock
-    ephem : pd.DataFrame
-        Satellite ephemeris parameters for measurement SVs
-    rx_ecef : ndarray
-        1x3 array of ECEF rx_pos position [m]
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    rx_ecef : np.ndarray
+        3x1 array of ECEF rx_pos position [m].
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        Satellite ephemeris parameters for measurement SVs.
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Precomputed positions of satellites, set to None if not available.
 
     Returns
     -------
-    tropo_delay : ndarray
-        Tropospheric corrections to pseudorange measurements
+    tropo_delay : np.ndarray
+        Tropospheric corrections to pseudorange measurements [m].
 
     Notes
     -----
     Based on code written by J. Makela.
     AE 456, Global Navigation Sat Systems, University of Illinois
     Urbana-Champaign. Fall 2017
 
     """
-
-    # Make sure things are arrays
-    if not isinstance(gpstime, np.ndarray):
-        gpstime = np.array(gpstime)
-    if not isinstance(gpsweek, np.ndarray):
-        gpsweek = np.array(gpsweek)
+    # Make sure that receiver position is 3x1
+    rx_ecef = np.reshape(rx_ecef, [3,1])
 
     # Determine the satellite locations
-    sv_posvel = find_sat(ephem, gpstime, gpsweek)
-    _, sv_pos, _ = _extract_pos_vel_arr(sv_posvel)
+    if sv_posvel is None:
+        assert ephem is not None, "Must provide ephemeris or positions" \
+                        + " to find troposphere delay"
+        sv_posvel = find_sv_states(gps_millis, ephem)
+    sv_pos, _ = _extract_pos_vel_arr(sv_posvel)
+    sv_pos = sv_pos.reshape(3, -1)
 
     # compute elevation and azimuth
-    el_az = find_elaz(rx_ecef, sv_pos)
-    el_r  = np.deg2rad(el_az[:,0])
+    el_az = ecef_to_el_az(rx_ecef, sv_pos)
+    el_r  = np.deg2rad(el_az[0, :])
 
     # Calculate the WGS-84 latitude/longitude of the receiver
     rx_lla = ecef_to_geodetic(rx_ecef)
-    height = rx_lla[:,2]
+    height = rx_lla[2, :]
 
     # Force height to be positive
     ind = np.argwhere(height < 0).flatten()
-    if len(ind) > 0:
+    if len(ind) > 0:  # pragma: no cover
         height[ind] = 0
 
     # Calculate the delay
-    # TODO: Store these numbers somewhere, we should know where they're from -BC
-    c_1 = 2.47
-    c_2 = 0.0121
-    c_3 = 1.33e-4
-    tropo_delay = c_1/(np.sin(el_r)+c_2) * np.exp(-height*c_3)/consts.C
+    tropo_delay = consts.TROPO_DELAY_C1/(np.sin(el_r)+consts.TROPO_DELAY_C2) \
+                     * np.exp(-height*consts.TROPO_DELAY_C3)/consts.C
 
+    # Convert tropospheric delaly in equivalent meters
+    tropo_delay = consts.C*tropo_delay
     return tropo_delay
 
 
-def find_elaz(rx_pos, sv_pos):
-    """Calculate the elevation and azimuth from a single receiver to multiple
-    satellites.
+def _calculate_iono_delay(gps_millis, iono_params, rx_ecef, ephem=None,
+                          sv_posvel=None, constellation="gps"):
+    """Calculate the ionospheric delay in pseudorange using the Klobuchar
+    model Section 5.3.2 [1]_.
 
     Parameters
     ----------
-    rx_pos : ndarray
-        1x3 vector containing [X, Y, Z] coordinate of receiver
-    sv_pos : ndarray
-        Nx3 array  containing [X, Y, Z] coordinates of satellites
+    gps_millis : int
+        Time at which measurements are needed, measured in milliseconds
+        since start of GPS epoch [ms].
+    iono_params : np.ndarray
+        Ionospheric atmospheric delay parameters for Klobuchar model,
+        passed in 2x4 array, use None if not available.
+    rx_ecef : np.ndarray
+        3x1 receiver position in ECEF frame of reference [m], use None
+        if not available.
+    ephem : gnss_lib_py.parsers.navdata.NavData
+        Satellite ephemeris parameters for measurement SVs, use None if
+        using satellite positions instead.
+    sv_posvel : gnss_lib_py.parsers.navdata.NavData
+        Precomputed positions of satellites corresponding to the input
+        `gps_millis`, set to None if not available.
+    constellation : string
+        Constellation used for the ionospheric parameters addition.
 
     Returns
     -------
-    el_az : ndarray
-        Nx2 array containing the elevation and azimuth from the
-        receiver to the requested satellites. Elevation and azimuth are
-        given in decimal degrees.
+    iono_delay : np.ndarray
+        Estimated delay caused by the ionosphere [m].
 
     Notes
     -----
-    Code written by J. Makela.
+    Based on code written by J. Makela.
     AE 456, Global Navigation Sat Systems, University of Illinois
     Urbana-Champaign. Fall 2017
 
+    References
+    ----------
+    ..  [1] Misra, P. and Enge, P,
+        "Global Positioning System: Signals, Measurements, and Performance."
+        2nd Edition, Ganga-Jamuna Press, 2006.
+
     """
+    _, gps_tow = gps_millis_to_tow(gps_millis)
 
-    # check for 1D case:
-    dim = len(rx_pos.shape)
-    if dim == 1:
-        rx_pos = np.reshape(rx_pos,(1,3))
-
-    dim = len(sv_pos.shape)
-    if dim == 1:
-        sv_pos = np.reshape(sv_pos,(1,3))
-
-    # Convert the receiver location to WGS84
-    rx_lla = ecef_to_geodetic(rx_pos)
-    assert np.shape(rx_lla)==(1,3)
-
-    # Create variables with the latitude and longitude in radians
-    lat = np.deg2rad(rx_lla[0,0])
-    lon = np.deg2rad(rx_lla[0,1])
-
-    # Create the 3 x 3 transform matrix from ECEF to ecef_to_ven
-    cos_lon = np.cos(lon)
-    cos_lat = np.cos(lat)
-    sin_lon = np.sin(lon)
-    sin_lat = np.sin(lat)
-    ecef_to_ven = np.array([[ cos_lat*cos_lon,  cos_lat*sin_lon, sin_lat],
-                            [-sin_lon        ,  cos_lon        , 0.     ],
-                            [-sin_lat*cos_lon, -sin_lat*sin_lon, cos_lat]])
-
-    # Replicate the rx_pos array to be the same size as the satellite array
-    rx_array = np.ones_like(sv_pos) * rx_pos
-
-    # Calculate the pseudorange for each satellite
-    p = sv_pos - rx_array
-
-    # Calculate the length of this vector
-    n = np.array([np.sqrt(p[:,0]**2 + p[:,1]**2 + p[:,2]**2)])
-
-    # Create the normalized unit vector
-    p = p / (np.ones_like(p) * n.T)
-
-    # Perform the transform of the normalized pseudorange from ECEF to VEN
-    p_ven = np.dot(ecef_to_ven, p.T)
-
-    # Calculate elevation and azimuth in degrees
-    el_az = np.zeros([sv_pos.shape[0],2])
-    el_az[:,0] = np.rad2deg((np.pi/2. - np.arccos(p_ven[0,:])))
-    el_az[:,1] = np.rad2deg(np.arctan2(p_ven[1,:],p_ven[2,:]))
-
-    return el_az
-
-def _compute_eccentric_anomoly(M, e, tol=1e-5, max_iter=10):
-    """Compute the eccentric anomaly from mean anomaly using the Newton-Raphson
-    method using equation: f(E) = M - E + e * sin(E) = 0.
+    #Reshape receiver position to 3x1
+    rx_ecef = np.reshape(rx_ecef, [3,1])
 
-    Parameters
-    ----------
-    M : pd.DataFrame
-        Mean Anomaly of GNSS satellite orbits
-    e : pd.DataFrame
-        Eccentricity of GNSS satellite orbits
-    tol : float
-        Tolerance for Newton-Raphson convergence
-    max_iter : int
-        Maximum number of iterations for Newton-Raphson
+    # Determine the satellite locations
+    if sv_posvel is None:
+        assert ephem is not None, "Must provide ephemeris or positions" \
+                                + " to find visible satellites"
+        sv_posvel = find_sv_states(gps_millis, ephem)
+    sv_pos, _ = _extract_pos_vel_arr(sv_posvel)
+    sv_pos = sv_pos.reshape(3, -1)
+    el_az = ecef_to_el_az(rx_ecef, sv_pos)
+    el_r = np.deg2rad(el_az[0, :])
+    az_r = np.deg2rad(el_az[1, :])
 
-    Returns
-    -------
-    E : pd.DataFrame
-        Eccentric Anomaly of GNSS satellite orbits
+    # Calculate the WGS-84 latitude/longitude of the receiver
+    wgs_llh = ecef_to_geodetic(rx_ecef)
+    lat_r = np.deg2rad(wgs_llh[0, :])
+    lon_r = np.deg2rad(wgs_llh[1, :])
+
+    # Parse the ionospheric parameters
+    alpha = iono_params[constellation][0,:]
+    beta = iono_params[constellation][1,:]
 
-    """
-    E = M
-    for _ in np.arange(0, max_iter):
-        f    = M - E + e * np.sin(E)
-        dfdE = e*np.cos(E) - 1.
-        dE   = -f / dfdE
-        E    = E + dE
+    # Calculate the psi angle
+    psi = 0.1356/(el_r+0.346) - 0.0691
+
+    # Calculate the ionospheric geodetic latitude
+    lat_i = lat_r + psi * np.cos(az_r)
+
+    # Make sure values are in bounds
+    ind = np.argwhere(np.abs(lat_i) > 1.3090)
+    if len(ind) > 0:
+        lat_i[ind] = 1.3090 * np.sign(lat_i[ind])  # pragma: no cover
+    # Calculate the ionospheric geodetic longitude
+    lon_i = lon_r + psi * np.sin(az_r)/np.cos(lat_i)
+
+    # Calculate the solar time corresponding to the gps_tow
+    solar_time = 1.3751e4 * lon_i + gps_tow
+
+    # Make sure values are in bounds
+    solar_time = np.mod(solar_time,86400)
+
+    # Calculate the geomagnetic latitude (semi-circles)
+    lat_m = (lat_i + 2.02e-1 * np.cos(lon_i - 5.08))/np.pi
+    # Calculate the period
+    period = beta[0]+beta[1]*lat_m+beta[2]*lat_m**2+beta[3]*lat_m**3
+
+    # Make sure values are in bounds
+    ind = np.argwhere(period < 72000).flatten()
+    if len(ind) > 0:
+        period[ind] = 72000  # pragma: no cover
+
+    # Calculate the local time angle
+    theta = 2*np.pi*(solar_time - 50400) / period
 
-    if any(dE > tol):
-        print("Eccentric Anomaly may not have converged: dE = ", dE)
+    # Calculate the amplitude term
+    amp = (alpha[0]+alpha[1]*lat_m+alpha[2]*lat_m**2+alpha[3]*lat_m**3)
+
+    # Make sure values are in bounds
+    ind = np.argwhere(amp < 0).flatten()
+    if len(ind) > 0:
+        amp[ind] = 0  # pragma: no cover
+
+    # Calculate the slant factor
+    slant_fact = 1.0 + 5.16e-1 * (1.6755-el_r)**3
+
+    # Calculate the ionospheric delay
+    iono_delay = slant_fact * 5.0e-9
+    ind = np.argwhere(np.abs(theta) < np.pi/2.).flatten()
+    if len(ind) > 0:
+        iono_delay[ind] = slant_fact[ind]* \
+            (5e-9+amp[ind]*(1-theta[ind]**2/2.+theta[ind]**4/24.))
 
-    return E
+    # Convert ionospheric delay to equivalent meters
+    iono_delay = consts.C*iono_delay
+    return iono_delay
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gnss_lib_py-0.1.9/gnss_lib_py/utils/visualizations.py` & `gnss_lib_py-0.2.0/gnss_lib_py/utils/visualizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,14 +281,15 @@
 
     # create new figure
     fig = plt.figure(figsize=(6,4.5))
     axes = fig.add_subplot(111, projection='polar')
 
     navdata = navdata.copy()
     navdata["az_sv_rad"] = np.radians(navdata["az_sv_deg"])
+    navdata = navdata.where("el_sv_deg",0,"geq")
 
     for c_idx, constellation in enumerate(_sort_gnss_ids(np.unique(navdata["gnss_id"]))):
         const_subset = navdata.where("gnss_id",constellation)
         color = "C" + str(c_idx % len(STANFORD_COLORS))
         cmap = _new_cmap(to_rgb(color))
         marker = MARKERS[c_idx % len(MARKERS)]
         const_label_created = False
@@ -804,14 +805,16 @@
     # assumed Mercator projection
     margin = 2.5
     height = (maxlat - minlat) * margin * width_to_height
     width = (maxlon - minlon) * margin
     lon_zoom = np.interp(width , lon_zoom_range, range(20, 0, -1))
     lat_zoom = np.interp(height, lon_zoom_range, range(20, 0, -1))
     zoom = floor(min(lon_zoom, lat_zoom))
+    # zoom level higher than 18 won't load load properly as of June 2023
+    zoom = min(zoom, 18)
 
     return zoom, center
 
 def _save_plotly(figures, titles=None, prefix="", fnames=None,
                  width=730, height=520): # pragma: no cover
     """Saves figures to file.
```

### Comparing `gnss_lib_py-0.1.9/pyproject.toml` & `gnss_lib_py-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gnss-lib-py"
-version = "0.1.9"
+version = "0.2.0"
 description = "Modular Python tool for parsing, analyzing, and visualizing Global Navigation Satellite Systems (GNSS) data and state estimates"
 authors = ["Derek Knowles <dcknowles@stanford.edu>",
            "Ashwin Kanhere <akanhere@stanford.edu>",
            ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Stanford-NavLab/gnss_lib_py"
```

### Comparing `gnss_lib_py-0.1.9/PKG-INFO` & `gnss_lib_py-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: gnss-lib-py
-Version: 0.1.9
+Version: 0.2.0
 Summary: Modular Python tool for parsing, analyzing, and visualizing Global Navigation Satellite Systems (GNSS) data and state estimates
 Home-page: https://github.com/Stanford-NavLab/gnss_lib_py
 License: MIT
 Keywords: gnss
 Author: Derek Knowles
 Author-email: dcknowles@stanford.edu
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: DateTime (>=4.3,<5.0)
 Requires-Dist: georinex (>=1.15.0,<2.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
@@ -59,15 +58,15 @@
 measurements into state estimates and visualization tools for measurements
 and state estimates.
 The modularity of `gnss_lib_py` is made possibly by the unifying
 `NavData` class, which contains methods to add, remove and modify
 numeric and string data consistently.
 We provide standard row names for `NavData` elements on the
 [reference page](https://gnss-lib-py.readthedocs.io/en/latest/reference/reference.html).
-These names ensure cross compatability between different datasets and
+These names ensure cross compatibility between different datasets and
 algorithms.
 
 Documentation
 -------------
 Full documentation is available on our [readthedocs website](https://gnss-lib-py.readthedocs.io/en/latest/index.html).
 
 
@@ -114,15 +113,19 @@
   * The data parsers in the `parsers` directory allow for either loading
     GNSS data into `gnss_lib_py`'s unifying `NavData` class or parsing
     precise ephemerides data.
     Currently, the following datasets and types are supported:
 
       * [2021 Google Android Derived Dataset](https://www.kaggle.com/c/google-smartphone-decimeter-challenge)
       * [2022 Google Android Derived Dataset](https://www.kaggle.com/competitions/smartphone-decimeter-2022)
-      * [Precise Ephemeris Data](https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/gnss_mgex.html)
+      * [TU Chemnitz smartLoc Dataset](https://www.tu-chemnitz.de/projekt/smartLoc/gnss_dataset.html.en#Datasets)
+      * [NMEA](https://www.sparkfun.com/datasheets/GPS/NMEA%20Reference%20Manual-Rev2.1-Dec07.pdf)
+      * [RINEX .o and .n](https://files.igs.org/pub/data/format/rinex305.pdf)
+      * [SP3 precise orbits](https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/orbit_products.html)
+      * [CLK clock products](https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/clock_products.html)
 
   * The `utils` directory contains utilities used to handle
     GNSS measurements, time conversions, visualizations, satellite
     simulation, file operations, etc.
 
 Installation
 ------------
```

