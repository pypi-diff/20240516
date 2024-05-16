# Comparing `tmp/argument_parsing-1.0.0.tar.gz` & `tmp/argument_parsing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argument_parsing-1.0.0.tar", last modified: Tue May 14 11:05:42 2024, max compression
+gzip compressed data, was "argument_parsing-1.0.1.tar", last modified: Thu May 16 09:22:33 2024, max compression
```

## Comparing `argument_parsing-1.0.0.tar` & `argument_parsing-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:05:42.773355 argument_parsing-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 11:05:37.000000 argument_parsing-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-14 11:05:42.773355 argument_parsing-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-05-14 11:05:37.000000 argument_parsing-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:05:42.769355 argument_parsing-1.0.0/argument_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-05-14 11:05:37.000000 argument_parsing-1.0.0/argument_parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:05:42.773355 argument_parsing-1.0.0/argument_parsing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-14 11:05:42.000000 argument_parsing-1.0.0/argument_parsing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 11:05:42.000000 argument_parsing-1.0.0/argument_parsing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:05:42.000000 argument_parsing-1.0.0/argument_parsing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:05:42.000000 argument_parsing-1.0.0/argument_parsing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 11:05:42.000000 argument_parsing-1.0.0/argument_parsing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:05:42.773355 argument_parsing-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-14 11:05:37.000000 argument_parsing-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:22:33.685652 argument_parsing-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-16 09:22:29.000000 argument_parsing-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-05-16 09:22:33.685652 argument_parsing-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-16 09:22:29.000000 argument_parsing-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:22:33.685652 argument_parsing-1.0.1/argument_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-16 09:22:29.000000 argument_parsing-1.0.1/argument_parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:22:33.685652 argument_parsing-1.0.1/argument_parsing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-05-16 09:22:33.000000 argument_parsing-1.0.1/argument_parsing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-16 09:22:33.000000 argument_parsing-1.0.1/argument_parsing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:22:33.000000 argument_parsing-1.0.1/argument_parsing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:22:33.000000 argument_parsing-1.0.1/argument_parsing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 09:22:33.000000 argument_parsing-1.0.1/argument_parsing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:22:33.685652 argument_parsing-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-16 09:22:29.000000 argument_parsing-1.0.1/setup.py
```

### Comparing `argument_parsing-1.0.0/LICENSE` & `argument_parsing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argument_parsing-1.0.0/PKG-INFO` & `argument_parsing-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,19 @@
-Metadata-Version: 2.1
-Name: argument_parsing
-Version: 1.0.0
-Summary: A zero dependency argument parser written in python.
-Home-page: https://github.com/flpeters/argument_parsing
-Download-URL: https://github.com/flpeters/argument_parsing
-Author: Florian Peters
-License: GNU General Public License v2 (GPLv2)
-Project-URL: Source Code, https://github.com/flpeters/argument_parsing
-Project-URL: Documentation, https://github.com/flpeters/argument_parsing
-Project-URL: Bug Tracker, https://github.com/flpeters/argument_parsing/issues
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[![PyPI Version](https://img.shields.io/pypi/v/argument-parsing?label=PyPI%20Version)](https://pypi.org/project/argument-parsing/)  
 
 # Introduction
 A zero dependency, single file string argument parser written in python.  
 You can define commands by creating simple python dictionaries, parse strings for the defined fields, and receive a structured result. The argument parser handles some basic python types, typecasting, missing values, default values, nested lists and tuples, error reporting, and any combination of the above.
 
 # Installation
-Currently the easiest way to use this module is to do a local pip install.
+This package is available on [PyPI](https://pypi.org/project/argument-parsing/):
+```console
+pip install argument-parsing
+```
+Another way to install this module is to do a local pip install.
 ```console
 git clone git@github.com:flpeters/argument_parsing.git
 cd argument_parsing
 pip install -e .
 ```
 
 # Documentation
@@ -119,15 +98,15 @@
 ```
 ```python
 arguments = '-weather -cloudy'
 ...
 result    = {'weather': '-cloudy'}
 is_set    = {'weather': True}
 ```
-When a default value is set, the keyword becomes optional. Should the keyword not be part of the `arguments`, then the default value will be placed in the `results` instead.
+When a default value is set, the keyword becomes optional. Should the keyword not be part of the `arguments`, then the default value will be placed in the results instead.
 ```python
 command   = {'weather': 'cloudy'}
 arguments = ''
 ...
 result    = {'weather': 'cloudy'}
 is_set    = {'weather': False}
 ```
@@ -173,15 +152,15 @@
 arguments = '-meters -15'
 ...
 result    = {'meters': -15}
 ```
 ```python
 arguments = '-meters +15.0'
 ...
-result    = {'meters': 15.0}
+result    = {'meters': 15}
 ```
 ```python
 arguments = '-meters 15.4'
 ...
 result    = {'meters': 15}
 # This will result in a warning that the remainder of 0.4 has been cut off.
 ```
@@ -223,37 +202,55 @@
 ...
 result    = {'celsius': nan}
 is_set    = {'celsius': False}
 ```
 
 ---
 
-A __composite type__ is a `list` or `tuple` of one or more values of potentially multiple datatypes. Since `list` or `tuple` have the same semantics and can be used interchangeably, they will be referred to as 'array' for the purpose of this documentation.  
+A __composite type__ is a `list` or `tuple` containing one or more values of potentially multiple datatypes. Since `list` or `tuple` have the same semantics and can be used interchangeably, they will be referred to as 'array' for the purpose of this documentation.  
 
 The following __composite types__ are supported:  
 
 #### un-bounded array
-Specifying only the type `list` or `tuple`, will result in an 'unbounded array' of that type, meaning that all values following the keyword will be added to the array, until either the end of the `arguments` string is reached, or a value starts with a hyphen-minus (`'-'`), which denotes the start of the next argument. All values of this unbounded array will be of type `str`. This kind of argument should be used with caution because, for instance, negative values will be treated as the start of a new argument due to them starting with a hyphen-minus sign.  
+Specifying only the type `list` or `tuple`, will result in an 'unbounded array' of that type, meaning that all values following the keyword will be added to the array, until either the end of the `arguments` string is reached, or a value starts with a hyphen-minus (`'-'`), which denotes the start of the next argument. All values of this unbounded array will be of type `str`. This kind of argument should be used with caution because, for instance, negative numbers will be treated as the start of a new argument due to them starting with a hyphen-minus sign.  
 ```python
-{
+command = {
     'unbounded_list' : list,
     'unbounded_tuple': tuple,
 }
+arguments = '-unbounded_list 1 2 3 4 5 a b c -unbounded_tuple 1.0 + 1.0 = 2.0'
+...
+result = {'unbounded_list' : ['1', '2', '3', '4', '5', 'a', 'b', 'c'],
+          'unbounded_tuple': ('1.0', '+', '1.0', '=', '2.0')}
+is_set = {'unbounded_list': True, 'unbounded_tuple': True}
 ```  
 
 #### fixed array
-By specifying an array containing the types, default values, and ordering you want the values to have, you can define a fixed array. Their construction can get arbitrarily complex, mixing and matching any supported primitive type and fixed arrays you want. The only thing not allowed, is using an unbounded array inside a fixed array. All values will be cast to the corresponding type using all the same semantics as if they were single values (see above).  
-The only exception to that is the `bool` type. Since the value can't be decided based on presence of absence, a value has to be given. The value has to be either `'True'`, `'False'`, or interpretable as a `float`, which will then be cast to a `bool`. This means that e.g. `'0.0'` will result in `False`, and `'123'` will result in `'True'` (careful, check the [casting rules](https://docs.python.org/3.3/library/stdtypes.html?highlight=frozenset#truth-value-testing) first).
+By specifying an array containing the types, default values, and ordering you want the values to have, you can define a fixed array. Their construction can get arbitrarily complex, mixing and matching any supported primitive type and fixed arrays you want. The only thing not allowed, is using an unbounded array inside a fixed array. All values will be cast to the corresponding type using all the same semantics as if they were single values (see above).   
+Please note that while default values can be used to define the array, you currently need to specify all of the values, even if the array has default values at the end and they could technically be omitted. Default values in the middle of the array also currently don't have a mechanism for not setting them. This also means that since the value of a `bool` type can't be decided based on presence or absence, a value has to be given. We recognize a value of either `'True'`, `'False'`, or one interpretable as a `float`, which will then be cast to a `bool`. This means that e.g. `'0.0'` will result in `False`, and `'123'` will result in `'True'` (careful, check the [casting rules](https://docs.python.org/3.3/library/stdtypes.html?highlight=frozenset#truth-value-testing) first). 
 ```python
-{
+command = {
     'arg1': [int]*5,
     'arg2': (3.14, 'pi', bool),
     'arg3': (bool, str, 123)*2,
     'arg4': [[0]*3, [1]*3, [str]*3],
     'arg5': [str, int, bool, True, [1, '2', 3, bool], (2.1, float)]
 }
+arguments = '-arg1 4 5 6 7 8 \
+             -arg2 6.28 tau True \
+             -arg3 False helloworld 123 True HelloWorld 321 \
+             -arg4 0 0 0 1 1 1 2 2 2 \
+             -arg5 1 1 1 1 1 1 1 1 1 1'
+...
+result = {
+    'arg1': [4, 5, 6, 7, 8],
+    'arg2': (6.28, 'tau', True),
+    'arg3': (False, 'helloworld', 123, True, 'HelloWorld', 321),
+    'arg4': [[0, 0, 0], [1, 1, 1], ['2', '2', '2']],
+    'arg5': ['1', 1, True, True, [1, '1', 1, True], (1.0, 1.0)]}
+is_set = {'arg1': True, 'arg2': True, 'arg3': True, 'arg4': True, 'arg5': True}
 ```
 
 # Attribution
 This argument parser is largely inspired by and based upon, but in no way affiliated with, the work by [Jonathan Blow](https://www.youtube.com/@jblow888) as seen in these two videos on his youtube channel.
 > [Jonathan Blow - Livestream: Metaprogramming Use Case: Command-Line Argument Parsing - Part 1](https://youtu.be/TwqXTf7VfZk)  
-> [Jonathan Blow - Livestream: Metaprogramming Use Case: Command-Line Argument Parsing - Part 2](https://youtu.be/pgiVrhsGkKY)
+> [Jonathan Blow - Livestream: Metaprogramming Use Case: Command-Line Argument Parsing - Part 2](https://youtu.be/pgiVrhsGkKY)
```

### Comparing `argument_parsing-1.0.0/README.md` & `argument_parsing-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,46 @@
+Metadata-Version: 2.1
+Name: argument_parsing
+Version: 1.0.1
+Summary: A zero dependency argument parser written in python.
+Home-page: https://github.com/flpeters/argument_parsing
+Download-URL: https://github.com/flpeters/argument_parsing
+Author: Florian Peters
+License: GNU General Public License v2 (GPLv2)
+Project-URL: Source Code, https://github.com/flpeters/argument_parsing
+Project-URL: Documentation, https://github.com/flpeters/argument_parsing
+Project-URL: Bug Tracker, https://github.com/flpeters/argument_parsing/issues
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI Version](https://img.shields.io/pypi/v/argument-parsing?label=PyPI%20Version)](https://pypi.org/project/argument-parsing/)  
+
 # Introduction
 A zero dependency, single file string argument parser written in python.  
 You can define commands by creating simple python dictionaries, parse strings for the defined fields, and receive a structured result. The argument parser handles some basic python types, typecasting, missing values, default values, nested lists and tuples, error reporting, and any combination of the above.
 
 # Installation
-Currently the easiest way to use this module is to do a local pip install.
+This package is available on [PyPI](https://pypi.org/project/argument-parsing/):
+```console
+pip install argument-parsing
+```
+Another way to install this module is to do a local pip install.
 ```console
 git clone git@github.com:flpeters/argument_parsing.git
 cd argument_parsing
 pip install -e .
 ```
 
 # Documentation
@@ -92,15 +125,15 @@
 ```
 ```python
 arguments = '-weather -cloudy'
 ...
 result    = {'weather': '-cloudy'}
 is_set    = {'weather': True}
 ```
-When a default value is set, the keyword becomes optional. Should the keyword not be part of the `arguments`, then the default value will be placed in the `results` instead.
+When a default value is set, the keyword becomes optional. Should the keyword not be part of the `arguments`, then the default value will be placed in the results instead.
 ```python
 command   = {'weather': 'cloudy'}
 arguments = ''
 ...
 result    = {'weather': 'cloudy'}
 is_set    = {'weather': False}
 ```
@@ -146,15 +179,15 @@
 arguments = '-meters -15'
 ...
 result    = {'meters': -15}
 ```
 ```python
 arguments = '-meters +15.0'
 ...
-result    = {'meters': 15.0}
+result    = {'meters': 15}
 ```
 ```python
 arguments = '-meters 15.4'
 ...
 result    = {'meters': 15}
 # This will result in a warning that the remainder of 0.4 has been cut off.
 ```
@@ -196,37 +229,55 @@
 ...
 result    = {'celsius': nan}
 is_set    = {'celsius': False}
 ```
 
 ---
 
-A __composite type__ is a `list` or `tuple` of one or more values of potentially multiple datatypes. Since `list` or `tuple` have the same semantics and can be used interchangeably, they will be referred to as 'array' for the purpose of this documentation.  
+A __composite type__ is a `list` or `tuple` containing one or more values of potentially multiple datatypes. Since `list` or `tuple` have the same semantics and can be used interchangeably, they will be referred to as 'array' for the purpose of this documentation.  
 
 The following __composite types__ are supported:  
 
 #### un-bounded array
-Specifying only the type `list` or `tuple`, will result in an 'unbounded array' of that type, meaning that all values following the keyword will be added to the array, until either the end of the `arguments` string is reached, or a value starts with a hyphen-minus (`'-'`), which denotes the start of the next argument. All values of this unbounded array will be of type `str`. This kind of argument should be used with caution because, for instance, negative values will be treated as the start of a new argument due to them starting with a hyphen-minus sign.  
+Specifying only the type `list` or `tuple`, will result in an 'unbounded array' of that type, meaning that all values following the keyword will be added to the array, until either the end of the `arguments` string is reached, or a value starts with a hyphen-minus (`'-'`), which denotes the start of the next argument. All values of this unbounded array will be of type `str`. This kind of argument should be used with caution because, for instance, negative numbers will be treated as the start of a new argument due to them starting with a hyphen-minus sign.  
 ```python
-{
+command = {
     'unbounded_list' : list,
     'unbounded_tuple': tuple,
 }
+arguments = '-unbounded_list 1 2 3 4 5 a b c -unbounded_tuple 1.0 + 1.0 = 2.0'
+...
+result = {'unbounded_list' : ['1', '2', '3', '4', '5', 'a', 'b', 'c'],
+          'unbounded_tuple': ('1.0', '+', '1.0', '=', '2.0')}
+is_set = {'unbounded_list': True, 'unbounded_tuple': True}
 ```  
 
 #### fixed array
-By specifying an array containing the types, default values, and ordering you want the values to have, you can define a fixed array. Their construction can get arbitrarily complex, mixing and matching any supported primitive type and fixed arrays you want. The only thing not allowed, is using an unbounded array inside a fixed array. All values will be cast to the corresponding type using all the same semantics as if they were single values (see above).  
-The only exception to that is the `bool` type. Since the value can't be decided based on presence of absence, a value has to be given. The value has to be either `'True'`, `'False'`, or interpretable as a `float`, which will then be cast to a `bool`. This means that e.g. `'0.0'` will result in `False`, and `'123'` will result in `'True'` (careful, check the [casting rules](https://docs.python.org/3.3/library/stdtypes.html?highlight=frozenset#truth-value-testing) first).
+By specifying an array containing the types, default values, and ordering you want the values to have, you can define a fixed array. Their construction can get arbitrarily complex, mixing and matching any supported primitive type and fixed arrays you want. The only thing not allowed, is using an unbounded array inside a fixed array. All values will be cast to the corresponding type using all the same semantics as if they were single values (see above).   
+Please note that while default values can be used to define the array, you currently need to specify all of the values, even if the array has default values at the end and they could technically be omitted. Default values in the middle of the array also currently don't have a mechanism for not setting them. This also means that since the value of a `bool` type can't be decided based on presence or absence, a value has to be given. We recognize a value of either `'True'`, `'False'`, or one interpretable as a `float`, which will then be cast to a `bool`. This means that e.g. `'0.0'` will result in `False`, and `'123'` will result in `'True'` (careful, check the [casting rules](https://docs.python.org/3.3/library/stdtypes.html?highlight=frozenset#truth-value-testing) first). 
 ```python
-{
+command = {
     'arg1': [int]*5,
     'arg2': (3.14, 'pi', bool),
     'arg3': (bool, str, 123)*2,
     'arg4': [[0]*3, [1]*3, [str]*3],
     'arg5': [str, int, bool, True, [1, '2', 3, bool], (2.1, float)]
 }
+arguments = '-arg1 4 5 6 7 8 \
+             -arg2 6.28 tau True \
+             -arg3 False helloworld 123 True HelloWorld 321 \
+             -arg4 0 0 0 1 1 1 2 2 2 \
+             -arg5 1 1 1 1 1 1 1 1 1 1'
+...
+result = {
+    'arg1': [4, 5, 6, 7, 8],
+    'arg2': (6.28, 'tau', True),
+    'arg3': (False, 'helloworld', 123, True, 'HelloWorld', 321),
+    'arg4': [[0, 0, 0], [1, 1, 1], ['2', '2', '2']],
+    'arg5': ['1', 1, True, True, [1, '1', 1, True], (1.0, 1.0)]}
+is_set = {'arg1': True, 'arg2': True, 'arg3': True, 'arg4': True, 'arg5': True}
 ```
 
 # Attribution
 This argument parser is largely inspired by and based upon, but in no way affiliated with, the work by [Jonathan Blow](https://www.youtube.com/@jblow888) as seen in these two videos on his youtube channel.
 > [Jonathan Blow - Livestream: Metaprogramming Use Case: Command-Line Argument Parsing - Part 1](https://youtu.be/TwqXTf7VfZk)  
-> [Jonathan Blow - Livestream: Metaprogramming Use Case: Command-Line Argument Parsing - Part 2](https://youtu.be/pgiVrhsGkKY)
+> [Jonathan Blow - Livestream: Metaprogramming Use Case: Command-Line Argument Parsing - Part 2](https://youtu.be/pgiVrhsGkKY)
```

### Comparing `argument_parsing-1.0.0/argument_parsing/__init__.py` & `argument_parsing-1.0.1/argument_parsing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 __all__ = ['parse_arguments', 'set_report_options']
 
 
 #######################################
 #               LOGGING               #
 #######################################
@@ -200,21 +200,24 @@
 
     elif arg_type == list or arg_type == tuple:
         if arg_default is None: # unbounded list / tuple
             if state['inside_array']:
                 report_error(SyntaxError(f"Using an unbounded list or tuple inside an array is not supported."))
                 return False
             array_success, state['cursor'], value = to_unbounded_array(args, state['cursor'])
-            if array_success: # NOTE: currently this can't actually fail... don't use unbounded lists kids.
+            if array_success: # NOTE: currently this can't actually fail...
                 result[arg_name] = arg_type(value)
             else: success = False
             
         else: # predefined list
             s = {'args': args, 'name': 'v', 'cursor': state['cursor'], 'inside_array': True}
             value = []
+            # TODO: we need to handle default values here as well. if the last keywords for this array all already have values,
+            #       then it's fine if they are missing.
+            #       When this is fixed, also change the documentation.
             for i, x in enumerate(arg_default):
                 t, d = typify(x)
                 n = f'{arg_name}[{i}]'
                 s['name'] = n
                 r = {n:d}
                 member_success = handle_one_argument(r, s, t, d)
                 if member_success: value.append(r[n])
```

### Comparing `argument_parsing-1.0.0/argument_parsing.egg-info/PKG-INFO` & `argument_parsing-1.0.1/argument_parsing.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argument_parsing
-Version: 1.0.0
+Version: 1.0.1
 Summary: A zero dependency argument parser written in python.
 Home-page: https://github.com/flpeters/argument_parsing
 Download-URL: https://github.com/flpeters/argument_parsing
 Author: Florian Peters
 License: GNU General Public License v2 (GPLv2)
 Project-URL: Source Code, https://github.com/flpeters/argument_parsing
 Project-URL: Documentation, https://github.com/flpeters/argument_parsing
@@ -21,20 +21,26 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI Version](https://img.shields.io/pypi/v/argument-parsing?label=PyPI%20Version)](https://pypi.org/project/argument-parsing/)  
+
 # Introduction
 A zero dependency, single file string argument parser written in python.  
 You can define commands by creating simple python dictionaries, parse strings for the defined fields, and receive a structured result. The argument parser handles some basic python types, typecasting, missing values, default values, nested lists and tuples, error reporting, and any combination of the above.
 
 # Installation
-Currently the easiest way to use this module is to do a local pip install.
+This package is available on [PyPI](https://pypi.org/project/argument-parsing/):
+```console
+pip install argument-parsing
+```
+Another way to install this module is to do a local pip install.
 ```console
 git clone git@github.com:flpeters/argument_parsing.git
 cd argument_parsing
 pip install -e .
 ```
 
 # Documentation
@@ -119,15 +125,15 @@
 ```
 ```python
 arguments = '-weather -cloudy'
 ...
 result    = {'weather': '-cloudy'}
 is_set    = {'weather': True}
 ```
-When a default value is set, the keyword becomes optional. Should the keyword not be part of the `arguments`, then the default value will be placed in the `results` instead.
+When a default value is set, the keyword becomes optional. Should the keyword not be part of the `arguments`, then the default value will be placed in the results instead.
 ```python
 command   = {'weather': 'cloudy'}
 arguments = ''
 ...
 result    = {'weather': 'cloudy'}
 is_set    = {'weather': False}
 ```
@@ -173,15 +179,15 @@
 arguments = '-meters -15'
 ...
 result    = {'meters': -15}
 ```
 ```python
 arguments = '-meters +15.0'
 ...
-result    = {'meters': 15.0}
+result    = {'meters': 15}
 ```
 ```python
 arguments = '-meters 15.4'
 ...
 result    = {'meters': 15}
 # This will result in a warning that the remainder of 0.4 has been cut off.
 ```
@@ -223,37 +229,55 @@
 ...
 result    = {'celsius': nan}
 is_set    = {'celsius': False}
 ```
 
 ---
 
-A __composite type__ is a `list` or `tuple` of one or more values of potentially multiple datatypes. Since `list` or `tuple` have the same semantics and can be used interchangeably, they will be referred to as 'array' for the purpose of this documentation.  
+A __composite type__ is a `list` or `tuple` containing one or more values of potentially multiple datatypes. Since `list` or `tuple` have the same semantics and can be used interchangeably, they will be referred to as 'array' for the purpose of this documentation.  
 
 The following __composite types__ are supported:  
 
 #### un-bounded array
-Specifying only the type `list` or `tuple`, will result in an 'unbounded array' of that type, meaning that all values following the keyword will be added to the array, until either the end of the `arguments` string is reached, or a value starts with a hyphen-minus (`'-'`), which denotes the start of the next argument. All values of this unbounded array will be of type `str`. This kind of argument should be used with caution because, for instance, negative values will be treated as the start of a new argument due to them starting with a hyphen-minus sign.  
+Specifying only the type `list` or `tuple`, will result in an 'unbounded array' of that type, meaning that all values following the keyword will be added to the array, until either the end of the `arguments` string is reached, or a value starts with a hyphen-minus (`'-'`), which denotes the start of the next argument. All values of this unbounded array will be of type `str`. This kind of argument should be used with caution because, for instance, negative numbers will be treated as the start of a new argument due to them starting with a hyphen-minus sign.  
 ```python
-{
+command = {
     'unbounded_list' : list,
     'unbounded_tuple': tuple,
 }
+arguments = '-unbounded_list 1 2 3 4 5 a b c -unbounded_tuple 1.0 + 1.0 = 2.0'
+...
+result = {'unbounded_list' : ['1', '2', '3', '4', '5', 'a', 'b', 'c'],
+          'unbounded_tuple': ('1.0', '+', '1.0', '=', '2.0')}
+is_set = {'unbounded_list': True, 'unbounded_tuple': True}
 ```  
 
 #### fixed array
-By specifying an array containing the types, default values, and ordering you want the values to have, you can define a fixed array. Their construction can get arbitrarily complex, mixing and matching any supported primitive type and fixed arrays you want. The only thing not allowed, is using an unbounded array inside a fixed array. All values will be cast to the corresponding type using all the same semantics as if they were single values (see above).  
-The only exception to that is the `bool` type. Since the value can't be decided based on presence of absence, a value has to be given. The value has to be either `'True'`, `'False'`, or interpretable as a `float`, which will then be cast to a `bool`. This means that e.g. `'0.0'` will result in `False`, and `'123'` will result in `'True'` (careful, check the [casting rules](https://docs.python.org/3.3/library/stdtypes.html?highlight=frozenset#truth-value-testing) first).
+By specifying an array containing the types, default values, and ordering you want the values to have, you can define a fixed array. Their construction can get arbitrarily complex, mixing and matching any supported primitive type and fixed arrays you want. The only thing not allowed, is using an unbounded array inside a fixed array. All values will be cast to the corresponding type using all the same semantics as if they were single values (see above).   
+Please note that while default values can be used to define the array, you currently need to specify all of the values, even if the array has default values at the end and they could technically be omitted. Default values in the middle of the array also currently don't have a mechanism for not setting them. This also means that since the value of a `bool` type can't be decided based on presence or absence, a value has to be given. We recognize a value of either `'True'`, `'False'`, or one interpretable as a `float`, which will then be cast to a `bool`. This means that e.g. `'0.0'` will result in `False`, and `'123'` will result in `'True'` (careful, check the [casting rules](https://docs.python.org/3.3/library/stdtypes.html?highlight=frozenset#truth-value-testing) first). 
 ```python
-{
+command = {
     'arg1': [int]*5,
     'arg2': (3.14, 'pi', bool),
     'arg3': (bool, str, 123)*2,
     'arg4': [[0]*3, [1]*3, [str]*3],
     'arg5': [str, int, bool, True, [1, '2', 3, bool], (2.1, float)]
 }
+arguments = '-arg1 4 5 6 7 8 \
+             -arg2 6.28 tau True \
+             -arg3 False helloworld 123 True HelloWorld 321 \
+             -arg4 0 0 0 1 1 1 2 2 2 \
+             -arg5 1 1 1 1 1 1 1 1 1 1'
+...
+result = {
+    'arg1': [4, 5, 6, 7, 8],
+    'arg2': (6.28, 'tau', True),
+    'arg3': (False, 'helloworld', 123, True, 'HelloWorld', 321),
+    'arg4': [[0, 0, 0], [1, 1, 1], ['2', '2', '2']],
+    'arg5': ['1', 1, True, True, [1, '1', 1, True], (1.0, 1.0)]}
+is_set = {'arg1': True, 'arg2': True, 'arg3': True, 'arg4': True, 'arg5': True}
 ```
 
 # Attribution
 This argument parser is largely inspired by and based upon, but in no way affiliated with, the work by [Jonathan Blow](https://www.youtube.com/@jblow888) as seen in these two videos on his youtube channel.
 > [Jonathan Blow - Livestream: Metaprogramming Use Case: Command-Line Argument Parsing - Part 1](https://youtu.be/TwqXTf7VfZk)  
 > [Jonathan Blow - Livestream: Metaprogramming Use Case: Command-Line Argument Parsing - Part 2](https://youtu.be/pgiVrhsGkKY)
```

### Comparing `argument_parsing-1.0.0/setup.py` & `argument_parsing-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         data['classifiers'].append(f'Development Status :: {dev_status[status-1]}')
     except (ValueError, IndexError):
         raise ValueError(f"Status '{status}' is an invalid value. \n"\
                          "It can only take on one of the following: {'1', '2', '3', '4', '5', '6', '7'}") from None
 
 
 metadata = dict(name             = 'argument_parsing',
-                version          = '1.0.0',
+                version          = '1.0.1',
                 description      = 'A zero dependency argument parser written in python.',
                 author           = 'Florian Peters',
                 packages         = find_packages(where='.'),
                 entry_points     = dict(console_scripts = list()),
                 install_requires = list(), # ['pip', 'packaging']
                 extras_require   = dict(),
                 classifiers      = list(),
```

