# Comparing `tmp/pyspk-1.7.tar.gz` & `tmp/pyspk-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspk-1.7.tar", last modified: Fri Jun 23 09:52:03 2023, max compression
+gzip compressed data, was "pyspk-1.8.tar", last modified: Sun Aug  6 16:51:03 2023, max compression
```

## Comparing `pyspk-1.7.tar` & `pyspk-1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-23 09:52:03.540349 pyspk-1.7/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.7/LICENSE.md
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.7/MANIFEST.in
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9142 2023-06-23 09:52:03.540180 pyspk-1.7/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     8621 2023-06-23 09:38:54.000000 pyspk-1.7/README.md
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-23 09:52:03.538313 pyspk-1.7/pyspk/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.7/pyspk/__init__.py
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-23 09:52:03.539961 pyspk-1.7/pyspk/__pycache__/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2023-06-21 11:12:32.000000 pyspk-1.7/pyspk/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     2169 2023-06-21 11:12:32.000000 pyspk-1.7/pyspk/__pycache__/fit_vals.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    14959 2023-06-21 11:12:32.000000 pyspk-1.7/pyspk/__pycache__/model.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.7/pyspk/fit_vals.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    16374 2023-06-23 09:38:28.000000 pyspk-1.7/pyspk/model.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.7/pyspk/stat_errors_200.csv
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.7/pyspk/stat_errors_500.csv
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-23 09:52:03.539411 pyspk-1.7/pyspk.egg-info/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9142 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      411 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/SOURCES.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/dependency_links.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/requires.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/top_level.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-06-23 09:52:03.540384 pyspk-1.7/setup.cfg
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-06-23 09:39:01.000000 pyspk-1.7/setup.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-08-06 16:51:03.369616 pyspk-1.8/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.8/LICENSE.md
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.8/MANIFEST.in
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    10567 2023-08-06 16:51:03.369425 pyspk-1.8/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    10046 2023-08-06 16:49:32.000000 pyspk-1.8/README.md
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-08-06 16:51:03.367512 pyspk-1.8/pyspk/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.8/pyspk/__init__.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-08-06 16:51:03.369113 pyspk-1.8/pyspk/__pycache__/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2023-06-21 11:12:32.000000 pyspk-1.8/pyspk/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     2169 2023-06-21 11:12:32.000000 pyspk-1.8/pyspk/__pycache__/fit_vals.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    14959 2023-06-21 11:12:32.000000 pyspk-1.8/pyspk/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.8/pyspk/fit_vals.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    18307 2023-08-06 16:49:32.000000 pyspk-1.8/pyspk/model.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.8/pyspk/stat_errors_200.csv
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.8/pyspk/stat_errors_500.csv
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-08-06 16:51:03.368547 pyspk-1.8/pyspk.egg-info/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    10567 2023-08-06 16:51:03.000000 pyspk-1.8/pyspk.egg-info/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      411 2023-08-06 16:51:03.000000 pyspk-1.8/pyspk.egg-info/SOURCES.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-08-06 16:51:03.000000 pyspk-1.8/pyspk.egg-info/dependency_links.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-08-06 16:51:03.000000 pyspk-1.8/pyspk.egg-info/requires.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-08-06 16:51:03.000000 pyspk-1.8/pyspk.egg-info/top_level.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-08-06 16:51:03.369653 pyspk-1.8/setup.cfg
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-08-06 16:49:32.000000 pyspk-1.8/setup.py
```

### Comparing `pyspk-1.7/LICENSE.md` & `pyspk-1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyspk-1.7/PKG-INFO` & `pyspk-1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.7
+Version: 1.8
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -69,37 +69,68 @@
 
 We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
 $$f_b/(\Omega_b/\Omega_m)= \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
-Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
+Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 4 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
 
 ```
 import pyspk.model as spk
 from astropy.cosmology import FlatLambdaCDM
 
 H0 = 70 
-Omega_b = 0.0463
 Omega_m = 0.2793
 
-cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m, Ob0=Omega_b) 
+cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m) 
 
 alpha = 4.189
 beta = 1.273
 gamma = 0.298
 z = 0.5
 
 k, sup = spk.sup_model(SO=500, z=z, alpha=alpha, beta=beta, gamma=gamma, cosmo=cosmo)
 ```
 
