# Comparing `tmp/fc_pruning-0.0.6.tar.gz` & `tmp/fc_pruning-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc_pruning-0.0.6.tar", last modified: Sat May 11 14:18:40 2024, max compression
+gzip compressed data, was "fc_pruning-0.0.8.tar", last modified: Thu May 16 21:37:11 2024, max compression
```

## Comparing `fc_pruning-0.0.6.tar` & `fc_pruning-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-11 14:18:40.194762 fc_pruning-0.0.6/
--rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-04-30 18:18:40.000000 fc_pruning-0.0.6/LICENSE
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-11 14:18:40.194653 fc_pruning-0.0.6/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-30 18:18:40.000000 fc_pruning-0.0.6/README.md
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-11 14:18:40.193179 fc_pruning-0.0.6/fc_pruning/
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-11 14:18:40.194312 fc_pruning-0.0.6/fc_pruning/Compress/
--rw-r--r--   0 aidamehammed   (501) staff       (20)       49 2024-04-30 18:22:57.000000 fc_pruning-0.0.6/fc_pruning/Compress/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     5650 2024-05-11 14:18:14.000000 fc_pruning-0.0.6/fc_pruning/Compress/compress.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4137 2024-05-11 14:18:14.000000 fc_pruning-0.0.6/fc_pruning/Compress/utils.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:22:57.000000 fc_pruning-0.0.6/fc_pruning/__init__.py
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-11 14:18:40.193751 fc_pruning-0.0.6/fc_pruning.egg-info/
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      311 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/SOURCES.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/dependency_links.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/requires.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       11 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/top_level.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-11 14:18:40.194813 fc_pruning-0.0.6/setup.cfg
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1202 2024-05-11 14:18:28.000000 fc_pruning-0.0.6/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:37:11.310260 fc_pruning-0.0.8/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-04-30 18:18:40.000000 fc_pruning-0.0.8/LICENSE
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-16 21:37:11.310165 fc_pruning-0.0.8/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-30 18:18:40.000000 fc_pruning-0.0.8/README.md
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:37:11.308728 fc_pruning-0.0.8/fc_pruning/
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:37:11.309892 fc_pruning-0.0.8/fc_pruning/Compress/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       49 2024-04-30 18:22:57.000000 fc_pruning-0.0.8/fc_pruning/Compress/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     5893 2024-05-16 21:05:08.000000 fc_pruning-0.0.8/fc_pruning/Compress/compress.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4213 2024-05-11 17:52:26.000000 fc_pruning-0.0.8/fc_pruning/Compress/utils.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:22:57.000000 fc_pruning-0.0.8/fc_pruning/__init__.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:37:11.309275 fc_pruning-0.0.8/fc_pruning.egg-info/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      311 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/SOURCES.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/dependency_links.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/requires.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       11 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/top_level.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-16 21:37:11.310314 fc_pruning-0.0.8/setup.cfg
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1202 2024-05-16 21:37:07.000000 fc_pruning-0.0.8/setup.py
```

### Comparing `fc_pruning-0.0.6/LICENSE` & `fc_pruning-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.6/PKG-INFO` & `fc_pruning-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc_pruning
-Version: 0.0.6
+Version: 0.0.8
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning/issues
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.6/README.md` & `fc_pruning-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.6/fc_pruning/Compress/compress.py` & `fc_pruning-0.0.8/fc_pruning/Compress/compress.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from FeatureCloud.app.engine.app import AppState
 from typing import TypedDict, Union, List, Type
 import torch
 import torch_pruning as tp
-import sys
 
 import fc_pruning.Compress.utils as pf
 
 
 class PruningType(TypedDict):
     model: torch.nn.Module
     reference_model: Union[List[torch.nn.Module], None]
     imp: Type[tp.pruner.importance.Importance]
     ignored_layers: Union[List[torch.nn.Module], None]
     pruning_ratio: float
 
 
