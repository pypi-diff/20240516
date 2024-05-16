# Comparing `tmp/jarguments-0.1.0.tar.gz` & `tmp/jarguments-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarguments-0.1.0.tar", last modified: Mon Apr 22 05:09:58 2024, max compression
+gzip compressed data, was "jarguments-0.2.0.tar", last modified: Thu May 16 00:37:04 2024, max compression
```

## Comparing `jarguments-0.1.0.tar` & `jarguments-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:09:58.966656 jarguments-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 05:09:53.000000 jarguments-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-22 05:09:58.966656 jarguments-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-22 05:09:53.000000 jarguments-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:09:58.962656 jarguments-0.1.0/jarguments/
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-22 05:09:53.000000 jarguments-0.1.0/jarguments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:09:58.966656 jarguments-0.1.0/jarguments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 05:09:58.966656 jarguments-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 05:09:53.000000 jarguments-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:37:04.055952 jarguments-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 00:36:58.000000 jarguments-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-16 00:37:04.055952 jarguments-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-16 00:36:58.000000 jarguments-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:37:04.051952 jarguments-0.2.0/jarguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-16 00:36:58.000000 jarguments-0.2.0/jarguments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-16 00:36:58.000000 jarguments-0.2.0/jarguments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-16 00:36:58.000000 jarguments-0.2.0/jarguments/handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-16 00:36:58.000000 jarguments-0.2.0/jarguments/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:37:04.051952 jarguments-0.2.0/jarguments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-16 00:37:04.000000 jarguments-0.2.0/jarguments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 00:37:04.000000 jarguments-0.2.0/jarguments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:37:04.000000 jarguments-0.2.0/jarguments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 00:37:04.000000 jarguments-0.2.0/jarguments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:37:04.000000 jarguments-0.2.0/jarguments.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:37:04.055952 jarguments-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-16 00:36:58.000000 jarguments-0.2.0/setup.py
```

### Comparing `jarguments-0.1.0/LICENSE` & `jarguments-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jarguments-0.1.0/PKG-INFO` & `jarguments-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,106 @@
 Metadata-Version: 2.1
 Name: jarguments
-Version: 0.1.0
-Summary: Providing a straightforward way to create command-line arguments.
+Version: 0.2.0
+Summary: Provides a straightforward way to create command line arguments.
 Home-page: https://github.com/silvncr/jarguments
 Author: silvncr
 License: MIT
-Classifier: Programming Language :: Python
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- omit from toc -->
 # jarguments
 
 simplifying args jargon
 
