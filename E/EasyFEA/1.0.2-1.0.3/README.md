# Comparing `tmp/EasyFEA-1.0.2.tar.gz` & `tmp/EasyFEA-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyFEA-1.0.2.tar", last modified: Tue May 14 08:00:25 2024, max compression
+gzip compressed data, was "EasyFEA-1.0.3.tar", last modified: Thu May 16 10:21:52 2024, max compression
```

## Comparing `EasyFEA-1.0.2.tar` & `EasyFEA-1.0.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.106489 EasyFEA-1.0.2/
--rw-r--r--   0 matnoel    (501) staff       (20)      307 2024-05-08 15:55:35.000000 EasyFEA-1.0.2/AUTHORS.md
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.099151 EasyFEA-1.0.2/EasyFEA/
--rw-r--r--   0 matnoel    (501) staff       (20)    36204 2024-05-08 13:48:20.000000 EasyFEA-1.0.2/EasyFEA/Geoms.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1077 2024-05-08 13:26:51.000000 EasyFEA-1.0.2/EasyFEA/Materials.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1345 2024-05-08 13:26:54.000000 EasyFEA-1.0.2/EasyFEA/Simulations.py
--rw-r--r--   0 matnoel    (501) staff       (20)      556 2024-05-14 07:57:58.000000 EasyFEA-1.0.2/EasyFEA/__about__.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1212 2024-05-08 13:26:46.000000 EasyFEA-1.0.2/EasyFEA/__init__.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.101208 EasyFEA-1.0.2/EasyFEA/fem/
--rw-r--r--   0 matnoel    (501) staff       (20)      530 2024-05-08 13:24:58.000000 EasyFEA-1.0.2/EasyFEA/fem/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)     6446 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/fem/_boundary_conditions.py
--rw-r--r--   0 matnoel    (501) staff       (20)    11489 2024-05-08 13:25:02.000000 EasyFEA-1.0.2/EasyFEA/fem/_gauss.py
--rw-r--r--   0 matnoel    (501) staff       (20)    65816 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/fem/_gmsh_interface.py
--rw-r--r--   0 matnoel    (501) staff       (20)    68220 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/fem/_group_elems.py
--rw-r--r--   0 matnoel    (501) staff       (20)    37442 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/fem/_mesh.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1918 2024-05-08 13:33:39.000000 EasyFEA-1.0.2/EasyFEA/fem/_utils.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.102406 EasyFEA-1.0.2/EasyFEA/fem/elems/
--rw-r--r--   0 matnoel    (501) staff       (20)      268 2024-05-08 13:24:31.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)    23380 2024-05-08 13:24:34.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_hexa.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1053 2024-05-08 13:24:38.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_point.py
--rw-r--r--   0 matnoel    (501) staff       (20)    13846 2024-05-08 13:24:41.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_prism.py
--rw-r--r--   0 matnoel    (501) staff       (20)     5103 2024-05-08 13:24:43.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_quad.py
--rw-r--r--   0 matnoel    (501) staff       (20)    13086 2024-05-08 13:24:50.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_seg.py
--rw-r--r--   0 matnoel    (501) staff       (20)     7470 2024-05-08 13:24:52.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_tetra.py
--rw-r--r--   0 matnoel    (501) staff       (20)    12113 2024-05-08 13:24:55.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_tri.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.103311 EasyFEA-1.0.2/EasyFEA/materials/
--rw-r--r--   0 matnoel    (501) staff       (20)      563 2024-05-08 13:25:20.000000 EasyFEA-1.0.2/EasyFEA/materials/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)    11048 2024-05-08 13:25:22.000000 EasyFEA-1.0.2/EasyFEA/materials/_beam.py
--rw-r--r--   0 matnoel    (501) staff       (20)    24573 2024-05-08 13:25:24.000000 EasyFEA-1.0.2/EasyFEA/materials/_elastic.py
--rw-r--r--   0 matnoel    (501) staff       (20)    50153 2024-05-08 13:35:30.000000 EasyFEA-1.0.2/EasyFEA/materials/_phasefield.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2509 2024-05-08 13:25:28.000000 EasyFEA-1.0.2/EasyFEA/materials/_thermal.py
--rw-r--r--   0 matnoel    (501) staff       (20)    17464 2024-05-08 13:34:07.000000 EasyFEA-1.0.2/EasyFEA/materials/_utils.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.104585 EasyFEA-1.0.2/EasyFEA/simulations/
--rw-r--r--   0 matnoel    (501) staff       (20)    14581 2024-05-08 13:36:06.000000 EasyFEA-1.0.2/EasyFEA/simulations/Solvers.py
--rw-r--r--   0 matnoel    (501) staff       (20)      268 2024-05-08 13:25:37.000000 EasyFEA-1.0.2/EasyFEA/simulations/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)    30482 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/simulations/_beam.py
--rw-r--r--   0 matnoel    (501) staff       (20)    19587 2024-05-08 13:25:42.000000 EasyFEA-1.0.2/EasyFEA/simulations/_dic.py
--rw-r--r--   0 matnoel    (501) staff       (20)    19497 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/simulations/_elastic.py
--rw-r--r--   0 matnoel    (501) staff       (20)    31172 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/simulations/_phasefield.py
--rw-r--r--   0 matnoel    (501) staff       (20)    59684 2024-05-14 07:58:25.000000 EasyFEA-1.0.2/EasyFEA/simulations/_simu.py
--rw-r--r--   0 matnoel    (501) staff       (20)     7050 2024-05-08 13:25:58.000000 EasyFEA-1.0.2/EasyFEA/simulations/_thermal.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1868 2024-05-08 13:48:35.000000 EasyFEA-1.0.2/EasyFEA/simulations/_utils.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.105646 EasyFEA-1.0.2/EasyFEA/utilities/
--rw-r--r--   0 matnoel    (501) staff       (20)    46290 2024-05-08 14:04:02.000000 EasyFEA-1.0.2/EasyFEA/utilities/Display.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3421 2024-05-08 13:48:35.000000 EasyFEA-1.0.2/EasyFEA/utilities/Folder.py
--rw-r--r--   0 matnoel    (501) staff       (20)     8041 2024-05-08 13:26:30.000000 EasyFEA-1.0.2/EasyFEA/utilities/Numba_Interface.py
--rw-r--r--   0 matnoel    (501) staff       (20)     9702 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/utilities/Paraview_Interface.py
--rw-r--r--   0 matnoel    (501) staff       (20)    27540 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/utilities/PyVista_Interface.py
--rw-r--r--   0 matnoel    (501) staff       (20)      291 2024-05-08 13:26:11.000000 EasyFEA-1.0.2/EasyFEA/utilities/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1618 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/utilities/_observers.py
--rw-r--r--   0 matnoel    (501) staff       (20)     7126 2024-05-08 13:26:16.000000 EasyFEA-1.0.2/EasyFEA/utilities/_tic.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.099821 EasyFEA-1.0.2/EasyFEA.egg-info/
--rw-r--r--   0 matnoel    (501) staff       (20)    48948 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/PKG-INFO
--rw-r--r--   0 matnoel    (501) staff       (20)     1433 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/SOURCES.txt
--rw-r--r--   0 matnoel    (501) staff       (20)        1 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/dependency_links.txt
--rw-r--r--   0 matnoel    (501) staff       (20)      132 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/requires.txt
--rw-r--r--   0 matnoel    (501) staff       (20)        8 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/top_level.txt
--rw-r--r--   0 matnoel    (501) staff       (20)    35149 2024-04-26 09:17:40.000000 EasyFEA-1.0.2/LICENSE.txt
--rw-r--r--   0 matnoel    (501) staff       (20)    48948 2024-05-14 08:00:25.106214 EasyFEA-1.0.2/PKG-INFO
--rw-r--r--   0 matnoel    (501) staff       (20)     7021 2024-05-14 07:23:45.000000 EasyFEA-1.0.2/README.md
--rw-r--r--   0 matnoel    (501) staff       (20)     1378 2024-05-14 07:54:14.000000 EasyFEA-1.0.2/pyproject.toml
--rw-r--r--   0 matnoel    (501) staff       (20)       38 2024-05-14 08:00:25.106535 EasyFEA-1.0.2/setup.cfg
--rw-r--r--   0 matnoel    (501) staff       (20)       61 2024-03-19 17:45:45.000000 EasyFEA-1.0.2/setup.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-16 10:21:52.771325 EasyFEA-1.0.3/
+-rw-r--r--   0 matnoel    (501) staff       (20)      307 2024-05-08 15:55:35.000000 EasyFEA-1.0.3/AUTHORS.md
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-16 10:21:52.763916 EasyFEA-1.0.3/EasyFEA/
+-rw-r--r--   0 matnoel    (501) staff       (20)    36195 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/Geoms.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1068 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/Materials.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1336 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/Simulations.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      547 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/__about__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1203 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/__init__.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-16 10:21:52.765758 EasyFEA-1.0.3/EasyFEA/fem/
+-rw-r--r--   0 matnoel    (501) staff       (20)      521 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     6437 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/_boundary_conditions.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    11480 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/_gauss.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    65807 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/_gmsh_interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    68211 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/_group_elems.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    37433 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/_mesh.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1909 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-16 10:21:52.766852 EasyFEA-1.0.3/EasyFEA/fem/elems/
+-rw-r--r--   0 matnoel    (501) staff       (20)      259 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/elems/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    23371 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/elems/_hexa.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1044 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/elems/_point.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    13837 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/elems/_prism.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     5094 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/elems/_quad.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    13077 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/elems/_seg.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7461 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/elems/_tetra.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    12104 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/fem/elems/_tri.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-16 10:21:52.767735 EasyFEA-1.0.3/EasyFEA/materials/
+-rw-r--r--   0 matnoel    (501) staff       (20)      554 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/materials/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    11039 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/materials/_beam.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    24564 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/materials/_elastic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    50144 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/materials/_phasefield.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2500 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/materials/_thermal.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    17455 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/materials/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-16 10:21:52.769147 EasyFEA-1.0.3/EasyFEA/simulations/
+-rw-r--r--   0 matnoel    (501) staff       (20)    14572 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/Solvers.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      259 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    30473 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/_beam.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    19578 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/_dic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    19488 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/_elastic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    31163 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/_phasefield.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    59675 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/_simu.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7041 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/_thermal.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1859 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/simulations/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-16 10:21:52.770406 EasyFEA-1.0.3/EasyFEA/utilities/
+-rw-r--r--   0 matnoel    (501) staff       (20)    46281 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/utilities/Display.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3412 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/utilities/Folder.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     8032 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/utilities/Numba_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     9693 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/utilities/Paraview_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    27531 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/utilities/PyVista_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      282 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/utilities/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1623 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/utilities/_observers.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7117 2024-05-16 10:12:19.000000 EasyFEA-1.0.3/EasyFEA/utilities/_tic.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-16 10:21:52.764603 EasyFEA-1.0.3/EasyFEA.egg-info/
+-rw-r--r--   0 matnoel    (501) staff       (20)    48913 2024-05-16 10:21:52.000000 EasyFEA-1.0.3/EasyFEA.egg-info/PKG-INFO
+-rw-r--r--   0 matnoel    (501) staff       (20)     1433 2024-05-16 10:21:52.000000 EasyFEA-1.0.3/EasyFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)        1 2024-05-16 10:21:52.000000 EasyFEA-1.0.3/EasyFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)      132 2024-05-16 10:21:52.000000 EasyFEA-1.0.3/EasyFEA.egg-info/requires.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)        8 2024-05-16 10:21:52.000000 EasyFEA-1.0.3/EasyFEA.egg-info/top_level.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)    35149 2024-05-16 10:01:36.000000 EasyFEA-1.0.3/LICENSE.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)    48913 2024-05-16 10:21:52.771044 EasyFEA-1.0.3/PKG-INFO
+-rw-r--r--   0 matnoel    (501) staff       (20)     6986 2024-05-16 10:12:24.000000 EasyFEA-1.0.3/README.md
+-rw-r--r--   0 matnoel    (501) staff       (20)     1378 2024-05-16 10:21:10.000000 EasyFEA-1.0.3/pyproject.toml
+-rw-r--r--   0 matnoel    (501) staff       (20)       38 2024-05-16 10:21:52.771373 EasyFEA-1.0.3/setup.cfg
+-rw-r--r--   0 matnoel    (501) staff       (20)       61 2024-03-19 17:45:45.000000 EasyFEA-1.0.3/setup.py
```

### Comparing `EasyFEA-1.0.2/EasyFEA/Geoms.py` & `EasyFEA-1.0.3/EasyFEA/Geoms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module containing the geometric classes used to build meshes."""
 
 from typing import Union
 import numpy as np
 import copy
 import matplotlib.pyplot as plt
```

### Comparing `EasyFEA-1.0.2/EasyFEA/Materials.py` & `EasyFEA-1.0.3/EasyFEA/Materials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module containing material behavior. Such as elastic, damage, thermal and beam materials."""
 
 from .materials import Reshape_variable
 
 # ----------------------------------------------
 # Elastic
