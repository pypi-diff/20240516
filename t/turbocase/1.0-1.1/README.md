# Comparing `tmp/turbocase-1.0.tar.gz` & `tmp/turbocase-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbocase-1.0.tar", last modified: Wed May 15 14:32:32 2024, max compression
+gzip compressed data, was "turbocase-1.1.tar", last modified: Wed May 15 14:45:34 2024, max compression
```

## Comparing `turbocase-1.0.tar` & `turbocase-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:32:32.442802 turbocase-1.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-15 14:32:32.442802 turbocase-1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1478 2024-05-15 14:28:38.000000 turbocase-1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 14:32:32.442802 turbocase-1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-15 14:30:20.000000 turbocase-1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:32:32.442802 turbocase-1.0/turbocase/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.0/turbocase/__init__.py
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 14:14:49.000000 turbocase-1.0/turbocase/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1356 2024-05-15 14:29:21.000000 turbocase-1.0/turbocase/cases.py
--rw-r--r--   0 root         (0) root         (0)     5424 2024-05-15 14:13:53.000000 turbocase-1.0/turbocase/kicad.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-05-15 14:08:06.000000 turbocase-1.0/turbocase/scad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:32:32.442802 turbocase-1.0/turbocase.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-15 14:32:32.000000 turbocase-1.0/turbocase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      330 2024-05-15 14:32:32.000000 turbocase-1.0/turbocase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 14:32:32.000000 turbocase-1.0/turbocase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-15 14:32:32.000000 turbocase-1.0/turbocase.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-15 14:32:32.000000 turbocase-1.0/turbocase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-15 14:32:32.000000 turbocase-1.0/turbocase.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:45:34.940369 turbocase-1.1/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-15 14:45:34.940369 turbocase-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-15 14:44:48.000000 turbocase-1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 14:45:34.940369 turbocase-1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-15 14:41:03.000000 turbocase-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:45:34.937036 turbocase-1.1/turbocase/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.1/turbocase/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-15 14:42:59.000000 turbocase-1.1/turbocase/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2024-05-15 14:29:21.000000 turbocase-1.1/turbocase/cases.py
+-rw-r--r--   0 root         (0) root         (0)     5424 2024-05-15 14:13:53.000000 turbocase-1.1/turbocase/kicad.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-05-15 14:08:06.000000 turbocase-1.1/turbocase/scad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:45:34.940369 turbocase-1.1/turbocase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-15 14:45:34.000000 turbocase-1.1/turbocase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      330 2024-05-15 14:45:34.000000 turbocase-1.1/turbocase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 14:45:34.000000 turbocase-1.1/turbocase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-15 14:45:34.000000 turbocase-1.1/turbocase.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-15 14:45:34.000000 turbocase-1.1/turbocase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-15 14:45:34.000000 turbocase-1.1/turbocase.egg-info/top_level.txt
```

### Comparing `turbocase-1.0/LICENSE.txt` & `turbocase-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `turbocase-1.0/README.md` & `turbocase-1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -14,18 +14,45 @@
 PCB to fit threaded metal inserts after 3D printing. It currently is hardcoded to the bag of M3 inserts I have.
 
 For connectors KiCAD needs to learn about the third dimension. For this purpose I have added a "Height" property to
 the connects I want to be processed by turbocase that defines the height from the top of the PCB to the top of the
 connector so an appropiate cutout can be made in the case. The rest of the shape of the connector is defined by the
 bounding box of the F.Fab layer of the connector.
 
+An example of a KiCAD PCB with a case outline on `User.6`:
+![KiCAD PCB with case outline](images/kicad.png)
+
+The generated case from this file:
+![OpenSCAD model of the generated case](images/scad.png)
+
+
 ## Installation
 
 ```shell-session
 $ pip install turbocase
 ```
 
 ## Usage
 
+1. Create a case outline in the `User.6` layer using the line drawing tools.
+2. Add the `Height` property to the connector footprints that need to be in the case export
+3. Ensure the screw holes for the PCB are MountingHole footprints
+4. Run the turbocase tool to make an OpenSCAD file:
 ```shell-session
 $ turbocase project/project.kicad_pcb case.scad
+```
+
+## Command line options
+
+```
+usage: turbocase [-h] [--layer LAYER] [--bottom BOTTOM] [--wall WALL] pcb output
+
+positional arguments:
+  pcb              Input kicad PCB file
+  output           Generated openSCAD case template
+
+options:
+  -h, --help       show this help message and exit
+  --layer LAYER    Layer with the case inner-outline [defaults to User.6]
+  --bottom BOTTOM  Bottom thickness in mm [default 1.2]
+  --wall WALL      Wall thickness in mm [default 1.2]
 ```
```

### Comparing `turbocase-1.0/turbocase/__main__.py` & `turbocase-1.1/turbocase/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,17 +5,23 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('pcb', help='Input kicad PCB file')
     parser.add_argument('output', help='Generated openSCAD case template')
     parser.add_argument('--layer', help='Layer with the case inner-outline [defaults to User.6]', default='User.6')
+    parser.add_argument('--bottom', help='Bottom thickness in mm [default 1.2]', default=1.2, type=float)
+    parser.add_argument('--wall', help='Wall thickness in mm [default 1.2]', default=1.2, type=float)
     args = parser.parse_args()
 
     case = load_pcb(args.pcb, args.layer)
+
+    case.floor_thickness = args.bottom
+    case.wall_thickness = args.wall
+
     code = scad.generate(case)
     with open(args.output, 'w') as handle:
         handle.write(code)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `turbocase-1.0/turbocase/cases.py` & `turbocase-1.1/turbocase/cases.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.0/turbocase/kicad.py` & `turbocase-1.1/turbocase/kicad.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.0/turbocase/scad.py` & `turbocase-1.1/turbocase/scad.py`

 * *Files identical despite different names*