-![[license](LICENSE)](https://img.shields.io/github/license/silvncr/jarguments)
-![[publish status](https://github.com/silvncr/jarguments/actions/workflows/python-publish.yml)](https://img.shields.io/github/actions/workflow/status/silvncr/jarguments/python-publish.yml)
-![[latest release](https://github.com/silvncr/jarguments/releases/latest)](https://img.shields.io/github/v/release/silvncr/jarguments)
+![version](https://img.shields.io/pypi/v/jarguments)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/jarguments/python-publish.yml)
+![downloads](https://img.shields.io/pypi/dm/jarguments)
 
 ## Summary
 
-Providing a straightforward way to create command-line arguments.
+Provides a straightforward way to create command line arguments.
 
-> Works on Python 3.6 and above. Tested on Windows 10.
+- :snake: Supports Python 3.8 and above. Tested on Windows 10.
+- :warning: This project is still in development. Contributions are welcome!
+- :star: The simplest way to show your support is to leave a star!
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Library](#library)
-  - [Command-line](#command-line)
 
 ## Installation
 
 ```sh
-pip install jarguments
+python -m pip install --upgrade jarguments
 ```
 
 ## Usage
 
-### Library
-
 There are three steps to using the jarguments library:
 
 1. Import the jarguments library.
 
     ```py
-    import jarguments as j
+    from jarguments import create, parse
     ```
 
 2. Provide your arguments with jarguments' classes.
 
     ```py
-    args = j.JParser(
-      j.JBool('show-text', help='determines whether "text" is shown'),
-      j.JInt('number', default=1),
-      j.JArgument('text', type=str, multiple=True),
+    # argument parser
+    args = parse.JParser(
+
+      # boolean argument
+      create.JBool('show-text', helpstring='determines whether "text" is shown'),
+
+      # integer argument
+      create.JInt('number', default=1),
+
+      # string argument
+      create.JStr('text'),
     )
     ```
 
 3. Use the outputs; they're parsed automatically!
 
     ```py
     if args.show_text:
       for _ in range(args.number):
         print(args.text)
     ```
 
-### Command-line
-
-- Now you can run your script with arguments:
+Now it works just like any other command line application.
 
-    ```sh
-    $ python example.py --show-text --text "hello" "world"
-    ["hello", "world"]
-    ```
+  ```sh
+  $ python example.py --show-text --text "hello" "world"
+  ["hello", "world"]
+  ```
 
 - Arguments without a default value are required. If you don't provide them, the script will raise an error:
 
     ```sh
     $ python example.py --show-text
     error: the following arguments are required: --text
     ```
 
-- If you want to see help messages, run your script with the `-h` or `--help` flag:
+- The `--help`/`-h` flag displays help messages:
 
     ```sh
     $ python example.py -h
     usage: example.py [-h] [--show-text [SHOW_TEXT]] [--number NUMBER] --text [TEXT ...]
 
     options:
       -h, --help            show this help message and exit
```

### Comparing `jarguments-0.1.0/README.md` & `jarguments-0.2.0/jarguments.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,106 @@
+Metadata-Version: 2.1
+Name: jarguments
+Version: 0.2.0
+Summary: Provides a straightforward way to create command line arguments.
+Home-page: https://github.com/silvncr/jarguments
+Author: silvncr
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!-- omit from toc -->
 # jarguments
 
 simplifying args jargon
 
-![[license](LICENSE)](https://img.shields.io/github/license/silvncr/jarguments)
-![[publish status](https://github.com/silvncr/jarguments/actions/workflows/python-publish.yml)](https://img.shields.io/github/actions/workflow/status/silvncr/jarguments/python-publish.yml)
-![[latest release](https://github.com/silvncr/jarguments/releases/latest)](https://img.shields.io/github/v/release/silvncr/jarguments)
+![version](https://img.shields.io/pypi/v/jarguments)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/jarguments/python-publish.yml)
+![downloads](https://img.shields.io/pypi/dm/jarguments)
 
 ## Summary
 
-Providing a straightforward way to create command-line arguments.
+Provides a straightforward way to create command line arguments.
 
-> Works on Python 3.6 and above. Tested on Windows 10.
+- :snake: Supports Python 3.8 and above. Tested on Windows 10.
+- :warning: This project is still in development. Contributions are welcome!
+- :star: The simplest way to show your support is to leave a star!
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Library](#library)
-  - [Command-line](#command-line)
 
 ## Installation
 
 ```sh
-pip install jarguments
+python -m pip install --upgrade jarguments
 ```
 
 ## Usage
 
-### Library
-
 There are three steps to using the jarguments library:
 
 1. Import the jarguments library.
 
     ```py
-    import jarguments as j
+    from jarguments import create, parse
     ```
 
 2. Provide your arguments with jarguments' classes.
 
     ```py
-    args = j.JParser(
-      j.JBool('show-text', help='determines whether "text" is shown'),
-      j.JInt('number', default=1),
-      j.JArgument('text', type=str, multiple=True),
+    # argument parser
+    args = parse.JParser(
+
+      # boolean argument
+      create.JBool('show-text', helpstring='determines whether "text" is shown'),
+
+      # integer argument
+      create.JInt('number', default=1),
+
+      # string argument
+      create.JStr('text'),
     )
     ```
 
 3. Use the outputs; they're parsed automatically!
 
     ```py
     if args.show_text:
       for _ in range(args.number):
         print(args.text)
     ```
 
-### Command-line
-
-- Now you can run your script with arguments:
+Now it works just like any other command line application.
 
-    ```sh
-    $ python example.py --show-text --text "hello" "world"
-    ["hello", "world"]
-    ```
+  ```sh
+  $ python example.py --show-text --text "hello" "world"
+  ["hello", "world"]
+  ```
 
 - Arguments without a default value are required. If you don't provide them, the script will raise an error:
 
     ```sh
     $ python example.py --show-text
     error: the following arguments are required: --text
     ```
 
-- If you want to see help messages, run your script with the `-h` or `--help` flag:
+- The `--help`/`-h` flag displays help messages:
 
     ```sh
     $ python example.py -h
     usage: example.py [-h] [--show-text [SHOW_TEXT]] [--number NUMBER] --text [TEXT ...]
 
     options:
       -h, --help            show this help message and exit
```

### Comparing `jarguments-0.1.0/jarguments.egg-info/PKG-INFO` & `jarguments-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,87 @@
-Metadata-Version: 2.1
-Name: jarguments
-Version: 0.1.0
-Summary: Providing a straightforward way to create command-line arguments.
-Home-page: https://github.com/silvncr/jarguments
-Author: silvncr
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- omit from toc -->
 # jarguments
 
 simplifying args jargon
 
-![[license](LICENSE)](https://img.shields.io/github/license/silvncr/jarguments)
-![[publish status](https://github.com/silvncr/jarguments/actions/workflows/python-publish.yml)](https://img.shields.io/github/actions/workflow/status/silvncr/jarguments/python-publish.yml)
-![[latest release](https://github.com/silvncr/jarguments/releases/latest)](https://img.shields.io/github/v/release/silvncr/jarguments)
+![version](https://img.shields.io/pypi/v/jarguments)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/jarguments/python-publish.yml)
+![downloads](https://img.shields.io/pypi/dm/jarguments)
 
 ## Summary
 
-Providing a straightforward way to create command-line arguments.
+Provides a straightforward way to create command line arguments.
 
-> Works on Python 3.6 and above. Tested on Windows 10.
+- :snake: Supports Python 3.8 and above. Tested on Windows 10.
+- :warning: This project is still in development. Contributions are welcome!
+- :star: The simplest way to show your support is to leave a star!
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Library](#library)
-  - [Command-line](#command-line)
 
 ## Installation
 
 ```sh
-pip install jarguments
+python -m pip install --upgrade jarguments
 ```
 
 ## Usage
 
-### Library
-
 There are three steps to using the jarguments library:
 
 1. Import the jarguments library.
 
     ```py
-    import jarguments as j
+    from jarguments import create, parse
     ```
 
 2. Provide your arguments with jarguments' classes.
 
     ```py
-    args = j.JParser(
-      j.JBool('show-text', help='determines whether "text" is shown'),
-      j.JInt('number', default=1),
-      j.JArgument('text', type=str, multiple=True),
+    # argument parser
+    args = parse.JParser(
+
+      # boolean argument
+      create.JBool('show-text', helpstring='determines whether "text" is shown'),
+
+      # integer argument
+      create.JInt('number', default=1),
+
+      # string argument
+      create.JStr('text'),
     )
     ```
 
 3. Use the outputs; they're parsed automatically!
 
     ```py
     if args.show_text:
       for _ in range(args.number):
         print(args.text)
     ```
 
-### Command-line
-
-- Now you can run your script with arguments:
+Now it works just like any other command line application.
 
-    ```sh
-    $ python example.py --show-text --text "hello" "world"
-    ["hello", "world"]
-    ```
+  ```sh
+  $ python example.py --show-text --text "hello" "world"
+  ["hello", "world"]
+  ```
 
 - Arguments without a default value are required. If you don't provide them, the script will raise an error:
 
     ```sh
     $ python example.py --show-text
     error: the following arguments are required: --text
     ```
 
-- If you want to see help messages, run your script with the `-h` or `--help` flag:
+- The `--help`/`-h` flag displays help messages:
 
     ```sh
     $ python example.py -h
     usage: example.py [-h] [--show-text [SHOW_TEXT]] [--number NUMBER] --text [TEXT ...]
 
     options:
       -h, --help            show this help message and exit
```

### Comparing `jarguments-0.1.0/setup.py` & `jarguments-0.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,43 @@
-from jarguments import __author__, __doc__, __license__, __module_name__, __python_version__, __version__
+'Setup script for the jarguments package.'
 
+from pathlib import Path
+
+from jarguments import (
+	__author__,
+	__doc__,
+	__license__,
+	__module_name__,
+	__python_version__,
+	__version__,
+)
 from setuptools import setup
 
 setup(
 	name=__module_name__,
 	version=__version__,
 	description=__doc__,
-	long_description=open('README.md', 'r').read(),
+	long_description=Path('README.md').read_text(),
 	long_description_content_type='text/markdown',
 	url=f'https://github.com/{__author__}/{__module_name__}',
 	author=__author__,
 	include_package_data=True,
 	license=__license__,
 	packages=[__module_name__],
 	package_data={},
 	setup_requires=['pytest_runner'],
 	python_requires=f'>={__python_version__}',
 	scripts=[],
 	tests_require=['pytest'],
 	entry_points={},
 	zip_safe=True,
 	classifiers=[
-		'Programming Language :: Python',
+		'Development Status :: 4 - Beta',
+		'License :: OSI Approved :: MIT License',
+		'Operating System :: OS Independent',
+		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3',
-		'Topic :: Software Development :: Libraries',
+		'Programming Language :: Python',
 		'Topic :: Software Development :: Libraries :: Python Modules',
+		'Topic :: Software Development :: Libraries',
 	],
 )
```

