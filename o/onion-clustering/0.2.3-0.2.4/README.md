# Comparing `tmp/onion_clustering-0.2.3.tar.gz` & `tmp/onion_clustering-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_clustering-0.2.3.tar", last modified: Wed May 15 12:23:42 2024, max compression
+gzip compressed data, was "onion_clustering-0.2.4.tar", last modified: Thu May 16 12:45:20 2024, max compression
```

## Comparing `onion_clustering-0.2.3.tar` & `onion_clustering-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-15 12:23:42.048009 onion_clustering-0.2.3/
--rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-15 12:22:55.000000 onion_clustering-0.2.3/.coverage
--rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-08 09:25:50.000000 onion_clustering-0.2.3/.gitignore
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.3/LICENSE
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-15 12:23:42.047214 onion_clustering-0.2.3/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-05-08 09:25:50.000000 onion_clustering-0.2.3/README.md
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-15 12:23:42.032962 onion_clustering-0.2.3/examples/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3663 2024-05-08 09:25:50.000000 onion_clustering-0.2.3/examples/example_script.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-05-08 09:25:50.000000 onion_clustering-0.2.3/examples/example_script_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-08 09:25:50.000000 onion_clustering-0.2.3/justfile
--rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-15 12:22:01.000000 onion_clustering-0.2.3/pyproject.toml
--rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.3/pytest.ini
--rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-15 12:23:42.048175 onion_clustering-0.2.3/setup.cfg
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-15 12:23:42.027348 onion_clustering-0.2.3/src/
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-15 12:23:42.037327 onion_clustering-0.2.3/src/onion_clustering/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-08 09:25:50.000000 onion_clustering-0.2.3/src/onion_clustering/__init__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-10 14:39:49.000000 onion_clustering-0.2.3/src/onion_clustering/classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    20386 2024-05-15 12:08:37.000000 onion_clustering-0.2.3/src/onion_clustering/first_classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    30063 2024-05-15 12:08:37.000000 onion_clustering-0.2.3/src/onion_clustering/functions.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    26215 2024-05-15 12:08:37.000000 onion_clustering-0.2.3/src/onion_clustering/main.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    20729 2024-05-15 12:08:37.000000 onion_clustering-0.2.3/src/onion_clustering/main_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-08 09:25:50.000000 onion_clustering-0.2.3/src/onion_clustering/utilities.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-15 12:23:42.046294 onion_clustering-0.2.3/src/onion_clustering.egg-info/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-15 12:23:41.000000 onion_clustering-0.2.3/src/onion_clustering.egg-info/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-15 12:23:42.000000 onion_clustering-0.2.3/src/onion_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-15 12:23:41.000000 onion_clustering-0.2.3/src/onion_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-15 12:23:41.000000 onion_clustering-0.2.3/src/onion_clustering.egg-info/requires.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-15 12:23:41.000000 onion_clustering-0.2.3/src/onion_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-15 12:23:42.041924 onion_clustering-0.2.3/test/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.3/test/__init__.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-15 12:23:42.044136 onion_clustering-0.2.3/test/output_multi/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      412 2024-05-15 12:16:50.000000 onion_clustering-0.2.3/test/output_multi/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-15 12:16:38.000000 onion_clustering-0.2.3/test/output_multi/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-15 12:16:38.000000 onion_clustering-0.2.3/test/output_multi/number_of_states.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-15 12:23:42.045690 onion_clustering-0.2.3/test/output_uni/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1662 2024-05-14 13:55:06.000000 onion_clustering-0.2.3/test/output_uni/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-14 13:55:01.000000 onion_clustering-0.2.3/test/output_uni/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-14 13:55:01.000000 onion_clustering-0.2.3/test/output_uni/number_of_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3112 2024-05-15 12:18:40.000000 onion_clustering-0.2.3/test/test_multi.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     2941 2024-05-14 13:56:18.000000 onion_clustering-0.2.3/test/test_uni.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.403943 onion_clustering-0.2.4/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-16 12:44:30.000000 onion_clustering-0.2.4/.coverage
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-08 09:25:50.000000 onion_clustering-0.2.4/.gitignore
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.4/LICENSE
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-16 12:45:20.403065 onion_clustering-0.2.4/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5465 2024-05-15 12:29:23.000000 onion_clustering-0.2.4/README.md
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.390815 onion_clustering-0.2.4/examples/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3647 2024-05-16 08:42:26.000000 onion_clustering-0.2.4/examples/example_script.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3637 2024-05-16 08:15:24.000000 onion_clustering-0.2.4/examples/example_script_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-08 09:25:50.000000 onion_clustering-0.2.4/justfile
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-16 12:44:50.000000 onion_clustering-0.2.4/pyproject.toml
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.4/pytest.ini
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-16 12:45:20.404119 onion_clustering-0.2.4/setup.cfg
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.385793 onion_clustering-0.2.4/src/
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.393908 onion_clustering-0.2.4/src/onion_clustering/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-08 09:25:50.000000 onion_clustering-0.2.4/src/onion_clustering/__init__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-10 14:39:49.000000 onion_clustering-0.2.4/src/onion_clustering/classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    20386 2024-05-15 12:08:37.000000 onion_clustering-0.2.4/src/onion_clustering/first_classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    30001 2024-05-16 12:40:18.000000 onion_clustering-0.2.4/src/onion_clustering/functions.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    26441 2024-05-16 09:15:31.000000 onion_clustering-0.2.4/src/onion_clustering/main.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    20729 2024-05-15 12:08:37.000000 onion_clustering-0.2.4/src/onion_clustering/main_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-08 09:25:50.000000 onion_clustering-0.2.4/src/onion_clustering/utilities.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.402034 onion_clustering-0.2.4/src/onion_clustering.egg-info/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/requires.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.397534 onion_clustering-0.2.4/test/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.4/test/__init__.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.399721 onion_clustering-0.2.4/test/output_multi/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      412 2024-05-15 12:16:50.000000 onion_clustering-0.2.4/test/output_multi/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-15 12:16:38.000000 onion_clustering-0.2.4/test/output_multi/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-15 12:16:38.000000 onion_clustering-0.2.4/test/output_multi/number_of_states.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.401384 onion_clustering-0.2.4/test/output_uni/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1662 2024-05-14 13:55:06.000000 onion_clustering-0.2.4/test/output_uni/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-14 13:55:01.000000 onion_clustering-0.2.4/test/output_uni/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-14 13:55:01.000000 onion_clustering-0.2.4/test/output_uni/number_of_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3112 2024-05-15 12:18:40.000000 onion_clustering-0.2.4/test/test_multi.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     2941 2024-05-14 13:56:18.000000 onion_clustering-0.2.4/test/test_uni.py
```

### Comparing `onion_clustering-0.2.3/.coverage` & `onion_clustering-0.2.4/.coverage`

 * *Files 2% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -48,16 +48,16 @@
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
 INSERT INTO line_bits VALUES(2,1,X'c27b0790e0e60750fe010000008edec94b7e07f91d2c37843fbfaffffdde000000000000000000000000f90300d27df3c97b1cf201c8f9fc85b53d7d7e000000762b789a0700a09180edf97fbfcf7900ef12');
 INSERT INTO line_bits VALUES(3,1,X'627f819075ff4564c9f37bbb029de2342ac68fdfe493593e052c220000000000840b00000090bbe7e7dd2768db75af3b56fc3e3ff271cb0479bf7f92f7f9317e5efee7e779f7fbfdf8962625db3f6e5680db5d7f7efcfffdfd3100008005b020efdfffc45f00000000000000000000000080f9bd7ffff3efbf7ffff1972db3fcec3f6e');
 INSERT INTO line_bits VALUES(4,1,X'625f0200c0f85dc08c5f40c66308c00b0858000080c0b74040003bc636f3fd1e3ffff7e79f2fe36100c66701020bfc9e00404084c7d866dee3e77fff7c190ffcbfefefbb11c02bfeff0b');
-INSERT INTO line_bits VALUES(5,1,X'a25f0230280f008003780000b4af96070080070080f6ad1c0000f01800e8f6db776500c0aed75bf90700000000cfddbf1c00200f0000481e8b250000007fc37940010000ee5e5f1e0000766ffe7ff2010000bcbf179e87ff00c7fbe6e7930f000000fff907000000fcbddddbc9010088470eff93ff008be79fdff838df2d');
-INSERT INTO line_bits VALUES(6,1,X'c2f70ec00400c019f203281f00000000f6ffcbff13e00f00fe000000603e1fe6e7fc3cfedbf6bd0200901f000000e4eee693f778e41f000000e4f261fdf2f879dcc1f4375ff21e87e003000080b3cfef8cffdc77cf0f0000c06e05cf9fa7790000349e3f3900d89effedf7390f000000e05d02');
+INSERT INTO line_bits VALUES(5,1,X'a25f0230280f008003780000b4af96070080070080f6ad1c0000f01800e8f6db776500c0aed75bf90700000000cfddbf1c00200f0000481e8b250000007fc37940010000ee5e9b5b1e0000766ffe7ff2010000bcbf179e87ff00c7fbe6e7930f000000fff907000000fcbddddbc9010088470eff93ff16cf3fbff171be5b');
+INSERT INTO line_bits VALUES(6,1,X'c2f70ec00400c019f203281f00000000e0edff97ff8dfc010000c07c3ecccfe3e7f1ff6efbfd0a00407e00000090bb9b4fdee3917f00000090cb87f5cbe3e77107d3df7cc97b1c820f000000ce3ebf33fe73df3d3f000000bb153c7f9ee60100d078fee400607bfeb7dfe73c000000807709');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `onion_clustering-0.2.3/LICENSE` & `onion_clustering-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/PKG-INFO` & `onion_clustering-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.3
+Version: 0.2.4
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
@@ -19,15 +19,15 @@
 A one-dimensional time-series, computed on *N* particles for *T* frames. The input files must contain an array with shape *(N, T)* Supported formats: .npy, .npz, .txt. Also .xyz trajectories are supported, with the fifth column containing the data values. 
 
 ## Usage
 Install the package using `pip install onion_clustering`. 
 
 The `examples/` folder contains an example of usage. Run `python3 example_script.py`, this will create the following files:
 * A text file called `input_parameters.txt` , whose format is explained below;
