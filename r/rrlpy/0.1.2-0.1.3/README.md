# Comparing `tmp/rrlpy-0.1.2.tar.gz` & `tmp/rrlpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrlpy-0.1.2.tar", last modified: Fri Sep 15 18:45:26 2023, max compression
+gzip compressed data, was "rrlpy-0.1.3.tar", last modified: Thu May 16 17:58:00 2024, max compression
```

## Comparing `rrlpy-0.1.2.tar` & `rrlpy-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,49 @@
--rw-r--r--   0        0        0     1547 2023-08-21 18:43:13.089722 rrlpy-0.1.2/LICENSE
--rw-r--r--   0        0        0       45 2023-08-28 14:58:57.017855 rrlpy-0.1.2/README.md
--rw-r--r--   0        0        0     1352 2023-09-15 18:45:25.845100 rrlpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      225 2023-09-15 18:40:14.609674 rrlpy-0.1.2/src/rrlpy/__init__.py
--rw-r--r--   0        0        0      869 2023-08-21 18:43:13.128723 rrlpy-0.1.2/src/rrlpy/cli.py
--rw-r--r--   0        0        0        0 2023-08-22 14:09:06.734514 rrlpy-0.1.2/src/rrlpy/continuum/__init__.py
--rw-r--r--   0        0        0     1648 2023-08-22 15:02:58.436864 rrlpy-0.1.2/src/rrlpy/continuum/core.py
--rw-r--r--   0        0        0        0 2023-09-15 18:26:17.705579 rrlpy-0.1.2/src/rrlpy/freq/__init__.py
--rw-r--r--   0        0        0     2955 2023-09-15 18:38:53.050775 rrlpy-0.1.2/src/rrlpy/freq/core.py
--rw-r--r--   0        0        0      152 2023-09-15 18:29:18.010522 rrlpy-0.1.2/src/rrlpy/freq/data/CH.txt
--rw-r--r--   0        0        0      192 2023-09-15 18:29:18.014522 rrlpy-0.1.2/src/rrlpy/freq/data/OH.txt
--rw-r--r--   0        0        0   388015 2023-09-15 18:29:18.060523 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_3HeIalpha.txt
--rw-r--r--   0        0        0   323246 2023-09-15 18:29:18.305526 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIalpha.txt
--rw-r--r--   0        0        0   310338 2023-09-15 18:29:18.370526 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIbeta.txt
--rwxr-xr-x   0        0        0    60715 2023-09-15 18:29:18.388527 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIdelta.txt
--rw-r--r--   0        0        0   337673 2023-09-15 18:29:18.426527 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIepsilon.txt
--rw-r--r--   0        0        0   319304 2023-09-15 18:29:18.462527 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIgamma.txt
--rw-r--r--   0        0        0   351575 2023-09-15 18:29:18.473528 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIzeta.txt
--rwxr-xr-x   0        0        0    60827 2023-09-15 18:29:18.671530 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIalpha.txt
--rwxr-xr-x   0        0        0    58705 2023-09-15 18:29:18.732530 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIbeta.txt
--rw-r--r--   0        0        0    45264 2023-09-15 18:29:18.758530 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIdelta.txt
--rw-r--r--   0        0        0   422062 2023-09-15 18:29:18.806531 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIepsilon.txt
--rw-r--r--   0        0        0    45270 2023-09-15 18:29:18.830531 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIgamma.txt
--rw-r--r--   0        0        0   378189 2023-09-15 18:29:18.498528 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HeIalpha.txt
--rw-r--r--   0        0        0   365656 2023-09-15 18:29:18.564528 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HeIbeta.txt
--rw-r--r--   0        0        0   374026 2023-09-15 18:29:18.597529 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HeIgamma.txt
--rwxr-xr-x   0        0        0    60827 2023-09-15 18:29:18.842531 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_NIalpha.txt
--rwxr-xr-x   0        0        0    58700 2023-09-15 18:29:18.846531 rrlpy-0.1.2/src/rrlpy/freq/data/RRL_NIbeta.txt
--rw-r--r--   0        0        0        0 2023-08-22 14:21:44.943790 rrlpy-0.1.2/src/rrlpy/hrrl/__init__.py
--rw-r--r--   0        0        0      586 2023-08-22 14:42:01.694220 rrlpy-0.1.2/src/rrlpy/hrrl/core.py
--rw-r--r--   0        0        0        0 2023-08-21 21:02:47.667398 rrlpy-0.1.2/src/rrlpy/rrl/__init__.py
--rw-r--r--   0        0        0       95 2023-08-22 17:42:47.404487 rrlpy-0.1.2/src/rrlpy/rrl/constants.py
--rw-r--r--   0        0        0     2409 2023-08-22 14:58:41.625100 rrlpy-0.1.2/src/rrlpy/rrl/core.py
--rw-r--r--   0        0        0      444 2023-08-28 17:06:00.677732 rrlpy-0.1.2/src/rrlpy/rrl/tests/test_core.py
--rw-r--r--   0        0        0       19 2023-08-21 18:43:13.134723 rrlpy-0.1.2/src/rrlpy/rrlpy.py
--rw-r--r--   0        0        0        0 2023-08-22 14:58:58.174278 rrlpy-0.1.2/src/rrlpy/utils/__init__.py
--rw-r--r--   0        0        0     1881 2023-08-22 15:07:16.623644 rrlpy-0.1.2/src/rrlpy/utils/core.py
--rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 rrlpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1547 2023-08-21 18:43:13.089722 rrlpy-0.1.3/LICENSE
+-rw-r--r--   0        0        0       45 2023-08-28 14:58:57.017855 rrlpy-0.1.3/README.md
+-rw-r--r--   0        0        0     1611 2024-05-16 17:58:00.238128 rrlpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      220 2024-05-16 17:57:03.819472 rrlpy-0.1.3/src/rrlpy/__init__.py
+-rw-r--r--   0        0        0      869 2023-08-21 18:43:13.128723 rrlpy-0.1.3/src/rrlpy/cli.py
+-rw-r--r--   0        0        0      108 2024-04-05 01:25:11.317755 rrlpy-0.1.3/src/rrlpy/continuum/__init__.py
+-rw-r--r--   0        0        0      693 2024-03-26 04:39:43.471649 rrlpy-0.1.3/src/rrlpy/continuum/continuum.py
+-rw-r--r--   0        0        0     1648 2023-08-22 15:02:58.436864 rrlpy-0.1.3/src/rrlpy/continuum/core.py
+-rw-r--r--   0        0        0       65 2024-04-05 01:02:28.631234 rrlpy-0.1.3/src/rrlpy/departure/__init__.py
+-rw-r--r--   0        0        0     3888 2024-04-11 04:12:49.263257 rrlpy-0.1.3/src/rrlpy/departure/bnbeta.py
+-rw-r--r--   0        0        0     1099 2024-04-05 00:57:12.183630 rrlpy-0.1.3/src/rrlpy/departure/tests/test_bnbeta.py
+-rw-r--r--   0        0        0       59 2024-03-26 04:15:20.649245 rrlpy-0.1.3/src/rrlpy/freq/__init__.py
+-rw-r--r--   0        0        0     4353 2024-04-05 01:28:38.377110 rrlpy-0.1.3/src/rrlpy/freq/core.py
+-rw-r--r--   0        0        0      152 2023-09-15 18:29:18.010522 rrlpy-0.1.3/src/rrlpy/freq/data/CH.txt
+-rw-r--r--   0        0        0      192 2023-09-15 18:29:18.014522 rrlpy-0.1.3/src/rrlpy/freq/data/OH.txt
+-rw-r--r--   0        0        0   388015 2023-09-15 18:29:18.060523 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_3HeIalpha.txt
+-rw-r--r--   0        0        0   323246 2023-09-15 18:29:18.305526 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIalpha.txt
+-rw-r--r--   0        0        0   310338 2023-09-15 18:29:18.370526 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIbeta.txt
+-rwxr-xr-x   0        0        0    60715 2023-09-15 18:29:18.388527 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIdelta.txt
+-rw-r--r--   0        0        0   337673 2023-09-15 18:29:18.426527 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIepsilon.txt
+-rw-r--r--   0        0        0   319304 2023-09-15 18:29:18.462527 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIgamma.txt
+-rw-r--r--   0        0        0   351575 2023-09-15 18:29:18.473528 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIzeta.txt
+-rwxr-xr-x   0        0        0    60827 2023-09-15 18:29:18.671530 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIalpha.txt
+-rwxr-xr-x   0        0        0    58705 2023-09-15 18:29:18.732530 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIbeta.txt
+-rw-r--r--   0        0        0    45264 2023-09-15 18:29:18.758530 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIdelta.txt
+-rw-r--r--   0        0        0   422062 2023-09-15 18:29:18.806531 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIepsilon.txt
+-rw-r--r--   0        0        0    45270 2023-09-15 18:29:18.830531 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIgamma.txt
+-rw-r--r--   0        0        0   378189 2023-09-15 18:29:18.498528 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HeIalpha.txt
+-rw-r--r--   0        0        0   365656 2023-09-15 18:29:18.564528 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HeIbeta.txt
+-rw-r--r--   0        0        0   374026 2023-09-15 18:29:18.597529 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HeIgamma.txt
+-rwxr-xr-x   0        0        0    60827 2023-09-15 18:29:18.842531 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_NIalpha.txt
+-rwxr-xr-x   0        0        0    58700 2023-09-15 18:29:18.846531 rrlpy-0.1.3/src/rrlpy/freq/data/RRL_NIbeta.txt
+-rw-r--r--   0        0        0        0 2023-08-22 14:21:44.943790 rrlpy-0.1.3/src/rrlpy/hrrl/__init__.py
+-rw-r--r--   0        0        0      586 2023-08-22 14:42:01.694220 rrlpy-0.1.3/src/rrlpy/hrrl/core.py
+-rw-r--r--   0        0        0       91 2024-03-19 15:55:47.818348 rrlpy-0.1.3/src/rrlpy/linewidth/__init__.py
+-rw-r--r--   0        0        0     7386 2024-05-01 20:01:45.694685 rrlpy-0.1.3/src/rrlpy/linewidth/core.py
+-rw-r--r--   0        0        0       90 2024-03-26 04:16:41.046149 rrlpy-0.1.3/src/rrlpy/rrl/__init__.py
+-rw-r--r--   0        0        0      207 2024-03-26 04:17:24.892642 rrlpy-0.1.3/src/rrlpy/rrl/constants.py
+-rw-r--r--   0        0        0     4004 2024-04-10 13:22:14.231420 rrlpy-0.1.3/src/rrlpy/rrl/core.py
+-rw-r--r--   0        0        0     1035 2024-04-05 02:06:02.957642 rrlpy-0.1.3/src/rrlpy/rrl/rrl.py
+-rw-r--r--   0        0        0      444 2023-08-28 17:06:00.677732 rrlpy-0.1.3/src/rrlpy/rrl/tests/test_core.py
+-rw-r--r--   0        0        0      523 2024-03-27 14:13:57.143060 rrlpy-0.1.3/src/rrlpy/rrl/tests/test_rrl.py
+-rw-r--r--   0        0        0       19 2023-08-21 18:43:13.134723 rrlpy-0.1.3/src/rrlpy/rrlpy.py
+-rw-r--r--   0        0        0        0 2024-03-21 01:23:02.560638 rrlpy-0.1.3/src/rrlpy/synth/__init__.py
+-rw-r--r--   0        0        0     8591 2024-05-01 20:10:33.893881 rrlpy-0.1.3/src/rrlpy/synth/layers.py
+-rw-r--r--   0        0        0     1535 2024-04-11 04:13:56.736032 rrlpy-0.1.3/src/rrlpy/synth/tests/test_layers.py
+-rw-r--r--   0        0        0       59 2024-04-05 01:47:37.678072 rrlpy-0.1.3/src/rrlpy/utils/__init__.py
+-rw-r--r--   0        0        0     2293 2024-04-05 02:05:23.686196 rrlpy-0.1.3/src/rrlpy/utils/core.py
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 rrlpy-0.1.3/PKG-INFO
```

### Comparing `rrlpy-0.1.2/LICENSE` & `rrlpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/pyproject.toml` & `rrlpy-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,40 +8,68 @@
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
 dynamic = []
 requires-python = ">=3.5"
 dependencies = [
     "astropy",
+    "scipy",
+    "numpy",
 ]
 description = "Radio Recombination Lines in Python"
