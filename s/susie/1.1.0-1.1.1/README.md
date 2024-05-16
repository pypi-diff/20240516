# Comparing `tmp/susie-1.1.0.tar.gz` & `tmp/susie-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "susie-1.1.0.tar", last modified: Tue May 14 18:50:06 2024, max compression
+gzip compressed data, was "susie-1.1.1.tar", last modified: Thu May 16 19:57:09 2024, max compression
```

## Comparing `susie-1.1.0.tar` & `susie-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.212435 susie-1.1.0/
--rw-r--r--   0 maliabarker   (501) staff       (20)     1065 2023-09-18 19:40:07.000000 susie-1.1.0/LICENSE.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-05-14 18:50:06.212073 susie-1.1.0/PKG-INFO
--rw-r--r--   0 maliabarker   (501) staff       (20)    10299 2024-03-27 19:16:09.000000 susie-1.1.0/README.md
--rw-r--r--   0 maliabarker   (501) staff       (20)       84 2023-10-09 21:44:27.000000 susie-1.1.0/pyproject.toml
--rw-r--r--   0 maliabarker   (501) staff       (20)      949 2024-05-14 18:50:06.212913 susie-1.1.0/setup.cfg
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.203427 susie-1.1.0/src/
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.207176 susie-1.1.0/src/susie/
--rw-r--r--   0 maliabarker   (501) staff       (20)       36 2023-08-31 20:39:34.000000 susie-1.1.0/src/susie/__init__.py
--rw-r--r--   0 maliabarker   (501) staff       (20)    43305 2024-05-14 18:44:33.000000 susie-1.1.0/src/susie/ephemeris.py
--rw-r--r--   0 maliabarker   (501) staff       (20)    22474 2024-05-13 21:14:53.000000 susie-1.1.0/src/susie/timing_data.py
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.211629 susie-1.1.0/src/susie.egg-info/
--rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/PKG-INFO
--rw-r--r--   0 maliabarker   (501) staff       (20)      332 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/SOURCES.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)        1 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/dependency_links.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)       31 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/requires.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)        6 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/top_level.txt
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.210902 susie-1.1.0/tests/
--rw-r--r--   0 maliabarker   (501) staff       (20)    22468 2024-05-14 18:44:23.000000 susie-1.1.0/tests/test_ephemeris.py
--rw-r--r--   0 maliabarker   (501) staff       (20)    27292 2024-05-14 18:44:11.000000 susie-1.1.0/tests/test_transit_times.py
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-16 19:57:09.181234 susie-1.1.1/
+-rw-r--r--   0 maliabarker   (501) staff       (20)     1065 2023-09-18 19:40:07.000000 susie-1.1.1/LICENSE.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-05-16 19:57:09.181076 susie-1.1.1/PKG-INFO
+-rw-r--r--   0 maliabarker   (501) staff       (20)    10299 2024-03-27 19:16:09.000000 susie-1.1.1/README.md
+-rw-r--r--   0 maliabarker   (501) staff       (20)       84 2023-10-09 21:44:27.000000 susie-1.1.1/pyproject.toml
+-rw-r--r--   0 maliabarker   (501) staff       (20)      949 2024-05-16 19:57:09.181607 susie-1.1.1/setup.cfg
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-16 19:57:09.176538 susie-1.1.1/src/
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-16 19:57:09.178441 susie-1.1.1/src/susie/
+-rw-r--r--   0 maliabarker   (501) staff       (20)       36 2023-08-31 20:39:34.000000 susie-1.1.1/src/susie/__init__.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    43360 2024-05-16 19:11:10.000000 susie-1.1.1/src/susie/ephemeris.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    16899 2024-05-16 19:18:58.000000 susie-1.1.1/src/susie/timing_data.py
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-16 19:57:09.180763 susie-1.1.1/src/susie.egg-info/
+-rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-05-16 19:57:09.000000 susie-1.1.1/src/susie.egg-info/PKG-INFO
+-rw-r--r--   0 maliabarker   (501) staff       (20)      332 2024-05-16 19:57:09.000000 susie-1.1.1/src/susie.egg-info/SOURCES.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)        1 2024-05-16 19:57:09.000000 susie-1.1.1/src/susie.egg-info/dependency_links.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)       31 2024-05-16 19:57:09.000000 susie-1.1.1/src/susie.egg-info/requires.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)        6 2024-05-16 19:57:09.000000 susie-1.1.1/src/susie.egg-info/top_level.txt
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-16 19:57:09.180190 susie-1.1.1/tests/
+-rw-r--r--   0 maliabarker   (501) staff       (20)    23079 2024-05-16 19:06:16.000000 susie-1.1.1/tests/test_ephemeris.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    27364 2024-05-16 19:06:16.000000 susie-1.1.1/tests/test_transit_times.py
```

### Comparing `susie-1.1.0/LICENSE.txt` & `susie-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `susie-1.1.0/PKG-INFO` & `susie-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: susie
-Version: 1.1.0
+Version: 1.1.1
 Summary: Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
 Author: Malia Barker, Holly VanLooy, Adrienne Kirk
 Author-email: maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 Project-URL: Bug Tracker, https://github.com/BoiseStatePlanetary/susie/issues
 Project-URL: Repository, https://github.com/BoiseStatePlanetary/susie/
 Project-URL: Documentation, https://susie.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
```

### Comparing `susie-1.1.0/README.md` & `susie-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `susie-1.1.0/setup.cfg` & `susie-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = susie
-version = 1.1.0
+version = 1.1.1
 author = Malia Barker, Holly VanLooy, Adrienne Kirk
 author_email = maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 description = Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 project_urls = 
 	Bug Tracker = https://github.com/BoiseStatePlanetary/susie/issues
```

### Comparing `susie-1.1.0/src/susie/ephemeris.py` & `susie-1.1.1/src/susie/ephemeris.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 import numpy as np
 import matplotlib.pyplot as plt
 from lmfit import Model
-from susie.timing_data import TimingData # REMEMBER TO COMMENT THIS OUT BEFORE GIT PUSHES
-# from susie.transit_times import TransitTimes
+# from susie.timing_data import TimingData # REMEMBER TO ONLY USE THIS FOR PACKAGE UPDATES
+from timing_data import TimingData # REMEMBER TO COMMENT THIS OUT BEFORE GIT PUSHES
 
 class BaseModelEphemeris(ABC):
     """Abstract class that defines the structure of different model ephemeris classes."""
     @abstractmethod
     def fit_model(self, x, y, yerr, tra_or_occ, **kwargs):
         """Fits a model ephemeris to transit data.
 
@@ -396,15 +396,15 @@
         result = []
         for i, t_type in enumerate(self.timing_data.tra_or_occ):
             if t_type == 'tra':
                 # transit data
                 result.append(np.sqrt((T0_err**2) + ((self.timing_data.epochs[i]**2)*(P_err**2))))
             elif t_type == 'occ':
                 # occultation data
-                result.append(np.sqrt(((T0_err**2) + (0.5 * (P_err**2))) + ((self.timing_data.epochs[i]**2)*(P_err**2))))
+                result.append(np.sqrt((T0_err**2) + (((self.timing_data.epochs[i]+0.5)**2)*(P_err**2))))
         return np.array(result)
     
     def _calc_quadratic_model_uncertainties(self, T0_err, P_err, dPdE_err):
         """Calculates the uncertainties of a given quadratic model when compared to actual data in TransitTimes.
         
         TODO: Update docstring
         Uses the equation σ(t pred, tra) = √(σ(T0)^2 + (σ(P)^2 * E^2) + (1/4 * σ(dP/dE)^2 * E^4)) where 
@@ -429,15 +429,15 @@
         result = []
         for i, t_type in enumerate(self.timing_data.tra_or_occ):
             if t_type == 'tra':
                 # transit data
                 result.append(np.sqrt((T0_err**2) + ((self.timing_data.epochs[i]**2)*(P_err**2)) + ((1/4)*(self.timing_data.epochs[i]**4)*(dPdE_err**2))))
             elif t_type == 'occ':
                 # occultation data