-### Method 3: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
+### Method 3: Redshift-dependent double power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
+
+We implemented a redshift-dependent double power-law fit to the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
+
+$$f_b/(\Omega_b/\Omega_m)= \frac{1}{2} \epsilon \left[\left(\frac{M_{500c}}{M_{\mathrm{pivot}}}\right)^{\alpha} + \left(\frac{M_{500c}}{M_{\mathrm{pivot}}}\right)^{\beta}\right] \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
+
+where $\epsilon$ sets the normalisation at the pivot point, $M_{\mathrm{pivot}}$, in units of $\mathrm{M}_ {\odot}$, $\alpha$ and $\beta$ are the power-law slopes at low and high mass respectively, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
+
+We find that this double redshift-dependent double power-law form provides a good fit to the whole range of baryon fractions in the ANTILLES simulations. 
+
+In the following example we use the redshift-dependent double power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
+
+```
+import pyspk.model as spk
+from astropy.cosmology import FlatLambdaCDM
+
+H0 = 68.0 
+Omega_m = 0.306
+
+cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m) 
+
+epsilon = 0.410
+alpha = -0.385
+beta = 0.451
+gamma = 0.125
+m_pivot = 1e13
+z = 0.2
+
+k, sup = spk.sup_model(SO=500, z=z, epsilon=epsilon, alpha=alpha, beta=beta, gamma=gamma, m_pivot=m_pivot, cosmo=cosmo)
+```
+
+
+### Method 4: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
 
 The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations (McCarthy et al. 2017), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
 
 
 ## Priors
 
 While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from the fits in Table 5 in Akino et al. (2022), and find the subset of simulations from our 400 models that agree to within $\pm 2$ or $3 \times \sigma$ of the inferred baryon budget at redshift $z=0.1$. We note that for our simulations, we include all stellar and gas particles within a spherical overdensity radius. Hence, in order to make reasonable comparisons with the fits in Akino et al. (2022), we included an additional 15\% contribution to the total stellar masses from the contribution of blue galaxies, and 30\% additional stellar mass to the brightest cluster galaxies (BCGs) to account for the diffuse intracluster light (ICL, see Akino et al. 2022).
```

### Comparing `pyspk-1.7/README.md` & `pyspk-1.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -56,37 +56,68 @@
 
 We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
 $$f_b/(\Omega_b/\Omega_m)= \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
-Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
+Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 4 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
 
 ```
 import pyspk.model as spk
 from astropy.cosmology import FlatLambdaCDM
 
 H0 = 70 
-Omega_b = 0.0463
 Omega_m = 0.2793
 
-cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m, Ob0=Omega_b) 
+cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m) 
 
 alpha = 4.189
 beta = 1.273
 gamma = 0.298
 z = 0.5
 
 k, sup = spk.sup_model(SO=500, z=z, alpha=alpha, beta=beta, gamma=gamma, cosmo=cosmo)
 ```
 