-* A text file called `data_directory.txt` containing one line with the path to the input data file (including the input data file name). 
+* A text file called `data_directory.txt` containing one line with the path to the input data file (including the input data file name); 
 and run the code. 
 
 ## input_parameters.txt 
 * `tau_window` (int): the length of the time window (in number of frames). 
 * `t_smooth` (int, optional): the length of the smoothing window (in number of frames) for the moving average. A value of `t_smooth = 1` correspond to no smoothing. Default is 1. 
 * `t_delay` (int, optional): is for ignoring the first tau_delay frames of the trajectory. Default is 0. 
 * `t_conv` (int, optional): converts number of frames in time units. Default is 1. 
@@ -61,21 +61,17 @@
 The `main_2d.py` algorithm works in a similar fashion, taking as input 2D or 3D data. The input file contained in `data_directory.txt` must contain an array of shape `(D, N, T)` where _D_ is the number of components. Only `.npy, .npz` are supported. You can find an example of usage in `examples/example_script_2d.py`
 
 ## Required Python 3 packages
 `matplotlib`, `numpy`, `plotly`, `scipy`. 
 
 ## Gaussian fitting procedure
 1. The histogram of the time-series is computed, using the `bins='auto'` numpy option (unless a different `bins` is passed as imput parameter). 
