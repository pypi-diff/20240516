# Comparing `tmp/fedjust-0.1.2.tar.gz` & `tmp/fedjust-0.1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedjust-0.1.2.tar", max compression
+gzip compressed data, was "fedjust-0.1.2.3.tar", max compression
```

## Comparing `fedjust-0.1.2.tar` & `fedjust-0.1.2.3.tar`

### file list

```diff
@@ -1,28 +1,16 @@
--rw-r--r--   0        0        0        0 2024-04-29 21:08:19.328339 fedjust-0.1.2/FedJust/__init__.py
--rw-r--r--   0        0        0     1328 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/aggregators/__pycache__/aggregator.cpython-310.pyc
--rw-r--r--   0        0        0     2048 2024-05-02 14:26:14.580289 fedjust-0.1.2/FedJust/aggregators/__pycache__/fedopt_aggregator.cpython-310.pyc
--rw-r--r--   0        0        0     1052 2024-04-29 21:08:19.328339 fedjust-0.1.2/FedJust/aggregators/aggregator.py
--rw-r--r--   0        0        0     1443 2024-05-02 14:26:01.448570 fedjust-0.1.2/FedJust/aggregators/fedopt_aggregator.py
--rw-r--r--   0        0        0     1594 2024-05-01 11:48:27.774254 fedjust-0.1.2/FedJust/files/__pycache__/archive.cpython-310.pyc
--rw-r--r--   0        0        0     1670 2024-05-01 11:48:27.774254 fedjust-0.1.2/FedJust/files/__pycache__/handlers.cpython-310.pyc
--rw-r--r--   0        0        0      958 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/files/__pycache__/loggers.cpython-310.pyc
--rw-r--r--   0        0        0     1515 2024-05-02 14:35:56.655748 fedjust-0.1.2/FedJust/files/archive.py
--rw-r--r--   0        0        0     1721 2024-04-29 21:08:19.328339 fedjust-0.1.2/FedJust/files/handlers.py
--rw-r--r--   0        0        0     2187 2024-04-29 21:08:19.328339 fedjust-0.1.2/FedJust/files/loggers.py
--rw-r--r--   0        0        0    11104 2024-05-01 12:59:51.537271 fedjust-0.1.2/FedJust/model/__pycache__/federated_model.cpython-310.pyc
--rw-r--r--   0        0        0    15871 2024-05-01 12:59:48.121354 fedjust-0.1.2/FedJust/model/federated_model.py
--rw-r--r--   0        0        0     5227 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/node/__pycache__/federated_node.cpython-310.pyc
--rw-r--r--   0        0        0     5910 2024-04-29 21:13:37.832090 fedjust-0.1.2/FedJust/node/federated_node.py
--rw-r--r--   0        0        0     2844 2024-05-01 12:26:55.777282 fedjust-0.1.2/FedJust/operations/__pycache__/evaluations.cpython-310.pyc
--rw-r--r--   0        0        0     3648 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/operations/__pycache__/orchestrations.cpython-310.pyc
--rw-r--r--   0        0        0     3335 2024-05-01 12:25:08.143947 fedjust-0.1.2/FedJust/operations/evaluations.py
--rw-r--r--   0        0        0     3430 2024-04-29 21:08:19.332339 fedjust-0.1.2/FedJust/operations/orchestrations.py
--rw-r--r--   0        0        0     4737 2024-05-01 12:56:25.406255 fedjust-0.1.2/FedJust/simulation/__pycache__/adaptive_optimizer_simulation.cpython-310.pyc
--rw-r--r--   0        0        0     8511 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/simulation/__pycache__/simulation.cpython-310.pyc
--rw-r--r--   0        0        0     6205 2024-05-01 12:56:19.110407 fedjust-0.1.2/FedJust/simulation/adaptive_optimizer_simulation.py
--rw-r--r--   0        0        0    10659 2024-04-29 21:08:19.332339 fedjust-0.1.2/FedJust/simulation/simulation.py
--rw-r--r--   0        0        0      906 2024-05-01 12:08:02.750896 fedjust-0.1.2/FedJust/utils/__pycache__/computations.cpython-310.pyc
--rw-r--r--   0        0        0      824 2024-05-01 12:07:32.211788 fedjust-0.1.2/FedJust/utils/computations.py
--rw-r--r--   0        0        0     3091 2024-04-29 21:08:19.332339 fedjust-0.1.2/README.md
--rw-r--r--   0        0        0      426 2024-05-02 14:37:08.390196 fedjust-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3664 1970-01-01 00:00:00.000000 fedjust-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-29 21:08:19.328339 fedjust-0.1.2.3/FedJust/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-29 21:08:19.328339 fedjust-0.1.2.3/FedJust/aggregators/aggregator.py
+-rw-r--r--   0        0        0     1442 2024-05-02 14:42:59.238594 fedjust-0.1.2.3/FedJust/aggregators/fedopt_aggregator.py
+-rw-r--r--   0        0        0     1515 2024-05-02 14:35:56.655748 fedjust-0.1.2.3/FedJust/files/archive.py
+-rw-r--r--   0        0        0     1721 2024-04-29 21:08:19.328339 fedjust-0.1.2.3/FedJust/files/handlers.py
+-rw-r--r--   0        0        0     2187 2024-04-29 21:08:19.328339 fedjust-0.1.2.3/FedJust/files/loggers.py
+-rw-r--r--   0        0        0    17018 2024-05-16 12:12:29.810973 fedjust-0.1.2.3/FedJust/model/federated_model.py
+-rw-r--r--   0        0        0     5910 2024-04-29 21:13:37.832090 fedjust-0.1.2.3/FedJust/node/federated_node.py
+-rw-r--r--   0        0        0     3335 2024-05-01 12:25:08.143947 fedjust-0.1.2.3/FedJust/operations/evaluations.py
+-rw-r--r--   0        0        0     3430 2024-04-29 21:08:19.332339 fedjust-0.1.2.3/FedJust/operations/orchestrations.py
+-rw-r--r--   0        0        0     6205 2024-05-01 12:56:19.110407 fedjust-0.1.2.3/FedJust/simulation/adaptive_optimizer_simulation.py
+-rw-r--r--   0        0        0    10659 2024-04-29 21:08:19.332339 fedjust-0.1.2.3/FedJust/simulation/simulation.py
+-rw-r--r--   0        0        0      824 2024-05-01 12:07:32.211788 fedjust-0.1.2.3/FedJust/utils/computations.py
+-rw-r--r--   0        0        0     3091 2024-04-29 21:08:19.332339 fedjust-0.1.2.3/README.md
+-rw-r--r--   0        0        0      428 2024-05-16 12:33:46.988040 fedjust-0.1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 fedjust-0.1.2.3/PKG-INFO
```

### Comparing `fedjust-0.1.2/FedJust/aggregators/aggregator.py` & `fedjust-0.1.2.3/FedJust/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/FedJust/aggregators/fedopt_aggregator.py` & `fedjust-0.1.2.3/FedJust/aggregators/fedopt_aggregator.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,9 +40,9 @@
             Learning rate used to 
         
         Returns
         -------
         OrderedDict"""        
         updated_weights = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
         for key in weights:
-            updated_weights[key] = weights[key] + (learning_rate * (-gradients[key]))
+            updated_weights[key] = weights[key] + (learning_rate * (gradients[key]))
         return updated_weights
```

### Comparing `fedjust-0.1.2/FedJust/files/archive.py` & `fedjust-0.1.2.3/FedJust/files/archive.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/FedJust/files/handlers.py` & `fedjust-0.1.2.3/FedJust/files/handlers.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/FedJust/files/loggers.py` & `fedjust-0.1.2.3/FedJust/files/loggers.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/FedJust/model/federated_model.py` & `fedjust-0.1.2.3/FedJust/model/federated_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,51 +72,68 @@
         self.optimizer = optimizer_template(params_to_update)
         
 
     def attach_dataset_id(
         self,
         local_dataset: list[datasets.arrow_dataset.Dataset, datasets.arrow_dataset.Dataset] | list[datasets.arrow_dataset.Dataset],
         node_name: int | str,
-        only_test: bool = False
+        only_test: bool = False,
+        hugging_face_map: bool = True
         ) -> None:
         """Attaches huggingface dataset to the model by firstly converting it into a pytorch-appropiate standard.
         
         Parameters
         ----------
         local_dataset: list[datasets.arrow_dataset.Dataset] 
             A local dataset that should be loaded into DataLoader
         node_name: int | str
             The name of the node attributed to particular dataset
         only_test: bool [default to False]: 
             If true, only a test set will be returned
         batch_size: int [default to 32]:
             Batch size used in test and train loader
