# Comparing `tmp/drv8830-0.0.1.tar.gz` & `tmp/drv8830-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drv8830-0.0.1.tar", last modified: Mon Sep 23 18:50:24 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `drv8830-0.0.1.tar` & `drv8830-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-23 18:50:24.000000 drv8830-0.0.1/
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1479 2019-09-23 14:59:05.000000 drv8830-0.0.1/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)      812 2019-09-23 18:50:09.000000 drv8830-0.0.1/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2019-09-23 18:48:33.000000 drv8830-0.0.1/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1003 2019-09-23 18:50:24.000000 drv8830-0.0.1/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)       31 2019-09-23 18:48:37.000000 drv8830-0.0.1/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      108 2019-09-23 18:48:40.000000 drv8830-0.0.1/MANIFEST.in
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-23 18:50:24.000000 drv8830-0.0.1/drv8830/
--rw-r--r--   0 pi        (1000) pi        (1000)     4556 2019-09-23 18:45:00.000000 drv8830-0.0.1/drv8830/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1852 2019-09-23 18:50:24.000000 drv8830-0.0.1/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-23 18:50:24.000000 drv8830-0.0.1/drv8830.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      240 2019-09-23 18:50:24.000000 drv8830-0.0.1/drv8830.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2019-09-23 18:50:24.000000 drv8830-0.0.1/drv8830.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2019-09-23 18:50:24.000000 drv8830-0.0.1/drv8830.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2019-09-23 18:50:24.000000 drv8830-0.0.1/drv8830.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1852 2019-09-23 18:50:24.000000 drv8830-0.0.1/drv8830.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 drv8830-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 drv8830-1.0.0/Makefile
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 drv8830-1.0.0/README.md
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 drv8830-1.0.0/REFERENCE.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 drv8830-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 drv8830-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 drv8830-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 drv8830-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 drv8830-1.0.0/uninstall.sh
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 drv8830-1.0.0/drv8830/__init__.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 drv8830-1.0.0/examples/two-motors.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 drv8830-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 drv8830-1.0.0/tests/test_features.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 drv8830-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 drv8830-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 drv8830-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 drv8830-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 drv8830-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `drv8830-0.0.1/setup.py` & `drv8830-1.0.0/LICENSE`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Copyright (c) 2016 Pimoroni
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Copyright (c) 2018 Pimoroni Ltd.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-"""
-
-from setuptools import setup, __version__
-from pkg_resources import parse_version
-
-minimum_version = parse_version('30.4.0')
-
-if parse_version(__version__) < minimum_version:
-    raise RuntimeError("Package setuptools must be at least version {}".format(minimum_version))
-
-setup(
-    packages=['drv8830'],
-    install_requires=['setuptools>={}'.format(minimum_version)]
-)
```

### Comparing `drv8830-0.0.1/drv8830/__init__.py` & `drv8830-1.0.0/drv8830/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from i2cdevice import Device, Register, BitField
+from i2cdevice import BitField, Device, Register
 from i2cdevice.adapter import Adapter, LookupAdapter
 
-
-__version__ = '0.0.1'
+__version__ = '1.0.0'
 
 I2C_ADDR1 = 0x60  # Default, both select jumpers bridged (not cut)
 I2C_ADDR2 = 0x61  # Cut A0
 I2C_ADDR3 = 0x63  # Cut A1
 I2C_ADDR4 = 0x64  # Cut A0 and A1
 
 
@@ -60,33 +59,47 @@
         self._drv8830.select_address(self._i2c_addr)
 
     def select_i2c_address(self, i2c_addr):
         self._i2c_addr = i2c_addr
         self._drv8830.select_address(self._i2c_addr)
 
     def set_outputs(self, out1, out2):
+        """Set the individual driver outputs.
+
+        Possible values are 1 (on) and 0 (off) with the following valid permutations:
+
+        * 1 1 - brake
+        * 0 0 - coast
+        * 1 0 - forward
+        * 0 1 - reverse
+
+        """
         self._drv8830.set('CONTROL', out1=out1, out2=out2)
 
     def brake(self):
+        """Set the driver outputs to braking mode."""
         self.set_direction('brake')
 
     def coast(self):
+        """Set the driver outputs to coasting mode."""
         self.set_direction('coast')
 
     def forward(self):
+        """Set the driver outputs to forward."""
         self.set_direction('forward')
 
     def reverse(self):
+        """Set the driver outputs to reverse."""
         self.set_direction('reverse')
 
     def set_direction(self, direction):
         """Set the motor driver direction.
 
         Basically does the same thing as set_outputs, but takes
-        a string name for directione, one of: coast, reverse,
+        a string name for direction, one of: coast, reverse,
         forward or brake.
 
         :param direction: string name of direction: coast, reverse, forward or brake
 
         """
         self._drv8830.set('CONTROL', direction=direction)
 
@@ -97,14 +110,15 @@
 
         :param voltage: from 0.48v to 5.06v
 
         """
         self._drv8830.set('CONTROL', voltage=voltage)
 
     def get_voltage(self):
+        """Return the currently set motor voltage."""
         return self._drv8830.get('CONTROL').voltage
 
     def get_fault(self):
         """Get motor driver fault information.
 
         Returns a namedtuple of the fault flags:
```