-                result.append(np.sqrt(((T0_err**2) + (0.5 * (P_err**2))) + ((self.timing_data.epochs[i]**2)*(P_err**2)) + ((1/4)*(self.timing_data.epochs[i]**4)*(dPdE_err**2))))
+                result.append(np.sqrt((T0_err**2) + (((self.timing_data.epochs[i]+0.5)**2)*(P_err**2)) + ((1/4)*(self.timing_data.epochs[i]**4)*(dPdE_err**2))))
         return np.array(result)
     
     def _calc_linear_ephemeris(self, E, P, T0):
         """Calculates the mid transit times using parameters from a linear model ephemeris.
         
         TODO: Update docstring
         Uses the equation (T0 + PE) to calculate the mid transit times over each epoch where T0 is 
@@ -674,15 +674,15 @@
             save_filepath: Optional(str)
                 The path used to save the plot if `save_plot` is True.
         
         Returns
         ------- 
             A MatplotLib plot of epochs vs. model predicted mid-transit times.
         """
-        plt.scatter(x=self.timing_data.epochs, y=model_data_dict['model_data'])
+        plt.scatter(x=self.timing_data.epochs, y=model_data_dict['model_data'], color='#0033A0')
         plt.xlabel('Epochs')
         plt.ylabel('Model Predicted Mid-Times (units)')
         plt.title(f'Predicted {model_data_dict["model_type"].capitalize()} Model Mid Times over Epochs')
         if save_plot == True:
             plt.savefig(save_filepath)
         plt.show()
 
@@ -815,17 +815,17 @@
             else:
                 self.timing_data.epochs = all_epochs[:i+1]
                 self.timing_data.mid_times = all_mid_times[:i+1]
                 self.timing_data.mid_time_uncertainties = all_uncertainties[:i+1]
                 self.timing_data.tra_or_occ = all_tra_or_occ[:i+1]
                 delta_bic = self.calc_delta_bic()
                 delta_bics.append(delta_bic)
-        plt.scatter(x=self.timing_data.epochs, y=delta_bics)
+        plt.scatter(x=self.timing_data.epochs, y=delta_bics, color='#0033A0')
         plt.grid(True)
-        plt.plot(self.timing_data.epochs, delta_bics)
+        plt.plot(self.timing_data.epochs, delta_bics, color='#0033A0')
         plt.xlabel('Epoch')
         plt.ylabel('$\Delta$BIC')
         plt.title("Value of $\Delta$BIC as Observational Epochs Increase")
         if save_plot is True:
             plt.savefig(save_filepath)
         plt.show()
 
@@ -862,20 +862,20 @@
     quad_bic = ephemeris_obj1.calc_bic(quad_model_data)
     # print(quad_bic)
     # STEP 5.5: Get the delta BIC value for both models
     delta_bic = ephemeris_obj1.calc_delta_bic()
     # print(delta_bic)
 
     # STEP 6: Show a plot of the model ephemeris data
-    # ephemeris_obj1.plot_model_ephemeris(linear_model_data, save_plot=False)
+    ephemeris_obj1.plot_model_ephemeris(linear_model_data, save_plot=False)
     # ephemeris_obj1.plot_model_ephemeris(quad_model_data, save_plot=False)
 
     # STEP 7: Uncertainties plot
     # ephemeris_obj1.plot_timing_uncertainties(linear_model_data, save_plot=False)
     # ephemeris_obj1.plot_timing_uncertainties(quad_model_data, save_plot=False)
     
     # STEP 8: O-C Plot
     # ephemeris_obj1.plot_oc_plot(save_plot=False)
 
     # STEP 9: Running delta BIC plot
-    ephemeris_obj1.plot_running_delta_bic(save_plot=False)
+    # ephemeris_obj1.plot_running_delta_bic(save_plot=False)
```

### Comparing `susie-1.1.0/src/susie/timing_data.py` & `susie-1.1.1/src/susie/timing_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,20 +55,14 @@
             * values of transit or occultation array or not all 'tra' or 'occ'
 
     Side Effects
     -------------
         Variables epochs and mid_times are shifted to start at zero by subtracting the minimum number from each value
     """
     def __init__(self, time_format, epochs, mid_times, mid_time_uncertainties=None, tra_or_occ=None, time_scale=None, object_ra=None, object_dec=None, observatory_lon=None, observatory_lat=None):
-        # In ephemeris, we would probably check if we had both transits and occultations
-        # If so, we would need to account for that (maybe just in the fitting implementation? anywhere else?)
-        # If not, then we just assign our data to the transit times data and let it run!
-        # Although, need to look into this still. Might just have this implemented in model fits and plotting?
-        self.transits = None
-        self.occultations = None
         self.epochs = epochs
         self.mid_times = mid_times
         self.tra_or_occ = tra_or_occ
         if mid_time_uncertainties is None:
             # If no uncertainties provided, make an array of 1s in the same shape of epochs
             mid_time_uncertainties =  np.ones_like(self.epochs, dtype=float)
         self.mid_time_uncertainties = mid_time_uncertainties
@@ -256,89 +250,8 @@
             # TODO import warning that we are minimizing their epochs and transit times
         if self.mid_times[0] != 0:
             self.mid_times -= np.min(self.mid_times)
         if self.tra_or_occ is None:
             # Create list of just 'tra'
             self.tra_or_occ = np.array(['tra' for element in self.epochs])
         if self.tra_or_occ is not None:
-            self._validate_tra_or_occ()
-
-
-"""———————————————————— OLD CODE, MAY NOT BE NEEDED ————————————————————"""
-
-
-# class TransitTimes():
-#     """Represents the pre-processed transit mid point timing data over observations.
-    
-#     Parameters
-#     ------------
-#         epochs: numpy.ndarray[int]
-#             List of orbit number reference points for transit timing observations
-#         mid_times: numpy.ndarray[float]
-#             List of observed transit timing mid points corresponding with epochs
-#         mid_time_uncertainties: numpy.ndarray[float]
-#             List of uncertainties corresponding to transit mid-times
-#     """
-#     def __init__(self, epochs, mid_times, mid_time_uncertainties):
-#         self.epochs = epochs
-#         self.mid_times = mid_times
-#         self.mid_time_uncertainties = mid_time_uncertainties
-
-
-# class OccultationTimes():
-#     """Represents the pre-processed occultation mid point timing data over observations.
-    
-#     Parameters
-#     ------------
-#         epochs: numpy.ndarray[int]
-#             List of orbit number reference points for occultation timing observations
-#         mid_times: numpy.ndarray[float]
-#             List of observed occultation timing mid points corresponding with epochs
-#         mid_time_uncertainties: numpy.ndarray[float]
-#             List of uncertainties corresponding to occultation mid-times
-#     """
-#     def __init__(self, epochs, mid_times, mid_time_uncertainties):
-#         self.epochs = epochs
-#         self.mid_times = mid_times
-#         self.mid_time_uncertainties = mid_time_uncertainties
-
-# def _validate_tra_or_occ_data(self,t_epochs,t_mid_times,t_mid_time_uncertainties,o_epochs, o_mid_times, o_mid_time_uncertainties):
-    #     # Check that all are of type array
-    #     if not isinstance(t_mid_times, np.ndarray):
-    #         raise TypeError("The variable 't_mid_times' expected a NumPy array (np.ndarray) but received a different data type")
-    #     if not isinstance(t_mid_time_uncertainties, np.ndarray):
-    #         raise TypeError("The variable 't_mid_time_uncertainties' expected a NumPy array (np.ndarray) but received a different data type")
-    #     if not isinstance(o_epochs, np.ndarray):
-    #         raise TypeError("The variable 'o_epochs' expected a NumPy array (np.ndarray) but received a different data type")
-    #     if not isinstance(o_mid_times, np.ndarray):
-    #         raise TypeError("The variable 'o_mid_times' expected a NumPy array (np.ndarray) but received a different data type")
-    #     if not isinstance(o_mid_time_uncertainties, np.ndarray):
-    #         raise TypeError("The variable 'o_mid_time_uncertainties' expected a NumPy array (np.ndarray) but received a different data type")
-    #     # Check that all are same shape
-    #     if t_epochs.shape != t_mid_times.shape != t_mid_time_uncertainties.shape:
-    #         raise ValueError("Shapes of 't_epochs', 't_mid_times', and 't_mid_time_uncertainties' arrays do not match.")
-    #     if o_epochs.shape != o_mid_times.shape != o_mid_time_uncertainties.shape:
-    #         raise ValueError("Shapes of 'o_epochs', 'o_mid_times', and 'o_mid_time_uncertainties' arrays do not match.")
-
-# # Once everything is validated and corrected, we can separate into transits and occultations if we are given the tra_or_occ data
-        # if self.tra_or_occ is None:
-        #     # All data are transit data
-        #     self.transits = TransitTimes(self.epochs, self.mid_times, self.mid_time_uncertainties)
-        # else:
-        #     self._validate_tra_or_occ(tra_or_occ)
-        #     tra_or_occ = np.char.strip(tra_or_occ) # Strip any whitespace
-        #     # Separate epochs, mid times, and uncertainties into their respective lists
-        #     # t_epochs = []
-        #     # for i in range(len(tra_or_occ)):
-        #     #     if tra_or_occ[i] == 'tra':
-        #     #         t_epochs.append(self.epochs[i])
-
-        #     t_epochs = np.array([self.epochs[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'tra'])
-        #     t_mid_times = np.array([self.mid_times[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'tra'])
-        #     t_mid_time_uncertainties = np.array([self.mid_time_uncertainties[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'tra'])
-        #     o_epochs = np.array([self.epochs[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'occ'])
-        #     o_mid_times = np.array([self.mid_times[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'occ'])
-        #     o_mid_time_uncertainties = np.array([self.mid_time_uncertainties[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'occ'])
-        #     self._validate_tra_or_occ_data(self,t_epochs,t_mid_times,t_mid_time_uncertainties,o_epochs, o_mid_times, o_mid_time_uncertainties)
-        #     # Create transit and occultation objects
-        #     self.transits = TransitTimes(t_epochs, t_mid_times, t_mid_time_uncertainties)
-        #     self.occultations = OccultationTimes(o_epochs, o_mid_times, o_mid_time_uncertainties)
+            self._validate_tra_or_occ()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `susie-1.1.0/src/susie.egg-info/PKG-INFO` & `susie-1.1.1/src/susie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: susie
-Version: 1.1.0
+Version: 1.1.1
 Summary: Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
 Author: Malia Barker, Holly VanLooy, Adrienne Kirk
 Author-email: maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 Project-URL: Bug Tracker, https://github.com/BoiseStatePlanetary/susie/issues
 Project-URL: Repository, https://github.com/BoiseStatePlanetary/susie/
 Project-URL: Documentation, https://susie.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
```

