# Comparing `tmp/geospann-0.1.3.tar.gz` & `tmp/geospann-0.1.4.tar.gz`

## Comparing `geospann-0.1.3.tar` & `geospann-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 geospann-0.1.3/.pypirc
--rw-r--r--   0        0        0  1032391 2020-02-02 00:00:00.000000 geospann-0.1.3/Example_realdata.ipynb
--rw-r--r--   0        0        0   366374 2020-02-02 00:00:00.000000 geospann-0.1.3/Example_simulation.ipynb
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 geospann-0.1.3/Example_simulation.md
--rw-r--r--   0        0        0    64623 2020-02-02 00:00:00.000000 geospann-0.1.3/Running_time.ipynb
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geospann-0.1.3/.idea/.gitignore
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 geospann-0.1.3/.idea/.name
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 geospann-0.1.3/.idea/NN-GLS.iml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 geospann-0.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 geospann-0.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 geospann-0.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 geospann-0.1.3/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 geospann-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0  1032391 2020-02-02 00:00:00.000000 geospann-0.1.3/.ipynb_checkpoints/Example_realdata-checkpoint.ipynb
--rw-r--r--   0        0        0   366374 2020-02-02 00:00:00.000000 geospann-0.1.3/.ipynb_checkpoints/Example_simulation-checkpoint.ipynb
--rw-r--r--   0        0        0    64623 2020-02-02 00:00:00.000000 geospann-0.1.3/.ipynb_checkpoints/Running_time-checkpoint.ipynb
--rw-r--r--   0        0        0    97026 2020-02-02 00:00:00.000000 geospann-0.1.3/data/Normalized_PM2.5_20190605.csv
--rw-r--r--   0        0        0   180525 2020-02-02 00:00:00.000000 geospann-0.1.3/data/US_heat_0605.png
--rwxr-xr-x   0        0        0  1112364 2020-02-02 00:00:00.000000 geospann-0.1.3/data/covariate0605.csv
--rw-r--r--   0        0        0   259168 2020-02-02 00:00:00.000000 geospann-0.1.3/data/nngls.png
--rwxr-xr-x   0        0        0    32432 2020-02-02 00:00:00.000000 geospann-0.1.3/data/pm25_0605.csv
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 geospann-0.1.3/data/running_time.csv
--rw-r--r--   0        0        0    93119 2020-02-02 00:00:00.000000 geospann-0.1.3/data/output_figures/output_10_0.png
--rw-r--r--   0        0        0    34117 2020-02-02 00:00:00.000000 geospann-0.1.3/data/output_figures/output_7_0.png
--rw-r--r--   0        0        0    53531 2020-02-02 00:00:00.000000 geospann-0.1.3/data/output_figures/output_8_0.png
--rw-r--r--   0        0        0    84381 2020-02-02 00:00:00.000000 geospann-0.1.3/data/output_figures/output_9_0.png
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geospann-0.1.3/geospaNN/__init__.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 geospann-0.1.3/geospaNN/main.py
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 geospann-0.1.3/geospaNN/model.py
--rw-r--r--   0        0        0    37612 2020-02-02 00:00:00.000000 geospann-0.1.3/geospaNN/utils.py
--rw-r--r--   0        0        0    13446 2020-02-02 00:00:00.000000 geospann-0.1.3/tests/test.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 geospann-0.1.3/LICENSE
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 geospann-0.1.3/README.md
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 geospann-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 geospann-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0  1032391 2020-02-02 00:00:00.000000 geospann-0.1.4/Example_realdata.ipynb
+-rw-r--r--   0        0        0   366374 2020-02-02 00:00:00.000000 geospann-0.1.4/Example_simulation.ipynb
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 geospann-0.1.4/Example_simulation.md
+-rw-r--r--   0        0        0    64623 2020-02-02 00:00:00.000000 geospann-0.1.4/Running_time.ipynb
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geospann-0.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 geospann-0.1.4/.idea/.name
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 geospann-0.1.4/.idea/NN-GLS.iml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 geospann-0.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 geospann-0.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 geospann-0.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 geospann-0.1.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 geospann-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0  1032391 2020-02-02 00:00:00.000000 geospann-0.1.4/.ipynb_checkpoints/Example_realdata-checkpoint.ipynb
+-rw-r--r--   0        0        0   366374 2020-02-02 00:00:00.000000 geospann-0.1.4/.ipynb_checkpoints/Example_simulation-checkpoint.ipynb
+-rw-r--r--   0        0        0    64623 2020-02-02 00:00:00.000000 geospann-0.1.4/.ipynb_checkpoints/Running_time-checkpoint.ipynb
+-rw-r--r--   0        0        0    97026 2020-02-02 00:00:00.000000 geospann-0.1.4/data/Normalized_PM2.5_20190605.csv
+-rw-r--r--   0        0        0   180525 2020-02-02 00:00:00.000000 geospann-0.1.4/data/US_heat_0605.png
+-rwxr-xr-x   0        0        0  1112364 2020-02-02 00:00:00.000000 geospann-0.1.4/data/covariate0605.csv
+-rw-r--r--   0        0        0   259168 2020-02-02 00:00:00.000000 geospann-0.1.4/data/nngls.png
+-rwxr-xr-x   0        0        0    32432 2020-02-02 00:00:00.000000 geospann-0.1.4/data/pm25_0605.csv
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 geospann-0.1.4/data/running_time.csv
+-rw-r--r--   0        0        0    93119 2020-02-02 00:00:00.000000 geospann-0.1.4/data/output_figures/output_10_0.png
+-rw-r--r--   0        0        0    34117 2020-02-02 00:00:00.000000 geospann-0.1.4/data/output_figures/output_7_0.png
+-rw-r--r--   0        0        0    53531 2020-02-02 00:00:00.000000 geospann-0.1.4/data/output_figures/output_8_0.png
+-rw-r--r--   0        0        0    84381 2020-02-02 00:00:00.000000 geospann-0.1.4/data/output_figures/output_9_0.png
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geospann-0.1.4/geospaNN/__init__.py
+-rw-r--r--   0        0        0    11498 2020-02-02 00:00:00.000000 geospann-0.1.4/geospaNN/main.py
+-rw-r--r--   0        0        0    15362 2020-02-02 00:00:00.000000 geospann-0.1.4/geospaNN/model.py
+-rw-r--r--   0        0        0    37733 2020-02-02 00:00:00.000000 geospann-0.1.4/geospaNN/utils.py
+-rw-r--r--   0        0        0    13502 2020-02-02 00:00:00.000000 geospann-0.1.4/tests/test.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 geospann-0.1.4/LICENSE
+-rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 geospann-0.1.4/README.md
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 geospann-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 geospann-0.1.4/PKG-INFO
```

### Comparing `geospann-0.1.3/Example_realdata.ipynb` & `geospann-0.1.4/Example_realdata.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/Example_simulation.ipynb` & `geospann-0.1.4/Example_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/Example_simulation.md` & `geospann-0.1.4/Example_simulation.md`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/Running_time.ipynb` & `geospann-0.1.4/Running_time.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/.idea/workspace.xml` & `geospann-0.1.4/.idea/workspace.xml`

 * *Files 11% similar despite different names*

#### Comparing `geospann-0.1.3/.idea/workspace.xml` & `geospann-0.1.4/.idea/workspace.xml`

```diff
@@ -1,14 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="55b6d3ef-0094-4559-b139-f97e41838c95" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/.pypirc" beforeDir="false" afterPath="$PROJECT_DIR$/.pypirc" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/dist/geospann-0.1.2-py3-none-any.whl" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/dist/geospann-0.1.2.tar.gz" beforeDir="false"/>
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/dist/geospann-0.1.3-py3-none-any.whl" beforeDir="false"/>
+      <change beforePath="$PROJECT_DIR$/dist/geospann-0.1.3.tar.gz" beforeDir="false"/>
+      <change beforePath="$PROJECT_DIR$/geospaNN/main.py" beforeDir="false" afterPath="$PROJECT_DIR$/geospaNN/main.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/geospaNN/model.py" beforeDir="false" afterPath="$PROJECT_DIR$/geospaNN/model.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/geospaNN/utils.py" beforeDir="false" afterPath="$PROJECT_DIR$/geospaNN/utils.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
```

### Comparing `geospann-0.1.3/.ipynb_checkpoints/Example_realdata-checkpoint.ipynb` & `geospann-0.1.4/.ipynb_checkpoints/Example_realdata-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/.ipynb_checkpoints/Example_simulation-checkpoint.ipynb` & `geospann-0.1.4/.ipynb_checkpoints/Example_simulation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/.ipynb_checkpoints/Running_time-checkpoint.ipynb` & `geospann-0.1.4/.ipynb_checkpoints/Running_time-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/Normalized_PM2.5_20190605.csv` & `geospann-0.1.4/data/Normalized_PM2.5_20190605.csv`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/US_heat_0605.png` & `geospann-0.1.4/data/US_heat_0605.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/covariate0605.csv` & `geospann-0.1.4/data/covariate0605.csv`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/nngls.png` & `geospann-0.1.4/data/nngls.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/pm25_0605.csv` & `geospann-0.1.4/data/pm25_0605.csv`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/running_time.csv` & `geospann-0.1.4/data/running_time.csv`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/output_figures/output_10_0.png` & `geospann-0.1.4/data/output_figures/output_10_0.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/output_figures/output_7_0.png` & `geospann-0.1.4/data/output_figures/output_7_0.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/output_figures/output_8_0.png` & `geospann-0.1.4/data/output_figures/output_8_0.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/data/output_figures/output_9_0.png` & `geospann-0.1.4/data/output_figures/output_9_0.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/geospaNN/utils.py` & `geospann-0.1.4/geospaNN/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     Attributes
     ----------
     B : torch.Tensor | numpy.array
         nxp array contains all non-zero values in B_dense.
     n : int
         The number of samples.
     neighbor_size : int
-        i.e. p in the documentation, the largest number of non-zero values in each row of B_dense.
+        i.e. k in the documentation, the largest number of non-zero values in each row of B_dense.
     Ind_list : numpy.array
         The nxp index array indicating the location where values in B was in B_dense. For example, the [i,j]'s index is k
         means that B_dense[i,k] = B[i,j].
 
     Methods
     -------
     to_numpy()
@@ -316,14 +316,18 @@
         D = torch.linalg.cholesky(cov)
         res = torch.matmul(torch.randn(1, n), D.t()) + mu
     elif isinstance(cov, NNGP_cov):
         if sparse:
             res = cov.correlate(torch.randn(1, n).reshape(-1)) + mu
         else:
             warnings.warn("To be implemented.")
+    else:
+        warnings.warn("Covariance matrix should be in the format of torch.Tensor or NNGP_cov.")
+        return
+
     return  res.reshape(-1)
 
 def make_rank(coord: torch.Tensor,
               neighbor_size: int,
               coord_ref: Optional = None
               ) -> np.ndarray:
     """Compose the nearest neighbor index list based on the coordinates.
@@ -332,18 +336,18 @@
     The index is based on the increasing order of the distances between ith location and the locations in the reference set.
 
     Parameters
     ----------
     coord
         The nxd coordinates array of target locations.
     neighbor_size
-    `   Suppose neighbor_size = p, only the top p nearest indexes will be returned.
+    `   Suppose neighbor_size = k, only the top k-nearest indexes will be returned.
     coord_ref
         The n_refxd coordinates array of reference locations. If None, use the target set itself as the reference.
-        (Any location's neighbor does not includes itself.)
+        (Any location's neighbor does not include itself.)
 
     Returns
     -------
     np.array
         A nxp array. The ith row is the indexes of the nearest neighbors for the ith location, ordered by the distance.
     """
     if coord_ref is None: neighbor_size += 1
@@ -890,15 +894,15 @@
     return batch
 
 def theta_update(theta0: torch.Tensor,
                  w: torch.Tensor,
                  coord: torch.Tensor,
                  neighbor_size: Optional[int] = 20
                  ) -> np.array:
-    """Update the spatial parameters using maximum likelihood
+    """Update the spatial parameters using maximum likelihood.
 
     This function updates the spatial parameters by assuming the observations are from a Gaussian Process with exponential
     covariance function. Spatial coordinates and initial values of theta are input for building the covariance.
     And L-BFGS-B algorithm is used to optimize the likelihood.
     Since the likelihood is computed repeatedly, NNGP approximation is used for efficient computation of the log-likelihood,
     with a default neighbor size being 20.
 
@@ -987,15 +991,14 @@
     theta
         theta[0], theta[1], theta[2] represent \sigma^2, \phi, \tau in the exponential covariance family.
     neighbor_size
         The number of nearest neighbors used for NNGP approximation. Default being 20.
     q
         Confidence coverage for the prediction interval. Default being 0.95.
 
-
     Returns
     -------
     w_test: torch.Tensor
         The kriging prediction.
     pred_U: torch.Tensor
         Confidence upper bound.
     pred_L: torch.Tensor
```

### Comparing `geospann-0.1.3/tests/test.py` & `geospann-0.1.4/tests/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-#import nngls
+import geospaNN
 import numpy as np
 import time
 import pandas as pd
 
 def f5(X): return (10*np.sin(np.pi*X[:,0]*X[:,1]) + 20*(X[:,2]-0.5)**2 + 10*X[:,3] +5*X[:,4])/6
 
 sigma = 1
@@ -15,50 +15,50 @@
 
 n = 1000
 rand = 0
 nn = 20
 batch_size = 50
 
 torch.manual_seed(2023 + rand)
-X, Y, coord, cov, corerr = Simulation(n, p, nn, funXY, theta, range=[0, 10])
+X, Y, coord, cov, corerr = geospaNN.Simulation(n, p, nn, funXY, theta, range=[0, 10])
 if False:
     np.random.seed(2023+rand)
     X, Y, I_B, F_diag, rank, coord, cov, corerr = Simulate(n, p, funXY, nn, theta.detach().numpy(), method=method, a=0,
                                                                  b=10, sparse = Sparse)
     corerr = torch.from_numpy(corerr)
     coord = torch.from_numpy(coord)
     id = range(int(n))
     print(BRISC_estimation(corerr[id].detach().numpy(), None, coord[id,:].detach().numpy())[1])
     theta_update(torch.tensor([1, 1.5, 0.01]), corerr[id], coord[id,:], neighbor_size = 20)
