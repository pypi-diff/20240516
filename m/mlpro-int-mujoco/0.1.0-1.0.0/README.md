# Comparing `tmp/mlpro_int_mujoco-0.1.0.tar.gz` & `tmp/mlpro_int_mujoco-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro_int_mujoco-0.1.0.tar", last modified: Wed May 15 07:24:51 2024, max compression
+gzip compressed data, was "mlpro_int_mujoco-1.0.0.tar", last modified: Thu May 16 09:18:42 2024, max compression
```

## Comparing `mlpro_int_mujoco-0.1.0.tar` & `mlpro_int_mujoco-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.325088 mlpro_int_mujoco-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-15 07:24:51.325088 mlpro_int_mujoco-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 07:24:51.325088 mlpro_int_mujoco-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.317088 mlpro_int_mujoco-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.317088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.317088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/envs/cartpole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.321088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.317088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.317088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.321088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Arrow.stl
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/X_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Y_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Z_letter.stl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.321088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/texture/
--rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/texture/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.317088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.321088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/base.stl
--rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/forearm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/shoulder.stl
--rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/upperarm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist1.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist2.stl
--rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist3.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/boxontable.xml
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/cartpole.xml
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/doublependulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/mlpro.xml
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/ur5.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.321088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40017 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/wrappers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.325088 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-15 07:24:51.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 07:24:51.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:24:51.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 07:24:51.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 07:24:51.000000 mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:24:51.325088 mlpro_int_mujoco-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-15 07:24:47.000000 mlpro_int_mujoco-0.1.0/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.942544 mlpro_int_mujoco-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-16 09:18:42.942544 mlpro_int_mujoco-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-16 09:18:42.942544 mlpro_int_mujoco-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.934544 mlpro_int_mujoco-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.934544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.938544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/envs/cartpole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.938544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.934544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.934544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.938544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Arrow.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/X_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Y_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Z_letter.stl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.938544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/texture/
+-rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/texture/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.934544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.942544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/base.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/forearm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/shoulder.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/upperarm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist2.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist3.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/boxontable.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/cartpole.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/doublependulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/mlpro.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/ur5.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.942544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40017 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/wrappers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.942544 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-16 09:18:42.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 09:18:42.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:18:42.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 09:18:42.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 09:18:42.000000 mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:18:42.942544 mlpro_int_mujoco-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-16 09:18:39.000000 mlpro_int_mujoco-1.0.0/test/test_examples.py
```

### Comparing `mlpro_int_mujoco-0.1.0/PKG-INFO` & `mlpro_int_mujoco-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-mujoco
-Version: 0.1.0
+Version: 1.0.0
 Summary: MLPro: Integration MuJoCo
 Home-page: https://mlpro-int-mujoco.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-mujoco.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro_int_mujoco-0.1.0/README.md` & `mlpro_int_mujoco-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/setup.cfg` & `mlpro_int_mujoco-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-mujoco
-version = 0.1.0
+version = 1.0.0
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration MuJoCo
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-mujoco.readthedocs.io
 project_urls =
```

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/envs/cartpole.py` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/envs/cartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Arrow.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Arrow.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/X_letter.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/X_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Y_letter.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Y_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Z_letter.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/mesh/Z_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/mlpro/texture/logo.png` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/mlpro/texture/logo.png`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/base.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/base.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/forearm.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/forearm.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/shoulder.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/shoulder.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/upperarm.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/upperarm.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist1.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist1.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist2.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist2.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist3.stl` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/assets/ur5/mesh/wrist3.stl`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/boxontable.xml` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/boxontable.xml`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/cartpole.xml` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/cartpole.xml`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/doublependulum.xml` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/doublependulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/mlpro.xml` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/mlpro.xml`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/pendulum.xml` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/pendulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/systems/ur5.xml` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/systems/ur5.xml`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco/wrappers/basics.py` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco/wrappers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco.egg-info/PKG-INFO` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-mujoco
-Version: 0.1.0
+Version: 1.0.0
 Summary: MLPro: Integration MuJoCo
 Home-page: https://mlpro-int-mujoco.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-mujoco.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro_int_mujoco-0.1.0/src/mlpro_int_mujoco.egg-info/SOURCES.txt` & `mlpro_int_mujoco-1.0.0/src/mlpro_int_mujoco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpro_int_mujoco-0.1.0/test/test_examples.py` & `mlpro_int_mujoco-1.0.0/test/test_examples.py`

 * *Files identical despite different names*