### Comparing `susie-1.1.0/tests/test_ephemeris.py` & `susie-1.1.1/tests/test_ephemeris.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,128 +1,127 @@
 import sys
 sys.path.append(".")
 import unittest
 import numpy as np
 import matplotlib.pyplot as plt
-
+from lmfit import Model
 from src.susie.timing_data import TimingData
 from src.susie.ephemeris import Ephemeris, LinearModelEphemeris, QuadraticModelEphemeris, ModelEphemerisFactory
 from scipy.optimize import curve_fit
 test_epochs = np.array([0, 294, 298, 573])
 test_mtts = np.array([0.0, 320.8780000000261, 325.24399999994785, 625.3850000002421])
 test_mtts_err = np.array([0.00043, 0.00028, 0.00062, 0.00042])
 test_tra_or_occ = np.array(['tra','occ','tra','occ'])
-test_P_linear = 1.0914223408652188 # period linear
-test_P_err_linear = 9.998517417992763e-07 # period error linear
-test_T0_linear =  -6.734666196939187e-05 # conjunction time
-test_T0_err_linear = 0.0003502975050463415 # conjunction time error
+test_P_linear = 1.09142234035412 # period linear
+test_P_err_linear = 0.0006807480614626216 # period error linear
+test_T0_linear =  -6.728390649943598e-05 # conjunction time
+test_T0_err_linear = 0.23692091722329203 # conjunction time error
 
 test_P_quad = 1.0914215464474404 #period quad
-test_P_err_quad = 9.150815726215122e-06 # period err quad
+test_P_err_quad =  0.0023688537695923505 # period err quad
 test_dPdE = 2.7744598987630543e-09#period change by epoch
-test_dPdE_err = 3.188345582283935e-08#period change by epoch error
+test_dPdE_err = 7.743357776955459e-06#period change by epoch error
 test_T0_quad = -1.415143555084551e-06 #conjunction time quad
-test_T0_err_quad = 0.00042940561938685084#conjunction time err quad
+test_T0_err_quad = 0.34674308676945004#conjunction time err quad
 
 test_observed_data = np.array([0.0, 320.8780000000261, 325.24399999994785, 625.3850000002421])
-test_uncertainties= np.array([0.00043, 0.00028, 0.00062, 0.00042])
-       
+test_uncertainties= np.array([0.00043, 0.00028, 0.00062, 0.00042])    
 
 
 class TestLinearModelEphemeris(unittest.TestCase):
     def linear_fit_instantiation(self):
         """ Tests that ephemeris is an instance of LinearModelEphemeris
         """
         self.ephemeris = LinearModelEphemeris()
         self.assertIsInstance(self.ephemeris, LinearModelEphemeris)
-    
+
     def test_linear_fit(self):
         """Tests that the lin_fit function works
 
-            Creates a numpy.ndarray[float] with the length of the test data
+            Creates a numpy.ndarray[int] with the length of the test data
         """
         linear_model = LinearModelEphemeris()
-        # recalculate
-        expected_result = np.array([-6.73466620e-05,  3.50213351e+02,  3.54978500e+02,  6.82559093e+02])
-        result = linear_model.lin_fit(test_mtts, test_P_linear, test_T0_linear, test_tra_or_occ)
+        test_tra_or_occ_enum = [0 if i == 'tra' else 1 for i in test_tra_or_occ]
+        T0 = 0
+        expected_result = np.array([0, 321, 325, 625])
+        result = linear_model.lin_fit(test_epochs, test_P_linear, T0, test_tra_or_occ_enum)
         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
 
     def test_lin_fit_model(self):
         """Testing that the dictionary parameters of fit model are equal to what they are suppose to be
 
             Tests the creation of a dictionary named return_data containing the linear fit model data in the order of:
             {'period': float,
             'period_err':float,
             'conjunction_time': float,
             'conjunction_time_err':float}    
         """
         linear_model = LinearModelEphemeris()
-        popt, pcov = curve_fit(linear_model.lin_fit, test_epochs, test_mtts, sigma=test_mtts_err, absolute_sigma=True)
-        unc = np.sqrt(np.diag(pcov))
+        result = linear_model.fit_model(test_epochs, test_mtts, test_mtts_err, test_tra_or_occ)
         return_data = {
-            'period': popt[0],
-            'period_err': unc[0],
-            'conjunction_time': popt[1],
-            'conjunction_time_err': unc[1]
-        }
-        self.assertEqual(popt[0], return_data['period'])
-        self.assertEqual(unc[0], return_data['period_err'])
-        self.assertEqual(popt[1], return_data['conjunction_time'])
-        self.assertEqual(unc[1], return_data['conjunction_time_err'])
+            'period': 1.0904734089104249,
+            'period_err': 0.0006807480614626216,
+            'conjunction_time': -0.1010330285087608 ,
+            'conjunction_time_err':  0.23692091722329203
+        }
+        self.assertEqual(result['period'], return_data['period'])
+        self.assertEqual(result['period_err'], return_data['period_err'])
+        self.assertEqual(result['conjunction_time'], return_data['conjunction_time'])
+        self.assertEqual(result['conjunction_time_err'], return_data['conjunction_time_err'])
 
 
 class TestQuadraticModelEphemeris(unittest.TestCase):
 
     def quad_fit_instantiation(self):
         """ Tests that ephemeris is an instance of QuadraticModelEphemeris
         """
         self.ephemeris = QuadraticModelEphemeris()
         self.assertIsInstance(self.ephemeris, QuadraticModelEphemeris)
 
     def test_quad_fit(self):
         """ Tests that the quad_fit function works
 
-            Creates a numpy.ndarray[float] with the length of the test data
+            Creates a numpy.ndarray[int] with the length of the test data
         """
         quadratic_model = QuadraticModelEphemeris()
