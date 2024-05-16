# Comparing `tmp/melee-0.8.1.zip` & `tmp/melee-0.9.0.zip`

## zipinfo {}

```diff
@@ -1,31 +1,31 @@
-Zip file size: 268949 bytes, number of entries: 29
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jul-26 17:18 melee-0.8.1/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jul-26 17:18 melee-0.8.1/melee/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jul-26 17:18 melee-0.8.1/melee.egg-info/
--rw-r--r--  2.0 unx      433 b- defN 20-Jul-26 17:18 melee-0.8.1/PKG-INFO
--rw-r--r--  2.0 unx      145 b- defN 20-Jul-26 17:18 melee-0.8.1/MANIFEST.in
--rw-r--r--  2.0 unx       79 b- defN 20-Jul-26 17:18 melee-0.8.1/setup.cfg
--rw-r--r--  2.0 unx     6001 b- defN 20-Jul-26 17:18 melee-0.8.1/README.md
--rw-r--r--  2.0 unx      723 b- defN 20-Jul-26 17:18 melee-0.8.1/setup.py
--rw-r--r--  2.0 unx  2330130 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/framedata.csv
--rw-r--r--  2.0 unx     1075 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/stages.py
--rw-r--r--  2.0 unx    32633 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/console.py
--rw-r--r--  2.0 unx    11707 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/controller.py
--rw-r--r--  2.0 unx    22212 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/enums.py
--rw-r--r--  2.0 unx      815 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/characterdata.csv
--rw-r--r--  2.0 unx    20841 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/menuhelper.py
--rw-r--r--  2.0 unx    15729 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/actiondata.csv
--rw-r--r--  2.0 unx       46 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/version.py
--rw-r--r--  2.0 unx     3423 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/slippstream.py
--rw-r--r--  2.0 unx     1944 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/slpfilestreamer.py
--rw-r--r--  2.0 unx     7225 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/gamestate.py
--rw-r--r--  2.0 unx     1386 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/techskill.py
--rw-r--r--  2.0 unx      398 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/__init__.py
--rw-r--r--  2.0 unx     3687 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/logger.py
--rw-r--r--  2.0 unx    40871 b- defN 20-Jul-26 17:18 melee-0.8.1/melee/framedata.py
--rw-r--r--  2.0 unx      491 b- defN 20-Jul-26 17:18 melee-0.8.1/melee.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      433 b- defN 20-Jul-26 17:18 melee-0.8.1/melee.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       65 b- defN 20-Jul-26 17:18 melee-0.8.1/melee.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 20-Jul-26 17:18 melee-0.8.1/melee.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        6 b- defN 20-Jul-26 17:18 melee-0.8.1/melee.egg-info/top_level.txt
-29 files, 2502499 bytes uncompressed, 265035 bytes compressed:  89.4%
+Zip file size: 268967 bytes, number of entries: 29
+drwxr-xr-x  2.0 unx        0 b- stor 20-Aug-01 22:57 melee-0.9.0/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Aug-01 22:57 melee-0.9.0/melee/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Aug-01 22:57 melee-0.9.0/melee.egg-info/
+-rw-r--r--  2.0 unx       79 b- defN 20-Aug-01 22:57 melee-0.9.0/setup.cfg
+-rw-r--r--  2.0 unx      723 b- defN 20-Aug-01 22:57 melee-0.9.0/setup.py
+-rw-r--r--  2.0 unx      145 b- defN 20-Aug-01 22:57 melee-0.9.0/MANIFEST.in
+-rw-r--r--  2.0 unx     6001 b- defN 20-Aug-01 22:57 melee-0.9.0/README.md
+-rw-r--r--  2.0 unx      433 b- defN 20-Aug-01 22:57 melee-0.9.0/PKG-INFO
+-rw-r--r--  2.0 unx    22212 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/enums.py
+-rw-r--r--  2.0 unx      398 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/__init__.py
+-rw-r--r--  2.0 unx      815 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/characterdata.csv
+-rw-r--r--  2.0 unx    32757 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/console.py
+-rw-r--r--  2.0 unx  2330130 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/framedata.csv
+-rw-r--r--  2.0 unx    11707 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/controller.py
+-rw-r--r--  2.0 unx    40871 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/framedata.py
+-rw-r--r--  2.0 unx     1944 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/slpfilestreamer.py
+-rw-r--r--  2.0 unx     1386 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/techskill.py
+-rw-r--r--  2.0 unx     3687 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/logger.py
+-rw-r--r--  2.0 unx     3423 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/slippstream.py
+-rw-r--r--  2.0 unx    20841 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/menuhelper.py
+-rw-r--r--  2.0 unx    15729 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/actiondata.csv
+-rw-r--r--  2.0 unx     7225 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/gamestate.py
+-rw-r--r--  2.0 unx     1075 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/stages.py
+-rw-r--r--  2.0 unx       46 b- defN 20-Aug-01 22:57 melee-0.9.0/melee/version.py
+-rw-r--r--  2.0 unx      491 b- defN 20-Aug-01 22:57 melee-0.9.0/melee.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        6 b- defN 20-Aug-01 22:57 melee-0.9.0/melee.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Aug-01 22:57 melee-0.9.0/melee.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       65 b- defN 20-Aug-01 22:57 melee-0.9.0/melee.egg-info/requires.txt
+-rw-r--r--  2.0 unx      433 b- defN 20-Aug-01 22:57 melee-0.9.0/melee.egg-info/PKG-INFO
+29 files, 2502623 bytes uncompressed, 265053 bytes compressed:  89.4%
```