-class PruneAppState(AppState):
+class PruneBase(AppState):
 
     def configure_pruning(self, pruning_ratio : float = 0.5, model: torch.nn.Module = None, reference_model: Union[List[torch.nn.Module]] = None,
                          imp: Type[tp.pruner.importance.Importance] = tp.importance.MagnitudeImportance(p=2), ex_input : torch.Tensor = None,
                          ignored_layers: Union[List[torch.nn.Module], None] = None ):
 
         '''
         Configures the pruning settings for your model.
@@ -55,35 +54,89 @@
         updated_pruning['ex_input'] = ex_input
         updated_pruning['ignored_layers'] = ignored_layers
 
 
         self.store('default_pruning', updated_pruning)
 
 
+    def prune(self, data):
+        '''
+        Prunes the model and returns pruned weights and binary mask.
 
 
-    def gather_data(self, use_pruning=True, **kwargs):
+        Parameters
+        ----------
+        data : torch.nn.Module
+              The model to be pruned.
+
+        Returns
+        -------
+        data_with_mask : list
+            List of data with masks for pruning.
         '''
-                Gathers data for federated learning, including pruning if enabled.
 
-                Parameters
-                ----------
-                use_pruning : bool, optional
-                    Flag to indicate whether to use pruning. Default is True.
+        default_pruning = self.load('default_pruning')
+
+        example_input = default_pruning['ex_input']
+        ignored_layers = default_pruning['ignored_layers']
+        pruning_ratio = default_pruning['pruning_ratio']
+        model = data
+        reference_model = default_pruning['reference_model']
+        imp = default_pruning['imp']
+
+        self.store('default_pruning', default_pruning)
+        self.store('reference_model', reference_model)
+
+
+
+        self.log('start pruning...')
+
+        # exclude last_layer from pruning
+        last_layer = pf.get_last_layer(model)
+
+
+        if ignored_layers is None:
+            ignored_layers = []
+        if last_layer not in ignored_layers:
+            ignored_layers.append(last_layer)
 
 
-                Returns
-                -------
-                data : list
-                    List of data to be sent to the coordinator.
-                '''
+
+        self.log(f'Size of model before pruning: {pf.print_size_of_model(model)} MB')
+
+        binary_mask = []
+        _, mask_client_list = pf.soft_prune(model, imp, example_input,
+                                        pruning_ratio, ignored_layers)
+        binary_mask.append(mask_client_list)
+        model = pf.hard_prune(model, imp, example_input,pruning_ratio, ignored_layers)
+
+        self.log(f'Size of model after pruning: {pf.print_size_of_model(model)} MB')
+
+        data_with_mask = pf.get_weights(model) + [binary_mask]
+
+        return data_with_mask
+
+class PruneAppState(PruneBase):
+    def gather_data(self, use_pruning=True, **kwargs):
+        '''
+        Gathers data for federated learning, including pruning if enabled.
+
+        Parameters
+        ----------
+        use_pruning : bool, optional
+            Flag to indicate whether to use pruning. Default is True.
+        Returns
+        -------
+        data : list
+            List of data to be sent to the coordinator.
+        '''
         data_with_mask_list = super().gather_data(**kwargs)
 
         if use_pruning:
-            reference_model= self.load('reference_model')
+            reference_model = self.load('reference_model')
 
             # extract data and binary_mask
             data = []
             binary_mask = []
             for data_with_mask in data_with_mask_list:
                 data.append(data_with_mask[:-1])
                 binary_mask.append(data_with_mask[-1])
@@ -94,78 +147,30 @@
                 reconstructed_model = pf.reconstruct_model(data[i], binary_mask[i][0], reference_model)
                 reconstructed_clients.append(reconstructed_model)
             data = reconstructed_clients
         else:
             data = data_with_mask_list
 
         return data