-        expected_result = np.array([-1.41514356e-06,  3.50213304e+02,  3.54978455e+02,  6.82559205e+02])
-        result = quadratic_model.quad_fit(test_mtts,test_dPdE, test_P_quad, test_T0_quad)
+        test_tra_or_occ_enum = [0 if i == 'tra' else 1 for i in test_tra_or_occ]
+        expected_result = np.array([0,321,325,625])
+        result = quadratic_model.quad_fit(test_epochs, 0,test_P_quad, 0, test_tra_or_occ_enum)
+        print(result)
         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
 
     def test_quad_fit_model(self):
         """Testing that the dictionary parameters of fit model are equal to what they are suppose to be
 
             Tests the creation of a dictionary named return_data containing the quadratic fit model data in the order of:
             {  'conjunction_time': float,
             'conjunction_time_err': float,
             'period': float,
             'period_err': float,
             'period_change_by_epoch': float,
             'period_change_by_epoch_err': float,
         """
         quad_model = QuadraticModelEphemeris()
-        popt, pcov = curve_fit(quad_model.quad_fit, test_epochs, test_mtts, sigma=test_mtts_err, absolute_sigma=True)
-        unc = np.sqrt(np.diag(pcov))
+        result = quad_model.fit_model(test_epochs, test_mtts,test_mtts_err,test_tra_or_occ)
         return_data = {
-            'conjunction_time': popt[2],
-            'conjunction_time_err': unc[2],
-            'period': popt[1],
-            'period_err': unc[1],
-            'period_change_by_epoch': popt[0],
-            'period_change_by_epoch_err': unc[0],
-        }
-        self.assertEqual(popt[1], return_data['period'])
-        self.assertEqual(unc[1], return_data['period_err'])
-        self.assertEqual(popt[2], return_data['conjunction_time'])
-        self.assertEqual(unc[2], return_data['conjunction_time_err'])
-        self.assertEqual(popt[0], return_data['period_change_by_epoch'])
-        self.assertEqual(unc[0], return_data['period_change_by_epoch_err'])
+            'period': 1.0892661840315387,
+            'period_err': 0.0023688537695923505,
+            'conjunction_time': -0.000865530018010096 ,
+            'conjunction_time_err':  0.34674308676945004,
+            'period_change_by_epoch':4.224191878694417e-06,
+            'period_change_by_epoch_err': 7.743357776955459e-06
+        }
+        self.assertEqual(result['period'], return_data['period'])
+        self.assertEqual(result['period_err'], return_data['period_err'])
+        self.assertEqual(result['conjunction_time'], return_data['conjunction_time'])
+        self.assertEqual(result['conjunction_time_err'], return_data['conjunction_time_err'])
+        self.assertEqual(result['period_change_by_epoch'], return_data['period_change_by_epoch'])
+        self.assertEqual(result['period_change_by_epoch_err'], return_data['period_change_by_epoch_err'])
 
-# Do I need to create a test for this class????
-# class TestModelEphemerisFactory(unittest.TestCase):
+class TestModelEphemerisFactory(unittest.TestCase):
     def model_no_errors(self):
         models = {
             'linear': LinearModelEphemeris(),
             'quadratic': QuadraticModelEphemeris()
         }
         test_model_type = 'linear'
         self.assertTrue(test_model_type in models)
@@ -156,65 +155,64 @@
                 # print(d1[key], d2[key])
                 self.assertTrue(np.allclose(d1[key], d2[key], rtol=1e-05, atol=1e-08))
             else:
                 self.assertAlmostEqual(d1[key], d2[key], places=places, msg=msg)
                 
 
     def setUp(self):
-       """ Sets up the intantiation of TransitTimes object and Ephemeris object
+       """ Sets up the intantiation of TimingData object and Ephemeris object
 
            Runs before every test in the TestEphemeris class
        """
-       self.transit = TimingData('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
-       self.assertIsInstance(self.transit, TimingData)
-       self.ephemeris = Ephemeris(self.transit)
-      
+       self.timing_data = TimingData('jd', test_epochs, test_mtts, test_mtts_err,test_tra_or_occ, time_scale='tdb')
+       self.assertIsInstance(self.timing_data, TimingData)
+       self.ephemeris = Ephemeris(self.timing_data)    
 
     def test_us_transit_times_instantiation(self):
-        """ Unsuccessful instantiation of the transit times object within the Ephemeris class
+        """ Unsuccessful instantiation of the timing data object within the Ephemeris class
 
-            Need a TransitTimes object to run Ephemeris
+            Need a TimingData object to run Ephemeris
         """
-        with self.assertRaises(ValueError, msg = "Variable 'transit_times' expected type of object 'TransitTimes'."):
+        with self.assertRaises(ValueError, msg = "Variable 'timing_data' expected type of object 'TimingData'."):
             self.ephemeris = Ephemeris(None)
 
+
+
     
     def test_get_model_parameters_linear(self):
         """ Tests the creation of the linear model parameters
 
             With the input of a linear model type, the linear model parameters dictionary is created
             The dictionary is the same one from fit_model in the LinearModelEphemeris
         """
         test_model_type= 'linear'
         model_parameters = self.ephemeris._get_model_parameters(test_model_type)
