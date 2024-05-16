# Comparing `tmp/javascript_fixes-1.1.8.tar.gz` & `tmp/javascript_fixes-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "javascript_fixes-1.1.8.tar", last modified: Wed Feb  7 05:17:27 2024, max compression
+gzip compressed data, was "javascript_fixes-1.1.9.tar", last modified: Wed Feb  7 05:24:54 2024, max compression
```

## Comparing `javascript_fixes-1.1.8.tar` & `javascript_fixes-1.1.9.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-02-07 05:17:27.671880 javascript_fixes-1.1.8/
--rw-rw-rw-   0        0        0     1099 2024-02-07 04:06:39.000000 javascript_fixes-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      141 2024-02-07 04:13:28.000000 javascript_fixes-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    14846 2024-02-07 05:17:27.671880 javascript_fixes-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    13678 2024-02-07 04:13:28.000000 javascript_fixes-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-02-07 05:17:27.671880 javascript_fixes-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0    10952 2024-02-07 05:17:26.000000 javascript_fixes-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-07 05:17:27.570931 javascript_fixes-1.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-02-07 05:17:27.637117 javascript_fixes-1.1.8/src/javascript_fixes/
--rw-rw-rw-   0        0        0     5223 2024-02-07 05:17:21.000000 javascript_fixes-1.1.8/src/javascript_fixes/__init__.py
--rw-rw-rw-   0        0        0     1672 2024-02-07 04:13:27.000000 javascript_fixes-1.1.8/src/javascript_fixes/__main__.py
--rw-rw-rw-   0        0        0      643 2024-02-07 04:06:39.000000 javascript_fixes-1.1.8/src/javascript_fixes/config.py
--rw-rw-rw-   0        0        0     6447 2024-02-07 04:06:39.000000 javascript_fixes-1.1.8/src/javascript_fixes/connection.py
--rw-rw-rw-   0        0        0     7209 2024-02-07 04:13:28.000000 javascript_fixes-1.1.8/src/javascript_fixes/errors.py
--rw-rw-rw-   0        0        0     6615 2024-02-07 04:06:39.000000 javascript_fixes-1.1.8/src/javascript_fixes/events.py
--rw-rw-rw-   0        0        0      586 2024-02-07 04:06:39.000000 javascript_fixes-1.1.8/src/javascript_fixes/json_patch.py
--rw-rw-rw-   0        0        0      387 2024-02-07 04:22:14.000000 javascript_fixes-1.1.8/src/javascript_fixes/packageinstall.py
--rw-rw-rw-   0        0        0    11319 2024-02-07 04:06:39.000000 javascript_fixes-1.1.8/src/javascript_fixes/proxy.py
--rw-rw-rw-   0        0        0     9837 2024-02-07 04:06:39.000000 javascript_fixes-1.1.8/src/javascript_fixes/pyi.py
-drwxrwxrwx   0        0        0        0 2024-02-07 05:17:27.670329 javascript_fixes-1.1.8/src/javascript_fixes.egg-info/
--rw-rw-rw-   0        0        0    14846 2024-02-07 05:17:27.000000 javascript_fixes-1.1.8/src/javascript_fixes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2024-02-07 05:17:27.000000 javascript_fixes-1.1.8/src/javascript_fixes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-07 05:17:27.000000 javascript_fixes-1.1.8/src/javascript_fixes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-02-07 05:17:27.000000 javascript_fixes-1.1.8/src/javascript_fixes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-02-07 05:17:27.000000 javascript_fixes-1.1.8/src/javascript_fixes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-07 05:24:54.925161 javascript_fixes-1.1.9/
+-rw-rw-rw-   0        0        0     1099 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      165 2024-02-07 05:24:09.000000 javascript_fixes-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    14930 2024-02-07 05:24:54.925161 javascript_fixes-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13762 2024-02-07 05:24:09.000000 javascript_fixes-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-02-07 05:24:54.925161 javascript_fixes-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0    10952 2024-02-07 05:24:53.000000 javascript_fixes-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-07 05:24:54.806651 javascript_fixes-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-02-07 05:24:54.874338 javascript_fixes-1.1.9/src/javascript_fixes/
+-rw-rw-rw-   0        0        0     5223 2024-02-07 05:17:21.000000 javascript_fixes-1.1.9/src/javascript_fixes/__init__.py
+-rw-rw-rw-   0        0        0     1678 2024-02-07 05:24:09.000000 javascript_fixes-1.1.9/src/javascript_fixes/__main__.py
+-rw-rw-rw-   0        0        0      643 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/config.py
+-rw-rw-rw-   0        0        0     6447 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/connection.py
+-rw-rw-rw-   0        0        0     7215 2024-02-07 05:24:09.000000 javascript_fixes-1.1.9/src/javascript_fixes/errors.py
+-rw-rw-rw-   0        0        0     6615 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/events.py
+drwxrwxrwx   0        0        0        0 2024-02-07 05:24:54.916336 javascript_fixes-1.1.9/src/javascript_fixes/js/
+-rw-rw-rw-   0        0        0     9963 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/js/bridge.js
+-rw-rw-rw-   0        0        0     4800 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/js/deps.js
+-rw-rw-rw-   0        0        0     4191 2024-02-07 05:24:09.000000 javascript_fixes-1.1.9/src/javascript_fixes/js/errors.js
+-rw-rw-rw-   0        0        0    11186 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/js/pyi.js
+-rw-rw-rw-   0        0        0      586 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/json_patch.py
+-rw-rw-rw-   0        0        0      387 2024-02-07 04:22:14.000000 javascript_fixes-1.1.9/src/javascript_fixes/packageinstall.py
+-rw-rw-rw-   0        0        0    11319 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/proxy.py
+-rw-rw-rw-   0        0        0     9837 2024-02-07 04:06:39.000000 javascript_fixes-1.1.9/src/javascript_fixes/pyi.py
+drwxrwxrwx   0        0        0        0 2024-02-07 05:24:54.922932 javascript_fixes-1.1.9/src/javascript_fixes.egg-info/
+-rw-rw-rw-   0        0        0    14930 2024-02-07 05:24:54.000000 javascript_fixes-1.1.9/src/javascript_fixes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2024-02-07 05:24:54.000000 javascript_fixes-1.1.9/src/javascript_fixes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-07 05:24:54.000000 javascript_fixes-1.1.9/src/javascript_fixes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-02-07 05:24:54.000000 javascript_fixes-1.1.9/src/javascript_fixes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-02-07 05:24:54.000000 javascript_fixes-1.1.9/src/javascript_fixes.egg-info/top_level.txt
```

### Comparing `javascript_fixes-1.1.8/LICENSE` & `javascript_fixes-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `javascript_fixes-1.1.8/PKG-INFO` & `javascript_fixes-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: javascript_fixes
-Version: 1.1.8
+Version: 1.1.9
 Summary: Call and interop Node.js APIs with Python
 Home-page: https://github.com/extremeheat/JSPyBridge
 Author: extremeheat
 Author-email: extreme@protonmail.ch
 Project-URL: Bug Reports, https://github.com/extremeheat/JSPyBridge/issues
 Project-URL: Say Thanks!, https://github.com/extremeheat/JSPyBridge
 Project-URL: Source, https://github.com/extremeheat/JSPyBridge/
@@ -24,15 +24,15 @@
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 # JSPyBridge
 [![NPM version](https://img.shields.io/npm/v/pythonia.svg)](http://npmjs.com/package/pythonia)
-[![PyPI](https://img.shields.io/pypi/v/javascript)](https://pypi.org/project/javascript/)
+[![PyPI](https://img.shields.io/pypi/v/javascript_fixes)](https://pypi.org/project/javascript_fixes/)
 [![Build Status](https://github.com/extremeheat/JSPyBridge/actions/workflows/node.yml/badge.svg)](https://github.com/extremeheat/JSPyBridge/actions/workflows/)
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/extremeheat/jspybridge)
 
 
 Interoperate Node.js and Python. You can run Python from Node.js, *or* run Node.js from Python. **Work in progress.** 
 
 Requires Node.js 14 and Python 3.8 or newer.
@@ -40,33 +40,33 @@
 ## Key Features
 
 * Ability to call async and sync functions and get object properties with a native feel
 * Built-in garbage collection
 * Bidirectional callbacks with arbitrary arguments
 * Iteration and exception handling support
 * Object inspection allows you to easily `console.log` or `print()` any foreign objects
-* (Bridge to call Python from JS) Python class extension and inheritance. [See pytorch and tensorflow examples](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/pytorch-train.js).
+* (Bridge to call Python from JS) Python class extension and inheritance. [See pytorch and tensorflow examples](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/pytorch-train.js).
 * (Bridge to call JS from Python) Native decorator-based event emitter support
 * (Bridge to call JS from Python) **First-class Jupyter Notebook/Google Colab support.** See some Google Colab uses below.
 
 
 ## Basic usage example
 
 See some examples [here](https://github.com/extremeheat/JSPyBridge/tree/master/examples). See [documentation](https://github.com/extremeheat/JSPyBridge#documentation) below and in [here](https://github.com/extremeheat/JSPyBridge/tree/master/docs).
 
 ### Access JavaScript from Python
 
 
 ```sh
