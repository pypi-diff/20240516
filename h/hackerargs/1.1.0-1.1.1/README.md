# Comparing `tmp/hackerargs-1.1.0.tar.gz` & `tmp/hackerargs-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackerargs-1.1.0.tar", last modified: Tue May 14 20:01:12 2024, max compression
+gzip compressed data, was "hackerargs-1.1.1.tar", last modified: Thu May 16 01:38:18 2024, max compression
```

## Comparing `hackerargs-1.1.0.tar` & `hackerargs-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-14 20:01:12.846654 hackerargs-1.1.0/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1055 2024-05-11 21:31:25.000000 hackerargs-1.1.0/LICENSE
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     4533 2024-05-14 20:01:12.840648 hackerargs-1.1.0/PKG-INFO
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     4205 2024-05-14 19:53:25.000000 hackerargs-1.1.0/README.md
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-14 20:01:12.700977 hackerargs-1.1.0/hackerargs/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       55 2024-05-12 02:54:31.000000 hackerargs-1.1.0/hackerargs/__init__.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      380 2024-05-12 19:36:14.000000 hackerargs-1.1.0/hackerargs/argparse_access.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     9253 2024-05-14 19:08:39.000000 hackerargs-1.1.0/hackerargs/args.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1185 2024-05-12 00:25:18.000000 hackerargs-1.1.0/hackerargs/strict_bool_yaml.py
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-14 20:01:12.833223 hackerargs-1.1.0/hackerargs.egg-info/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     4533 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/PKG-INFO
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      399 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/SOURCES.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        1 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/dependency_links.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        7 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/requires.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       11 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/top_level.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      394 2024-05-14 19:59:34.000000 hackerargs-1.1.0/pyproject.toml
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       38 2024-05-14 20:01:12.847644 hackerargs-1.1.0/setup.cfg
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-14 20:01:12.817928 hackerargs-1.1.0/tests/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      414 2024-05-14 19:08:39.000000 hackerargs-1.1.0/tests/test_access.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      934 2024-05-14 19:08:39.000000 hackerargs-1.1.0/tests/test_argv_string.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      776 2024-05-12 21:02:22.000000 hackerargs-1.1.0/tests/test_positional.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      913 2024-05-12 21:02:25.000000 hackerargs-1.1.0/tests/test_priority.py
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-16 01:38:18.922626 hackerargs-1.1.1/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1062 2024-05-16 01:37:57.000000 hackerargs-1.1.1/LICENSE
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     5185 2024-05-16 01:38:18.906534 hackerargs-1.1.1/PKG-INFO
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     4842 2024-05-15 16:45:20.000000 hackerargs-1.1.1/README.md
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-16 01:38:18.667178 hackerargs-1.1.1/hackerargs/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       55 2024-05-12 02:54:31.000000 hackerargs-1.1.1/hackerargs/__init__.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      380 2024-05-12 19:36:14.000000 hackerargs-1.1.1/hackerargs/argparse_access.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     9246 2024-05-16 01:36:50.000000 hackerargs-1.1.1/hackerargs/args.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1185 2024-05-12 00:25:18.000000 hackerargs-1.1.1/hackerargs/strict_bool_yaml.py
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-16 01:38:18.898534 hackerargs-1.1.1/hackerargs.egg-info/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     5185 2024-05-16 01:38:18.000000 hackerargs-1.1.1/hackerargs.egg-info/PKG-INFO
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      399 2024-05-16 01:38:18.000000 hackerargs-1.1.1/hackerargs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        1 2024-05-16 01:38:18.000000 hackerargs-1.1.1/hackerargs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        7 2024-05-16 01:38:18.000000 hackerargs-1.1.1/hackerargs.egg-info/requires.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       11 2024-05-16 01:38:18.000000 hackerargs-1.1.1/hackerargs.egg-info/top_level.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      409 2024-05-16 01:37:51.000000 hackerargs-1.1.1/pyproject.toml
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       38 2024-05-16 01:38:18.922626 hackerargs-1.1.1/setup.cfg
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-16 01:38:18.874526 hackerargs-1.1.1/tests/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      456 2024-05-16 01:36:50.000000 hackerargs-1.1.1/tests/test_access.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      934 2024-05-14 19:08:39.000000 hackerargs-1.1.1/tests/test_argv_string.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      776 2024-05-12 21:02:22.000000 hackerargs-1.1.1/tests/test_positional.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      913 2024-05-12 21:02:25.000000 hackerargs-1.1.1/tests/test_priority.py
```

### Comparing `hackerargs-1.1.0/LICENSE` & `hackerargs-1.1.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2024 Max Shen
+Copyright 2024 Genentech, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `hackerargs-1.1.0/PKG-INFO` & `hackerargs-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-Metadata-Version: 2.1
-Name: hackerargs
-Version: 1.1.0
-Summary: Simple config and argument system
-Author: Max Shen
-Project-URL: Homepage, https://github.com/maxwshen/hackerargs
-Project-URL: Issues, https://github.com/maxwshen/hackerargs/issues
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PyYAML
-
 # hackerargs
 
 ![Python package testing badge](https://github.com/maxwshen/hackerargs/actions/workflows/python-package.yml/badge.svg)
 ![Supports python 3.9-3.12](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 
 
 **hackerargs** minimizes new lines of code to add a configurable argument anywhere in your codebase, so you can focus on coding.
 
+Hackerargs is for everyone, but is especially designed for researchers using config-heavy ML libraries like pytorch, coding largely from scratch in solo or small-team repos, and running experiments varying CLI args with wandb.
+
 ```python
 # in any python file in your codebase
 from hackerargs import args
 
 class Model:
     def __init__(self):
         self.parameter = args.setdefault(key, default_value)
         # run forth and code with confidence!