-        expected_result = {
-            'period': 1.0914223408652188,  
-            'period_err': 9.998517417992763e-07,
-            'conjunction_time': -6.734666196939187e-05, 
-            'conjunction_time_err': 0.0003502975050463415
+        expected_result = {'period': 1.0904734089104249,
+            'period_err': 0.0006807480614626216,
+            'conjunction_time': -0.1010330285087608 ,
+            'conjunction_time_err':  0.23692091722329203  
         }
         self.assertDictEqual(model_parameters,expected_result)   
 
     def test_get_model_parameters_quad(self):
         """ Tests the creation of the quadratic model parameters
 
             With the input of a quadratic model type, the quadratic model parameters dictionary is created
             The dictionary is the same one from fit_model in the QuadraticModelEphemeris
         """
         test_model_type = 'quadratic'
         model_parameters = self.ephemeris._get_model_parameters(test_model_type)   
-        expected_result = {
-            'conjunction_time': -1.415143555084551e-06,
-            'conjunction_time_err': 0.00042940561938685084,
-            'period': 1.0914215464474404,
-            'period_err': 9.150815726215122e-06,
-            'period_change_by_epoch': 2.7744598987630543e-09,
-            'period_change_by_epoch_err': 3.188345582283935e-08,
+        expected_result = {'period': 1.0892661840315387, 
+            'period_err': 0.0023688537695923505,
+            'conjunction_time': -0.000865530018010096, 
+            'conjunction_time_err': 0.34674308676945004, 
+            'period_change_by_epoch': 4.224191878694417e-06, 
+            'period_change_by_epoch_err': 7.743357776955459e-06
         }
-        self.assertDictEqual(model_parameters,expected_result)
+        self.assertDictEqual(model_parameters, expected_result)
 
 
     def test_k_value_linear(self):
         """ Tests the correct k value is returned given the linear model type
 
             The k value for a linear model is 2
         """
@@ -235,255 +233,255 @@
 
     
     def test_calc_linear_model_uncertainties(self):
         """ Tests that the correct array of linear uncertainties are produced
 
             Produces a numpy array with the length of the epochs
         """
-        expected_result = np.array([0.0003503 , 0.00045729, 0.00045988, 0.00067152])
+        expected_result = np.array([0.23692092, 0.31014149, 0.31190525, 0.45638284 ])
         result = self.ephemeris._calc_linear_model_uncertainties(test_T0_err_linear, test_P_err_linear)
         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
 
     def test_calc_quad_model_uncertainties(self):
         """ Tests that the correct array of quadratic uncertainties are produced
 
             Produces a numpy array with the length of the epochs
         """
-        expected_result = np.array([0.00042941, 0.00305304, 0.00310238, 0.00742118])
+        expected_result = np.array([ 0.34674309, 0.84691127, 0.85834968, 1.89170591 ])
         result = self.ephemeris._calc_quadratic_model_uncertainties(test_T0_err_quad, test_P_err_quad,test_dPdE_err)
         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
 
-    def test_calc_linear_ephemeris(self):
-        """ Tests that the correct linear model data is produced
-
-            The model data is a numpy array of calcuated mid transit times
-        """
-        expected_result = np.array([-6.73466620e-05, 3.20878101e+02, 3.25243790e+02, 6.25384934e+02])#test model data linear
-        result = self.ephemeris._calc_linear_ephemeris(test_epochs, test_P_linear, test_T0_linear)
-        self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
-
-
-    def test_calc_quadratic_ephemeris(self):
-        """ Tests that the correct quadratic model data is produced
-
-            The model data is a numpy array of calcuated mid transit times
-        """
-        expected_result = np.array([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])#test model data quad
-        result = self.ephemeris._calc_quadratic_ephemeris(test_epochs,test_P_quad,test_T0_quad,test_dPdE)
-        self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
+#     def test_calc_linear_ephemeris(self):
+#         """ Tests that the correct linear model data is produced
 
-
-    def test_calc_chi_squared_linear(self):
-        """ Tests the calculated chi squared value
-
-            The linear chi squared value is a float that is calculated with the model data produced by test_calc_linear_ephemeris 
-        """
-        test_linear_model_data = np.array([-6.73466620e-05, 3.20878101e+02, 3.25243790e+02, 6.25384934e+02])
-        expected_result = 0.29406284565290114
-        result = self.ephemeris._calc_chi_squared(test_linear_model_data)
-        self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))   
-
-
-    def test_calc_chi_squared_quad(self):
-        """ Tests the calculated chi squared value
-
-            The quadratic chi squared value is a float that is calculated with the model data produced by test_calc_quadratic_ephemeris 
-        """
-        test_quad_model_data = np.array([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
-        expected_result = 0.20766342879185204
-        result = self.ephemeris._calc_chi_squared(test_quad_model_data)
-        self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))   
+#             The model data is a numpy array of calcuated mid transit times
+#         """
+#         expected_result = np.array([-6.73466620e-05, 3.20878101e+02, 3.25243790e+02, 6.25384934e+02])#test model data linear
+#         result = self.ephemeris._calc_linear_ephemeris(test_epochs, test_P_linear, test_T0_linear)
+#         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
+
+
+#     def test_calc_quadratic_ephemeris(self):
+#         """ Tests that the correct quadratic model data is produced
+
+#             The model data is a numpy array of calcuated mid transit times
+#         """
+#         expected_result = np.array([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])#test model data quad
+#         result = self.ephemeris._calc_quadratic_ephemeris(test_epochs,test_P_quad,test_T0_quad,test_dPdE)
+#         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
+
+
+#     def test_calc_chi_squared_linear(self):
+#         """ Tests the calculated chi squared value
+
+#             The linear chi squared value is a float that is calculated with the model data produced by test_calc_linear_ephemeris 
+#         """
+#         test_linear_model_data = np.array([-6.73466620e-05, 3.20878101e+02, 3.25243790e+02, 6.25384934e+02])
+#         expected_result = 0.29406284565290114
+#         result = self.ephemeris._calc_chi_squared(test_linear_model_data)
+#         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))   
+
+
+#     def test_calc_chi_squared_quad(self):
+#         """ Tests the calculated chi squared value
+
+#             The quadratic chi squared value is a float that is calculated with the model data produced by test_calc_quadratic_ephemeris 
+#         """
+#         test_quad_model_data = np.array([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
+#         expected_result = 0.20766342879185204
+#         result = self.ephemeris._calc_chi_squared(test_quad_model_data)
+#         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))   
     
-    def test_get_model_ephemeris_linear(self):
-        """ Tests that the linear model type produces the linear model parameters with the linear model type and linear model data included
-
-            Uses the test_get_model_parameters_linear and test_calc_linear_ephemeris to produce a dictionary with:
-            {
-            'period': float,  
-            'period_err': float,
-            'conjunction_time': float,
-            'conjunction_time_err':  float,
-            'model_type': 'linear', 
-            'model_data': np.array
-        }
-        """
-        test_model_type = 'linear'
-        model_parameters_linear = {
-            'period': 1.0914223408652188,  
-            'period_err': 9.998517417992763e-07,
-            'conjunction_time': -6.734666196939187e-05, 
-            'conjunction_time_err':  0.0003502975050463415,
-            'model_type': 'linear', 
-            'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
-        }
-        result = self.ephemeris.get_model_ephemeris(test_model_type)
-        self.assertDictAlmostEqual(result, model_parameters_linear)
+#     def test_get_model_ephemeris_linear(self):
+#         """ Tests that the linear model type produces the linear model parameters with the linear model type and linear model data included
 
