# Comparing `tmp/ohmslaw-1.0rc5.tar.gz` & `tmp/ohmslaw-1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmslaw-1.0rc5.tar", last modified: Thu May 16 13:22:43 2024, max compression
+gzip compressed data, was "ohmslaw-1.0rc6.tar", last modified: Thu May 16 13:31:37 2024, max compression
```

## Comparing `ohmslaw-1.0rc5.tar` & `ohmslaw-1.0rc6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:22:43.499722 ohmslaw-1.0rc5/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-16 13:09:17.000000 ohmslaw-1.0rc5/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     2874 2024-05-16 13:22:43.499722 ohmslaw-1.0rc5/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1587 2024-05-16 13:09:17.000000 ohmslaw-1.0rc5/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:22:43.499722 ohmslaw-1.0rc5/ohmslaw/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      145 2024-05-16 13:09:17.000000 ohmslaw-1.0rc5/ohmslaw/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2189 2024-05-16 13:09:17.000000 ohmslaw-1.0rc5/ohmslaw/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2796 2024-05-16 13:21:21.000000 ohmslaw-1.0rc5/ohmslaw/cli.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:22:43.499722 ohmslaw-1.0rc5/ohmslaw.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     2874 2024-05-16 13:22:43.000000 ohmslaw-1.0rc5/ohmslaw.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      245 2024-05-16 13:22:43.000000 ohmslaw-1.0rc5/ohmslaw.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-16 13:22:43.000000 ohmslaw-1.0rc5/ohmslaw.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       45 2024-05-16 13:22:43.000000 ohmslaw-1.0rc5/ohmslaw.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        8 2024-05-16 13:22:43.000000 ohmslaw-1.0rc5/ohmslaw.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1430 2024-05-16 13:21:49.000000 ohmslaw-1.0rc5/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-16 13:22:43.499722 ohmslaw-1.0rc5/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:31:37.326623 ohmslaw-1.0rc6/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-16 13:09:17.000000 ohmslaw-1.0rc6/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     2874 2024-05-16 13:31:37.322623 ohmslaw-1.0rc6/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1587 2024-05-16 13:09:17.000000 ohmslaw-1.0rc6/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:31:37.322623 ohmslaw-1.0rc6/ohmslaw/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      145 2024-05-16 13:30:25.000000 ohmslaw-1.0rc6/ohmslaw/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2189 2024-05-16 13:09:17.000000 ohmslaw-1.0rc6/ohmslaw/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3128 2024-05-16 13:30:56.000000 ohmslaw-1.0rc6/ohmslaw/cli.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-16 13:31:37.322623 ohmslaw-1.0rc6/ohmslaw.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     2874 2024-05-16 13:31:37.000000 ohmslaw-1.0rc6/ohmslaw.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      245 2024-05-16 13:31:37.000000 ohmslaw-1.0rc6/ohmslaw.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-16 13:31:37.000000 ohmslaw-1.0rc6/ohmslaw.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       45 2024-05-16 13:31:37.000000 ohmslaw-1.0rc6/ohmslaw.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        8 2024-05-16 13:31:37.000000 ohmslaw-1.0rc6/ohmslaw.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1430 2024-05-16 13:30:50.000000 ohmslaw-1.0rc6/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-16 13:31:37.326623 ohmslaw-1.0rc6/setup.cfg
```

### Comparing `ohmslaw-1.0rc5/LICENSE` & `ohmslaw-1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmslaw-1.0rc5/PKG-INFO` & `ohmslaw-1.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmslaw
-Version: 1.0rc5
+Version: 1.0rc6
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
-Metadata-Version: 2.1 Name: ohmslaw Version: 1.0rc5 Summary: python3 library
+Metadata-Version: 2.1 Name: ohmslaw Version: 1.0rc6 Summary: python3 library
 for Ohms law. Author-email: Juan Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/ohmslaw Project-URL: Bug Reports, https://github.com/juanbindez/
 ohmslaw/issues Project-URL: Read the Docs, http://ohmslaw.readthedocs.io/
 Keywords: eletric,ohms,calc,tools Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
```

### Comparing `ohmslaw-1.0rc5/README.md` & `ohmslaw-1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `ohmslaw-1.0rc5/ohmslaw/__main__.py` & `ohmslaw-1.0rc6/ohmslaw/__main__.py`

 * *Files identical despite different names*

### Comparing `ohmslaw-1.0rc5/ohmslaw/cli.py` & `ohmslaw-1.0rc6/ohmslaw/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 import argparse
-
 from ohmslaw.__main__ import Ohms
 
-class OhmsCLI:
-    """Command line interface for Ohms calculations."""
 