-2. The histogram is smoothed with moving average with `window_size=3` (unless there are less that 50 bins, in wich case no smoothing occurs). 
+2. The histogram is smoothed with moving average with a window proportional to the number of bins (unless there are less that 50 bins, in wich case no smoothing occurs). 
 3. The absolute maximum of the histogram is found. 
 4. Two Gaussian fits are performed:
  * The first one inside the interval between the two minima surrounding the maximum. 
  * The second one inside the interval where the peak around the maxima has its half height. 
-5. Both fits, if converged, are evaluated according to the following points:
- * `mu` is contained inside the fit interval;
- * `sigma` is smaller than the fit interval;
- * the height of the peak is at least half the value of the maximum;
- * the relative uncertanty over the fit parameters is smaller than 0.5.
+5. Both fits, if converged, are evaluated according to the coefficinet of determination r^2. 
 6. Finally, the fit with the best score is chosen. If only one of the two converged, that one is chosen. If none of the fits converges, the iterative procedure stops, returning a warning message. 
 
 ## Aknowledgements
 Thanks to Andrew Tarzia for all the help with the code formatting and documentation, and to Domiziano Doria, Chiara Lionello and Simone Martino for the beta-testing. Writing all this code wouldn't have been possible without the help of ChatGPT.
```

### Comparing `onion_clustering-0.2.3/README.md` & `onion_clustering-0.2.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A one-dimensional time-series, computed on *N* particles for *T* frames. The input files must contain an array with shape *(N, T)* Supported formats: .npy, .npz, .txt. Also .xyz trajectories are supported, with the fifth column containing the data values. 
 
 ## Usage
 Install the package using `pip install onion_clustering`. 
 
 The `examples/` folder contains an example of usage. Run `python3 example_script.py`, this will create the following files:
 * A text file called `input_parameters.txt` , whose format is explained below;
-* A text file called `data_directory.txt` containing one line with the path to the input data file (including the input data file name). 
+* A text file called `data_directory.txt` containing one line with the path to the input data file (including the input data file name); 
 and run the code. 
 
 ## input_parameters.txt 
 * `tau_window` (int): the length of the time window (in number of frames). 
 * `t_smooth` (int, optional): the length of the smoothing window (in number of frames) for the moving average. A value of `t_smooth = 1` correspond to no smoothing. Default is 1. 
 * `t_delay` (int, optional): is for ignoring the first tau_delay frames of the trajectory. Default is 0. 
 * `t_conv` (int, optional): converts number of frames in time units. Default is 1. 
