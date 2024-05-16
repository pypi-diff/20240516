# Comparing `tmp/sparse-lmm-0.8.tar.gz` & `tmp/sparse-lmm-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse-lmm-0.8.tar", last modified: Mon May 13 00:56:48 2024, max compression
+gzip compressed data, was "sparse-lmm-0.9.tar", last modified: Mon May 13 01:24:36 2024, max compression
```

## Comparing `sparse-lmm-0.8.tar` & `sparse-lmm-0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/
--rw-rw-r--   0 techt     (1000) techt     (1000)        8 2024-01-02 05:58:54.000000 sparse-lmm-0.8/.gitignore
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/.idea/
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/.idea/inspectionProfiles/
--rw-rw-r--   0 techt     (1000) techt     (1000)      174 2023-10-13 15:02:00.000000 sparse-lmm-0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      177 2023-10-13 15:02:00.000000 sparse-lmm-0.8/.idea/misc.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      300 2023-10-13 15:10:13.000000 sparse-lmm-0.8/.idea/modules.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      441 2023-10-13 20:23:31.000000 sparse-lmm-0.8/.idea/sparse-lmm.iml
--rw-rw-r--   0 techt     (1000) techt     (1000)      180 2023-10-13 15:02:00.000000 sparse-lmm-0.8/.idea/vcs.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)    14213 2024-05-13 00:56:07.000000 sparse-lmm-0.8/.idea/workspace.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)     1071 2023-09-18 00:20:17.000000 sparse-lmm-0.8/LICENSE.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-13 00:56:48.031495 sparse-lmm-0.8/PKG-INFO
--rw-rw-r--   0 techt     (1000) techt     (1000)        0 2023-09-18 03:45:22.000000 sparse-lmm-0.8/README.md
--rw-rw-r--   0 techt     (1000) techt     (1000)    39332 2023-09-17 23:16:18.000000 sparse-lmm-0.8/combined_plots.png
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/dist/
--rw-rw-r--   0 techt     (1000) techt     (1000)    43128 2023-10-13 20:31:30.000000 sparse-lmm-0.8/dist/sparse-lmm-0.4.tar.gz
--rw-rw-r--   0 techt     (1000) techt     (1000)     7102 2023-10-13 20:31:30.000000 sparse-lmm-0.8/dist/sparse_lmm-0.4-py3-none-any.whl
--rw-rw-r--   0 techt     (1000) techt     (1000)       38 2024-05-13 00:56:48.031495 sparse-lmm-0.8/setup.cfg
--rw-rw-r--   0 techt     (1000) techt     (1000)      576 2024-05-13 00:54:10.000000 sparse-lmm-0.8/setup.py
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/sparse_lmm/
--rw-rw-r--   0 techt     (1000) techt     (1000)     9815 2024-05-13 00:53:56.000000 sparse-lmm-0.8/sparse_lmm/VariableSelection.py
--rw-rw-r--   0 techt     (1000) techt     (1000)     8341 2024-01-02 05:12:00.000000 sparse-lmm-0.8/sparse_lmm/VariableSelection_new.py
--rw-rw-r--   0 techt     (1000) techt     (1000)      236 2023-09-18 04:02:20.000000 sparse-lmm-0.8/sparse_lmm/__init__.py
--rw-rw-r--   0 techt     (1000) techt     (1000)    37017 2024-01-02 03:51:59.000000 sparse-lmm-0.8/sparse_lmm/combined_plots.png
--rwxrwxr-x   0 techt     (1000) techt     (1000)     5011 2023-09-14 18:54:06.000000 sparse-lmm-0.8/sparse_lmm/helpingMethods.py
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/sparse_lmm.egg-info/
--rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-13 00:56:47.000000 sparse-lmm-0.8/sparse_lmm.egg-info/PKG-INFO
--rw-rw-r--   0 techt     (1000) techt     (1000)      586 2024-05-13 00:56:48.000000 sparse-lmm-0.8/sparse_lmm.egg-info/SOURCES.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)        1 2024-05-13 00:56:47.000000 sparse-lmm-0.8/sparse_lmm.egg-info/dependency_links.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)       12 2024-05-13 00:56:47.000000 sparse-lmm-0.8/sparse_lmm.egg-info/requires.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)       11 2024-05-13 00:56:47.000000 sparse-lmm-0.8/sparse_lmm.egg-info/top_level.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)     1734 2023-10-13 01:48:51.000000 sparse-lmm-0.8/test.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 01:24:36.904640 sparse-lmm-0.9/
+-rw-rw-r--   0 techt     (1000) techt     (1000)        8 2024-01-02 05:58:54.000000 sparse-lmm-0.9/.gitignore
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 01:24:36.900640 sparse-lmm-0.9/.idea/
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 01:24:36.904640 sparse-lmm-0.9/.idea/inspectionProfiles/
+-rw-rw-r--   0 techt     (1000) techt     (1000)      174 2023-10-13 15:02:00.000000 sparse-lmm-0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      177 2023-10-13 15:02:00.000000 sparse-lmm-0.9/.idea/misc.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      300 2023-10-13 15:10:13.000000 sparse-lmm-0.9/.idea/modules.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      441 2023-10-13 20:23:31.000000 sparse-lmm-0.9/.idea/sparse-lmm.iml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      180 2023-10-13 15:02:00.000000 sparse-lmm-0.9/.idea/vcs.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)    14213 2024-05-13 01:24:35.000000 sparse-lmm-0.9/.idea/workspace.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)     1071 2023-09-18 00:20:17.000000 sparse-lmm-0.9/LICENSE.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-13 01:24:36.904640 sparse-lmm-0.9/PKG-INFO
+-rw-rw-r--   0 techt     (1000) techt     (1000)        0 2023-09-18 03:45:22.000000 sparse-lmm-0.9/README.md
+-rw-rw-r--   0 techt     (1000) techt     (1000)    39332 2023-09-17 23:16:18.000000 sparse-lmm-0.9/combined_plots.png
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 01:24:36.904640 sparse-lmm-0.9/dist/
+-rw-rw-r--   0 techt     (1000) techt     (1000)    43128 2023-10-13 20:31:30.000000 sparse-lmm-0.9/dist/sparse-lmm-0.4.tar.gz
+-rw-rw-r--   0 techt     (1000) techt     (1000)     7102 2023-10-13 20:31:30.000000 sparse-lmm-0.9/dist/sparse_lmm-0.4-py3-none-any.whl
+-rw-rw-r--   0 techt     (1000) techt     (1000)       38 2024-05-13 01:24:36.904640 sparse-lmm-0.9/setup.cfg
+-rw-rw-r--   0 techt     (1000) techt     (1000)      576 2024-05-13 01:24:30.000000 sparse-lmm-0.9/setup.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 01:24:36.904640 sparse-lmm-0.9/sparse_lmm/
+-rw-rw-r--   0 techt     (1000) techt     (1000)     9412 2024-05-13 01:23:19.000000 sparse-lmm-0.9/sparse_lmm/VariableSelection.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)     8341 2024-01-02 05:12:00.000000 sparse-lmm-0.9/sparse_lmm/VariableSelection_new.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)      236 2023-09-18 04:02:20.000000 sparse-lmm-0.9/sparse_lmm/__init__.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)    37017 2024-01-02 03:51:59.000000 sparse-lmm-0.9/sparse_lmm/combined_plots.png
+-rwxrwxr-x   0 techt     (1000) techt     (1000)     5011 2023-09-14 18:54:06.000000 sparse-lmm-0.9/sparse_lmm/helpingMethods.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 01:24:36.904640 sparse-lmm-0.9/sparse_lmm.egg-info/
+-rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-13 01:24:36.000000 sparse-lmm-0.9/sparse_lmm.egg-info/PKG-INFO
+-rw-rw-r--   0 techt     (1000) techt     (1000)      586 2024-05-13 01:24:36.000000 sparse-lmm-0.9/sparse_lmm.egg-info/SOURCES.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)        1 2024-05-13 01:24:36.000000 sparse-lmm-0.9/sparse_lmm.egg-info/dependency_links.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)       12 2024-05-13 01:24:36.000000 sparse-lmm-0.9/sparse_lmm.egg-info/requires.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)       11 2024-05-13 01:24:36.000000 sparse-lmm-0.9/sparse_lmm.egg-info/top_level.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)     1734 2023-10-13 01:48:51.000000 sparse-lmm-0.9/test.py
```

### Comparing `sparse-lmm-0.8/.idea/workspace.xml` & `sparse-lmm-0.9/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `sparse-lmm-0.8/.idea/workspace.xml` & `sparse-lmm-0.9/.idea/workspace.xml`

