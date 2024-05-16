# Comparing `tmp/mass_composition-0.5.2.tar.gz` & `tmp/mass_composition-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.5.2.tar", max compression
+gzip compressed data, was "mass_composition-0.6.0.tar", max compression
```

## Comparing `mass_composition-0.5.2.tar` & `mass_composition-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1069 2024-05-15 21:36:56.586194 mass_composition-0.5.2/LICENSE
--rw-r--r--   0        0        0     3491 2024-05-15 21:36:56.586194 mass_composition-0.5.2/README.md
--rw-r--r--   0        0        0      360 2024-05-15 21:36:56.998195 mass_composition-0.5.2/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9816 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0    11761 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/dag.py
--rw-r--r--   0        0        0       59 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     6565 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0    41619 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/flowsheet.py
--rw-r--r--   0        0        0     2080 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    52834 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      908 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19410 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0     5752 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0     3357 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/stream.py
--rw-r--r--   0        0        0       42 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     4867 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0      842 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/parallel.py
--rw-r--r--   0        0        0     1033 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0     2164 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1717 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8865 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     2014 2024-05-15 21:36:57.006195 mass_composition-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 mass_composition-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-16 00:07:57.169050 mass_composition-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3491 2024-05-16 00:07:57.169050 mass_composition-0.6.0/README.md
+-rw-r--r--   0        0        0      360 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9816 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0    11761 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     6604 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0    41619 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/flowsheet.py
+-rw-r--r--   0        0        0     2080 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    56291 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      908 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19483 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0     5752 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0     6010 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/stream.py
+-rw-r--r--   0        0        0       42 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     4867 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0      842 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/parallel.py
+-rw-r--r--   0        0        0     1033 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     1717 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8865 2024-05-16 00:07:57.577050 mass_composition-0.6.0/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     2040 2024-05-16 00:07:57.581050 mass_composition-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 mass_composition-0.6.0/PKG-INFO
```

### Comparing `mass_composition-0.5.2/LICENSE` & `mass_composition-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/README.md` & `mass_composition-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/balance.py` & `mass_composition-0.6.0/elphick/mass_composition/balance.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/config/config_read.py` & `mass_composition-0.6.0/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.6.0/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/dag.py` & `mass_composition-0.6.0/elphick/mass_composition/dag.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.6.0/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.6.0/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.6.0/elphick/mass_composition/datasets/register.csv`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.6.0/elphick/mass_composition/datasets/sample_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,25 +111,25 @@
 
 
 def size_by_assay_2() -> pd.DataFrame:
     """ 3 x Sample Size x Assay dataset (balanced)
     """
     mc_size: MassComposition = MassComposition(size_by_assay(), name='feed')
     partition = partial(napier_munn, d50=0.150, ep=0.1, dim='size')
-    mc_coarse, mc_fine = mc_size.apply_partition(definition=partition, name_1='coarse', name_2='fine')
+    mc_coarse, mc_fine = mc_size.split_by_partition(partition_definition=partition, name_1='coarse', name_2='fine')
     fs: Flowsheet = Flowsheet().from_streams([mc_size, mc_coarse, mc_fine])
     return fs.to_dataframe()
 
 
 def size_by_assay_3() -> pd.DataFrame:
     """ 3 x Sample Size x Assay dataset (unbalanced)
     """
     mc_size: MassComposition = MassComposition(size_by_assay(), name='feed')
     partition = partial(napier_munn, d50=0.150, ep=0.1, dim='size')
-    mc_coarse, mc_fine = mc_size.apply_partition(definition=partition, name_1='coarse', name_2='fine')
+    mc_coarse, mc_fine = mc_size.split_by_partition(partition_definition=partition, name_1='coarse', name_2='fine')
     # add error to the coarse stream to create an imbalance
     df_coarse_2 = mc_coarse.data.to_dataframe().apply(lambda x: np.random.normal(loc=x, scale=np.std(x)))
     mc_coarse_2: MassComposition = MassComposition(data=df_coarse_2, name='coarse')
     mc_coarse_2 = mc_coarse_2.set_parent_node(mc_size)
     fs_ub: Flowsheet = Flowsheet().from_streams([mc_size, mc_coarse_2, mc_fine])
     return fs_ub.to_dataframe()
 
@@ -152,15 +152,15 @@
     df_met.columns = [col.replace('LOITotal', 'LOI') for col in df_met.columns]
     return df_met
 
 
 def demo_size_network() -> Flowsheet:
     mc_size: MassComposition = MassComposition(size_by_assay(), name='size sample')
     partition = partial(perfect, d50=0.150, dim='size')
-    mc_coarse, mc_fine = mc_size.apply_partition(definition=partition)
+    mc_coarse, mc_fine = mc_size.split_by_partition(partition_definition=partition)
     mc_coarse.name = 'coarse'
     mc_fine.name = 'fine'
     fs: Flowsheet = Flowsheet().from_streams([mc_size, mc_coarse, mc_fine])
     return fs
 
 
 if __name__ == '__main__':
```