@@ -47,21 +47,17 @@
 The `main_2d.py` algorithm works in a similar fashion, taking as input 2D or 3D data. The input file contained in `data_directory.txt` must contain an array of shape `(D, N, T)` where _D_ is the number of components. Only `.npy, .npz` are supported. You can find an example of usage in `examples/example_script_2d.py`
 
 ## Required Python 3 packages
 `matplotlib`, `numpy`, `plotly`, `scipy`. 
 
 ## Gaussian fitting procedure
 1. The histogram of the time-series is computed, using the `bins='auto'` numpy option (unless a different `bins` is passed as imput parameter). 
-2. The histogram is smoothed with moving average with `window_size=3` (unless there are less that 50 bins, in wich case no smoothing occurs). 
+2. The histogram is smoothed with moving average with a window proportional to the number of bins (unless there are less that 50 bins, in wich case no smoothing occurs). 
 3. The absolute maximum of the histogram is found. 
 4. Two Gaussian fits are performed:
  * The first one inside the interval between the two minima surrounding the maximum. 
  * The second one inside the interval where the peak around the maxima has its half height. 
-5. Both fits, if converged, are evaluated according to the following points:
- * `mu` is contained inside the fit interval;
- * `sigma` is smaller than the fit interval;
- * the height of the peak is at least half the value of the maximum;
- * the relative uncertanty over the fit parameters is smaller than 0.5.
+5. Both fits, if converged, are evaluated according to the coefficinet of determination r^2. 
 6. Finally, the fit with the best score is chosen. If only one of the two converged, that one is chosen. If none of the fits converges, the iterative procedure stops, returning a warning message. 
 
 ## Aknowledgements
 Thanks to Andrew Tarzia for all the help with the code formatting and documentation, and to Domiziano Doria, Chiara Lionello and Simone Martino for the beta-testing. Writing all this code wouldn't have been possible without the help of ChatGPT.
```

### Comparing `onion_clustering-0.2.3/examples/example_script.py` & `onion_clustering-0.2.4/examples/example_script.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ### Set all the analysis parameters ###
 # Use git clone git@github.com:matteobecchi/onion_example_files.git
 # to download example datasets
 PATH_TO_INPUT_DATA = "../onion_example_files/data/univariate_time-series.npy"
 TAU_WINDOW = 4  # time resolution of the analysis
 
 ### Optional parametrers ###
-T_SMOOTH = 1  # window for moving average (default 1)
+T_SMOOTH = 1  # window for moving average (default 1 - no average)
 T_DELAY = 1  # remove the first t_delay frames (default 0)
 T_CONV = 1.0  # convert frames in time units (default 1)
 TIME_UNITS = "frames"  # the time units (default 'frames')
 EXAMPLE_ID = 0  # particle plotted as example (default 0)
 NUM_TAU_W = 20  # number of values of tau_window tested (default 20)
 MIN_TAU_W = 2  # min number of tau_window tested (default 2)
 MIN_T_SMOOTH = 1  # min value of t_smooth tested (default 1)
@@ -41,37 +41,38 @@
 try:
     ### Create the 'data_directory.txt' file ###
     with open("data_directory.txt", "w+", encoding="utf-8") as file:
         print(PATH_TO_INPUT_DATA, file=file)
 
     ### Create the 'input_parameter.txt' file ###
     with open("input_parameters.txt", "w+", encoding="utf-8") as file:
-        print("tau_window\t" + str(TAU_WINDOW), file=file)
-        print("t_smooth\t" + str(T_SMOOTH), file=file)
-        print("t_delay\t" + str(T_DELAY), file=file)
-        print("t_conv\t" + str(T_CONV), file=file)
-        print("t_units\t" + TIME_UNITS, file=file)
-        print("example_ID\t" + str(EXAMPLE_ID), file=file)
-        print("num_tau_w\t" + str(NUM_TAU_W), file=file)
-        print("min_tau_w\t" + str(MIN_TAU_W), file=file)
-        print("min_t_smooth\t" + str(MIN_T_SMOOTH), file=file)
-        print("max_t_smooth\t" + str(MAX_T_SMOOTH), file=file)
-        print("step_t_smooth\t" + str(STEP_T_SMOOTH), file=file)
+        print(f"tau_window\t{TAU_WINDOW}", file=file)
+        print(f"t_smooth\t{T_SMOOTH}", file=file)
+        print(f"t_delay\t{T_DELAY}", file=file)
+        print(f"t_conv\t{T_CONV}", file=file)
+        print(f"t_units\t{TIME_UNITS}", file=file)
+        print(f"example_ID\t{EXAMPLE_ID}", file=file)
+        print(f"num_tau_w\t{NUM_TAU_W}", file=file)
+        print(f"min_tau_w\t{MIN_TAU_W}", file=file)
+        print(f"min_t_smooth\t{MIN_T_SMOOTH}", file=file)
+        print(f"max_t_smooth\t{MAX_T_SMOOTH}", file=file)
+        print(f"step_t_smooth\t{STEP_T_SMOOTH}", file=file)
         if MAX_TAU_W != "auto":