-        
+        higging_face_map: bool [default to True]:
+            If set to True, will use hugging face map function,
+            that takes more time to process but results in a more
+            stable and reversable transformation of the results.
         Returns
         -------------
         None
         """
         self.node_name = node_name
         if only_test == False:
-            local_dataset[0] = local_dataset[0].with_transform(self.transform_func)
-            local_dataset[1] = local_dataset[1].with_transform(self.transform_func)
+            if hugging_face_map:
+                convert_tensor = transforms.ToTensor()
+                local_dataset[0] = local_dataset[0].map(lambda sample: {"image": convert_tensor(sample['image'])})
+                local_dataset[0].set_format("pt", columns=["image"], output_all_columns=True)
+                    
+                local_dataset[1] = local_dataset[1].map(lambda sample: {"image": convert_tensor(sample['image'])})
+                local_dataset[1].set_format("pt", columns=["image"], output_all_columns=True)
+            else:
+                local_dataset[0] = local_dataset[0].with_transform(self.transform_func)
+                local_dataset[1] = local_dataset[1].with_transform(self.transform_func)
             self.trainloader = torch.utils.data.DataLoader(
                 local_dataset[0],
                 batch_size=self.batch_size,
                 shuffle=True,
                 num_workers=0,
             )
             self.testloader = torch.utils.data.DataLoader(
                 local_dataset[1],
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=0,
             )
         else:
-            local_dataset[0] = local_dataset[0].with_transform(self.transform_func)
+            if hugging_face_map:
+                convert_tensor = transforms.ToTensor()
+                local_dataset[0] = local_dataset[0].map(lambda sample: {"image": convert_tensor(sample['image'])})
+                local_dataset[0].set_format("pt", columns=["image"], output_all_columns=True)
+            else:
+                local_dataset[0] = local_dataset[0].with_transform(self.transform_func)
             self.testloader = torch.utils.data.DataLoader(
                 local_dataset[0],
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=0,
             )
```

### Comparing `fedjust-0.1.2/FedJust/node/federated_node.py` & `fedjust-0.1.2.3/FedJust/node/federated_node.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/FedJust/operations/__pycache__/orchestrations.cpython-310.pyc` & `fedjust-0.1.2.3/FedJust/operations/orchestrations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,228 +1,215 @@
-00000000: 6f0d 0d0a 0000 0000 430c 3066 660d 0000  o.......C.0ff...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0014 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 5a05 6400  m.Z...d.d.l.Z.d.
-00000050: 6404 6c06 6d07 5a07 0100 0905 0906 0903  d.l.m.Z.........
-00000060: 6418 6407 6507 6408 6508 6409 6508 640a  d.d.e.d.e.d.e.d.
-00000070: 6509 640b 650a 640c 6509 640d 650b 6508  e.d.e.d.e.d.e.e.
-00000080: 6503 6501 650c 1900 6501 650c 1900 6604  e.e.e...e.e...f.
-00000090: 1900 660e 640e 640f 8405 5a0d 6410 650e  ..f.d.d...Z.d.e.
-000000a0: 6508 6507 8502 1900 6411 6508 6412 6505  e.e.....d.e.d.e.
-000000b0: 6a0f 6a10 640d 650e 6511 6507 8502 1900  j.j.d.e.e.e.....
-000000c0: 6608 6413 6414 8404 5a12 6410 650e 6508  f.d.d...Z.d.e.e.
-000000d0: 6507 8502 1900 6411 6508 6412 6505 6a0f  e.....d.e.d.e.j.
-000000e0: 6a10 6415 6505 6a13 640d 650e 6511 6507  j.d.e.j.d.e.e.e.
-000000f0: 8502 1900 660a 6416 6417 8404 5a14 6403  ....f.d.d...Z.d.
-00000100: 5300 2919 e900 0000 0029 01da 044c 6973  S.)......)...Lis
-00000110: 7429 01da 0b4f 7264 6572 6564 4469 6374  t)...OrderedDict
-00000120: 4e29 01da 0d46 6564 6572 6174 6564 4e6f  N)...FederatedNo
-00000130: 6465 da07 7765 6967 6874 7346 da04 6e6f  de..weightsF..no
-00000140: 6465 da09 6974 6572 6174 696f 6eda 0c6c  de..iteration..l
-00000150: 6f63 616c 5f65 706f 6368 73da 046d 6f64  ocal_epochs..mod
-00000160: 65da 0a73 6176 655f 6d6f 6465 6cda 0973  e..save_model..s
-00000170: 6176 655f 7061 7468 da06 7265 7475 726e  ave_path..return
-00000180: 6306 0000 0000 0000 0000 0000 000a 0000  c...............
-00000190: 0007 0000 0043 0000 0073 2800 0000 7c00  .....C...s(...|.
-000001a0: 6a00 7c01 7c02 7c03 7c04 7c05 6401 8d05  j.|.|.|.|.|.d...
-000001b0: 5c04 7d06 7d07 7d08 7d09 7c06 7c07 7c08  \.}.}.}.}.|.|.|.
-000001c0: 7c09 6604 5300 2902 6139 0300 0055 7365  |.f.S.).a9...Use
-000001d0: 6420 746f 2063 6f6d 6d61 6e64 2074 6865  d to command the
-000001e0: 206e 6f64 6520 746f 2073 7461 7274 2074   node to start t
-000001f0: 6865 206c 6f63 616c 2074 7261 696e 696e  he local trainin
-00000200: 672e 0a20 2020 2049 6e76 6f6b 6573 202e  g..    Invokes .
-00000210: 7472 6169 6e5f 6c6f 6361 6c5f 6d6f 6465  train_local_mode
-00000220: 6c20 6d65 7468 6f64 2061 6e64 2072 6574  l method and ret
-00000230: 7572 6e73 2074 6865 2072 6573 756c 7473  urns the results
-00000240: 2e0a 2020 2020 0a20 2020 2050 6172 616d  ..    .    Param
-00000250: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00000260: 2d2d 2d2d 0a20 2020 206e 6f64 653a 2046  ----.    node: F
-00000270: 6564 6572 6174 6564 4e6f 6465 200a 2020  ederatedNode .  
-00000280: 2020 2020 2020 4e6f 6465 2074 6861 7420        Node that 
-00000290: 7765 2077 616e 7420 746f 2074 7261 696e  we want to train
-000002a0: 2e0a 2020 2020 6974 6572 6174 696f 6e3a  ..    iteration:
-000002b0: 2069 6e74 0a20 2020 2020 2020 2043 7572   int.        Cur
-000002c0: 7265 6e74 2028 676c 6f62 616c 2920 6974  rent (global) it
-000002d0: 6572 6174 696f 6e2e 0a20 2020 206c 6f63  eration..    loc
-000002e0: 616c 5f65 706f 6368 733a 2069 6e74 0a20  al_epochs: int. 
-000002f0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
-00000300: 206c 6f63 616c 2065 706f 6368 7320 666f   local epochs fo
-00000310: 7220 7768 6963 6820 746f 2074 7261 696e  r which to train
-00000320: 2061 206e 6f64 650a 2020 2020 6d6f 6465   a node.    mode
-00000330: 3a20 7374 7220 2864 6566 6175 6c74 2074  : str (default t
-00000340: 6f20 4661 6c73 6529 0a20 2020 2020 2020  o False).       
-00000350: 204d 6f64 6520 6f66 2074 6865 2074 7261   Mode of the tra
-00000360: 696e 696e 672e 200a 2020 2020 2020 2020  ining. .        
-00000370: 4d6f 6465 203d 2027 7765 6967 6874 7327  Mode = 'weights'
-00000380: 3a20 4e6f 6465 2077 696c 6c20 7265 7475  : Node will retu
-00000390: 726e 206d 6f64 656c 2773 2077 6569 6768  rn model's weigh
-000003a0: 7473 2e0a 2020 2020 2020 2020 4d6f 6465  ts..        Mode
-000003b0: 203d 2027 6772 6164 6965 6e74 7327 3a20   = 'gradients': 
-000003c0: 4e6f 6465 2077 696c 6c20 7265 7475 726e  Node will return
-000003d0: 206d 6f64 656c 2773 2067 7261 6469 656e   model's gradien
-000003e0: 7473 2e0a 2020 2020 7361 7665 5f6d 6f64  ts..    save_mod
-000003f0: 656c 3a20 626f 6f6c 2028 6465 6661 756c  el: bool (defaul
-00000400: 7420 746f 2046 616c 7365 290a 2020 2020  t to False).    
-00000410: 2020 2020 426f 6f6c 6561 6e20 666c 6167      Boolean flag
-00000420: 2074 6f20 656e 6162 6c65 206d 6f64 656c   to enable model
-00000430: 2073 6176 696e 672e 0a20 2020 2073 6176   saving..    sav
-00000440: 655f 7061 7468 3a20 7374 7220 2864 6566  e_path: str (def
-00000450: 6175 6c74 2074 6f20 4e6f 6e65 290a 2020  ault to None).  
-00000460: 2020 2020 2020 5361 7665 2070 6174 6820        Save path 
-00000470: 666f 7220 7072 6573 6572 7669 6e67 2061  for preserving a
-00000480: 206d 6f64 656c 2028 6170 706c 6963 6162   model (applicab
-00000490: 6c65 206f 6e6c 7920 7768 656e 2073 6176  le only when sav
-000004a0: 655f 6d6f 6465 6c20 3d20 5472 7565 290a  e_model = True).
-000004b0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000004c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000004d0: 7470 756c 655b 696e 742c 204f 7264 6572  tpule[int, Order
-000004e0: 6564 4469 6374 2c20 4c69 7374 5b66 6c6f  edDict, List[flo
-000004f0: 6174 5d2c 204c 6973 745b 666c 6f61 745d  at], List[float]
-00000500: 5d0a 2020 2020 2905 7207 0000 0072 0800  ].    ).r....r..
-00000510: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000520: 0029 01da 1174 7261 696e 5f6c 6f63 616c  .)...train_local
-00000530: 5f6d 6f64 656c 290a 7206 0000 0072 0700  _model).r....r..
-00000540: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000550: 0072 0b00 0000 da07 6e6f 6465 5f69 6472  .r......node_idr
-00000560: 0500 0000 da09 6c6f 7373 5f6c 6973 74da  ......loss_list.
-00000570: 0d61 6363 7572 6163 795f 6c69 7374 a900  .accuracy_list..
-00000580: 7211 0000 00fa 662f 686f 6d65 2f6d 7a75  r.....f/home/mzu
-00000590: 7a69 616b 2f73 6e61 702f 736e 6170 642d  ziak/snap/snapd-
-000005a0: 6465 736b 746f 702d 696e 7465 6772 6174  desktop-integrat
-000005b0: 696f 6e2f 3833 2f44 6f63 756d 656e 7473  ion/83/Documents
-000005c0: 2f46 6564 4a75 7374 2f46 6564 4a75 7374  /FedJust/FedJust
-000005d0: 2f6f 7065 7261 7469 6f6e 732f 6f72 6368  /operations/orch
-000005e0: 6573 7472 6174 696f 6e73 2e70 79da 0b74  estrations.py..t
-000005f0: 7261 696e 5f6e 6f64 6573 0800 0000 7310  rain_nodes....s.
-00000600: 0000 0004 1e02 0102 0102 0102 0102 010e  ................
-00000610: fb0c 0672 1300 0000 da05 6e6f 6465 73da  ...r......nodes.
-00000620: 0b73 616d 706c 655f 7369 7a65 da09 6765  .sample_size..ge
-00000630: 6e65 7261 746f 7263 0300 0000 0000 0000  neratorc........
-00000640: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
-00000650: 732a 0000 007c 026a 0074 017c 00a0 02a1  s*...|.j.t.|....
-00000660: 0083 017c 0164 0164 028d 037d 0364 0364  ...|.d.d...}.d.d
-00000670: 0484 007c 0344 0083 017d 037c 0353 0029  ...|.D...}.|.S.)
-00000680: 0561 0702 0000 5361 6d70 6c65 2074 6865  .a....Sample the
-00000690: 206e 6f64 6573 2067 6976 656e 2074 6865   nodes given the
-000006a0: 2070 726f 7669 6465 6420 7361 6d70 6c65   provided sample
-000006b0: 2073 697a 652e 2049 6620 7361 6d70 6c65   size. If sample
-000006c0: 5f73 697a 6520 6973 2062 6967 6765 720a  _size is bigger.
-000006d0: 2020 2020 6f72 2065 7175 616c 2074 6f20      or equal to 
-000006e0: 7468 6520 6e75 6d62 6572 206f 6620 6176  the number of av
-000006f0: 2e20 6e6f 6465 732c 2074 6865 2073 616d  . nodes, the sam
-00000700: 706c 6572 2077 696c 6c20 7265 7475 726e  pler will return
-00000710: 2074 6865 206f 7269 6769 6e61 6c20 6c69   the original li
-00000720: 7374 2e0a 2020 2020 0a20 2020 2050 6172  st..    .    Par
-00000730: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00000740: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206e  ------.        n
-00000750: 6f64 6573 3a20 6469 6374 5b69 6e74 3a20  odes: dict[int: 
-00000760: 4665 6465 7261 7465 644e 6f64 655d 2920  FederatedNode]) 
-00000770: 0a20 2020 2020 2020 2020 2020 204f 7269  .            Ori
-00000780: 6769 6e61 6c20 6469 6374 696f 6e61 7279  ginal dictionary
-00000790: 206f 6620 6e6f 6465 7320 746f 2062 6520   of nodes to be 
-000007a0: 7361 6d70 6c65 6420 6672 6f6d 2e0a 2020  sampled from..  
-000007b0: 2020 2020 2020 7361 6d70 6c65 5f73 697a        sample_siz
-000007c0: 653a 2069 6e74 2c0a 2020 2020 2020 2020  e: int,.        
-000007d0: 2020 2020 5369 7a65 206f 6620 7468 6520      Size of the 
-000007e0: 7361 6d70 6c65 0a20 2020 2020 2020 2067  sample.        g
-000007f0: 656e 6572 6174 6f72 3a20 6e70 2e72 616e  enerator: np.ran
-00000800: 646f 6d2e 4765 6e65 7261 746f 720a 2020  dom.Generator.  
-00000810: 2020 2020 2020 2020 2020 4120 6e75 6d70            A nump
-00000820: 7920 6765 6e65 7261 746f 7220 696e 6974  y generator init
-00000830: 6961 6c69 7a65 6420 6f6e 2074 6865 2073  ialized on the s
-00000840: 6572 7665 7220 7369 6465 2e0a 2020 2020  erver side..    
-00000850: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-00000860: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00000870: 2064 6963 745b 6964 3a20 4665 6465 7261   dict[id: Federa
-00000880: 7465 644e 6f64 655d 0a20 2020 2046 2902  tedNode].    F).
-00000890: da04 7369 7a65 da07 7265 706c 6163 6563  ..size..replacec
-000008a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000008b0: 0400 0000 5300 0000 f314 0000 0069 007c  ....S........i.|
-000008c0: 005d 067d 017c 016a 007c 0193 0271 0253  .].}.|.j.|...q.S
-000008d0: 0072 1100 0000 a901 720e 0000 00a9 02da  .r......r.......
-000008e0: 022e 3072 0600 0000 7211 0000 0072 1100  ..0r....r....r..
-000008f0: 0000 7212 0000 00da 0a3c 6469 6374 636f  ..r......<dictco
-00000900: 6d70 3e43 0000 00f3 0200 0000 1400 7a20  mp>C..........z 
-00000910: 7361 6d70 6c65 5f6e 6f64 6573 2e3c 6c6f  sample_nodes.<lo
-00000920: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-00000930: 2903 da06 6368 6f69 6365 da04 6c69 7374  )...choice..list
-00000940: da06 7661 6c75 6573 2904 7214 0000 0072  ..values).r....r
-00000950: 1500 0000 7216 0000 00da 0673 616d 706c  ....r......sampl
-00000960: 6572 1100 0000 7211 0000 0072 1200 0000  er....r....r....
-00000970: da0c 7361 6d70 6c65 5f6e 6f64 6573 2f00  ..sample_nodes/.
-00000980: 0000 7306 0000 0018 130e 0104 0172 2300  ..s..........r#.
-00000990: 0000 da0e 7361 6d70 6c69 6e67 5f61 7272  ....sampling_arr
-000009a0: 6179 6304 0000 0000 0000 0000 0000 0005  ayc.............
-000009b0: 0000 0006 0000 0043 0000 0073 2400 0000  .......C...s$...
-000009c0: 7c02 6a00 7c00 7c01 7c03 6401 6402 8d04  |.j.|.|.|.d.d...
-000009d0: 7d04 6403 6404 8400 7c04 4400 8301 7d04  }.d.d...|.D...}.
-000009e0: 7c04 5300 2905 6159 0200 0053 616d 706c  |.S.).aY...Sampl
-000009f0: 6520 7468 6520 6e6f 6465 7320 6769 7665  e the nodes give
-00000a00: 6e20 7468 6520 7072 6f76 6964 6564 2073  n the provided s
-00000a10: 616d 706c 6520 7369 7a65 2e20 4974 2072  ample size. It r
-00000a20: 6571 7569 7265 7320 7061 7373 696e 6720  equires passing 
-00000a30: 6120 7361 6d70 6c69 6e67 2061 7272 6179  a sampling array
-00000a40: 0a20 2020 2063 6f6e 7461 696e 696e 6720  .    containing 
-00000a50: 6c69 7374 206f 6620 7765 6967 6874 7320  list of weights 
-00000a60: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-00000a70: 6561 6368 206e 6f64 652e 0a20 2020 200a  each node..    .
-00000a80: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000a90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000aa0: 2020 2020 2020 6e6f 6465 733a 2064 6963        nodes: dic
-00000ab0: 745b 696e 743a 2046 6564 6572 6174 6564  t[int: Federated
-00000ac0: 4e6f 6465 5d29 200a 2020 2020 2020 2020  Node]) .        
-00000ad0: 2020 2020 4f72 6967 696e 616c 2064 6963      Original dic
-00000ae0: 7469 6f6e 6172 7920 6f66 206e 6f64 6573  tionary of nodes
-00000af0: 2074 6f20 6265 2073 616d 706c 6564 2066   to be sampled f
-00000b00: 726f 6d2e 0a20 2020 2020 2020 2073 616d  rom..        sam
-00000b10: 706c 655f 7369 7a65 3a20 696e 742c 0a20  ple_size: int,. 
-00000b20: 2020 2020 2020 2020 2020 2053 697a 6520             Size 
-00000b30: 6f66 2074 6865 2073 616d 706c 650a 2020  of the sample.  
-00000b40: 2020 2020 2020 6765 6e65 7261 746f 723a        generator:
-00000b50: 206e 702e 7261 6e64 6f6d 2e47 656e 6572   np.random.Gener
-00000b60: 6174 6f72 0a20 2020 2020 2020 2020 2020  ator.           
-00000b70: 2041 206e 756d 7079 2067 656e 6572 6174   A numpy generat
-00000b80: 6f72 2069 6e69 7469 616c 697a 6564 206f  or initialized o
-00000b90: 6e20 7468 6520 7365 7276 6572 2073 6964  n the server sid
-00000ba0: 652e 0a20 2020 2020 2020 2073 616d 706c  e..        sampl
-00000bb0: 696e 675f 6172 7261 793a 206e 702e 6172  ing_array: np.ar
-00000bc0: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-00000bd0: 5361 6d70 6c69 6e67 2061 7272 6179 2063  Sampling array c
-00000be0: 6f6e 7461 696e 696e 6720 7765 6967 6874  ontaining weight
-00000bf0: 7320 666f 7220 7468 6520 7361 6d70 6c69  s for the sampli
-00000c00: 6e67 0a20 2020 200a 2020 2020 5265 7475  ng.    .    Retu
-00000c10: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00000c20: 2020 2020 2020 2020 6469 6374 5b69 643a          dict[id:
-00000c30: 2046 6564 6572 6174 6564 4e6f 6465 5d0a   FederatedNode].
-00000c40: 2020 2020 4629 0372 1700 0000 da01 7072      F).r......pr
-00000c50: 1800 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00000c60: 0002 0000 0004 0000 0053 0000 0072 1900  .........S...r..
-00000c70: 0000 7211 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000c80: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-00000c90: 721d 0000 005e 0000 0072 1e00 0000 7a29  r....^...r....z)
-00000ca0: 7361 6d70 6c65 5f77 6569 6768 7465 645f  sample_weighted_
-00000cb0: 6e6f 6465 732e 3c6c 6f63 616c 733e 2e3c  nodes.<locals>.<
-00000cc0: 6469 6374 636f 6d70 3e29 0172 1f00 0000  dictcomp>).r....
-00000cd0: 2905 7214 0000 0072 1500 0000 7216 0000  ).r....r....r...
-00000ce0: 0072 2400 0000 7222 0000 0072 1100 0000  .r$...r"...r....
-00000cf0: 7211 0000 0072 1200 0000 da15 7361 6d70  r....r......samp
-00000d00: 6c65 5f77 6569 6768 7465 645f 6e6f 6465  le_weighted_node
-00000d10: 7347 0000 0073 0600 0000 1216 0e01 0401  sG...s..........
-00000d20: 7226 0000 0029 0372 0500 0000 464e 2915  r&...).r....FN).
-00000d30: da06 7479 7069 6e67 7202 0000 00da 0b63  ..typingr......c
-00000d40: 6f6c 6c65 6374 696f 6e73 7203 0000 00da  ollectionsr.....
-00000d50: 056e 756d 7079 da02 6e70 da1b 4665 644a  .numpy..np..FedJ
-00000d60: 7573 742e 6e6f 6465 2e66 6564 6572 6174  ust.node.federat
-00000d70: 6564 5f6e 6f64 6572 0400 0000 da03 696e  ed_noder......in
-00000d80: 74da 0373 7472 da04 626f 6f6c da05 7475  t..str..bool..tu
-00000d90: 706c 65da 0566 6c6f 6174 7213 0000 00da  ple..floatr.....
-00000da0: 0464 6963 74da 0672 616e 646f 6dda 0947  .dict..random..G
-00000db0: 656e 6572 6174 6f72 da02 6964 7223 0000  enerator..idr#..
-00000dc0: 00da 0561 7272 6179 7226 0000 0072 1100  ...arrayr&...r..
-00000dd0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00000de0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000df0: 4c00 0000 0c00 0c01 0802 0c02 0206 0201  L...............
-00000e00: 0201 04fa 0201 02ff 0202 02fe 0203 02fd  ................
-00000e10: 0204 02fc 0205 02fb 0206 02fa 1606 0afa  ................
-00000e20: 0e27 0201 02ff 0602 02fe 0a02 0afe 0e18  .'..............
-00000e30: 0201 02ff 0602 02fe 0403 02fd 0a03 0efd  ................
+00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000010: 7274 204c 6973 740a 6672 6f6d 2063 6f6c  rt List.from col
+00000020: 6c65 6374 696f 6e73 2069 6d70 6f72 7420  lections import 
+00000030: 4f72 6465 7265 6444 6963 740a 0a69 6d70  OrderedDict..imp
+00000040: 6f72 7420 6e75 6d70 7920 6173 206e 7020  ort numpy as np 
+00000050: 200a 0a66 726f 6d20 4665 644a 7573 742e   ..from FedJust.
+00000060: 6e6f 6465 2e66 6564 6572 6174 6564 5f6e  node.federated_n
+00000070: 6f64 6520 696d 706f 7274 2046 6564 6572  ode import Feder
+00000080: 6174 6564 4e6f 6465 0a0a 6465 6620 7472  atedNode..def tr
+00000090: 6169 6e5f 6e6f 6465 7328 0a20 2020 206e  ain_nodes(.    n
+000000a0: 6f64 653a 2046 6564 6572 6174 6564 4e6f  ode: FederatedNo
+000000b0: 6465 2c0a 2020 2020 6974 6572 6174 696f  de,.    iteratio
+000000c0: 6e3a 2069 6e74 2c0a 2020 2020 6c6f 6361  n: int,.    loca
+000000d0: 6c5f 6570 6f63 6873 3a20 696e 742c 0a20  l_epochs: int,. 
+000000e0: 2020 206d 6f64 653a 2073 7472 203d 2027     mode: str = '
+000000f0: 7765 6967 6874 7327 2c0a 2020 2020 7361  weights',.    sa
+00000100: 7665 5f6d 6f64 656c 3a20 626f 6f6c 203d  ve_model: bool =
+00000110: 2046 616c 7365 2c0a 2020 2020 7361 7665   False,.    save
+00000120: 5f70 6174 683a 2073 7472 203d 204e 6f6e  _path: str = Non
+00000130: 6529 202d 3e20 7475 706c 655b 696e 742c  e) -> tuple[int,
+00000140: 204f 7264 6572 6564 4469 6374 2c20 4c69   OrderedDict, Li
+00000150: 7374 5b66 6c6f 6174 5d2c 204c 6973 745b  st[float], List[
+00000160: 666c 6f61 745d 5d3a 0a20 2020 2022 2222  float]]:.    """
+00000170: 5573 6564 2074 6f20 636f 6d6d 616e 6420  Used to command 
+00000180: 7468 6520 6e6f 6465 2074 6f20 7374 6172  the node to star
+00000190: 7420 7468 6520 6c6f 6361 6c20 7472 6169  t the local trai
+000001a0: 6e69 6e67 2e0a 2020 2020 496e 766f 6b65  ning..    Invoke
+000001b0: 7320 2e74 7261 696e 5f6c 6f63 616c 5f6d  s .train_local_m
+000001c0: 6f64 656c 206d 6574 686f 6420 616e 6420  odel method and 
+000001d0: 7265 7475 726e 7320 7468 6520 7265 7375  returns the resu
+000001e0: 6c74 732e 0a20 2020 200a 2020 2020 5061  lts..    .    Pa
+000001f0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00000200: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e6f 6465  -------.    node
+00000210: 3a20 4665 6465 7261 7465 644e 6f64 6520  : FederatedNode 
+00000220: 0a20 2020 2020 2020 204e 6f64 6520 7468  .        Node th
+00000230: 6174 2077 6520 7761 6e74 2074 6f20 7472  at we want to tr
+00000240: 6169 6e2e 0a20 2020 2069 7465 7261 7469  ain..    iterati
+00000250: 6f6e 3a20 696e 740a 2020 2020 2020 2020  on: int.        
+00000260: 4375 7272 656e 7420 2867 6c6f 6261 6c29  Current (global)
+00000270: 2069 7465 7261 7469 6f6e 2e0a 2020 2020   iteration..    
+00000280: 6c6f 6361 6c5f 6570 6f63 6873 3a20 696e  local_epochs: in
+00000290: 740a 2020 2020 2020 2020 4e75 6d62 6572  t.        Number
+000002a0: 206f 6620 6c6f 6361 6c20 6570 6f63 6873   of local epochs
+000002b0: 2066 6f72 2077 6869 6368 2074 6f20 7472   for which to tr
+000002c0: 6169 6e20 6120 6e6f 6465 0a20 2020 206d  ain a node.    m
+000002d0: 6f64 653a 2073 7472 2028 6465 6661 756c  ode: str (defaul
+000002e0: 7420 746f 2046 616c 7365 290a 2020 2020  t to False).    
+000002f0: 2020 2020 4d6f 6465 206f 6620 7468 6520      Mode of the 
+00000300: 7472 6169 6e69 6e67 2e20 0a20 2020 2020  training. .     
+00000310: 2020 204d 6f64 6520 3d20 2777 6569 6768     Mode = 'weigh
+00000320: 7473 273a 204e 6f64 6520 7769 6c6c 2072  ts': Node will r
+00000330: 6574 7572 6e20 6d6f 6465 6c27 7320 7765  eturn model's we
+00000340: 6967 6874 732e 0a20 2020 2020 2020 204d  ights..        M
+00000350: 6f64 6520 3d20 2767 7261 6469 656e 7473  ode = 'gradients
+00000360: 273a 204e 6f64 6520 7769 6c6c 2072 6574  ': Node will ret
+00000370: 7572 6e20 6d6f 6465 6c27 7320 6772 6164  urn model's grad
+00000380: 6965 6e74 732e 0a20 2020 2073 6176 655f  ients..    save_
+00000390: 6d6f 6465 6c3a 2062 6f6f 6c20 2864 6566  model: bool (def
+000003a0: 6175 6c74 2074 6f20 4661 6c73 6529 0a20  ault to False). 
+000003b0: 2020 2020 2020 2042 6f6f 6c65 616e 2066         Boolean f
+000003c0: 6c61 6720 746f 2065 6e61 626c 6520 6d6f  lag to enable mo
+000003d0: 6465 6c20 7361 7669 6e67 2e0a 2020 2020  del saving..    
+000003e0: 7361 7665 5f70 6174 683a 2073 7472 2028  save_path: str (
+000003f0: 6465 6661 756c 7420 746f 204e 6f6e 6529  default to None)
+00000400: 0a20 2020 2020 2020 2053 6176 6520 7061  .        Save pa
+00000410: 7468 2066 6f72 2070 7265 7365 7276 696e  th for preservin
+00000420: 6720 6120 6d6f 6465 6c20 2861 7070 6c69  g a model (appli
+00000430: 6361 626c 6520 6f6e 6c79 2077 6865 6e20  cable only when 
+00000440: 7361 7665 5f6d 6f64 656c 203d 2054 7275  save_model = Tru
+00000450: 6529 0a20 2020 2052 6574 7572 6e73 0a20  e).    Returns. 
+00000460: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00000470: 2020 2074 7075 6c65 5b69 6e74 2c20 4f72     tpule[int, Or
+00000480: 6465 7265 6444 6963 742c 204c 6973 745b  deredDict, List[
+00000490: 666c 6f61 745d 2c20 4c69 7374 5b66 6c6f  float], List[flo
+000004a0: 6174 5d5d 0a20 2020 2022 2222 0a20 2020  at]].    """.   
+000004b0: 206e 6f64 655f 6964 2c20 7765 6967 6874   node_id, weight
+000004c0: 732c 206c 6f73 735f 6c69 7374 2c20 6163  s, loss_list, ac
+000004d0: 6375 7261 6379 5f6c 6973 7420 3d20 6e6f  curacy_list = no
+000004e0: 6465 2e74 7261 696e 5f6c 6f63 616c 5f6d  de.train_local_m
+000004f0: 6f64 656c 280a 2020 2020 2020 2020 6974  odel(.        it
+00000500: 6572 6174 696f 6e20 3d20 6974 6572 6174  eration = iterat
+00000510: 696f 6e2c 0a20 2020 2020 2020 206c 6f63  ion,.        loc
+00000520: 616c 5f65 706f 6368 7320 3d20 6c6f 6361  al_epochs = loca
+00000530: 6c5f 6570 6f63 6873 2c0a 2020 2020 2020  l_epochs,.      
+00000540: 2020 6d6f 6465 203d 206d 6f64 652c 0a20    mode = mode,. 
+00000550: 2020 2020 2020 2073 6176 655f 6d6f 6465         save_mode
+00000560: 6c20 3d20 7361 7665 5f6d 6f64 656c 2c0a  l = save_model,.
+00000570: 2020 2020 2020 2020 7361 7665 5f70 6174          save_pat
+00000580: 683d 7361 7665 5f70 6174 6829 0a20 2020  h=save_path).   
+00000590: 2072 6574 7572 6e20 286e 6f64 655f 6964   return (node_id
+000005a0: 2c20 7765 6967 6874 732c 206c 6f73 735f  , weights, loss_
+000005b0: 6c69 7374 2c20 6163 6375 7261 6379 5f6c  list, accuracy_l
+000005c0: 6973 7429 0a0a 0a64 6566 2073 616d 706c  ist)...def sampl
+000005d0: 655f 6e6f 6465 7328 6e6f 6465 733a 2064  e_nodes(nodes: d
+000005e0: 6963 745b 696e 743a 2046 6564 6572 6174  ict[int: Federat
+000005f0: 6564 4e6f 6465 5d2c 200a 2020 2020 2020  edNode], .      
+00000600: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
+00000610: 655f 7369 7a65 3a20 696e 742c 0a20 2020  e_size: int,.   
+00000620: 2020 2020 2020 2020 2020 2020 2020 6765                ge
+00000630: 6e65 7261 746f 723a 206e 702e 7261 6e64  nerator: np.rand
+00000640: 6f6d 2e47 656e 6572 6174 6f72 2920 2d3e  om.Generator) ->
+00000650: 2064 6963 745b 6964 3a20 4665 6465 7261   dict[id: Federa
+00000660: 7465 644e 6f64 655d 3a0a 2020 2020 2222  tedNode]:.    ""
+00000670: 2253 616d 706c 6520 7468 6520 6e6f 6465  "Sample the node
+00000680: 7320 6769 7665 6e20 7468 6520 7072 6f76  s given the prov
+00000690: 6964 6564 2073 616d 706c 6520 7369 7a65  ided sample size
+000006a0: 2e20 4966 2073 616d 706c 655f 7369 7a65  . If sample_size
+000006b0: 2069 7320 6269 6767 6572 0a20 2020 206f   is bigger.    o
+000006c0: 7220 6571 7561 6c20 746f 2074 6865 206e  r equal to the n
+000006d0: 756d 6265 7220 6f66 2061 762e 206e 6f64  umber of av. nod
+000006e0: 6573 2c20 7468 6520 7361 6d70 6c65 7220  es, the sampler 
+000006f0: 7769 6c6c 2072 6574 7572 6e20 7468 6520  will return the 
+00000700: 6f72 6967 696e 616c 206c 6973 742e 0a20  original list.. 
+00000710: 2020 200a 2020 2020 5061 7261 6d65 7465     .    Paramete
+00000720: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00000730: 2d0a 2020 2020 2020 2020 6e6f 6465 733a  -.        nodes:
+00000740: 2064 6963 745b 696e 743a 2046 6564 6572   dict[int: Feder
+00000750: 6174 6564 4e6f 6465 5d29 200a 2020 2020  atedNode]) .    
+00000760: 2020 2020 2020 2020 4f72 6967 696e 616c          Original
+00000770: 2064 6963 7469 6f6e 6172 7920 6f66 206e   dictionary of n
+00000780: 6f64 6573 2074 6f20 6265 2073 616d 706c  odes to be sampl
+00000790: 6564 2066 726f 6d2e 0a20 2020 2020 2020  ed from..       
+000007a0: 2073 616d 706c 655f 7369 7a65 3a20 696e   sample_size: in
+000007b0: 742c 0a20 2020 2020 2020 2020 2020 2053  t,.            S
+000007c0: 697a 6520 6f66 2074 6865 2073 616d 706c  ize of the sampl
+000007d0: 650a 2020 2020 2020 2020 6765 6e65 7261  e.        genera
+000007e0: 746f 723a 206e 702e 7261 6e64 6f6d 2e47  tor: np.random.G
+000007f0: 656e 6572 6174 6f72 0a20 2020 2020 2020  enerator.       
+00000800: 2020 2020 2041 206e 756d 7079 2067 656e       A numpy gen
+00000810: 6572 6174 6f72 2069 6e69 7469 616c 697a  erator initializ
+00000820: 6564 206f 6e20 7468 6520 7365 7276 6572  ed on the server
+00000830: 2073 6964 652e 0a20 2020 200a 2020 2020   side..    .    
+00000840: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00000850: 2d2d 2d0a 2020 2020 2020 2020 6469 6374  ---.        dict
+00000860: 5b69 643a 2046 6564 6572 6174 6564 4e6f  [id: FederatedNo
+00000870: 6465 5d0a 2020 2020 2222 220a 2020 2020  de].    """.    
+00000880: 7361 6d70 6c65 203d 2067 656e 6572 6174  sample = generat
+00000890: 6f72 2e63 686f 6963 6528 6c69 7374 286e  or.choice(list(n
+000008a0: 6f64 6573 2e76 616c 7565 7328 2929 2c20  odes.values()), 
+000008b0: 7369 7a65 3d73 616d 706c 655f 7369 7a65  size=sample_size
+000008c0: 2c20 7265 706c 6163 653d 4661 6c73 6529  , replace=False)
+000008d0: 2023 2043 6f6e 7665 7273 696f 6e20 746f   # Conversion to
+000008e0: 2061 7272 6179 0a20 2020 2073 616d 706c   array.    sampl
+000008f0: 6520 3d20 7b6e 6f64 652e 6e6f 6465 5f69  e = {node.node_i
+00000900: 643a 206e 6f64 6520 666f 7220 6e6f 6465  d: node for node
+00000910: 2069 6e20 7361 6d70 6c65 7d20 2320 4261   in sample} # Ba
+00000920: 636b 2d63 6f6e 7665 7273 696f 6e20 746f  ck-conversion to
+00000930: 2064 6963 6974 6f6e 6172 790a 2020 2020   dicitonary.    
+00000940: 7265 7475 726e 2073 616d 706c 650a 0a0a  return sample...
+00000950: 6465 6620 7361 6d70 6c65 5f77 6569 6768  def sample_weigh
+00000960: 7465 645f 6e6f 6465 7328 6e6f 6465 733a  ted_nodes(nodes:
+00000970: 2064 6963 745b 696e 743a 2046 6564 6572   dict[int: Feder
+00000980: 6174 6564 4e6f 6465 5d2c 200a 2020 2020  atedNode], .    
+00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009a0: 2020 2020 2020 7361 6d70 6c65 5f73 697a        sample_siz
+000009b0: 653a 2069 6e74 2c0a 2020 2020 2020 2020  e: int,.        
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 2020 6765 6e65 7261 746f 723a 206e 702e    generator: np.
+000009e0: 7261 6e64 6f6d 2e47 656e 6572 6174 6f72  random.Generator
+000009f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000a00: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+00000a10: 6c69 6e67 5f61 7272 6179 3a20 6e70 2e61  ling_array: np.a
+00000a20: 7272 6179 2920 2d3e 2064 6963 745b 6964  rray) -> dict[id
+00000a30: 3a20 4665 6465 7261 7465 644e 6f64 655d  : FederatedNode]
+00000a40: 3a0a 2020 2020 2222 2253 616d 706c 6520  :.    """Sample 
+00000a50: 7468 6520 6e6f 6465 7320 6769 7665 6e20  the nodes given 
+00000a60: 7468 6520 7072 6f76 6964 6564 2073 616d  the provided sam
+00000a70: 706c 6520 7369 7a65 2e20 4974 2072 6571  ple size. It req
+00000a80: 7569 7265 7320 7061 7373 696e 6720 6120  uires passing a 
+00000a90: 7361 6d70 6c69 6e67 2061 7272 6179 0a20  sampling array. 
+00000aa0: 2020 2063 6f6e 7461 696e 696e 6720 6c69     containing li
+00000ab0: 7374 206f 6620 7765 6967 6874 7320 6173  st of weights as
+00000ac0: 736f 6369 6174 6564 2077 6974 6820 6561  sociated with ea
+00000ad0: 6368 206e 6f64 652e 0a20 2020 200a 2020  ch node..    .  
+00000ae0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00000af0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000b00: 2020 2020 6e6f 6465 733a 2064 6963 745b      nodes: dict[
+00000b10: 696e 743a 2046 6564 6572 6174 6564 4e6f  int: FederatedNo
+00000b20: 6465 5d29 200a 2020 2020 2020 2020 2020  de]) .          
+00000b30: 2020 4f72 6967 696e 616c 2064 6963 7469    Original dicti
+00000b40: 6f6e 6172 7920 6f66 206e 6f64 6573 2074  onary of nodes t
+00000b50: 6f20 6265 2073 616d 706c 6564 2066 726f  o be sampled fro
+00000b60: 6d2e 0a20 2020 2020 2020 2073 616d 706c  m..        sampl
+00000b70: 655f 7369 7a65 3a20 696e 742c 0a20 2020  e_size: int,.   
+00000b80: 2020 2020 2020 2020 2053 697a 6520 6f66           Size of
+00000b90: 2074 6865 2073 616d 706c 650a 2020 2020   the sample.    
+00000ba0: 2020 2020 6765 6e65 7261 746f 723a 206e      generator: n
+00000bb0: 702e 7261 6e64 6f6d 2e47 656e 6572 6174  p.random.Generat
+00000bc0: 6f72 0a20 2020 2020 2020 2020 2020 2041  or.            A
+00000bd0: 206e 756d 7079 2067 656e 6572 6174 6f72   numpy generator
+00000be0: 2069 6e69 7469 616c 697a 6564 206f 6e20   initialized on 
+00000bf0: 7468 6520 7365 7276 6572 2073 6964 652e  the server side.
+00000c00: 0a20 2020 2020 2020 2073 616d 706c 696e  .        samplin
+00000c10: 675f 6172 7261 793a 206e 702e 6172 7261  g_array: np.arra
+00000c20: 790a 2020 2020 2020 2020 2020 2020 5361  y.            Sa
+00000c30: 6d70 6c69 6e67 2061 7272 6179 2063 6f6e  mpling array con
+00000c40: 7461 696e 696e 6720 7765 6967 6874 7320  taining weights 
+00000c50: 666f 7220 7468 6520 7361 6d70 6c69 6e67  for the sampling
+00000c60: 0a20 2020 200a 2020 2020 5265 7475 726e  .    .    Return
+00000c70: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00000c80: 2020 2020 2020 6469 6374 5b69 643a 2046        dict[id: F
+00000c90: 6564 6572 6174 6564 4e6f 6465 5d0a 2020  ederatedNode].  
+00000ca0: 2020 2222 220a 2020 2020 7361 6d70 6c65    """.    sample
+00000cb0: 203d 2067 656e 6572 6174 6f72 2e63 686f   = generator.cho
+00000cc0: 6963 6528 6e6f 6465 732c 2073 697a 653d  ice(nodes, size=
+00000cd0: 7361 6d70 6c65 5f73 697a 652c 2070 203d  sample_size, p =
+00000ce0: 2073 616d 706c 696e 675f 6172 7261 792c   sampling_array,
+00000cf0: 2072 6570 6c61 6365 3d46 616c 7365 290a   replace=False).
+00000d00: 2020 2020 7361 6d70 6c65 203d 207b 6e6f      sample = {no
+00000d10: 6465 2e6e 6f64 655f 6964 3a20 6e6f 6465  de.node_id: node
+00000d20: 2066 6f72 206e 6f64 6520 696e 2073 616d   for node in sam
+00000d30: 706c 657d 2023 2042 6163 6b2d 636f 6e76  ple} # Back-conv
+00000d40: 6572 7369 6f6e 2074 6f20 6469 6369 746f  ersion to dicito
+00000d50: 6e61 7279 0a20 2020 2072 6574 7572 6e20  nary.    return 
+00000d60: 7361 6d70 6c65                           sample
```

### Comparing `fedjust-0.1.2/FedJust/operations/evaluations.py` & `fedjust-0.1.2.3/FedJust/operations/evaluations.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/FedJust/simulation/adaptive_optimizer_simulation.py` & `fedjust-0.1.2.3/FedJust/simulation/adaptive_optimizer_simulation.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/FedJust/simulation/simulation.py` & `fedjust-0.1.2.3/FedJust/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/FedJust/utils/computations.py` & `fedjust-0.1.2.3/FedJust/utils/computations.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/README.md` & `fedjust-0.1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2/PKG-INFO` & `fedjust-0.1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedJust
-Version: 0.1.2
+Version: 0.1.2.3
 Summary: 
 Author: Scolpe
 Author-email: 63779111+Scolpe@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