-pip3 install javascript
+pip3 install javascript_fixes
 ```
 
 
 ```py
-from javascript import require, globalThis
+from javascript_fixes import require, globalThis
 
 chalk, fs = require("chalk"), require("fs")
 
 print("Hello", chalk.red("world!"), "it's", globalThis.Date().toLocaleString())
 fs.writeFileSync("HelloWorld.txt", "hi!")
 ```
 
@@ -93,29 +93,29 @@
 
 ### Examples
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/extremeheat/jspybridge)
 
 Check out some cool examples below! Try them on Gitpod! Click the Open in Gitpod link above, and then open the examples folder.
 
 
-[![PyTorch](https://www.vectorlogo.zone/logos/pytorch/pytorch-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/pytorch-train.js)
-[![numpy](https://www.vectorlogo.zone/logos/numpy/numpy-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/matplotlib.js)
-[![tensorflow](https://www.vectorlogo.zone/logos/tensorflow/tensorflow-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/tensorflow.js)
+[![PyTorch](https://www.vectorlogo.zone/logos/pytorch/pytorch-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/pytorch-train.js)
+[![numpy](https://www.vectorlogo.zone/logos/numpy/numpy-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/matplotlib.js)
+[![tensorflow](https://www.vectorlogo.zone/logos/tensorflow/tensorflow-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/tensorflow.js)
 [![mineflayer](https://www.vectorlogo.zone/logos/minecraft/minecraft-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/python/mineflayer.py)
 <!-- <img src="https://matplotlib.org/stable/_static/logo2_compressed.svg" alt="matplotlib" width="120" height="70">
  -->
 
 
 ### Bridge feature comparison
 
 Unlike other bridges, you may notice you're not just writing Python code in JavaScript, or vice-versa. You can operate on objects
 on the other side of the bridge as if the objects existed on your side. This is achieved through real interop support: you can call
 callbacks, and do loss-less function calls with any arguments you like (with the exception of floating points percision of course).
 
-|  | python(ia) bridge | javascript bridge | [npm:python-bridge](https://www.npmjs.com/package/python-bridge) |
+|  | python(ia) bridge | javascript_fixes bridge | [npm:python-bridge](https://www.npmjs.com/package/python-bridge) |
 |---|---|---|---|
 | Garbage collection | ✔ | ✔ | ❌ |
 | Class extension support | ✔ | Not built-in (rare use case), can be manually done with custom proxy | ❌ |
 | Passthrough stdin | ❌ (Standard input is not piped to bridge processes. Instead, listen to standard input then expose an API on the other side of the bridge recieve the data.) | ❌ | ✔ |
 | Passthrough stdout, stderr | ✔ | ✔ | ✔ |
 | Long-running sync calls | ✔ | ✔ | ✔ |
 | Long-running async calls | ❌ (need to manually create new thread) | ✔ (AsyncTask) | ❌ (need to manually create new thread) |
@@ -133,15 +133,15 @@
 
 # Documentation
 
 ## From Python
 
 You can import the bridge module with 
 ```py