-### Method 3: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
+### Method 3: Redshift-dependent double power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
+
+We implemented a redshift-dependent double power-law fit to the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
+
+$$f_b/(\Omega_b/\Omega_m)= \frac{1}{2} \epsilon \left[\left(\frac{M_{500c}}{M_{\mathrm{pivot}}}\right)^{\alpha} + \left(\frac{M_{500c}}{M_{\mathrm{pivot}}}\right)^{\beta}\right] \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
+
+where $\epsilon$ sets the normalisation at the pivot point, $M_{\mathrm{pivot}}$, in units of $\mathrm{M}_ {\odot}$, $\alpha$ and $\beta$ are the power-law slopes at low and high mass respectively, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
+
+We find that this double redshift-dependent double power-law form provides a good fit to the whole range of baryon fractions in the ANTILLES simulations. 
+
+In the following example we use the redshift-dependent double power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
+
+```
+import pyspk.model as spk
+from astropy.cosmology import FlatLambdaCDM
+
+H0 = 68.0 
+Omega_m = 0.306
+
+cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m) 
+
+epsilon = 0.410
+alpha = -0.385
+beta = 0.451
+gamma = 0.125
+m_pivot = 1e13
+z = 0.2
+
+k, sup = spk.sup_model(SO=500, z=z, epsilon=epsilon, alpha=alpha, beta=beta, gamma=gamma, m_pivot=m_pivot, cosmo=cosmo)
+```
+
+
+### Method 4: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
 
 The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations (McCarthy et al. 2017), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
 
 
 ## Priors
 
 While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from the fits in Table 5 in Akino et al. (2022), and find the subset of simulations from our 400 models that agree to within $\pm 2$ or $3 \times \sigma$ of the inferred baryon budget at redshift $z=0.1$. We note that for our simulations, we include all stellar and gas particles within a spherical overdensity radius. Hence, in order to make reasonable comparisons with the fits in Akino et al. (2022), we included an additional 15\% contribution to the total stellar masses from the contribution of blue galaxies, and 30\% additional stellar mass to the brightest cluster galaxies (BCGs) to account for the diffuse intracluster light (ICL, see Akino et al. 2022).
```

### Comparing `pyspk-1.7/pyspk/__pycache__/fit_vals.cpython-38.pyc` & `pyspk-1.8/pyspk/__pycache__/fit_vals.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyspk-1.7/pyspk/__pycache__/model.cpython-38.pyc` & `pyspk-1.8/pyspk/__pycache__/model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyspk-1.7/pyspk/fit_vals.py` & `pyspk-1.8/pyspk/fit_vals.py`

 * *Files identical despite different names*

### Comparing `pyspk-1.7/pyspk/model.py` & `pyspk-1.8/pyspk/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .fit_vals import best_fit_vals as _best_fit_vals
 from .fit_vals import limits as _limits
 import warnings as _warnings
 import pkgutil as _pkgutil
 
 _warnings.filterwarnings("always", category=UserWarning)
 
+
 def _power_law(m_halo, fb_a, fb_pow, fb_pivot=1):
     """
     Simple power-law function fit to the baryon fraction - halo mass relation
 
     Parameters
     ----------
     m_halo: array of float
@@ -200,15 +201,15 @@
     inter_max_x0 = _Akima1DInterpolator(_limits[str(SO)]['z'], _limits[str(SO)]['max_x0'])
     inter_max_x1 = _Akima1DInterpolator(_limits[str(SO)]['z'], _limits[str(SO)]['max_x1'])
     inter_max_x2 = _Akima1DInterpolator(_limits[str(SO)]['z'], _limits[str(SO)]['max_x2'])
 
     min_fb = 10 ** (inter_min_x0(z) + inter_min_x1(z) * _np.log10(m_halo) + inter_min_x2(z) * _np.log10(m_halo) ** 2)
     max_fb = 10 ** (inter_max_x0(z) + inter_max_x1(z) * _np.log10(m_halo) + inter_max_x2(z) * _np.log10(m_halo) ** 2)
 
-    return min_fb, max_fb
+    return min_fb * 0.8, max_fb * 1.2
 
 
 def _get_params(SO, z):
     """
     Computes the best fit parameters for the SP(k) model at a specific redshift. 
 
     Parameters
@@ -264,17 +265,54 @@
     A = _np.exp(alpha) / 100
     B = _np.power(m_halo / 1e14, beta - 1)
     C = _np.power(cosmo.efunc(z) / cosmo.efunc(0.3), gamma)
 
     return A * B * C
 
 