### Comparing `mass_composition-0.5.2/elphick/mass_composition/flowsheet.py` & `mass_composition-0.6.0/elphick/mass_composition/flowsheet.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/layout.py` & `mass_composition-0.6.0/elphick/mass_composition/layout.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/mass_composition.py` & `mass_composition-0.6.0/elphick/mass_composition/mass_composition.py`

 * *Files 11% similar despite different names*

```diff
@@ -491,14 +491,16 @@
               fraction: float,
               name_1: Optional[str] = None,
               name_2: Optional[str] = None) -> Tuple['MassComposition', 'MassComposition']:
         """Split the object by mass
 
         A simple mass split maintaining the same composition
 
+        See also: split_by_partition, split_by_function, split_by_estimator
+
         Args:
             fraction: A constant in the range [0.0, 1.0]
             name_1: The name of the reference stream created by the split
             name_2: The name of the complement stream created by the split
 
         Returns:
             tuple of two datasets, the first with the mass fraction specified, the other the complement
@@ -511,44 +513,105 @@
         comp: MassComposition = MassComposition(name=xr_ds_2.mc.name, constraints=self.constraints)
         comp.set_data(data=xr_ds_2, constraints=self.constraints)
 
         self._post_process_split(out, comp, name_1, name_2)
 
         return out, comp
 
-    def apply_partition(self,
-                        definition: Callable,
-                        name_1: Optional[str] = None,
-                        name_2: Optional[str] = None) -> Tuple['MassComposition', 'MassComposition']:
+    def split_by_partition(self,
+                           partition_definition: Callable,
+                           name_1: Optional[str] = None,
+                           name_2: Optional[str] = None) -> Tuple['MassComposition', 'MassComposition']:
         """Partition the object along a given dimension.
 
         This method applies the defined separation resulting in two new objects.
 
-        See also: split
+        See also: split, split_by_function, split_by_estimator
 
         Args:
-            definition: A partition function that defines the efficiency of separation along a dimension
+            partition_definition: A partition function that defines the efficiency of separation along a dimension
             name_1: The name of the reference stream created by the split
             name_2: The name of the complement stream created by the split
 
         Returns:
             tuple of two datasets, the first with the mass fraction specified, the other the complement
         """
         out = deepcopy(self)
         comp = deepcopy(self)
 
-        xr_ds_1, xr_ds_2 = self._data.mc.apply_partition(definition=definition)
+        xr_ds_1, xr_ds_2 = self._data.mc.split_by_partition(partition_definition=partition_definition)
 
         out._data = xr_ds_1
         comp._data = xr_ds_2
 
         self._post_process_split(out, comp, name_1, name_2)
 
         return out, comp
 
+    def split_by_function(self,
+                          split_function: Callable,
+                          name_1: Optional[str] = None,
+                          name_2: Optional[str] = None) -> Tuple['MassComposition', 'MassComposition']:
+        """Split an object using a function.
+
+        This method applies the function to self, resulting in two new objects. The object returned with name_1
+        is the result of the function.  The object returned with name_2 is the complement.
+
+        See also: split, split_by_estimator, split_by_partition
+
+        Args:
+            split_function: Any function that transforms the dataframe from a MassComposition object into a new
+             dataframe with values representing a new (output) stream.  The returned dataframe structure must be
+             identical to the input dataframe.
+            name_1: The name of the stream created by the function
+            name_2: The name of the complement stream created by the split, which is calculated automatically.
+
+        Returns:
+            tuple of two datasets, the first with the mass fraction specified, the other the complement
+        """
+        out_data: pd.DataFrame = split_function(self.data.to_dataframe())
+        out: MassComposition = MassComposition(name=name_1, constraints=self.constraints, data=out_data)
+        comp: MassComposition = self.sub(other=out, name=name_2)
+
+        self._post_process_split(out, comp, name_1, name_2)
+
+        return out, comp
+
+    def split_by_estimator(self,
+                           estimator: 'sklearn.base.BaseEstimator',
+                           name_1: Optional[str] = None,
+                           name_2: Optional[str] = None) -> Tuple['MassComposition', 'MassComposition']:
+        """Split an object using a sklearn estimator.
+
+        This method applies the function to self, resulting in two new objects. The object returned with name_1
+        is the result of the estimator.predict() method.  The object returned with name_2 is the complement.
+
+        See also: split, split_by_function, split_by_partition
+
+        Args:
+            estimator: Any sklearn estimator that transforms the dataframe from a MassComposition object into a new
+             dataframe with values representing a new (output) stream using the predict method.  The returned
+             dataframe structure must be identical to the input dataframe.
+            name_1: The name of the stream created by the estimator.
+            name_2: The name of the complement stream created by the split, which is calculated automatically.
+
+        Returns:
+            tuple of two datasets, the first with the mass fraction specified, the other the complement
+        """
+        out_data: Union[pd.DataFrame, np.ndarray] = estimator.predict(self.data.to_dataframe())
+        if isinstance(out_data, np.ndarray):
+            out_data = pd.DataFrame(out_data, index=self.data.to_dataframe().index,
+                                    columns=self.data.to_dataframe().columns)
+        out: MassComposition = MassComposition(name=name_1, constraints=self.constraints, data=out_data)
+        comp: MassComposition = self.sub(other=out, name=name_2)
+
+        self._post_process_split(out, comp, name_1, name_2)
+
+        return out, comp
+
     def calculate_partition(self, ref: 'MassComposition') -> pd.DataFrame:
         """Calculate the partition of the ref stream relative to self"""
         self._check_one_dim_interval()
         return calculate_partition(df_feed=self.data.to_dataframe(), df_ref=ref.data.to_dataframe(),
                                    col_mass_dry='mass_dry')
 
     # def resample(self, dim: str, num_intervals: int = 50, edge_precision: int = 8) -> 'MassComposition':
@@ -574,15 +637,15 @@
         # TODO: add support for supplementary variables
 
         df_upsampled: pd.DataFrame = mass_preserving_interp(self.data.to_dataframe(),
                                                             interval_edges=interval_edges, precision=precision,
                                                             include_original_edges=include_original_edges)
 
         obj: MassComposition = MassComposition(df_upsampled, name=self.name)
-        obj.nodes = self._nodes
+        obj._nodes = self._nodes
         obj.constraints = self.constraints
         return obj
 
     def add(self, other: 'MassComposition', name: Optional[str] = None) -> 'MassComposition':
         """Add two objects
 
         Adds other to self, with optional name of the returned object
@@ -987,15 +1050,15 @@
         """
 
         xr_sub: xr.Dataset = self._data.mc.sub(other._data)
 
         res: MassComposition = MassComposition(name=xr_sub.mc.name, constraints=self.constraints)
         res.set_data(data=xr_sub, constraints=self.constraints)
 
-        res.nodes = [self._nodes[1], random_int()]
+        res._nodes = [self._nodes[1], random_int()]
         return res
 
     def __truediv__(self, other: 'MassComposition') -> 'MassComposition':
         """Divide self by the supplied object
 
         Perform the division with the mass-composition variables only and then append any attribute variables.
         Args:
@@ -1046,14 +1109,15 @@
             obj_1._data.mc.rename(name_1)
         if name_2:
             obj_2._data.mc.rename(name_2)
         obj_1._nodes = [self._nodes[1], random_int()]
         obj_2._nodes = [self._nodes[1], random_int()]
         obj_1._name = name_1
         obj_2._name = name_2
+
         return obj_1, obj_2
 
     def _intervals_to_columns(self, interval_index: pd.IntervalIndex) -> pd.DataFrame:
         """Reconstruct columns from an interval index
 
         Uses the left and right names stored in the xr.Dataset attrs
```