## zipnote {}

```diff
@@ -1,88 +1,88 @@
-Filename: melee-0.8.1/
+Filename: melee-0.9.0/
 Comment: 
 
-Filename: melee-0.8.1/melee/
+Filename: melee-0.9.0/melee/
 Comment: 
 
-Filename: melee-0.8.1/melee.egg-info/
+Filename: melee-0.9.0/melee.egg-info/
 Comment: 
 
-Filename: melee-0.8.1/PKG-INFO
+Filename: melee-0.9.0/setup.cfg
 Comment: 
 
-Filename: melee-0.8.1/MANIFEST.in
+Filename: melee-0.9.0/setup.py
 Comment: 
 
-Filename: melee-0.8.1/setup.cfg
+Filename: melee-0.9.0/MANIFEST.in
 Comment: 
 
-Filename: melee-0.8.1/README.md
+Filename: melee-0.9.0/README.md
 Comment: 
 
-Filename: melee-0.8.1/setup.py
+Filename: melee-0.9.0/PKG-INFO
 Comment: 
 
-Filename: melee-0.8.1/melee/framedata.csv
+Filename: melee-0.9.0/melee/enums.py
 Comment: 
 
-Filename: melee-0.8.1/melee/stages.py
+Filename: melee-0.9.0/melee/__init__.py
 Comment: 
 
-Filename: melee-0.8.1/melee/console.py
+Filename: melee-0.9.0/melee/characterdata.csv
 Comment: 
 
-Filename: melee-0.8.1/melee/controller.py
+Filename: melee-0.9.0/melee/console.py
 Comment: 
 
-Filename: melee-0.8.1/melee/enums.py
+Filename: melee-0.9.0/melee/framedata.csv
 Comment: 
 
-Filename: melee-0.8.1/melee/characterdata.csv
+Filename: melee-0.9.0/melee/controller.py
 Comment: 
 
-Filename: melee-0.8.1/melee/menuhelper.py
+Filename: melee-0.9.0/melee/framedata.py
 Comment: 
 
-Filename: melee-0.8.1/melee/actiondata.csv
+Filename: melee-0.9.0/melee/slpfilestreamer.py
 Comment: 
 
-Filename: melee-0.8.1/melee/version.py
+Filename: melee-0.9.0/melee/techskill.py
 Comment: 
 
-Filename: melee-0.8.1/melee/slippstream.py
+Filename: melee-0.9.0/melee/logger.py
 Comment: 
 
-Filename: melee-0.8.1/melee/slpfilestreamer.py
+Filename: melee-0.9.0/melee/slippstream.py
 Comment: 
 
-Filename: melee-0.8.1/melee/gamestate.py
+Filename: melee-0.9.0/melee/menuhelper.py
 Comment: 
 
-Filename: melee-0.8.1/melee/techskill.py
+Filename: melee-0.9.0/melee/actiondata.csv
 Comment: 
 
-Filename: melee-0.8.1/melee/__init__.py
+Filename: melee-0.9.0/melee/gamestate.py
 Comment: 
 
-Filename: melee-0.8.1/melee/logger.py
+Filename: melee-0.9.0/melee/stages.py
 Comment: 
 
-Filename: melee-0.8.1/melee/framedata.py
+Filename: melee-0.9.0/melee/version.py
 Comment: 
 
-Filename: melee-0.8.1/melee.egg-info/SOURCES.txt
+Filename: melee-0.9.0/melee.egg-info/SOURCES.txt
 Comment: 
 
-Filename: melee-0.8.1/melee.egg-info/PKG-INFO
+Filename: melee-0.9.0/melee.egg-info/top_level.txt
 Comment: 
 
-Filename: melee-0.8.1/melee.egg-info/requires.txt
+Filename: melee-0.9.0/melee.egg-info/dependency_links.txt
 Comment: 
 
-Filename: melee-0.8.1/melee.egg-info/dependency_links.txt
+Filename: melee-0.9.0/melee.egg-info/requires.txt
 Comment: 
 
-Filename: melee-0.8.1/melee.egg-info/top_level.txt
+Filename: melee-0.9.0/melee.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `melee-0.8.1/README.md` & `melee-0.9.0/README.md`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/setup.py` & `melee-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     packages = ['melee'],
     install_requires=[
         'pyenet',
         'serial',
         'py-ubjson',
         'pywin32; platform_system=="Windows"'
     ],
-    version = '0.8.1',
+    version = '0.9.0',
     description = 'Open API written in Python 3 for making your own Smash Bros: Melee AI that works with Slippi Online',
     author = 'AltF4',
     author_email = 'altf4petro@gmail.com',
     url = 'https://github.com/altf4/libmelee',
     download_url = 'https://api.github.com/repos/libmelee/libmelee/tarball',
     keywords = ['dolphin', 'AI', 'video games', 'melee', 'smash bros', 'slippi'],
     classifiers = [],
```