-        # value can be taken from CLI or yaml config if provided
+        # value is taken from CLI or yaml config if given
 ```
 
-- Hackerargs is a global, write-once-only dict. The first setting of each key is final, ensuring exact reproducibility when saving to yaml, and later loading it to rerun your script.
-- We emphasize `val = setdefault(key, default_val)` as a primitive, which returns your key's value if it already exists, and setting it to default_val otherwise. No more fumbling with errors accessing missing keys. Initializing args from CLI or yaml config takes priority over runtime setdefault.
+- In hackerargs, `args` is a global, write-once-only dict
+- We emphasize `val = args.setdefault(key, default_val)` as a primitive. It returns your key's value if it already exists, and also sets it to default_val if missing. No more fumbling with errors accessing missing keys. Write-once only means initialized args from CLI or yaml config are used at runtime, and exact reproducibility on reruns by reloading saved yaml config
+- Write cleaner code, simplify function parameters, and operate at a higher level of abstraction: no more passing args around, or long function signatures filled with low-level details
 
 Features
-- Values have python types inferred as floats, ints, strings, lists, etc. with PyYAML loader. YAML v1.1 except "on/off/yes/no" are not parsed as booleans
+- Type inference as floats, ints, strings, lists, etc. with PyYAML loader (YAML v1.1), except "on/off/yes/no" are not parsed as booleans
 - Optional integration with argparse
-- Works with wandb sweeps: log config using `wandb.config.update(args)`, and run sweep experiments in CLI `--{key} {val}` format.
+- Works with wandb sweeps: log config using `wandb.config.update(args)`, and run sweep experiments in CLI `--{key} {val}` format
 
 # Installation
 
 Hackerargs is a pip package and conda package:
 
 ```bash
 pip install hackerargs
@@ -59,30 +51,37 @@
 
 if __name__ == '__main__':
     args.parse_args()
     main()
     args.save_to_yaml(yaml_file)
 ```
 
-parse_args can be called by itself, or with a YAML config file, or argparse.ArgumentParser:
+parse_args can be called with no arguments:
+
+- `args.parse_args()`: Parse CLI options in `--{key} {val}` format. Then, if `--config {yaml_file}` provided, load from yaml file.
+
+parse_args can also take either a YAML config file, or argparse.ArgumentParser.
 
-- `args.parse_args()`
 - `args.parse_args('config.yaml')`
 - `args.parse_args(argparse.ArgumentParser())`
-- `args.parse_args(argparse.ArgumentParser(), 'config.yaml')`: The input order doesn't matter. 
+- `args.parse_args(argparse.ArgumentParser(), 'config.yaml')`
+- `args.parse_args('config.yaml', argparse.ArgumentParser())`
 
 parse_args parses `sys.argv` by default, but you can use a custom argv instead:
 - `args.parse_args(..., argv = ['--string', 'text', '--int', '42'])`
 
 
 ### Priority
-1. (Highest priority) ArgumentParser options specified by user
-2. Unknown CLI options (not recognized by ArgumentParser) specified by user. These are parsed in `--{key} {val}` format. If no argparser is given, then all CLI options are parsed this way.
-3. YAML config. If `--config {yaml_file}` CLI option is given, it is used instead of a yaml file given as input to parse_args() in python. As such, `--config` is a protected CLI option when using hackerargs.
-4. (Lowest priority) ArgumentParser default values for options not specified by user.
+
+In general, CLI options > yaml config (if provided).
+
+1. (Highest priority) ArgumentParser options specified by user via CLI, if ArgumentParser is given
+2. Unknown CLI options (not recognized by ArgumentParser) specified by user. These are parsed in `--{key} {val}` format. If no ArgumentParser is given, then all CLI options are parsed this way
+3. YAML config. If `--config {yaml_file}` CLI option is given, it is used instead of a yaml file given as input to parse_args() in python. As such, `--config` is a protected CLI option when using hackerargs
+4. (Lowest priority) ArgumentParser default values for options not specified by user via CLI, if ArgumentParser is given
 
 As a write-once-only dict, initialized values take priority over runtime values.
 
 
 ### Access
 
 Running `python train.py --string text --int 42 --float 3.14 --list [1,2]`, we have:
```