### Comparing `mass_composition-0.5.2/elphick/mass_composition/mc_node.py` & `mass_composition-0.6.0/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/mc_status.py` & `mass_composition-0.6.0/elphick/mass_composition/mc_status.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.6.0/elphick/mass_composition/mc_xarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,52 +265,52 @@
         comp._obj[self._obj.mc_vars_mass] = comp._obj[self._obj.mc_vars_mass] * (1 - fraction)
         comp.rename(f'({1 - fraction} * {self.name})')
 
         xr.set_options(keep_attrs='default')
 
         return out._obj, comp._obj
 
-    def apply_partition(self, definition: Callable) -> Tuple[xr.Dataset, xr.Dataset]:
+    def split_by_partition(self, partition_definition: Callable) -> Tuple[xr.Dataset, xr.Dataset]:
         """Partition the object along a given dimension.
 
         This method applies the defined partition resulting in two new objects.
 
         See also: split
 
         Args:
-            definition: A partition function that defines the efficiency of separation along a dimension
+            partition_definition: A partition function that defines the efficiency of separation along a dimension
 
         Returns:
             tuple of two datasets, the first defined by the function, the other the complement
         """
 
         xr.set_options(keep_attrs=True)
 
         out = deepcopy(self)
         comp = deepcopy(self)
 
