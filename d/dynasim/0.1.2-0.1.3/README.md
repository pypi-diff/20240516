# Comparing `tmp/dynasim-0.1.2.tar.gz` & `tmp/dynasim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynasim-0.1.2.tar", last modified: Thu Apr 11 08:33:48 2024, max compression
+gzip compressed data, was "dynasim-0.1.3.tar", last modified: Thu May 16 07:42:02 2024, max compression
```

## Comparing `dynasim-0.1.2.tar` & `dynasim-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-04-11 08:33:48.406197 dynasim-0.1.2/
--rw-------   0 marcus     (501) staff       (20)     1067 2024-02-14 13:34:54.000000 dynasim-0.1.2/LICENSE
--rw-r--r--   0 marcus     (501) staff       (20)     4475 2024-04-11 08:33:48.405913 dynasim-0.1.2/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)     3995 2024-04-11 07:57:51.000000 dynasim-0.1.2/README.md
--rw-------   0 marcus     (501) staff       (20)      553 2024-04-11 08:01:29.000000 dynasim-0.1.2/pyproject.toml
--rw-r--r--   0 marcus     (501) staff       (20)       38 2024-04-11 08:33:48.406251 dynasim-0.1.2/setup.cfg
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-04-11 08:33:48.401083 dynasim-0.1.2/src/
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-04-11 08:33:48.404512 dynasim-0.1.2/src/dynasim/
--rw-------   0 marcus     (501) staff       (20)      197 2024-02-12 08:50:38.000000 dynasim-0.1.2/src/dynasim/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     3462 2024-04-11 07:55:38.000000 dynasim-0.1.2/src/dynasim/actuators.py
--rw-r--r--   0 marcus     (501) staff       (20)     3831 2024-02-14 14:28:03.000000 dynasim-0.1.2/src/dynasim/base.py
--rw-------   0 marcus     (501) staff       (20)     2962 2024-02-14 15:09:07.000000 dynasim-0.1.2/src/dynasim/nonlinearities.py
--rw-r--r--   0 marcus     (501) staff       (20)     2456 2024-02-12 08:50:38.000000 dynasim-0.1.2/src/dynasim/simulators.py
--rw-------   0 marcus     (501) staff       (20)     8365 2024-02-14 14:48:48.000000 dynasim-0.1.2/src/dynasim/systems.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-04-11 08:33:48.405660 dynasim-0.1.2/src/dynasim.egg-info/
--rw-r--r--   0 marcus     (501) staff       (20)     4475 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)      354 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/SOURCES.txt
--rw-r--r--   0 marcus     (501) staff       (20)        1 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/dependency_links.txt
--rw-r--r--   0 marcus     (501) staff       (20)       12 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/requires.txt
--rw-r--r--   0 marcus     (501) staff       (20)        8 2024-04-11 08:33:48.000000 dynasim-0.1.2/src/dynasim.egg-info/top_level.txt
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-05-16 07:42:02.372285 dynasim-0.1.3/
+-rw-------   0 marcus     (501) staff       (20)     1067 2024-02-14 13:34:54.000000 dynasim-0.1.3/LICENSE
+-rw-r--r--   0 marcus     (501) staff       (20)     6211 2024-05-16 07:42:02.371839 dynasim-0.1.3/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)     5731 2024-05-15 16:28:54.000000 dynasim-0.1.3/README.md
+-rw-------   0 marcus     (501) staff       (20)      553 2024-05-15 16:09:32.000000 dynasim-0.1.3/pyproject.toml
+-rw-r--r--   0 marcus     (501) staff       (20)       38 2024-05-16 07:42:02.372346 dynasim-0.1.3/setup.cfg
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-05-16 07:41:54.280350 dynasim-0.1.3/src/
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-05-16 07:42:00.542966 dynasim-0.1.3/src/dynasim/
+-rw-r--r--   0 marcus     (501) staff       (20)      197 2024-05-15 16:31:01.000000 dynasim-0.1.3/src/dynasim/__init__.py
+-rw-r--r--   0 marcus     (501) staff       (20)     4364 2024-05-15 16:31:01.000000 dynasim-0.1.3/src/dynasim/actuators.py
+-rw-r--r--   0 marcus     (501) staff       (20)        0 2024-05-15 16:31:01.000000 dynasim-0.1.3/src/dynasim/base.py
+-rw-------   0 marcus     (501) staff       (20)     2962 2024-05-15 16:31:01.000000 dynasim-0.1.3/src/dynasim/nonlinearities.py
+-rw-r--r--   0 marcus     (501) staff       (20)     2456 2024-05-15 16:31:01.000000 dynasim-0.1.3/src/dynasim/simulators.py
+-rw-------   0 marcus     (501) staff       (20)    13871 2024-05-15 16:31:01.000000 dynasim-0.1.3/src/dynasim/systems.py
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2024-05-16 07:42:02.371198 dynasim-0.1.3/src/dynasim.egg-info/
+-rw-r--r--   0 marcus     (501) staff       (20)     6211 2024-05-16 07:41:54.000000 dynasim-0.1.3/src/dynasim.egg-info/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)      354 2024-05-16 07:41:54.000000 dynasim-0.1.3/src/dynasim.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus     (501) staff       (20)        1 2024-05-16 07:41:54.000000 dynasim-0.1.3/src/dynasim.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus     (501) staff       (20)       12 2024-05-16 07:41:54.000000 dynasim-0.1.3/src/dynasim.egg-info/requires.txt
+-rw-r--r--   0 marcus     (501) staff       (20)        8 2024-05-16 07:41:54.000000 dynasim-0.1.3/src/dynasim.egg-info/top_level.txt
```

### Comparing `dynasim-0.1.2/LICENSE` & `dynasim-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynasim-0.1.2/PKG-INFO` & `dynasim-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-Metadata-Version: 2.1
-Name: dynasim
-Version: 0.1.2
-Summary: Dynamic System Simulators
-Author-email: Marcus Haywood-Alexander <mhaywood@ethz.ch>
-Project-URL: Homepage, https://github.com/MarcusHA94/dynasim
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-
 # DynaSim
 
 <!--- These are examples. See https://shields.io for others or to customize this set of shields. You might want to include dependencies, project status and licence info here --->
 ![GitHub repo size](https://img.shields.io/github/repo-size/MarcusHA94/dynasim)
 ![GitHub contributors](https://img.shields.io/github/contributors/MarcusHA94/dynasim)
 
 <!-- Project name is a `<utility/tool/feature>` that allows `<insert_target_audience>` to do `<action/task_it_does>`. -->
 
 The dynasim package simulates dynamic systems in the form:
 ```math
 \mathbf{M}\ddot{\mathbf{x}} + \mathbf{C}\dot{\mathbf{x}} + \mathbf{K}\mathbf{x} + \mathbf{C}_n g_c(\mathbf{x}, \dot{\mathbf{x}}) + \mathbf{K}_n g_k(\mathbf{x}, \dot{\mathbf{x}}) = \mathbf{f}
 ```
-where $\mathbf{\Xi}_n g_{\bullet}(\mathbf{x},\dot{\mathbf{x}})$ represents the nonlinear system forces. For example, a 3DOF Duffing oscillator, connected at one end, would have representative nonlinear forces,
+where $\mathbf{\Xi}_n g_{\bullet}(\mathbf{x},\dot{\mathbf{x}}) = \mathbf{C}_n g_c(\mathbf{x}, \dot{\mathbf{x}}) + \mathbf{K}_n g_k(\mathbf{x}, \dot{\mathbf{x}})$ represents the nonlinear system forces. For example, a 3DOF Duffing oscillator, connected at one end, would have representative nonlinear forces,
 ```math
 \mathbf{K}_n g_n(\mathbf{x}) = \begin{bmatrix}
     k_{n,1} & - k_{n,2} & 0 \\
     0 & k_{n,2} & -k_{n,3} \\
     0 & 0 & k_{n,3}
 \end{bmatrix}
 \begin{bmatrix}
@@ -37,15 +22,15 @@
     (x_2-x_1)^3 \\
     (x_3 - x_2)^3
 \end{bmatrix}
 ```
 
 ## Installing DynaSim
 
-To install SynaSim, follow these steps:
+To install DynaSim, follow these steps:
 
 Linux and macOS:
 ```
 python3 -m pip install dynasim
 ```
 
 Windows:
@@ -60,29 +45,30 @@
 
 ```
 import numpy as np
 import dynasim
 
 # create required variables
 n_dof = 5
+
+# create a time vector of 2048 time points up to 120 seconds
 nt = 2048
 time_span = np.linspace(0, 120, nt)
-# time vector of 2048 time points up to 120 seconds
 
 # create vectors of system parameters for sequential MDOF
 m_vec = 10.0 * np.ones(n_dof)
 c_vec = 1.0 * np.ones(n_dof)
 k_vec = 15.0 * np.ones(n_dof)
 # imposes every other connection as having an additional cubic stiffness
 kn_vec = np.array([25.0 * (i%2) for i in range(n_dof)])
 
 # create nonlinearities
 system_nonlin = dynasim.nonlinearities.exponent_stiffness(kn_vec, exponent=3, dofs=n_dof)
 # instantiate system and embed nonlinearity
-system = dynasim.systems.cantilever(m_vec, c_vec, k_vec, dofs=n_dof, nonlinearity=system_nonlin)
+system = dynasim.systems.mdof_cantilever(m_vec, c_vec, k_vec, dofs=n_dof, nonlinearity=system_nonlin)
 
 # create excitations and embed to system
 system.excitations = [None] * n_dof
 system.excitations[-1] = dynasim.actuators.sine_sweep(w_l = 0.5, w_u = 2.0, F0 = 1.0)
 
 # simulate system
 data = system.simulate(time_span, z0=None)
@@ -122,14 +108,57 @@
 ### Totally custom system
 
 One can generate a custom system by instantiating an MDOF system with corresponding modal matrices, but the nonlinearity must also be instantiated and 
 ```
 dynasim.base.mdof_system(M, C, K, Cn, Kn)
 ```
 
+## Continuous Beams
+
+These work much like the MDOF systems but with a few tweaks. Where ```beam_kwargs_cmb``` is a dictionary of combined properties of the beam.
+```
+beam_kwargs_cmb = {
+    "EI" : EI,  # Young's Modulus multiplied by second moment of intertia
+    "pA" : pA,  # density multiplied by cross sectional area
+    "c" : c,  # damping
+    "l" : l  # length of beam
+}
+ss_beam = dynasim.systems.cont_beam("cmb_vars", **beam_kwargs_cmb)
+```
+
+One can then generate and retrieve the mode shapes of the beam via
+```
+xx, phis = ss_beam.gen_modes(support, n_modes, nx)
+```
+Where ```support``` is a string representing different support types for the beam, options available are:
+| Code | Description |
+|------|-------------|
+| `ss-ss` | Simply supported at both ends |
+| `fx-fx` | Fixed at both ends |
+| `fr-fr` | Free at both ends |
+| `fx-ss` | Fixed at one end and simply supported at the other |
+| `fx-fr` | Fixed at one end and free at the other |
+
+Then, excitations are added as a list of dictionaries containing the location (in m) and excitation (prescribed as with mdof systems)
+```
+ss_beam.excitations = [
+    {
+        "excitation" : dynasim.actuators.sinusoid(1.2, 1.0),
+        "loc" : 0.25
+    }
+]
+```
+Then simulate just as with the MDOF system, however, the returned data here is the modal coordinates, and so to retrieve displacement, simply multiply by, and sum through, the mode shapes.
+```
+data = ss_beam.simulate(tt, z0 = tau0)
+
+ww = np.sum(np.matmul(data['x'][:,:,np.newaxis], phis.T[:,np.newaxis,:]), axis=0)
+wwd = np.sum(np.matmul(data['xdot'][:,:,np.newaxis], phis.T[:,np.newaxis,:]), axis=0)
+```
+
 ## Contact
 
 If you want to contact me you can reach me at <mhaywood@ethz.ch>.
 
 ## License
 <!--- If you're not sure which open license to use see https://choosealicense.com/--->
```

### Comparing `dynasim-0.1.2/pyproject.toml` & `dynasim-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynasim"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Marcus Haywood-Alexander", email="mhaywood@ethz.ch" },
 ]
 description = "Dynamic System Simulators"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dynasim-0.1.2/src/dynasim/actuators.py` & `dynasim-0.1.3/src/dynasim/actuators.py`

 * *Files 26% similar despite different names*

```diff
@@ -93,34 +93,59 @@
 
         np.random.seed(seed)
         phases = np.random.randn(self.freqs.shape[0]) * pi/2
         F_mat = np.sin(time.reshape(-1,1) @ self.freqs.reshape(1,-1) + phases.T)
 
         return (F_mat @ self.Sx).reshape(-1)
 
-class shaker():
+class mdof_shaker():
     '''
-    Shaker class generates force signals at each DOF using excitation class
+    MDOF shaker class generates force signals at each DOF using excitation class
     '''
 
     def __init__(self, excitations=None, seed=43810):
 
         self.excitations = excitations
         self.dofs = len(excitations)
         self.seed = seed
 
     def generate(self, time):
         nt = time.shape[0]
         self.f = np.zeros((self.dofs,nt))
         for n, excite in enumerate(self.excitations):
             match excite:
                 case excitation():
-                    self.f[n,:] = self.excitations[n]._generate(time, self.seed+n)
+                    self.f[n, :] = self.excitations[n]._generate(time, self.seed+n)
                 case np.ndarray():
-                    self.f[n,:] = self.excitations[n]
+                    self.f[n, :] = self.excitations[n]
                 case None:
-                    self.f[n,:] = np.zeros(nt)
+                    self.f[n, :] = np.zeros(nt)
 
         return self.f
+    
+class point_shakers():
+    '''
+    Point shakers class generates force signals at a specific locations using excitation class
+    '''
+
+    def __init__(self, excitations=None, xx=None, seed=43810):
+
+        self.excitations = excitations
+        "excitations is a list of dictionaries containing location and excitation"
+        self.xx = xx
+        self.seed = seed
+
+    def generate(self, time):
+        nt = time.shape[0]
+        nx = self.xx.shape[0]
+        self.f = np.zeros((nx, nt))
+        for excite in self.excitations:
+            self.loc_id = np.argmin(np.abs(self.xx-excite['loc']))
+            match excite['excitation']:
+                case excitation():
+                    self.f[self.loc_id, :] = excite['excitation']._generate(time, self.seed)
+                case np.ndarray():
+                    self.f[self.loc_id, :] = self.excitation
+        return self.f
```

### Comparing `dynasim-0.1.2/src/dynasim/nonlinearities.py` & `dynasim-0.1.3/src/dynasim/nonlinearities.py`

 * *Files identical despite different names*

### Comparing `dynasim-0.1.2/src/dynasim/simulators.py` & `dynasim-0.1.3/src/dynasim/simulators.py`

 * *Files identical despite different names*

