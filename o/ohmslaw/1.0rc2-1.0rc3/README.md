# Comparing `tmp/ohmslaw-1.0rc2.tar.gz` & `tmp/ohmslaw-1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmslaw-1.0rc2.tar", last modified: Thu May 16 02:02:40 2024, max compression
+gzip compressed data, was "ohmslaw-1.0rc3.tar", last modified: Thu May 16 02:20:48 2024, max compression
```

## Comparing `ohmslaw-1.0rc2.tar` & `ohmslaw-1.0rc3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-16 02:02:40.722793 ohmslaw-1.0rc2/
--rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-05-16 01:55:11.000000 ohmslaw-1.0rc2/LICENSE
--rw-r--r--   0 juan      (1000) juan      (1000)     1311 2024-05-16 02:02:40.722793 ohmslaw-1.0rc2/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)       24 2024-05-16 01:55:11.000000 ohmslaw-1.0rc2/README.md
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-16 02:02:40.718793 ohmslaw-1.0rc2/ohmslaw/
--rw-rw-r--   0 juan      (1000) juan      (1000)      145 2024-05-16 02:00:29.000000 ohmslaw-1.0rc2/ohmslaw/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2174 2024-05-16 01:59:29.000000 ohmslaw-1.0rc2/ohmslaw/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-05-16 01:55:11.000000 ohmslaw-1.0rc2/ohmslaw/cli.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-16 02:02:40.722793 ohmslaw-1.0rc2/ohmslaw.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     1311 2024-05-16 02:02:40.000000 ohmslaw-1.0rc2/ohmslaw.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)      245 2024-05-16 02:02:40.000000 ohmslaw-1.0rc2/ohmslaw.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-16 02:02:40.000000 ohmslaw-1.0rc2/ohmslaw.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       45 2024-05-16 02:02:40.000000 ohmslaw-1.0rc2/ohmslaw.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        8 2024-05-16 02:02:40.000000 ohmslaw-1.0rc2/ohmslaw.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     1430 2024-05-16 01:58:16.000000 ohmslaw-1.0rc2/pyproject.toml
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-16 02:02:40.722793 ohmslaw-1.0rc2/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-16 02:20:48.797268 ohmslaw-1.0rc3/
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-05-16 01:55:11.000000 ohmslaw-1.0rc3/LICENSE
+-rw-r--r--   0 juan      (1000) juan      (1000)     2864 2024-05-16 02:20:48.797268 ohmslaw-1.0rc3/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1577 2024-05-16 02:19:54.000000 ohmslaw-1.0rc3/README.md
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-16 02:20:48.793268 ohmslaw-1.0rc3/ohmslaw/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      145 2024-05-16 02:00:29.000000 ohmslaw-1.0rc3/ohmslaw/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2172 2024-05-16 02:19:46.000000 ohmslaw-1.0rc3/ohmslaw/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-05-16 01:55:11.000000 ohmslaw-1.0rc3/ohmslaw/cli.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-16 02:20:48.793268 ohmslaw-1.0rc3/ohmslaw.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     2864 2024-05-16 02:20:48.000000 ohmslaw-1.0rc3/ohmslaw.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)      245 2024-05-16 02:20:48.000000 ohmslaw-1.0rc3/ohmslaw.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-16 02:20:48.000000 ohmslaw-1.0rc3/ohmslaw.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       45 2024-05-16 02:20:48.000000 ohmslaw-1.0rc3/ohmslaw.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        8 2024-05-16 02:20:48.000000 ohmslaw-1.0rc3/ohmslaw.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1430 2024-05-16 02:20:09.000000 ohmslaw-1.0rc3/pyproject.toml
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-16 02:20:48.797268 ohmslaw-1.0rc3/setup.cfg
```

### Comparing `ohmslaw-1.0rc2/LICENSE` & `ohmslaw-1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmslaw-1.0rc2/ohmslaw/__main__.py` & `ohmslaw-1.0rc3/ohmslaw/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 class Ohms:
     """A class representing basic electrical calculations based on Ohm's Law."""
     
-    def voltage(self, I: float, R: float) -> float:
+    def volts(self, I: float, R: float) -> float:
         """
         Calculate voltage using Ohm's Law.
 
         Parameters:
             I (float): The current in amperes.
             R (float): The resistance in ohms.
```

### Comparing `ohmslaw-1.0rc2/pyproject.toml` & `ohmslaw-1.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ohmslaw"
-version = "1.0-rc2"
+version = "1.0-rc3"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "python3 library for Ohms law."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