```diff
@@ -237,15 +237,15 @@
       <workItem from="1704830174041" duration="628000"/>
       <workItem from="1704920402164" duration="619000"/>
       <workItem from="1705458945901" duration="11000"/>
       <workItem from="1705614736560" duration="316000"/>
       <workItem from="1706066522765" duration="2781000"/>
       <workItem from="1711508793025" duration="1057000"/>
       <workItem from="1711761443949" duration="581000"/>
-      <workItem from="1715282022782" duration="10098000"/>
+      <workItem from="1715282022782" duration="11806000"/>
     </task>
     <task id="LOCAL-00001" summary="update">
       <created>1704167599803</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1704167599803</updated>
```

### Comparing `sparse-lmm-0.8/LICENSE.txt` & `sparse-lmm-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.8/combined_plots.png` & `sparse-lmm-0.9/combined_plots.png`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.8/dist/sparse-lmm-0.4.tar.gz` & `sparse-lmm-0.9/dist/sparse-lmm-0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.8/dist/sparse_lmm-0.4-py3-none-any.whl` & `sparse-lmm-0.9/dist/sparse_lmm-0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.8/setup.py` & `sparse-lmm-0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sparse-lmm',
-    version='0.8',
+    version='0.9',
     packages=find_packages(),
     install_requires=['scipy', 'numpy'
                       ],
     author='Haohan Wang',
     author_email='haohanw@illinois.edu',
     description='An implementation of Linear Mixed Model, a statistical model that promotes sparse variable selection '
                 'in the presence of correlated and linearly dependent variables. ',