-            print("max_tau_w\t" + str(MAX_TAU_W), file=file)
+            print(f"max_tau_w\t{MAX_TAU_W}", file=file)
         if BINS != "auto":
-            print("bins\t" + str(BINS), file=file)
+            print(f"bins\t{BINS}", file=file)
 
     ### Perform the clustering analysis ###
     cl_ob = main.main()
 
     ### Plot the output figures in output_figures/ ###
 
     # Plots number of states and fraction_0 as a function of tau_window
     cl_ob.plot_tra_figure()
+    cl_ob.plot_pop_fractions()
 
     # Plots the raw data
     cl_ob.plot_input_data("Fig0")
 
     # Plots the data with the clustering thresholds and Gaussians
     cl_ob.plot_cumulative_figure()
```

### Comparing `onion_clustering-0.2.3/examples/example_script_2d.py` & `onion_clustering-0.2.4/examples/example_script_2d.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,36 +41,37 @@
 try:
     ### Create the 'data_directory.txt' file ###
     with open("data_directory.txt", "w+", encoding="utf-8") as file:
         print(PATH_TO_INPUT_DATA, file=file)
 
     ### Create the 'input_parameter.txt' file ###
     with open("input_parameters.txt", "w+", encoding="utf-8") as file:
-        print("tau_window\t" + str(TAU_WINDOW), file=file)
-        print("t_smooth\t" + str(T_SMOOTH), file=file)
-        print("t_delay\t" + str(T_DELAY), file=file)
-        print("t_conv\t" + str(T_CONV), file=file)
-        print("time_units\t" + TIME_UNITS, file=file)
-        print("example_ID\t" + str(EXAMPLE_ID), file=file)
-        print("num_tau_w\t" + str(NUM_TAU_W), file=file)
-        print("min_tau_w\t" + str(MIN_TAU_W), file=file)
-        print("min_t_smooth\t" + str(MIN_T_SMOOTH), file=file)
-        print("max_t_smooth\t" + str(MAX_T_SMOOTH), file=file)
-        print("step_t_smooth\t" + str(STEP_T_SMOOTH), file=file)
+        print(f"tau_window\t{TAU_WINDOW}", file=file)
+        print(f"t_smooth\t{T_SMOOTH}", file=file)
+        print(f"t_delay\t{T_DELAY}", file=file)
+        print(f"t_conv\t{T_CONV}", file=file)
+        print(f"t_units\t{TIME_UNITS}", file=file)
+        print(f"example_ID\t{EXAMPLE_ID}", file=file)
+        print(f"num_tau_w\t{NUM_TAU_W}", file=file)
+        print(f"min_tau_w\t{MIN_TAU_W}", file=file)
+        print(f"min_t_smooth\t{MIN_T_SMOOTH}", file=file)
+        print(f"max_t_smooth\t{MAX_T_SMOOTH}", file=file)
+        print(f"step_t_smooth\t{STEP_T_SMOOTH}", file=file)
         if MAX_TAU_W != "auto":
-            print("max_tau_w\t" + str(MAX_TAU_W), file=file)
+            print(f"max_tau_w\t{MAX_TAU_W}", file=file)
         if BINS != "auto":
-            print("bins\t" + str(BINS), file=file)
+            print(f"bins\t{BINS}", file=file)
 
     ### Run the code ###
     cl_ob = main_2d.main()
 
     ### Plot the output figures in output_figures/ ###
     # Plots number of states and fraction_0 as a function of tau_window
     cl_ob.plot_tra_figure()
+    cl_ob.plot_pop_fractions()
 
     # Plots the raw data
     cl_ob.plot_input_data("Fig0")
 
     # Plots the data with the clustering thresholds and Gaussians
     cl_ob.plot_cumulative_figure()
```

### Comparing `onion_clustering-0.2.3/justfile` & `onion_clustering-0.2.4/justfile`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/pyproject.toml` & `onion_clustering-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onion_clustering"
-version = "0.2.3"
+version = "0.2.4"
 description = "Code for unsupervised clustering of time-correlated data."
 # license = "MIT"
 maintainers = [
   { name = "Matteo Becchi", email = "bechmath@gmail.com" },
 ]
 dependencies = [
   "matplotlib",
```

### Comparing `onion_clustering-0.2.3/src/onion_clustering/classes.py` & `onion_clustering-0.2.4/src/onion_clustering/classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/src/onion_clustering/first_classes.py` & `onion_clustering-0.2.4/src/onion_clustering/first_classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/src/onion_clustering/functions.py` & `onion_clustering-0.2.4/src/onion_clustering/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,17 +553,25 @@
     def min_of_gaussians(x):
         min_values = np.minimum(
             gaussian(x, mean1, sigma1, area1),
             gaussian(x, mean2, sigma2, area2),
         )
         return min_values
 