+def _double_power_law(epsilon, alpha, beta, gamma, m_pivot, m_halo, z, cosmo):
+    """
+    Returns a redshift dependent double power-law function of the baryon fraction 
+    as a function of halo mass.
+
+    Parameters
+    ----------
+    epsilon : float
+        normalization parameter.
+    alpha : float
+        power-law slope at low mass.
+    beta : float
+        power-law slope at high mass.
+    gamma : float
+        sets redshift dependence of the normalisation. 
+    m_pivot : float
+        double power law pivot point in M_sun units. 
+    m_halo: array of float
+        halo mass in M_sun units.
+    z : float
+        redshift z
+    cosmo: astropy cosmology object
+        astropy cosmology object with the desired cosmology
+        
+    Returns
+    -------
+    output: array of float
+        baryon fraction normalised by the Universal baryon fraction: f_b / (Omega_b / Omega_m)
+    """
+
+    A = 0.5 * epsilon * _np.power(cosmo.efunc(z) / cosmo.efunc(0.3), gamma)
+    B = _np.power(m_halo / m_pivot, alpha)
+    C = _np.power(m_halo / m_pivot, beta)
+
+    return A * (B + C)
+
+
 def sup_model(SO, z, fb_a=None, fb_pow=None, fb_pivot=1, M_halo=None, fb=None, extrapolate=False,
-              alpha=None, beta=None, gamma=None, cosmo=None, k_array=None, k_min=0.1, k_max=8, n=100, 
-              errors=False, verbose=False):
+              epsilon=None, alpha=None, beta=None, gamma=None, m_pivot=None, cosmo=None, 
+              k_array=None, k_min=0.1, k_max=8, n=100, errors=False, verbose=False):
     """
     Returns the suppression of the total matter power spectrum as a function of scale 'k' using the SP(k) model.
     Automatically selects the required optimal mass as a function of scale and redshift. Requires the baryon 
     fraction - halo mass relation, either by specifying power-law fitting parameters, or non-parametric 
     proving arrays with fb and M_halo at a specific redshift. The function accepts a simple power law form 
     or an Akino et al 2022 fucntional form. If a non-parametric relation is given, an 
     interpolator is used to compute fb at the optimal mass. 
@@ -295,20 +333,24 @@
         array containing the (binned) baryon fraction normalised by the universal baryon fraction: 
         f_b / (Omega_b / Omega_m) for the fb - M-halo relation.
     M_halo : array of float, optional
         array containing the (binned) halo mass for the fb - M-halo relation in M_sun units.
         For interpolation, out-of-bounds points return NaNs.
     extrapolate: boolean, default False
         Whether to extrapolate to out-of-bounds points based on first and last intervals, or to return NaNs.
+    epsilon : float
+        normalization parameter for double power-law form.
     alpha : float, optional
-        sets the Akino power law constant
+        sets the Akino power law constant, or power-law slope at low mass for double power-law form.
     beta : float, optional
-        sets the Akino power law exponent
+        sets the Akino power law exponent, or power-law slope at high mass for double power-law form.
     gamma : float, optional
-        sets the Akino power law redshift dependence. 
+        sets the redshift dependence for Akino or double power-law form. 
+    m_pivot : float
+        double power law pivot point in M_sun units.
     cosmo: astropy cosmology object, optional
         astropy cosmology object with the desired cosmology
     k_array : array of float, optional
         array containing the desired co-moving wavenumber in units [h/Mpc]. If given, k_min, k_max and n are ignored.
     k_min : float, default 0.1
         minimum co-moving wavenumber in units [h/Mpc]
     k_max : float, default 8, max 12
@@ -395,14 +437,25 @@
             if extrapolate:
                 fb_inter.extrapolate = True
             f_b = 10 ** fb_inter(best_mass)
         except:
             raise Exception('\033[91mWhen using binned data, both halo mass and baryon '
                             'fraction should be given as monotonically increasing arrays. '
                             'Please specify: M_halo (array) and fb (array). \033[0m')
+
+    elif (epsilon is not None) or (m_pivot is not None):
+        if verbose:
+            print('\033[36mUsing double power law for fb - M_halo at z=%.3f \033[0m' % z)
+        try:
+            f_b = _double_power_law(epsilon, alpha, beta, gamma, m_pivot, 10 ** best_mass, z, cosmo)
+        except:
+            raise Exception('\033[91mUsing double power-law. '
+                            'Please specify: epsilon, alpha, beta, gamma, '
+                            'm_pivot and cosmology (cosmo) \033[0m') from None
+
     else:
         if verbose:
             print('\033[36mUsing an Akino et al. 2022 power-law fit for fb ' 
                   '- M_halo at z=%.3f. \033[0m' % z)
         try:
             f_b = _akino(alpha, beta, gamma, 10 ** best_mass, z, cosmo)
         except:
```

### Comparing `pyspk-1.7/pyspk/stat_errors_200.csv` & `pyspk-1.8/pyspk/stat_errors_200.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.7/pyspk/stat_errors_500.csv` & `pyspk-1.8/pyspk/stat_errors_500.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.7/pyspk.egg-info/PKG-INFO` & `pyspk-1.8/pyspk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.7
+Version: 1.8
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -69,37 +69,68 @@
 
 We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
 $$f_b/(\Omega_b/\Omega_m)= \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
-Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
+Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 4 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
 
 ```
 import pyspk.model as spk
 from astropy.cosmology import FlatLambdaCDM
 
 H0 = 70 
-Omega_b = 0.0463
 Omega_m = 0.2793
 
-cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m, Ob0=Omega_b) 
+cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m) 
 
 alpha = 4.189
 beta = 1.273
 gamma = 0.298
 z = 0.5
 
 k, sup = spk.sup_model(SO=500, z=z, alpha=alpha, beta=beta, gamma=gamma, cosmo=cosmo)
 ```
 
-### Method 3: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
+### Method 3: Redshift-dependent double power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
+
+We implemented a redshift-dependent double power-law fit to the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
+
+$$f_b/(\Omega_b/\Omega_m)= \frac{1}{2} \epsilon \left[\left(\frac{M_{500c}}{M_{\mathrm{pivot}}}\right)^{\alpha} + \left(\frac{M_{500c}}{M_{\mathrm{pivot}}}\right)^{\beta}\right] \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
+
+where $\epsilon$ sets the normalisation at the pivot point, $M_{\mathrm{pivot}}$, in units of $\mathrm{M}_ {\odot}$, $\alpha$ and $\beta$ are the power-law slopes at low and high mass respectively, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
+
+We find that this double redshift-dependent double power-law form provides a good fit to the whole range of baryon fractions in the ANTILLES simulations. 
+
+In the following example we use the redshift-dependent double power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
+
+```
+import pyspk.model as spk
+from astropy.cosmology import FlatLambdaCDM
+
+H0 = 68.0 
+Omega_m = 0.306
+
+cosmo = FlatLambdaCDM(H0=H0, Om0=Omega_m) 
+
+epsilon = 0.410
+alpha = -0.385
+beta = 0.451
+gamma = 0.125
+m_pivot = 1e13
+z = 0.2
+
+k, sup = spk.sup_model(SO=500, z=z, epsilon=epsilon, alpha=alpha, beta=beta, gamma=gamma, m_pivot=m_pivot, cosmo=cosmo)
+```
+
+
+### Method 4: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
 
 The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations (McCarthy et al. 2017), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
 
 
 ## Priors
 
 While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from the fits in Table 5 in Akino et al. (2022), and find the subset of simulations from our 400 models that agree to within $\pm 2$ or $3 \times \sigma$ of the inferred baryon budget at redshift $z=0.1$. We note that for our simulations, we include all stellar and gas particles within a spherical overdensity radius. Hence, in order to make reasonable comparisons with the fits in Akino et al. (2022), we included an additional 15\% contribution to the total stellar masses from the contribution of blue galaxies, and 30\% additional stellar mass to the brightest cluster galaxies (BCGs) to account for the diffuse intracluster light (ICL, see Akino et al. 2022).
```

### Comparing `pyspk-1.7/setup.py` & `pyspk-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     print(long_description)
 
 setuptools.setup(
     name="pyspk",
-    version=1.7,
+    version=1.8,
     description="Python package to predict the suppression of the total matter power spectrum due to baryonic physics",
     url="https://github.com/jemme07/pyspk",
     author="Jaime Salcido",
     author_email="j.salcidonegrete@ljmu.ac.uk",
     packages=['pyspk'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