```

### Comparing `sparse-lmm-0.8/sparse_lmm/VariableSelection.py` & `sparse-lmm-0.9/sparse_lmm/VariableSelection.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,29 +225,20 @@
         if X_new.ndim == 1:
             X_new = X_new.reshape(1, -1)
 
         # Check if necessary parameters are initialized
         if self.K is None or self.U is None or self.S is None:
             raise ValueError("Model has not been properly initialized with training data.")
 
-        # Project the new data using the U matrix derived from training
-        U_new = np.dot(X_new, self.U)
-
-        # Scale the transformed data by the diagonal matrix Sdi_sqrt derived from training
-        delta0_new = np.exp(self.ldelta0)
-        Sdi_new = 1. / (self.S + delta0_new)
-        Sdi_sqrt_new = np.sqrt(Sdi_new)
-        SUX_new = U_new * np.tile(Sdi_sqrt_new, (X_new.shape[1], 1)).T
-
         # Multiply the transformed data by beta coefficients to get predictions
         # Ensure beta is reshaped appropriately for matrix multiplication
         if self.beta.ndim == 1:
             self.beta = self.beta.reshape(-1, 1)
 
-        y_pred = np.dot(SUX_new, self.beta) + self.lasso.intercept_
+        y_pred = np.dot(X_new, self.beta) + self.lasso.intercept_
 
         return y_pred.flatten()  # Flatten in case the output is a single sample
 
     def getBeta(self):
         return self.beta
 
 if __name__ == '__main__':
```

### Comparing `sparse-lmm-0.8/sparse_lmm/VariableSelection_new.py` & `sparse-lmm-0.9/sparse_lmm/VariableSelection_new.py`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.8/sparse_lmm/combined_plots.png` & `sparse-lmm-0.9/sparse_lmm/combined_plots.png`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.8/sparse_lmm/helpingMethods.py` & `sparse-lmm-0.9/sparse_lmm/helpingMethods.py`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.8/sparse_lmm.egg-info/SOURCES.txt` & `sparse-lmm-0.9/sparse_lmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.8/test.py` & `sparse-lmm-0.9/test.py`

 * *Files identical despite different names*