-    def __init__(self):
-        self.parser = argparse.ArgumentParser(description='Perform electrical calculations based on Ohm\'s Law')
-        self.subparsers = self.parser.add_subparsers(dest='operation', help='Operation to perform')
-
-        # Subparser for volts operation
-        volts_parser = self.subparsers.add_parser('volts', help='Calculate voltage using Ohm\'s Law')
-        volts_parser.add_argument('-I', type=float, required=True, help='Current in amperes')
-        volts_parser.add_argument('-R', type=float, required=True, help='Resistance in ohms')
-
-        # Subparser for current operation
-        current_parser = self.subparsers.add_parser('current', help='Calculate current using Ohm\'s Law')
-        current_parser.add_argument('-V', type=float, required=True, help='Voltage in volts')
-        current_parser.add_argument('-R', type=float, required=True, help='Resistance in ohms')
-
-        # Subparser for resistance operation
-        resistance_parser = self.subparsers.add_parser('resistance', help='Calculate resistance using Ohm\'s Law')
-        resistance_parser.add_argument('-V', type=float, required=True, help='Voltage in volts')
-        resistance_parser.add_argument('-I', type=float, required=True, help='Current in amperes')
-
-        # Subparser for find_resistor operation
-        find_resistor_parser = self.subparsers.add_parser('find_resistor', help='Calculate resistor value to limit current')
-        find_resistor_parser.add_argument('--source', type=float, required=True, help='Source voltage in volts')
-        find_resistor_parser.add_argument('--component_voltage', type=float, required=True, help='Component voltage in volts')
-        find_resistor_parser.add_argument('--component_current', type=float, default=0.02, help='Component current in amperes (default: 0.02)')
-
-    def main(self):
-        args = self.parser.parse_args()
-        ohms = Ohms()
-
-        if args.operation == 'volts':
-            result = ohms.volts(args.I, args.R)
-        elif args.operation == 'current':
-            result = ohms.current(args.V, args.R)
-        elif args.operation == 'resistance':
-            result = ohms.resistance(args.V, args.I)
-        elif args.operation == 'find_resistor':
-            result = ohms.find_resistor(args.source, args.component_voltage, args.component_current)
+def calculate_volts(I, R):
+    """Calculate voltage using Ohm's Law."""
+    ohms = Ohms()
+    return ohms.volts(I, R)
+
+def calculate_current(V, R):
+    """Calculate current using Ohm's Law."""
+    ohms = Ohms()
+    return ohms.current(V, R)
+
+def calculate_resistance(V, I):
+    """Calculate resistance using Ohm's Law."""
+    ohms = Ohms()
+    return ohms.resistance(V, I)
+
+def find_resistor(source, component_voltage, component_current=0.02):
+    """Calculate resistor value to limit current."""
+    ohms = Ohms()
+    return ohms.find_resistor(source, component_voltage, component_current)
+
+def main():
+    import argparse
+    parser = argparse.ArgumentParser(description="Perform electrical calculations based on Ohm's Law")
+    subparsers = parser.add_subparsers(dest='operation', help='Operation to perform')
+
+    # Subparser for volts operation
+    volts_parser = subparsers.add_parser('volts', help='Calculate voltage using Ohm\'s Law')
+    volts_parser.add_argument('-I', type=float, required=True, help='Current in amperes')
+    volts_parser.add_argument('-R', type=float, required=True, help='Resistance in ohms')
+
+    # Subparser for current operation
+    current_parser = subparsers.add_parser('current', help='Calculate current using Ohm\'s Law')
+    current_parser.add_argument('-V', type=float, required=True, help='Voltage in volts')
+    current_parser.add_argument('-R', type=float, required=True, help='Resistance in ohms')
+
+    # Subparser for resistance operation
+    resistance_parser = subparsers.add_parser('resistance', help='Calculate resistance using Ohm\'s Law')
+    resistance_parser.add_argument('-V', type=float, required=True, help='Voltage in volts')
+    resistance_parser.add_argument('-I', type=float, required=True, help='Current in amperes')
+
+    # Subparser for find_resistor operation
+    find_resistor_parser = subparsers.add_parser('find_resistor', help='Calculate resistor value to limit current')
+    find_resistor_parser.add_argument('--source', type=float, required=True, help='Source voltage in volts')
+    find_resistor_parser.add_argument('--component_voltage', type=float, required=True, help='Component voltage in volts')
+    find_resistor_parser.add_argument('--component_current', type=float, default=0.02, help='Component current in amperes (default: 0.02)')
+
+    args = parser.parse_args()
+
+    if args.operation == 'volts':
+        result = calculate_volts(args.I, args.R)
+    elif args.operation == 'current':
+        result = calculate_current(args.V, args.R)
+    elif args.operation == 'resistance':
+        result = calculate_resistance(args.V, args.I)
+    elif args.operation == 'find_resistor':
+        result = find_resistor(args.source, args.component_voltage, args.component_current)
 
-        print("Result:", result)
+    print("Result:", result)
 
 if __name__ == "__main__":
-    cli = OhmsCLI()
-    cli.main()
+    main()
+
 
 """
     python cli.py volts -I 2 -R 4
     python cli.py current -V 10 -R 5
     python cli.py resistance -V 5 -I 2
     python cli.py find_resistor --source 10 --component_voltage 2
```

### Comparing `ohmslaw-1.0rc5/ohmslaw.egg-info/PKG-INFO` & `ohmslaw-1.0rc6/ohmslaw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmslaw
-Version: 1.0rc5
+Version: 1.0rc6
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
-Metadata-Version: 2.1 Name: ohmslaw Version: 1.0rc5 Summary: python3 library
+Metadata-Version: 2.1 Name: ohmslaw Version: 1.0rc6 Summary: python3 library
 for Ohms law. Author-email: Juan Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/ohmslaw Project-URL: Bug Reports, https://github.com/juanbindez/
 ohmslaw/issues Project-URL: Read the Docs, http://ohmslaw.readthedocs.io/
 Keywords: eletric,ohms,calc,tools Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
```

### Comparing `ohmslaw-1.0rc5/pyproject.toml` & `ohmslaw-1.0rc6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ohmslaw"
-version = "1.0-rc5"
+version = "1.0-rc6"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "python3 library for Ohms law."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