### Comparing `hackerargs-1.1.0/README.md` & `hackerargs-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,47 @@
+Metadata-Version: 2.1
+Name: hackerargs
+Version: 1.1.1
+Summary: Easy config system, minimizing new lines of code
+Author: Max Shen
+Project-URL: Homepage, https://github.com/maxwshen/hackerargs
+Project-URL: Issues, https://github.com/maxwshen/hackerargs/issues
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: PyYAML
+
 # hackerargs
 
 ![Python package testing badge](https://github.com/maxwshen/hackerargs/actions/workflows/python-package.yml/badge.svg)
 ![Supports python 3.9-3.12](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 
 
 **hackerargs** minimizes new lines of code to add a configurable argument anywhere in your codebase, so you can focus on coding.
 
+Hackerargs is for everyone, but is especially designed for researchers using config-heavy ML libraries like pytorch, coding largely from scratch in solo or small-team repos, and running experiments varying CLI args with wandb.
+
 ```python
 # in any python file in your codebase
 from hackerargs import args
 
 class Model:
     def __init__(self):
         self.parameter = args.setdefault(key, default_value)
         # run forth and code with confidence!
-        # value can be taken from CLI or yaml config if provided
+        # value is taken from CLI or yaml config if given
 ```
 
-- Hackerargs is a global, write-once-only dict. The first setting of each key is final, ensuring exact reproducibility when saving to yaml, and later loading it to rerun your script.
-- We emphasize `val = setdefault(key, default_val)` as a primitive, which returns your key's value if it already exists, and setting it to default_val otherwise. No more fumbling with errors accessing missing keys. Initializing args from CLI or yaml config takes priority over runtime setdefault.
+- In hackerargs, `args` is a global, write-once-only dict
+- We emphasize `val = args.setdefault(key, default_val)` as a primitive. It returns your key's value if it already exists, and also sets it to default_val if missing. No more fumbling with errors accessing missing keys. Write-once only means initialized args from CLI or yaml config are used at runtime, and exact reproducibility on reruns by reloading saved yaml config
+- Write cleaner code, simplify function parameters, and operate at a higher level of abstraction: no more passing args around, or long function signatures filled with low-level details
 
 Features
-- Values have python types inferred as floats, ints, strings, lists, etc. with PyYAML loader. YAML v1.1 except "on/off/yes/no" are not parsed as booleans
+- Type inference as floats, ints, strings, lists, etc. with PyYAML loader (YAML v1.1), except "on/off/yes/no" are not parsed as booleans
 - Optional integration with argparse
-- Works with wandb sweeps: log config using `wandb.config.update(args)`, and run sweep experiments in CLI `--{key} {val}` format.
+- Works with wandb sweeps: log config using `wandb.config.update(args)`, and run sweep experiments in CLI `--{key} {val}` format
 
 # Installation
 
 Hackerargs is a pip package and conda package:
 
 ```bash
 pip install hackerargs
@@ -48,30 +62,37 @@
 
 if __name__ == '__main__':
     args.parse_args()
     main()
     args.save_to_yaml(yaml_file)
 ```
 
-parse_args can be called by itself, or with a YAML config file, or argparse.ArgumentParser:
+parse_args can be called with no arguments:
+
+- `args.parse_args()`: Parse CLI options in `--{key} {val}` format. Then, if `--config {yaml_file}` provided, load from yaml file.
+
+parse_args can also take either a YAML config file, or argparse.ArgumentParser.
 
-- `args.parse_args()`
 - `args.parse_args('config.yaml')`
 - `args.parse_args(argparse.ArgumentParser())`
-- `args.parse_args(argparse.ArgumentParser(), 'config.yaml')`: The input order doesn't matter. 
+- `args.parse_args(argparse.ArgumentParser(), 'config.yaml')`
+- `args.parse_args('config.yaml', argparse.ArgumentParser())`
 
 parse_args parses `sys.argv` by default, but you can use a custom argv instead:
 - `args.parse_args(..., argv = ['--string', 'text', '--int', '42'])`
 
 
 ### Priority
-1. (Highest priority) ArgumentParser options specified by user
-2. Unknown CLI options (not recognized by ArgumentParser) specified by user. These are parsed in `--{key} {val}` format. If no argparser is given, then all CLI options are parsed this way.
-3. YAML config. If `--config {yaml_file}` CLI option is given, it is used instead of a yaml file given as input to parse_args() in python. As such, `--config` is a protected CLI option when using hackerargs.
-4. (Lowest priority) ArgumentParser default values for options not specified by user.
+
+In general, CLI options > yaml config (if provided).
+
+1. (Highest priority) ArgumentParser options specified by user via CLI, if ArgumentParser is given
+2. Unknown CLI options (not recognized by ArgumentParser) specified by user. These are parsed in `--{key} {val}` format. If no ArgumentParser is given, then all CLI options are parsed this way
+3. YAML config. If `--config {yaml_file}` CLI option is given, it is used instead of a yaml file given as input to parse_args() in python. As such, `--config` is a protected CLI option when using hackerargs
+4. (Lowest priority) ArgumentParser default values for options not specified by user via CLI, if ArgumentParser is given
 
 As a write-once-only dict, initialized values take priority over runtime values.
 
 
 ### Access
 
 Running `python train.py --string text --int 42 --float 3.14 --list [1,2]`, we have:
```

### Comparing `hackerargs-1.1.0/hackerargs/args.py` & `hackerargs-1.1.1/hackerargs/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,11 +243,11 @@
             Create parent folders recursively if needed.
         """
         Path(os.path.dirname(out_yaml_file)).mkdir(
             parents = True, 
             exist_ok = True
         )
         with open(out_yaml_file, 'w') as f:
-            yaml.dump(self._privatedict, f)
+            yaml.dump(dict(self), f)
         logger.info(f'Saved hackerargs to {out_yaml_file}.')
         return
```

### Comparing `hackerargs-1.1.0/hackerargs/strict_bool_yaml.py` & `hackerargs-1.1.1/hackerargs/strict_bool_yaml.py`

 * *Files identical despite different names*

### Comparing `hackerargs-1.1.0/hackerargs.egg-info/PKG-INFO` & `hackerargs-1.1.1/hackerargs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hackerargs
-Version: 1.1.0
-Summary: Simple config and argument system
+Version: 1.1.1
+Summary: Easy config system, minimizing new lines of code
 Author: Max Shen
 Project-URL: Homepage, https://github.com/maxwshen/hackerargs
 Project-URL: Issues, https://github.com/maxwshen/hackerargs/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML
 
@@ -13,32 +13,35 @@
 
 ![Python package testing badge](https://github.com/maxwshen/hackerargs/actions/workflows/python-package.yml/badge.svg)
 ![Supports python 3.9-3.12](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 
 
 **hackerargs** minimizes new lines of code to add a configurable argument anywhere in your codebase, so you can focus on coding.
 
+Hackerargs is for everyone, but is especially designed for researchers using config-heavy ML libraries like pytorch, coding largely from scratch in solo or small-team repos, and running experiments varying CLI args with wandb.
+
 ```python
 # in any python file in your codebase
 from hackerargs import args
 
 class Model:
     def __init__(self):
         self.parameter = args.setdefault(key, default_value)
         # run forth and code with confidence!
-        # value can be taken from CLI or yaml config if provided
+        # value is taken from CLI or yaml config if given
 ```
 
-- Hackerargs is a global, write-once-only dict. The first setting of each key is final, ensuring exact reproducibility when saving to yaml, and later loading it to rerun your script.
-- We emphasize `val = setdefault(key, default_val)` as a primitive, which returns your key's value if it already exists, and setting it to default_val otherwise. No more fumbling with errors accessing missing keys. Initializing args from CLI or yaml config takes priority over runtime setdefault.
+- In hackerargs, `args` is a global, write-once-only dict
+- We emphasize `val = args.setdefault(key, default_val)` as a primitive. It returns your key's value if it already exists, and also sets it to default_val if missing. No more fumbling with errors accessing missing keys. Write-once only means initialized args from CLI or yaml config are used at runtime, and exact reproducibility on reruns by reloading saved yaml config
+- Write cleaner code, simplify function parameters, and operate at a higher level of abstraction: no more passing args around, or long function signatures filled with low-level details
 
 Features
-- Values have python types inferred as floats, ints, strings, lists, etc. with PyYAML loader. YAML v1.1 except "on/off/yes/no" are not parsed as booleans
+- Type inference as floats, ints, strings, lists, etc. with PyYAML loader (YAML v1.1), except "on/off/yes/no" are not parsed as booleans
 - Optional integration with argparse
-- Works with wandb sweeps: log config using `wandb.config.update(args)`, and run sweep experiments in CLI `--{key} {val}` format.
+- Works with wandb sweeps: log config using `wandb.config.update(args)`, and run sweep experiments in CLI `--{key} {val}` format
 
 # Installation
 
 Hackerargs is a pip package and conda package:
 
 ```bash
 pip install hackerargs
@@ -59,30 +62,37 @@
 
 if __name__ == '__main__':
     args.parse_args()
     main()
     args.save_to_yaml(yaml_file)
 ```
 
-parse_args can be called by itself, or with a YAML config file, or argparse.ArgumentParser:
+parse_args can be called with no arguments:
+
+- `args.parse_args()`: Parse CLI options in `--{key} {val}` format. Then, if `--config {yaml_file}` provided, load from yaml file.
+
+parse_args can also take either a YAML config file, or argparse.ArgumentParser.
 
-- `args.parse_args()`
 - `args.parse_args('config.yaml')`
 - `args.parse_args(argparse.ArgumentParser())`
-- `args.parse_args(argparse.ArgumentParser(), 'config.yaml')`: The input order doesn't matter. 
+- `args.parse_args(argparse.ArgumentParser(), 'config.yaml')`
+- `args.parse_args('config.yaml', argparse.ArgumentParser())`
 
 parse_args parses `sys.argv` by default, but you can use a custom argv instead:
 - `args.parse_args(..., argv = ['--string', 'text', '--int', '42'])`
 
 
 ### Priority
-1. (Highest priority) ArgumentParser options specified by user
-2. Unknown CLI options (not recognized by ArgumentParser) specified by user. These are parsed in `--{key} {val}` format. If no argparser is given, then all CLI options are parsed this way.
-3. YAML config. If `--config {yaml_file}` CLI option is given, it is used instead of a yaml file given as input to parse_args() in python. As such, `--config` is a protected CLI option when using hackerargs.
-4. (Lowest priority) ArgumentParser default values for options not specified by user.
+
+In general, CLI options > yaml config (if provided).
+
+1. (Highest priority) ArgumentParser options specified by user via CLI, if ArgumentParser is given
+2. Unknown CLI options (not recognized by ArgumentParser) specified by user. These are parsed in `--{key} {val}` format. If no ArgumentParser is given, then all CLI options are parsed this way
+3. YAML config. If `--config {yaml_file}` CLI option is given, it is used instead of a yaml file given as input to parse_args() in python. As such, `--config` is a protected CLI option when using hackerargs
+4. (Lowest priority) ArgumentParser default values for options not specified by user via CLI, if ArgumentParser is given
 
 As a write-once-only dict, initialized values take priority over runtime values.
 
 
 ### Access
 
 Running `python train.py --string text --int 42 --float 3.14 --list [1,2]`, we have:
```

### Comparing `hackerargs-1.1.0/tests/test_argv_string.py` & `hackerargs-1.1.1/tests/test_argv_string.py`

 * *Files identical despite different names*

### Comparing `hackerargs-1.1.0/tests/test_positional.py` & `hackerargs-1.1.1/tests/test_positional.py`

 * *Files identical despite different names*

### Comparing `hackerargs-1.1.0/tests/test_priority.py` & `hackerargs-1.1.1/tests/test_priority.py`

 * *Files identical despite different names*