```

### Comparing `EasyFEA-1.0.2/EasyFEA/Simulations.py` & `EasyFEA-1.0.3/EasyFEA/Simulations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """This module contains all available simulation classes."""
 
 from .simulations._simu import _Simu, Load_Simu
 from .simulations._utils import Save_Force_Displacement, Load_Force_Displacement
 
 # ----------------------------------------------
```

### Comparing `EasyFEA-1.0.2/EasyFEA/__about__.py` & `EasyFEA-1.0.3/EasyFEA/__about__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 try:
     # Python 3.8+
     from importlib import metadata
 except ImportError:
     try:
         import importlib_metadata as metadata
```

### Comparing `EasyFEA-1.0.2/EasyFEA/__init__.py` & `EasyFEA-1.0.3/EasyFEA/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 # ----------------------------------------------
 # utilities
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/__init__.py` & `EasyFEA-1.0.3/EasyFEA/fem/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from ._utils import ElemType, MatrixType
 from ._mesh import Mesh, Mesh_Optim, Calc_projector
 from ._boundary_conditions import BoundaryCondition, LagrangeCondition
 from ._gmsh_interface import Mesher, gmsh
 from ._group_elems import _GroupElem, GroupElemFactory
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/_boundary_conditions.py` & `EasyFEA-1.0.3/EasyFEA/fem/_boundary_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module containing classes used to create boundary conditions."""
 
 import numpy as np
 
 class BoundaryCondition:
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/_gauss.py` & `EasyFEA-1.0.3/EasyFEA/fem/_gauss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module containing the Gauss class used to determine the coordinates and weights of integration points."""
 
 import numpy as np
 
 # utils
 from ._utils import ElemType, MatrixType
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/_gmsh_interface.py` & `EasyFEA-1.0.3/EasyFEA/fem/_gmsh_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module providing an interface with Gmsh (https://gmsh.info/).\n
 This module facilitates the manipulation of _Geom objects to create meshes through Gmsh with ease."""
 
 import gmsh
 import sys
 import os
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/_group_elems.py` & `EasyFEA-1.0.3/EasyFEA/fem/_group_elems.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Element group creation module.
 A mesh uses several element groups.
 For instance, a TRI3 mesh uses the elements POINT, SEG2 and TRI3."""
 
 from abc import ABC, abstractmethod, abstractproperty
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/_mesh.py` & `EasyFEA-1.0.3/EasyFEA/fem/_mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module containing the mesh class.
 This class allows you to manipulate different groups of elements.
 These element groups are used to construct finite element matrices."""
 
 import numpy as np
 import scipy.sparse as sp
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/_utils.py` & `EasyFEA-1.0.3/EasyFEA/fem/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from enum import Enum
 
 class ElemType(str, Enum):
     """Implemented element types"""
 
     POINT = "POINT"
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/elems/_hexa.py` & `EasyFEA-1.0.3/EasyFEA/fem/elems/_hexa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Hexa element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/elems/_point.py` & `EasyFEA-1.0.3/EasyFEA/fem/elems/_point.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Point element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/elems/_prism.py` & `EasyFEA-1.0.3/EasyFEA/fem/elems/_prism.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Prism element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/elems/_quad.py` & `EasyFEA-1.0.3/EasyFEA/fem/elems/_quad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Quad element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/elems/_seg.py` & `EasyFEA-1.0.3/EasyFEA/fem/elems/_seg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Seg element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/elems/_tetra.py` & `EasyFEA-1.0.3/EasyFEA/fem/elems/_tetra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Tetra element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
```

### Comparing `EasyFEA-1.0.2/EasyFEA/fem/elems/_tri.py` & `EasyFEA-1.0.3/EasyFEA/fem/elems/_tri.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Tri element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
```

### Comparing `EasyFEA-1.0.2/EasyFEA/materials/_beam.py` & `EasyFEA-1.0.3/EasyFEA/materials/_beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union
 
 # utilities
 from .. import np
 # others
```

### Comparing `EasyFEA-1.0.2/EasyFEA/materials/_elastic.py` & `EasyFEA-1.0.3/EasyFEA/materials/_elastic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union
 
 # utilities
 from .. import np
 # others
```

### Comparing `EasyFEA-1.0.2/EasyFEA/materials/_phasefield.py` & `EasyFEA-1.0.3/EasyFEA/materials/_phasefield.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union
 from enum import Enum
 
 from scipy.linalg import sqrtm
```

### Comparing `EasyFEA-1.0.2/EasyFEA/materials/_thermal.py` & `EasyFEA-1.0.3/EasyFEA/materials/_thermal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from typing import Union
 
 # utilities
 from .. import np
 
 from ._utils import _IModel, ModelType
```

### Comparing `EasyFEA-1.0.2/EasyFEA/materials/_utils.py` & `EasyFEA-1.0.3/EasyFEA/materials/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union
 from enum import Enum
 
 # utilities
 from ..utilities._observers import Observable
```

### Comparing `EasyFEA-1.0.2/EasyFEA/simulations/Solvers.py` & `EasyFEA-1.0.3/EasyFEA/simulations/Solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Interface module to various solvers available on python for solving linear systems of type [A](x) = (b)."""
 
 import sys
 from enum import Enum
 import numpy as np
 import scipy.sparse as sparse
```

### Comparing `EasyFEA-1.0.2/EasyFEA/simulations/_beam.py` & `EasyFEA-1.0.3/EasyFEA/simulations/_beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from typing import Union
 import numpy as np
 from scipy import sparse
 
 # utilities
 from ..utilities import Display, Tic
```

### Comparing `EasyFEA-1.0.2/EasyFEA/simulations/_dic.py` & `EasyFEA-1.0.3/EasyFEA/simulations/_dic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """DIC analysis module"""
 
 import numpy as np
 from scipy import interpolate, sparse
 from scipy.sparse.linalg import splu
 import pickle
```

### Comparing `EasyFEA-1.0.2/EasyFEA/simulations/_elastic.py` & `EasyFEA-1.0.3/EasyFEA/simulations/_elastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from typing import Union, Callable
 import numpy as np
 from scipy import sparse
 
 # utilities
 from ..utilities import Folder, Display, Tic
```

### Comparing `EasyFEA-1.0.2/EasyFEA/simulations/_phasefield.py` & `EasyFEA-1.0.3/EasyFEA/simulations/_phasefield.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from typing import Union
 import numpy as np
 from scipy import sparse
 import pandas as pd
 
 # utilities
```

### Comparing `EasyFEA-1.0.2/EasyFEA/simulations/_simu.py` & `EasyFEA-1.0.3/EasyFEA/simulations/_simu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from abc import ABC, abstractmethod
 import pickle
 from datetime import datetime
 from typing import Union
 import numpy as np
 from scipy import sparse
```

### Comparing `EasyFEA-1.0.2/EasyFEA/simulations/_thermal.py` & `EasyFEA-1.0.3/EasyFEA/simulations/_thermal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from typing import Union
 import numpy as np
 from scipy import sparse
 
 # utilities
 from ..utilities import Tic
```

### Comparing `EasyFEA-1.0.2/EasyFEA/simulations/_utils.py` & `EasyFEA-1.0.3/EasyFEA/simulations/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from ..utilities import Folder, Display
 import numpy as np
 
 import pickle
 
 # ----------------------------------------------
```

### Comparing `EasyFEA-1.0.2/EasyFEA/utilities/Display.py` & `EasyFEA-1.0.3/EasyFEA/utilities/Display.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module containing functions used to display simulations and meshes with matplotlib (https://matplotlib.org/)."""
 
 import platform
 from typing import Union, Callable
 import numpy as np
 import pandas as pd
```

### Comparing `EasyFEA-1.0.2/EasyFEA/utilities/Folder.py` & `EasyFEA-1.0.3/EasyFEA/utilities/Folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module containing functions used to facilitate folder and file creation using (os)."""
 
 import os
 
 def Get_Path(filename="") -> str:
     """Returns the folder containing the file. Otherwise returns the EasyFEA folder."""
```

### Comparing `EasyFEA-1.0.2/EasyFEA/utilities/Numba_Interface.py` & `EasyFEA-1.0.3/EasyFEA/utilities/Numba_Interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Numba functions to speed up calculations."""
 
 import numpy as np
 from numba import njit, prange, jit
 
 __USE_CACHE = True
```

### Comparing `EasyFEA-1.0.2/EasyFEA/utilities/Paraview_Interface.py` & `EasyFEA-1.0.3/EasyFEA/utilities/Paraview_Interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """This module allows you to save a simulation on Paraview (https://www.paraview.org/)."""
 
 import numpy as np
 
 # utilities
 from . import Display, Folder, Tic
```

### Comparing `EasyFEA-1.0.2/EasyFEA/utilities/PyVista_Interface.py` & `EasyFEA-1.0.3/EasyFEA/utilities/PyVista_Interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module providing an interface with PyVista (https://docs.pyvista.org/version/stable/)."""
 
 from typing import Union, Callable
 from cycler import cycler
 from scipy.sparse import csr_matrix
 import pyvista as pv
```

### Comparing `EasyFEA-1.0.2/EasyFEA/utilities/_observers.py` & `EasyFEA-1.0.3/EasyFEA/utilities/_observers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 from abc import ABC, abstractmethod
 
 class Observable:
     """The observable interface"""
 
     @property
     def observers(self):
         """Oberservers looking for the observable obect"""
         try:
-            return self.__observers
+            return self.__observers.copy()
         except AttributeError:
             # here self.__observers has not been created yet
             self.__observers: list[_IObserver] = []
-            return self.__observers
+            return self.__observers.copy()
     
     def _Add_observer(self, observer) -> None:
         """Add observer."""
 
         if not isinstance(observer, _IObserver):
             from .Display import MyPrintError
             MyPrintError(f'observer must be an {_IObserver.__name__}')
```

### Comparing `EasyFEA-1.0.2/EasyFEA/utilities/_tic.py` & `EasyFEA-1.0.3/EasyFEA/utilities/_tic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 # This file is part of the EasyFEA project.
-# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+# EasyFEA is distributed under the terms of the GNU General Public License v3 or later, see LICENSE.txt and CREDITS.md for more information.
 
 """Module containing the Tic class for timing tasks."""
 
 import time
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
```

### Comparing `EasyFEA-1.0.2/EasyFEA.egg-info/PKG-INFO` & `EasyFEA-1.0.3/EasyFEA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyFEA
-Version: 1.0.2
+Version: 1.0.3
 Summary: User-friendly Python library that simplifies finite element analysis.
 Author-email: Matthieu Noel <matthieu.noel7@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -800,36 +800,36 @@
 
 EasyFEA includes a few optional dependencies for reducing resolution time or for performing DIC:
 
 + [`pypardiso`](https://pypi.org/project/pypardiso/) (Python > 3.8 & Intel oneAPI)  - Library for solving large systems of sparse linear equations.
 + [`petsc`](https://pypi.org/project/petsc/) and [`petsc4py`](https://pypi.org/project/petsc4py/) - Python bindings for PETSc.
 + [`opencv-python`](https://pypi.org/project/opencv-python/) - Computer Vision package.
 
-# Naming conventions
+## Naming conventions
 
 **EasyFEA** uses Object-Oriented Programming ([OOP](https://en.wikipedia.org/wiki/Object-oriented_programming)) with the following naming conventions:
 + `PascalCasing` for classes
 + `camelCasing` for properties
 + `Snake_Casing` or `Snake_casing` for functions/methods
 
 In this library, objects can contain both **public** and **private** properties or functions.
 
 **Private** parameters or functions are designated by a double underscore, such as `__privateParam`. In addition, parameters or functions beginning with an underscore, such as `_My_Function` are accessible to advanced users, but should be used with caution.
 
-# Contributing
+## Contributing
 
 **EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
 
 To learn more about contributing to EasyFEA, please consult the [Contributing Guide](https://github.com/matnoel/EasyFEA/blob/main/CONTRIBUTING.md).
 
-# Citing EasyFEA
+## Citing EasyFEA
 
 If you are using EasyFEA as part of your scientific research, please contribute to the scientific visibility of the project by citing it as follows.
 
-> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, ⟨swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35⟩. ⟨hal-04571962⟩ 
+> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, https://hal.science/hal-04571962
 
 Bibtex:
 
 ```
 @softwareversion{noel:hal-04571962v1,
   TITLE = {{EasyFEA: a user-friendly Python library that simplifies finite element analysis}},
   AUTHOR = {Noel, Matthieu},
@@ -843,12 +843,12 @@
   LICENSE = {GNU General Public License v3.0 or later},
   KEYWORDS = {Finite element analyses ; Computational Mechanics ; Numerical Simulation ; Phase field modeling of brittle fracture ; Linear elasticity ; Euler-Bernoulli beam ; DIC - Digital Image Correlation ; User friendly ; Object oriented programming ; Mesh Generation},
   HAL_ID = {hal-04571962},
   HAL_VERSION = {v1},
 }
 ```
 
-# License
+## License
 
 Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 
-EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+EasyFEA is distributed under the terms of the [GNU General Public License v3.0 or later](https://spdx.org/licenses/GPL-3.0-or-later.html), see [LICENSE.txt](https://github.com/matnoel/EasyFEA/blob/main/LICENSE.txt) and [CREDITS.md](https://github.com/matnoel/EasyFEA/blob/main/CREDITS.md) for more information.
```

### Comparing `EasyFEA-1.0.2/EasyFEA.egg-info/SOURCES.txt` & `EasyFEA-1.0.3/EasyFEA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EasyFEA-1.0.2/LICENSE.txt` & `EasyFEA-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EasyFEA-1.0.2/PKG-INFO` & `EasyFEA-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyFEA
-Version: 1.0.2
+Version: 1.0.3
 Summary: User-friendly Python library that simplifies finite element analysis.
 Author-email: Matthieu Noel <matthieu.noel7@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -800,36 +800,36 @@
 
 EasyFEA includes a few optional dependencies for reducing resolution time or for performing DIC:
 
 + [`pypardiso`](https://pypi.org/project/pypardiso/) (Python > 3.8 & Intel oneAPI)  - Library for solving large systems of sparse linear equations.
 + [`petsc`](https://pypi.org/project/petsc/) and [`petsc4py`](https://pypi.org/project/petsc4py/) - Python bindings for PETSc.
 + [`opencv-python`](https://pypi.org/project/opencv-python/) - Computer Vision package.
 
-# Naming conventions
+## Naming conventions
 
 **EasyFEA** uses Object-Oriented Programming ([OOP](https://en.wikipedia.org/wiki/Object-oriented_programming)) with the following naming conventions:
 + `PascalCasing` for classes
 + `camelCasing` for properties
 + `Snake_Casing` or `Snake_casing` for functions/methods
 
 In this library, objects can contain both **public** and **private** properties or functions.
 
 **Private** parameters or functions are designated by a double underscore, such as `__privateParam`. In addition, parameters or functions beginning with an underscore, such as `_My_Function` are accessible to advanced users, but should be used with caution.
 
-# Contributing
+## Contributing
 
 **EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
 
 To learn more about contributing to EasyFEA, please consult the [Contributing Guide](https://github.com/matnoel/EasyFEA/blob/main/CONTRIBUTING.md).
 
-# Citing EasyFEA
+## Citing EasyFEA
 
 If you are using EasyFEA as part of your scientific research, please contribute to the scientific visibility of the project by citing it as follows.
 
-> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, ⟨swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35⟩. ⟨hal-04571962⟩ 
+> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, https://hal.science/hal-04571962
 
 Bibtex:
 
 ```
 @softwareversion{noel:hal-04571962v1,
   TITLE = {{EasyFEA: a user-friendly Python library that simplifies finite element analysis}},
   AUTHOR = {Noel, Matthieu},
@@ -843,12 +843,12 @@
   LICENSE = {GNU General Public License v3.0 or later},
   KEYWORDS = {Finite element analyses ; Computational Mechanics ; Numerical Simulation ; Phase field modeling of brittle fracture ; Linear elasticity ; Euler-Bernoulli beam ; DIC - Digital Image Correlation ; User friendly ; Object oriented programming ; Mesh Generation},
   HAL_ID = {hal-04571962},
   HAL_VERSION = {v1},
 }
 ```
 
-# License
+## License
 
 Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 
-EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+EasyFEA is distributed under the terms of the [GNU General Public License v3.0 or later](https://spdx.org/licenses/GPL-3.0-or-later.html), see [LICENSE.txt](https://github.com/matnoel/EasyFEA/blob/main/LICENSE.txt) and [CREDITS.md](https://github.com/matnoel/EasyFEA/blob/main/CREDITS.md) for more information.
```

### Comparing `EasyFEA-1.0.2/README.md` & `EasyFEA-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -88,36 +88,36 @@
 
 EasyFEA includes a few optional dependencies for reducing resolution time or for performing DIC:
 
 + [`pypardiso`](https://pypi.org/project/pypardiso/) (Python > 3.8 & Intel oneAPI)  - Library for solving large systems of sparse linear equations.
 + [`petsc`](https://pypi.org/project/petsc/) and [`petsc4py`](https://pypi.org/project/petsc4py/) - Python bindings for PETSc.
 + [`opencv-python`](https://pypi.org/project/opencv-python/) - Computer Vision package.
 
-# Naming conventions
+## Naming conventions
 
 **EasyFEA** uses Object-Oriented Programming ([OOP](https://en.wikipedia.org/wiki/Object-oriented_programming)) with the following naming conventions:
 + `PascalCasing` for classes
 + `camelCasing` for properties
 + `Snake_Casing` or `Snake_casing` for functions/methods
 
 In this library, objects can contain both **public** and **private** properties or functions.
 
 **Private** parameters or functions are designated by a double underscore, such as `__privateParam`. In addition, parameters or functions beginning with an underscore, such as `_My_Function` are accessible to advanced users, but should be used with caution.
 
-# Contributing
+## Contributing
 
 **EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
 
 To learn more about contributing to EasyFEA, please consult the [Contributing Guide](https://github.com/matnoel/EasyFEA/blob/main/CONTRIBUTING.md).
 
-# Citing EasyFEA
+## Citing EasyFEA
 
 If you are using EasyFEA as part of your scientific research, please contribute to the scientific visibility of the project by citing it as follows.
 
-> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, ⟨swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35⟩. ⟨hal-04571962⟩ 
+> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, https://hal.science/hal-04571962
 
 Bibtex:
 
 ```
 @softwareversion{noel:hal-04571962v1,
   TITLE = {{EasyFEA: a user-friendly Python library that simplifies finite element analysis}},
   AUTHOR = {Noel, Matthieu},
@@ -131,12 +131,12 @@
   LICENSE = {GNU General Public License v3.0 or later},
   KEYWORDS = {Finite element analyses ; Computational Mechanics ; Numerical Simulation ; Phase field modeling of brittle fracture ; Linear elasticity ; Euler-Bernoulli beam ; DIC - Digital Image Correlation ; User friendly ; Object oriented programming ; Mesh Generation},
   HAL_ID = {hal-04571962},
   HAL_VERSION = {v1},
 }
 ```
 
-# License
+## License
 
 Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
 
-EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+EasyFEA is distributed under the terms of the [GNU General Public License v3.0 or later](https://spdx.org/licenses/GPL-3.0-or-later.html), see [LICENSE.txt](https://github.com/matnoel/EasyFEA/blob/main/LICENSE.txt) and [CREDITS.md](https://github.com/matnoel/EasyFEA/blob/main/CREDITS.md) for more information.
```

### Comparing `EasyFEA-1.0.2/pyproject.toml` & `EasyFEA-1.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EasyFEA"
-version = "1.0.2"
+version = "1.0.3"
 description = "User-friendly Python library that simplifies finite element analysis."
 authors = [
     {name = "Matthieu Noel", email = "matthieu.noel7@gmail.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["finite-element-analysis", "phase-field", "python", "easy", "fem"]
```