## Comparing `melee-0.8.1/melee/framedata.csv` & `melee-0.9.0/melee/framedata.csv`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/stages.py` & `melee-0.9.0/melee/stages.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/console.py` & `melee-0.9.0/melee/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 class Console:
     """The console object that represents your Dolphin / Wii / SLP file
     """
     def __init__(self,
                  path=None,
                  is_dolphin=True,
                  slippi_address="127.0.0.1",
+                 slippi_port=51441,
                  online_delay=2,
                  logger=None):
         """Create a Console object
 
         Args:
             path (str): Path to the directory where your dolphin executable is
                 located. (if applicable) None tells console to use the installed copy of the emulator
@@ -46,15 +47,15 @@
         self.logger = logger
         self.is_dolphin = is_dolphin
         self.path = path
         self.processingtime = 0
         self._frametimestamp = time.time()
         self.slippi_address = slippi_address
         """(str): IP address of the Dolphin / Wii to connect to."""
-        self.slippi_port = 51441
+        self.slippi_port = slippi_port
         """(int): TCP port of slippi server. Default 51441"""
         self.eventsize = [0] * 0x100
         self.render = True
         self.connected = False
         self.nick = ""
         """(str): The nickname the console has given itself."""
         self.version = ""
@@ -73,14 +74,15 @@
             self._slippstream = SlippstreamClient(self.slippi_address, self.slippi_port)
 
             # Setup some dolphin config options
             dolphin_config_path = self._get_dolphin_config_path() + "Dolphin.ini"
             config = configparser.SafeConfigParser()
             config.read(dolphin_config_path)
             config.set("Core", 'slippienablespectator', "True")
+            config.set("Core", 'slippispectatorlocalport', str(self.slippi_port))
             # Set online delay
             config.set("Core", 'slippionlinedelay', str(online_delay))
             # Turn on background input so we don't need to have window focus on dolphin
             config.set("Input", 'backgroundinput', "True")
             with open(dolphin_config_path, 'w') as dolphinfile:
                 config.write(dolphinfile)
         else:
```

## Comparing `melee-0.8.1/melee/controller.py` & `melee-0.9.0/melee/controller.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/enums.py` & `melee-0.9.0/melee/enums.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/characterdata.csv` & `melee-0.9.0/melee/characterdata.csv`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/menuhelper.py` & `melee-0.9.0/melee/menuhelper.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/actiondata.csv` & `melee-0.9.0/melee/actiondata.csv`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/slippstream.py` & `melee-0.9.0/melee/slippstream.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/slpfilestreamer.py` & `melee-0.9.0/melee/slpfilestreamer.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/gamestate.py` & `melee-0.9.0/melee/gamestate.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/techskill.py` & `melee-0.9.0/melee/techskill.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/logger.py` & `melee-0.9.0/melee/logger.py`

 * *Files identical despite different names*

## Comparing `melee-0.8.1/melee/framedata.py` & `melee-0.9.0/melee/framedata.py`

 * *Files identical despite different names*

