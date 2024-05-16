# Comparing `tmp/mlscat-0.0.7.tar.gz` & `tmp/mlscat-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlscat-0.0.7.tar", last modified: Thu Apr 25 07:52:53 2024, max compression
+gzip compressed data, was "mlscat-0.0.8.tar", last modified: Wed May 15 13:37:44 2024, max compression
```

## Comparing `mlscat-0.0.7.tar` & `mlscat-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-25 07:52:53.235413 mlscat-0.0.7/
--rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-04-25 07:52:53.235413 mlscat-0.0.7/PKG-INFO
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      523 2024-04-17 06:13:37.000000 mlscat-0.0.7/README.md
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-25 07:52:53.235413 mlscat-0.0.7/mlscat/
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      131 2024-04-25 07:52:31.000000 mlscat-0.0.7/mlscat/__init__.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      172 2024-04-17 06:13:37.000000 mlscat-0.0.7/mlscat/api.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     2111 2024-04-17 06:24:18.000000 mlscat-0.0.7/mlscat/attacks.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1441 2024-04-19 02:06:03.000000 mlscat-0.0.7/mlscat/ranks.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1993 2024-04-25 07:24:37.000000 mlscat-0.0.7/mlscat/security.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)    25666 2024-04-19 02:11:10.000000 mlscat-0.0.7/mlscat/utils.py
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-25 07:52:53.235413 mlscat-0.0.7/mlscat.egg-info/
--rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/PKG-INFO
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      269 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/SOURCES.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        1 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/dependency_links.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        6 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/requires.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        7 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/top_level.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       38 2024-04-25 07:52:53.235413 mlscat-0.0.7/setup.cfg
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      590 2024-04-17 12:37:41.000000 mlscat-0.0.7/setup.py
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-15 13:37:44.280662 mlscat-0.0.8/
+-rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-05-15 13:37:44.280662 mlscat-0.0.8/PKG-INFO
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      523 2024-04-17 06:13:37.000000 mlscat-0.0.8/README.md
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-15 13:37:44.280662 mlscat-0.0.8/mlscat/
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       41 2024-05-15 13:35:57.000000 mlscat-0.0.8/mlscat/__init__.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     2972 2024-05-15 12:27:06.000000 mlscat-0.0.8/mlscat/attacks.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1573 2024-05-15 13:35:36.000000 mlscat-0.0.8/mlscat/data.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1024 2024-05-15 12:27:54.000000 mlscat-0.0.8/mlscat/leakage.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      986 2024-05-15 12:56:33.000000 mlscat-0.0.8/mlscat/preprocess.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1993 2024-05-15 12:07:34.000000 mlscat-0.0.8/mlscat/security.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)    25946 2024-05-15 12:35:40.000000 mlscat-0.0.8/mlscat/utils.py
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-15 13:37:44.280662 mlscat-0.0.8/mlscat.egg-info/
+-rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/PKG-INFO
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      293 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/SOURCES.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        1 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/dependency_links.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        6 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/requires.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        7 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/top_level.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       38 2024-05-15 13:37:44.280662 mlscat-0.0.8/setup.cfg
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      590 2024-04-17 12:37:41.000000 mlscat-0.0.8/setup.py
```

### Comparing `mlscat-0.0.7/PKG-INFO` & `mlscat-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

### Comparing `mlscat-0.0.7/README.md` & `mlscat-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.7/mlscat/attacks.py` & `mlscat-0.0.8/mlscat/attacks.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,7 +54,35 @@
 def pearson(x:np.array, y:np.array):
     x = (x-np.mean(x,axis=0))/np.std(x,axis=0)
     x = x/np.linalg.norm(x,axis=0)
     y = (y-np.mean(y,axis=0))/np.std(y,axis=0)
     y = y/np.linalg.norm(y,axis=0)
     m = np.dot(x.T,y)
     return abs(m)
+
+
+def rank(predictions, targets, key:int, num_trace:int, interval:int):
+    '''
+    ### key rank
+    `A function to calc right key rank`
+    
+    Args:
+    `predictions`: key prediction array.
+    `targets`    : range every keys prediction.
+    `key`        : key value(for byte).
+    `num_trace`  : traces number for prediction.
+    `interval`   : rank interval.
+    
+    Returns:
+        key rank ndarray.
+    '''
+    rank_time = np.zeros(int(num_trace/interval))
+    pred = np.zeros(256)
+    idx = np.random.randint(predictions.shape[0], size=num_trace)
+    for i, p in enumerate(idx):
+        for k in range(predictions.shape[1]): #256
+            pred[k] += predictions[p, targets[p, k]]
+        
+        if i % interval == 0:
+            ranked = np.argsort(pred)[::-1]
+            rank_time[int(i/interval)] = list(ranked).index(key)
+    return rank_time
```

### Comparing `mlscat-0.0.7/mlscat/security.py` & `mlscat-0.0.8/mlscat/security.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.7/mlscat/utils.py` & `mlscat-0.0.8/mlscat/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,30 +35,40 @@
     # TODO: Supporting custom mask scheme
     else:
         pass
 
 
 def fit_cnn(data):
     '''
-    `fit_cnn`
+    ### fit_cnn
 
-    ## Parameters
-    `data`: ndarray which saved the traces
+    Args:
+    `data`: ndarray which saved the traces.
 
-    ## return 
+    Returns:
     array which fit cnn inputs
     '''
     return np.expand_dims(data, data.ndim)
 
-def get_targets(plaintexts):
+def get_targets(plaintexts, mask=-1) -> np.ndarray:
+    '''
+    ### get targets
+    
+    Args:
+    `plaintexts`: plaintext array, shape = (n, 1).
+    `mask`: white box if mask != -1 (except there no mask measure).
+    
+    Returns:
+    targets array.
+    '''
     targets = np.zeros(shape=(plaintexts.shape[0], 256))
     for num, plaintext in enumerate(plaintexts):
         tmp_targets = np.zeros(shape=256)
         for key in range(256):
-            tmp_targets[key] = AES_Sbox[key ^ plaintext]
+            tmp_targets[key] = AES_Sbox[key ^ plaintext] if mask == -1 else AES_Sbox[key ^ plaintext] ^ mask[num]
         targets[num] = tmp_targets
     return targets.astype(np.int64)
 
 
 # Code is ported from https://github.com/fastai/fastai
 class OneCycleLR(Callback):
     def __init__(self,
```

### Comparing `mlscat-0.0.7/mlscat.egg-info/PKG-INFO` & `mlscat-0.0.8/mlscat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

### Comparing `mlscat-0.0.7/setup.py` & `mlscat-0.0.8/setup.py`

 * *Files identical despite different names*

