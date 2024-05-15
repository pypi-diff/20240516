# Comparing `tmp/ntv_numpy-0.1.2.tar.gz` & `tmp/ntv_numpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntv_numpy-0.1.2.tar", last modified: Wed Apr 10 21:44:33 2024, max compression
+gzip compressed data, was "ntv_numpy-0.2.0.tar", last modified: Sun May  5 21:52:58 2024, max compression
```

## Comparing `ntv_numpy-0.1.2.tar` & `ntv_numpy-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 21:44:33.472978 ntv_numpy-0.1.2/
--rw-rw-rw-   0        0        0    10790 2024-04-10 21:44:33.472978 ntv_numpy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    10017 2024-04-10 21:37:16.000000 ntv_numpy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 21:44:33.466505 ntv_numpy-0.1.2/ntv_numpy/
--rw-rw-rw-   0        0        0     1563 2024-04-10 06:55:40.000000 ntv_numpy-0.1.2/ntv_numpy/__init__.py
--rw-rw-rw-   0        0        0    14738 2024-04-09 21:42:42.000000 ntv_numpy-0.1.2/ntv_numpy/data_array.py
--rw-rw-rw-   0        0        0    24520 2024-04-09 21:45:12.000000 ntv_numpy-0.1.2/ntv_numpy/ndarray.py
--rw-rw-rw-   0        0        0     5054 2024-03-05 23:18:41.000000 ntv_numpy-0.1.2/ntv_numpy/ntv_numpy.ini
--rw-rw-rw-   0        0        0    12366 2024-04-09 21:53:06.000000 ntv_numpy-0.1.2/ntv_numpy/numpy_ntv_connector.py
--rw-rw-rw-   0        0        0    16413 2024-04-10 12:55:37.000000 ntv_numpy-0.1.2/ntv_numpy/xconnector.py
--rw-rw-rw-   0        0        0    16394 2024-04-10 12:33:19.000000 ntv_numpy-0.1.2/ntv_numpy/xdataset.py
--rw-rw-rw-   0        0        0     9691 2024-04-10 08:34:11.000000 ntv_numpy-0.1.2/ntv_numpy/xndarray.py
-drwxrwxrwx   0        0        0        0 2024-04-10 21:44:33.471982 ntv_numpy-0.1.2/ntv_numpy.egg-info/
--rw-rw-rw-   0        0        0    10790 2024-04-10 21:44:33.000000 ntv_numpy-0.1.2/ntv_numpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-04-10 21:44:33.000000 ntv_numpy-0.1.2/ntv_numpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 21:44:33.000000 ntv_numpy-0.1.2/ntv_numpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-10 21:44:33.000000 ntv_numpy-0.1.2/ntv_numpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-10 21:44:33.000000 ntv_numpy-0.1.2/ntv_numpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-10 21:44:33.473973 ntv_numpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1220 2024-04-10 21:37:45.000000 ntv_numpy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 21:44:33.470986 ntv_numpy-0.1.2/tests/
--rw-rw-rw-   0        0        0    24858 2024-04-10 06:54:44.000000 ntv_numpy-0.1.2/tests/test_ntv_numpy.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:52:58.540196 ntv_numpy-0.2.0/
+-rw-rw-rw-   0        0        0    12125 2024-05-05 21:52:58.539698 ntv_numpy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11352 2024-05-05 21:16:27.000000 ntv_numpy-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 21:52:58.532731 ntv_numpy-0.2.0/ntv_numpy/
+-rw-rw-rw-   0        0        0     1983 2024-05-05 21:28:10.000000 ntv_numpy-0.2.0/ntv_numpy/__init__.py
+-rw-rw-rw-   0        0        0     9057 2024-05-05 20:21:42.000000 ntv_numpy-0.2.0/ntv_numpy/data_array.py
+-rw-rw-rw-   0        0        0    22905 2024-05-05 20:24:37.000000 ntv_numpy-0.2.0/ntv_numpy/ndarray.py
+-rw-rw-rw-   0        0        0     2603 2024-05-05 20:56:51.000000 ntv_numpy-0.2.0/ntv_numpy/ndtype.py
+-rw-rw-rw-   0        0        0     5166 2024-04-23 08:57:01.000000 ntv_numpy-0.2.0/ntv_numpy/ntv_numpy.ini
+-rw-rw-rw-   0        0        0     8050 2024-05-05 20:29:43.000000 ntv_numpy-0.2.0/ntv_numpy/numpy_ntv_connector.py
+-rw-rw-rw-   0        0        0    26795 2024-05-05 20:51:45.000000 ntv_numpy-0.2.0/ntv_numpy/xconnector.py
+-rw-rw-rw-   0        0        0    19014 2024-05-05 20:53:50.000000 ntv_numpy-0.2.0/ntv_numpy/xdataset.py
+-rw-rw-rw-   0        0        0     9535 2024-05-05 20:39:24.000000 ntv_numpy-0.2.0/ntv_numpy/xndarray.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:52:58.538204 ntv_numpy-0.2.0/ntv_numpy.egg-info/
+-rw-rw-rw-   0        0        0    12125 2024-05-05 21:52:58.000000 ntv_numpy-0.2.0/ntv_numpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-05-05 21:52:58.000000 ntv_numpy-0.2.0/ntv_numpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 21:52:58.000000 ntv_numpy-0.2.0/ntv_numpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-05 21:52:58.000000 ntv_numpy-0.2.0/ntv_numpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 21:52:58.000000 ntv_numpy-0.2.0/ntv_numpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-05 21:52:58.541192 ntv_numpy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2024-05-05 21:19:25.000000 ntv_numpy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:52:58.537209 ntv_numpy-0.2.0/tests/
+-rw-rw-rw-   0        0        0    31561 2024-05-04 21:34:22.000000 ntv_numpy-0.2.0/tests/test_ntv_numpy.py
```

### Comparing `ntv_numpy-0.1.2/PKG-INFO` & `ntv_numpy-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: ntv_numpy
-Version: 0.1.2
-Summary: NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability
-Home-page: https://github.com/loco-philippe/ntv-numpy/blob/main/README.md
-Author: Philippe Thomy
-Author-email: philippe@loco-labs.io
-Keywords: numpy,JSON-NTV,semantic JSON,development,environmental data,multidimensional
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9, <4
-Description-Content-Type: text/markdown
-Requires-Dist: json_ntv
-Requires-Dist: numpy
-Requires-Dist: shapely
-
 ### *NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability*
 
 For more information, see the [user guide](https://loco-philippe.github.io/ntv-numpy/docs/user_guide.html) or the [github repository](https://github.com/loco-philippe/ntv-numpy).
 
 # Why a new format for multidimensional data ?
 
 Each tool has a specific structure for processing multidimensional data with the following consequences:
@@ -52,17 +33,18 @@
 
 ```mermaid
 ---
 title: Example of interoperability
 ---
 flowchart LR
     A[Xarray] <--lossless--> B[Neutral\nXdataset]
-    B <--lossless--> C[NDData]
     D[Scipp] <--lossless--> B
+    C[NDData] <--lossless--> B
     B <--lossless--> E[JSON]
+    B <--lossless--> F[DataFrame]
 ```
 
 ### Data example
 
 ```python
 In [1]: example = {
                 'example:xdataset': {
@@ -78,56 +60,59 @@
                         
                         'ranking': [['month', [2, 2], [1, 2, 3, 4]], ['var1']],
                         'z': [['float', [10, 20]], ['x']],
                         'z.uncertainty': [[[0.1, 0.2]]],
                         
                         'z_bis': [[['z1_bis', 'z2_bis']]],
                 
-                        'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/'}
+                        'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/',
+                        'location': [['string', ['paris']]]}
                 }
         }
 
 In [2]: from ntv_numpy import Xdataset
 
         x_example = Xdataset.read_json(example)
-        x_example.info
+        x_example.info['structure']
 Out[2]: {'name': 'example',
         'xtype': 'group',
         'data_vars': ['var1', 'var2'],
         'data_arrays': ['z_bis'],
         'dimensions': ['x', 'y'],
         'coordinates': ['ranking', 'z'],
         'additionals': ['var1.mask1', 'var1.mask2', 'var1.variance', 'z.uncertainty'],
         'metadata': ['info'],
+        'uniques': ['location'],
         'validity': 'undefined',
         'length': 4,
-        'width': 12}
+        'width': 13}
 ```
 
 The JSON representation is equivalent to the Xdataset entity (Json conversion reversible)
 
 ```python
 In [3]: x_json = x_example.to_json()
         x_example_json = Xdataset.read_json(x_json)
         x_example_json == x_example
-Out[2]: True
+Out[3]: True
 ```
 
 ### Xarray interoperability
 
 ```python
 In [4]: x_xarray = x_example.to_xarray()
         print(x_xarray)
-Out[4]: <xarray.Dataset> Size: 182B
+Out[4]: <xarray.Dataset> Size: 202B
         Dimensions:        (x: 2, y: 2)
         Coordinates:
           * x              (x) <U6 48B '23F0AE' '578B98'
           * y              (y) datetime64[ns] 16B 2021-01-01 2022-02-02
             ranking        (x, y) int32 16B 1 2 3 4
             z              (x) float64 16B 10.0 20.0
+            location       <U5 20B 'paris'
             var1.mask1     (x) bool 2B True False
             var1.mask2     (x, y) bool 4B True False False True
             var1.variance  (x, y) float64 32B 0.1 0.2 0.3 0.4
             z.uncertainty  (x) float64 16B 0.1 0.2
         Data variables:
             var1           (x, y) float64 32B 10.1 0.4 3.4 8.2
         Attributes:
@@ -136,25 +121,55 @@
             var2:     [['var2.ntv'], ['x', 'y']]
             z_bis:    [['string', ['z1_bis', 'z2_bis']]]
 ```
 
 Reversibility:
 
 ```python
-In [3]: x_example_xr = Xdataset.from_xarray(x_xarray)
+In [5]: x_example_xr = Xdataset.from_xarray(x_xarray)
         x_example_xr == x_example_json == x_example
-Out[2]: True
+Out[5]: True
+```
+
+### Pandas interoperability
+
+```python
+In [6]: x_dataframe = x_example.to_dataframe()
+        print(x_example.to_dataframe(json_name=False))
+        print(x_xarray)
+Out[6]: 
+                   ranking     z  z.uncertainty  var1  var1.mask1  var1.mask2  \
+x      y                                                                        
+23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True   
+       2022-02-02        2  10.0            0.1   0.4        True       False   
+578B98 2021-01-01        3  20.0            0.2   3.4       False       False   
+       2022-02-02        4  20.0            0.2   8.2       False        True   
+
+                   var1.variance location  
+x      y                                   
+23F0AE 2021-01-01            0.1    paris  
+       2022-02-02            0.2    paris  
+578B98 2021-01-01            0.3    paris  
+       2022-02-02            0.4    paris 
+```
+
+Reversibility:
+
+```python
+In [7]: x_example_pd = Xdataset.from_dataframe(x_dataframe)
+        x_example_pd == x_example_xr == x_example_json == x_example
+Out[7]: True
 ```
 
 ### scipp interoperability
 
 ```python
-In [4]: x_scipp = x_example.to_scipp()
+In [8]: x_scipp = x_example.to_scipp()
         print(x_scipp['example'])
-Out[4]: <scipp.Dataset>
+Out[8]: <scipp.Dataset>
 Dimensions: Sizes[x:string:2, y:date:2, ]
 Coordinates:
 * ranking:month           int32  [dimensionless]  (x:string, y:date)  [1, 2, 3, 4]
 * x:string               string  [dimensionless]  (x:string)  ["23F0AE", "578B98"]
 * y:date              datetime64            [ns]  (y:date)  [2021-01-01T00:00:00.000000000, 2022-02-02T00:00:00.000000000]
 * z:float               float64  [dimensionless]  (x:string)  [10, 20]
 Data:
@@ -163,17 +178,17 @@
         mask1:boolean      bool  [dimensionless]  (x:string)  [True, False]
         mask2:boolean      bool  [dimensionless]  (x:string, y:date)  [True, False, False, True]
 ```
 
 Reversibility:
 
 ```python
-In [3]: x_example_sc = Xdataset.from_scipp(x_scipp)
-        x_example_sc == x_example_xr == x_example_json == x_example
-Out[2]: True
+In [9]: x_example_sc = Xdataset.from_scipp(x_scipp)
+        x_example_sc == x_example_pd == x_example_xr == x_example_json == x_example
+Out[9]: True
 ```
 
 ### NDData interoperability
 
 ```python
 In [1]: example = {
                 'example:xdataset': {
@@ -187,35 +202,35 @@
                                 'CTYPE2': 'DEC--TAN', 'CRVAL1': 5.63056810618, 'CRVAL2': -72.05457184279, 'LONPOLE': 180.0,
                                 'LATPOLE': -72.05457184279, 'WCSNAME': 'IDC_qbu1641sj', 'MJDREF': 0.0, 'RADESYS': 'ICRS'},
                         'psf': [['float[erg/s]', [1,2,3,4]]]
                 }
         } 
         n_example = Xdataset.read_json(example)
         n_example.info 
-Out[4]: {'name': 'example',
+Out[1]: {'name': 'example',
         'xtype': 'group',
         'data_arrays': ['data', 'psf'],
         'additionals': ['data.mask', 'data.uncertainty'],
         'metadata': ['meta', 'wcs'],
         'validity': 'valid',
         'width': 6}
 ```
 
 ```python
-In [4]: n_nddata = n_example.to_nddata()
+In [2]: n_nddata = n_example.to_nddata()
         n_nddata
-Out[4]: NDData([1., 2., ——, ——], unit='erg / s')
+Out[2]: NDData([1., 2., ——, ——], unit='erg / s')
 ```
 
 Reversibility:
 
 ```python
-In [5]: n_example_ndd = Xdataset.from_nddata(n_nddata)
+In [3]: n_example_ndd = Xdataset.from_nddata(n_nddata)
         n_example_ndd == n_example
-Out[5]: True
+Out[3]: True
 ```
 
 ## URI usage
 
 In the example, only structural data is exchanged with json format.
 
 ```python
@@ -241,15 +256,15 @@
                 }
         }
 ```
 
 The complete example can be rebuild with loading data (path + file name).
 
 ```python
-In [5]: # simulation of reading files at the indicated "path"
+In [2]: # simulation of reading files at the indicated "path"
         var1          = np.array([10.1, 0.4, 3.4, 8.2])
         var1_variance = Ndarray([0.1, 0.2, 0.3, 0.4], ntv_type='float')
         var1_mask1    = np.array([True, False])
         var1_mask2    = np.array([True, False, False, True])
         var2          = Ndarray('var2.ntv')
         x             = np.array(['23F0AE', '578B98'])
         y             = np.array(['2021-01-01', '2022-02-02'], dtype='datetime64[D]')
@@ -261,9 +276,9 @@
         array_data = [var1, var1_variance, var1_mask1, var1_mask2, var2, x, y, ranking, z, z_uncertainty, z_bis]
 
         x_example_mixte_numpy = copy(x_example_mixte)
         for data, xnda in zip(array_data, x_example_mixte_numpy.xnd):
         xnda.set_ndarray(Ndarray(data))
 
         x_example_mixte_numpy == x_example_mixte_json == x_example_sc == x_example_xr == x_example_json == x_example
-Out[5]: True
+Out[2]: True
 ```
```

### Comparing `ntv_numpy-0.1.2/README.md` & `ntv_numpy-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: ntv_numpy
+Version: 0.2.0
+Summary: NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability
+Home-page: https://github.com/loco-philippe/ntv-numpy/blob/main/README.md
+Author: Philippe Thomy
+Author-email: philippe@loco-labs.io
+Keywords: numpy,JSON-NTV,semantic JSON,development,environmental data,multidimensional
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9, <4
+Description-Content-Type: text/markdown
+Requires-Dist: json_ntv
+Requires-Dist: numpy
+Requires-Dist: shapely
+
 ### *NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability*
 
 For more information, see the [user guide](https://loco-philippe.github.io/ntv-numpy/docs/user_guide.html) or the [github repository](https://github.com/loco-philippe/ntv-numpy).
 
 # Why a new format for multidimensional data ?
 
 Each tool has a specific structure for processing multidimensional data with the following consequences:
@@ -33,17 +52,18 @@
 
 ```mermaid
 ---
 title: Example of interoperability
 ---
 flowchart LR
     A[Xarray] <--lossless--> B[Neutral\nXdataset]
-    B <--lossless--> C[NDData]
     D[Scipp] <--lossless--> B
+    C[NDData] <--lossless--> B
     B <--lossless--> E[JSON]
+    B <--lossless--> F[DataFrame]
 ```
 
 ### Data example
 
 ```python
 In [1]: example = {
                 'example:xdataset': {
@@ -59,56 +79,59 @@
                         
                         'ranking': [['month', [2, 2], [1, 2, 3, 4]], ['var1']],
                         'z': [['float', [10, 20]], ['x']],
                         'z.uncertainty': [[[0.1, 0.2]]],
                         
                         'z_bis': [[['z1_bis', 'z2_bis']]],
                 
-                        'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/'}
+                        'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/',
+                        'location': [['string', ['paris']]]}
                 }
         }
 
 In [2]: from ntv_numpy import Xdataset
 
         x_example = Xdataset.read_json(example)
-        x_example.info
+        x_example.info['structure']
 Out[2]: {'name': 'example',
         'xtype': 'group',
         'data_vars': ['var1', 'var2'],
         'data_arrays': ['z_bis'],
         'dimensions': ['x', 'y'],
         'coordinates': ['ranking', 'z'],
         'additionals': ['var1.mask1', 'var1.mask2', 'var1.variance', 'z.uncertainty'],
         'metadata': ['info'],
+        'uniques': ['location'],
         'validity': 'undefined',
         'length': 4,
-        'width': 12}
+        'width': 13}
 ```
 
 The JSON representation is equivalent to the Xdataset entity (Json conversion reversible)
 
 ```python
 In [3]: x_json = x_example.to_json()
         x_example_json = Xdataset.read_json(x_json)
         x_example_json == x_example
-Out[2]: True
+Out[3]: True
 ```
 
 ### Xarray interoperability
 
 ```python
 In [4]: x_xarray = x_example.to_xarray()
         print(x_xarray)
-Out[4]: <xarray.Dataset> Size: 182B
+Out[4]: <xarray.Dataset> Size: 202B
         Dimensions:        (x: 2, y: 2)
         Coordinates:
           * x              (x) <U6 48B '23F0AE' '578B98'
           * y              (y) datetime64[ns] 16B 2021-01-01 2022-02-02
             ranking        (x, y) int32 16B 1 2 3 4
             z              (x) float64 16B 10.0 20.0
+            location       <U5 20B 'paris'
             var1.mask1     (x) bool 2B True False
             var1.mask2     (x, y) bool 4B True False False True
             var1.variance  (x, y) float64 32B 0.1 0.2 0.3 0.4
             z.uncertainty  (x) float64 16B 0.1 0.2
         Data variables:
             var1           (x, y) float64 32B 10.1 0.4 3.4 8.2
         Attributes:
@@ -117,25 +140,55 @@
             var2:     [['var2.ntv'], ['x', 'y']]
             z_bis:    [['string', ['z1_bis', 'z2_bis']]]
 ```
 
 Reversibility:
 
 ```python
-In [3]: x_example_xr = Xdataset.from_xarray(x_xarray)
+In [5]: x_example_xr = Xdataset.from_xarray(x_xarray)
         x_example_xr == x_example_json == x_example
-Out[2]: True
+Out[5]: True
+```
+
+### Pandas interoperability
+
+```python
+In [6]: x_dataframe = x_example.to_dataframe()
+        print(x_example.to_dataframe(json_name=False))
+        print(x_xarray)
+Out[6]: 
+                   ranking     z  z.uncertainty  var1  var1.mask1  var1.mask2  \
+x      y                                                                        
+23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True   
+       2022-02-02        2  10.0            0.1   0.4        True       False   
+578B98 2021-01-01        3  20.0            0.2   3.4       False       False   
+       2022-02-02        4  20.0            0.2   8.2       False        True   
+
+                   var1.variance location  
+x      y                                   
+23F0AE 2021-01-01            0.1    paris  
+       2022-02-02            0.2    paris  
+578B98 2021-01-01            0.3    paris  
+       2022-02-02            0.4    paris 
+```
+
+Reversibility:
+
+```python
+In [7]: x_example_pd = Xdataset.from_dataframe(x_dataframe)
+        x_example_pd == x_example_xr == x_example_json == x_example
+Out[7]: True
 ```
 
 ### scipp interoperability
 
 ```python
-In [4]: x_scipp = x_example.to_scipp()
+In [8]: x_scipp = x_example.to_scipp()
         print(x_scipp['example'])
-Out[4]: <scipp.Dataset>
+Out[8]: <scipp.Dataset>
 Dimensions: Sizes[x:string:2, y:date:2, ]
 Coordinates:
 * ranking:month           int32  [dimensionless]  (x:string, y:date)  [1, 2, 3, 4]
 * x:string               string  [dimensionless]  (x:string)  ["23F0AE", "578B98"]
 * y:date              datetime64            [ns]  (y:date)  [2021-01-01T00:00:00.000000000, 2022-02-02T00:00:00.000000000]
 * z:float               float64  [dimensionless]  (x:string)  [10, 20]
 Data:
@@ -144,17 +197,17 @@
         mask1:boolean      bool  [dimensionless]  (x:string)  [True, False]
         mask2:boolean      bool  [dimensionless]  (x:string, y:date)  [True, False, False, True]
 ```
 
 Reversibility:
 
 ```python
-In [3]: x_example_sc = Xdataset.from_scipp(x_scipp)
-        x_example_sc == x_example_xr == x_example_json == x_example
-Out[2]: True
+In [9]: x_example_sc = Xdataset.from_scipp(x_scipp)
+        x_example_sc == x_example_pd == x_example_xr == x_example_json == x_example
+Out[9]: True
 ```
 
 ### NDData interoperability
 
 ```python
 In [1]: example = {
                 'example:xdataset': {
@@ -168,35 +221,35 @@
                                 'CTYPE2': 'DEC--TAN', 'CRVAL1': 5.63056810618, 'CRVAL2': -72.05457184279, 'LONPOLE': 180.0,
                                 'LATPOLE': -72.05457184279, 'WCSNAME': 'IDC_qbu1641sj', 'MJDREF': 0.0, 'RADESYS': 'ICRS'},
                         'psf': [['float[erg/s]', [1,2,3,4]]]
                 }
         } 
         n_example = Xdataset.read_json(example)
         n_example.info 
-Out[4]: {'name': 'example',
+Out[1]: {'name': 'example',
         'xtype': 'group',
         'data_arrays': ['data', 'psf'],
         'additionals': ['data.mask', 'data.uncertainty'],
         'metadata': ['meta', 'wcs'],
         'validity': 'valid',
         'width': 6}
 ```
 
 ```python
-In [4]: n_nddata = n_example.to_nddata()
+In [2]: n_nddata = n_example.to_nddata()
         n_nddata
-Out[4]: NDData([1., 2., ——, ——], unit='erg / s')
+Out[2]: NDData([1., 2., ——, ——], unit='erg / s')
 ```
 
 Reversibility:
 
 ```python
-In [5]: n_example_ndd = Xdataset.from_nddata(n_nddata)
+In [3]: n_example_ndd = Xdataset.from_nddata(n_nddata)
         n_example_ndd == n_example
-Out[5]: True
+Out[3]: True
 ```
 
 ## URI usage
 
 In the example, only structural data is exchanged with json format.
 
 ```python
@@ -222,15 +275,15 @@
                 }
         }
 ```
 
 The complete example can be rebuild with loading data (path + file name).
 
 ```python
-In [5]: # simulation of reading files at the indicated "path"
+In [2]: # simulation of reading files at the indicated "path"
         var1          = np.array([10.1, 0.4, 3.4, 8.2])
         var1_variance = Ndarray([0.1, 0.2, 0.3, 0.4], ntv_type='float')
         var1_mask1    = np.array([True, False])
         var1_mask2    = np.array([True, False, False, True])
         var2          = Ndarray('var2.ntv')
         x             = np.array(['23F0AE', '578B98'])
         y             = np.array(['2021-01-01', '2022-02-02'], dtype='datetime64[D]')
@@ -242,9 +295,9 @@
         array_data = [var1, var1_variance, var1_mask1, var1_mask2, var2, x, y, ranking, z, z_uncertainty, z_bis]
 
         x_example_mixte_numpy = copy(x_example_mixte)
         for data, xnda in zip(array_data, x_example_mixte_numpy.xnd):
         xnda.set_ndarray(Ndarray(data))
 
         x_example_mixte_numpy == x_example_mixte_json == x_example_sc == x_example_xr == x_example_json == x_example
-Out[5]: True
+Out[2]: True
 ```
```

### Comparing `ntv_numpy-0.1.2/ntv_numpy/ndarray.py` & `ntv_numpy-0.2.0/ntv_numpy/ndarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,63 +16,64 @@
 """
 
 import datetime
 import json
 
 from decimal import Decimal
 import numpy as np
-from json_ntv import Ntv, ShapelyConnec, Datatype, NtvConnector
+from json_ntv import Ntv, ShapelyConnec, NtvConnector  # , Datatype
 from ntv_numpy.data_array import Dfull, Dcomplete, Darray, Dutil
+from ntv_numpy.ndtype import Ndtype, NP_NTYPE
 
 
 class Ndarray:
     ''' The Ndarray class is the JSON interface of numpy.ndarrays.
 
     *static methods*
     - `read_json`
     - `to_json`
-    - `equals`
+    - `set_shape`
     '''
 
-    def __init__(self, dar, ntv_type=None, shape=None):
+    def __init__(self, dar, ntv_type=None, shape=None, str_uri=True):
         '''Ndarray constructor.
 
         *Parameters*
 
         - **dar**: Darray or np.ndarray - data to represent
         - **shape** : list of integer (default None) - length of dimensions
         - **ntv_type**: string (default None) - NTVtype to apply
+        - **str_uri**: boolean(default True) - if True and dar is a string,
+        dar is an uri else a np.array
         '''
         dar = [None] if isinstance(dar, list) and len(dar) == 0 else dar
         if isinstance(dar, Ndarray):
             self.uri = dar.uri
             self.is_json = dar.is_json
             self.ntvtype = dar.ntvtype
             self.shape = dar.shape
             self.darray = dar.darray
             return
-        if isinstance(dar, str):
+        if isinstance(dar, str) and str_uri:
             self.uri = dar
             self.is_json = True
-            self.ntvtype = Datatype(ntv_type) if ntv_type else None
+            self.ntvtype = Ndtype(ntv_type) if ntv_type else None
             self.shape = shape
             self.darray = None
             return
         if shape:
             dar = Dfull(dar, dtype=Nutil.dtype(ntv_type), unidim=True).data
         else:
-            # dar = np.array(dar if isinstance(dar, (list, np.ndarray)) else [dar],
             dar = np.array(dar, dtype=Nutil.dtype(ntv_type))
             shape = list(dar.shape)
         dar = np.array(dar).reshape(-1)
-        # ntv_type = Nutil.nda_ntv_type(dar) if not (ntv_type or dar is None) else ntv_type
         ntv_type = Nutil.nda_ntv_type(dar, ntv_type)
         self.uri = None
         self.is_json = Nutil.is_json(dar[0])
-        self.ntvtype = Datatype(ntv_type)
+        self.ntvtype = Ndtype(ntv_type)
         self.shape = shape
         self.darray = dar.astype(Nutil.dtype(str(self.ntvtype)))
 
     def __repr__(self):
         '''return classname, the shape and the ntv_type'''
         uri = self.uri if self.uri else ''
         typ = self.ntv_type if self.ntv_type else ''
@@ -97,15 +98,14 @@
             return True
         if self.darray is None or other.darray is None:
             return False
         return Dutil.equals(self.darray, other.darray)
 
     def __len__(self):
         ''' len of ndarray'''
-        # return len(self.darray) if self.darray is not None else Ndarray.len_shape(self.shape)
         return len(self.darray) if self.darray is not None else 0
 
     def __contains__(self, item):
         ''' item of darray values'''
         return item in self.darray if self.darray is not None else None
 
     def __getitem__(self, ind):
@@ -130,14 +130,21 @@
         return str(self.ntvtype) if self.ntvtype else None
 
     @property
     def ndarray(self):
         '''representation with a np.ndarray not flattened'''
         return self.darray.reshape(self.shape) if not self.darray is None else None
 
+    def set_shape(self, shape):
+        '''update the shape'''
+        if Ndarray.len_shape(shape) != len(self.darray):
+            raise NdarrayError(
+                "shape is not consistent with the ndarray length")
+        self.shape = list(shape)
+
     def update(self, nda, nda_uri=True):
         '''update uri and darray and return the result (True, False)
 
         *Parameters*
 
         - **nda** : string, list, np.ndarray, Ndarray - data to include
         - **nda_uri** : boolean (default True) - if True, existing shape and
@@ -174,15 +181,15 @@
         new_shape = shape if self.shape is None else self.shape
         new_ntv_type = ntv_type if self.ntv_type is None else self.ntv_type
         if (len(darray) != Ndarray.len_shape(new_shape) or
                 new_ntv_type != ntv_type or new_shape != shape):
             return False
         self.uri = None
         self.darray = darray
-        self.ntvtype = Datatype(new_ntv_type)
+        self.ntvtype = Ndtype(new_ntv_type)
         self.shape = new_shape
         return True
 
     def set_uri(self, uri, no_ntv_type=False, no_shape=False):
         '''set a new uri and remove ndarray and optionaly ntv_type and shape.
         Return the result (True, False)
 
@@ -314,60 +321,30 @@
     - `nda_ntv_type`
     - `dtype`
     - `json_ntv`
     - `split_name`
     - `split_json_name`
 
     '''
-
-    DATATION_DT = {'date': 'datetime64[D]', 'year': 'datetime64[Y]',
-                   'yearmonth': 'datetime64[M]',
-                   'datetime': 'datetime64[s]', 'datetime[ms]': 'datetime64[ms]',
-                   'datetime[us]': 'datetime64[us]', 'datetime[ns]': 'datetime64[ns]',
-                   'datetime[ps]': 'datetime64[ps]', 'datetime[fs]': 'datetime64[fs]',
-                   'timedelta': 'timedelta64[s]', 'timedelta[ms]': 'timedelta64[ms]',
-                   'timedelta[us]': 'timedelta64[us]', 'timedelta[ns]': 'timedelta64[ns]',
-                   'timedelta[ps]': 'timedelta64[ps]', 'timedelta[fs]': 'timedelta64[fs]',
-                   'timedelta[D]': 'timedelta64[D]', 'timedelta[Y]': 'timedelta64[Y]',
-                   'timedelta[M]': 'timedelta64[M]'}
-    DT_DATATION = {val: key for key, val in DATATION_DT.items()}
-
-    # CONNECTOR_DT = {'field': 'Series', 'tab': 'DataFrame'}
     CONNECTOR_DT = {'field': 'Series', 'tab': 'DataFrame'}
-    DT_CONNECTOR = {val: key for key, val in CONNECTOR_DT.items()}
-
     PYTHON_DT = {'array': 'list', 'time': 'datetime.time',
                  'object': 'dict', 'null': 'NoneType', 'decimal64': 'Decimal',
                  'ndarray': 'ndarray', 'narray': 'narray'}
-    DT_PYTHON = {val: key for key, val in PYTHON_DT.items()}
-
-    # OTHER_DT = {'boolean': 'bool', 'string': 'str'}
-    OTHER_DT = {'boolean': 'bool', 'string': 'str', 'base16': 'bytes'}
-    DT_OTHER = {val: key for key, val in OTHER_DT.items()}
-
     LOCATION_DT = {'point': 'Point',
                    'line': 'LineString', 'polygon': 'Polygon'}
+    DT_CONNECTOR = {val: key for key, val in CONNECTOR_DT.items()}
+    DT_PYTHON = {val: key for key, val in PYTHON_DT.items()}
     DT_LOCATION = {val: key for key, val in LOCATION_DT.items()}
+    DT_NTVTYPE = DT_LOCATION | DT_CONNECTOR | DT_PYTHON
 
-    NUMBER_DT = {'json': 'object', 'number': None, 'month': 'int', 'day': 'int',
-                 'wday': 'int', 'yday': 'int', 'week': 'hour', 'minute': 'int',
-                 'second': 'int'}
-    # STRING_DT = {'base16': 'str', 'base32': 'str', 'base64': 'str',
-    STRING_DT = {'base32': 'str', 'base64': 'str',
-                 'period': 'str', 'duration': 'str', 'jpointer': 'str',
-                 'uri': 'str', 'uriref': 'str', 'iri': 'str', 'iriref': 'str',
-                 'email': 'str', 'regex': 'str', 'hostname': 'str', 'ipv4': 'str',
-                 'ipv6': 'str', 'file': 'str', 'geojson': 'str', }
     FORMAT_CLS = {'full': Dfull, 'complete': Dcomplete}
+    STRUCT_DT = {'Ntv': 'object', 'NtvSingle': 'object', 'NtvList': 'object'}
     CONVERT_DT = {'object': 'object', 'array': 'object', 'json': 'object',
                   'number': 'float', 'boolean': 'bool', 'null': 'object',
                   'string': 'str', 'integer': 'int'}
-    STRUCT_DT = {'Ntv': 'object', 'NtvSingle': 'object', 'NtvList': 'object'}
-
-    DT_NTVTYPE = DT_DATATION | DT_LOCATION | DT_OTHER | DT_CONNECTOR | DT_PYTHON
 
     @staticmethod
     def is_json(obj):
         ''' check if obj is a json structure and return True if obj is a json-value
 
         *Parameters*
 
@@ -388,68 +365,77 @@
                 if not min(isinstance(key, str) for key in obj.keys()):
                     return False
                 return min(is_js(obj_in) for obj_in in obj.values())
             case _:
                 return False
 
     @staticmethod
+    def extend_array(arr, til, shap, order):
+        '''return a flattened np.ndarray extended in additional dimensions
+
+        parameters:
+
+        - arr: np.array to extend
+        - til: integer - parameter to apply to np.tile function
+        - shap: list of integer - shape of the array
+        - order: list of integer - order of dimensions to apply
+        '''
+        old_order = list(range(len(order)))
+        arr_tab = np.tile(arr, til).reshape(shap)
+        return np.moveaxis(arr_tab, old_order, order).flatten()
+
+    @staticmethod
     def convert(ntv_type, nda, tojson=True, convert=True):
         ''' convert np.ndarray with external NTVtype.
 
         *Parameters*
 
         - **ntv_type** : string - NTVtype deduced from the np.ndarray name_type and dtype,
         - **nda** : np.ndarray to be converted.
         - **tojson** : boolean (default True) - apply to json function
         - **convert** : boolean (default True) - If True, convert json data with
         non Numpy ntv_type into data with python type
         '''
+
+        dtype = Nutil.dtype(ntv_type)
+        jtype = Nutil.dtype(ntv_type, convert=False)
         if tojson:
             match ntv_type:
-                case dat if dat in Nutil.DATATION_DT:
-                    return nda.astype(Nutil.DATATION_DT[dat]).astype(str)
-                case 'bytes':
-                    return nda.astype('bytes').astype(str)
-                case 'time':
-                    return nda.astype(str)
-                case 'decimal64':
-                    return nda.astype(float)
+                case dat if Ndtype(dat).category == 'datation':
+                    return nda.astype(dtype).astype(jtype)
+                case 'base16':
+                    return nda.astype(dtype)
+                case 'time' | 'decimal64':
+                    return nda.astype(jtype)
                 case 'geojson':
                     return np.frompyfunc(ShapelyConnec.to_geojson, 1, 1)(nda)
                 case _:
                     return nda
         else:
             match [ntv_type, convert]:
                 case [None, _]:
                     return nda
-                case [dat, _] if dat in Nutil.DATATION_DT:
-                    return nda.astype(Nutil.DATATION_DT[dat])
-                case [std, _] if std in Nutil.OTHER_DT:
-                    return nda.astype(Nutil.OTHER_DT[std])
-                case ['time', True]:
+                case [_, False]:
+                    return nda.astype(jtype)
+                case ['time', _]:
                     return np.frompyfunc(datetime.time.fromisoformat, 1, 1)(nda)
-                case ['decimal64', True]:
+                case ['decimal64', _]:
                     return np.frompyfunc(Decimal, 1, 1)(nda)
-                case ['narray', True]:
+                case ['narray', _]:
                     nar = np.frompyfunc(Ndarray.read_json, 1, 1)(nda)
                     return np.frompyfunc(Ndarray.to_ndarray, 1, 1)(nar)
-                case ['ndarray', True]:
+                case ['ndarray', _]:
                     return np.frompyfunc(Ndarray.read_json, 1, 1)(nda)
-                case [python, _] if python in Nutil.PYTHON_DT:
-                    return nda.astype('object')
-                case [connec, True] if connec in Nutil.CONNECTOR_DT:
+                case [('point' | 'line' | 'polygon' | 'geometry'), _]:
+                    return np.frompyfunc(ShapelyConnec.to_geometry, 1, 1)(nda)
+                case [connec, _] if connec in Nutil.CONNECTOR_DT:
                     return np.fromiter([NtvConnector.uncast(nd, None, connec)[0]
                                         for nd in nda], dtype='object')
-                case [('point' | 'line' | 'polygon' | 'geometry'), True]:
-                    return np.frompyfunc(ShapelyConnec.to_geometry, 1, 1)(nda)
-                case [_, False]:
-                    return nda.astype(Nutil.CONVERT_DT[
-                        Nutil.dtype(ntv_type, convert=False)])
                 case _:
-                    return nda.astype(Nutil.dtype(ntv_type))
+                    return nda.astype(dtype)
 
         # float.fromhex(x.hex()) == x, bytes(bytearray.fromhex(x.hex())) == x
     @staticmethod
     def ntv_val(ntv_type, nda, form, is_json=False):
         ''' convert a np.ndarray into NTV json-value.
 
         *Parameters*
@@ -469,15 +455,14 @@
         if is_json:
             return Format(darray.data, ref=ref, coding=coding).to_json()
         match ntv_type:
             case 'narray':
                 data = [Ndarray(nd).to_json(header=False)
                         for nd in darray.data]
             case 'ndarray':
-                # data = [Ndarray.to_json(nd) for nd in darray.data]
                 data = [Ndarray(nd).to_json(header=False)
                         for nd in darray.data]
             case connec if connec in Nutil.CONNECTOR_DT:
                 data = [NtvConnector.cast(nd, None, connec)[0]
                         for nd in darray.data]
             case 'point' | 'line' | 'polygon' | 'geometry':
                 data = np.frompyfunc(ShapelyConnec.to_coord, 1, 1)(darray.data)
@@ -485,15 +470,15 @@
                 data = nda
             case _:
                 data = Nutil.convert(ntv_type, darray.data)
         return Format(data, ref=ref, coding=coding).to_json()
 
     @staticmethod
     def add_ext(typ, ext):
-        '''return extended type : "typ[ext]"'''
+        '''return extended type string: "typ[ext]"'''
         ext = '[' + ext + ']' if ext else ''
         return '' if not typ else typ + ext
 
     @staticmethod
     def split_type(typ):
         '''return a tuple with typ and extension'''
         if not isinstance(typ, str):
@@ -522,71 +507,72 @@
             return ['', '']
         spl = string.split('.', maxsplit=1)
         spl = [spl[0], ''] if len(spl) < 2 else spl
         return spl
 
     @staticmethod
     def ntv_type(dtype, ntv_type=None, ext=None):
-        ''' return NTVtype from dtype, additional type and extension.
+        ''' return ntv_type string from dtype, additional type and extension.
 
         *Parameters*
 
         - **dtype** : string - dtype of the ndarray
         - **ntv_type** : string - additional type
         - **ext** : string - type extension
         '''
+        np_ntype = NP_NTYPE | Nutil.DT_NTVTYPE | {
+            'int': 'int', 'object': 'object'}
         if ntv_type:
             return Nutil.add_ext(ntv_type, ext)
         match dtype:
-            case dat if dat in Nutil.DT_NTVTYPE:
-                return Nutil.add_ext(Nutil.DT_NTVTYPE[dat], ext)
             case string if string[:3] == 'str':
                 return Nutil.add_ext('string', ext)
-            case byte if byte[:5] == 'bytes':
-                # return Nutil.add_ext('bytes', ext)
+            case bytesxx if bytesxx[:5] == 'bytes':
                 return Nutil.add_ext('base16', ext)
+            case dtyp if dtyp in np_ntype:
+                return Nutil.add_ext(np_ntype[dtyp], ext)
+            case date if date[:10] == 'datetime64':
+                return 'datetime' + date[10:]
+            case delta if delta[:11] == 'timedelta64':
+                return 'timedelta' + delta[11:]
             case _:
                 return Nutil.add_ext(dtype, ext)
 
     @staticmethod
     def nda_ntv_type(nda, ntv_type=None, ext=None):
-        '''return ntv_type from an ndarray, additional type and extension.
+        '''return ntv_type string from an ndarray, additional type and extension.
 
         *Parameters*
 
         - **nda** : ndarray - data used to calculate the ntv_type
         - **ntv_type** : string - additional type
         - **ext** : string - type extension
         '''
         if ntv_type or nda is None:
             return ntv_type
         dtype = nda.dtype.name
         pytype = nda.flat[0].__class__.__name__
         dtype = pytype if dtype == 'object' and not pytype in Nutil.STRUCT_DT else dtype
-        # dtype = pytype if dtype == 'object' and pytype in Nutil.DT_NTVTYPE else dtype
-        # dtype = nda.flat[0].__class__.__name__ if dtype == 'object' else dtype
         return Nutil.ntv_type(dtype, ntv_type, ext)
 
     @staticmethod
     def dtype(ntv_type, convert=True):
         ''' return dtype from ntv_type
 
         *parameters*
 
         - **convert** : boolean (default True) - if True, dtype if from converted data
         '''
-        DTYPE = (Nutil.DATATION_DT | Nutil.NUMBER_DT | Nutil.OTHER_DT |
-                 Nutil.STRING_DT)
-        OBJECT = Nutil.LOCATION_DT | Nutil.CONNECTOR_DT | Nutil.PYTHON_DT
-        type_base = Nutil.split_type(ntv_type)[0]
+        if not ntv_type:
+            return None
         if convert:
-            if type_base in OBJECT:
-                return 'object'
-            return DTYPE.get(ntv_type, DTYPE.get(type_base, type_base))
-        return Datatype(ntv_type).json_type
+            if ntv_type[:8] == 'datetime' and ntv_type[8:]:
+                return 'datetime64' + ntv_type[8:]
+            return Ndtype(ntv_type).dtype
+        return Nutil.CONVERT_DT[Ndtype(ntv_type).json_type]
 
     @staticmethod
     def json_ntv(ntv_name, ntv_type, ntv_value, **kwargs):
         ''' return the JSON representation of a NTV entity
 
         *parameters*
```

### Comparing `ntv_numpy-0.1.2/ntv_numpy/ntv_numpy.ini` & `ntv_numpy-0.2.0/ntv_numpy/ntv_numpy.ini`

 * *Files 5% similar despite different names*

```diff
@@ -18,299 +18,306 @@
 00000110: 6865 2064 7479 7065 206f 6620 7468 6520  he dtype of the 
 00000120: 6e64 6172 7261 792c 2069 6620 276e 756c  ndarray, if 'nul
 00000130: 6c27 204e 756d 5079 2063 686f 6f73 6520  l' NumPy choose 
 00000140: 7468 6520 6474 7970 650d 0a20 2020 2022  the dtype..    "
 00000150: 6474 7970 6522 5d0d 0a0d 0a23 2064 6566  dtype"]....# def
 00000160: 696e 6520 7468 6520 7479 7065 7320 7769  ine the types wi
 00000170: 7468 2061 204e 756d 5079 2063 6f6e 7665  th a NumPy conve
-00000180: 7273 696f 6e0d 0a74 7970 6520 2020 3d20  rsion..type   = 
-00000190: 5b0d 0a0d 0a20 2020 2023 2077 6974 686f  [....    # witho
-000001a0: 7574 206e 7476 5f74 7970 6520 0d0a 2020  ut ntv_type ..  
-000001b0: 2020 2320 2020 2020 6474 7970 6520 6973    #     dtype is
-000001c0: 203a 2027 696e 7478 7827 2c20 2766 6c6f   : 'intxx', 'flo
-000001d0: 6174 7878 272c 2027 626f 6f6c 6561 6e27  atxx', 'boolean'
-000001e0: 2c20 0d0a 2020 2020 2320 2020 2020 2020  , ..    #       
-000001f0: 2020 2020 2020 2020 206f 7220 276f 626a           or 'obj
-00000200: 6563 7427 2028 6a73 6f6e 2d61 7272 6179  ect' (json-array
-00000210: 2c20 6a73 6f6e 2d6f 626a 6563 7429 0d0a  , json-object)..
-00000220: 2020 2020 5b22 222c 0909 2020 2020 226a      ["",..    "j
-00000230: 736f 6e22 2c20 2020 2020 6e75 6c6c 2020  son",     null  
-00000240: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00000250: 0d0a 0d0a 2020 2020 2320 7769 7468 206e  ....    # with n
-00000260: 7476 5f74 7970 6520 6f6e 6c79 2069 6e20  tv_type only in 
-00000270: 6a73 6f6e 2064 6174 6120 286e 6f74 206e  json data (not n
-00000280: 756d 6265 7273 2920 2020 200d 0a20 2020  umbers)    ..   
-00000290: 205b 2264 6174 6522 2c09 2020 2020 6e75   ["date",.    nu
-000002a0: 6c6c 2c09 2020 2020 2264 6174 6574 696d  ll,.    "datetim
-000002b0: 6536 345b 445d 2220 2020 2020 5d2c 200d  e64[D]"     ], .
-000002c0: 0a20 2020 205b 2279 6561 726d 6f6e 7468  .    ["yearmonth
-000002d0: 222c 2020 206e 756c 6c2c 0920 2020 2022  ",   null,.    "
-000002e0: 6461 7465 7469 6d65 3634 5b4d 5d22 2020  datetime64[M]"  
-000002f0: 2020 205d 2c20 0d0a 2020 2020 5b22 7965     ], ..    ["ye
-00000300: 6172 222c 0920 2020 206e 756c 6c2c 0920  ar",.    null,. 
-00000310: 2020 2022 6461 7465 7469 6d65 3634 5b59     "datetime64[Y
-00000320: 5d22 2020 2020 205d 2c0d 0a20 2020 205b  ]"     ],..    [
-00000330: 2273 7472 696e 6722 2c09 2020 2020 6e75  "string",.    nu
-00000340: 6c6c 2c09 2020 2020 2273 7472 2220 2020  ll,.    "str"   
-00000350: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-00000360: 0d0a 2020 2020 2320 7769 7468 206e 7476  ..    # with ntv
-00000370: 5f74 7970 6520 6f6e 6c79 2069 6e20 6a73  _type only in js
-00000380: 6f6e 2064 6174 6120 616e 6420 7769 7468  on data and with
-00000390: 204e 5456 7479 7065 2065 7874 656e 7369   NTVtype extensi
-000003a0: 6f6e 2028 6e6f 7420 6e75 6d62 6572 7329  on (not numbers)
-000003b0: 2020 2020 0d0a 2020 2020 5b22 6461 7465      ..    ["date
-000003c0: 7469 6d65 222c 096e 756c 6c2c 0920 2020  time",.null,.   
-000003d0: 2022 6461 7465 7469 6d65 3634 2220 2020   "datetime64"   
-000003e0: 2020 2020 205d 2c0d 0a20 2020 205b 2274       ],..    ["t
-000003f0: 696d 6564 656c 7461 222c 096e 756c 6c2c  imedelta",.null,
-00000400: 0920 2020 2022 7469 6d65 6465 6c74 6136  .    "timedelta6
-00000410: 3422 2020 2020 2020 205d 2c0d 0a0d 0a20  4"       ],.... 
-00000420: 2020 2023 2077 6974 6820 6e74 765f 7479     # with ntv_ty
-00000430: 7065 206f 6e6c 7920 696e 206a 736f 6e20  pe only in json 
-00000440: 6461 7461 2028 6e75 6d62 6572 7320 616e  data (numbers an
-00000450: 6420 6279 7465 7329 2020 2020 0d0a 2020  d bytes)    ..  
-00000460: 2020 5b22 666c 6f61 7431 3622 2c09 2020    ["float16",.  
-00000470: 2020 6e75 6c6c 2c09 2020 2020 2266 6c6f    null,.    "flo
-00000480: 6174 3136 2220 2020 2020 2020 2020 2020  at16"           
-00000490: 5d2c 0d0a 2020 2020 5b22 666c 6f61 7433  ],..    ["float3
-000004a0: 3222 2c09 2020 2020 6e75 6c6c 2c09 2020  2",.    null,.  
-000004b0: 2020 2266 6c6f 6174 3332 2220 2020 2020    "float32"     
-000004c0: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-000004d0: 666c 6f61 7436 3422 2c09 2020 2020 6e75  float64",.    nu
-000004e0: 6c6c 2c09 2020 2020 2266 6c6f 6174 3634  ll,.    "float64
-000004f0: 2220 2020 2020 2020 2020 2020 5d2c 0d0a  "           ],..
-00000500: 2020 2020 5b22 666c 6f61 7439 3622 2c09      ["float96",.
-00000510: 2020 2020 6e75 6c6c 2c09 2020 2020 2266      null,.    "f
-00000520: 6c6f 6174 3936 2220 2020 2020 2020 2020  loat96"         
-00000530: 2020 5d2c 0d0a 2020 2020 5b22 666c 6f61    ],..    ["floa
-00000540: 7431 3238 222c 2020 2020 6e75 6c6c 2c09  t128",    null,.
-00000550: 2020 2020 2266 6c6f 6174 3132 3822 2020      "float128"  
-00000560: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00000570: 5b22 7569 6e74 3822 2c09 2020 2020 6e75  ["uint8",.    nu
-00000580: 6c6c 2c09 2020 2020 2275 696e 7438 2220  ll,.    "uint8" 
-00000590: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-000005a0: 2020 2020 5b22 7569 6e74 3136 222c 0920      ["uint16",. 
-000005b0: 2020 206e 756c 6c2c 0920 2020 2022 7569     null,.    "ui
-000005c0: 6e74 3136 2220 2020 2020 2020 2020 2020  nt16"           
-000005d0: 205d 2c0d 0a20 2020 205b 2275 696e 7433   ],..    ["uint3
-000005e0: 3222 2c09 2020 2020 6e75 6c6c 2c09 2020  2",.    null,.  
-000005f0: 2020 2275 696e 7433 3222 2020 2020 2020    "uint32"      
-00000600: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-00000610: 7569 6e74 3634 222c 0920 2020 206e 756c  uint64",.    nul
-00000620: 6c2c 2009 2020 2020 2275 696e 7436 3422  l, .    "uint64"
-00000630: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-00000640: 2020 2020 5b22 696e 7438 222c 0920 2020      ["int8",.   
-00000650: 206e 756c 6c2c 0920 2020 2022 696e 7438   null,.    "int8
-00000660: 2220 2020 2020 2020 2020 2020 2020 205d  "              ]
-00000670: 2c0d 0a20 2020 205b 2269 6e74 3136 222c  ,..    ["int16",
-00000680: 0920 2020 206e 756c 6c2c 0920 2020 2022  .    null,.    "
-00000690: 696e 7431 3622 2020 2020 2020 2020 2020  int16"          
-000006a0: 2020 205d 2c0d 0a20 2020 205b 2269 6e74     ],..    ["int
-000006b0: 3332 222c 0920 2020 206e 756c 6c2c 0920  32",.    null,. 
-000006c0: 2020 2022 696e 7433 3222 2020 2020 2020     "int32"      
-000006d0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-000006e0: 2269 6e74 3634 222c 2020 2020 2020 206e  "int64",       n
-000006f0: 756c 6c2c 2020 2009 2269 6e74 3634 2220  ull,   ."int64" 
-00000700: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-00000710: 2020 2020 5b22 626f 6f6c 6561 6e22 2c09      ["boolean",.
-00000720: 2020 2020 6e75 6c6c 2c20 2020 0922 626f      null,   ."bo
-00000730: 6f6c 2220 2020 2020 2020 2020 2020 2020  ol"             
-00000740: 205d 2c0d 0a20 2020 205b 2262 696e 6172   ],..    ["binar
-00000750: 7922 2c09 2020 2020 6e75 6c6c 2c20 2020  y",.    null,   
-00000760: 0922 6279 7465 7322 2020 2020 2020 2020  ."bytes"        
-00000770: 2020 2020 205d 2c0d 0a0d 0a20 2020 2023       ],....    #
-00000780: 2077 6974 6820 6e74 765f 7479 7065 2063   with ntv_type c
-00000790: 6f6e 7665 7274 6564 2069 6e20 6f62 6a65  onverted in obje
-000007a0: 6374 2064 7479 7065 2028 7374 616e 6461  ct dtype (standa
-000007b0: 7264 2070 7974 686f 6e20 7479 7065 290d  rd python type).
-000007c0: 0a20 2020 205b 2274 696d 6522 2c09 2020  .    ["time",.  
-000007d0: 2020 6e75 6c6c 2c09 2020 2020 226f 626a    null,.    "obj
-000007e0: 6563 7422 2020 2020 2020 2020 2020 2020  ect"            
-000007f0: 5d2c 0d0a 2020 2020 5b22 6172 7261 7922  ],..    ["array"
-00000800: 2c09 2020 2020 6e75 6c6c 2c09 2020 2020  ,.    null,.    
-00000810: 226f 626a 6563 7422 2020 2020 2020 2020  "object"        
-00000820: 2020 2020 5d2c 0d0a 2020 2020 5b22 6f62      ],..    ["ob
-00000830: 6a65 6374 222c 0920 2020 206e 756c 6c2c  ject",.    null,
-00000840: 0920 2020 2022 6f62 6a65 6374 2220 2020  .    "object"   
-00000850: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000860: 205b 226e 756c 6c22 2c09 2020 2020 6e75   ["null",.    nu
-00000870: 6c6c 2c20 0920 2020 2022 6f62 6a65 6374  ll, .    "object
-00000880: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
-00000890: 0a20 2020 205b 2264 6563 696d 616c 3634  .    ["decimal64
-000008a0: 222c 2020 206e 756c 6c2c 2009 2020 2020  ",   null, .    
-000008b0: 226f 626a 6563 7422 2020 2020 2020 2020  "object"        
-000008c0: 2020 2020 5d2c 0d0a 0d0a 2020 2020 2320      ],....    # 
-000008d0: 7769 7468 206e 7476 5f74 7970 6520 636f  with ntv_type co
-000008e0: 6e76 6572 7465 6420 696e 206f 626a 6563  nverted in objec
-000008f0: 7420 6474 7970 6520 2870 7974 686f 6e20  t dtype (python 
-00000900: 6f62 6a65 6374 2029 0d0a 2020 2020 5b22  object )..    ["
-00000910: 6e64 6172 7261 7922 2c20 2020 2020 6e75  ndarray",     nu
-00000920: 6c6c 2c20 0920 2020 2022 6f62 6a65 6374  ll, .    "object
-00000930: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
-00000940: 0a20 2020 205b 226e 7476 222c 0920 2020  .    ["ntv",.   
-00000950: 2020 2020 206e 756c 6c2c 0920 2020 2022       null,.    "
-00000960: 6f62 6a65 6374 2220 2020 2020 2020 2020  object"         
-00000970: 2020 205d 2c0d 0a20 2020 205b 2270 6f69     ],..    ["poi
-00000980: 6e74 222c 0920 2020 206e 756c 6c2c 2020  nt",.    null,  
-00000990: 2009 226f 626a 6563 7422 2020 2020 2020   ."object"      
-000009a0: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-000009b0: 6c69 6e65 222c 0920 2020 206e 756c 6c2c  line",.    null,
-000009c0: 0920 2020 2022 6f62 6a65 6374 2220 2020  .    "object"   
-000009d0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-000009e0: 205b 2270 6f6c 7967 6f6e 222c 0920 2020   ["polygon",.   
-000009f0: 206e 756c 6c2c 0920 2020 2022 6f62 6a65   null,.    "obje
-00000a00: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
-00000a10: 2c0d 0a20 2020 205b 2266 6965 6c64 222c  ,..    ["field",
-00000a20: 0920 2020 206e 756c 6c2c 0920 2020 2022  .    null,.    "
-00000a30: 6f62 6a65 6374 2220 2020 2020 2020 2020  object"         
-00000a40: 2020 205d 2c0d 0a20 2020 205b 2274 6162     ],..    ["tab
-00000a50: 222c 0920 2020 2020 2020 206e 756c 6c2c  ",.        null,
-00000a60: 0920 2020 2022 6f62 6a65 6374 2220 2020  .    "object"   
-00000a70: 2020 2020 2020 2020 205d 2c0d 0a0d 0a20           ],.... 
-00000a80: 2020 2023 2077 6974 6820 6e74 765f 7479     # with ntv_ty
-00000a90: 7065 2069 6e20 6164 645f 7479 7065 2061  pe in add_type a
-00000aa0: 6e64 2069 6e20 6a73 6f6e 2064 6174 6120  nd in json data 
-00000ab0: 286e 756d 6265 7273 290d 0a20 2020 205b  (numbers)..    [
-00000ac0: 226a 736f 6e22 2c09 2020 2020 226a 736f  "json",.    "jso
-00000ad0: 6e22 2c20 0922 6f62 6a65 6374 2220 2020  n", ."object"   
-00000ae0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000af0: 205b 226e 756d 6265 7222 2c09 2020 2020   ["number",.    
-00000b00: 226e 756d 6265 7222 2c09 6e75 6c6c 2020  "number",.null  
-00000b10: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00000b20: 0d0a 2020 2020 5b22 666c 6f61 7422 2c09  ..    ["float",.
-00000b30: 2020 2020 2266 6c6f 6174 222c 0922 666c      "float",."fl
-00000b40: 6f61 7422 2020 2020 2020 2020 2020 2020  oat"            
-00000b50: 205d 2c0d 0a20 2020 205b 2269 6e74 222c   ],..    ["int",
-00000b60: 0920 2020 2020 2020 2022 696e 7422 2c09  .        "int",.
-00000b70: 2020 2020 2269 6e74 2220 2020 2020 2020      "int"       
-00000b80: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00000b90: 5b22 6d6f 6e74 6822 2c09 2020 2020 226d  ["month",.    "m
-00000ba0: 6f6e 7468 222c 0922 696e 7422 2020 2020  onth",."int"    
-00000bb0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00000bc0: 2020 205b 2264 6179 222c 0920 2020 2020     ["day",.     
-00000bd0: 2020 2022 6461 7922 2c09 2020 2020 2269     "day",.    "i
-00000be0: 6e74 2220 2020 2020 2020 2020 2020 2020  nt"             
-00000bf0: 2020 5d2c 0d0a 2020 2020 5b22 7764 6179    ],..    ["wday
-00000c00: 222c 0920 2020 2022 7764 6179 222c 0920  ",.    "wday",. 
-00000c10: 2020 2022 696e 7422 2020 2020 2020 2020     "int"        
-00000c20: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-00000c30: 2279 6461 7922 2c09 2020 2020 2279 6461  "yday",.    "yda
-00000c40: 7922 2c09 2020 2020 2269 6e74 2220 2020  y",.    "int"   
-00000c50: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-00000c60: 2020 2020 5b22 7765 656b 222c 0920 2020      ["week",.   
-00000c70: 2022 7765 656b 222c 0920 2020 2022 696e   "week",.    "in
-00000c80: 7422 2020 2020 2020 2020 2020 2020 2020  t"              
-00000c90: 205d 2c0d 0a20 2020 205b 2268 6f75 7222   ],..    ["hour"
-00000ca0: 2c09 2020 2020 2268 6f75 7222 2c09 2020  ,.    "hour",.  
-00000cb0: 2020 2269 6e74 2220 2020 2020 2020 2020    "int"         
-00000cc0: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-00000cd0: 6d69 6e75 7465 222c 0920 2020 2022 6d69  minute",.    "mi
-00000ce0: 6e75 7465 222c 0922 696e 7422 2020 2020  nute",."int"    
-00000cf0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00000d00: 2020 205b 2273 6563 6f6e 6422 2c09 2020     ["second",.  
-00000d10: 2020 2273 6563 6f6e 6422 2c09 2269 6e74    "second",."int
-00000d20: 2220 2020 2020 2020 2020 2020 2020 2020  "               
-00000d30: 5d2c 2020 2020 0d0a 2020 2020 0d0a 2020  ],    ..    ..  
-00000d40: 2020 2320 7769 7468 206e 7476 5f74 7970    # with ntv_typ
-00000d50: 6520 696e 2061 6464 5f74 7970 6520 616e  e in add_type an
-00000d60: 6420 696e 206a 736f 6e20 6461 7461 2028  d in json data (
-00000d70: 6e6f 7420 6e75 6d62 6572 7329 0d0a 2020  not numbers)..  
-00000d80: 2020 5b22 6261 7365 3136 222c 0920 2020    ["base16",.   
-00000d90: 2022 6261 7365 3136 222c 0922 7374 7269   "base16",."stri
-00000da0: 6e67 2220 2020 2020 2020 2020 2020 205d  ng"            ]
-00000db0: 2c0d 0a20 2020 205b 2262 6173 6533 3222  ,..    ["base32"
-00000dc0: 2c09 2020 2020 2262 6173 6533 3222 2c09  ,.    "base32",.
-00000dd0: 2273 7472 696e 6722 2020 2020 2020 2020  "string"        
-00000de0: 2020 2020 5d2c 0d0a 2020 2020 5b22 6261      ],..    ["ba
-00000df0: 7365 3634 222c 0920 2020 2022 6261 7365  se64",.    "base
-00000e00: 3634 222c 0922 7374 7269 6e67 2220 2020  64",."string"   
-00000e10: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000e20: 205b 2270 6572 696f 6422 2c09 2020 2020   ["period",.    
-00000e30: 2270 6572 696f 6422 2c09 2273 7472 696e  "period",."strin
-00000e40: 6722 2020 2020 2020 2020 2020 2020 5d2c  g"            ],
-00000e50: 0d0a 2020 2020 5b22 6475 7261 7469 6f6e  ..    ["duration
-00000e60: 222c 2020 2020 2264 7572 6174 696f 6e22  ",    "duration"
-00000e70: 2c09 2273 7472 696e 6722 2020 2020 2020  ,."string"      
-00000e80: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-00000e90: 6a70 6f69 6e74 6572 222c 2020 2020 226a  jpointer",    "j
-00000ea0: 706f 696e 7465 7222 2c09 2273 7472 696e  pointer",."strin
-00000eb0: 6722 2020 2020 2020 2020 2020 2020 5d2c  g"            ],
-00000ec0: 0d0a 2020 2020 5b22 7572 6922 2c09 2020  ..    ["uri",.  
-00000ed0: 2020 2020 2020 2275 7269 222c 0920 2020        "uri",.   
-00000ee0: 2022 7374 7269 6e67 2220 2020 2020 2020   "string"       
-00000ef0: 2020 2020 205d 2c0d 0a20 2020 205b 2275       ],..    ["u
-00000f00: 7269 7265 6622 2c09 2020 2020 2275 7269  riref",.    "uri
-00000f10: 7265 6622 2c09 2273 7472 696e 6722 2020  ref",."string"  
-00000f20: 2020 2020 2020 2020 2020 5d2c 2020 2020            ],    
-00000f30: 0d0a 2020 2020 5b22 6972 6922 2c09 2020  ..    ["iri",.  
-00000f40: 2020 2020 2020 2269 7269 222c 0920 2020        "iri",.   
-00000f50: 2022 7374 7269 6e67 2220 2020 2020 2020   "string"       
-00000f60: 2020 2020 205d 2c0d 0a20 2020 205b 2269       ],..    ["i
-00000f70: 7269 7265 6622 2c09 2020 2020 2269 7269  riref",.    "iri
-00000f80: 7265 6622 2c09 2273 7472 696e 6722 2020  ref",."string"  
-00000f90: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00000fa0: 2020 5b22 656d 6169 6c22 2c09 2020 2020    ["email",.    
-00000fb0: 2265 6d61 696c 222c 0922 7374 7269 6e67  "email",."string
-00000fc0: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
-00000fd0: 0a20 2020 205b 2272 6567 6578 222c 0920  .    ["regex",. 
-00000fe0: 2020 2022 7265 6765 7822 2c09 2273 7472     "regex",."str
-00000ff0: 696e 6722 2020 2020 2020 2020 2020 2020  ing"            
-00001000: 5d2c 0d0a 2020 2020 5b22 686f 7374 6e61  ],..    ["hostna
-00001010: 6d65 222c 2020 2020 2268 6f73 746e 616d  me",    "hostnam
-00001020: 6522 2c09 2273 7472 696e 6722 2020 2020  e",."string"    
-00001030: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00001040: 5b22 6970 7634 222c 0920 2020 2022 6970  ["ipv4",.    "ip
-00001050: 7634 222c 0920 2020 2022 7374 7269 6e67  v4",.    "string
-00001060: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
-00001070: 0a20 2020 205b 2269 7076 3622 2c09 2020  .    ["ipv6",.  
-00001080: 2020 2269 7076 3622 2c09 2020 2020 2273    "ipv6",.    "s
-00001090: 7472 696e 6722 2020 2020 2020 2020 2020  tring"          
-000010a0: 2020 5d2c 0d0a 2020 2020 5b22 6669 6c65    ],..    ["file
-000010b0: 222c 0920 2020 2022 6669 6c65 222c 0920  ",.    "file",. 
-000010c0: 2020 2022 7374 7269 6e67 2220 2020 2020     "string"     
-000010d0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-000010e0: 2267 656f 6a73 6f6e 222c 0920 2020 2022  "geojson",.    "
-000010f0: 6765 6f6a 736f 6e22 2c09 2273 7472 696e  geojson",."strin
-00001100: 6722 2020 2020 2020 2020 2020 2020 5d2c  g"            ],
-00001110: 0d0a 2020 2020 0d0a 2020 2020 2320 7769  ..    ..    # wi
-00001120: 7468 206e 7476 5f74 7970 6520 636f 6e76  th ntv_type conv
-00001130: 6572 7465 6420 696e 206f 626a 6563 7420  erted in object 
-00001140: 6474 7970 6520 2870 7974 686f 6e20 7479  dtype (python ty
-00001150: 7065 290d 0a20 2020 205b 2267 656f 6d65  pe)..    ["geome
-00001160: 7472 7922 2c20 2020 2022 6765 6f6d 6574  try",    "geomet
-00001170: 7279 222c 0922 6f62 6a65 6374 2220 2020  ry",."object"   
-00001180: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00001190: 205b 2274 696d 6561 7272 6179 222c 0922   ["timearray",."
-000011a0: 7469 6d65 6172 7261 7922 2c22 6f62 6a65  timearray","obje
-000011b0: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
-000011c0: 0d0a 2020 2020 5d0d 0a0d 0a23 2064 6566  ..    ]....# def
-000011d0: 696e 6520 7468 6520 7479 7065 7320 7769  ine the types wi
-000011e0: 7468 2061 204e 5456 2063 6f6e 7665 7273  th a NTV convers
-000011f0: 696f 6e20 2827 6f74 6865 7274 7970 6527  ion ('othertype'
-00001200: 2069 7320 6e6f 7420 7573 6564 290d 0a6f   is not used)..o
-00001210: 7468 6572 7479 7065 203d 205b 0d0a 2020  thertype = [..  
-00001220: 2020 5b22 6461 7422 2c09 2020 2020 2020    ["dat",.      
-00001230: 2020 2020 2020 2264 6174 222c 0920 2020        "dat",.   
-00001240: 2020 2020 2022 6f62 6a65 6374 2220 2020       "object"   
-00001250: 205d 2c0d 0a20 2020 205b 226d 756c 7469   ],..    ["multi
-00001260: 706f 696e 7422 2c09 2020 2020 226d 756c  point",.    "mul
-00001270: 7469 706f 696e 7422 2c20 2020 226f 626a  tipoint",   "obj
-00001280: 6563 7422 2020 2020 5d2c 0d0a 2020 2020  ect"    ],..    
-00001290: 5b22 6d75 6c74 696c 696e 6522 2c09 2020  ["multiline",.  
-000012a0: 2020 226d 756c 7469 6c69 6e65 222c 2020    "multiline",  
-000012b0: 2020 226f 626a 6563 7422 2020 2020 5d2c    "object"    ],
-000012c0: 0d0a 2020 2020 5b22 6d75 6c74 6970 6f6c  ..    ["multipol
-000012d0: 7967 6f6e 222c 0922 6d75 6c74 6970 6f6c  ygon",."multipol
-000012e0: 7967 6f6e 222c 0922 6f62 6a65 6374 2220  ygon",."object" 
-000012f0: 2020 205d 2c0d 0a20 2020 205b 2262 6f78     ],..    ["box
-00001300: 222c 0920 2020 2020 2020 2020 2020 2022  ",.            "
-00001310: 626f 7822 2c09 2020 2020 2020 2020 226f  box",.        "o
-00001320: 626a 6563 7422 2020 2020 5d2c 0d0a 2020  bject"    ],..  
-00001330: 2020 5b22 636f 6465 6f6c 6322 2c09 2020    ["codeolc",.  
-00001340: 2020 2020 2020 2263 6f64 656f 6c63 222c        "codeolc",
-00001350: 0920 2020 2022 6f62 6a65 6374 2220 2020  .    "object"   
-00001360: 205d 2c0d 0a20 2020 205b 2272 6f77 222c   ],..    ["row",
-00001370: 0920 2020 2020 2020 2020 2020 2022 726f  .            "ro
-00001380: 7722 2c09 2020 2020 2020 2020 226f 626a  w",.        "obj
-00001390: 6563 7422 2020 2020 5d0d 0a20 2020 205d  ect"    ]..    ]
-000013a0: 0d0a 0d0a 2320 7265 706c 6163 6520 285c  ....# replace (\
-000013b0: 772b 2920 2d3e 2022 2431 222c 0d0a       w+) -> "$1",..
+00000180: 7273 696f 6e0d 0a74 7970 6573 2020 203d  rsion..types   =
+00000190: 205b 0d0a 0d0a 2020 2020 2320 7769 7468   [....    # with
+000001a0: 6f75 7420 6e74 765f 7479 7065 200d 0a20  out ntv_type .. 
+000001b0: 2020 2023 2020 2020 2064 7479 7065 2069     #     dtype i
+000001c0: 7320 3a20 2769 6e74 7878 272c 2027 666c  s : 'intxx', 'fl
+000001d0: 6f61 7478 7827 2c20 2762 6f6f 6c65 616e  oatxx', 'boolean
+000001e0: 272c 200d 0a20 2020 2023 2020 2020 2020  ', ..    #      
+000001f0: 2020 2020 2020 2020 2020 6f72 2027 6f62            or 'ob
+00000200: 6a65 6374 2720 286a 736f 6e2d 6172 7261  ject' (json-arra
+00000210: 792c 206a 736f 6e2d 6f62 6a65 6374 290d  y, json-object).
+00000220: 0a20 2020 205b 2222 2c09 0920 2020 2022  .    ["",..    "
+00000230: 6a73 6f6e 222c 2020 2020 206e 756c 6c20  json",     null 
+00000240: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00000250: 2c0d 0a0d 0a20 2020 2023 2077 6974 6820  ,....    # with 
+00000260: 6e74 765f 7479 7065 206f 6e6c 7920 696e  ntv_type only in
+00000270: 206a 736f 6e20 6461 7461 2028 6e6f 7420   json data (not 
+00000280: 6e75 6d62 6572 7329 2020 2020 0d0a 2020  numbers)    ..  
+00000290: 2020 5b22 6461 7465 222c 0920 2020 206e    ["date",.    n
+000002a0: 756c 6c2c 0920 2020 2022 6461 7465 7469  ull,.    "dateti
+000002b0: 6d65 3634 5b44 5d22 2020 2020 205d 2c20  me64[D]"     ], 
+000002c0: 0d0a 2020 2020 5b22 7965 6172 6d6f 6e74  ..    ["yearmont
+000002d0: 6822 2c20 2020 6e75 6c6c 2c09 2020 2020  h",   null,.    
+000002e0: 2264 6174 6574 696d 6536 345b 4d5d 2220  "datetime64[M]" 
+000002f0: 2020 2020 5d2c 200d 0a20 2020 205b 2279      ], ..    ["y
+00000300: 6561 7222 2c09 2020 2020 6e75 6c6c 2c09  ear",.    null,.
+00000310: 2020 2020 2264 6174 6574 696d 6536 345b      "datetime64[
+00000320: 595d 2220 2020 2020 5d2c 0d0a 2020 2020  Y]"     ],..    
+00000330: 5b22 7374 7269 6e67 222c 0920 2020 206e  ["string",.    n
+00000340: 756c 6c2c 0920 2020 2022 7374 7222 2020  ull,.    "str"  
+00000350: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00000360: 0a0d 0a20 2020 2023 2077 6974 6820 6e74  ...    # with nt
+00000370: 765f 7479 7065 206f 6e6c 7920 696e 206a  v_type only in j
+00000380: 736f 6e20 6461 7461 2061 6e64 2077 6974  son data and wit
+00000390: 6820 4e54 5674 7970 6520 6578 7465 6e73  h NTVtype extens
+000003a0: 696f 6e20 286e 6f74 206e 756d 6265 7273  ion (not numbers
+000003b0: 2920 2020 200d 0a20 2020 205b 2264 6174  )    ..    ["dat
+000003c0: 6574 696d 6522 2c09 6e75 6c6c 2c09 2020  etime",.null,.  
+000003d0: 2020 2264 6174 6574 696d 6536 345b 735d    "datetime64[s]
+000003e0: 2220 2020 2020 5d2c 0d0a 2020 2020 5b22  "     ],..    ["
+000003f0: 7469 6d65 6465 6c74 6122 2c09 6e75 6c6c  timedelta",.null
+00000400: 2c09 2020 2020 2274 696d 6564 656c 7461  ,.    "timedelta
+00000410: 3634 5b73 5d22 2020 2020 5d2c 0d0a 0d0a  64[s]"    ],....
+00000420: 2020 2020 2320 7769 7468 206e 7476 5f74      # with ntv_t
+00000430: 7970 6520 6f6e 6c79 2069 6e20 6a73 6f6e  ype only in json
+00000440: 2064 6174 6120 286e 756d 6265 7273 2061   data (numbers a
+00000450: 6e64 2062 7974 6573 2920 2020 200d 0a20  nd bytes)    .. 
+00000460: 2020 205b 2266 6c6f 6174 3136 222c 0920     ["float16",. 
+00000470: 2020 206e 756c 6c2c 0920 2020 2022 666c     null,.    "fl
+00000480: 6f61 7431 3622 2020 2020 2020 2020 2020  oat16"          
+00000490: 205d 2c0d 0a20 2020 205b 2266 6c6f 6174   ],..    ["float
+000004a0: 3332 222c 0920 2020 206e 756c 6c2c 0920  32",.    null,. 
+000004b0: 2020 2022 666c 6f61 7433 3222 2020 2020     "float32"    
+000004c0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+000004d0: 2266 6c6f 6174 3634 222c 0920 2020 206e  "float64",.    n
+000004e0: 756c 6c2c 0920 2020 2022 666c 6f61 7436  ull,.    "float6
+000004f0: 3422 2020 2020 2020 2020 2020 205d 2c0d  4"           ],.
+00000500: 0a20 2020 205b 2266 6c6f 6174 3936 222c  .    ["float96",
+00000510: 0920 2020 206e 756c 6c2c 0920 2020 2022  .    null,.    "
+00000520: 666c 6f61 7439 3622 2020 2020 2020 2020  float96"        
+00000530: 2020 205d 2c0d 0a20 2020 205b 2266 6c6f     ],..    ["flo
+00000540: 6174 3132 3822 2c20 2020 206e 756c 6c2c  at128",    null,
+00000550: 0920 2020 2022 666c 6f61 7431 3238 2220  .    "float128" 
+00000560: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00000570: 205b 2275 696e 7438 222c 0920 2020 206e   ["uint8",.    n
+00000580: 756c 6c2c 0920 2020 2022 7569 6e74 3822  ull,.    "uint8"
+00000590: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+000005a0: 0a20 2020 205b 2275 696e 7431 3622 2c09  .    ["uint16",.
+000005b0: 2020 2020 6e75 6c6c 2c09 2020 2020 2275      null,.    "u
+000005c0: 696e 7431 3622 2020 2020 2020 2020 2020  int16"          
+000005d0: 2020 5d2c 0d0a 2020 2020 5b22 7569 6e74    ],..    ["uint
+000005e0: 3332 222c 0920 2020 206e 756c 6c2c 0920  32",.    null,. 
+000005f0: 2020 2022 7569 6e74 3332 2220 2020 2020     "uint32"     
+00000600: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00000610: 2275 696e 7436 3422 2c09 2020 2020 6e75  "uint64",.    nu
+00000620: 6c6c 2c20 0920 2020 2022 7569 6e74 3634  ll, .    "uint64
+00000630: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
+00000640: 0a20 2020 205b 2269 6e74 3822 2c09 2020  .    ["int8",.  
+00000650: 2020 6e75 6c6c 2c09 2020 2020 2269 6e74    null,.    "int
+00000660: 3822 2020 2020 2020 2020 2020 2020 2020  8"              
+00000670: 5d2c 0d0a 2020 2020 5b22 696e 7431 3622  ],..    ["int16"
+00000680: 2c09 2020 2020 6e75 6c6c 2c09 2020 2020  ,.    null,.    
+00000690: 2269 6e74 3136 2220 2020 2020 2020 2020  "int16"         
+000006a0: 2020 2020 5d2c 0d0a 2020 2020 5b22 696e      ],..    ["in
+000006b0: 7433 3222 2c09 2020 2020 6e75 6c6c 2c09  t32",.    null,.
+000006c0: 2020 2020 2269 6e74 3332 2220 2020 2020      "int32"     
+000006d0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+000006e0: 5b22 696e 7436 3422 2c20 2020 2020 2020  ["int64",       
+000006f0: 6e75 6c6c 2c20 2020 0922 696e 7436 3422  null,   ."int64"
+00000700: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00000710: 0a20 2020 205b 2262 6f6f 6c65 616e 222c  .    ["boolean",
+00000720: 0920 2020 206e 756c 6c2c 2020 2009 2262  .    null,   ."b
+00000730: 6f6f 6c22 2020 2020 2020 2020 2020 2020  ool"            
+00000740: 2020 5d2c 0d0a 2020 2020 5b22 6261 7365    ],..    ["base
+00000750: 3136 222c 0920 2020 206e 756c 6c2c 2020  16",.    null,  
+00000760: 2009 2262 7974 6573 2220 2020 2020 2020   ."bytes"       
+00000770: 2020 2020 2020 5d2c 0d0a 0d0a 2020 2020        ],....    
+00000780: 2320 7769 7468 206e 7476 5f74 7970 6520  # with ntv_type 
+00000790: 636f 6e76 6572 7465 6420 696e 206f 626a  converted in obj
+000007a0: 6563 7420 6474 7970 6520 2873 7461 6e64  ect dtype (stand
+000007b0: 6172 6420 7079 7468 6f6e 2074 7970 6529  ard python type)
+000007c0: 0d0a 2020 2020 5b22 7469 6d65 222c 0920  ..    ["time",. 
+000007d0: 2020 206e 756c 6c2c 0920 2020 2022 6f62     null,.    "ob
+000007e0: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
+000007f0: 205d 2c0d 0a20 2020 205b 2261 7272 6179   ],..    ["array
+00000800: 222c 0920 2020 206e 756c 6c2c 0920 2020  ",.    null,.   
+00000810: 2022 6f62 6a65 6374 2220 2020 2020 2020   "object"       
+00000820: 2020 2020 205d 2c0d 0a20 2020 205b 226f       ],..    ["o
+00000830: 626a 6563 7422 2c09 2020 2020 6e75 6c6c  bject",.    null
+00000840: 2c09 2020 2020 226f 626a 6563 7422 2020  ,.    "object"  
+00000850: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+00000860: 2020 5b22 6e75 6c6c 222c 0920 2020 206e    ["null",.    n
+00000870: 756c 6c2c 2009 2020 2020 226f 626a 6563  ull, .    "objec
+00000880: 7422 2020 2020 2020 2020 2020 2020 5d2c  t"            ],
+00000890: 0d0a 2020 2020 5b22 6465 6369 6d61 6c36  ..    ["decimal6
+000008a0: 3422 2c20 2020 6e75 6c6c 2c20 0920 2020  4",   null, .   
+000008b0: 2022 6f62 6a65 6374 2220 2020 2020 2020   "object"       
+000008c0: 2020 2020 205d 2c0d 0a0d 0a20 2020 2023       ],....    #
+000008d0: 2077 6974 6820 6e74 765f 7479 7065 2063   with ntv_type c
+000008e0: 6f6e 7665 7274 6564 2069 6e20 6f62 6a65  onverted in obje
+000008f0: 6374 2064 7479 7065 2028 7079 7468 6f6e  ct dtype (python
+00000900: 206f 626a 6563 7420 290d 0a20 2020 205b   object )..    [
+00000910: 226e 6461 7272 6179 222c 2020 2020 206e  "ndarray",     n
+00000920: 756c 6c2c 2009 2020 2020 226f 626a 6563  ull, .    "objec
+00000930: 7422 2020 2020 2020 2020 2020 2020 5d2c  t"            ],
+00000940: 0d0a 2020 2020 5b22 6e61 7272 6179 222c  ..    ["narray",
+00000950: 2020 2020 2020 6e75 6c6c 2c20 0920 2020        null, .   
+00000960: 2022 6f62 6a65 6374 2220 2020 2020 2020   "object"       
+00000970: 2020 2020 205d 2c0d 0a20 2020 205b 226e       ],..    ["n
+00000980: 7476 222c 0920 2020 2020 2020 206e 756c  tv",.        nul
+00000990: 6c2c 0920 2020 2022 6f62 6a65 6374 2220  l,.    "object" 
+000009a0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+000009b0: 2020 205b 2270 6f69 6e74 222c 0920 2020     ["point",.   
+000009c0: 206e 756c 6c2c 2020 2009 226f 626a 6563   null,   ."objec
+000009d0: 7422 2020 2020 2020 2020 2020 2020 5d2c  t"            ],
+000009e0: 0d0a 2020 2020 5b22 6c69 6e65 222c 0920  ..    ["line",. 
+000009f0: 2020 206e 756c 6c2c 0920 2020 2022 6f62     null,.    "ob
+00000a00: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
+00000a10: 205d 2c0d 0a20 2020 205b 2270 6f6c 7967   ],..    ["polyg
+00000a20: 6f6e 222c 0920 2020 206e 756c 6c2c 0920  on",.    null,. 
+00000a30: 2020 2022 6f62 6a65 6374 2220 2020 2020     "object"     
+00000a40: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00000a50: 2266 6965 6c64 222c 0920 2020 206e 756c  "field",.    nul
+00000a60: 6c2c 0920 2020 2022 6f62 6a65 6374 2220  l,.    "object" 
+00000a70: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00000a80: 2020 205b 2274 6162 222c 0920 2020 2020     ["tab",.     
+00000a90: 2020 206e 756c 6c2c 0920 2020 2022 6f62     null,.    "ob
+00000aa0: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
+00000ab0: 205d 2c0d 0a0d 0a20 2020 2023 2077 6974   ],....    # wit
+00000ac0: 6820 6e74 765f 7479 7065 2069 6e20 6164  h ntv_type in ad
+00000ad0: 645f 7479 7065 2061 6e64 2069 6e20 6a73  d_type and in js
+00000ae0: 6f6e 2064 6174 6120 286e 756d 6265 7273  on data (numbers
+00000af0: 290d 0a20 2020 205b 226a 736f 6e22 2c09  )..    ["json",.
+00000b00: 2020 2020 226a 736f 6e22 2c20 0922 6f62      "json", ."ob
+00000b10: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
+00000b20: 205d 2c0d 0a20 2020 205b 226e 756d 6265   ],..    ["numbe
+00000b30: 7222 2c09 2020 2020 226e 756d 6265 7222  r",.    "number"
+00000b40: 2c09 6e75 6c6c 2020 2020 2020 2020 2020  ,.null          
+00000b50: 2020 2020 2020 5d2c 0d0a 2020 2020 235b        ],..    #[
+00000b60: 226e 756d 6265 7222 2c09 2020 2020 226e  "number",.    "n
+00000b70: 756d 6265 7222 2c09 226f 626a 6563 7422  umber",."object"
+00000b80: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
+00000b90: 2020 2020 5b22 666c 6f61 7422 2c09 2020      ["float",.  
+00000ba0: 2020 2266 6c6f 6174 222c 0922 666c 6f61    "float",."floa
+00000bb0: 7422 2020 2020 2020 2020 2020 2020 205d  t"             ]
+00000bc0: 2c0d 0a20 2020 205b 2269 6e74 222c 0920  ,..    ["int",. 
+00000bd0: 2020 2020 2020 2022 696e 7422 2c09 2020         "int",.  
+00000be0: 2020 2269 6e74 2220 2020 2020 2020 2020    "int"         
+00000bf0: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000c00: 6d6f 6e74 6822 2c09 2020 2020 226d 6f6e  month",.    "mon
+00000c10: 7468 222c 0922 696e 7422 2020 2020 2020  th",."int"      
+00000c20: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00000c30: 205b 2264 6179 222c 0920 2020 2020 2020   ["day",.       
+00000c40: 2022 6461 7922 2c09 2020 2020 2269 6e74   "day",.    "int
+00000c50: 2220 2020 2020 2020 2020 2020 2020 2020  "               
+00000c60: 5d2c 0d0a 2020 2020 5b22 7764 6179 222c  ],..    ["wday",
+00000c70: 0920 2020 2022 7764 6179 222c 0920 2020  .    "wday",.   
+00000c80: 2022 696e 7422 2020 2020 2020 2020 2020   "int"          
+00000c90: 2020 2020 205d 2c0d 0a20 2020 205b 2279       ],..    ["y
+00000ca0: 6461 7922 2c09 2020 2020 2279 6461 7922  day",.    "yday"
+00000cb0: 2c09 2020 2020 2269 6e74 2220 2020 2020  ,.    "int"     
+00000cc0: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+00000cd0: 2020 5b22 7765 656b 222c 0920 2020 2022    ["week",.    "
+00000ce0: 7765 656b 222c 0920 2020 2022 696e 7422  week",.    "int"
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00000d00: 2c0d 0a20 2020 205b 2268 6f75 7222 2c09  ,..    ["hour",.
+00000d10: 2020 2020 2268 6f75 7222 2c09 2020 2020      "hour",.    
+00000d20: 2269 6e74 2220 2020 2020 2020 2020 2020  "int"           
+00000d30: 2020 2020 5d2c 0d0a 2020 2020 5b22 6d69      ],..    ["mi
+00000d40: 6e75 7465 222c 0920 2020 2022 6d69 6e75  nute",.    "minu
+00000d50: 7465 222c 0922 696e 7422 2020 2020 2020  te",."int"      
+00000d60: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00000d70: 205b 2273 6563 6f6e 6422 2c09 2020 2020   ["second",.    
+00000d80: 2273 6563 6f6e 6422 2c09 2269 6e74 2220  "second",."int" 
+00000d90: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00000da0: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+00000db0: 2320 7769 7468 206e 7476 5f74 7970 6520  # with ntv_type 
+00000dc0: 696e 2061 6464 5f74 7970 6520 616e 6420  in add_type and 
+00000dd0: 696e 206a 736f 6e20 6461 7461 2028 6e6f  in json data (no
+00000de0: 7420 6e75 6d62 6572 7329 0d0a 2020 2020  t numbers)..    
+00000df0: 5b22 6269 6e61 7279 222c 0920 2020 2022  ["binary",.    "
+00000e00: 6269 6e61 7279 222c 2020 0922 7374 7222  binary",  ."str"
+00000e10: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00000e20: 2c0d 0a20 2020 205b 2262 6173 6533 3222  ,..    ["base32"
+00000e30: 2c09 2020 2020 2262 6173 6533 3222 2c09  ,.    "base32",.
+00000e40: 2273 7472 2220 2020 2020 2020 2020 2020  "str"           
+00000e50: 2020 2020 5d2c 0d0a 2020 2020 5b22 6261      ],..    ["ba
+00000e60: 7365 3634 222c 0920 2020 2022 6261 7365  se64",.    "base
+00000e70: 3634 222c 0922 7374 7222 2020 2020 2020  64",."str"      
+00000e80: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00000e90: 205b 2270 6572 696f 6422 2c09 2020 2020   ["period",.    
+00000ea0: 2270 6572 696f 6422 2c09 2273 7472 2220  "period",."str" 
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00000ec0: 0d0a 2020 2020 5b22 6475 7261 7469 6f6e  ..    ["duration
+00000ed0: 222c 2020 2020 2264 7572 6174 696f 6e22  ",    "duration"
+00000ee0: 2c09 2273 7472 2220 2020 2020 2020 2020  ,."str"         
+00000ef0: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000f00: 6a70 6f69 6e74 6572 222c 2020 2020 226a  jpointer",    "j
+00000f10: 706f 696e 7465 7222 2c09 2273 7472 2220  pointer",."str" 
+00000f20: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00000f30: 0d0a 2020 2020 5b22 7572 6922 2c09 2020  ..    ["uri",.  
+00000f40: 2020 2020 2020 2275 7269 222c 0920 2020        "uri",.   
+00000f50: 2022 7374 7222 2020 2020 2020 2020 2020   "str"          
+00000f60: 2020 2020 205d 2c0d 0a20 2020 205b 2275       ],..    ["u
+00000f70: 7269 7265 6622 2c09 2020 2020 2275 7269  riref",.    "uri
+00000f80: 7265 6622 2c09 2273 7472 2220 2020 2020  ref",."str"     
+00000f90: 2020 2020 2020 2020 2020 5d2c 2020 2020            ],    
+00000fa0: 0d0a 2020 2020 5b22 6972 6922 2c09 2020  ..    ["iri",.  
+00000fb0: 2020 2020 2020 2269 7269 222c 0920 2020        "iri",.   
+00000fc0: 2022 7374 7222 2020 2020 2020 2020 2020   "str"          
+00000fd0: 2020 2020 205d 2c0d 0a20 2020 205b 2269       ],..    ["i
+00000fe0: 7269 7265 6622 2c09 2020 2020 2269 7269  riref",.    "iri
+00000ff0: 7265 6622 2c09 2273 7472 2220 2020 2020  ref",."str"     
+00001000: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+00001010: 2020 5b22 656d 6169 6c22 2c09 2020 2020    ["email",.    
+00001020: 2265 6d61 696c 222c 0922 7374 7222 2020  "email",."str"  
+00001030: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00001040: 0a20 2020 205b 2272 6567 6578 222c 0920  .    ["regex",. 
+00001050: 2020 2022 7265 6765 7822 2c09 2273 7472     "regex",."str
+00001060: 2220 2020 2020 2020 2020 2020 2020 2020  "               
+00001070: 5d2c 0d0a 2020 2020 5b22 686f 7374 6e61  ],..    ["hostna
+00001080: 6d65 222c 2020 2020 2268 6f73 746e 616d  me",    "hostnam
+00001090: 6522 2c09 2273 7472 2220 2020 2020 2020  e",."str"       
+000010a0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+000010b0: 5b22 6970 7634 222c 0920 2020 2022 6970  ["ipv4",.    "ip
+000010c0: 7634 222c 0920 2020 2022 7374 7222 2020  v4",.    "str"  
+000010d0: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+000010e0: 0a20 2020 205b 2269 7076 3622 2c09 2020  .    ["ipv6",.  
+000010f0: 2020 2269 7076 3622 2c09 2020 2020 2273    "ipv6",.    "s
+00001100: 7472 2220 2020 2020 2020 2020 2020 2020  tr"             
+00001110: 2020 5d2c 0d0a 2020 2020 5b22 6669 6c65    ],..    ["file
+00001120: 222c 0920 2020 2022 6669 6c65 222c 0920  ",.    "file",. 
+00001130: 2020 2022 7374 7222 2020 2020 2020 2020     "str"        
+00001140: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00001150: 2267 656f 6a73 6f6e 222c 0920 2020 2022  "geojson",.    "
+00001160: 6765 6f6a 736f 6e22 2c09 2273 7472 2220  geojson",."str" 
+00001170: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00001180: 0d0a 2020 2020 0d0a 2020 2020 2320 7769  ..    ..    # wi
+00001190: 7468 206e 7476 5f74 7970 6520 636f 6e76  th ntv_type conv
+000011a0: 6572 7465 6420 696e 206f 626a 6563 7420  erted in object 
+000011b0: 6474 7970 6520 2870 7974 686f 6e20 7479  dtype (python ty
+000011c0: 7065 290d 0a20 2020 205b 2267 656f 6d65  pe)..    ["geome
+000011d0: 7472 7922 2c20 2020 2022 6765 6f6d 6574  try",    "geomet
+000011e0: 7279 222c 0922 6f62 6a65 6374 2220 2020  ry",."object"   
+000011f0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+00001200: 205b 2274 696d 6561 7272 6179 222c 0922   ["timearray",."
+00001210: 7469 6d65 6172 7261 7922 2c22 6f62 6a65  timearray","obje
+00001220: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
+00001230: 0d0a 2020 2020 5d0d 0a0d 0a23 2064 6566  ..    ]....# def
+00001240: 696e 6520 7468 6520 7479 7065 7320 7769  ine the types wi
+00001250: 7468 2061 204e 5456 2063 6f6e 7665 7273  th a NTV convers
+00001260: 696f 6e20 2827 6f74 6865 7274 7970 6527  ion ('othertype'
+00001270: 2069 7320 6e6f 7420 7573 6564 290d 0a6f   is not used)..o
+00001280: 7468 6572 7479 7065 203d 205b 0d0a 2020  thertype = [..  
+00001290: 2020 5b22 6461 7422 2c09 2020 2020 2020    ["dat",.      
+000012a0: 2020 2020 2020 2264 6174 222c 0920 2020        "dat",.   
+000012b0: 2020 2020 2022 6f62 6a65 6374 2220 2020       "object"   
+000012c0: 205d 2c0d 0a20 2020 205b 226d 756c 7469   ],..    ["multi
+000012d0: 706f 696e 7422 2c09 2020 2020 226d 756c  point",.    "mul
+000012e0: 7469 706f 696e 7422 2c20 2020 226f 626a  tipoint",   "obj
+000012f0: 6563 7422 2020 2020 5d2c 0d0a 2020 2020  ect"    ],..    
+00001300: 5b22 6d75 6c74 696c 696e 6522 2c09 2020  ["multiline",.  
+00001310: 2020 226d 756c 7469 6c69 6e65 222c 2020    "multiline",  
+00001320: 2020 226f 626a 6563 7422 2020 2020 5d2c    "object"    ],
+00001330: 0d0a 2020 2020 5b22 6d75 6c74 6970 6f6c  ..    ["multipol
+00001340: 7967 6f6e 222c 0922 6d75 6c74 6970 6f6c  ygon",."multipol
+00001350: 7967 6f6e 222c 0922 6f62 6a65 6374 2220  ygon",."object" 
+00001360: 2020 205d 2c0d 0a20 2020 205b 2262 6f78     ],..    ["box
+00001370: 222c 0920 2020 2020 2020 2020 2020 2022  ",.            "
+00001380: 626f 7822 2c09 2020 2020 2020 2020 226f  box",.        "o
+00001390: 626a 6563 7422 2020 2020 5d2c 0d0a 2020  bject"    ],..  
+000013a0: 2020 5b22 636f 6465 6f6c 6322 2c09 2020    ["codeolc",.  
+000013b0: 2020 2020 2020 2263 6f64 656f 6c63 222c        "codeolc",
+000013c0: 0920 2020 2022 6f62 6a65 6374 2220 2020  .    "object"   
+000013d0: 205d 2c0d 0a20 2020 205b 2272 6f77 222c   ],..    ["row",
+000013e0: 0920 2020 2020 2020 2020 2020 2022 726f  .            "ro
+000013f0: 7722 2c09 2020 2020 2020 2020 226f 626a  w",.        "obj
+00001400: 6563 7422 2020 2020 5d0d 0a20 2020 205d  ect"    ]..    ]
+00001410: 0d0a 0d0a 2320 7265 706c 6163 6520 285c  ....# replace (\
+00001420: 772b 2920 2d3e 2022 2431 222c 0d0a       w+) -> "$1",..
```

### Comparing `ntv_numpy-0.1.2/ntv_numpy/xdataset.py` & `ntv_numpy-0.2.0/ntv_numpy/xdataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 # -*- coding: utf-8 -*-
 """
-Created on Thu Mar  7 09:56:11 2024
+@author: Philippe@loco-labs.io
 
-@author: a lab in the Air
+The `xdataset` module is part of the `ntv-numpy.ntv_numpy` package ([specification document](
+https://loco-philippe.github.io/ES/JSON%20semantic%20format%20(JSON-NTV).htm)).
+
+It contains the classes `Xdataset`, `XdatasetInterface`, `XdatasetCategory` for 
+the multidimensional dataset.
+
+For more information, see the
+[user guide](https://loco-philippe.github.io/ntv-numpy/docs/user_guide.html)
+ or the [github repository](https://github.com/loco-philippe/ntv-numpy).
 """
 from abc import ABC, abstractmethod
 import json
+import pprint
 from json_ntv import Ntv
 from ntv_numpy.ndarray import Nutil
 from ntv_numpy.xndarray import Xndarray
 from ntv_numpy.xconnector import XarrayConnec, ScippConnec, AstropyNDDataConnec
+from ntv_numpy.xconnector import PandasConnec
 
 
 class XdatasetCategory(ABC):
     ''' category of Xndarray (dynamic tuple of full_name) - see Xdataset docstring'''
 
     xnd: list = NotImplemented
     names: list = NotImplemented
 
     @abstractmethod
     def dims(self, var, json_name=False):
         '''method defined in Xdataset class'''
 
     @property
-    def global_vars(self):
-        '''return a tuple of namedarrays or variable Xndarray full_name'''
-        return tuple(sorted(nda for nda in self.namedarrays + self.variables))
-
-    @property
     def data_arrays(self):
         '''return a tuple of data_arrays Xndarray full_name'''
-        return tuple(sorted(nda for nda in self.namedarrays if not nda in self.dimensions))
+        return tuple(sorted(nda for nda in self.namedarrays
+                            if not nda in self.dimensions + self.uniques))
 
     @property
     def dimensions(self):
         '''return a tuple of dimensions Xndarray full_name'''
         dimable = []
         for var in self.variables:
             dimable += self.dims(var)
         return tuple(sorted(set(nda for nda in dimable if nda in self.namedarrays)))
 
     @property
+    def shape(self):
+        '''return an array with the length of dimensions'''
+        return [len(self[dim]) for dim in self.dimensions]
+
+    @property
     def coordinates(self):
         '''return a tuple of coordinates Xndarray full_name'''
         dims = set(self.dimensions)
         if not dims:
             return ()
         return tuple(sorted(set(xnda.name for xnda in self.xnd
                                 if xnda.xtype == 'variable' and set(xnda.links) != dims)))
@@ -67,48 +78,56 @@
     def variables(self):
         '''return a tuple of variables Xndarray full_name'''
         return tuple(sorted(xnda.name for xnda in self.xnd if xnda.xtype == 'variable'))
 
     @property
     def undef_vars(self):
         '''return a tuple of variables Xndarray full_name with inconsistent shape'''
-        return tuple(sorted([var for var in self.variables if self[var].shape !=
-                             [len(self[dim]) for dim in self.dims(var)]]))
+        return tuple(sorted(var for var in self.variables if self[var].shape !=
+                            [len(self[dim]) for dim in self.dims(var)]))
 
     @property
     def undef_links(self):
         '''return a tuple of variables Xndarray full_name with inconsistent links'''
-        return tuple(sorted([link for var in self.variables for link in self[var].links
-                             if not link in self.names]))
+        return tuple(sorted(link for var in self.variables for link in self[var].links
+                            if not link in self.names))
 
     @property
     def masks(self):
         '''return a tuple of additional Xndarray full_name with boolean ntv_type'''
-        return tuple(sorted([xnda.full_name for xnda in self.xnd
-                             if xnda.xtype == 'additional' and xnda.ntv_type == 'boolean']))
+        return tuple(sorted(xnda.full_name for xnda in self.xnd
+                            if xnda.xtype == 'additional' and xnda.ntv_type == 'boolean'))
 
     @property
     def data_add(self):
         '''return a tuple of additional Xndarray full_name with not boolean ntv_type'''
-        return tuple(sorted([xnda.full_name for xnda in self.xnd
-                             if xnda.xtype == 'additional' and xnda.ntv_type != 'boolean']))
+        return tuple(sorted(xnda.full_name for xnda in self.xnd
+                            if xnda.xtype == 'additional' and xnda.ntv_type != 'boolean'))
 
     @property
     def metadata(self):
         '''return a tuple of metadata Xndarray full_name'''
-        return tuple(sorted(xnda.name for xnda in self.xnd if xnda.xtype == 'metadata'))
+        return tuple(sorted(xnda.full_name for xnda in self.xnd if xnda.xtype == 'meta'))
+
+    @property
+    def uniques(self):
+        '''return a tuple of unique Xndarray full_name'''
+        return tuple(full_name for full_name in self.namedarrays if len(self[full_name]) == 1)
 
     @property
     def additionals(self):
         '''return a tuple of additionals Xndarray full_name'''
         return tuple(sorted(xnda.full_name for xnda in self.xnd if xnda.xtype == 'additional'))
 
-    def var_group(self, name):
+    def group(self, grp):
         '''return a tuple of Xndarray full_name with the same name'''
-        return tuple(sorted(xnda.full_name for xnda in self.xnd if xnda.name == name))
+        if isinstance(grp, str):
+            return tuple(sorted(xnda.full_name for xnda in self.xnd
+                                if grp in (xnda.name, xnda.full_name)))
+        return tuple(sorted(nam for gr_nam in grp for nam in self.group(gr_nam)))
 
     def add_group(self, add_name):
         '''return a tuple of Xndarray full_name with the same add_name'''
         return tuple(sorted(xnda.full_name for xnda in self.xnd if xnda.add_name == add_name))
 
 
 class XdatasetInterface(ABC):
@@ -150,15 +169,14 @@
         notype = kwargs['notype'] if ('notype' in kwargs and isinstance(kwargs['notype'], list) and
                                       len(kwargs['notype']) == len(self)) else [False] * len(self)
         forma = kwargs['format'] if ('format' in kwargs and isinstance(kwargs['format'], list) and
                                      len(kwargs['format']) == len(self)) else ['full'] * len(self)
         noshape = kwargs.get('noshape', True)
         dic_xnd = {}
         for xna, notyp, forma in zip(self.xnd, notype, forma):
-            # not_shape = True if len(xna.links) == 1 else noshape
             dic_xnd |= xna.to_json(notype=notyp, novalue=kwargs.get('novalue', False),
                                    noshape=noshape, format=forma, header=False)
         return Nutil.json_ntv(self.name, 'xdataset', dic_xnd,
                               header=kwargs.get('header', True),
                               encoded=kwargs.get('encoded', False))
 
     def to_xarray(self, **kwargs):
@@ -198,63 +216,77 @@
         return AstropyNDDataConnec.xexport(self, **kwargs)
 
     @staticmethod
     def from_nddata(ndd, **kwargs):
         '''return a Xdataset from a NDData'''
         return AstropyNDDataConnec.ximport(ndd, Xdataset, **kwargs)
 
+    def to_dataframe(self, **kwargs):
+        '''return a pd.DataFrame from a Xdataset'''
+        return PandasConnec.xexport(self, **kwargs)
+
+    @staticmethod
+    def from_dataframe(dfr, **kwargs):
+        '''return a Xdataset from a pd.DataFrame'''
+        return PandasConnec.ximport(dfr, Xdataset, **kwargs)
+
 
 class Xdataset(XdatasetCategory, XdatasetInterface):
     ''' Representation of a multidimensional Dataset
 
     *Attributes :*
     - **name** :  String - name of the Xdataset
     - **xnd**:   list of Xndarray
 
     *dynamic values (@property)*
     - `xtype`
     - `validity`
     - `dic_xnd`
     - `partition`
+    - `length`
     - `info`
 
     *methods*
     - `parent`
     - `dims`
     - `shape_dims`
     - `to_canonical`
     - `to_ndarray`
+    - `to_darray`
 
     *XdatasetCategory (@property)*
     - `names`
-    - `global_vars`
     - `data_arrays`
     - `dimensions`
     - `coordinates`
     - `data_vars`
     - `namedarrays`
     - `variables`
     - `undef_vars`
     - `undef_links`
     - `masks`
     - `data_add`
+    - `meta`
     - `metadata`
+    - `uniques`
     - `additionals`
-    - `var_group`
+    - `group`
     - `add_group`
 
     *XdatasetInterface methods *
     - `read_json` (static)
     - `to_json`
     - `from_xarray` (static)
     - `to_xarray`
     - `from_scipp` (static)
     - `to_scipp`
     - `from_nddata` (static)
     - `to_nddata`
+    - `from_dataframe` (static)
+    - `to_dataframe`
     '''
 
     def __init__(self, xnd=None, name=None):
         '''Xdataset constructor
 
             *Parameters*
 
@@ -271,15 +303,16 @@
             case xnda if isinstance(xnda, Xndarray):
                 self.xnd = [xnda]
             case _:
                 self.xnd = []
 
     def __repr__(self):
         '''return classname and number of value'''
-        return self.__class__.__name__ + '[' + str(len(self)) + ']'
+        return (self.__class__.__name__ + '[' + str(len(self)) + ']\n' +
+                pprint.pformat(self.to_json(novalue=True, header=False, noshape=False)))
 
     def __str__(self):
         '''return json string format'''
         return json.dumps(self.to_json())
 
     def __eq__(self, other):
         '''equal if xnd are equal'''
@@ -393,14 +426,19 @@
 
     @property
     def dic_xnd(self):
         '''return a dict of Xndarray where key is the full_name'''
         return {xnda.full_name: xnda for xnda in self.xnd}
 
     @property
+    def length(self):
+        '''return the max length of Xndarray'''
+        return max(len(xnda) for xnda in self.xnd)
+
+    @property
     def names(self):
         '''return a tuple with the Xndarray full_name'''
         return tuple(xnda.full_name for xnda in self.xnd)
 
     @property
     def partition(self):
         '''return a dict of Xndarray grouped with category'''
@@ -410,38 +448,64 @@
                 } if self.data_arrays else {}
         dic |= {'dimensions': list(self.dimensions)} if self.dimensions else {}
         dic |= {'coordinates': list(self.coordinates)
                 } if self.coordinates else {}
         dic |= {'additionals': list(self.additionals)
                 } if self.additionals else {}
         dic |= {'metadata': list(self.metadata)} if self.metadata else {}
+        dic |= {'uniques': list(self.uniques)} if self.uniques else {}
         return dic
 
     @property
     def info(self):
         '''return a dict with Xdataset information '''
         inf = {'name': self.name, 'xtype': self.xtype} | self.partition
         inf['validity'] = self.validity
         inf['length'] = len(self[self.data_vars[0]]) if self.data_vars else 0
         inf['width'] = len(self)
-        return {key: val for key, val in inf.items() if val}
+        data = {name: {key: val for key, val in self[name].info.items() if key != 'name'}
+                for name in self.names}
+        return {'structure': {key: val for key, val in inf.items() if val},
+                'data': {key: val for key, val in data.items() if val}}
+
+    @property
+    def tab_info(self):
+        '''return a dict with Xdataset information for tabular interface'''
+        info = self.info
+        data = info['data']
+        t_info = {}
+        if 'dimensions' in info['structure']:
+            t_info['dimensions'] = info['structure']['dimensions']
+        t_info['data'] = {name: {key: val for key, val in data[name].items()
+                                 if key in ['shape', 'xtype', 'meta', 'links']}
+                          for name in data}
+        return t_info
 
     def to_canonical(self):
         '''remove optional links of the included Xndarray'''
         for name in self.names:
             if self[name].links in ([self[name].name], [name]):
                 self[name].links = None
         for add in self.additionals:
             if self[add].links in [self[self[add].name].links,
                                    [self[add].name]]:
                 self[add].links = None
+        for unic in self.uniques:
+            self[unic].links = None
         return self
 
     def to_ndarray(self, full_name):
         '''convert a Xndarray from a Xdataset in a np.ndarray'''
         if self.shape_dims(full_name) is None:
             data = self[full_name].ndarray
         else:
             data = self[full_name].darray.reshape(self.shape_dims(full_name))
         if data.dtype.name[:8] == 'datetime':
             data = data.astype('datetime64[ns]')
         return data
+
+    def to_darray(self, full_name):
+        '''convert a Xndarray from a Xdataset in a flattened np.ndarray'''
+        data = self[full_name].darray
+        if data.dtype.name[:8] == 'datetime':
+            data = data.astype('datetime64[ns]')
+        return data
```

### Comparing `ntv_numpy-0.1.2/ntv_numpy/xndarray.py` & `ntv_numpy-0.2.0/ntv_numpy/xndarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,25 +53,24 @@
 
         - **full_name**: string (default None) - name with additional name
         - **nda** : Ndarray (default None) - data
         - **links**: List of string (default None) - dims or other names of associated Xndarray
         - **ntv_type**: string (default None) - ntv_type to apply to data
         - **meta**: dict (default None) - information
         '''
-        # print('init xnd', full_name, nda.to_json(), links, meta)
         if isinstance(full_name, Xndarray):
             self.name = full_name.name
             self.add_name = full_name.add_name
             self.nda = full_name.nda
             self.links = full_name.links
             self.meta = full_name.meta
             return
         self.name, self.add_name = Nutil.split_name(full_name)
         self.nda = Ndarray(nda) if not nda is None else None
-        self.links = sorted(links) if links else None
+        self.links = links if links else None
         self.meta = meta if meta else None
         if self.meta is None and self.nda is None:
             raise NdarrayError('A Xndarray has to have metadata or Ndarray')
 
     def __repr__(self):
         '''return classname and number of value'''
         return self.__class__.__name__ + '[' + self.full_name + ']'
@@ -102,17 +101,15 @@
 
     def __getitem__(self, ind):
         ''' return ndarray value item'''
         if self.nda is None:
             return None
         if isinstance(ind, tuple):
             return [self.nda[i] for i in ind]
-            # return [copy(self.values[i]) for i in ind]
         return self.nda[ind]
-        # return copy(self.values[ind])
 
     def __copy__(self):
         ''' Copy all the data '''
         return self.__class__(self)
 
     @property
     def darray(self):
@@ -149,27 +146,29 @@
         ''' infos of the Xndarray'''
         inf = {'name': self.full_name}
         inf['length'] = len(self)
         if self.nda:
             inf['mode'] = self.mode
             inf['ntvtype'] = self.ntv_type
             inf['shape'] = self.shape
+        inf['uri'] = self.uri
+        inf['meta'] = self.meta
         inf['xtype'] = self.xtype
         inf['links'] = self.links
         return {key: val for key, val in inf.items() if val}
 
     @property
     def xtype(self):
         '''nature of the Xndarray (undefined, namedarray, variable, additional,
-        inconsistent)'''
+        meta, inconsistent)'''
         match [self.links, self.add_name, self.mode]:
             case [_, _, 'inconsistent']:
                 return 'inconsistent'
             case [_, _, 'undefined']:
-                return 'metadata'
+                return 'meta'
             case [None, '', _]:
                 return 'namedarray'
             case [_, '', _]:
                 return 'variable'
             case [_, str(), _]:
                 return 'additional'
             case _:
@@ -243,15 +242,14 @@
         '''
         option = {'notype': False, 'format': 'full',
                   'noshape': True, 'header': True, 'encoded': False,
                   'novalue': False, 'noname': False} | kwargs
         if not option['format'] in ['full', 'complete']:
             option['noshape'] = False
         opt_nda = option | {'header': False}
-        # nda_str = Ndarray.to_json(self.nda,
         nda_str = self.nda.to_json(**opt_nda) if not self.nda is None else None
         lis = [nda_str, self.links, self.meta]
         lis = [val for val in lis if not val is None]
         return Nutil.json_ntv(None if option['noname'] else self.full_name,
                               None if option['noname'] else 'xndarray',
                               lis[0] if lis == [self.meta] else lis,
                               header=option['header'], encoded=option['encoded'])
```

### Comparing `ntv_numpy-0.1.2/ntv_numpy.egg-info/PKG-INFO` & `ntv_numpy-0.2.0/ntv_numpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntv_numpy
-Version: 0.1.2
+Version: 0.2.0
 Summary: NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability
 Home-page: https://github.com/loco-philippe/ntv-numpy/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: numpy,JSON-NTV,semantic JSON,development,environmental data,multidimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -52,17 +52,18 @@
 
 ```mermaid
 ---
 title: Example of interoperability
 ---
 flowchart LR
     A[Xarray] <--lossless--> B[Neutral\nXdataset]
-    B <--lossless--> C[NDData]
     D[Scipp] <--lossless--> B
+    C[NDData] <--lossless--> B
     B <--lossless--> E[JSON]
+    B <--lossless--> F[DataFrame]
 ```
 
 ### Data example
 
 ```python
 In [1]: example = {
                 'example:xdataset': {
@@ -78,56 +79,59 @@
                         
                         'ranking': [['month', [2, 2], [1, 2, 3, 4]], ['var1']],
                         'z': [['float', [10, 20]], ['x']],
                         'z.uncertainty': [[[0.1, 0.2]]],
                         
                         'z_bis': [[['z1_bis', 'z2_bis']]],
                 
-                        'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/'}
+                        'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/',
+                        'location': [['string', ['paris']]]}
                 }
         }
 
 In [2]: from ntv_numpy import Xdataset
 
         x_example = Xdataset.read_json(example)
-        x_example.info
+        x_example.info['structure']
 Out[2]: {'name': 'example',
         'xtype': 'group',
         'data_vars': ['var1', 'var2'],
         'data_arrays': ['z_bis'],
         'dimensions': ['x', 'y'],
         'coordinates': ['ranking', 'z'],
         'additionals': ['var1.mask1', 'var1.mask2', 'var1.variance', 'z.uncertainty'],
         'metadata': ['info'],
+        'uniques': ['location'],
         'validity': 'undefined',
         'length': 4,
-        'width': 12}
+        'width': 13}
 ```
 
 The JSON representation is equivalent to the Xdataset entity (Json conversion reversible)
 
 ```python
 In [3]: x_json = x_example.to_json()
         x_example_json = Xdataset.read_json(x_json)
         x_example_json == x_example
-Out[2]: True
+Out[3]: True
 ```
 
 ### Xarray interoperability
 
 ```python
 In [4]: x_xarray = x_example.to_xarray()
         print(x_xarray)
-Out[4]: <xarray.Dataset> Size: 182B
+Out[4]: <xarray.Dataset> Size: 202B
         Dimensions:        (x: 2, y: 2)
         Coordinates:
           * x              (x) <U6 48B '23F0AE' '578B98'
           * y              (y) datetime64[ns] 16B 2021-01-01 2022-02-02
             ranking        (x, y) int32 16B 1 2 3 4
             z              (x) float64 16B 10.0 20.0
+            location       <U5 20B 'paris'
             var1.mask1     (x) bool 2B True False
             var1.mask2     (x, y) bool 4B True False False True
             var1.variance  (x, y) float64 32B 0.1 0.2 0.3 0.4
             z.uncertainty  (x) float64 16B 0.1 0.2
         Data variables:
             var1           (x, y) float64 32B 10.1 0.4 3.4 8.2
         Attributes:
@@ -136,25 +140,55 @@
             var2:     [['var2.ntv'], ['x', 'y']]
             z_bis:    [['string', ['z1_bis', 'z2_bis']]]
 ```
 
 Reversibility:
 
 ```python
-In [3]: x_example_xr = Xdataset.from_xarray(x_xarray)
+In [5]: x_example_xr = Xdataset.from_xarray(x_xarray)
         x_example_xr == x_example_json == x_example
-Out[2]: True
+Out[5]: True
+```
+
+### Pandas interoperability
+
+```python
+In [6]: x_dataframe = x_example.to_dataframe()
+        print(x_example.to_dataframe(json_name=False))
+        print(x_xarray)
+Out[6]: 
+                   ranking     z  z.uncertainty  var1  var1.mask1  var1.mask2  \
+x      y                                                                        
+23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True   
+       2022-02-02        2  10.0            0.1   0.4        True       False   
+578B98 2021-01-01        3  20.0            0.2   3.4       False       False   
+       2022-02-02        4  20.0            0.2   8.2       False        True   
+
+                   var1.variance location  
+x      y                                   
+23F0AE 2021-01-01            0.1    paris  
+       2022-02-02            0.2    paris  
+578B98 2021-01-01            0.3    paris  
+       2022-02-02            0.4    paris 
+```
+
+Reversibility:
+
+```python
+In [7]: x_example_pd = Xdataset.from_dataframe(x_dataframe)
+        x_example_pd == x_example_xr == x_example_json == x_example
+Out[7]: True
 ```
 
 ### scipp interoperability
 
 ```python
-In [4]: x_scipp = x_example.to_scipp()
+In [8]: x_scipp = x_example.to_scipp()
         print(x_scipp['example'])
-Out[4]: <scipp.Dataset>
+Out[8]: <scipp.Dataset>
 Dimensions: Sizes[x:string:2, y:date:2, ]
 Coordinates:
 * ranking:month           int32  [dimensionless]  (x:string, y:date)  [1, 2, 3, 4]
 * x:string               string  [dimensionless]  (x:string)  ["23F0AE", "578B98"]
 * y:date              datetime64            [ns]  (y:date)  [2021-01-01T00:00:00.000000000, 2022-02-02T00:00:00.000000000]
 * z:float               float64  [dimensionless]  (x:string)  [10, 20]
 Data:
@@ -163,17 +197,17 @@
         mask1:boolean      bool  [dimensionless]  (x:string)  [True, False]
         mask2:boolean      bool  [dimensionless]  (x:string, y:date)  [True, False, False, True]
 ```
 
 Reversibility:
 
 ```python
-In [3]: x_example_sc = Xdataset.from_scipp(x_scipp)
-        x_example_sc == x_example_xr == x_example_json == x_example
-Out[2]: True
+In [9]: x_example_sc = Xdataset.from_scipp(x_scipp)
+        x_example_sc == x_example_pd == x_example_xr == x_example_json == x_example
+Out[9]: True
 ```
 
 ### NDData interoperability
 
 ```python
 In [1]: example = {
                 'example:xdataset': {
@@ -187,35 +221,35 @@
                                 'CTYPE2': 'DEC--TAN', 'CRVAL1': 5.63056810618, 'CRVAL2': -72.05457184279, 'LONPOLE': 180.0,
                                 'LATPOLE': -72.05457184279, 'WCSNAME': 'IDC_qbu1641sj', 'MJDREF': 0.0, 'RADESYS': 'ICRS'},
                         'psf': [['float[erg/s]', [1,2,3,4]]]
                 }
         } 
         n_example = Xdataset.read_json(example)
         n_example.info 
-Out[4]: {'name': 'example',
+Out[1]: {'name': 'example',
         'xtype': 'group',
         'data_arrays': ['data', 'psf'],
         'additionals': ['data.mask', 'data.uncertainty'],
         'metadata': ['meta', 'wcs'],
         'validity': 'valid',
         'width': 6}
 ```
 
 ```python
-In [4]: n_nddata = n_example.to_nddata()
+In [2]: n_nddata = n_example.to_nddata()
         n_nddata
-Out[4]: NDData([1., 2., ——, ——], unit='erg / s')
+Out[2]: NDData([1., 2., ——, ——], unit='erg / s')
 ```
 
 Reversibility:
 
 ```python
-In [5]: n_example_ndd = Xdataset.from_nddata(n_nddata)
+In [3]: n_example_ndd = Xdataset.from_nddata(n_nddata)
         n_example_ndd == n_example
-Out[5]: True
+Out[3]: True
 ```
 
 ## URI usage
 
 In the example, only structural data is exchanged with json format.
 
 ```python
@@ -241,15 +275,15 @@
                 }
         }
 ```
 
 The complete example can be rebuild with loading data (path + file name).
 
 ```python
-In [5]: # simulation of reading files at the indicated "path"
+In [2]: # simulation of reading files at the indicated "path"
         var1          = np.array([10.1, 0.4, 3.4, 8.2])
         var1_variance = Ndarray([0.1, 0.2, 0.3, 0.4], ntv_type='float')
         var1_mask1    = np.array([True, False])
         var1_mask2    = np.array([True, False, False, True])
         var2          = Ndarray('var2.ntv')
         x             = np.array(['23F0AE', '578B98'])
         y             = np.array(['2021-01-01', '2022-02-02'], dtype='datetime64[D]')
@@ -261,9 +295,9 @@
         array_data = [var1, var1_variance, var1_mask1, var1_mask2, var2, x, y, ranking, z, z_uncertainty, z_bis]
 
         x_example_mixte_numpy = copy(x_example_mixte)
         for data, xnda in zip(array_data, x_example_mixte_numpy.xnd):
         xnda.set_ndarray(Ndarray(data))
 
         x_example_mixte_numpy == x_example_mixte_json == x_example_sc == x_example_xr == x_example_json == x_example
-Out[5]: True
+Out[2]: True
 ```
```

### Comparing `ntv_numpy-0.1.2/setup.py` & `ntv_numpy-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ntv_numpy",
-    version="0.1.2",
+    version="0.2.0",
     description="NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loco-philippe/ntv-numpy/blob/main/README.md",
     author="Philippe Thomy",
     author_email="philippe@loco-labs.io",
     classifiers=[
```

### Comparing `ntv_numpy-0.1.2/tests/test_ntv_numpy.py` & `ntv_numpy-0.2.0/tests/test_ntv_numpy.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import xarray as xr
 
 import ntv_pandas as npd
 
 #from ntv_numpy.numpy_ntv_connector import read_json_tab, to_json_tab
 from ntv_numpy import NdarrayConnec, XndarrayConnec
 from ntv_numpy import Darray, Dfull, Dcomplete, Ndarray, Xndarray, Nutil, Xdataset, Dutil
+from ntv_numpy.xconnector import PandasConnec
  
 from json_ntv import NtvConnector, Ntv, NtvSingle, NtvList
 SeriesConnec = NtvConnector.connector()['SeriesConnec']
 DataFrameConnec = NtvConnector.connector()['DataFrameConnec']
 nd_equals = Dutil.equals
 
 #read_json({':ndarray': ['int64', [1, 2]]})
@@ -256,16 +257,16 @@
                   [{'ranking': [['int', [2, 2], [1, 2, 3, 4]], ['var1']]}, 'absolute', 'variable'],
                   [{'x': [['string', ['x1', 'x2']], {'test': 21}]}, 'absolute', 'namedarray'],
                   [{'y': [['string', ['y1', 'y2']]]}, 'absolute', 'namedarray'],
                   [{'z': [['string', ['z1', 'z2']], ['x']]}, 'absolute', 'variable'],
                   [{'x.mask': [['boolean', [True, False]]]}, 'absolute', 'additional'],
                   [{'x.variance': [['float64', [0.1, 0.2]]]}, 'absolute', 'additional'],
                   [{'z.variance': [['float64', [0.1, 0.2]]]}, 'absolute', 'additional'],
-                  [{'unit': 'kg'}, 'undefined', 'metadata'],
-                  [{'info': {'example': 'everything'}}, 'undefined', 'metadata'],
+                  [{'unit': 'kg'}, 'undefined', 'meta'],
+                  [{'info': {'example': 'everything'}}, 'undefined', 'meta'],
                 ]
         
         for ex, mode, xtype in example:
             #print(ex)
             self.assertEqual(ex, Xndarray.read_json(ex).to_json(header=False)) 
             self.assertEqual(mode, Xndarray.read_json(ex).mode) 
             self.assertEqual(xtype, Xndarray.read_json(ex).xtype) 
@@ -303,67 +304,71 @@
             'ranking': [[[2, 2], [1, 2, 3, 4]], ['var1']],
             'x': [[['x1', 'x2']], {'test': 21}],
             'y': [[['y1', 'y2']]],
             'z': [[['z1', 'z2']], ['x']],
             'x.mask1': [[[True, False]]],
             'x.variance': [[[0.1, 0.2]]],
             'z.variance': [[[0.1, 0.2]]],
-            'unit': 'kg',
+            'unit': [[['kg']]],
             'info': {'example': 'everything'}}}
         
         notype = [True, False, True, True, True, True, True, True, True, True, True]
         xds = Xdataset.read_json(example)        
         self.assertEqual(xds.to_json(notype=notype, noshape=True, header=False), example)                                          
         self.assertEqual(xds.dimensions, ('x', 'y'))
         self.assertEqual(xds.partition, {'coordinates': ['ranking', 'z'],
-         'data_vars': ['var1', 'var2'], 'metadata': ['info', 'unit'],
+         'data_vars': ['var1', 'var2'], 'uniques': ['unit'], 'metadata': ['info'],
          'additionals': ['x.mask1', 'x.variance', 'z.variance'], 'dimensions': ['x', 'y']})
         
         xdim = Xdataset(xds[xds.dimensions])
         self.assertEqual(xdim.to_json(novalue=True, noshape=True), {':xdataset': {
                          'x': [['string', ['-']], {'test': 21}],
                          'y': [['string', ['-']]]}})        
                                   
     def test_xdataset_info(self):    
         
         xd = Xdataset([Xndarray('example', np.array(['x1', 'x2']))], 'test')
-        self.assertEqual(xd.info, {'name': 'test', 'xtype': 'group', 'validity': 'valid',
-                                   'data_arrays': ['example'], 'width': 1})
+        self.assertEqual(xd.info, {'structure': {'name': 'test', 'xtype': 'group', 
+                'validity': 'valid', 'data_arrays': ['example'], 'width': 1},
+                                   'data': {'example': {'length': 2, 'mode': 'absolute',
+                'ntvtype': 'string', 'shape': [2], 'xtype': 'namedarray'}}})
 
         example = {'test': {
             'var1': [['https://github.com/loco-philippe/ntv-numpy/tree/main/example/ex_ndarray.ntv'], ['x', 'y']],
             'var2': [['float[kg]', [2, 2], [10.1, 0.4, 3.4, 8.2]], ['x', 'y']],
             'ranking': [[[2, 2], [1, 2, 3, 4]], ['var2']],
             'x': [[['x1', 'x2']], {'test': 21}],
             'y': [[['y1', 'y2']]],
             'z': [[['z1', 'z2']], ['x']],
             'z_bis': [[['z1_bis', 'z2_bis']]],
             'x.mask1': [[[True, False]], ['x']],
             'x.variance': [[[0.1, 0.2]], ['x']],
             'z.variance': [[[0.1, 0.2]], ['x']],
-            'unit': 'kg',
+            'unit': [[['kg']]],
             'info': {'example': 'everything'}}}
         xd = Xdataset.read_json(example)
-        self.assertEqual(xd.info, { 'name': 'test', 'xtype': 'group',
+        self.assertEqual(xd.info['structure'], { 'name': 'test', 'xtype': 'group',
                                     'data_vars': ['var1', 'var2'],
                                     'data_arrays': ['z_bis'],
                                     'dimensions': ['x', 'y'],
                                     'coordinates': ['ranking', 'z'],
                                     'additionals': ['x.mask1', 'x.variance', 'z.variance'],
-                                    'metadata': ['info', 'unit'],
+                                    'metadata': ['info'],
+                                    'uniques': ['unit'],
                                     'validity': 'undefined', 'width': 12})
 
         del(xd[('var1', 'z_bis')])
-        self.assertEqual(xd.info, { 'name': 'test', 'xtype': 'mono',
+        self.assertEqual(xd.info['structure'], { 'name': 'test', 'xtype': 'mono',
                                     'data_vars': ['var2'],
                                     'dimensions': ['x', 'y'],
                                     'length' : 4,
                                     'coordinates': ['ranking', 'z'],
                                     'additionals': ['x.mask1', 'x.variance', 'z.variance'],
-                                    'metadata': ['info', 'unit'],
+                                    'metadata': ['info'],
+                                    'uniques': ['unit'],
                                     'validity': 'valid', 'width': 10})        
 
         example = {'test': {
             'var1': [['float[m3]', [2, 2], 'path/var1.ntv'], ['x', 'y']],
             'var2': [['float[kg]', [2, 2], 'path/var2.ntv'], ['x', 'y']],
             'ranking': [[[2, 2], 'path/ranking.ntv'], ['var2']],
             'x': [['path/x.ntv'], {'test': 21}],
@@ -372,23 +377,25 @@
             'z_bis': [['path/z_bis.ntv']],
             'x.mask1': [['path/x.mask1.ntv'], ['x']],
             'x.variance': [['path/x.variance.ntv'], ['x']],
             'z.variance': [['path/z.variance.ntv'], ['x']],
             'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/'}}}
        
         xd = Xdataset.read_json(example)
-        self.assertEqual(xd.info, { 'name': 'test', 'xtype': 'group',
+        self.assertEqual(xd.info['structure'], { 'name': 'test', 'xtype': 'group',
                                     'data_vars': ['var1', 'var2'],
                                     'data_arrays': ['z_bis'],
                                     'dimensions': ['x', 'y'],
                                     'coordinates': ['ranking', 'z'],
                                     'additionals': ['x.mask1', 'x.variance', 'z.variance'],
                                     'metadata': ['info'],
                                     'validity': 'undefined', 'width': 11})
 
+class Test_Xdataset_xarray_scipp(unittest.TestCase):    
+
     def test_xdataset_DataArray(self):    
         
         examples = [
             {'test': {
                 'var2': [['float[kg]', [2, 2], [10.1, 0.4, 3.4, 8.2]], ['x', 'y']],
                 'unit': 'kg', 'info': {'example': 'everything'},
                 'ranking': [[[2, 2], [1, 2, 3, 4]], ['var2']],  #!!!
@@ -414,15 +421,15 @@
 
                 'y': [['date', ['2021-01-01', '2022-02-02']]],
 
                 'z': [['float', [10, 20]], ['x']],
                 #'z_bis': [[['z1_bis', 'z2_bis']]],
                 'z.variance': [[[0.1, 0.2]]],
 
-                'unit': 'kg',
+                'unit': [[['kg']]],
                 'info': {'example': 'everything'}
             }}]
         for example in examples:
             xd = Xdataset.read_json(example) 
             xd2 = Xdataset.from_xarray(xd.to_xarray(dataset=False))
             self.assertEqual(xd, xd2)
             xd2 = Xdataset.from_xarray(xd.to_xarray())
@@ -467,24 +474,33 @@
 
             'z': [['float', [10, 20]], ['x']],
             #'z_bis': [[['z1_bis', 'z2_bis']]],
             'z.variance': [['float', [0.1, 0.2]]],
 
             #'unit': 'kg',
             #'info': {'example': 'everything'}
-            } #}
+            }, #},
+            { 'x': [['int32', [10, 20]]],
+              'y': [['string', ['a', 'b', 'c']]],
+              'z': [['int32', [1, 2, 3]]],
+              'year': [['int32', [2020, 2021]]],
+              'point': [['string', [3, 2], ['pt1', 'pt2', 'pt3', 'pt4', 'pt5', 'pt6']], ['y', 'x']],
+              'along_x': [['float64', [-1.18, -0.74]], ['x']],
+              'foo': [['float64',  [2, 3, 3, 2], list(range(36))], ['x', 'y', 'z', 'year']]}
             ]
         for example in examples:
             xd = Xdataset.read_json(example) 
             xd2 = Xdataset.from_scipp(xd.to_scipp(dataset=False, datagroup=False))
             self.assertEqual(xd, xd2)
             xd2 = Xdataset.from_scipp(xd.to_scipp(dataset=False))
             self.assertEqual(xd, xd2)
             xd2 = Xdataset.from_scipp(xd.to_scipp())
             self.assertEqual(xd, xd2)        
+            xd2 = Xdataset.from_scipp(xd.to_scipp(datagroup=False))
+            self.assertEqual(xd, xd2)        
 
     def test_xdataset_mixte(self):    
         
         examples = [{ 'test:xdataset': {
             'var1': [['https://github.com/loco-philippe/ntv-numpy/tree/main/example/ex_ndarray.ntv'], ['x', 'y']],    
             'var2': [['float[kg]', [2, 2], [10.1, 0.4, 3.4, 8.2]], ['x', 'y']],
             'var2.variance': [[[2, 2], [0.1, 0.2, 0.3, 0.4]]],
@@ -500,22 +516,146 @@
             'y': [['date', ['2021-01-01', '2022-02-02']]],
 
             'z': [['float', [10, 20]], ['x']],
             'z_bis': [[['z1_bis', 'z2_bis']]],
             'z.uncertainty': [[[0.1, 0.2]]],
             'z.variance': [['float', [0.1, 0.2]]],
 
-            'info': {'example': 'everything'}
+            'info': {'example': 'everything'},
+            'location': [[['paris']]]
             } }
             ]
         for example in examples:
             xd = Xdataset.read_json(example) 
             xd_sc = Xdataset.from_scipp(xd.to_scipp(dataset=False))
             xd_xr = Xdataset.from_xarray(xd.to_xarray(dataset=False))
             self.assertTrue(xd == xd_sc == xd_xr)
             xd_sc = Xdataset.from_scipp(xd.to_scipp())
             xd_xr = Xdataset.from_xarray(xd.to_xarray())
             self.assertTrue(xd == xd_sc == xd_xr)
 
+class Test_Xdataset_pandas(unittest.TestCase):    
+
+    def test_xdataset_dataframe(self):    
+
+        ds = xr.Dataset({"foo": (("x", "y", "z", "year"), np.random.randn(2, 3, 3, 2))},
+            coords={
+                "x": [10, 20], "y": ["a", "b", "c"], "z": [1,2,3], "year": [2020, 2021],
+                "point": (("x", "y"), np.array(["pt1", "pt2", "pt3", "pt4", "pt5", "pt6"]).reshape(2,3)),
+                "along_x": ("x", np.random.randn(2)), "scalar": 123})
+        xdt = Xdataset.from_xarray(ds)
+        df = ds.to_dataframe().reset_index()        
+        dimensions = ['x', 'y', 'z', 'year']
+        for name in xdt.names[:]:
+            #tab = xdt.to_tab_array(name, dimensions)
+            tab = PandasConnec._to_np_series(xdt, name, dimensions)
+            if not tab is None: 
+                self.assertTrue(np.all(np.array(df[name]) == tab), name)
+
+        dfr = xdt.to_dataframe(json_name=True)
+        xds = Xdataset.from_dataframe(dfr)
+        self.assertEqual(xds, xdt)
+
+    def test_xdataset_multidim(self):    
+
+        example = { 'test:xdataset': {
+            'var1': [['https://github.com/loco-philippe/ntv-numpy/tree/main/example/ex_ndarray.ntv'], ['x', 'y']],    
+            'var2': [['float[kg]', [2, 2], [10.1, 0.4, 3.4, 8.2]], ['x', 'y']],
+            'var2.variance': [[[2, 2], [0.1, 0.2, 0.3, 0.4]]],
+            'var2.mask1': [[[True, False]], ['x']],
+            'var2.mask2': [[[2, 2], [True, False, False, True]]],
+        
+            'ranking': [['month', [2, 2], [1, 2, 3, 4]], ['var2']],
+        
+        
+            'x': [['string', ['23F0AE', '578B98']]], #, {'test': 21}],
+            'x.mask1': [[[True, False]]],
+        
+            'y': [['date', ['2021-01-01', '2022-02-02']]],
+        
+            'z': [['float', [10, 20]], ['x']],
+            'z_bis': [[['z1_bis', 'z2_bis']]],
+            'z.uncertainty': [[[0.1, 0.2]]],
+            'z.variance': [['float', [0.1, 0.2]]],
+        
+            'info': {'example': 'everything'},
+            'location': 'paris'
+            } }
+        xd = Xdataset.read_json(example) 
+        df = xd.to_dataframe()
+        xd2 = Xdataset.from_dataframe(df)
+        self.assertEqual(xd, xd2)
+
+        example = { ':xdataset': {
+            'var2': [['float[kg]', [2, 2], [10.1, 0.4, 3.4, 8.2]], ['x', 'y']],
+            'var2.variance': [[[2, 2], [0.1, 0.2, 0.3, 0.4]]],
+            'var2.mask1': [[[True, False]], ['x']],
+            'var2.mask2': [[[2, 2], [True, False, False, True]]],
+        
+            'ranking': [['month', [2, 2], [1, 2, 3, 4]], ['x', 'y']],
+        
+        
+            'x': [['string', ['23F0AE', '578B98']]], #, {'test': 21}],
+            'x.mask1': [[[True, False]]],
+        
+            'y': [['date', ['2021-01-01', '2022-02-02']]],
+        
+            'z': [['float', [10, 20]], ['x']],
+            'z.uncertainty': [[[0.1, 0.2]]],
+            'z.variance': [['float', [0.1, 0.2]]],
+        
+            'location': [['string', ['paris']]]
+            } }
+        xd = Xdataset.read_json(example) 
+        df = xd.to_dataframe()
+        xd2 = Xdataset.from_dataframe(df)
+        self.assertEqual(xd, xd2)
+        df3 = xd.to_dataframe(info=False)
+        xd3 = Xdataset.from_dataframe(df3)        
+        self.assertEqual(xd2, xd3)
+
+    def test_xdataset_multipart(self):    
+
+        fruits = {'plants':      ['fruit', 'fruit', 'fruit', 'fruit', 'vegetable', 'vegetable', 'vegetable', 'vegetable'],
+          'plts':        ['fr', 'fr', 'fr', 'fr', 've', 've', 've', 've'], 
+          'quantity':    ['1 kg', '10 kg', '1 kg', '10 kg', '1 kg', '10 kg', '1 kg', '10 kg'],
+          'product':     ['apple', 'apple', 'orange', 'orange', 'peppers', 'peppers', 'carrot', 'carrot'],
+          'price':       [1, 10, 2, 20, 1.5, 15, 1.5, 20],
+          'price level': ['low', 'low', 'high', 'high', 'low', 'low', 'high', 'high'],
+          'group':       ['fruit 1', 'fruit 10', 'fruit 1', 'veget', 'veget', 'veget', 'veget', 'veget'],
+          'id':          [1001, 1002, 1003, 1004, 1005, 1006, 1007, 1008],
+          'supplier':    ["sup1", "sup1", "sup1", "sup2", "sup2", "sup2", "sup2", "sup1"],
+          'location':    ["fr", "gb", "es", "ch", "gb", "fr", "es", "ch"],
+          'valid':       ["ok", "ok", "ok", "ok", "ok", "ok", "ok", "ok"]}
+        df1 = pd.DataFrame(fruits)
+        a_df = df1.npd.analysis(distr=True)
+        xdt = Xdataset.from_dataframe(df1)
+        df3 = xdt.to_dataframe(json_name=False).reset_index()
+        df2 = df1.sort_values(a_df.partitions(mode='id')[0]).reset_index(drop=True)
+        df4 = df3.sort_values(a_df.partitions(mode='id')[0]).reset_index(drop=True)[df2.columns]
+        self.assertTrue(df4.equals(df2))
+        
+    def test_xdataset_unidim(self):    
+
+        simple = { 'a': [1,2,3,4,4],
+                   'b': [10,20,30,40,40],
+                   #'b2': [10,20,30,40,40],
+                   'c': [1,1,3,4,4],
+                   'd': [1,1,1,4,4],
+                   'e': [1,1,1,1,1]}
+        df1 = pd.DataFrame(simple)
+        df3 = Xdataset.from_dataframe(df1).to_dataframe(json_name=False)[df1.columns]
+        self.assertTrue(df3.equals(df1))
+
+        simple = { 'a': [1,2,3,4,5],
+                   'b': [10,20,30,40,50],
+                   'b2': [10,20,30,40,40],
+                   'c': [1,1,3,4,4],
+                   'd': [1,1,1,4,4],
+                   'e': [1,1,1,1,1]}
+        df1 = pd.DataFrame(simple)
+        df3 = Xdataset.from_dataframe(df1).to_dataframe(json_name=False).reset_index()[df1.columns]
+        self.assertTrue(df3.equals(df1))
+
 if __name__ == '__main__':    
     unittest.main(verbosity=2)
```