-    area_gaussian_1, _ = quad(gauss_1, -np.inf, np.inf)
-    area_gaussian_2, _ = quad(gauss_2, -np.inf, np.inf)
-    shared_area, _ = quad(min_of_gaussians, -np.inf, np.inf)
+    area_gaussian_1, _ = quad(
+        gauss_1, int(mean1 - 3 * sigma1) - 1, int(mean1 + 3 * sigma1) + 1
+    )
+    area_gaussian_2, _ = quad(
+        gauss_2, int(mean2 - 3 * sigma2) - 1, int(mean2 + 3 * sigma2) + 1
+    )
+
+    x_min = int(np.min([mean1 - 3 * sigma1, mean2 - 3 * sigma2])) - 1
+    x_max = int(np.max([mean1 + 3 * sigma1, mean2 + 3 * sigma2])) + 1
+    shared_area, _ = quad(min_of_gaussians, x_min, x_max)
+
     shared_fraction_1 = shared_area / area_gaussian_1
     shared_fraction_2 = shared_area / area_gaussian_2
 
     return shared_fraction_1, shared_fraction_2
 
 
 def final_state_settings(
@@ -930,21 +938,14 @@
         candidate_merge = []
         for pair in proposed_merge:
             if pair[0] == j:
                 candidate_merge.append(pair)
         if len(candidate_merge) == 1:
             best_merge.append(candidate_merge[0])
         else:
-            # list_of_distances = [
-            #     np.linalg.norm(
-            #         sorted_states[pair[1]].mean - sorted_states[pair[0]].mean
-            #     )
-            #     for pair in candidate_merge
-            # ]
-            # best_merge.append(candidate_merge[np.argmin(list_of_distances)])
             importance = [
                 sorted_states[pair[1]].perc for pair in candidate_merge
             ]
             best_merge.append(candidate_merge[np.argmax(importance)])
 
     # Settle merging chains
     # if [i, j], all the [k, i] become [k, j]
```

### Comparing `onion_clustering-0.2.3/src/onion_clustering/main.py` & `onion_clustering-0.2.4/src/onion_clustering/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     return clustering_object
 
 
 def perform_gauss_fit(
     param: List[int],
     data: List[np.ndarray],
     int_type: str,
-) -> Tuple[bool, float, np.ndarray]:
+) -> Tuple[bool, float, np.ndarray, np.ndarray]:
     """
     Perform Gaussian fit on given data.
 
     Parameters
     ----------
 
     id0 : int
@@ -119,79 +119,64 @@
 
     bool
         True if the fit is successful, False otherwise.
 
     coeff_det_r2 : float
         Coefficient of determination of the fit. Zero if the fit fails.
 
-    popt : np.ndarray or None
-        Parameters of the Gaussian fit if successful, None otherwise.
+    popt : np.ndarray of shape (3,)
+        Parameters of the Gaussian fit if successful, zeros otherwise.
+
+    perr : np.ndarray of shape (3,)
+        Uncertanties on the Gaussian fit if successful, zeros otherwise.
     """
+    ### Initialize return values ###
+    flag = False
+    coeff_det_r2 = 0
+    popt = np.empty(3)
+    perr = np.empty(3)
+
     id0, id1, max_ind, n_data = param
     bins, counts = data
 
     selected_bins = bins[id0:id1]
     selected_counts = counts[id0:id1]
     mu0 = bins[max_ind]
     sigma0 = (bins[id1] - bins[id0]) / 6
     area0 = counts[max_ind] * np.sqrt(np.pi) * sigma0
     try:
         with warnings.catch_warnings():
             warnings.filterwarnings("error")
