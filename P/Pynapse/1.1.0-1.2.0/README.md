# Comparing `tmp/pynapse-1.1.0.tar.gz` & `tmp/pynapse-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynapse-1.1.0.tar", last modified: Tue May 14 07:12:59 2024, max compression
+gzip compressed data, was "pynapse-1.2.0.tar", last modified: Thu May 16 06:34:11 2024, max compression
```

## Comparing `pynapse-1.1.0.tar` & `pynapse-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 07:12:59.856742 pynapse-1.1.0/
--rw-rw-rw-   0        0        0     2800 2024-05-14 07:12:59.841120 pynapse-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 07:12:59.825499 pynapse-1.1.0/Pynapse/
--rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-1.1.0/Pynapse/__init__.py
--rw-rw-rw-   0        0        0     3419 2024-05-14 07:06:57.000000 pynapse-1.1.0/Pynapse/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:12:59.841120 pynapse-1.1.0/Pynapse.egg-info/
--rw-rw-rw-   0        0        0     2800 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2679 2024-05-14 07:09:24.000000 pynapse-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 07:12:59.856742 pynapse-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      316 2024-05-14 07:12:22.000000 pynapse-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:34:11.343202 pynapse-1.2.0/
+-rw-rw-rw-   0        0        0     2850 2024-05-16 06:34:11.341205 pynapse-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 06:34:11.302931 pynapse-1.2.0/Pynapse/
+-rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-1.2.0/Pynapse/__init__.py
+-rw-rw-rw-   0        0        0     3811 2024-05-16 06:32:43.000000 pynapse-1.2.0/Pynapse/main.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:34:11.339208 pynapse-1.2.0/Pynapse.egg-info/
+-rw-rw-rw-   0        0        0     2850 2024-05-16 06:34:10.000000 pynapse-1.2.0/Pynapse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-16 06:34:10.000000 pynapse-1.2.0/Pynapse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 06:34:10.000000 pynapse-1.2.0/Pynapse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 06:34:10.000000 pynapse-1.2.0/Pynapse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 06:34:10.000000 pynapse-1.2.0/Pynapse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2729 2024-05-16 06:34:00.000000 pynapse-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 06:34:11.343202 pynapse-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      316 2024-05-16 06:33:23.000000 pynapse-1.2.0/setup.py
```

### Comparing `pynapse-1.1.0/PKG-INFO` & `pynapse-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pynapse
-Version: 1.1.0
+Version: 1.2.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
@@ -67,12 +67,12 @@
 Net_Save.load('model.json', layers)                 # Load the network from a json file
 
 prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
 print(prediction)                                   # Print the prediction
 ```
 
 # CHANGES
-- added verbose
+- changed printing output loss from (output - y) to cross entropy
 
 
 # WHY NAMED "Pynapse"
 #### This module has been named "Pynapse" meaning Python and Synapse
```

### Comparing `pynapse-1.1.0/Pynapse/main.py` & `pynapse-1.2.0/Pynapse/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,35 +43,42 @@
                 dvalues = layer.dinputs
 
 
     def train(self, X, y, epochs, lr=0.1, v=True):
         if v == True: # made like this so we are not checking if v = true to print many times (to hopefully be faster than constantly checking)
             for epoch in range(epochs):
                 output = self.forward(X)
-                loss = output - y
-                self.backward(loss)
+                loss = self.cross_entropy(y, output)
+                self.backward(output - y)
 
                 #update weights and biases
                 for layer in self.layers:
                     if hasattr(layer, 'weights'):
                         layer.weights -= lr * layer.dweights
                         layer.biases -= lr * layer.dbiases
                 print(f"Epoch: {epoch} Loss: {loss}")
         else:
             for epoch in range(epochs):
                 output = self.forward(X)
-                loss = output - y
-                self.backward(loss)
+                loss = self.cross_entropy(y, output)
+                self.backward(output - y)
 
                 #update weights and biases
                 for layer in self.layers:
                     if hasattr(layer, 'weights'):
                         layer.weights -= lr * layer.dweights
                         layer.biases -= lr * layer.dbiases
 
+    def cross_entropy(self, y_true, y_pred):
+        # Avoid numerical instability by adding a small epsilon
+        epsilon = 1e-15
+        y_pred_clipped = np.clip(y_pred, epsilon, 1 - epsilon)
+        # Compute cross-entropy loss
+        return -np.mean(y_true * np.log(y_pred_clipped) + (1 - y_true) * np.log(1 - y_pred_clipped))
+
 class Bin_Round:
     def Bin_Round(X):
         if X >= 0.5:
             return 1
         elif X < 0.5:
             return 0
         else:
```

### Comparing `pynapse-1.1.0/Pynapse.egg-info/PKG-INFO` & `pynapse-1.2.0/Pynapse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pynapse
-Version: 1.1.0
+Version: 1.2.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
@@ -67,12 +67,12 @@
 Net_Save.load('model.json', layers)                 # Load the network from a json file
 
 prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
 print(prediction)                                   # Print the prediction
 ```
 
 # CHANGES
-- added verbose
+- changed printing output loss from (output - y) to cross entropy
 
 
 # WHY NAMED "Pynapse"
 #### This module has been named "Pynapse" meaning Python and Synapse
```

### Comparing `pynapse-1.1.0/README.md` & `pynapse-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,12 +61,12 @@
 Net_Save.load('model.json', layers)                 # Load the network from a json file
 
 prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
 print(prediction)                                   # Print the prediction
 ```
 
 # CHANGES
-- added verbose
+- changed printing output loss from (output - y) to cross entropy
 
 
 # WHY NAMED "Pynapse"
 #### This module has been named "Pynapse" meaning Python and Synapse
```