-data = make_graph(X, Y, coord, nn)
-data_train, data_val, data_test = split_data(X, Y, coord, neighbor_size=20,
+data = geospaNN.make_graph(X, Y, coord, nn)
+data_train, data_val, data_test = geospaNN.split_data(X, Y, coord, neighbor_size=20,
                                              test_proportion=0.2)
 
 mlp = torch.nn.Sequential(
     torch.nn.Linear(p, 50),
     torch.nn.ReLU(),
     torch.nn.Linear(50, 20),
     torch.nn.ReLU(),
     torch.nn.Linear(20, 10),
     torch.nn.ReLU(),
     torch.nn.Linear(10, 1),
 )
-nn_model = nn_train(mlp, lr =  0.01, min_delta = 0.001)
+nn_model = geospaNN.nn_train(mlp, lr =  0.01, min_delta = 0.001)
 training_log = nn_model.train(data_train, data_val, data_test)
-theta0 = theta_update(torch.tensor([1, 1.5, 0.01]), mlp(data_train.x).squeeze() - data_train.y, data_train.pos, neighbor_size = 20)
+theta0 = geospaNN.theta_update(torch.tensor([1, 1.5, 0.01]), mlp(data_train.x).squeeze() - data_train.y, data_train.pos, neighbor_size = 20)
 mlp = torch.nn.Sequential(
     torch.nn.Linear(p, 50),
     torch.nn.ReLU(),
     torch.nn.Linear(50, 20),
     torch.nn.ReLU(),
     torch.nn.Linear(20, 10),
     torch.nn.ReLU(),
     torch.nn.Linear(10, 1),
 )
-model = nngls(p=p, neighbor_size=nn, coord_dimensions=2, mlp=mlp, theta=torch.tensor(theta0))
+model = geospaNN.nngls(p=p, neighbor_size=nn, coord_dimensions=2, mlp=mlp, theta=torch.tensor(theta0))
 nngls_model = nngls_train(model, lr =  0.01, min_delta = 0.001)
 training_log = nngls_model.train(data_train, data_val, data_test,
                                  Update_init = 100, Update_step = 10)
 theta_hat = theta_update(torch.tensor(theta0),
                          model.estimate(data_train.x).squeeze() - data_train.y,
                          data_train.pos, neighbor_size = nn)
```

### Comparing `geospann-0.1.3/LICENSE` & `geospann-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geospann-0.1.3/README.md` & `geospann-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,533 +1,580 @@
 00000000: 5b21 5b50 7950 495d 2868 7474 7073 3a2f  [![PyPI](https:/
 00000010: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000020: 7079 7069 2f76 2f67 656f 7370 614e 4e29  pypi/v/geospaNN)
-00000030: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-00000040: 7267 2f70 726f 6a65 6374 2f67 656f 7370  rg/project/geosp
-00000050: 614e 4e29 0a0a 2320 4765 6f73 7061 4e4e  aNN)..# GeospaNN
-00000060: 202d 204e 6575 7261 6c20 6e65 7477 6f72   - Neural networ
-00000070: 6b73 2066 6f72 2067 656f 7370 6174 6961  ks for geospatia
-00000080: 6c20 6461 7461 0a2a 2a41 7574 686f 7273  l data.**Authors
-00000090: 2a2a 3a20 5765 6e74 616f 205a 6861 6e20  **: Wentao Zhan 
-000000a0: 283c 777a 6861 6e33 406a 6875 2e65 6475  (<wzhan3@jhu.edu
-000000b0: 3e29 2c20 4162 6869 7275 7020 4461 7474  >), Abhirup Datt
-000000c0: 6120 283c 6162 6869 6461 7474 6140 6a68  a (<abhidatta@jh
-000000d0: 752e 6564 753e 290a 2323 2041 2070 6163  u.edu>).## A pac
-000000e0: 6b61 6765 2062 6173 6564 206f 6e20 7468  kage based on th
-000000f0: 6520 7061 7065 723a 205b 4e65 7572 616c  e paper: [Neural
-00000100: 206e 6574 776f 726b 7320 666f 7220 6765   networks for ge
-00000110: 6f73 7061 7469 616c 2064 6174 615d 2868  ospatial data](h
-00000120: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-00000130: 2f70 6466 2f32 3330 342e 3039 3135 372e  /pdf/2304.09157.
-00000140: 7064 6629 0a2a 2a47 656f 7370 614e 4e2a  pdf).**GeospaNN*
-00000150: 2a20 6973 2061 2066 6f72 6d61 6c20 696d  * is a formal im
-00000160: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
-00000170: 7468 6520 4e65 7572 616c 204e 6574 776f  the Neural Netwo
-00000180: 726b 7320 666f 7220 6765 6f73 7061 7469  rks for geospati
-00000190: 616c 2064 6174 6120 7072 6f70 6f73 6564  al data proposed
-000001a0: 2069 6e20 5a68 616e 2065 742e 616c 2028   in Zhan et.al (
-000001b0: 3230 3233 292e 200a 5468 6520 7061 636b  2023). .The pack
-000001c0: 6167 6520 6973 2064 6576 656c 6f70 6564  age is developed
-000001d0: 2075 7369 6e67 205b 5079 546f 7263 685d   using [PyTorch]
-000001e0: 2868 7474 7073 3a2f 2f70 7974 6f72 6368  (https://pytorch
-000001f0: 2e6f 7267 2f29 2061 6e64 2075 6e64 6572  .org/) and under
-00000200: 2074 6865 2066 7261 6d65 776f 726b 206f   the framework o
-00000210: 6620 5b50 7947 5d28 6874 7470 733a 2f2f  f [PyG](https://
-00000220: 7079 746f 7263 682d 6765 6f6d 6574 7269  pytorch-geometri
-00000230: 632e 7265 6164 7468 6564 6f63 732e 696f  c.readthedocs.io
-00000240: 2f65 6e2f 6c61 7465 7374 2f29 206c 6962  /en/latest/) lib
-00000250: 7261 7279 2e20 0a43 6f6d 6269 6e69 6e67  rary. .Combining
-00000260: 2074 6865 2069 6465 6120 6f66 2047 7261   the idea of Gra
-00000270: 7068 204e 6575 7261 6c20 4e65 7477 6f72  ph Neural Networ
-00000280: 6b73 2028 474e 4e29 2061 6e64 2073 7061  ks (GNN) and spa
-00000290: 7469 616c 2070 7265 6469 6374 696f 6e2c  tial prediction,
-000002a0: 200a 2a2a 6765 6f73 7061 4e4e 2a2a 2073   .**geospaNN** s
-000002b0: 696d 756c 7461 6e65 6f75 736c 7920 7072  imultaneously pr
-000002c0: 6f76 6964 6573 2065 6666 6963 6965 6e74  ovides efficient
-000002d0: 2065 7374 696d 6174 696f 6e20 666f 7220   estimation for 
-000002e0: 7468 6520 6e6f 6e2d 7370 6174 6961 6c20  the non-spatial 
-000002f0: 6566 6665 6374 2061 6e64 2070 7265 6469  effect and predi
-00000300: 6374 696f 6e20 666f 7220 7468 6520 7370  ction for the sp
-00000310: 6174 6961 6c20 6566 6665 6374 2c20 0a61  atial effect, .a
-00000320: 6e64 2063 616e 2073 6163 6c65 2075 7020  nd can sacle up 
-00000330: 746f 2068 756e 6472 6564 7320 6f66 2074  to hundreds of t
-00000340: 686f 7573 616e 6473 206f 6620 7361 6d70  housands of samp
-00000350: 6c65 732e 200a 5573 6572 7320 6172 6520  les. .Users are 
-00000360: 7765 6c63 6f6d 6520 746f 2070 726f 7669  welcome to provi
-00000370: 6465 2061 6e79 2068 656c 7066 756c 2073  de any helpful s
-00000380: 7567 6765 7374 696f 6e73 2061 6e64 2063  uggestions and c
-00000390: 6f6d 6d65 6e74 732e 0a0a 2323 204f 7665  omments...## Ove
-000003a0: 7276 6965 770a 5468 6520 5079 7468 6f6e  rview.The Python
-000003b0: 2070 6163 6b61 6765 202a 2a67 656f 7370   package **geosp
-000003c0: 614e 4e2a 2a27 2073 7461 6e64 7320 666f  aNN**' stands fo
-000003d0: 7220 6120 2767 656f 7370 6174 6961 6c20  r a 'geospatial 
-000003e0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-000003f0: 6620 4e65 7572 616c 204e 6574 776f 726b  f Neural Network
-00000400: 7327 2c20 7768 6572 6520 7765 2069 6d70  s', where we imp
-00000410: 656c 656d 656e 7473 2074 6865 200a 4e65  elements the .Ne
-00000420: 7572 616c 204e 6574 776f 726b 7320 666f  ural Networks fo
-00000430: 7220 616e 616c 7973 6973 206f 6620 6765  r analysis of ge
-00000440: 6f73 7061 7469 616c 2064 6174 6120 7468  ospatial data th
-00000450: 6174 2065 7870 6c69 6369 746c 7920 6163  at explicitly ac
-00000460: 636f 756e 7473 2066 6f72 2073 7061 7469  counts for spati
-00000470: 616c 2064 6570 656e 6465 6e63 6520 284e  al dependence (N
-00000480: 4e2d 474c 5329 2070 726f 706f 7365 6420  N-GLS) proposed 
-00000490: 696e 205a 6861 6e20 6574 2e61 6c20 2832  in Zhan et.al (2
-000004a0: 3032 3329 2e20 0a54 7261 6469 7469 6f6e  023). .Tradition
-000004b0: 616c 6c79 2c20 7468 6520 616e 616c 7973  ally, the analys
-000004c0: 6973 206f 6620 6765 6f73 7061 7469 616c  is of geospatial
-000004d0: 2064 6174 6120 7472 6561 7473 2074 6865   data treats the
-000004e0: 2073 7061 7469 616c 206f 7574 636f 6d65   spatial outcome
-000004f0: 2024 7928 7329 2420 6173 2061 2063 6f6d   $y(s)$ as a com
-00000500: 6269 6e61 7469 6f6e 206f 6620 7468 6520  bination of the 
-00000510: 6669 7865 6420 6566 6665 6374 200a 286c  fixed effect .(l
-00000520: 696e 6561 7220 6f72 206e 6f6e 2d6c 696e  inear or non-lin
-00000530: 6561 7229 206f 6620 636f 7661 7269 6174  ear) of covariat
-00000540: 6573 2024 7828 7329 2420 616e 6420 7468  es $x(s)$ and th
-00000550: 6520 7370 6174 6961 6c6c 7920 636f 7272  e spatially corr
-00000560: 656c 6174 6564 2072 616e 646f 6d20 6566  elated random ef
-00000570: 6665 6374 2024 7728 7329 242e 200a 5468  fect $w(s)$. .Th
-00000580: 6520 636c 6173 7369 6361 6c20 4e65 7572  e classical Neur
-00000590: 616c 204e 6574 776f 726b 7320 284e 4e29  al Networks (NN)
-000005a0: 2c20 6173 206f 6e65 206f 6620 7468 6520  , as one of the 
-000005b0: 6d6f 7374 2070 6f70 756c 6172 206d 6163  most popular mac
-000005c0: 6869 6e65 206c 6561 726e 696e 6720 6170  hine learning ap
-000005d0: 7072 6f61 6368 6573 2c0a 636f 756c 6420  proaches,.could 
-000005e0: 6265 2075 7365 6420 746f 2063 6170 7475  be used to captu
-000005f0: 7265 2074 6865 206e 6f6e 2d6c 696e 6561  re the non-linea
-00000600: 7220 6669 7865 6420 6566 6665 6374 2e20  r fixed effect. 
-00000610: 0a48 6f77 6576 6572 2c20 7768 696c 6520  .However, while 
-00000620: 4e4e 2061 7373 756d 6520 7468 6520 696e  NN assume the in
-00000630: 6465 7065 6e64 656e 6365 2061 6d6f 6e67  dependence among
-00000640: 206f 6273 6572 7661 7469 6f6e 732c 2067   observations, g
-00000650: 656f 7370 6174 6961 6c20 6461 7461 206e  eospatial data n
-00000660: 6174 7572 616c 6c79 2069 6e68 6572 6974  aturally inherit
-00000670: 7320 7370 6174 6961 6c20 6465 7065 6e64  s spatial depend
-00000680: 656e 6379 2c20 0a77 6869 6368 2069 7320  ency, .which is 
-00000690: 696e 7465 7270 7265 7465 6420 6279 2054  interpreted by T
-000006a0: 6f62 6c65 7227 7320 6669 7273 7420 6c61  obler's first la
-000006b0: 7720 6f66 2067 656f 6772 6170 6879 3a20  w of geography: 
-000006c0: 0a65 7665 7279 7468 696e 6720 6973 2072  .everything is r
-000006d0: 656c 6174 6564 2074 6f20 6576 6572 7974  elated to everyt
-000006e0: 6869 6e67 2065 6c73 652c 2062 7574 206e  hing else, but n
-000006f0: 6561 7262 7920 7468 696e 6773 2061 7265  earby things are
-00000700: 206d 6f72 6520 7265 6c61 7465 6420 7468   more related th
-00000710: 616e 2064 6973 7461 6e74 2074 6869 6e67  an distant thing
-00000720: 732e 200a 4f6e 2074 6865 206f 7468 6572  s. .On the other
-00000730: 2068 616e 642c 2074 7261 6469 7469 6f6e   hand, tradition
-00000740: 616c 2067 656f 7370 6174 6961 6c20 6461  al geospatial da
-00000750: 7461 2072 656c 6965 7320 6f6e 2074 6865  ta relies on the
-00000760: 206d 6f64 656c 2d62 6173 6564 2061 7070   model-based app
-00000770: 726f 6163 6865 7320 746f 2068 616e 646c  roaches to handl
-00000780: 6520 7468 6520 7370 6174 6961 6c20 6465  e the spatial de
-00000790: 7065 6e64 656e 6379 2e20 0a46 6f72 2065  pendency. .For e
-000007a0: 7861 6d70 6c65 2c20 6279 2061 7373 756d  xample, by assum
-000007b0: 696e 6720 2477 2873 2924 2062 6569 6e67  ing $w(s)$ being
-000007c0: 2061 2073 7461 7469 6f6e 6172 7920 4761   a stationary Ga
-000007d0: 7573 7369 616e 2070 726f 6365 7373 2028  ussian process (
-000007e0: 4750 292c 2073 696d 706c 6520 7465 6368  GP), simple tech
-000007f0: 6e69 7175 6573 206c 696b 6520 6b72 6967  niques like krig
-00000800: 696e 6720 6361 6e20 7072 6f76 6964 6520  ing can provide 
-00000810: 0a70 6f77 6572 6675 6c20 7072 6564 6963  .powerful predic
-00000820: 7469 6f6e 2070 6572 666f 726d 616e 6365  tion performance
-00000830: 2062 7920 7072 6f70 6572 6c79 2061 6767   by properly agg
-00000840: 7265 6761 7469 6e67 2074 6865 206e 6569  regating the nei
-00000850: 6768 626f 7269 6e67 2069 6e66 6f72 6d61  ghboring informa
-00000860: 7469 6f6e 2e0a 4f75 7220 7061 636b 6167  tion..Our packag
-00000870: 6520 2a2a 6765 6f73 7061 4e4e 2a2a 2074  e **geospaNN** t
-00000880: 616b 6573 2074 6865 2061 6476 616e 7461  akes the advanta
-00000890: 6765 7320 6672 6f6d 2062 6f74 6820 7065  ges from both pe
-000008a0: 7273 7065 6374 6976 6520 616e 6420 7072  rspective and pr
-000008b0: 6f76 6964 6573 2061 6e20 6566 6669 6369  ovides an effici
-000008c0: 656e 7420 746f 6f6c 2066 6f72 2067 656f  ent tool for geo
-000008d0: 7370 6174 6961 6c20 6461 7461 2061 6e61  spatial data ana
-000008e0: 6c79 7369 732e 0a49 6e20 7468 6520 7061  lysis..In the pa
-000008f0: 636b 6167 652c 2047 5020 6973 2069 6e76  ckage, GP is inv
-00000900: 6f6c 7665 6420 6173 2061 2074 7261 696e  olved as a train
-00000910: 6162 6c65 2074 6172 6765 7420 696e 746f  able target into
-00000920: 2074 6865 204e 6575 7261 6c20 4e65 7477   the Neural Netw
-00000930: 6f72 6b20 616e 6420 7573 6564 2074 6f20  ork and used to 
-00000940: 6775 6964 6520 7468 6520 6e65 6967 6862  guide the neighb
-00000950: 6f72 686f 6f64 2061 6767 7265 6761 7469  orhood aggregati
-00000960: 6f6e 206f 6e0a 7468 6520 6f75 7470 7574  on on.the output
-00000970: 206c 6179 6572 2e20 4571 7569 7661 6c65   layer. Equivale
-00000980: 6e74 6c79 2c20 6120 6d6f 7265 2065 6666  ntly, a more eff
-00000990: 6963 6965 6e74 206c 6f73 7320 6675 6e63  icient loss func
-000009a0: 7469 6f6e 2069 7320 636f 6d70 6f73 6564  tion is composed
-000009b0: 2066 6f72 2074 6865 2067 656f 7370 6174   for the geospat
-000009c0: 6961 6c20 7365 7474 696e 6720 746f 2069  ial setting to i
-000009d0: 6d70 726f 7665 2074 6865 200a 6573 7469  mprove the .esti
-000009e0: 6d61 7469 6f6e 2c20 616e 6420 7468 6520  mation, and the 
-000009f0: 6964 6561 206d 696d 6963 7320 7468 6520  idea mimics the 
-00000a00: 636f 6d70 6172 6973 6f6e 2062 6574 7765  comparison betwe
-00000a10: 656e 204f 4c53 2061 6e64 2047 4c53 2069  en OLS and GLS i
-00000a20: 6e20 6c69 6e65 6172 2072 6567 7265 7373  n linear regress
-00000a30: 696f 6e2e 0a41 7320 6120 646f 776e 7374  ion..As a downst
-00000a40: 7265 616d 206f 6620 6573 7469 6d61 7469  ream of estimati
-00000a50: 6e67 2024 6628 7829 242c 202a 2a67 656f  ng $f(x)$, **geo
-00000a60: 7370 614e 4e2a 2a20 7072 6f76 6964 6573  spaNN** provides
-00000a70: 2061 6363 7572 6174 6520 7370 6174 6961   accurate spatia
-00000a80: 6c20 7072 6564 6963 7469 6f6e 2c20 7468  l prediction, th
-00000a90: 7573 2063 6f6e 636c 7564 6573 2061 2063  us concludes a c
-00000aa0: 6f6d 706c 6574 6520 6765 6f73 7061 7469  omplete geospati
-00000ab0: 616c 2061 6e61 6c79 7369 7320 7069 7065  al analysis pipe
-00000ac0: 6c69 6e65 2e0a 4974 2073 686f 756c 6420  line..It should 
-00000ad0: 6265 2068 6967 686c 6967 6874 6564 2074  be highlighted t
-00000ae0: 6861 7420 2a2a 6765 6f73 7061 4e4e 2a2a  hat **geospaNN**
-00000af0: 2720 6973 2063 6f6d 7061 7469 626c 6520  ' is compatible 
-00000b00: 7769 7468 2074 6865 2066 7261 6d65 776f  with the framewo
-00000b10: 726b 206f 6620 4772 6170 6820 4e65 7572  rk of Graph Neur
-00000b20: 616c 204e 6574 776f 726b 7320 2847 4e4e  al Networks (GNN
-00000b30: 292c 2074 6875 7320 6265 696e 6720 6869  ), thus being hi
-00000b40: 6768 6c79 2067 656e 6572 616c 697a 6162  ghly generalizab
-00000b50: 6c65 2e0a 2854 6865 2069 6d70 6c65 6d65  le..(The impleme
-00000b60: 6e74 6174 696f 6e20 6f66 202a 2a67 656f  ntation of **geo
-00000b70: 7370 614e 4e2a 2a27 2075 7365 7320 7468  spaNN**' uses th
-00000b80: 6520 2774 6f72 6368 5f67 656f 6d27 206d  e 'torch_geom' m
-00000b90: 6f64 756c 652e 290a 546f 2061 6363 656c  odule.).To accel
-00000ba0: 6572 6174 6520 7468 6520 7472 6169 6e69  erate the traini
-00000bb0: 6e67 2070 726f 6365 7373 2066 6f72 2074  ng process for t
-00000bc0: 6865 2047 502c 200a 2a2a 6765 6f73 7061  he GP, .**geospa
-00000bd0: 4e4e 2a2a 2720 6170 7072 6f78 696d 6174  NN**' approximat
-00000be0: 6520 7468 6520 776f 726b 696e 6720 636f  e the working co
-00000bf0: 7272 656c 6174 696f 6e20 7374 7275 6374  rrelation struct
-00000c00: 7572 6520 7573 696e 6720 4e65 6172 6573  ure using Neares
-00000c10: 7420 4e65 6967 6862 6f72 2047 6175 7373  t Neighbor Gauss
-00000c20: 6961 6e20 5072 6f63 6573 7320 284e 4e47  ian Process (NNG
-00000c30: 5029 2028 4461 7474 6120 6574 2061 6c2e  P) (Datta et al.
-00000c40: 2c20 3230 3136 2920 0a77 6869 6368 206d  , 2016) .which m
-00000c50: 616b 6573 2069 7420 7375 6974 6162 6c65  akes it suitable
-00000c60: 2066 6f72 206c 6172 6765 7220 6461 7461   for larger data
-00000c70: 7365 7473 2074 6f77 6172 6473 2061 2073  sets towards a s
-00000c80: 697a 6520 6f66 2031 206d 696c 6c69 6f6e  ize of 1 million
-00000c90: 2e0a 0a21 5b49 6c6c 7573 7472 6174 696f  ...![Illustratio
-00000ca0: 6e20 6f66 204e 4e2d 474c 535d 282e 2f64  n of NN-GLS](./d
-00000cb0: 6174 612f 6e6e 676c 732e 706e 6729 0a0a  ata/nngls.png)..
-00000cc0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000cd0: 0a28 4375 7272 656e 746c 7929 2074 6f20  .(Currently) to 
-00000ce0: 696e 7374 616c 6c20 7468 6520 6465 7665  install the deve
-00000cf0: 6c6f 706d 656e 7420 7665 7273 696f 6e20  lopment version 
-00000d00: 6f66 2074 6865 2070 6163 6b61 6765 2c20  of the package, 
-00000d10: 6120 7072 652d 696e 7374 616c 6c65 6420  a pre-installed 
-00000d20: 5079 546f 7263 6820 616e 6420 5079 4720  PyTorch and PyG 
-00000d30: 6c69 6272 6172 6965 7320 6172 6520 6e65  libraries are ne
-00000d40: 6564 6564 2e20 496e 7374 616c 6c61 7469  eded. Installati
-00000d50: 6f6e 2069 6e20 7468 6520 666f 6c6c 6f77  on in the follow
-00000d60: 696e 6720 6f72 6465 7220 6973 2072 6563  ing order is rec
-00000d70: 6f6d 6d65 6e64 6564 2074 6f20 6176 6f69  ommended to avoi
-00000d80: 6420 616e 7920 636f 6d70 696c 6174 696f  d any compilatio
-00000d90: 6e20 6973 7375 652e 0a31 2e20 546f 2069  n issue..1. To i
-00000da0: 6e73 7461 6c6c 2050 7954 6f72 6368 2c20  nstall PyTorch, 
-00000db0: 6669 6e64 2061 6e64 2069 6e73 7461 6c6c  find and install
-00000dc0: 2074 6865 2062 696e 6172 7920 7375 6974   the binary suit
-00000dd0: 6162 6c65 2066 6f72 2079 6f75 7220 6d61  able for your ma
-00000de0: 6368 696e 6520 5b68 6572 655d 2868 7474  chine [here](htt
-00000df0: 7073 3a2f 2f70 7974 6f72 6368 2e6f 7267  ps://pytorch.org
-00000e00: 2f29 2e0a 322e 2054 6865 6e20 746f 2069  /)..2. Then to i
-00000e10: 6e73 7461 6c6c 2074 6865 2050 7947 206c  nstall the PyG l
-00000e20: 6962 7261 7279 2c20 6669 6e64 2061 6e64  ibrary, find and
-00000e30: 2069 6e73 7461 6c6c 2074 6865 2070 726f   install the pro
-00000e40: 7065 7220 6269 6e61 7279 205b 6865 7265  per binary [here
-00000e50: 5d28 6874 7470 733a 2f2f 7079 746f 7263  ](https://pytorc
-00000e60: 682d 6765 6f6d 6574 7269 632e 7265 6164  h-geometric.read
-00000e70: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000e80: 7465 7374 2f6e 6f74 6573 2f69 6e73 7461  test/notes/insta
-00000e90: 6c6c 6174 696f 6e2e 6874 6d6c 292e 0a33  llation.html)..3
-00000ea0: 2e20 4d61 6b65 2073 7572 6520 746f 2061  . Make sure to a
-00000eb0: 6c73 6f20 696e 7374 616c 6c20 7468 6520  lso install the 
-00000ec0: 6465 7065 6e64 656e 6369 6573 2069 6e63  dependencies inc
-00000ed0: 6c75 6469 6e67 202a 7079 675f 6c69 622a  luding *pyg_lib*
-00000ee0: 2c20 2a74 6f72 6368 5f73 6361 7474 6572  , *torch_scatter
-00000ef0: 2a2c 202a 746f 7263 685f 7370 6172 7365  *, *torch_sparse
-00000f00: 2a2c 202a 746f 7263 685f 636c 7573 7465  *, *torch_cluste
-00000f10: 722a 2c20 616e 6420 2a74 6f72 6368 5f73  r*, and *torch_s
-00000f20: 706c 696e 655f 636f 6e76 2a2e 0a0a 4f6e  pline_conv*...On
-00000f30: 6365 2050 7954 6f72 6368 2061 6e64 2050  ce PyTorch and P
-00000f40: 7947 2061 7265 2073 7563 6365 7373 6675  yG are successfu
-00000f50: 6c6c 7920 696e 7374 616c 6c65 642c 2075  lly installed, u
-00000f60: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
-00000f70: 2063 6f6d 6d61 6e64 2069 6e20 7468 6520   command in the 
-00000f80: 7465 726d 696e 616c 3a0a 6060 6063 6f6d  terminal:.```com
-00000f90: 6d61 6e64 6c69 6e65 5c0a 7069 7020 696e  mandline\.pip in
-00000fa0: 7374 616c 6c20 6874 7470 733a 2f2f 6769  stall https://gi
-00000fb0: 7468 7562 2e63 6f6d 2f57 656e 7461 6f5a  thub.com/WentaoZ
-00000fc0: 6861 6e31 3939 382f 6765 6f73 7061 4e4e  han1998/geospaNN
-00000fd0: 2f61 7263 6869 7665 2f6d 6169 6e2e 7a69  /archive/main.zi
-00000fe0: 700a 6060 600a 0a54 6f20 696e 7374 616c  p.```..To instal
-00000ff0: 6c20 7468 6520 7079 7069 2076 6572 7369  l the pypi versi
-00001000: 6f6e 2c20 7573 6520 7468 6520 666f 6c6c  on, use the foll
-00001010: 6f77 696e 6720 636f 6d6d 616e 6420 696e  owing command in
-00001020: 2074 6865 2074 6572 6d69 6e61 6c3a 0a60   the terminal:.`
-00001030: 6060 636f 6d6d 616e 646c 696e 655c 0a70  ``commandline\.p
-00001040: 6970 2069 6e73 7461 6c6c 2067 656f 7370  ip install geosp
-00001050: 614e 4e0a 6060 600a 0a23 2320 416e 2065  aNN.```..## An e
-00001060: 6173 7920 7275 6e6e 696e 6720 7361 6d70  asy running samp
-00001070: 6c65 3a0a 0a46 6972 7374 2069 6d70 6f72  le:..First impor
-00001080: 7420 7468 6520 6d6f 6475 6c65 7320 616e  t the modules an
-00001090: 6420 7365 7420 7570 2074 6865 2070 6172  d set up the par
-000010a0: 616d 6574 6572 730a 312e 2044 6566 696e  ameters.1. Defin
-000010b0: 6520 7468 6520 4672 6965 646d 616e 2773  e the Friedman's
-000010c0: 2066 756e 6374 696f 6e2c 2061 6e64 2073   function, and s
-000010d0: 7065 6369 6679 2074 6865 2064 696d 656e  pecify the dimen
-000010e0: 7369 6f6e 206f 6620 696e 7075 7420 636f  sion of input co
-000010f0: 7661 7269 6174 6573 2e0a 322e 2053 6574  variates..2. Set
-00001100: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
-00001110: 666f 7220 7468 6520 7370 6174 6961 6c20  for the spatial 
-00001120: 7072 6f63 6573 732e 0a33 2e20 5365 7420  process..3. Set 
-00001130: 7468 6520 6879 7065 7270 6172 616d 6574  the hyperparamet
-00001140: 6572 7320 6f66 2074 6865 2064 6174 612e  ers of the data.
-00001150: 0a60 6060 636f 6d6d 616e 646c 696e 655c  .```commandline\
-00001160: 0a69 6d70 6f72 7420 746f 7263 680a 696d  .import torch.im
-00001170: 706f 7274 2067 656f 7370 614e 4e0a 696d  port geospaNN.im
-00001180: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-00001190: 0a0a 2320 312e 0a64 6566 2066 3528 5829  ..# 1..def f5(X)
-000011a0: 3a20 7265 7475 726e 2028 3130 2a6e 702e  : return (10*np.
-000011b0: 7369 6e28 6e70 2e70 692a 585b 3a2c 305d  sin(np.pi*X[:,0]
-000011c0: 2a58 5b3a 2c31 5d29 202b 2032 302a 2858  *X[:,1]) + 20*(X
-000011d0: 5b3a 2c32 5d2d 302e 3529 2a2a 3220 2b20  [:,2]-0.5)**2 + 
-000011e0: 3130 2a58 5b3a 2c33 5d20 2b35 2a58 5b3a  10*X[:,3] +5*X[:
-000011f0: 2c34 5d29 2f36 0a0a 7020 3d20 353b 2066  ,4])/6..p = 5; f
-00001200: 756e 5859 203d 2066 350a 0a23 2032 2e0a  unXY = f5..# 2..
-00001210: 7369 676d 6120 3d20 310a 7068 6920 3d20  sigma = 1.phi = 
-00001220: 332f 6e70 2e73 7172 7428 3229 0a74 6175  3/np.sqrt(2).tau
-00001230: 203d 2030 2e30 310a 7468 6574 6120 3d20   = 0.01.theta = 
-00001240: 746f 7263 682e 7465 6e73 6f72 285b 7369  torch.tensor([si
-00001250: 676d 612c 2070 6869 2c20 7461 755d 290a  gma, phi, tau]).
-00001260: 0a23 2033 2e0a 6e20 3d20 3130 3030 2020  .# 3..n = 1000  
-00001270: 2020 2020 2020 2020 2020 2320 5369 7a65            # Size
-00001280: 206f 6620 7468 6520 7369 6d75 6c61 7465   of the simulate
-00001290: 6420 7361 6d70 6c65 2e0a 6e6e 203d 2032  d sample..nn = 2
-000012a0: 3020 2020 2020 2020 2020 2020 2020 2320  0             # 
-000012b0: 4e65 6967 6862 6f72 2073 697a 6520 7573  Neighbor size us
-000012c0: 6564 2066 6f72 204e 4e47 502e 0a62 6174  ed for NNGP..bat
-000012d0: 6368 5f73 697a 6520 3d20 3530 2020 2020  ch_size = 50    
-000012e0: 2023 2042 6174 6368 2073 697a 6520 666f   # Batch size fo
-000012f0: 7220 7472 6169 6e69 6e67 2074 6865 206e  r training the n
-00001300: 6575 7261 6c20 6e65 7477 6f72 6b73 2e0a  eural networks..
-00001310: 6060 600a 0a4e 6578 742c 2073 696d 756c  ```..Next, simul
-00001320: 6174 6520 616e 6420 7370 6c69 7420 7468  ate and split th
-00001330: 6520 6461 7461 2e0a 312e 2053 696d 756c  e data..1. Simul
-00001340: 6174 6520 7468 6520 7370 6174 6961 6c6c  ate the spatiall
-00001350: 7920 636f 7272 656c 6174 6564 2064 6174  y correlated dat
-00001360: 6120 7769 7468 2073 7061 7469 616c 2063  a with spatial c
-00001370: 6f6f 7264 696e 6174 6573 2072 616e 646f  oordinates rando
-00001380: 6d6c 7920 7361 6d70 6c65 6420 6f6e 2061  mly sampled on a
-00001390: 205b 302c 2031 305d 5e32 2073 7175 6172   [0, 10]^2 squar
-000013a0: 6564 2064 6f6d 6169 6e2e 0a32 2e20 4275  ed domain..2. Bu
-000013b0: 696c 6420 7468 6520 6e65 6172 6573 7420  ild the nearest 
-000013c0: 6e65 6967 6862 6f72 2067 7261 7068 2c20  neighbor graph, 
-000013d0: 6173 2061 2074 6f72 6368 5f67 656f 6d65  as a torch_geome
-000013e0: 7472 6963 2e64 6174 612e 4461 7461 206f  tric.data.Data o
-000013f0: 626a 6563 742e 0a33 2e20 5370 6c69 7420  bject..3. Split 
-00001400: 6461 7461 2069 6e74 6f20 7472 6169 6e69  data into traini
-00001410: 6e67 2c20 7661 6c69 6461 7469 6f6e 2c20  ng, validation, 
-00001420: 7465 7374 696e 6720 7365 7473 2e0a 6060  testing sets..``
-00001430: 6063 6f6d 6d61 6e64 6c69 6e65 5c0a 2320  `commandline\.# 
-00001440: 312e 0a74 6f72 6368 2e6d 616e 7561 6c5f  1..torch.manual_
-00001450: 7365 6564 2832 3032 3429 0a58 2c20 592c  seed(2024).X, Y,
-00001460: 2063 6f6f 7264 2c20 636f 762c 2063 6f72   coord, cov, cor
-00001470: 6572 7220 3d20 6765 6f73 7061 4e4e 2e53  err = geospaNN.S
-00001480: 696d 756c 6174 696f 6e28 6e2c 2070 2c20  imulation(n, p, 
-00001490: 6e6e 2c20 6675 6e58 592c 2074 6865 7461  nn, funXY, theta
-000014a0: 2c20 7261 6e67 653d 5b30 2c20 3130 5d29  , range=[0, 10])
-000014b0: 0a0a 2320 322e 0a64 6174 6120 3d20 6765  ..# 2..data = ge
-000014c0: 6f73 7061 4e4e 2e6d 616b 655f 6772 6170  ospaNN.make_grap
-000014d0: 6828 582c 2059 2c20 636f 6f72 642c 206e  h(X, Y, coord, n
-000014e0: 6e29 0a0a 2320 332e 0a64 6174 615f 7472  n)..# 3..data_tr
-000014f0: 6169 6e2c 2064 6174 615f 7661 6c2c 2064  ain, data_val, d
-00001500: 6174 615f 7465 7374 203d 2067 656f 7370  ata_test = geosp
-00001510: 614e 4e2e 7370 6c69 745f 6461 7461 2858  aNN.split_data(X
-00001520: 2c20 592c 2063 6f6f 7264 2c20 6e65 6967  , Y, coord, neig
-00001530: 6862 6f72 5f73 697a 653d 3230 2c0a 2020  hbor_size=20,.  
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 2074 6573 745f 7072 6f70 6f72 7469 6f6e   test_proportion
-00001580: 3d30 2e32 290a 6060 6020 2020 200a 0a43  =0.2).```    ..C
-00001590: 6f6d 706f 7365 2074 6865 206d 6c70 2073  ompose the mlp s
-000015a0: 7472 7563 7475 7265 2061 6e64 2074 7261  tructure and tra
-000015b0: 696e 2065 6173 696c 792e 0a31 2e20 4465  in easily..1. De
-000015c0: 6669 6e65 2074 6865 206d 6c70 2073 7472  fine the mlp str
-000015d0: 7563 7475 7265 2028 746f 7263 682e 6e6e  ucture (torch.nn
-000015e0: 2920 746f 2075 7365 2e0a 322e 2044 6566  ) to use..2. Def
-000015f0: 696e 6520 7468 6520 4e4e 2d47 4c53 2063  ine the NN-GLS c
-00001600: 6f72 7265 7370 6f6e 6469 6e67 206d 6f64  orresponding mod
-00001610: 656c 2e0a 332e 2044 6566 696e 6520 7468  el..3. Define th
-00001620: 6520 4e4e 2d47 4c53 2074 7261 696e 696e  e NN-GLS trainin
-00001630: 6720 636c 6173 7320 7769 7468 206c 6561  g class with lea
-00001640: 726e 696e 6720 7261 7465 2061 6e64 2074  rning rate and t
-00001650: 6f6c 6572 616e 6365 2e0a 342e 2054 7261  olerance..4. Tra
-00001660: 696e 2074 6865 206d 6f64 656c 2e0a 6060  in the model..``
-00001670: 6063 6f6d 6d61 6e64 6c69 6e65 5c0a 2320  `commandline\.# 
-00001680: 312e 2020 2020 2020 2020 2020 2020 200a  1.             .
-00001690: 6d6c 7020 3d20 746f 7263 682e 6e6e 2e53  mlp = torch.nn.S
-000016a0: 6571 7565 6e74 6961 6c28 0a20 2020 2074  equential(.    t
-000016b0: 6f72 6368 2e6e 6e2e 4c69 6e65 6172 2870  orch.nn.Linear(p
-000016c0: 2c20 3530 292c 0a20 2020 2074 6f72 6368  , 50),.    torch
-000016d0: 2e6e 6e2e 5265 4c55 2829 2c0a 2020 2020  .nn.ReLU(),.    
-000016e0: 746f 7263 682e 6e6e 2e4c 696e 6561 7228  torch.nn.Linear(
-000016f0: 3530 2c20 3230 292c 0a20 2020 2074 6f72  50, 20),.    tor
-00001700: 6368 2e6e 6e2e 5265 4c55 2829 2c0a 2020  ch.nn.ReLU(),.  
-00001710: 2020 746f 7263 682e 6e6e 2e4c 696e 6561    torch.nn.Linea
-00001720: 7228 3230 2c20 3130 292c 0a20 2020 2074  r(20, 10),.    t
-00001730: 6f72 6368 2e6e 6e2e 5265 4c55 2829 2c0a  orch.nn.ReLU(),.
-00001740: 2020 2020 746f 7263 682e 6e6e 2e4c 696e      torch.nn.Lin
-00001750: 6561 7228 3130 2c20 3129 2c0a 290a 0a23  ear(10, 1),.)..#
-00001760: 2032 2e0a 6d6f 6465 6c20 3d20 6765 6f73   2..model = geos
-00001770: 7061 4e4e 2e6e 6e67 6c73 2870 3d70 2c20  paNN.nngls(p=p, 
-00001780: 6e65 6967 6862 6f72 5f73 697a 653d 6e6e  neighbor_size=nn
-00001790: 2c20 636f 6f72 645f 6469 6d65 6e73 696f  , coord_dimensio
-000017a0: 6e73 3d32 2c20 6d6c 703d 6d6c 702c 2074  ns=2, mlp=mlp, t
-000017b0: 6865 7461 3d74 6f72 6368 2e74 656e 736f  heta=torch.tenso
-000017c0: 7228 5b31 2e35 2c20 352c 2030 2e31 5d29  r([1.5, 5, 0.1])
-000017d0: 290a 0a23 2033 2e0a 6e6e 676c 735f 6d6f  )..# 3..nngls_mo
-000017e0: 6465 6c20 3d20 6765 6f73 7061 4e4e 2e6e  del = geospaNN.n
-000017f0: 6e67 6c73 5f74 7261 696e 286d 6f64 656c  ngls_train(model
-00001800: 2c20 6c72 203d 2020 302e 3031 2c20 6d69  , lr =  0.01, mi
-00001810: 6e5f 6465 6c74 6120 3d20 302e 3030 3129  n_delta = 0.001)
-00001820: 0a0a 2320 342e 0a74 7261 696e 696e 675f  ..# 4..training_
-00001830: 6c6f 6720 3d20 6e6e 676c 735f 6d6f 6465  log = nngls_mode
-00001840: 6c2e 7472 6169 6e28 6461 7461 5f74 7261  l.train(data_tra
-00001850: 696e 2c20 6461 7461 5f76 616c 2c20 6461  in, data_val, da
-00001860: 7461 5f74 6573 742c 0a20 2020 2020 2020  ta_test,.       
-00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001880: 2020 2020 2020 2020 2020 5570 6461 7465            Update
-00001890: 5f69 6e69 7420 3d20 3130 2c20 5570 6461  _init = 10, Upda
-000018a0: 7465 5f73 7465 7020 3d20 3130 290a 6060  te_step = 10).``
-000018b0: 600a 0a45 7374 696d 6174 696f 6e20 6672  `..Estimation fr
-000018c0: 6f6d 2074 6865 206d 6f64 656c 2e20 5468  om the model. Th
-000018d0: 6520 7661 7269 6162 6c65 2069 7320 6120  e variable is a 
-000018e0: 746f 7263 682e 5465 6e73 6f72 206f 626a  torch.Tensor obj
-000018f0: 6563 7420 6f66 2074 6865 2073 616d 6520  ect of the same 
-00001900: 6469 6d65 6e73 696f 6e0a 6060 6063 6f6d  dimension.```com
-00001910: 6d61 6e64 6c69 6e65 5c0a 7472 6169 6e5f  mandline\.train_
-00001920: 6573 7469 6d61 7465 203d 206d 6f64 656c  estimate = model
-00001930: 2e65 7374 696d 6174 6528 6461 7461 5f74  .estimate(data_t
-00001940: 7261 696e 2e78 290a 6060 600a 0a4b 7269  rain.x).```..Kri
-00001950: 6769 6e67 2070 7265 6469 6374 696f 6e20  ging prediction 
-00001960: 6672 6f6d 2074 6865 206d 6f64 656c 2e20  from the model. 
-00001970: 5468 6520 6669 7273 7420 7661 7269 6162  The first variab
-00001980: 6c65 2069 7320 7375 7070 6f73 6564 2074  le is supposed t
-00001990: 6f20 6265 2074 6865 2064 6174 6120 7573  o be the data us
-000019a0: 6564 2066 6f72 2074 7261 696e 696e 672c  ed for training,
-000019b0: 2061 6e64 2074 6865 2073 6563 6f6e 6420   and the second 
-000019c0: 0a76 6172 6961 626c 6520 6120 746f 7263  .variable a torc
-000019d0: 685f 6765 6f6d 6574 7269 632e 6461 7461  h_geometric.data
-000019e0: 2e44 6174 6120 6f62 6a65 6374 2077 6869  .Data object whi
-000019f0: 6368 2063 616e 2062 6520 636f 6d70 6f73  ch can be compos
-00001a00: 6564 2062 7920 6765 6f73 7061 4e4e 2e6d  ed by geospaNN.m
-00001a10: 616b 655f 6772 6170 6828 2927 2e0a 6060  ake_graph()'..``
-00001a20: 6063 6f6d 6d61 6e64 6c69 6e65 5c0a 7465  `commandline\.te
-00001a30: 7374 5f70 7265 6469 6374 203d 206d 6f64  st_predict = mod
-00001a40: 656c 2e70 7265 6469 6374 2864 6174 615f  el.predict(data_
-00001a50: 7472 6169 6e2c 2064 6174 615f 7465 7374  train, data_test
-00001a60: 290a 6060 600a 0a23 2320 5275 6e6e 696e  ).```..## Runnin
-00001a70: 6720 6578 616d 706c 6573 3a0a 2a20 4120  g examples:.* A 
-00001a80: 7369 6d75 6c61 7469 6f6e 2065 7870 6572  simulation exper
-00001a90: 696d 656e 7420 7769 7468 2061 2063 6f6d  iment with a com
-00001aa0: 6d6f 6e20 7370 6174 6961 6c20 7365 7474  mon spatial sett
-00001ab0: 696e 6720 6973 2073 686f 776e 205b 6865  ing is shown [he
-00001ac0: 7265 5d28 6874 7470 733a 2f2f 6769 7468  re](https://gith
-00001ad0: 7562 2e63 6f6d 2f57 656e 7461 6f5a 6861  ub.com/WentaoZha
-00001ae0: 6e31 3939 382f 6765 6f73 7061 4e4e 2f62  n1998/geospaNN/b
-00001af0: 6c6f 622f 6d61 696e 2f45 7861 6d70 6c65  lob/main/Example
-00001b00: 5f73 696d 756c 6174 696f 6e2e 6970 796e  _simulation.ipyn
-00001b10: 6229 2e0a 0a2a 2041 2072 6561 6c20 6461  b)...* A real da
-00001b20: 7461 2065 7870 6572 696d 656e 7420 6973  ta experiment is
-00001b30: 2073 686f 776e 205b 6865 7265 5d28 6874   shown [here](ht
-00001b40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001b50: 2f57 656e 7461 6f5a 6861 6e31 3939 382f  /WentaoZhan1998/
-00001b60: 6765 6f73 7061 4e4e 2f62 6c6f 622f 6d61  geospaNN/blob/ma
-00001b70: 696e 2f45 7861 6d70 6c65 5f72 6561 6c64  in/Example_reald
-00001b80: 6174 612e 6970 796e 6229 2e20 0a2a 2054  ata.ipynb). .* T
-00001b90: 6865 2050 4d32 2e35 2064 6174 6120 6973  he PM2.5 data is
-00001ba0: 2063 6f6c 6c65 6374 6564 2066 726f 6d20   collected from 
-00001bb0: 7468 6520 5b55 2e53 2e20 456e 7669 726f  the [U.S. Enviro
-00001bc0: 6e6d 656e 7461 6c20 5072 6f74 6563 7469  nmental Protecti
-00001bd0: 6f6e 2041 6765 6e63 795d 2868 7474 7073  on Agency](https
-00001be0: 3a2f 2f77 7777 2e65 7061 2e67 6f76 2f6f  ://www.epa.gov/o
-00001bf0: 7574 646f 6f72 2d61 6972 2d71 7561 6c69  utdoor-air-quali
-00001c00: 7479 2d64 6174 612f 646f 776e 6c6f 6164  ty-data/download
-00001c10: 2d64 6169 6c79 2d64 6174 6129 2064 6174  -daily-data) dat
-00001c20: 6173 6574 7320 666f 7220 6561 6368 2073  asets for each s
-00001c30: 7461 7465 2061 7265 2063 6f6c 6c65 6374  tate are collect
-00001c40: 6564 2061 6e64 2062 6f75 6e64 2074 6f67  ed and bound tog
-00001c50: 6574 6865 7220 746f 206f 6274 6169 6e20  ether to obtain 
-00001c60: 2770 6d32 355f 3230 3232 2e63 7376 272e  'pm25_2022.csv'.
-00001c70: 2064 6169 6c79 2050 4d32 2e35 2066 696c   daily PM2.5 fil
-00001c80: 6573 2061 7265 2073 7562 7365 7473 206f  es are subsets o
-00001c90: 6620 2770 6d32 355f 3230 3232 2e63 7376  f 'pm25_2022.csv
-00001ca0: 2720 7072 6f64 7563 6564 2062 7920 2772  ' produced by 'r
-00001cb0: 6561 6c64 6174 615f 7072 6570 726f 6365  ealdata_preproce
-00001cc0: 7373 2e70 7927 2e20 4f6e 6520 6361 6e20  ss.py'. One can 
-00001cd0: 736b 6970 2074 6865 2070 7265 7072 6f63  skip the preproc
-00001ce0: 6573 7369 6e67 2061 6e64 2075 7365 2074  essing and use t
-00001cf0: 6865 2064 6169 6c79 2066 696c 6573 2064  he daily files d
-00001d00: 6972 6563 746f 7279 2e20 0a2a 2054 6865  irectory. .* The
-00001d10: 206d 6574 656f 726f 6c6f 6769 6361 6c20   meteorological 
-00001d20: 6461 7461 2069 7320 636f 6c6c 6563 7465  data is collecte
-00001d30: 6420 6672 6f6d 2074 6865 205b 4e61 7469  d from the [Nati
-00001d40: 6f6e 616c 2043 656e 7465 7273 2066 6f72  onal Centers for
-00001d50: 2045 6e76 6972 6f6e 6d65 6e74 616c 2050   Environmental P
-00001d60: 7265 6469 6374 696f 6ee2 8099 7320 284e  rediction...s (N
-00001d70: 4345 5029 204e 6f72 7468 2041 6d65 7269  CEP) North Ameri
-00001d80: 6361 6e20 5265 6769 6f6e 616c 2052 6561  can Regional Rea
-00001d90: 6e61 6c79 7369 7320 284e 4152 5229 2070  nalysis (NARR) p
-00001da0: 726f 6475 6374 5d28 6874 7470 733a 2f2f  roduct](https://
-00001db0: 7073 6c2e 6e6f 6161 2e67 6f76 2f64 6174  psl.noaa.gov/dat
-00001dc0: 612f 6772 6964 6465 642f 6461 7461 2e6e  a/gridded/data.n
-00001dd0: 6172 722e 6874 6d6c 292e 2054 6865 2027  arr.html). The '
-00001de0: 2e6e 6327 2028 6e65 7443 4446 2920 6669  .nc' (netCDF) fi
-00001df0: 6c65 7320 7368 6f75 6c64 2062 6520 646f  les should be do
-00001e00: 776e 6c6f 6164 6564 2066 726f 6d20 7468  wnloaded from th
-00001e10: 6520 7765 6273 6974 6520 616e 6420 7361  e website and sa
-00001e20: 7665 6420 696e 2074 6865 2072 6f6f 7420  ved in the root 
-00001e30: 6469 7265 6374 6f72 7920 746f 2072 756e  directory to run
-00001e40: 2027 7265 616c 6461 7461 5f70 7265 7072   'realdata_prepr
-00001e50: 6f63 6573 732e 7079 272e 204f 7468 6572  ocess.py'. Other
-00001e60: 7769 7365 2c20 6f6e 6520 6d61 7920 736b  wise, one may sk
-00001e70: 6970 2074 6865 2070 7265 7072 6f63 6573  ip the preproces
-00001e80: 7369 6e67 2061 6e64 2075 7365 2063 6f76  sing and use cov
-00001e90: 6172 6961 7465 2066 696c 6573 2064 6972  ariate files dir
-00001ea0: 6563 746c 792e 200a 0a23 2320 4369 7461  ectly. ..## Cita
-00001eb0: 7469 6f6e 0a50 6c65 6173 6520 6369 7465  tion.Please cite
-00001ec0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
-00001ed0: 6170 6572 2077 6865 6e20 796f 7520 7573  aper when you us
-00001ee0: 6520 2a2a 6765 6f73 7061 4e4e 2a2a 3a0a  e **geospaNN**:.
-00001ef0: 0a3e 205a 6861 6e2c 2057 656e 7461 6f2c  .> Zhan, Wentao,
-00001f00: 2061 6e64 2041 6268 6972 7570 2044 6174   and Abhirup Dat
-00001f10: 7461 2e20 224e 6575 7261 6c20 6e65 7477  ta. "Neural netw
-00001f20: 6f72 6b73 2066 6f72 2067 656f 7370 6174  orks for geospat
-00001f30: 6961 6c20 6461 7461 2e22 2061 7258 6976  ial data." arXiv
-00001f40: 2070 7265 7072 696e 7420 6172 5869 763a   preprint arXiv:
-00001f50: 3233 3034 2e30 3931 3537 2028 3230 3233  2304.09157 (2023
-00001f60: 292e 0a0a 2323 2052 6566 6572 656e 6365  )...## Reference
-00001f70: 730a 0a44 6174 7461 2c20 4162 6869 7275  s..Datta, Abhiru
-00001f80: 702c 2053 7564 6970 746f 2042 616e 6572  p, Sudipto Baner
-00001f90: 6a65 652c 2041 6e64 7265 7720 4f2e 2046  jee, Andrew O. F
-00001fa0: 696e 6c65 792c 2061 6e64 2041 6c61 6e20  inley, and Alan 
-00001fb0: 452e 2047 656c 6661 6e64 2e20 2248 6965  E. Gelfand. "Hie
-00001fc0: 7261 7263 6869 6361 6c20 6e65 6172 6573  rarchical neares
-00001fd0: 742d 6e65 6967 6862 6f72 2047 6175 7373  t-neighbor Gauss
-00001fe0: 6961 6e20 7072 6f63 6573 7320 6d6f 6465  ian process mode
-00001ff0: 6c73 2066 6f72 206c 6172 6765 2067 656f  ls for large geo
-00002000: 7374 6174 6973 7469 6361 6c20 6461 7461  statistical data
-00002010: 7365 7473 2e22 204a 6f75 726e 616c 206f  sets." Journal o
-00002020: 6620 7468 6520 416d 6572 6963 616e 2053  f the American S
-00002030: 7461 7469 7374 6963 616c 2041 7373 6f63  tatistical Assoc
-00002040: 6961 7469 6f6e 2031 3131 2c20 6e6f 2e20  iation 111, no. 
-00002050: 3531 3420 2832 3031 3629 3a20 3830 302d  514 (2016): 800-
-00002060: 3831 322e 205b 6c69 6e6b 5d28 6874 7470  812. [link](http
-00002070: 733a 2f2f 7777 772e 7461 6e64 666f 6e6c  s://www.tandfonl
-00002080: 696e 652e 636f 6d2f 646f 692f 6675 6c6c  ine.com/doi/full
-00002090: 2f31 302e 3130 3830 2f30 3136 3231 3435  /10.1080/0162145
-000020a0: 392e 3230 3135 2e31 3034 3430 3931 290a  9.2015.1044091).
-000020b0: 0a5a 6861 6e2c 2057 656e 7461 6f2c 2061  .Zhan, Wentao, a
-000020c0: 6e64 2041 6268 6972 7570 2044 6174 7461  nd Abhirup Datta
-000020d0: 2e20 224e 6575 7261 6c20 6e65 7477 6f72  . "Neural networ
-000020e0: 6b73 2066 6f72 2067 656f 7370 6174 6961  ks for geospatia
-000020f0: 6c20 6461 7461 2e22 2061 7258 6976 2070  l data." arXiv p
-00002100: 7265 7072 696e 7420 6172 5869 763a 3233  reprint arXiv:23
-00002110: 3034 2e30 3931 3537 2028 3230 3233 292e  04.09157 (2023).
-00002120: 205b 6c69 6e6b 5d28 6874 7470 733a 2f2f   [link](https://
-00002130: 6172 7869 762e 6f72 672f 6162 732f 3233  arxiv.org/abs/23
-00002140: 3034 2e30 3931 3537 290a                 04.09157).
+00000020: 7079 7069 2f76 2f67 656f 7370 614e 4e3f  pypi/v/geospaNN?
+00000030: 6c6f 676f 3d50 7950 4929 5d28 6874 7470  logo=PyPI)](http
+00000040: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000050: 6a65 6374 2f67 656f 7370 614e 4e29 0a21  ject/geospaNN).!
+00000060: 5b50 7950 4920 2d20 5079 7468 6f6e 2056  [PyPI - Python V
+00000070: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
+00000080: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000090: 7970 692f 7079 7665 7273 696f 6e73 2f67  ypi/pyversions/g
+000000a0: 656f 7370 614e 4e29 0a0a 2320 4765 6f73  eospaNN)..# Geos
+000000b0: 7061 4e4e 202d 204e 6575 7261 6c20 6e65  paNN - Neural ne
+000000c0: 7477 6f72 6b73 2066 6f72 2067 656f 7370  tworks for geosp
+000000d0: 6174 6961 6c20 6461 7461 0a2a 2a41 7574  atial data.**Aut
+000000e0: 686f 7273 2a2a 3a20 5765 6e74 616f 205a  hors**: Wentao Z
+000000f0: 6861 6e20 283c 777a 6861 6e33 406a 6875  han (<wzhan3@jhu
+00000100: 2e65 6475 3e29 2c20 4162 6869 7275 7020  .edu>), Abhirup 
+00000110: 4461 7474 6120 283c 6162 6869 6461 7474  Datta (<abhidatt
+00000120: 6140 6a68 752e 6564 753e 290a 2323 2041  a@jhu.edu>).## A
+00000130: 2070 6163 6b61 6765 2062 6173 6564 206f   package based o
+00000140: 6e20 7468 6520 7061 7065 723a 205b 4e65  n the paper: [Ne
+00000150: 7572 616c 206e 6574 776f 726b 7320 666f  ural networks fo
+00000160: 7220 6765 6f73 7061 7469 616c 2064 6174  r geospatial dat
+00000170: 615d 2868 7474 7073 3a2f 2f61 7278 6976  a](https://arxiv
+00000180: 2e6f 7267 2f70 6466 2f32 3330 342e 3039  .org/pdf/2304.09
+00000190: 3135 372e 7064 6629 0a2a 2a47 656f 7370  157.pdf).**Geosp
+000001a0: 614e 4e2a 2a20 6973 2061 2066 6f72 6d61  aNN** is a forma
+000001b0: 6c20 696d 706c 656d 656e 7461 7469 6f6e  l implementation
+000001c0: 206f 6620 4e4e 2d47 4c53 2c20 7468 6520   of NN-GLS, the 
+000001d0: 4e65 7572 616c 204e 6574 776f 726b 7320  Neural Networks 
+000001e0: 666f 7220 6765 6f73 7061 7469 616c 2064  for geospatial d
+000001f0: 6174 6120 7072 6f70 6f73 6564 2069 6e20  ata proposed in 
+00000200: 5a68 616e 2065 742e 616c 2028 3230 3233  Zhan et.al (2023
+00000210: 292c 200a 7468 6174 2065 7870 6c69 6369  ), .that explici
+00000220: 746c 7920 6163 636f 756e 7473 2066 6f72  tly accounts for
+00000230: 2073 7061 7469 616c 2063 6f72 7265 6c61   spatial correla
+00000240: 7469 6f6e 2069 6e20 7468 6520 6461 7461  tion in the data
+00000250: 2e20 5468 6520 7061 636b 6167 6520 6973  . The package is
+00000260: 2064 6576 656c 6f70 6564 2075 7369 6e67   developed using
+00000270: 205b 5079 546f 7263 685d 2868 7474 7073   [PyTorch](https
+00000280: 3a2f 2f70 7974 6f72 6368 2e6f 7267 2f29  ://pytorch.org/)
+00000290: 2061 6e64 200a 756e 6465 7220 7468 6520   and .under the 
+000002a0: 6672 616d 6577 6f72 6b20 6f66 205b 5079  framework of [Py
+000002b0: 475d 2868 7474 7073 3a2f 2f70 7974 6f72  G](https://pytor
+000002c0: 6368 2d67 656f 6d65 7472 6963 2e72 6561  ch-geometric.rea
+000002d0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000002e0: 6174 6573 742f 2920 6c69 6272 6172 792e  atest/) library.
+000002f0: 200a 4e4e 2d47 4c53 2069 7320 6120 6765   .NN-GLS is a ge
+00000300: 6f67 7261 7068 6963 616c 6c79 2d69 6e66  ographically-inf
+00000310: 6f72 6d65 6420 4772 6170 6820 4e65 7572  ormed Graph Neur
+00000320: 616c 204e 6574 776f 726b 2028 474e 4e29  al Network (GNN)
+00000330: 2066 6f72 2061 6e61 6c79 7a69 6e67 206c   for analyzing l
+00000340: 6172 6765 2061 6e64 2069 7272 6567 756c  arge and irregul
+00000350: 6172 2067 656f 7370 6174 6961 6c20 6461  ar geospatial da
+00000360: 7461 2c20 0a74 6861 7420 636f 6d62 696e  ta, .that combin
+00000370: 6573 206d 756c 7469 2d6c 6179 6572 2070  es multi-layer p
+00000380: 6572 6365 7074 726f 6e73 2c20 4761 7573  erceptrons, Gaus
+00000390: 7369 616e 2070 726f 6365 7373 6573 2c20  sian processes, 
+000003a0: 616e 6420 6765 6e65 7261 6c69 7a65 6420  and generalized 
+000003b0: 6c65 6173 7420 7371 7561 7265 7320 2847  least squares (G
+000003c0: 4c53 2920 6c6f 7373 2e20 0a4e 4e2d 474c  LS) loss. .NN-GL
+000003d0: 5320 6f66 6665 7273 2062 6f74 6820 7265  S offers both re
+000003e0: 6772 6573 7369 6f6e 2066 756e 6374 696f  gression functio
+000003f0: 6e20 6573 7469 6d61 7469 6f6e 2061 6e64  n estimation and
+00000400: 2073 7061 7469 616c 2070 7265 6469 6374   spatial predict
+00000410: 696f 6e2c 2061 6e64 2063 616e 2073 6361  ion, and can sca
+00000420: 6c65 2075 7020 746f 2073 616d 706c 6520  le up to sample 
+00000430: 7369 7a65 7320 6f66 2068 756e 6472 6564  sizes of hundred
+00000440: 7320 6f66 2074 686f 7573 616e 6473 2e20  s of thousands. 
+00000450: 0a55 7365 7273 2061 7265 2077 656c 636f  .Users are welco
+00000460: 6d65 2074 6f20 7072 6f76 6964 6520 616e  me to provide an
+00000470: 7920 6865 6c70 6675 6c20 7375 6767 6573  y helpful sugges
+00000480: 7469 6f6e 7320 616e 6420 636f 6d6d 656e  tions and commen
+00000490: 7473 2e0a 0a23 2320 4f76 6572 7669 6577  ts...## Overview
+000004a0: 0a54 6865 2050 7974 686f 6e20 7061 636b  .The Python pack
+000004b0: 6167 6520 2a2a 6765 6f73 7061 4e4e 2a2a  age **geospaNN**
+000004c0: 2073 7461 6e64 7320 666f 7220 2767 656f   stands for 'geo
+000004d0: 7370 6174 6961 6c20 4e65 7572 616c 204e  spatial Neural N
+000004e0: 6574 776f 726b 7327 2c20 7768 6572 6520  etworks', where 
+000004f0: 7765 2069 6d70 6c65 6d65 6e74 204e 4e2d  we implement NN-
+00000500: 474c 532c 200a 6e65 7572 616c 206e 6574  GLS, .neural net
+00000510: 776f 726b 7320 7461 696c 6f72 6564 2066  works tailored f
+00000520: 6f72 2061 6e61 6c79 7369 7320 6f66 2067  or analysis of g
+00000530: 656f 7370 6174 6961 6c20 6461 7461 2074  eospatial data t
+00000540: 6861 7420 6578 706c 6963 6974 6c79 2061  hat explicitly a
+00000550: 6363 6f75 6e74 7320 666f 7220 7370 6174  ccounts for spat
+00000560: 6961 6c20 6465 7065 6e64 656e 6365 2028  ial dependence (
+00000570: 5a68 616e 2065 742e 616c 2c20 3230 3233  Zhan et.al, 2023
+00000580: 292e 200a 4765 6f73 7061 7469 616c 2064  ). .Geospatial d
+00000590: 6174 6120 6e61 7475 7261 6c6c 7920 6578  ata naturally ex
+000005a0: 6869 6269 7473 2073 7061 7469 616c 2063  hibits spatial c
+000005b0: 6f72 7265 6c61 7469 6f6e 206f 7220 6465  orrelation or de
+000005c0: 7065 6e64 656e 6365 2061 6e64 2074 7261  pendence and tra
+000005d0: 6469 7469 6f6e 616c 2067 656f 7374 6174  ditional geostat
+000005e0: 6973 7469 6361 6c20 616e 616c 7973 6973  istical analysis
+000005f0: 206f 6674 656e 2072 656c 6965 7320 6f6e   often relies on
+00000600: 200a 6d6f 6465 6c2d 6261 7365 6420 6170   .model-based ap
+00000610: 7072 6f61 6368 6573 2074 6f20 6861 6e64  proaches to hand
+00000620: 6c65 2074 6865 2073 7061 7469 616c 2064  le the spatial d
+00000630: 6570 656e 6465 6e63 792c 2074 7265 6174  ependency, treat
+00000640: 696e 6720 7468 6520 7370 6174 6961 6c20  ing the spatial 
+00000650: 6f75 7463 6f6d 6520 2479 2873 2924 2061  outcome $y(s)$ a
+00000660: 7320 6120 6c69 6e65 6172 2072 6567 7265  s a linear regre
+00000670: 7373 696f 6e20 6f6e 2063 6f76 6172 6961  ssion on covaria
+00000680: 7465 7320 2478 2873 2924 2061 6e64 200a  tes $x(s)$ and .
+00000690: 6d6f 6465 6c69 6e67 2064 6570 656e 6465  modeling depende
+000006a0: 6e63 7920 7468 726f 7567 6820 7468 6520  ncy through the 
+000006b0: 7370 6174 6961 6c6c 7920 636f 7272 656c  spatially correl
+000006c0: 6174 6564 2065 7272 6f72 732e 200a 466f  ated errors. .Fo
+000006d0: 7220 6578 616d 706c 652c 2075 7369 6e67  r example, using
+000006e0: 2047 6175 7373 6961 6e20 7072 6f63 6573   Gaussian proces
+000006f0: 7365 7320 2847 5029 2074 6f20 6d6f 6465  ses (GP) to mode
+00000700: 6c20 6465 7065 6e64 656e 7420 6572 726f  l dependent erro
+00000710: 7273 2c20 0a73 696d 706c 6520 7465 6368  rs, .simple tech
+00000720: 6e69 7175 6573 206c 696b 6520 6b72 6967  niques like krig
+00000730: 696e 6720 6361 6e20 7072 6f76 6964 6520  ing can provide 
+00000740: 706f 7765 7266 756c 2070 7265 6469 6374  powerful predict
+00000750: 696f 6e20 7065 7266 6f72 6d61 6e63 6520  ion performance 
+00000760: 6279 2070 726f 7065 726c 7920 6167 6772  by properly aggr
+00000770: 6567 6174 696e 6720 7468 6520 6e65 6967  egating the neig
+00000780: 6862 6f72 696e 6720 696e 666f 726d 6174  hboring informat
+00000790: 696f 6e2e 200a 4f6e 2074 6865 206f 7468  ion. .On the oth
+000007a0: 6572 2068 616e 642c 2061 7274 6966 6963  er hand, artific
+000007b0: 6961 6c20 4e65 7572 616c 204e 6574 776f  ial Neural Netwo
+000007c0: 726b 7320 284e 4e29 2c20 6f6e 6520 6f66  rks (NN), one of
+000007d0: 2074 6865 206d 6f73 7420 706f 7075 6c61   the most popula
+000007e0: 7220 6d61 6368 696e 6520 6c65 6172 6e69  r machine learni
+000007f0: 6e67 2061 7070 726f 6163 6865 732c 2063  ng approaches, c
+00000800: 6f75 6c64 2062 6520 7573 6564 2074 6f20  ould be used to 
+00000810: 6573 7469 6d61 7465 206e 6f6e 2d6c 696e  estimate non-lin
+00000820: 6561 7220 7265 6772 6573 7369 6f6e 2066  ear regression f
+00000830: 756e 6374 696f 6e73 2e20 0a48 6f77 6576  unctions. .Howev
+00000840: 6572 2c20 636f 6d6d 6f6e 206e 6575 7261  er, common neura
+00000850: 6c20 6e65 7477 6f72 6b73 206c 696b 6520  l networks like 
+00000860: 6d75 6c74 692d 6c61 7965 7220 7065 7263  multi-layer perc
+00000870: 6570 7472 6f6e 7320 284d 4c50 2920 646f  eptrons (MLP) do
+00000880: 6573 206e 6f74 2069 6e63 6f72 706f 7261  es not incorpora
+00000890: 7465 2063 6f72 7265 6c61 7469 6f6e 2061  te correlation a
+000008a0: 6d6f 6e67 2064 6174 6120 756e 6974 732e  mong data units.
+000008b0: 0a0a 4f75 7220 7061 636b 6167 6520 2a2a  ..Our package **
+000008c0: 6765 6f73 7061 4e4e 2a2a 2074 616b 6573  geospaNN** takes
+000008d0: 2074 6865 2061 6476 616e 7461 6765 7320   the advantages 
+000008e0: 6672 6f6d 2062 6f74 6820 7065 7273 7065  from both perspe
+000008f0: 6374 6976 6573 2061 6e64 2070 726f 7669  ctives and provi
+00000900: 6465 7320 616e 2065 6666 6963 6965 6e74  des an efficient
+00000910: 2074 6f6f 6c20 666f 7220 6765 6f73 7061   tool for geospa
+00000920: 7469 616c 2064 6174 6120 616e 616c 7973  tial data analys
+00000930: 6973 2e20 0a49 6e20 4e4e 2d47 4c53 2c20  is. .In NN-GLS, 
+00000940: 616e 204d 4c50 2069 7320 7573 6564 2074  an MLP is used t
+00000950: 6f20 6d6f 6465 6c20 7468 6520 6e6f 6e2d  o model the non-
+00000960: 6c69 6e65 6172 2072 6567 7265 7373 696f  linear regressio
+00000970: 6e20 6675 6e63 7469 6f6e 2077 6869 6c65  n function while
+00000980: 2061 2047 5020 6973 2075 7365 6420 746f   a GP is used to
+00000990: 206d 6f64 656c 2074 6865 2073 7061 7469   model the spati
+000009a0: 616c 2064 6570 656e 6465 6e63 652e 200a  al dependence. .
+000009b0: 5468 6520 7265 7375 6c74 696e 6720 6c6f  The resulting lo
+000009c0: 7373 2066 756e 6374 696f 6e20 7468 656e  ss function then
+000009d0: 2062 6563 6f6d 6573 2061 2067 656e 6572   becomes a gener
+000009e0: 616c 697a 6564 206c 6561 7374 2073 7175  alized least squ
+000009f0: 6172 6573 2028 474c 5329 206c 6f73 7320  ares (GLS) loss 
+00000a00: 696e 666f 726d 6564 2062 7920 7468 6520  informed by the 
+00000a10: 4750 2063 6f76 6172 6961 6e63 6520 6d61  GP covariance ma
+00000a20: 7472 6978 2c20 0a74 6865 7265 6279 2065  trix, .thereby e
+00000a30: 7870 6c69 6369 746c 7920 696e 636f 7270  xplicitly incorp
+00000a40: 6f72 6174 696e 6720 7370 6174 6961 6c20  orating spatial 
+00000a50: 636f 7272 656c 6174 696f 6e20 696e 746f  correlation into
+00000a60: 2074 6865 206e 6575 7261 6c20 6e65 7477   the neural netw
+00000a70: 6f72 6b20 6f70 7469 6d69 7a61 7469 6f6e  ork optimization
+00000a80: 2e20 0a54 6865 2069 6465 6120 6d69 6d69  . .The idea mimi
+00000a90: 6373 2074 6865 2065 7874 656e 7369 6f6e  cs the extension
+00000aa0: 206f 6620 6f72 6469 6e61 7279 206c 6561   of ordinary lea
+00000ab0: 7374 2073 7175 6172 6573 2028 4f4c 5329  st squares (OLS)
+00000ac0: 206c 6f73 7320 746f 2047 4c53 206c 6f73   loss to GLS los
+00000ad0: 7320 696e 206c 696e 6561 7220 7265 6772  s in linear regr
+00000ae0: 6573 7369 6f6e 2066 6f72 2064 6570 656e  ession for depen
+00000af0: 6465 6e74 2064 6174 612e 0a0a 5a68 616e  dent data...Zhan
+00000b00: 2061 6e64 2044 6174 7461 2c20 3230 3233   and Datta, 2023
+00000b10: 2073 686f 7773 2074 6861 7420 6e65 7572   shows that neur
+00000b20: 616c 206e 6574 776f 726b 7320 7769 7468  al networks with
+00000b30: 2047 4c53 206c 6f73 7320 6361 6e20 6265   GLS loss can be
+00000b40: 2072 6570 7265 7365 6e74 6564 2061 7320   represented as 
+00000b50: 6120 6772 6170 6820 6e65 7572 616c 206e  a graph neural n
+00000b60: 6574 776f 726b 2c20 0a77 6974 6820 7468  etwork, .with th
+00000b70: 6520 4750 2063 6f76 6172 6961 6e63 6573  e GP covariances
+00000b80: 2067 7569 6469 6e67 2074 6865 206e 6569   guiding the nei
+00000b90: 6768 626f 7268 6f6f 6420 6167 6772 6567  ghborhood aggreg
+00000ba0: 6174 696f 6e20 6f6e 2074 6865 206f 7574  ation on the out
+00000bb0: 7075 7420 6c61 7965 722e 200a 5468 7573  put layer. .Thus
+00000bc0: 204e 4e2d 474c 5320 6973 2069 6d70 6c65   NN-GLS is imple
+00000bd0: 6d65 6e74 6564 2069 6e20 2a2a 6765 6f73  mented in **geos
+00000be0: 7061 4e4e 2a2a 2077 6974 6820 7468 6520  paNN** with the 
+00000bf0: 6672 616d 6577 6f72 6b20 6f66 2047 7261  framework of Gra
+00000c00: 7068 204e 6575 7261 6c20 4e65 7477 6f72  ph Neural Networ
+00000c10: 6b73 2028 474e 4e29 2c20 616e 6420 6973  ks (GNN), and is
+00000c20: 2068 6967 686c 7920 6765 6e65 7261 6c69   highly generali
+00000c30: 7a61 626c 652e 200a 2854 6865 2069 6d70  zable. .(The imp
+00000c40: 6c65 6d65 6e74 6174 696f 6e20 6f66 2067  lementation of g
+00000c50: 656f 7370 614e 4e27 2075 7365 7320 7468  eospaNN' uses th
+00000c60: 6520 2774 6f72 6368 5f67 656f 6d27 206d  e 'torch_geom' m
+00000c70: 6f64 756c 652e 290a 0a2a 2a67 656f 7370  odule.)..**geosp
+00000c80: 614e 4e2a 2a20 7072 6f76 6964 6573 2061  aNN** provides a
+00000c90: 6e20 6573 7469 6d61 7465 206f 6620 7265  n estimate of re
+00000ca0: 6772 6573 7369 6f6e 2066 756e 6374 696f  gression functio
+00000cb0: 6e20 f09d 9193 28f0 9d91 a529 2061 7320  n ....(....) as 
+00000cc0: 7765 6c6c 2061 7320 6163 6375 7261 7465  well as accurate
+00000cd0: 2073 7061 7469 616c 2070 7265 6469 6374   spatial predict
+00000ce0: 696f 6e73 2075 7369 6e67 2047 6175 7373  ions using Gauss
+00000cf0: 6961 6e20 7072 6f63 6573 7320 286b 7269  ian process (kri
+00000d00: 6769 6e67 292c 200a 616e 6420 7468 7573  ging), .and thus
+00000d10: 2063 6f6e 7374 6974 7574 6573 2061 2063   constitutes a c
+00000d20: 6f6d 706c 6574 6520 6765 6f73 7061 7469  omplete geospati
+00000d30: 616c 2061 6e61 6c79 7369 7320 7069 7065  al analysis pipe
+00000d40: 6c69 6e65 2e20 0a54 6f20 6163 6365 6c65  line. .To accele
+00000d50: 7261 7465 2074 6865 2074 7261 696e 696e  rate the trainin
+00000d60: 6720 7072 6f63 6573 7320 666f 7220 7468  g process for th
+00000d70: 6520 4750 2c20 2a2a 6765 6f73 7061 4e4e  e GP, **geospaNN
+00000d80: 2a2a 2061 7070 726f 7869 6d61 7465 7320  ** approximates 
+00000d90: 7468 6520 776f 726b 696e 6720 636f 7272  the working corr
+00000da0: 656c 6174 696f 6e20 7374 7275 6374 7572  elation structur
+00000db0: 6520 7573 696e 6720 0a4e 6561 7265 7374  e using .Nearest
+00000dc0: 204e 6569 6768 626f 7220 4761 7573 7369   Neighbor Gaussi
+00000dd0: 616e 2050 726f 6365 7373 2028 4e4e 4750  an Process (NNGP
+00000de0: 2920 2844 6174 7461 2065 7420 616c 2e2c  ) (Datta et al.,
+00000df0: 2032 3031 3629 2077 6869 6368 206d 616b   2016) which mak
+00000e00: 6573 2069 7420 7375 6974 6162 6c65 2066  es it suitable f
+00000e10: 6f72 206c 6172 6765 7220 6461 7461 7365  or larger datase
+00000e20: 7473 2074 6f77 6172 6473 2061 2073 697a  ts towards a siz
+00000e30: 6520 6f66 2031 206d 696c 6c69 6f6e 2e0a  e of 1 million..
+00000e40: 0a3c 6469 7620 616c 6967 6e3d 2263 656e  .<div align="cen
+00000e50: 7465 7222 3e0a 3c61 2068 7265 663d 2268  ter">.<a href="h
+00000e60: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00000e70: 2f70 6466 2f32 3330 342e 3039 3135 372e  /pdf/2304.09157.
+00000e80: 7064 6622 3e0a 2020 3c69 6d67 0a20 2020  pdf">.  <img.   
+00000e90: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000ea0: 7468 7562 2e63 6f6d 2f57 656e 7461 6f5a  thub.com/WentaoZ
+00000eb0: 6861 6e31 3939 382f 6765 6f73 7061 4e4e  han1998/geospaNN
+00000ec0: 2f62 6c6f 622f 6d61 696e 2f64 6174 612f  /blob/main/data/
+00000ed0: 6e6e 676c 732e 706e 673f 7261 773d 5472  nngls.png?raw=Tr
+00000ee0: 7565 220a 2020 2020 7769 6474 683d 2238  ue".    width="8
+00000ef0: 3030 220a 2020 3e0a 3c2f 613e 0a3c 2f64  00".  >.</a>.</d
+00000f00: 6976 3e0a 0a23 2320 496e 7374 616c 6c61  iv>..## Installa
+00000f10: 7469 6f6e 0a28 4375 7272 656e 746c 7929  tion.(Currently)
+00000f20: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
+00000f30: 6465 7665 6c6f 706d 656e 7420 7665 7273  development vers
+00000f40: 696f 6e20 6f66 2074 6865 2070 6163 6b61  ion of the packa
+00000f50: 6765 2c20 6120 7072 652d 696e 7374 616c  ge, a pre-instal
+00000f60: 6c65 6420 5079 546f 7263 6820 616e 6420  led PyTorch and 
+00000f70: 5079 4720 6c69 6272 6172 6965 7320 6172  PyG libraries ar
+00000f80: 6520 6e65 6564 6564 2e20 496e 7374 616c  e needed. Instal
+00000f90: 6c61 7469 6f6e 2069 6e20 7468 6520 666f  lation in the fo
+00000fa0: 6c6c 6f77 696e 6720 6f72 6465 7220 6973  llowing order is
+00000fb0: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
+00000fc0: 6176 6f69 6420 616e 7920 636f 6d70 696c  avoid any compil
+00000fd0: 6174 696f 6e20 6973 7375 652e 0a31 2e20  ation issue..1. 
+00000fe0: 546f 2069 6e73 7461 6c6c 2050 7954 6f72  To install PyTor
+00000ff0: 6368 2c20 6669 6e64 2061 6e64 2069 6e73  ch, find and ins
+00001000: 7461 6c6c 2074 6865 2062 696e 6172 7920  tall the binary 
+00001010: 7375 6974 6162 6c65 2066 6f72 2079 6f75  suitable for you
+00001020: 7220 6d61 6368 696e 6520 5b68 6572 655d  r machine [here]
+00001030: 2868 7474 7073 3a2f 2f70 7974 6f72 6368  (https://pytorch
+00001040: 2e6f 7267 2f29 2e0a 322e 2054 6865 6e20  .org/)..2. Then 
+00001050: 746f 2069 6e73 7461 6c6c 2074 6865 2050  to install the P
+00001060: 7947 206c 6962 7261 7279 2c20 6669 6e64  yG library, find
+00001070: 2061 6e64 2069 6e73 7461 6c6c 2074 6865   and install the
+00001080: 2070 726f 7065 7220 6269 6e61 7279 205b   proper binary [
+00001090: 6865 7265 5d28 6874 7470 733a 2f2f 7079  here](https://py
+000010a0: 746f 7263 682d 6765 6f6d 6574 7269 632e  torch-geometric.
+000010b0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+000010c0: 6e2f 6c61 7465 7374 2f6e 6f74 6573 2f69  n/latest/notes/i
+000010d0: 6e73 7461 6c6c 6174 696f 6e2e 6874 6d6c  nstallation.html
+000010e0: 292e 0a33 2e20 4d61 6b65 2073 7572 6520  )..3. Make sure 
+000010f0: 746f 2061 6c73 6f20 696e 7374 616c 6c20  to also install 
+00001100: 7468 6520 6465 7065 6e64 656e 6369 6573  the dependencies
+00001110: 2069 6e63 6c75 6469 6e67 202a 7079 675f   including *pyg_
+00001120: 6c69 622a 2c20 2a74 6f72 6368 5f73 6361  lib*, *torch_sca
+00001130: 7474 6572 2a2c 202a 746f 7263 685f 7370  tter*, *torch_sp
+00001140: 6172 7365 2a2c 202a 746f 7263 685f 636c  arse*, *torch_cl
+00001150: 7573 7465 722a 2c20 616e 6420 2a74 6f72  uster*, and *tor
+00001160: 6368 5f73 706c 696e 655f 636f 6e76 2a2e  ch_spline_conv*.
+00001170: 0a0a 4f6e 6365 2050 7954 6f72 6368 2061  ..Once PyTorch a
+00001180: 6e64 2050 7947 2061 7265 2073 7563 6365  nd PyG are succe
+00001190: 7373 6675 6c6c 7920 696e 7374 616c 6c65  ssfully installe
+000011a0: 642c 2075 7365 2074 6865 2066 6f6c 6c6f  d, use the follo
+000011b0: 7769 6e67 2063 6f6d 6d61 6e64 2069 6e20  wing command in 
+000011c0: 7468 6520 7465 726d 696e 616c 2066 6f72  the terminal for
+000011d0: 2074 6865 206c 6174 6573 7420 7665 7273   the latest vers
+000011e0: 696f 6e3a 0a60 6060 636f 6d6d 616e 646c  ion:.```commandl
+000011f0: 696e 655c 0a70 6970 2069 6e73 7461 6c6c  ine\.pip install
+00001200: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00001210: 636f 6d2f 5765 6e74 616f 5a68 616e 3139  com/WentaoZhan19
+00001220: 3938 2f67 656f 7370 614e 4e2f 6172 6368  98/geospaNN/arch
+00001230: 6976 652f 6d61 696e 2e7a 6970 0a60 6060  ive/main.zip.```
+00001240: 0a0a 546f 2069 6e73 7461 6c6c 2074 6865  ..To install the
+00001250: 2070 7970 6920 7665 7273 696f 6e2c 2075   pypi version, u
+00001260: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00001270: 2063 6f6d 6d61 6e64 2069 6e20 7468 6520   command in the 
+00001280: 7465 726d 696e 616c 3a0a 6060 6063 6f6d  terminal:.```com
+00001290: 6d61 6e64 6c69 6e65 5c0a 7069 7020 696e  mandline\.pip in
+000012a0: 7374 616c 6c20 6765 6f73 7061 4e4e 0a60  stall geospaNN.`
+000012b0: 6060 0a0a 2323 2041 6e20 6561 7379 2072  ``..## An easy r
+000012c0: 756e 6e69 6e67 2073 616d 706c 653a 0a0a  unning sample:..
+000012d0: 4669 7273 7420 696d 706f 7274 2074 6865  First import the
+000012e0: 206d 6f64 756c 6573 2061 6e64 2073 6574   modules and set
+000012f0: 2075 7020 7468 6520 7061 7261 6d65 7465   up the paramete
+00001300: 7273 0a31 2e20 4465 6669 6e65 2074 6865  rs.1. Define the
+00001310: 2046 7269 6564 6d61 6e27 7320 6675 6e63   Friedman's func
+00001320: 7469 6f6e 2c20 616e 6420 7370 6563 6966  tion, and specif
+00001330: 7920 7468 6520 6469 6d65 6e73 696f 6e20  y the dimension 
+00001340: 6f66 2069 6e70 7574 2063 6f76 6172 6961  of input covaria
+00001350: 7465 732e 0a32 2e20 5365 7420 7468 6520  tes..2. Set the 
+00001360: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
+00001370: 6865 2073 7061 7469 616c 2070 726f 6365  he spatial proce
+00001380: 7373 2e0a 332e 2053 6574 2074 6865 2068  ss..3. Set the h
+00001390: 7970 6572 7061 7261 6d65 7465 7273 206f  yperparameters o
+000013a0: 6620 7468 6520 6461 7461 2e0a 6060 6063  f the data..```c
+000013b0: 6f6d 6d61 6e64 6c69 6e65 5c0a 696d 706f  ommandline\.impo
+000013c0: 7274 2074 6f72 6368 0a69 6d70 6f72 7420  rt torch.import 
+000013d0: 6765 6f73 7061 4e4e 0a69 6d70 6f72 7420  geospaNN.import 
+000013e0: 6e75 6d70 7920 6173 206e 700a 0a23 2031  numpy as np..# 1
+000013f0: 2e0a 6465 6620 6635 2858 293a 2072 6574  ..def f5(X): ret
+00001400: 7572 6e20 2831 302a 6e70 2e73 696e 286e  urn (10*np.sin(n
+00001410: 702e 7069 2a58 5b3a 2c30 5d2a 585b 3a2c  p.pi*X[:,0]*X[:,
+00001420: 315d 2920 2b20 3230 2a28 585b 3a2c 325d  1]) + 20*(X[:,2]
+00001430: 2d30 2e35 292a 2a32 202b 2031 302a 585b  -0.5)**2 + 10*X[
+00001440: 3a2c 335d 202b 352a 585b 3a2c 345d 292f  :,3] +5*X[:,4])/
+00001450: 360a 0a70 203d 2035 3b20 6675 6e58 5920  6..p = 5; funXY 
+00001460: 3d20 6635 0a0a 2320 322e 0a73 6967 6d61  = f5..# 2..sigma
+00001470: 203d 2031 0a70 6869 203d 2033 2f6e 702e   = 1.phi = 3/np.
+00001480: 7371 7274 2832 290a 7461 7520 3d20 302e  sqrt(2).tau = 0.
+00001490: 3031 0a74 6865 7461 203d 2074 6f72 6368  01.theta = torch
+000014a0: 2e74 656e 736f 7228 5b73 6967 6d61 2c20  .tensor([sigma, 
+000014b0: 7068 692c 2074 6175 5d29 0a0a 2320 332e  phi, tau])..# 3.
+000014c0: 0a6e 203d 2031 3030 3020 2020 2020 2020  .n = 1000       
+000014d0: 2020 2020 2023 2053 697a 6520 6f66 2074       # Size of t
+000014e0: 6865 2073 696d 756c 6174 6564 2073 616d  he simulated sam
+000014f0: 706c 652e 0a6e 6e20 3d20 3230 2020 2020  ple..nn = 20    
+00001500: 2020 2020 2020 2020 2023 204e 6569 6768           # Neigh
+00001510: 626f 7220 7369 7a65 2075 7365 6420 666f  bor size used fo
+00001520: 7220 4e4e 4750 2e0a 6261 7463 685f 7369  r NNGP..batch_si
+00001530: 7a65 203d 2035 3020 2020 2020 2320 4261  ze = 50     # Ba
+00001540: 7463 6820 7369 7a65 2066 6f72 2074 7261  tch size for tra
+00001550: 696e 696e 6720 7468 6520 6e65 7572 616c  ining the neural
+00001560: 206e 6574 776f 726b 732e 0a60 6060 0a0a   networks..```..
+00001570: 4e65 7874 2c20 7369 6d75 6c61 7465 2061  Next, simulate a
+00001580: 6e64 2073 706c 6974 2074 6865 2064 6174  nd split the dat
+00001590: 612e 0a31 2e20 5369 6d75 6c61 7465 2074  a..1. Simulate t
+000015a0: 6865 2073 7061 7469 616c 6c79 2063 6f72  he spatially cor
+000015b0: 7265 6c61 7465 6420 6461 7461 2077 6974  related data wit
+000015c0: 6820 7370 6174 6961 6c20 636f 6f72 6469  h spatial coordi
+000015d0: 6e61 7465 7320 7261 6e64 6f6d 6c79 2073  nates randomly s
+000015e0: 616d 706c 6564 206f 6e20 6120 5b30 2c20  ampled on a [0, 
+000015f0: 3130 5d5e 3220 7371 7561 7265 6420 646f  10]^2 squared do
+00001600: 6d61 696e 2e0a 322e 2042 7569 6c64 2074  main..2. Build t
+00001610: 6865 206e 6561 7265 7374 206e 6569 6768  he nearest neigh
+00001620: 626f 7220 6772 6170 682c 2061 7320 6120  bor graph, as a 
+00001630: 746f 7263 685f 6765 6f6d 6574 7269 632e  torch_geometric.
+00001640: 6461 7461 2e44 6174 6120 6f62 6a65 6374  data.Data object
+00001650: 2e0a 332e 2053 706c 6974 2064 6174 6120  ..3. Split data 
+00001660: 696e 746f 2074 7261 696e 696e 672c 2076  into training, v
+00001670: 616c 6964 6174 696f 6e2c 2074 6573 7469  alidation, testi
+00001680: 6e67 2073 6574 732e 0a60 6060 636f 6d6d  ng sets..```comm
+00001690: 616e 646c 696e 655c 0a23 2031 2e0a 746f  andline\.# 1..to
+000016a0: 7263 682e 6d61 6e75 616c 5f73 6565 6428  rch.manual_seed(
+000016b0: 3230 3234 290a 582c 2059 2c20 636f 6f72  2024).X, Y, coor
+000016c0: 642c 2063 6f76 2c20 636f 7265 7272 203d  d, cov, corerr =
+000016d0: 2067 656f 7370 614e 4e2e 5369 6d75 6c61   geospaNN.Simula
+000016e0: 7469 6f6e 286e 2c20 702c 206e 6e2c 2066  tion(n, p, nn, f
+000016f0: 756e 5859 2c20 7468 6574 612c 2072 616e  unXY, theta, ran
+00001700: 6765 3d5b 302c 2031 305d 290a 0a23 2032  ge=[0, 10])..# 2
+00001710: 2e0a 6461 7461 203d 2067 656f 7370 614e  ..data = geospaN
+00001720: 4e2e 6d61 6b65 5f67 7261 7068 2858 2c20  N.make_graph(X, 
+00001730: 592c 2063 6f6f 7264 2c20 6e6e 290a 0a23  Y, coord, nn)..#
+00001740: 2033 2e0a 6461 7461 5f74 7261 696e 2c20   3..data_train, 
+00001750: 6461 7461 5f76 616c 2c20 6461 7461 5f74  data_val, data_t
+00001760: 6573 7420 3d20 6765 6f73 7061 4e4e 2e73  est = geospaNN.s
+00001770: 706c 6974 5f64 6174 6128 582c 2059 2c20  plit_data(X, Y, 
+00001780: 636f 6f72 642c 206e 6569 6768 626f 725f  coord, neighbor_
+00001790: 7369 7a65 3d32 302c 0a20 2020 2020 2020  size=20,.       
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017c0: 2020 2020 2020 2020 2020 2020 7465 7374              test
+000017d0: 5f70 726f 706f 7274 696f 6e3d 302e 3229  _proportion=0.2)
+000017e0: 0a60 6060 2020 2020 0a0a 436f 6d70 6f73  .```    ..Compos
+000017f0: 6520 7468 6520 6d6c 7020 7374 7275 6374  e the mlp struct
+00001800: 7572 6520 616e 6420 7472 6169 6e20 6561  ure and train ea
+00001810: 7369 6c79 2e0a 312e 2044 6566 696e 6520  sily..1. Define 
+00001820: 7468 6520 6d6c 7020 7374 7275 6374 7572  the mlp structur
+00001830: 6520 2874 6f72 6368 2e6e 6e29 2074 6f20  e (torch.nn) to 
+00001840: 7573 652e 0a32 2e20 4465 6669 6e65 2074  use..2. Define t
+00001850: 6865 204e 4e2d 474c 5320 636f 7272 6573  he NN-GLS corres
+00001860: 706f 6e64 696e 6720 6d6f 6465 6c2e 0a33  ponding model..3
+00001870: 2e20 4465 6669 6e65 2074 6865 204e 4e2d  . Define the NN-
+00001880: 474c 5320 7472 6169 6e69 6e67 2063 6c61  GLS training cla
+00001890: 7373 2077 6974 6820 6c65 6172 6e69 6e67  ss with learning
+000018a0: 2072 6174 6520 616e 6420 746f 6c65 7261   rate and tolera
+000018b0: 6e63 652e 0a34 2e20 5472 6169 6e20 7468  nce..4. Train th
+000018c0: 6520 6d6f 6465 6c2e 0a60 6060 636f 6d6d  e model..```comm
+000018d0: 616e 646c 696e 655c 0a23 2031 2e20 2020  andline\.# 1.   
+000018e0: 2020 2020 2020 2020 2020 0a6d 6c70 203d            .mlp =
+000018f0: 2074 6f72 6368 2e6e 6e2e 5365 7175 656e   torch.nn.Sequen
+00001900: 7469 616c 280a 2020 2020 746f 7263 682e  tial(.    torch.
+00001910: 6e6e 2e4c 696e 6561 7228 702c 2035 3029  nn.Linear(p, 50)
+00001920: 2c0a 2020 2020 746f 7263 682e 6e6e 2e52  ,.    torch.nn.R
+00001930: 654c 5528 292c 0a20 2020 2074 6f72 6368  eLU(),.    torch
+00001940: 2e6e 6e2e 4c69 6e65 6172 2835 302c 2032  .nn.Linear(50, 2
+00001950: 3029 2c0a 2020 2020 746f 7263 682e 6e6e  0),.    torch.nn
+00001960: 2e52 654c 5528 292c 0a20 2020 2074 6f72  .ReLU(),.    tor
+00001970: 6368 2e6e 6e2e 4c69 6e65 6172 2832 302c  ch.nn.Linear(20,
+00001980: 2031 3029 2c0a 2020 2020 746f 7263 682e   10),.    torch.
+00001990: 6e6e 2e52 654c 5528 292c 0a20 2020 2074  nn.ReLU(),.    t
+000019a0: 6f72 6368 2e6e 6e2e 4c69 6e65 6172 2831  orch.nn.Linear(1
+000019b0: 302c 2031 292c 0a29 0a0a 2320 322e 0a6d  0, 1),.)..# 2..m
+000019c0: 6f64 656c 203d 2067 656f 7370 614e 4e2e  odel = geospaNN.
+000019d0: 6e6e 676c 7328 703d 702c 206e 6569 6768  nngls(p=p, neigh
+000019e0: 626f 725f 7369 7a65 3d6e 6e2c 2063 6f6f  bor_size=nn, coo
+000019f0: 7264 5f64 696d 656e 7369 6f6e 733d 322c  rd_dimensions=2,
+00001a00: 206d 6c70 3d6d 6c70 2c20 7468 6574 613d   mlp=mlp, theta=
+00001a10: 746f 7263 682e 7465 6e73 6f72 285b 312e  torch.tensor([1.
+00001a20: 352c 2035 2c20 302e 315d 2929 0a0a 2320  5, 5, 0.1]))..# 
+00001a30: 332e 0a6e 6e67 6c73 5f6d 6f64 656c 203d  3..nngls_model =
+00001a40: 2067 656f 7370 614e 4e2e 6e6e 676c 735f   geospaNN.nngls_
+00001a50: 7472 6169 6e28 6d6f 6465 6c2c 206c 7220  train(model, lr 
+00001a60: 3d20 2030 2e30 312c 206d 696e 5f64 656c  =  0.01, min_del
+00001a70: 7461 203d 2030 2e30 3031 290a 0a23 2034  ta = 0.001)..# 4
+00001a80: 2e0a 7472 6169 6e69 6e67 5f6c 6f67 203d  ..training_log =
+00001a90: 206e 6e67 6c73 5f6d 6f64 656c 2e74 7261   nngls_model.tra
+00001aa0: 696e 2864 6174 615f 7472 6169 6e2c 2064  in(data_train, d
+00001ab0: 6174 615f 7661 6c2c 2064 6174 615f 7465  ata_val, data_te
+00001ac0: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
+00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ae0: 2020 2020 2055 7064 6174 655f 696e 6974       Update_init
+00001af0: 203d 2031 302c 2055 7064 6174 655f 7374   = 10, Update_st
+00001b00: 6570 203d 2031 3029 0a60 6060 0a0a 4573  ep = 10).```..Es
+00001b10: 7469 6d61 7469 6f6e 2066 726f 6d20 7468  timation from th
+00001b20: 6520 6d6f 6465 6c2e 2054 6865 2076 6172  e model. The var
+00001b30: 6961 626c 6520 6973 2061 2074 6f72 6368  iable is a torch
+00001b40: 2e54 656e 736f 7220 6f62 6a65 6374 206f  .Tensor object o
+00001b50: 6620 7468 6520 7361 6d65 2064 696d 656e  f the same dimen
+00001b60: 7369 6f6e 0a60 6060 636f 6d6d 616e 646c  sion.```commandl
+00001b70: 696e 655c 0a74 7261 696e 5f65 7374 696d  ine\.train_estim
+00001b80: 6174 6520 3d20 6d6f 6465 6c2e 6573 7469  ate = model.esti
+00001b90: 6d61 7465 2864 6174 615f 7472 6169 6e2e  mate(data_train.
+00001ba0: 7829 0a60 6060 0a0a 4b72 6967 696e 6720  x).```..Kriging 
+00001bb0: 7072 6564 6963 7469 6f6e 2066 726f 6d20  prediction from 
+00001bc0: 7468 6520 6d6f 6465 6c2e 2054 6865 2066  the model. The f
+00001bd0: 6972 7374 2076 6172 6961 626c 6520 6973  irst variable is
+00001be0: 2073 7570 706f 7365 6420 746f 2062 6520   supposed to be 
+00001bf0: 7468 6520 6461 7461 2075 7365 6420 666f  the data used fo
+00001c00: 7220 7472 6169 6e69 6e67 2c20 616e 6420  r training, and 
+00001c10: 7468 6520 7365 636f 6e64 200a 7661 7269  the second .vari
+00001c20: 6162 6c65 2061 2074 6f72 6368 5f67 656f  able a torch_geo
+00001c30: 6d65 7472 6963 2e64 6174 612e 4461 7461  metric.data.Data
+00001c40: 206f 626a 6563 7420 7768 6963 6820 6361   object which ca
+00001c50: 6e20 6265 2063 6f6d 706f 7365 6420 6279  n be composed by
+00001c60: 2067 656f 7370 614e 4e2e 6d61 6b65 5f67   geospaNN.make_g
+00001c70: 7261 7068 2829 272e 0a60 6060 636f 6d6d  raph()'..```comm
+00001c80: 616e 646c 696e 655c 0a74 6573 745f 7072  andline\.test_pr
+00001c90: 6564 6963 7420 3d20 6d6f 6465 6c2e 7072  edict = model.pr
+00001ca0: 6564 6963 7428 6461 7461 5f74 7261 696e  edict(data_train
+00001cb0: 2c20 6461 7461 5f74 6573 7429 0a60 6060  , data_test).```
+00001cc0: 0a0a 2323 2052 756e 6e69 6e67 2065 7861  ..## Running exa
+00001cd0: 6d70 6c65 733a 0a2a 2041 2073 696d 756c  mples:.* A simul
+00001ce0: 6174 696f 6e20 6578 7065 7269 6d65 6e74  ation experiment
+00001cf0: 2077 6974 6820 6120 636f 6d6d 6f6e 2073   with a common s
+00001d00: 7061 7469 616c 2073 6574 7469 6e67 2069  patial setting i
+00001d10: 7320 7368 6f77 6e20 5b68 6572 655d 2868  s shown [here](h
+00001d20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001d30: 6d2f 5765 6e74 616f 5a68 616e 3139 3938  m/WentaoZhan1998
+00001d40: 2f67 656f 7370 614e 4e2f 626c 6f62 2f6d  /geospaNN/blob/m
+00001d50: 6169 6e2f 4578 616d 706c 655f 7369 6d75  ain/Example_simu
+00001d60: 6c61 7469 6f6e 2e69 7079 6e62 292e 0a0a  lation.ipynb)...
+00001d70: 2a20 4120 7265 616c 2064 6174 6120 6578  * A real data ex
+00001d80: 7065 7269 6d65 6e74 2069 7320 7368 6f77  periment is show
+00001d90: 6e20 5b68 6572 655d 2868 7474 7073 3a2f  n [here](https:/
+00001da0: 2f67 6974 6875 622e 636f 6d2f 5765 6e74  /github.com/Went
+00001db0: 616f 5a68 616e 3139 3938 2f67 656f 7370  aoZhan1998/geosp
+00001dc0: 614e 4e2f 626c 6f62 2f6d 6169 6e2f 4578  aNN/blob/main/Ex
+00001dd0: 616d 706c 655f 7265 616c 6461 7461 2e69  ample_realdata.i
+00001de0: 7079 6e62 292e 200a 2a20 5468 6520 504d  pynb). .* The PM
+00001df0: 322e 3520 6461 7461 2069 7320 636f 6c6c  2.5 data is coll
+00001e00: 6563 7465 6420 6672 6f6d 2074 6865 205b  ected from the [
+00001e10: 552e 532e 2045 6e76 6972 6f6e 6d65 6e74  U.S. Environment
+00001e20: 616c 2050 726f 7465 6374 696f 6e20 4167  al Protection Ag
+00001e30: 656e 6379 5d28 6874 7470 733a 2f2f 7777  ency](https://ww
+00001e40: 772e 6570 612e 676f 762f 6f75 7464 6f6f  w.epa.gov/outdoo
+00001e50: 722d 6169 722d 7175 616c 6974 792d 6461  r-air-quality-da
+00001e60: 7461 2f64 6f77 6e6c 6f61 642d 6461 696c  ta/download-dail
+00001e70: 792d 6461 7461 2920 6461 7461 7365 7473  y-data) datasets
+00001e80: 2066 6f72 2065 6163 6820 7374 6174 6520   for each state 
+00001e90: 6172 6520 636f 6c6c 6563 7465 6420 616e  are collected an
+00001ea0: 6420 626f 756e 6420 746f 6765 7468 6572  d bound together
+00001eb0: 2074 6f20 6f62 7461 696e 2027 706d 3235   to obtain 'pm25
+00001ec0: 5f32 3032 322e 6373 7627 2e20 6461 696c  _2022.csv'. dail
+00001ed0: 7920 504d 322e 3520 6669 6c65 7320 6172  y PM2.5 files ar
+00001ee0: 6520 7375 6273 6574 7320 6f66 2027 706d  e subsets of 'pm
+00001ef0: 3235 5f32 3032 322e 6373 7627 2070 726f  25_2022.csv' pro
+00001f00: 6475 6365 6420 6279 2027 7265 616c 6461  duced by 'realda
+00001f10: 7461 5f70 7265 7072 6f63 6573 732e 7079  ta_preprocess.py
+00001f20: 272e 204f 6e65 2063 616e 2073 6b69 7020  '. One can skip 
+00001f30: 7468 6520 7072 6570 726f 6365 7373 696e  the preprocessin
+00001f40: 6720 616e 6420 7573 6520 7468 6520 6461  g and use the da
+00001f50: 696c 7920 6669 6c65 7320 6469 7265 6374  ily files direct
+00001f60: 6f72 792e 200a 2a20 5468 6520 6d65 7465  ory. .* The mete
+00001f70: 6f72 6f6c 6f67 6963 616c 2064 6174 6120  orological data 
+00001f80: 6973 2063 6f6c 6c65 6374 6564 2066 726f  is collected fro
+00001f90: 6d20 7468 6520 5b4e 6174 696f 6e61 6c20  m the [National 
+00001fa0: 4365 6e74 6572 7320 666f 7220 456e 7669  Centers for Envi
+00001fb0: 726f 6e6d 656e 7461 6c20 5072 6564 6963  ronmental Predic
+00001fc0: 7469 6f6e e280 9973 2028 4e43 4550 2920  tion...s (NCEP) 
+00001fd0: 4e6f 7274 6820 416d 6572 6963 616e 2052  North American R
+00001fe0: 6567 696f 6e61 6c20 5265 616e 616c 7973  egional Reanalys
+00001ff0: 6973 2028 4e41 5252 2920 7072 6f64 7563  is (NARR) produc
+00002000: 745d 2868 7474 7073 3a2f 2f70 736c 2e6e  t](https://psl.n
+00002010: 6f61 612e 676f 762f 6461 7461 2f67 7269  oaa.gov/data/gri
+00002020: 6464 6564 2f64 6174 612e 6e61 7272 2e68  dded/data.narr.h
+00002030: 746d 6c29 2e20 5468 6520 272e 6e63 2720  tml). The '.nc' 
+00002040: 286e 6574 4344 4629 2066 696c 6573 2073  (netCDF) files s
+00002050: 686f 756c 6420 6265 2064 6f77 6e6c 6f61  hould be downloa
+00002060: 6465 6420 6672 6f6d 2074 6865 2077 6562  ded from the web
+00002070: 7369 7465 2061 6e64 2073 6176 6564 2069  site and saved i
+00002080: 6e20 7468 6520 726f 6f74 2064 6972 6563  n the root direc
+00002090: 746f 7279 2074 6f20 7275 6e20 2772 6561  tory to run 'rea
+000020a0: 6c64 6174 615f 7072 6570 726f 6365 7373  ldata_preprocess
+000020b0: 2e70 7927 2e20 4f74 6865 7277 6973 652c  .py'. Otherwise,
+000020c0: 206f 6e65 206d 6179 2073 6b69 7020 7468   one may skip th
+000020d0: 6520 7072 6570 726f 6365 7373 696e 6720  e preprocessing 
+000020e0: 616e 6420 7573 6520 636f 7661 7269 6174  and use covariat
+000020f0: 6520 6669 6c65 7320 6469 7265 6374 6c79  e files directly
+00002100: 2e20 0a0a 2323 2043 6974 6174 696f 6e0a  . ..## Citation.
+00002110: 506c 6561 7365 2063 6974 6520 7468 6520  Please cite the 
+00002120: 666f 6c6c 6f77 696e 6720 7061 7065 7220  following paper 
+00002130: 7768 656e 2079 6f75 2075 7365 202a 2a67  when you use **g
+00002140: 656f 7370 614e 4e2a 2a3a 0a0a 3e20 5a68  eospaNN**:..> Zh
+00002150: 616e 2c20 5765 6e74 616f 2c20 616e 6420  an, Wentao, and 
+00002160: 4162 6869 7275 7020 4461 7474 612e 2022  Abhirup Datta. "
+00002170: 4e65 7572 616c 206e 6574 776f 726b 7320  Neural networks 
+00002180: 666f 7220 6765 6f73 7061 7469 616c 2064  for geospatial d
+00002190: 6174 612e 2220 4a6f 7572 6e61 6c20 6f66  ata." Journal of
+000021a0: 2074 6865 2041 6d65 7269 6361 6e20 5374   the American St
+000021b0: 6174 6973 7469 6361 6c20 4173 736f 6369  atistical Associ
+000021c0: 6174 696f 6e20 5468 656f 7279 2061 6e64  ation Theory and
+000021d0: 204d 6574 686f 6473 2028 3230 3234 2c20   Methods (2024, 
+000021e0: 696e 2070 7265 7373 2920 6172 5869 7620  in press) arXiv 
+000021f0: 7072 6570 7269 6e74 2061 7258 6976 3a32  preprint arXiv:2
+00002200: 3330 342e 3039 3135 370a 200a 0a23 2320  304.09157. ..## 
+00002210: 5265 6665 7265 6e63 6573 0a0a 4461 7474  References..Datt
+00002220: 612c 2041 6268 6972 7570 2c20 5375 6469  a, Abhirup, Sudi
+00002230: 7074 6f20 4261 6e65 726a 6565 2c20 416e  pto Banerjee, An
+00002240: 6472 6577 204f 2e20 4669 6e6c 6579 2c20  drew O. Finley, 
+00002250: 616e 6420 416c 616e 2045 2e20 4765 6c66  and Alan E. Gelf
+00002260: 616e 642e 2022 4869 6572 6172 6368 6963  and. "Hierarchic
+00002270: 616c 206e 6561 7265 7374 2d6e 6569 6768  al nearest-neigh
+00002280: 626f 7220 4761 7573 7369 616e 2070 726f  bor Gaussian pro
+00002290: 6365 7373 206d 6f64 656c 7320 666f 7220  cess models for 
+000022a0: 6c61 7267 6520 6765 6f73 7461 7469 7374  large geostatist
+000022b0: 6963 616c 2064 6174 6173 6574 732e 2220  ical datasets." 
+000022c0: 4a6f 7572 6e61 6c20 6f66 2074 6865 2041  Journal of the A
+000022d0: 6d65 7269 6361 6e20 5374 6174 6973 7469  merican Statisti
+000022e0: 6361 6c20 4173 736f 6369 6174 696f 6e20  cal Association 
+000022f0: 3131 312c 206e 6f2e 2035 3134 2028 3230  111, no. 514 (20
+00002300: 3136 293a 2038 3030 2d38 3132 2e20 5b6c  16): 800-812. [l
+00002310: 696e 6b5d 2868 7474 7073 3a2f 2f77 7777  ink](https://www
+00002320: 2e74 616e 6466 6f6e 6c69 6e65 2e63 6f6d  .tandfonline.com
+00002330: 2f64 6f69 2f66 756c 6c2f 3130 2e31 3038  /doi/full/10.108
+00002340: 302f 3031 3632 3134 3539 2e32 3031 352e  0/01621459.2015.
+00002350: 3130 3434 3039 3129 0a0a 5a68 616e 2c20  1044091)..Zhan, 
+00002360: 5765 6e74 616f 2c20 616e 6420 4162 6869  Wentao, and Abhi
+00002370: 7275 7020 4461 7474 612e 2022 4e65 7572  rup Datta. "Neur
+00002380: 616c 206e 6574 776f 726b 7320 666f 7220  al networks for 
+00002390: 6765 6f73 7061 7469 616c 2064 6174 612e  geospatial data.
+000023a0: 2220 4a6f 7572 6e61 6c20 6f66 2074 6865  " Journal of the
+000023b0: 2041 6d65 7269 6361 6e20 5374 6174 6973   American Statis
+000023c0: 7469 6361 6c20 4173 736f 6369 6174 696f  tical Associatio
+000023d0: 6e20 5468 656f 7279 2061 6e64 204d 6574  n Theory and Met
+000023e0: 686f 6473 2028 3230 3234 2c20 696e 2070  hods (2024, in p
+000023f0: 7265 7373 2920 6172 5869 7620 7072 6570  ress) arXiv prep
+00002400: 7269 6e74 2061 7258 6976 3a32 3330 342e  rint arXiv:2304.
+00002410: 3039 3135 3720 5b6c 696e 6b5d 2868 7474  09157 [link](htt
+00002420: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00002430: 6273 2f32 3330 342e 3039 3135 3729 0a    bs/2304.09157).
```

### Comparing `geospann-0.1.3/pyproject.toml` & `geospann-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geospaNN"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Wentao Zhan", email="wzhan3@jhu.edu" },
     { name="Abhirup Datta", email="abhidatta@jhu.edu" }
 ]
 maintainers = [
     { name="Wentao Zhan", email="wzhan3@jhu.edu" },
 ]