-            popt, _, infodict, _, _ = scipy.optimize.curve_fit(
+            popt, pcov, infodict, _, _ = scipy.optimize.curve_fit(
                 gaussian,
                 selected_bins,
                 selected_counts,
                 p0=[mu0, sigma0, area0],
                 full_output=True,
             )
             if popt[1] < 0:
                 popt[1] *= -1
                 popt[2] *= -1
             popt[2] *= n_data
+            perr = np.array([np.sqrt(pcov[i][i]) for i in range(popt.size)])
+            perr[2] *= n_data
             ss_res = np.sum(infodict["fvec"] ** 2)
             ss_tot = np.sum((selected_counts - np.mean(selected_counts)) ** 2)
             coeff_det_r2 = 1 - ss_res / ss_tot
-            return True, coeff_det_r2, popt
+            flag = True
     except OptimizeWarning:
         print(f"\t{int_type} fit: Optimize warning. ")
-        return (
-            False,
-            0,
-            np.empty(
-                3,
-            ),
-        )
     except RuntimeError:
         print(f"\t{int_type} fit: Runtime error. ")
-        return (
-            False,
-            0,
-            np.empty(
-                3,
-            ),
-        )
     except TypeError:
         print(f"\t{int_type} fit: TypeError.")
-        return (
-            False,
-            0,
-            np.empty(
-                3,
-            ),
-        )
     except ValueError:
         print(f"\t{int_type} fit: ValueError.")
-        return (
-            False,
-            0,
-            np.empty(
-                3,
-            ),
-        )
+
+    return flag, coeff_det_r2, popt, perr
 
 
 def gauss_fit_max(
     m_clean: np.ndarray,
     par: Parameters,
     number_of_sigmas: float,
     filename: str,
@@ -256,60 +241,69 @@
         min_id0 -= 1
     while min_id1 < counts.size - 1 and counts[min_id1] > counts[min_id1 + 1]:
         min_id1 += 1
 
     ### 5. Try the fit between the minima and check its goodness ###
     fit_param = [min_id0, min_id1, max_ind, flat_m.size]
     fit_data = [bins, counts]
-    flag_min, r_2_min, popt_min = perform_gauss_fit(fit_param, fit_data, "Min")
+    flag_min, r_2_min, popt_min, perr_min = perform_gauss_fit(
+        fit_param, fit_data, "Min"
+    )
 
     ### 6. Find the inrterval of half height ###
     half_id0 = np.max([max_ind - gap, 0])
     half_id1 = np.min([max_ind + gap, counts.size - 1])
     while half_id0 > 0 and counts[half_id0] > max_val / 2:
         half_id0 -= 1
     while half_id1 < counts.size - 1 and counts[half_id1] > max_val / 2:
         half_id1 += 1
 
     ### 7. Try the fit between the minima and check its goodness ###
     fit_param = [half_id0, half_id1, max_ind, flat_m.size]
     fit_data = [bins, counts]
-    flag_half, r_2_half, popt_half = perform_gauss_fit(
+    flag_half, r_2_half, popt_half, perr_half = perform_gauss_fit(
         fit_param, fit_data, "Half"
     )
 
     ### 8. Choose the best fit ###
     r_2 = r_2_min
     if flag_min == 1 and flag_half == 0:
         popt = popt_min
+        perr = perr_min
     elif flag_min == 0 and flag_half == 1:
         popt = popt_half
+        perr = perr_half
         r_2 = r_2_half
     elif flag_min * flag_half == 1:
         if r_2_min >= r_2_half:
             popt = popt_min
+            perr = perr_min
         else:
             popt = popt_half
+            perr = perr_half
             r_2 = r_2_half
     else:
         print("\tWARNING: this fit is not converging.")
         return None
 
     state = StateUni(popt[0], popt[1], popt[2])
     state.build_boundaries(number_of_sigmas)
 
     with open(OUTPUT_FILE, "a", encoding="utf-8") as file:
         print("\n", file=file)
         print(
-            f"\tmu = {state.mean:.4f}, sigma = {state.sigma:.4f},"
-            f" area = {state.area:.4f}"
+            f"\tmu = {state.mean:.4f} ({perr[0]:.4f}), "
+            f"sigma = {state.sigma:.4f} ({perr[1]:.4f}), "
+            f"area = {state.area:.4f} ({perr[2]:.4f})"
         )
+        print(f"\tFit r2 = {r_2}")
         print(
-            f"\tmu = {state.mean:.4f}, sigma = {state.sigma:.4f},"
-            f" area = {state.area:.4f}",
+            f"\tmu = {state.mean:.4f} ({perr[0]:.4f}), "
+            f"sigma = {state.sigma:.4f} ({perr[1]:.4f}), "
+            f"area = {state.area:.4f} ({perr[2]:.4f})",
             file=file,
         )
         print(f"\tFit r2 = {r_2}", file=file)
 
     if full_out:
         ### Plot the distribution and the fitted gaussians
         y_spread = np.max(m_clean) - np.min(m_clean)
@@ -487,30 +481,30 @@
             min_id1 < counts.size - 1 and counts[min_id1] > counts[min_id1 + 1]
         ):
             min_id1 += 1
 
         ### 5. Try the fit between the minima and check its goodness ###
         fit_param = [min_id0, min_id1, m_ind, flat_m.size]
         fit_data = [bins, counts]
-        flag_min, r_2_min, popt_min = perform_gauss_fit(
+        flag_min, r_2_min, popt_min, _ = perform_gauss_fit(
             fit_param, fit_data, "Min"
         )
 
         ### 6. Find the inrterval of half height ###
         half_id0 = np.max([m_ind - gap, 0])
         half_id1 = np.min([m_ind + gap, counts.size - 1])
         while half_id0 > 0 and counts[half_id0] > max_val[i] / 2:
             half_id0 -= 1
         while half_id1 < counts.size - 1 and counts[half_id1] > max_val[i] / 2:
             half_id1 += 1
 
         ### 7. Try the fit between the minima and check its goodness ###
         fit_param = [half_id0, half_id1, m_ind, flat_m.size]
         fit_data = [bins, counts]
-        flag_half, r_2_half, popt_half = perform_gauss_fit(
+        flag_half, r_2_half, popt_half, _ = perform_gauss_fit(
             fit_param, fit_data, "Half"
         )
 
         ### 8. Choose the best fit ###
         if flag_min == 1 and flag_half == 0:
             popt = popt_min
         elif flag_min == 0 and flag_half == 1:
```

### Comparing `onion_clustering-0.2.3/src/onion_clustering/main_2d.py` & `onion_clustering-0.2.4/src/onion_clustering/main_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/src/onion_clustering/utilities.py` & `onion_clustering-0.2.4/src/onion_clustering/utilities.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/src/onion_clustering.egg-info/PKG-INFO` & `onion_clustering-0.2.4/src/onion_clustering.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.3
+Version: 0.2.4
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
@@ -19,15 +19,15 @@
 A one-dimensional time-series, computed on *N* particles for *T* frames. The input files must contain an array with shape *(N, T)* Supported formats: .npy, .npz, .txt. Also .xyz trajectories are supported, with the fifth column containing the data values. 
 
 ## Usage
 Install the package using `pip install onion_clustering`. 
 
 The `examples/` folder contains an example of usage. Run `python3 example_script.py`, this will create the following files:
 * A text file called `input_parameters.txt` , whose format is explained below;
-* A text file called `data_directory.txt` containing one line with the path to the input data file (including the input data file name). 
+* A text file called `data_directory.txt` containing one line with the path to the input data file (including the input data file name); 
 and run the code. 
 
 ## input_parameters.txt 
 * `tau_window` (int): the length of the time window (in number of frames). 
 * `t_smooth` (int, optional): the length of the smoothing window (in number of frames) for the moving average. A value of `t_smooth = 1` correspond to no smoothing. Default is 1. 
 * `t_delay` (int, optional): is for ignoring the first tau_delay frames of the trajectory. Default is 0. 
 * `t_conv` (int, optional): converts number of frames in time units. Default is 1. 
@@ -61,21 +61,17 @@
 The `main_2d.py` algorithm works in a similar fashion, taking as input 2D or 3D data. The input file contained in `data_directory.txt` must contain an array of shape `(D, N, T)` where _D_ is the number of components. Only `.npy, .npz` are supported. You can find an example of usage in `examples/example_script_2d.py`
 
 ## Required Python 3 packages
 `matplotlib`, `numpy`, `plotly`, `scipy`. 
 
 ## Gaussian fitting procedure
 1. The histogram of the time-series is computed, using the `bins='auto'` numpy option (unless a different `bins` is passed as imput parameter). 
-2. The histogram is smoothed with moving average with `window_size=3` (unless there are less that 50 bins, in wich case no smoothing occurs). 
+2. The histogram is smoothed with moving average with a window proportional to the number of bins (unless there are less that 50 bins, in wich case no smoothing occurs). 
 3. The absolute maximum of the histogram is found. 
 4. Two Gaussian fits are performed:
  * The first one inside the interval between the two minima surrounding the maximum. 
  * The second one inside the interval where the peak around the maxima has its half height. 
-5. Both fits, if converged, are evaluated according to the following points:
- * `mu` is contained inside the fit interval;
- * `sigma` is smaller than the fit interval;
- * the height of the peak is at least half the value of the maximum;
- * the relative uncertanty over the fit parameters is smaller than 0.5.
+5. Both fits, if converged, are evaluated according to the coefficinet of determination r^2. 
 6. Finally, the fit with the best score is chosen. If only one of the two converged, that one is chosen. If none of the fits converges, the iterative procedure stops, returning a warning message. 
 
 ## Aknowledgements
 Thanks to Andrew Tarzia for all the help with the code formatting and documentation, and to Domiziano Doria, Chiara Lionello and Simone Martino for the beta-testing. Writing all this code wouldn't have been possible without the help of ChatGPT.
```

### Comparing `onion_clustering-0.2.3/src/onion_clustering.egg-info/SOURCES.txt` & `onion_clustering-0.2.4/src/onion_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/test/output_uni/final_states.txt` & `onion_clustering-0.2.4/test/output_uni/final_states.txt`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/test/test_multi.py` & `onion_clustering-0.2.4/test/test_multi.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.3/test/test_uni.py` & `onion_clustering-0.2.4/test/test_uni.py`

 * *Files identical despite different names*

