# Comparing `tmp/Audio_SpectraCLI-3.1.tar.gz` & `tmp/Audio_SpectraCLI-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Audio_SpectraCLI-3.1.tar", last modified: Thu Mar 28 14:33:58 2024, max compression
+gzip compressed data, was "Audio_SpectraCLI-3.2.tar", last modified: Thu May 16 15:31:10 2024, max compression
```

## Comparing `Audio_SpectraCLI-3.1.tar` & `Audio_SpectraCLI-3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:58.803037 Audio_SpectraCLI-3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:58.803037 Audio_SpectraCLI-3.1/Audio_SpectraCLI/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 14:33:41.000000 Audio_SpectraCLI-3.1/Audio_SpectraCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-28 14:33:57.000000 Audio_SpectraCLI-3.1/Audio_SpectraCLI/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:58.803037 Audio_SpectraCLI-3.1/Audio_SpectraCLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-03-28 14:33:58.000000 Audio_SpectraCLI-3.1/Audio_SpectraCLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-28 14:33:58.000000 Audio_SpectraCLI-3.1/Audio_SpectraCLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:33:58.000000 Audio_SpectraCLI-3.1/Audio_SpectraCLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 14:33:58.000000 Audio_SpectraCLI-3.1/Audio_SpectraCLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-28 14:33:58.000000 Audio_SpectraCLI-3.1/Audio_SpectraCLI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-28 14:33:41.000000 Audio_SpectraCLI-3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-03-28 14:33:58.803037 Audio_SpectraCLI-3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-28 14:33:58.803037 Audio_SpectraCLI-3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-28 14:33:57.000000 Audio_SpectraCLI-3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/Audio_SpectraCLI/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 15:30:51.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-16 15:31:07.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 15:30:51.000000 Audio_SpectraCLI-3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-16 15:31:07.000000 Audio_SpectraCLI-3.2/setup.py
```

### Comparing `Audio_SpectraCLI-3.1/Audio_SpectraCLI/main.py` & `Audio_SpectraCLI-3.2/Audio_SpectraCLI/main.py`

 * *Files identical despite different names*

### Comparing `Audio_SpectraCLI-3.1/LICENSE` & `Audio_SpectraCLI-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Audio_SpectraCLI-3.1/setup.cfg` & `Audio_SpectraCLI-3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Audio-SpectraCLI
-version = 3.1
+version = 3.2
 author = Aditya Seth
 author_email = contact@adityaseth.in
 description = AudioSpectraCLI is a command-line tool that provides real-time FFT visualization of audio spectra. It captures audio input from the microphone and displays the corresponding frequency spectrum directly in the terminal window, allowing users to monitor and analyze audio signals without the need for graphical interfaces.
 license = MIT
 home-page = https://github.com/AdityaSeth777/Audio-SpectraCLI
 
 [egg_info]
```

### Comparing `Audio_SpectraCLI-3.1/setup.py` & `Audio_SpectraCLI-3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Audio_SpectraCLI",
-    version="3.1",
+    version="3.2",
     author="Aditya Seth",
     long_description=open("Readme.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "matplotlib",
```