-from javascript import require
+from javascript_fixes import require
 ```
 
 This will import the require function which you can use just like in Node.js. This is a slightly
 modified require function which does dependency management for you. The first paramater is the name
 or location of the file to import. Internally, this calls the ES6 dynamic `import()` function. Which
 supports both CommonJS and ES6 modules.
 
@@ -179,15 +179,15 @@
     return (new Date()).toLocaleString()
 }
 module.exports = { whatTimeIsIt }
 ```
 
 Then we can call it from Python !
 ```py
-from javascript import require
+from javascript_fixes import require
 time = require('./time.js')
 print(time.whatTimeIsIt())
 ```
 
 ### Event emitter
 
 *You must use the provided On, Once, decorator and off function over the normal dot methods.*
@@ -202,15 +202,15 @@
     }
 }
 module.exports = { MyEmitter }
 ```
 
 listener.py
 ```py
-from javascript import require, On, off
+from javascript_fixes import require, On, off
 MyEmitter = require('./emitter.js')
 # New class instance
 myEmitter = MyEmitter()
 # Decorator usage
 @On(myEmitter, 'increment')
 def handleIncrement(this, counter):
     print("Incremented", counter)
@@ -278,15 +278,15 @@
   be in the correct order to what the Python function expects.
 * Some Python objects accept arbitrary keyword arguments. You can call these functions by using
   the special `$` function syntax. 
   * When you do a function call with a `$` before the parenthesis, such as `await some.pythonCall$()`, 
     the final argument is evaluated as a kwarg dictionary. You can supply named arguments this way.
 * Property access with a $ at the end acts as a error suppression operator. 
   * Any errors will be ignored and instead undefined will be returned
