# Comparing `tmp/ohmslaw-1.0rc8.tar.gz` & `tmp/ohmslaw-1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmslaw-1.0rc8.tar", last modified: Thu May 16 13:43:56 2024, max compression
+gzip compressed data, was "ohmslaw-1.0rc9.tar", last modified: Thu May 16 13:49:17 2024, max compression
```

## Comparing `ohmslaw-1.0rc8.tar` & `ohmslaw-1.0rc9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:43:56.952690 ohmslaw-1.0rc8/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-16 13:09:17.000000 ohmslaw-1.0rc8/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     2874 2024-05-16 13:43:56.952690 ohmslaw-1.0rc8/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1587 2024-05-16 13:09:17.000000 ohmslaw-1.0rc8/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:43:56.952690 ohmslaw-1.0rc8/ohmslaw/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      145 2024-05-16 13:30:25.000000 ohmslaw-1.0rc8/ohmslaw/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2189 2024-05-16 13:09:17.000000 ohmslaw-1.0rc8/ohmslaw/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3188 2024-05-16 13:42:43.000000 ohmslaw-1.0rc8/ohmslaw/cli.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:43:56.952690 ohmslaw-1.0rc8/ohmslaw.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     2874 2024-05-16 13:43:56.000000 ohmslaw-1.0rc8/ohmslaw.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      245 2024-05-16 13:43:56.000000 ohmslaw-1.0rc8/ohmslaw.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-16 13:43:56.000000 ohmslaw-1.0rc8/ohmslaw.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       45 2024-05-16 13:43:56.000000 ohmslaw-1.0rc8/ohmslaw.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        8 2024-05-16 13:43:56.000000 ohmslaw-1.0rc8/ohmslaw.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1430 2024-05-16 13:42:19.000000 ohmslaw-1.0rc8/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-16 13:43:56.952690 ohmslaw-1.0rc8/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:49:17.158396 ohmslaw-1.0rc9/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-16 13:09:17.000000 ohmslaw-1.0rc9/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     2874 2024-05-16 13:49:17.158396 ohmslaw-1.0rc9/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1587 2024-05-16 13:09:17.000000 ohmslaw-1.0rc9/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:49:17.150396 ohmslaw-1.0rc9/ohmslaw/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      145 2024-05-16 13:30:25.000000 ohmslaw-1.0rc9/ohmslaw/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2189 2024-05-16 13:09:17.000000 ohmslaw-1.0rc9/ohmslaw/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3212 2024-05-16 13:48:04.000000 ohmslaw-1.0rc9/ohmslaw/cli.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:49:17.154396 ohmslaw-1.0rc9/ohmslaw.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     2874 2024-05-16 13:49:17.000000 ohmslaw-1.0rc9/ohmslaw.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      245 2024-05-16 13:49:17.000000 ohmslaw-1.0rc9/ohmslaw.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-16 13:49:17.000000 ohmslaw-1.0rc9/ohmslaw.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       45 2024-05-16 13:49:17.000000 ohmslaw-1.0rc9/ohmslaw.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        8 2024-05-16 13:49:17.000000 ohmslaw-1.0rc9/ohmslaw.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1430 2024-05-16 13:48:32.000000 ohmslaw-1.0rc9/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-16 13:49:17.158396 ohmslaw-1.0rc9/setup.cfg
```

### Comparing `ohmslaw-1.0rc8/LICENSE` & `ohmslaw-1.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmslaw-1.0rc8/PKG-INFO` & `ohmslaw-1.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmslaw
-Version: 1.0rc8
+Version: 1.0rc9
 Summary: python3 library for Ohms law.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/ohmslaw
 Project-URL: Bug Reports, https://github.com/juanbindez/ohmslaw/issues
 Project-URL: Read the Docs, http://ohmslaw.readthedocs.io/
 Keywords: eletric,ohms,calc,tools
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ohmslaw Version: 1.0rc8 Summary: python3 library
+Metadata-Version: 2.1 Name: ohmslaw Version: 1.0rc9 Summary: python3 library
 for Ohms law. Author-email: Juan Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/ohmslaw Project-URL: Bug Reports, https://github.com/juanbindez/
 ohmslaw/issues Project-URL: Read the Docs, http://ohmslaw.readthedocs.io/
 Keywords: eletric,ohms,calc,tools Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
```

### Comparing `ohmslaw-1.0rc8/README.md` & `ohmslaw-1.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `ohmslaw-1.0rc8/ohmslaw/__main__.py` & `ohmslaw-1.0rc9/ohmslaw/__main__.py`

 * *Files identical despite different names*

### Comparing `ohmslaw-1.0rc8/ohmslaw/cli.py` & `ohmslaw-1.0rc9/ohmslaw/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return ohms.resistance(V, I)
 
 def find_resistor(source, component_voltage, component_current=0.02):
     """Calculate resistor value to limit current."""
     ohms = Ohms()
     return ohms.find_resistor(source, component_voltage, component_current)
 
-def main():
+def main() -> str:
     import argparse
     parser = argparse.ArgumentParser(description="Perform electrical calculations based on Ohm's Law")
     subparsers = parser.add_subparsers(dest='operation', help='Operation to perform')
 
     # Subparser for volts operation
     volts_parser = subparsers.add_parser('volts', help='Calculate voltage using Ohm\'s Law')
     volts_parser.add_argument('-I', type=float, required=True, help='Current in amperes')
@@ -49,21 +49,21 @@
     find_resistor_parser.add_argument('--component_current', type=float, default=0.02, help='Component current in amperes (default: 0.02)')
 
     args = parser.parse_args()
 
     result = []
 
     if args.operation == 'volts':
-        result = calculate_volts(args.I, args.R), + "V"
+        result = str(calculate_volts(args.I, args.R)) + "V"
     elif args.operation == 'current':
-        result = calculate_current(args.V, args.R), + "A"
+        result = str(calculate_current(args.V, args.R)) + "A"
     elif args.operation == 'resistance':
-        result = calculate_resistance(args.V, args.I), + "Ohms"
+        result = str(calculate_resistance(args.V, args.I)) + "Ohms"
     elif args.operation == 'find_resistor':
-        result = find_resistor(args.source, args.component_voltage, args.component_current) + "Ohms"
+        result = str(find_resistor(args.source, args.component_voltage, args.component_current)) + "Ohms"
 
     print(result)
     return result
 
 if __name__ == "__main__":
     main()
```

### Comparing `ohmslaw-1.0rc8/ohmslaw.egg-info/PKG-INFO` & `ohmslaw-1.0rc9/ohmslaw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmslaw
-Version: 1.0rc8
+Version: 1.0rc9
 Summary: python3 library for Ohms law.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/ohmslaw
 Project-URL: Bug Reports, https://github.com/juanbindez/ohmslaw/issues
 Project-URL: Read the Docs, http://ohmslaw.readthedocs.io/
 Keywords: eletric,ohms,calc,tools
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ohmslaw Version: 1.0rc8 Summary: python3 library
+Metadata-Version: 2.1 Name: ohmslaw Version: 1.0rc9 Summary: python3 library
 for Ohms law. Author-email: Juan Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/ohmslaw Project-URL: Bug Reports, https://github.com/juanbindez/
 ohmslaw/issues Project-URL: Read the Docs, http://ohmslaw.readthedocs.io/
 Keywords: eletric,ohms,calc,tools Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
```

### Comparing `ohmslaw-1.0rc8/pyproject.toml` & `ohmslaw-1.0rc9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ohmslaw"
-version = "1.0-rc8"
+version = "1.0-rc9"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "python3 library for Ohms law."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