-    def test_get_model_ephemeris_quad(self):
-        """ Tests that the quadratic model type produces the quadratic model parameters with the quadratic model type and quadratic model data included
-
-            Uses the test_get_model_parameters_linear and test_calc_linear_ephemeris to produce a dictionary with:
-            {
-            'period': float,  
-            'period_err': float,
-            'conjunction_time': float,
-            'conjunction_time_err':  float,
-            'period_change_by_epoch': float,
-            'period_change_by_epoch_err': float,
-            'model_type': 'quadratic', 
-            'model_data': np.array
-        }
-        """
-        test_model_type = 'quadratic'
-        model_parameters_quad = {
-            'conjunction_time': -1.415143555084551e-06,
-            'conjunction_time_err': 0.00042940561938685084,
-            'period': 1.0914215464474404,
-            'period_err': 9.150815726215122e-06,
-            'period_change_by_epoch': 2.7744598987630543e-09,
-            'period_change_by_epoch_err': 3.188345582283935e-08,
-            'model_type': 'quadratic',
-            'model_data': ([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
-        }
-        result = self.ephemeris.get_model_ephemeris(test_model_type)
-        self.assertDictAlmostEqual(result, model_parameters_quad)
-
-    def test_get_ephemeris_uncertainites_model_type_err(self):
-        """ Unsuccessful test to calculate uncertainties
-
-            Model type is needed
-        """
-        model_parameters_linear = {
-            'period': 1.0914223408652188,  
-            'period_err': 9.998517417992763e-07,
-            'conjunction_time': -6.734666196939187e-05, 
-            'conjunction_time_err':  0.0003502975050463415,
-            'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
-        }
-        with self.assertRaises(KeyError, msg = "Cannot find model type in model data. Please run the get_model_ephemeris method to return ephemeris fit parameters."):
-            self.ephemeris.get_ephemeris_uncertainties(model_parameters_linear)
+#             Uses the test_get_model_parameters_linear and test_calc_linear_ephemeris to produce a dictionary with:
+#             {
+#             'period': float,  
+#             'period_err': float,
+#             'conjunction_time': float,
+#             'conjunction_time_err':  float,
+#             'model_type': 'linear', 
+#             'model_data': np.array
+#         }
+#         """
+#         test_model_type = 'linear'
+#         model_parameters_linear = {
+#             'period': 1.0914223408652188,  
+#             'period_err': 9.998517417992763e-07,
+#             'conjunction_time': -6.734666196939187e-05, 
+#             'conjunction_time_err':  0.0003502975050463415,
+#             'model_type': 'linear', 
+#             'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
+#         }
+#         result = self.ephemeris.get_model_ephemeris(test_model_type)
+#         self.assertDictAlmostEqual(result, model_parameters_linear)
+
+#     def test_get_model_ephemeris_quad(self):
+#         """ Tests that the quadratic model type produces the quadratic model parameters with the quadratic model type and quadratic model data included
+
+#             Uses the test_get_model_parameters_linear and test_calc_linear_ephemeris to produce a dictionary with:
+#             {
+#             'period': float,  
+#             'period_err': float,
+#             'conjunction_time': float,
+#             'conjunction_time_err':  float,
+#             'period_change_by_epoch': float,
+#             'period_change_by_epoch_err': float,
+#             'model_type': 'quadratic', 
+#             'model_data': np.array
+#         }
+#         """
+#         test_model_type = 'quadratic'
+#         model_parameters_quad = {
+#             'conjunction_time': -1.415143555084551e-06,
+#             'conjunction_time_err': 0.00042940561938685084,
+#             'period': 1.0914215464474404,
+#             'period_err': 9.150815726215122e-06,
+#             'period_change_by_epoch': 2.7744598987630543e-09,
+#             'period_change_by_epoch_err': 3.188345582283935e-08,
+#             'model_type': 'quadratic',
+#             'model_data': ([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
+#         }
+#         result = self.ephemeris.get_model_ephemeris(test_model_type)
+#         self.assertDictAlmostEqual(result, model_parameters_quad)
+
+#     def test_get_ephemeris_uncertainites_model_type_err(self):
+#         """ Unsuccessful test to calculate uncertainties
+
+#             Model type is needed
+#         """
+#         model_parameters_linear = {
+#             'period': 1.0914223408652188,  
+#             'period_err': 9.998517417992763e-07,
+#             'conjunction_time': -6.734666196939187e-05, 
+#             'conjunction_time_err':  0.0003502975050463415,
+#             'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
+#         }
+#         with self.assertRaises(KeyError, msg = "Cannot find model type in model data. Please run the get_model_ephemeris method to return ephemeris fit parameters."):
+#             self.ephemeris.get_ephemeris_uncertainties(model_parameters_linear)
     
-    def test_get_ephemeris_uncertainties_lin_err(self):
-        """ Unsuccessful test to calculate uncertainties
+#     def test_get_ephemeris_uncertainties_lin_err(self):
+#         """ Unsuccessful test to calculate uncertainties
 
-            Period error and conjunction time error values are needed
-        """
-        model_parameters_linear = {
-            'period': 1.0914223408652188,  
-            'conjunction_time': -6.734666196939187e-05, 
-            'model_type': 'linear', 
-            'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
-        }
-        with self.assertRaises(KeyError, msg = "Cannot find conjunction time and period errors in model data. Please run the get_model_ephemeris method with 'linear' model_type to return ephemeris fit parameters."):
-            self.ephemeris.get_ephemeris_uncertainties(model_parameters_linear)
-
-
-    def test_get_ephemeris_uncertainties_quad_err(self):
-        """ Unsuccessful test to calculate uncertainties
-
-            Conjunction time error, period error and period change by epoch error is needed
-        """
-        model_parameters_quad = {
-            'conjunction_time': -1.415143555084551e-06,
-            'period': 1.0914215464474404,
-            'period_change_by_epoch': 2.7744598987630543e-09,
-            'model_type': 'quadratic',
-            'model_data': ([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
-        }
-        with self.assertRaises(KeyError, msg = "Cannot find conjunction time, period, and/or period change by epoch errors in model data. Please run the get_model_ephemeris method with 'quadratic' model_type to return ephemeris fit parameters."):
-            self.ephemeris.get_ephemeris_uncertainties(model_parameters_quad)
+#             Period error and conjunction time error values are needed
+#         """
+#         model_parameters_linear = {
+#             'period': 1.0914223408652188,  
+#             'conjunction_time': -6.734666196939187e-05, 
+#             'model_type': 'linear', 
+#             'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
+#         }
+#         with self.assertRaises(KeyError, msg = "Cannot find conjunction time and period errors in model data. Please run the get_model_ephemeris method with 'linear' model_type to return ephemeris fit parameters."):
+#             self.ephemeris.get_ephemeris_uncertainties(model_parameters_linear)
+
+
+#     def test_get_ephemeris_uncertainties_quad_err(self):
+#         """ Unsuccessful test to calculate uncertainties
+
+#             Conjunction time error, period error and period change by epoch error is needed
+#         """
+#         model_parameters_quad = {
+#             'conjunction_time': -1.415143555084551e-06,
+#             'period': 1.0914215464474404,
+#             'period_change_by_epoch': 2.7744598987630543e-09,
+#             'model_type': 'quadratic',
+#             'model_data': ([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
+#         }
+#         with self.assertRaises(KeyError, msg = "Cannot find conjunction time, period, and/or period change by epoch errors in model data. Please run the get_model_ephemeris method with 'quadratic' model_type to return ephemeris fit parameters."):
+#             self.ephemeris.get_ephemeris_uncertainties(model_parameters_quad)
 
     
    
-    def test_get_ephemeris_uncertainites_linear(self):
-        """ Sucessful test to calculate linear uncertainties
+#     def test_get_ephemeris_uncertainites_linear(self):
+#         """ Sucessful test to calculate linear uncertainties
 
-            Expected result is the numpy array produced by test_calc_linear_model_uncertaintie
-        """
-        model_parameters_linear = {
-            'period': 1.0914223408652188,  
-            'period_err': 9.998517417992763e-07,
-            'conjunction_time': -6.734666196939187e-05, 
-            'conjunction_time_err': 0.0003502975050463415,
-            'model_type': 'linear', 
-            'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
-        }
-        expected_result = np.array([0.0003503 , 0.00045729, 0.00045988, 0.00067152])
-        self.ephemeris.get_ephemeris_uncertainties(model_parameters_linear)
-        results = self.ephemeris.get_ephemeris_uncertainties(model_parameters_linear)
-        self.assertTrue(np.allclose(expected_result, results, rtol=1e-05, atol=1e-08)) 
+#             Expected result is the numpy array produced by test_calc_linear_model_uncertaintie
+#         """
+#         model_parameters_linear = {
+#             'period': 1.0914223408652188,  
+#             'period_err': 9.998517417992763e-07,
+#             'conjunction_time': -6.734666196939187e-05, 
+#             'conjunction_time_err': 0.0003502975050463415,
+#             'model_type': 'linear', 
+#             'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
+#         }
+#         expected_result = np.array([0.0003503 , 0.00045729, 0.00045988, 0.00067152])
+#         self.ephemeris.get_ephemeris_uncertainties(model_parameters_linear)
+#         results = self.ephemeris.get_ephemeris_uncertainties(model_parameters_linear)
+#         self.assertTrue(np.allclose(expected_result, results, rtol=1e-05, atol=1e-08)) 
          
-    def test_get_ephemeris_uncertainites_quad(self):
-        """ Sucessful test to calculate quadratic uncertainties
+#     def test_get_ephemeris_uncertainites_quad(self):
+#         """ Sucessful test to calculate quadratic uncertainties
 
-            Expected result is the numpy array produced by test_calc_quadratic_model_uncertaintie
-        """
-        model_parameters_quad = {
-            'conjunction_time': -1.415143555084551e-06,
-            'conjunction_time_err': 0.00042940561938685084,
-            'period': 1.0914215464474404,
-            'period_err': 9.150815726215122e-06,
-            'period_change_by_epoch': 2.7744598987630543e-09,
-            'period_change_by_epoch_err': 3.188345582283935e-08,
-            'model_type': 'quadratic',
-            'model_data': ([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
-        }
-        expected_result = np.array([0.00042941, 0.00305304, 0.00310238, 0.00742118])
-        self.ephemeris.get_ephemeris_uncertainties(model_parameters_quad)
-        results = self.ephemeris.get_ephemeris_uncertainties(model_parameters_quad)
-        self.assertTrue(np.allclose(expected_result, results, rtol=1e-05, atol=1e-08)) 
+#             Expected result is the numpy array produced by test_calc_quadratic_model_uncertaintie
+#         """
+#         model_parameters_quad = {
+#             'conjunction_time': -1.415143555084551e-06,
+#             'conjunction_time_err': 0.00042940561938685084,
+#             'period': 1.0914215464474404,
+#             'period_err': 9.150815726215122e-06,
+#             'period_change_by_epoch': 2.7744598987630543e-09,
+#             'period_change_by_epoch_err': 3.188345582283935e-08,
+#             'model_type': 'quadratic',
+#             'model_data': ([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
+#         }
+#         expected_result = np.array([0.00042941, 0.00305304, 0.00310238, 0.00742118])
+#         self.ephemeris.get_ephemeris_uncertainties(model_parameters_quad)
+#         results = self.ephemeris.get_ephemeris_uncertainties(model_parameters_quad)
+#         self.assertTrue(np.allclose(expected_result, results, rtol=1e-05, atol=1e-08)) 
          
-    def test_calc_bic_lin(self):
-        """ Tests the calculation of the linear bic
+#     def test_calc_bic_lin(self):
+#         """ Tests the calculation of the linear bic
 
-            Uses the linear k value and linear chi squared value
-        """
-        model_parameters_linear = {
-            'period': 1.0914223408652188,  
-            'period_err': 9.998517417992763e-07,
-            'conjunction_time': -6.734666196939187e-05, 
-            'conjunction_time_err': 0.0003502975050463415,
-            'model_type': 'linear', 
-            'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
-        }
-        # k_value = 2
-        # linear_chi_squared = 0.29406284565290114
-        expected_result = 3.0666515678926825
-        result = self.ephemeris.calc_bic(model_parameters_linear)
-        self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))   
+#             Uses the linear k value and linear chi squared value
+#         """
+#         model_parameters_linear = {
+#             'period': 1.0914223408652188,  
+#             'period_err': 9.998517417992763e-07,
+#             'conjunction_time': -6.734666196939187e-05, 
+#             'conjunction_time_err': 0.0003502975050463415,
+#             'model_type': 'linear', 
+#             'model_data': ([-6.73466620e-05,  3.20878101e+02,  3.25243790e+02,  6.25384934e+02])
+#         }
+#         # k_value = 2
+#         # linear_chi_squared = 0.29406284565290114
+#         expected_result = 3.0666515678926825
+#         result = self.ephemeris.calc_bic(model_parameters_linear)
+#         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))   
         
-    def test_calc_bic_quad(self):
-        """ Tests the calculation of the quadratic bic
+#     def test_calc_bic_quad(self):
+#         """ Tests the calculation of the quadratic bic
 
-            Uses the quadratic k value and quadratic chi squared value
-        """
-        model_parameters_quad = {
-            'conjunction_time': -1.415143555084551e-06,
-            'conjunction_time_err': 0.00042940561938685084,
-            'period': 1.0914215464474404,
-            'period_err': 9.150815726215122e-06,
-            'period_change_by_epoch': 2.7744598987630543e-09,
-            'period_change_by_epoch_err': 3.188345582283935e-08,
-            'model_type': 'quadratic',
-            'model_data': ([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
-        }
-        # k_value = 3
-        # quad_chi_squared = 0.20766342879185204
-        expected_result = 4.3665465121515235
-        result = self.ephemeris.calc_bic(model_parameters_quad)
-        self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08)) 
+#             Uses the quadratic k value and quadratic chi squared value
+#         """
+#         model_parameters_quad = {
+#             'conjunction_time': -1.415143555084551e-06,
+#             'conjunction_time_err': 0.00042940561938685084,
+#             'period': 1.0914215464474404,
+#             'period_err': 9.150815726215122e-06,
+#             'period_change_by_epoch': 2.7744598987630543e-09,
+#             'period_change_by_epoch_err': 3.188345582283935e-08,
+#             'model_type': 'quadratic',
+#             'model_data': ([-1.41514356e-06,  3.20878053e+02,  3.25243743e+02,  6.25385000e+02])
+#         }
+#         # k_value = 3
+#         # quad_chi_squared = 0.20766342879185204
+#         expected_result = 4.3665465121515235
+#         result = self.ephemeris.calc_bic(model_parameters_quad)
+#         self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08)) 
     
-    def test_calc_delta_bic(self):
-        """ Tests the calulation of the delta bic
+#     def test_calc_delta_bic(self):
+#         """ Tests the calulation of the delta bic
 
-            Uses both the quadratic bic and linear bic
-        """
-        # linear_bic = 3.0666515678926825
-        # quad_bic = 4.3665465121515235
-        expected_result = -1.299894944258841
-        result = self.ephemeris.calc_delta_bic() 
-        self.assertTrue(expected_result, result)
+#             Uses both the quadratic bic and linear bic
+#         """
+#         # linear_bic = 3.0666515678926825
+#         # quad_bic = 4.3665465121515235
+#         expected_result = -1.299894944258841
+#         result = self.ephemeris.calc_delta_bic() 
+#         self.assertTrue(expected_result, result)
 
     
 
     if __name__ == '__main__':
             unittest.main()
```

### Comparing `susie-1.1.0/tests/test_transit_times.py` & `susie-1.1.1/tests/test_transit_times.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import sys
 sys.path.append(".")
 from src.susie.timing_data import TimingData
 import unittest
 import numpy as np
+from numpy.testing import assert_array_equal
+
 
 # test_epochs = [0, 294, 298, 573, 579, 594, 602, 636, 637, 655, 677, 897, 901, 911, 912, 919, 941, 941, 963, 985, 992, 994, 995, 997, 1015, 1247, 1257, 1258, 1260, 1272, 1287, 1290, 1311, 1312, 1313, 1316, 1317, 1323, 1324, 1333, 1334, 1344, 1345, 1346, 1347, 1357, 1365, 1366, 1585, 1589, 1611, 1619, 1621, 1633, 1637, 1640, 1653, 1661, 1662, 1914, 1915, 1916, 1917, 1937, 1938, 1960, 1964, 1967, 1968, 1969, 1978, 1981, 1991, 1996, 2005, 2012, 2019, 2021, 2022, 2264, 2286, 2288, 2318, 2319, 2331, 2332, 2338, 2339, 2371, 2593, 2634, 2635, 2667, 2668, 2690, 2892, 2910, 2921, 2924, 2942, 2943, 2978, 2979, 2984, 2985, 2988, 2992, 2992, 2997, 2999, 3010, 3017, 3018, 3019, 3217, 3239, 3248, 3260, 3261, 3264, 3306, 3307, 3314, 3316, 3318, 3335, 3335, 3336, 3339, 3341, 3341, 3342, 3342, 3345, 3356, 3570, 3625, 3646, 3657]
 # test_mtts = [0.0, 320.8780000000261, 325.24399999994785, 625.3850000002421, 631.933999999892, 648.3059999998659, 657.0360000003129, 694.1440000003204, 695.2370000001974, 714.8820000002161, 738.8940000003204, 979.0049999998882, 983.3710000002757, 994.285000000149, 995.3769999998622, 1003.0160000002943, 1027.0270000002347, 1027.027999999933, 1051.0389999998733, 1075.0509999999776, 1082.691000000108, 1084.8730000001378, 1085.9650000003166, 1088.1480000000447, 1107.7930000000633, 1361.003000000026, 1371.9169999998994, 1373.0079999999143, 1375.191000000108, 1388.2889999998733, 1404.658999999985, 1407.933999999892, 1430.8530000001192, 1431.945000000298, 1433.036000000313, 1436.3100000000559, 1437.4020000002347, 1443.9500000001863, 1445.0419999998994, 1454.8640000000596, 1455.9560000002384, 1466.8700000001118, 1467.9620000002906, 1469.0530000003055, 1470.1450000000186, 1481.058999999892, 1489.7900000000373, 1490.8810000000522, 1729.9020000002347, 1734.2690000003204, 1758.2800000002608, 1767.0109999999404, 1769.194000000134, 1782.2910000002012, 1786.657000000123, 1789.9300000001676, 1804.1189999999478, 1812.851000000257, 1813.942000000272, 2088.9799999999814, 2090.0709999999963, 2091.163000000175, 2092.25400000019, 2114.0819999999367, 2115.1740000001155, 2139.185000000056, 2143.5509999999776, 2146.8250000001863, 2147.916000000201, 2149.0079999999143, 2158.8310000002384, 2162.1049999999814, 2173.0190000003204, 2178.4769999999553, 2188.2990000001155, 2195.939000000246, 2203.5789999999106, 2205.7620000001043, 2206.853000000119, 2470.9769999999553, 2494.9879999998957, 2497.1710000000894, 2529.913000000175, 2531.0049999998882, 2544.1019999999553, 2545.19299999997, 2551.7420000000857, 2552.8330000001006, 2587.7590000000782, 2830.0540000000037, 2874.8020000001416, 2875.8930000001565, 2910.81799999997, 2911.910000000149, 2935.9210000000894, 3156.388000000268, 3176.033999999985, 3188.0389999998733, 3191.313000000082, 3210.9590000002645, 3212.0500000002794, 3250.25, 3251.341000000015, 3256.7990000001155, 3257.8900000001304, 3261.1639999998733, 3265.529000000097, 3265.530999999959, 3270.9870000001974, 3273.1699999999255, 3285.1750000002794, 3292.814999999944, 3293.907000000123, 3294.998000000138, 3511.098999999929, 3535.1099999998696, 3544.933999999892, 3558.0300000002608, 3559.121999999974, 3562.3960000001825, 3608.2349999998696, 3609.3270000000484, 3616.966000000015, 3619.149999999907, 3621.3330000001006, 3639.885000000242, 3639.8870000001043, 3640.978000000119, 3644.253000000026, 3646.435000000056, 3646.435000000056, 3647.526000000071, 3647.526000000071, 3650.8009999999776, 3662.805999999866, 3896.3700000001118, 3956.3980000000447, 3979.31799999997, 3991.323000000324]
 # test_mtts_err = [0.00043, 0.00028, 0.00062, 0.00042, 0.00043, 0.00032, 0.00036, 0.00046, 0.00041, 0.00019, 0.00043, 0.00072, 0.00079, 0.00037, 0.00031, 0.0004, 0.0004, 0.00028, 0.00028, 0.00068, 0.00035, 0.00029, 0.00024, 0.00029, 0.00039, 0.00027, 0.00021, 0.00027, 0.00024, 0.00032, 0.00031, 0.00022, 0.00018, 0.00017, 0.00033, 0.00011, 0.0001, 0.00017, 0.00032, 0.00039, 0.00035, 0.00034, 0.00035, 0.00032, 0.00042, 0.00037, 0.00037, 0.00031, 0.00033, 0.00039, 0.0003, 0.0003, 0.0003, 0.0003, 0.00046, 0.00024, 0.00038, 0.00027, 0.00029, 0.00021, 0.0003, 0.00033, 0.00071, 0.00019, 0.00043, 0.00034, 0.00034, 0.00019, 0.00019, 0.00031, 0.00028, 0.00032, 0.0004, 0.00029, 0.00029, 0.00025, 0.00034, 0.00034, 0.00046, 0.00043, 0.00039, 0.00049, 0.00046, 0.00049, 0.00035, 0.00036, 0.00022, 0.0002, 0.00031, 0.00042, 0.00033, 0.00033, 0.00055, 0.00023, 0.00021, 0.00035, 0.00025, 0.00034, 0.00037, 0.00028, 0.00023, 0.00028, 0.00039, 0.00024, 0.00022, 0.00029, 0.00043, 0.00036, 0.00026, 0.00048, 0.00032, 0.0004, 0.00018, 0.00021, 0.00056, 0.00023, 0.0003, 0.00022, 0.00034, 0.00028, 0.00027, 0.00035, 0.00031, 0.00032, 0.00033, 0.0005, 0.00031, 0.00032, 0.00091, 0.00035, 0.00026, 0.00021, 0.00034, 0.00034, 0.00038, 0.0004, 0.00026, 0.0003, 0.00044]
 test_epochs = np.array([0, 294, 298, 573])
 test_mtts = np.array([0.0, 320.8780000000261, 325.24399999994785, 625.3850000002421])
 test_mtts_err = np.array([0.00043, 0.00028, 0.00062, 0.00042])
@@ -74,18 +76,18 @@
 
     # Test successful np.arrays
     def test_suc_arrays(self):
         """ Successful test to check that epochs, mid times, mid time uncertainties, and tra_or_occ are all type np.arrays
 
         """
         self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, tra_or_occ, time_scale='tdb')
-        self.assertTrue(all(isinstance(value, np.ndarray) for value in self.timing_data.epochs))
-        self.assertTrue(all(isinstance(value, np.ndarray) for value in self.timing_data.mid_times))
-        self.assertTrue(all(isinstance(value, np.ndarray) for value in self.timing_data.mid_time_uncertainties))  
-        self.assertTrue(all(isinstance(value, np.ndarray) for value in self.timing_data.tra_or_occ))  
+        self.assertTrue(isinstance( self.timing_data.epochs, np.ndarray))
+        self.assertTrue(isinstance(self.timing_data.mid_times, np.ndarray))
+        self.assertTrue(isinstance(self.timing_data.mid_time_uncertainties, np.ndarray))
+        self.assertTrue(isinstance(self.timing_data.tra_or_occ, np.ndarray))
 
     # Tests for unsucessful np.arrays
     def test_us_epochs_arr_type_str(self):
         """ Unsuccessful test to check for numpy array validation for the epochs.
             
             The epochs are strings instead of numpy array and should raise an error.
         """
@@ -264,15 +266,17 @@
 
     # Tests for the same shape of arrays
     def test_variable_shape(self):
         """ Successful test to check that all of the varibles have the same shape.
 
         """
         self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, tra_or_occ, time_scale='tdb')