-        if not isinstance(definition, Callable):
+        if not isinstance(partition_definition, Callable):
             raise TypeError("The definition is not a callable function")
-        if 'dim' not in definition.keywords.keys():
+        if 'dim' not in partition_definition.keywords.keys():
             raise NotImplementedError("The callable function passed does not have a dim")
 
-        dim = definition.keywords['dim']
-        definition.keywords.pop('dim')
+        dim = partition_definition.keywords['dim']
+        partition_definition.keywords.pop('dim')
         if isinstance(self._obj[dim].data[0], pd.Interval):
             if dim == 'size':
                 x = mean_size(pd.arrays.IntervalArray(self._obj[dim].data))
             else:
                 x = pd.arrays.IntervalArray(self._obj[dim].data).mid
         else:
             # assume the index is already the mean, not a passing or retained value.
             self._logger.warning('The provided callable is being applied across a dimension that is '
                                  'not an interval. This is not typical usage.  It is assumed that the '
                                  'dimension data represents the centre/mean, and not an edge like '
                                  'retained or passing.')
-        pn = definition(x)
+        pn = partition_definition(x)
         if not ((dim in self._obj.dims) and (len(self._obj.dims) == 1)):
             # TODO: Set the dim to match the partition if it does not already
             # obj_mass = obj_mass.swap_dims(dim=)
             pass
 
         out._obj = out.mul(pn / 100)
         comp._obj = self.sub(out._obj)
```

### Comparing `mass_composition-0.5.2/elphick/mass_composition/plot.py` & `mass_composition-0.6.0/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.6.0/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.6.0/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.6.0/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/components.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/interp.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/loader.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/loader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/parallel.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/partition.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/size.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/size.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/utils/viz.py` & `mass_composition-0.6.0/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/elphick/mass_composition/variables.py` & `mass_composition-0.6.0/elphick/mass_composition/variables.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.2/pyproject.toml` & `mass_composition-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.5.2"
+version = "0.6.0"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
 
@@ -14,15 +14,15 @@
 
 [tool.poetry.scripts]
 bump-version = "scripts.bump_version:main"
 
 [tool.towncrier]
 package = "elphick.mass_composition"
 package_dir = "elphick/mass_composition"
-filename = "HISTORY.rst"
+filename = "CHANGELOG.rst"
 directory = "towncrier/newsfragments"
 [tool.towncrier.fragment.feature]
 [tool.towncrier.fragment.bugfix]
 [tool.towncrier.fragment.doc]
 [tool.towncrier.fragment.removal]
 [tool.towncrier.fragment.misc]
 
@@ -62,11 +62,12 @@
 kaleido = "0.2.1"
 sphinx-autodoc-typehints = "^1.18.3"
 myst-parser = "^0.18.0"
 ydata-profiling = "^4.3.2"
 sphinxcontrib-datatemplates = "^0.9.2"
 sphinxemoji = "^0.2.0"
 towncrier = "^23.11.0"
+scikit-learn = "^1.4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mass_composition-0.5.2/PKG-INFO` & `mass_composition-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.5.2
+Version: 0.6.0
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