```

### Comparing `geospann-0.1.3/PKG-INFO` & `geospann-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: geospaNN
-Version: 0.1.3
+Version: 0.1.4
 Summary: A PyThon implementation of NNGLS
 Project-URL: Homepage, https://github.com/WentaoZhan1998/geospaNN
 Project-URL: Repository, https://github.com/WentaoZhan1998/geospaNN.git
 Project-URL: Issues, https://github.com/WentaoZhan1998/geospaNN/issues
 Author-email: Wentao Zhan <wzhan3@jhu.edu>, Abhirup Datta <abhidatta@jhu.edu>
 Maintainer-email: Wentao Zhan <wzhan3@jhu.edu>
 License-File: LICENSE
@@ -23,60 +23,71 @@
 Requires-Dist: scipy
 Requires-Dist: torch-geometric>=2.3.0
 Requires-Dist: torch-scatter>=2.1.2
 Requires-Dist: torch-sparse>=0.6.18
 Requires-Dist: torch>=2.0.0
 Description-Content-Type: text/markdown
 
-[![PyPI](https://img.shields.io/pypi/v/geospaNN)](https://pypi.org/project/geospaNN)
+[![PyPI](https://img.shields.io/pypi/v/geospaNN?logo=PyPI)](https://pypi.org/project/geospaNN)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/geospaNN)
 
 # GeospaNN - Neural networks for geospatial data
 **Authors**: Wentao Zhan (<wzhan3@jhu.edu>), Abhirup Datta (<abhidatta@jhu.edu>)
 ## A package based on the paper: [Neural networks for geospatial data](https://arxiv.org/pdf/2304.09157.pdf)
-**GeospaNN** is a formal implementation of the Neural Networks for geospatial data proposed in Zhan et.al (2023). 
-The package is developed using [PyTorch](https://pytorch.org/) and under the framework of [PyG](https://pytorch-geometric.readthedocs.io/en/latest/) library. 
-Combining the idea of Graph Neural Networks (GNN) and spatial prediction, 
-**geospaNN** simultaneously provides efficient estimation for the non-spatial effect and prediction for the spatial effect, 
-and can sacle up to hundreds of thousands of samples. 
+**GeospaNN** is a formal implementation of NN-GLS, the Neural Networks for geospatial data proposed in Zhan et.al (2023), 
+that explicitly accounts for spatial correlation in the data. The package is developed using [PyTorch](https://pytorch.org/) and 
+under the framework of [PyG](https://pytorch-geometric.readthedocs.io/en/latest/) library. 
+NN-GLS is a geographically-informed Graph Neural Network (GNN) for analyzing large and irregular geospatial data, 
+that combines multi-layer perceptrons, Gaussian processes, and generalized least squares (GLS) loss. 
+NN-GLS offers both regression function estimation and spatial prediction, and can scale up to sample sizes of hundreds of thousands. 
 Users are welcome to provide any helpful suggestions and comments.
 
 ## Overview
-The Python package **geospaNN**' stands for a 'geospatial implementation of Neural Networks', where we impelements the 
-Neural Networks for analysis of geospatial data that explicitly accounts for spatial dependence (NN-GLS) proposed in Zhan et.al (2023). 
-Traditionally, the analysis of geospatial data treats the spatial outcome $y(s)$ as a combination of the fixed effect 
-(linear or non-linear) of covariates $x(s)$ and the spatially correlated random effect $w(s)$. 
-The classical Neural Networks (NN), as one of the most popular machine learning approaches,
-could be used to capture the non-linear fixed effect. 
-However, while NN assume the independence among observations, geospatial data naturally inherits spatial dependency, 
-which is interpreted by Tobler's first law of geography: 
-everything is related to everything else, but nearby things are more related than distant things. 
-On the other hand, traditional geospatial data relies on the model-based approaches to handle the spatial dependency. 
-For example, by assuming $w(s)$ being a stationary Gaussian process (GP), simple techniques like kriging can provide 
-powerful prediction performance by properly aggregating the neighboring information.
-Our package **geospaNN** takes the advantages from both perspective and provides an efficient tool for geospatial data analysis.
-In the package, GP is involved as a trainable target into the Neural Network and used to guide the neighborhood aggregation on
-the output layer. Equivalently, a more efficient loss function is composed for the geospatial setting to improve the 
-estimation, and the idea mimics the comparison between OLS and GLS in linear regression.
-As a downstream of estimating $f(x)$, **geospaNN** provides accurate spatial prediction, thus concludes a complete geospatial analysis pipeline.
-It should be highlighted that **geospaNN**' is compatible with the framework of Graph Neural Networks (GNN), thus being highly generalizable.
-(The implementation of **geospaNN**' uses the 'torch_geom' module.)
-To accelerate the training process for the GP, 
-**geospaNN**' approximate the working correlation structure using Nearest Neighbor Gaussian Process (NNGP) (Datta et al., 2016) 
-which makes it suitable for larger datasets towards a size of 1 million.
-
-![Illustration of NN-GLS](./data/nngls.png)
-
+The Python package **geospaNN** stands for 'geospatial Neural Networks', where we implement NN-GLS, 
+neural networks tailored for analysis of geospatial data that explicitly accounts for spatial dependence (Zhan et.al, 2023). 
+Geospatial data naturally exhibits spatial correlation or dependence and traditional geostatistical analysis often relies on 
+model-based approaches to handle the spatial dependency, treating the spatial outcome $y(s)$ as a linear regression on covariates $x(s)$ and 
+modeling dependency through the spatially correlated errors. 
+For example, using Gaussian processes (GP) to model dependent errors, 
+simple techniques like kriging can provide powerful prediction performance by properly aggregating the neighboring information. 
+On the other hand, artificial Neural Networks (NN), one of the most popular machine learning approaches, could be used to estimate non-linear regression functions. 
+However, common neural networks like multi-layer perceptrons (MLP) does not incorporate correlation among data units.
+
+Our package **geospaNN** takes the advantages from both perspectives and provides an efficient tool for geospatial data analysis. 
+In NN-GLS, an MLP is used to model the non-linear regression function while a GP is used to model the spatial dependence. 
+The resulting loss function then becomes a generalized least squares (GLS) loss informed by the GP covariance matrix, 
+thereby explicitly incorporating spatial correlation into the neural network optimization. 
+The idea mimics the extension of ordinary least squares (OLS) loss to GLS loss in linear regression for dependent data.
+
+Zhan and Datta, 2023 shows that neural networks with GLS loss can be represented as a graph neural network, 
+with the GP covariances guiding the neighborhood aggregation on the output layer. 
+Thus NN-GLS is implemented in **geospaNN** with the framework of Graph Neural Networks (GNN), and is highly generalizable. 
+(The implementation of geospaNN' uses the 'torch_geom' module.)
+
+**geospaNN** provides an estimate of regression function 𝑓(𝑥) as well as accurate spatial predictions using Gaussian process (kriging), 
+and thus constitutes a complete geospatial analysis pipeline. 
+To accelerate the training process for the GP, **geospaNN** approximates the working correlation structure using 
+Nearest Neighbor Gaussian Process (NNGP) (Datta et al., 2016) which makes it suitable for larger datasets towards a size of 1 million.
+
+<div align="center">
+<a href="https://arxiv.org/pdf/2304.09157.pdf">
+  <img
+    src="https://github.com/WentaoZhan1998/geospaNN/blob/main/data/nngls.png?raw=True"
+    width="800"
+  >
+</a>
+</div>
 
 ## Installation
 (Currently) to install the development version of the package, a pre-installed PyTorch and PyG libraries are needed. Installation in the following order is recommended to avoid any compilation issue.
 1. To install PyTorch, find and install the binary suitable for your machine [here](https://pytorch.org/).
 2. Then to install the PyG library, find and install the proper binary [here](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html).
 3. Make sure to also install the dependencies including *pyg_lib*, *torch_scatter*, *torch_sparse*, *torch_cluster*, and *torch_spline_conv*.
 
-Once PyTorch and PyG are successfully installed, use the following command in the terminal:
+Once PyTorch and PyG are successfully installed, use the following command in the terminal for the latest version:
 ```commandline\
 pip install https://github.com/WentaoZhan1998/geospaNN/archive/main.zip
 ```
 
 To install the pypi version, use the following command in the terminal:
 ```commandline\
 pip install geospaNN
@@ -172,14 +183,15 @@
 * A real data experiment is shown [here](https://github.com/WentaoZhan1998/geospaNN/blob/main/Example_realdata.ipynb). 
 * The PM2.5 data is collected from the [U.S. Environmental Protection Agency](https://www.epa.gov/outdoor-air-quality-data/download-daily-data) datasets for each state are collected and bound together to obtain 'pm25_2022.csv'. daily PM2.5 files are subsets of 'pm25_2022.csv' produced by 'realdata_preprocess.py'. One can skip the preprocessing and use the daily files directory. 
 * The meteorological data is collected from the [National Centers for Environmental Prediction’s (NCEP) North American Regional Reanalysis (NARR) product](https://psl.noaa.gov/data/gridded/data.narr.html). The '.nc' (netCDF) files should be downloaded from the website and saved in the root directory to run 'realdata_preprocess.py'. Otherwise, one may skip the preprocessing and use covariate files directly. 
 
 ## Citation
 Please cite the following paper when you use **geospaNN**:
 
-> Zhan, Wentao, and Abhirup Datta. "Neural networks for geospatial data." arXiv preprint arXiv:2304.09157 (2023).
+> Zhan, Wentao, and Abhirup Datta. "Neural networks for geospatial data." Journal of the American Statistical Association Theory and Methods (2024, in press) arXiv preprint arXiv:2304.09157
+ 
 
 ## References
 
 Datta, Abhirup, Sudipto Banerjee, Andrew O. Finley, and Alan E. Gelfand. "Hierarchical nearest-neighbor Gaussian process models for large geostatistical datasets." Journal of the American Statistical Association 111, no. 514 (2016): 800-812. [link](https://www.tandfonline.com/doi/full/10.1080/01621459.2015.1044091)
 
-Zhan, Wentao, and Abhirup Datta. "Neural networks for geospatial data." arXiv preprint arXiv:2304.09157 (2023). [link](https://arxiv.org/abs/2304.09157)
+Zhan, Wentao, and Abhirup Datta. "Neural networks for geospatial data." Journal of the American Statistical Association Theory and Methods (2024, in press) arXiv preprint arXiv:2304.09157 [link](https://arxiv.org/abs/2304.09157)
```