-version = "0.1.2"
+version = "0.1.3"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 homepage = "https://github.com/astrofle/RRLpy"
 repository = "https://github.com/astrofle/RRLpy"
 
 [tool.pdm.version]
 source = "file"
 path = "src/rrlpy/__init__.py"
 
 [tool.black]
 preview = true
-line-length = 100
+line-length = 120
 
 [tool.ruff]
-line-length = 100
+select = [
+    "F",
+    "E",
+    "W",
+    "B",
+    "I",
+    "RUF",
+]
+fixable = [
+    "ALL",
+]
+unfixable = [
+    "B",
+]
+ignore = [
+    "E741",
+    "B905",
+]
+line-length = 120
+src = [
+    "src",
+]
 
 [tool.ruff.per-file-ignores]
 "src/rrlpy/rrl/constants.py" = [
     "F401",
 ]
+"__init__.py" = [
+    "E402",
+    "F405",
+    "F403",
+]
 
 [tool.pyright]
 reportImplicitStringConcatenation = false
 
 [tool.isort]
 profile = "black"
 combine_as_imports = true
```

### Comparing `rrlpy-0.1.2/src/rrlpy/cli.py` & `rrlpy-0.1.3/src/rrlpy/cli.py`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/continuum/core.py` & `rrlpy-0.1.3/src/rrlpy/continuum/core.py`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_3HeIalpha.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_3HeIalpha.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIalpha.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIalpha.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIbeta.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIbeta.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIdelta.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIdelta.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIepsilon.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIepsilon.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIgamma.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIgamma.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_CIzeta.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_CIzeta.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIalpha.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIalpha.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIbeta.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIbeta.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIdelta.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIdelta.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIepsilon.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIepsilon.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HIgamma.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HIgamma.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HeIalpha.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HeIalpha.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HeIbeta.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HeIbeta.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_HeIgamma.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_HeIgamma.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_NIalpha.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_NIalpha.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/freq/data/RRL_NIbeta.txt` & `rrlpy-0.1.3/src/rrlpy/freq/data/RRL_NIbeta.txt`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/hrrl/core.py` & `rrlpy-0.1.3/src/rrlpy/hrrl/core.py`

 * *Files identical despite different names*