-
-    def send_data_to_coordinator(self, data, use_pruning= True, **kwargs):
+ def send_data_to_coordinator(self, data, use_pruning= True, **kwargs):
         '''
             Sends data to the coordinator, including pruning if enabled.
 
             Parameters
             ----------
             data : list
                 List of data to be sent to the coordinator.
             use_pruning : bool, optional
-                Flag to indicate whether to use pruning. Default is True.
+                Flag to indicate whether to use pruning. Default is True. Enabled if no finetuning is desired.
 
             Returns
             -------
             data_with_mask : list
                 List of data with masks for pruning.
             '''
         if use_pruning:
-
-            default_pruning = self.load('default_pruning')
-
-            example_input = default_pruning['ex_input']
-            ignored_layers = default_pruning['ignored_layers']
-            pruning_ratio = default_pruning['pruning_ratio']
-            model = data
-            reference_model = default_pruning['reference_model']
-            imp = default_pruning['imp']
-
-            self.store('default_pruning', default_pruning)
-            self.store('reference_model', reference_model)
-
-
-
-            self.log('start pruning...')
-
-            # exclude last_layer from pruning
-            last_layer = pf.get_last_layer(model)
-
-
-            if ignored_layers is None:
-                ignored_layers = []
-            if last_layer not in ignored_layers:
-                ignored_layers.append(last_layer)
-
-
-
-            self.log(f'Size of model before pruning: {pf.print_size_of_model(model)} MB')
-
-            binary_mask = []
-
-            mmodel, mask_client_list = pf.soft_prune(model, imp, example_input,
-                                            pruning_ratio, ignored_layers)
-            binary_mask.append(mask_client_list)
-            model = pf.hard_prune(model, imp, example_input,pruning_ratio, ignored_layers)
-
-            # here finetuning...
-
-
-            self.log(f'Size of model after pruning: {pf.print_size_of_model(model)} MB')
-
-
-
-            data_with_mask = pf.get_weights(model) + [binary_mask]
-
+            data_with_mask = self.prune(data)
             super().send_data_to_coordinator(data_with_mask,**kwargs)
         else:
             super().send_data_to_coordinator(data, **kwargs)
             data_with_mask = data
-        return data_with_mask
-
-
+        return data_with_mask
```

### Comparing `fc_pruning-0.0.6/fc_pruning/Compress/utils.py` & `fc_pruning-0.0.8/fc_pruning/Compress/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,23 @@
         for idx, val in enumerate(param.view(-1)):
             if val == 0:
                 mask.view(-1)[idx] = 0
         mask_list.append(mask)
 
     return mask_list
 
-
 def soft_prune(model, imp, example_inputs, pruning_ratio=None, ignored_layers=None):
     pmodel = copy.deepcopy(model)
 
+    #print('error')
+
     pruner = tp.pruner.MetaPruner(
         pmodel,
         example_inputs,
+        #iterative_steps=1,
         importance=imp,
         pruning_ratio=pruning_ratio,
         ignored_layers=ignored_layers
     )
 
     print('Applying soft pruning step')
     for group in pruner.step(interactive=True):
@@ -69,14 +71,15 @@
 def hard_prune(model, imp, example_inputs, pruning_ratio=None, ignored_layers=None):
     pmodel = copy.deepcopy(model)
 
     pruner = tp.pruner.MetaPruner(
         pmodel,
         example_inputs,
         importance=imp,
+        #iterative_steps=1,
         pruning_ratio=pruning_ratio,
         ignored_layers=ignored_layers,
     )
 
     print('Applying hard pruning step')
 
     if isinstance(imp, tp.importance.TaylorImportance):
```

### Comparing `fc_pruning-0.0.6/fc_pruning.egg-info/PKG-INFO` & `fc_pruning-0.0.8/fc_pruning.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-pruning
-Version: 0.0.6
+Version: 0.0.8
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning/issues
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.6/setup.py` & `fc_pruning-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="fc_pruning",
-                 version="0.0.6",
+                 version="0.0.8",
                  author="Aida Mehammed",
                  author_email="aida.mehammed@studium.uni-hamburg.de",
                  description="FC Pruning",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AidaMehammed/fc_pruning",
                  project_urls={
```