-        self.assertEqual(test_epochs.shape, test_mtts.shape, test_mtts_err.shape, tra_or_occ.shape)
+        self.assertEqual(test_epochs.shape, test_mtts.shape)
+        self.assertEqual(test_epochs.shape, test_mtts_err.shape)
+        self.assertEqual(test_epochs.shape, tra_or_occ.shape)
 
     def test_variable_shape_fail(self):
         """ Unsuccessful test of the varibles shape.
 
             The epochs, mid times and mid time uncertainties all have different shapes.
         """
         new_test_epochs= np.array([0, 298, 573])  
@@ -323,20 +327,19 @@
     
     # def calc_bary_time_uncertinties(self):
     #    test_mtts_err=np.array([1.0, 1.0, 1.0, 1.0])
     #    self.timing_data =  TimingData('jd', test_epochs, test_mtts,test_mtts_err, object_ra=97.64, object_dec=29.67, observatory_lat=43.60, observatory_lon=-116.21)
 
 
     # Tests for validate tra_or_occ
-    ###### NEED TO FINISH ######
     def test_tra_or_occ_None(self):
-        self.timing_data = TimingData('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb', tra_or_occ = None)
+        self.timing_data = TimingData('jd', test_epochs, test_mtts, test_mtts_err, tra_or_occ = None, time_scale='tdb')
         expected_result = np.array(['tra','tra','tra','tra'])