### Comparing `rrlpy-0.1.2/src/rrlpy/utils/core.py` & `rrlpy-0.1.3/src/rrlpy/utils/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,7 +78,29 @@
         The error on the area.
     """
 
     err1 = np.power(amplitude_err * sigma * np.sqrt(2 * np.pi), 2)
     err2 = np.power(sigma_err * amplitude * np.sqrt(2 * np.pi), 2)
 
     return np.sqrt(err1 + err2)
+
+
+def sigma2fwhm(sigma):
+    """
+    Converts the :math:`\\sigma` parameter of a Gaussian distribution to its FWHM.
+
+    .. math:
+
+       FWHM=2\\sqrt{2\\ln2}\\sigma
+
+    Parameters
+    ----------
+    sigma : float
+        Standard deviation of a Gaussian.
+
+    Returns
+    -------
+    fwhm : float
+        Full Width at Half Maximum of the Gaussian.
+    """
+
+    return sigma * 2.0 * np.sqrt(2.0 * np.log(2.0))
```

### Comparing `rrlpy-0.1.2/PKG-INFO` & `rrlpy-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrlpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Radio Recombination Lines in Python
 Home-page: https://github.com/astrofle/RRLpy
 Author-Email: Pedro Salas <psalas@nrao.edu>, astrofle <psalas@nrao.edu>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             Radio Recombination Lines in Python
@@ -37,12 +37,14 @@
         Public License instead of this License.  But first, please read
         <http://www.gnu.org/philosophy/why-not-lgpl.html>.
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/astrofle/RRLpy
 Project-URL: Repository, https://github.com/astrofle/RRLpy
 Requires-Python: >=3.5
 Requires-Dist: astropy
+Requires-Dist: scipy
+Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # RRLpy
 
 Radio Recombination Lines in Python
```