-* See [docs/javascript.md](docs/javascript.md) for more docs, and the examples for more info
+* See [docs/javascript_fixes.md](docs/javascript_fixes.md) for more docs, and the examples for more info
 
 ### Usage
 
 <details>
   <summary>👉 Click here to see some code usage examples 👈</summary>
 
 ### Basic import
```

### Comparing `javascript_fixes-1.1.8/README.md` & `javascript_fixes-1.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # JSPyBridge
 [![NPM version](https://img.shields.io/npm/v/pythonia.svg)](http://npmjs.com/package/pythonia)
-[![PyPI](https://img.shields.io/pypi/v/javascript)](https://pypi.org/project/javascript/)
+[![PyPI](https://img.shields.io/pypi/v/javascript_fixes)](https://pypi.org/project/javascript_fixes/)
 [![Build Status](https://github.com/extremeheat/JSPyBridge/actions/workflows/node.yml/badge.svg)](https://github.com/extremeheat/JSPyBridge/actions/workflows/)
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/extremeheat/jspybridge)
 
 
 Interoperate Node.js and Python. You can run Python from Node.js, *or* run Node.js from Python. **Work in progress.** 
 
 Requires Node.js 14 and Python 3.8 or newer.
@@ -12,33 +12,33 @@
 ## Key Features
 
 * Ability to call async and sync functions and get object properties with a native feel
 * Built-in garbage collection
 * Bidirectional callbacks with arbitrary arguments
 * Iteration and exception handling support
 * Object inspection allows you to easily `console.log` or `print()` any foreign objects
-* (Bridge to call Python from JS) Python class extension and inheritance. [See pytorch and tensorflow examples](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/pytorch-train.js).
+* (Bridge to call Python from JS) Python class extension and inheritance. [See pytorch and tensorflow examples](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/pytorch-train.js).
 * (Bridge to call JS from Python) Native decorator-based event emitter support
 * (Bridge to call JS from Python) **First-class Jupyter Notebook/Google Colab support.** See some Google Colab uses below.
 
 
 ## Basic usage example
 
 See some examples [here](https://github.com/extremeheat/JSPyBridge/tree/master/examples). See [documentation](https://github.com/extremeheat/JSPyBridge#documentation) below and in [here](https://github.com/extremeheat/JSPyBridge/tree/master/docs).
 
 ### Access JavaScript from Python
 
 
 ```sh
-pip3 install javascript
+pip3 install javascript_fixes
 ```
 
 
 ```py
-from javascript import require, globalThis
+from javascript_fixes import require, globalThis
 
 chalk, fs = require("chalk"), require("fs")
 
 print("Hello", chalk.red("world!"), "it's", globalThis.Date().toLocaleString())
 fs.writeFileSync("HelloWorld.txt", "hi!")
 ```
 
@@ -65,29 +65,29 @@
 
 ### Examples
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/extremeheat/jspybridge)
 
 Check out some cool examples below! Try them on Gitpod! Click the Open in Gitpod link above, and then open the examples folder.
 
 
-[![PyTorch](https://www.vectorlogo.zone/logos/pytorch/pytorch-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/pytorch-train.js)
-[![numpy](https://www.vectorlogo.zone/logos/numpy/numpy-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/matplotlib.js)
-[![tensorflow](https://www.vectorlogo.zone/logos/tensorflow/tensorflow-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/tensorflow.js)
+[![PyTorch](https://www.vectorlogo.zone/logos/pytorch/pytorch-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/pytorch-train.js)
+[![numpy](https://www.vectorlogo.zone/logos/numpy/numpy-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/matplotlib.js)
+[![tensorflow](https://www.vectorlogo.zone/logos/tensorflow/tensorflow-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/tensorflow.js)
 [![mineflayer](https://www.vectorlogo.zone/logos/minecraft/minecraft-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/python/mineflayer.py)
 <!-- <img src="https://matplotlib.org/stable/_static/logo2_compressed.svg" alt="matplotlib" width="120" height="70">
  -->
 
 
 ### Bridge feature comparison
 
 Unlike other bridges, you may notice you're not just writing Python code in JavaScript, or vice-versa. You can operate on objects
 on the other side of the bridge as if the objects existed on your side. This is achieved through real interop support: you can call
 callbacks, and do loss-less function calls with any arguments you like (with the exception of floating points percision of course).
 
-|  | python(ia) bridge | javascript bridge | [npm:python-bridge](https://www.npmjs.com/package/python-bridge) |
+|  | python(ia) bridge | javascript_fixes bridge | [npm:python-bridge](https://www.npmjs.com/package/python-bridge) |
 |---|---|---|---|
 | Garbage collection | ✔ | ✔ | ❌ |
 | Class extension support | ✔ | Not built-in (rare use case), can be manually done with custom proxy | ❌ |
 | Passthrough stdin | ❌ (Standard input is not piped to bridge processes. Instead, listen to standard input then expose an API on the other side of the bridge recieve the data.) | ❌ | ✔ |
 | Passthrough stdout, stderr | ✔ | ✔ | ✔ |
 | Long-running sync calls | ✔ | ✔ | ✔ |
 | Long-running async calls | ❌ (need to manually create new thread) | ✔ (AsyncTask) | ❌ (need to manually create new thread) |
@@ -105,15 +105,15 @@
 
 # Documentation
 
 ## From Python
 
 You can import the bridge module with 
 ```py
-from javascript import require
+from javascript_fixes import require
 ```
 
 This will import the require function which you can use just like in Node.js. This is a slightly
 modified require function which does dependency management for you. The first paramater is the name
 or location of the file to import. Internally, this calls the ES6 dynamic `import()` function. Which
 supports both CommonJS and ES6 modules.
 
@@ -151,15 +151,15 @@
     return (new Date()).toLocaleString()
 }
 module.exports = { whatTimeIsIt }
 ```
 
 Then we can call it from Python !
 ```py
-from javascript import require
+from javascript_fixes import require
 time = require('./time.js')
 print(time.whatTimeIsIt())
 ```
 
 ### Event emitter
 
 *You must use the provided On, Once, decorator and off function over the normal dot methods.*
@@ -174,15 +174,15 @@
     }
 }
 module.exports = { MyEmitter }
 ```
 
 listener.py
 ```py
-from javascript import require, On, off
+from javascript_fixes import require, On, off
 MyEmitter = require('./emitter.js')
 # New class instance
 myEmitter = MyEmitter()
 # Decorator usage
 @On(myEmitter, 'increment')
 def handleIncrement(this, counter):
     print("Incremented", counter)
@@ -250,15 +250,15 @@
   be in the correct order to what the Python function expects.
 * Some Python objects accept arbitrary keyword arguments. You can call these functions by using
   the special `$` function syntax. 
   * When you do a function call with a `$` before the parenthesis, such as `await some.pythonCall$()`, 
     the final argument is evaluated as a kwarg dictionary. You can supply named arguments this way.
 * Property access with a $ at the end acts as a error suppression operator. 
   * Any errors will be ignored and instead undefined will be returned
-* See [docs/javascript.md](docs/javascript.md) for more docs, and the examples for more info
+* See [docs/javascript_fixes.md](docs/javascript_fixes.md) for more docs, and the examples for more info
 
 ### Usage
 
 <details>
   <summary>👉 Click here to see some code usage examples 👈</summary>
 
 ### Basic import
```

### Comparing `javascript_fixes-1.1.8/setup.py` & `javascript_fixes-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.1.8',  # Required
+    version='1.1.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Call and interop Node.js APIs with Python',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/__init__.py` & `javascript_fixes-1.1.9/src/javascript_fixes/__init__.py`

 * *Files identical despite different names*

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/__main__.py` & `javascript_fixes-1.1.9/src/javascript_fixes/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, sys, argparse, shutil
 
 PACKAGEJSON = '{\n\t"name": "js-modules",\n\t"description": "This folder holds the installed JS deps",\n\t"dependencies": {}\n}'
 
 parser = argparse.ArgumentParser(
-    description="javascript (JSPyBridge) package manager. Use this to clear or update the internal package store."
+    description="javascript_fixes (JSPyBridge) package manager. Use this to clear or update the internal package store."
 )
 parser.add_argument("--clean", default=False, action="store_true")
 parser.add_argument("--update", default=False, action="store_true")
 parser.add_argument("--install", default=False, action="store")
 parser.add_argument("--uninstall", default=False, action="store")
 args = parser.parse_args()
```

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/config.py` & `javascript_fixes-1.1.9/src/javascript_fixes/config.py`

 * *Files identical despite different names*

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/connection.py` & `javascript_fixes-1.1.9/src/javascript_fixes/connection.py`

 * *Files identical despite different names*

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/errors.py` & `javascript_fixes-1.1.9/src/javascript_fixes/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     log(
         "☕",
         chalk.bold(chalk.bgred(" JavaScript Error ")),
         f"Call to '{failedCall.replace('~~', '')}' failed:",
     )
 
     for at, line in pyStacktrace:
-        if "javascript" in at or "IPython" in at:
+        if "javascript_fixes" in at or "IPython" in at:
             continue
         if not line:
             log(" ", chalk.gray(at))
         else:
             log(chalk.gray(">"), format_line(line))
             log(" ", chalk.gray(at))
```

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/events.py` & `javascript_fixes-1.1.9/src/javascript_fixes/events.py`

 * *Files identical despite different names*

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/json_patch.py` & `javascript_fixes-1.1.9/src/javascript_fixes/json_patch.py`

 * *Files identical despite different names*

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/proxy.py` & `javascript_fixes-1.1.9/src/javascript_fixes/proxy.py`

 * *Files identical despite different names*

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes/pyi.py` & `javascript_fixes-1.1.9/src/javascript_fixes/pyi.py`

 * *Files identical despite different names*

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes.egg-info/PKG-INFO` & `javascript_fixes-1.1.9/src/javascript_fixes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: javascript_fixes
-Version: 1.1.8
+Version: 1.1.9
 Summary: Call and interop Node.js APIs with Python
 Home-page: https://github.com/extremeheat/JSPyBridge
 Author: extremeheat
 Author-email: extreme@protonmail.ch
 Project-URL: Bug Reports, https://github.com/extremeheat/JSPyBridge/issues
 Project-URL: Say Thanks!, https://github.com/extremeheat/JSPyBridge
 Project-URL: Source, https://github.com/extremeheat/JSPyBridge/
@@ -24,15 +24,15 @@
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 # JSPyBridge
 [![NPM version](https://img.shields.io/npm/v/pythonia.svg)](http://npmjs.com/package/pythonia)
-[![PyPI](https://img.shields.io/pypi/v/javascript)](https://pypi.org/project/javascript/)
+[![PyPI](https://img.shields.io/pypi/v/javascript_fixes)](https://pypi.org/project/javascript_fixes/)
 [![Build Status](https://github.com/extremeheat/JSPyBridge/actions/workflows/node.yml/badge.svg)](https://github.com/extremeheat/JSPyBridge/actions/workflows/)
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/extremeheat/jspybridge)
 
 
 Interoperate Node.js and Python. You can run Python from Node.js, *or* run Node.js from Python. **Work in progress.** 
 
 Requires Node.js 14 and Python 3.8 or newer.
@@ -40,33 +40,33 @@
 ## Key Features
 
 * Ability to call async and sync functions and get object properties with a native feel
 * Built-in garbage collection
 * Bidirectional callbacks with arbitrary arguments
 * Iteration and exception handling support
 * Object inspection allows you to easily `console.log` or `print()` any foreign objects
-* (Bridge to call Python from JS) Python class extension and inheritance. [See pytorch and tensorflow examples](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/pytorch-train.js).
+* (Bridge to call Python from JS) Python class extension and inheritance. [See pytorch and tensorflow examples](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/pytorch-train.js).
 * (Bridge to call JS from Python) Native decorator-based event emitter support
 * (Bridge to call JS from Python) **First-class Jupyter Notebook/Google Colab support.** See some Google Colab uses below.
 
 
 ## Basic usage example
 
 See some examples [here](https://github.com/extremeheat/JSPyBridge/tree/master/examples). See [documentation](https://github.com/extremeheat/JSPyBridge#documentation) below and in [here](https://github.com/extremeheat/JSPyBridge/tree/master/docs).
 
 ### Access JavaScript from Python
 
 
 ```sh
-pip3 install javascript
+pip3 install javascript_fixes
 ```
 
 
 ```py
-from javascript import require, globalThis
+from javascript_fixes import require, globalThis
 
 chalk, fs = require("chalk"), require("fs")
 
 print("Hello", chalk.red("world!"), "it's", globalThis.Date().toLocaleString())
 fs.writeFileSync("HelloWorld.txt", "hi!")
 ```
 
@@ -93,29 +93,29 @@
 
 ### Examples
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/extremeheat/jspybridge)
 
 Check out some cool examples below! Try them on Gitpod! Click the Open in Gitpod link above, and then open the examples folder.
 
 
-[![PyTorch](https://www.vectorlogo.zone/logos/pytorch/pytorch-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/pytorch-train.js)
-[![numpy](https://www.vectorlogo.zone/logos/numpy/numpy-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/matplotlib.js)
-[![tensorflow](https://www.vectorlogo.zone/logos/tensorflow/tensorflow-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript/tensorflow.js)
+[![PyTorch](https://www.vectorlogo.zone/logos/pytorch/pytorch-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/pytorch-train.js)
+[![numpy](https://www.vectorlogo.zone/logos/numpy/numpy-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/matplotlib.js)
+[![tensorflow](https://www.vectorlogo.zone/logos/tensorflow/tensorflow-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/javascript_fixes/tensorflow.js)
 [![mineflayer](https://www.vectorlogo.zone/logos/minecraft/minecraft-ar21.svg)](https://github.com/extremeheat/JSPyBridge/blob/master/examples/python/mineflayer.py)
 <!-- <img src="https://matplotlib.org/stable/_static/logo2_compressed.svg" alt="matplotlib" width="120" height="70">
  -->
 
 
 ### Bridge feature comparison
 
 Unlike other bridges, you may notice you're not just writing Python code in JavaScript, or vice-versa. You can operate on objects
 on the other side of the bridge as if the objects existed on your side. This is achieved through real interop support: you can call
 callbacks, and do loss-less function calls with any arguments you like (with the exception of floating points percision of course).
 
-|  | python(ia) bridge | javascript bridge | [npm:python-bridge](https://www.npmjs.com/package/python-bridge) |
+|  | python(ia) bridge | javascript_fixes bridge | [npm:python-bridge](https://www.npmjs.com/package/python-bridge) |
 |---|---|---|---|
 | Garbage collection | ✔ | ✔ | ❌ |
 | Class extension support | ✔ | Not built-in (rare use case), can be manually done with custom proxy | ❌ |
 | Passthrough stdin | ❌ (Standard input is not piped to bridge processes. Instead, listen to standard input then expose an API on the other side of the bridge recieve the data.) | ❌ | ✔ |
 | Passthrough stdout, stderr | ✔ | ✔ | ✔ |
 | Long-running sync calls | ✔ | ✔ | ✔ |
 | Long-running async calls | ❌ (need to manually create new thread) | ✔ (AsyncTask) | ❌ (need to manually create new thread) |
@@ -133,15 +133,15 @@
 
 # Documentation
 
 ## From Python
 
 You can import the bridge module with 
 ```py
-from javascript import require
+from javascript_fixes import require
 ```
 
 This will import the require function which you can use just like in Node.js. This is a slightly
 modified require function which does dependency management for you. The first paramater is the name
 or location of the file to import. Internally, this calls the ES6 dynamic `import()` function. Which
 supports both CommonJS and ES6 modules.
 
@@ -179,15 +179,15 @@
     return (new Date()).toLocaleString()
 }
 module.exports = { whatTimeIsIt }
 ```
 
 Then we can call it from Python !
 ```py
-from javascript import require
+from javascript_fixes import require
 time = require('./time.js')
 print(time.whatTimeIsIt())
 ```
 
 ### Event emitter
 
 *You must use the provided On, Once, decorator and off function over the normal dot methods.*
@@ -202,15 +202,15 @@
     }
 }
 module.exports = { MyEmitter }
 ```
 
 listener.py
 ```py
-from javascript import require, On, off
+from javascript_fixes import require, On, off
 MyEmitter = require('./emitter.js')
 # New class instance
 myEmitter = MyEmitter()
 # Decorator usage
 @On(myEmitter, 'increment')
 def handleIncrement(this, counter):
     print("Incremented", counter)
@@ -278,15 +278,15 @@
   be in the correct order to what the Python function expects.
 * Some Python objects accept arbitrary keyword arguments. You can call these functions by using
   the special `$` function syntax. 
   * When you do a function call with a `$` before the parenthesis, such as `await some.pythonCall$()`, 
     the final argument is evaluated as a kwarg dictionary. You can supply named arguments this way.
 * Property access with a $ at the end acts as a error suppression operator. 
   * Any errors will be ignored and instead undefined will be returned
-* See [docs/javascript.md](docs/javascript.md) for more docs, and the examples for more info
+* See [docs/javascript_fixes.md](docs/javascript_fixes.md) for more docs, and the examples for more info
 
 ### Usage
 
 <details>
   <summary>👉 Click here to see some code usage examples 👈</summary>
 
 ### Basic import
```

### Comparing `javascript_fixes-1.1.8/src/javascript_fixes.egg-info/SOURCES.txt` & `javascript_fixes-1.1.9/src/javascript_fixes.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,8 +12,12 @@
 src/javascript_fixes/packageinstall.py
 src/javascript_fixes/proxy.py
 src/javascript_fixes/pyi.py
 src/javascript_fixes.egg-info/PKG-INFO
 src/javascript_fixes.egg-info/SOURCES.txt
 src/javascript_fixes.egg-info/dependency_links.txt
 src/javascript_fixes.egg-info/requires.txt
-src/javascript_fixes.egg-info/top_level.txt
+src/javascript_fixes.egg-info/top_level.txt
+src/javascript_fixes/js/bridge.js
+src/javascript_fixes/js/deps.js
+src/javascript_fixes/js/errors.js
+src/javascript_fixes/js/pyi.js
```