-        result = self.timing_data._validate()
-        self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
+        result = self.timing_data.tra_or_occ
+        assert_array_equal(expected_result, result)
 
     
     def test_only_tra_or_occ_value(self):
         """ Unsuccessful test to check if the tra_or_occ array contains values other than 'tra' or 'occ'.
 
         """
         not_tra_or_occ = np.array(['tra','occ','trac','oc'])
@@ -353,17 +356,19 @@
 
 
     def test_tra_or_occ_shape(self):
         """ Unsuccessful test to check the length of the tra_or_occ array.
 
             The tra_or_occ array must be the same length as the epochs. mid times and mid time uncertainties arrays.
         """
+        not_test_epochs = np.array([0,1])
+        not_test_mtts = np.array([0.,1.0,3.0,4.0,5.0])
         not_tra_or_occ = np.array(['occ','tra','occ'])
         with self.assertRaises(ValueError, msg= "Shapes of 'tra_or_occ', 'mid_time_uncertainties', and 'mid_times' arrays do not match."):
-             TimingData('jd', test_epochs, test_mtts, test_mtts_err,not_tra_or_occ, time_scale='tdb')  
+             TimingData('jd', not_test_epochs, not_test_mtts, test_mtts_err,not_tra_or_occ, time_scale='tdb')  
 
     def test_tra_or_occ_str(self):
         """ Unsuccessful test to check the data values within the tra_or_occ array.
 
             The data values must be a string and will raise an error if not.
         """
         not_tra_or_occ = np.array([1,2,3,4])
```

