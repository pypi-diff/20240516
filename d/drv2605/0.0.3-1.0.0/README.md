# Comparing `tmp/drv2605-0.0.3.tar.gz` & `tmp/drv2605-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drv2605-0.0.3.tar", last modified: Tue Nov  5 15:31:39 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `drv2605-0.0.3.tar` & `drv2605-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-11-05 15:31:39.000000 drv2605-0.0.3/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-11-05 15:31:39.000000 drv2605-0.0.3/drv2605.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)       23 2019-11-05 15:31:39.000000 drv2605-0.0.3/drv2605.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      241 2019-11-05 15:31:39.000000 drv2605-0.0.3/drv2605.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1983 2019-11-05 15:31:39.000000 drv2605-0.0.3/drv2605.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2019-11-05 15:31:39.000000 drv2605-0.0.3/drv2605.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2019-11-05 15:31:39.000000 drv2605-0.0.3/drv2605.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      109 2019-11-05 15:21:58.000000 drv2605-0.0.3/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)      826 2019-11-05 15:21:58.000000 drv2605-0.0.3/README.rst
--rw-r--r--   0 pi        (1000) pi        (1000)     1983 2019-11-05 15:31:39.000000 drv2605-0.0.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2019-11-05 15:21:58.000000 drv2605-0.0.3/LICENSE.txt
--rwxr-xr-x   0 pi        (1000) pi        (1000)     2109 2019-11-05 15:29:25.000000 drv2605-0.0.3/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)      127 2019-11-05 15:30:34.000000 drv2605-0.0.3/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      134 2019-11-05 15:31:39.000000 drv2605-0.0.3/setup.cfg
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-11-05 15:31:39.000000 drv2605-0.0.3/drv2605/
--rw-r--r--   0 pi        (1000) pi        (1000)    15508 2019-11-05 15:30:57.000000 drv2605-0.0.3/drv2605/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 drv2605-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 drv2605-1.0.0/Makefile
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 drv2605-1.0.0/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 drv2605-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 drv2605-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 drv2605-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 drv2605-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 drv2605-1.0.0/uninstall.sh
+-rw-r--r--   0        0        0    15515 2020-02-02 00:00:00.000000 drv2605-1.0.0/drv2605/__init__.py
+-rwxr-xr-x   0        0        0     1521 2020-02-02 00:00:00.000000 drv2605-1.0.0/examples/haptic-trackball.py
+-rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 drv2605-1.0.0/examples/tap-tap-tap.py
+-rwxr-xr-x   0        0        0     1544 2020-02-02 00:00:00.000000 drv2605-1.0.0/examples/test-pattern.py
+-rwxr-xr-x   0        0        0     1803 2020-02-02 00:00:00.000000 drv2605-1.0.0/examples/test-waveform.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 drv2605-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 drv2605-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 drv2605-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 drv2605-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 drv2605-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `drv2605-0.0.3/LICENSE.txt` & `drv2605-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drv2605-0.0.3/drv2605/__init__.py` & `drv2605-1.0.0/drv2605/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import time
 import math
-import smbus
-from i2cdevice import Device, Register, BitField
+import time
+
+from i2cdevice import BitField, Device, Register
 from i2cdevice.adapter import Adapter, LookupAdapter
 
-__version__ = '0.0.3'
+__version__ = '1.0.0'
 
 DRV2605_ADDR = 0x5a
 
 
 class WaitTimeAdapter(Adapter):
     def _encode(self, value):
         return (value // 10) | 0x80
@@ -313,15 +313,16 @@
 
 
 if __name__ == "__main__":
     import sys
 
     enable_calibration = True
 
-    bus = smbus.SMBus(1)
+    import smbus2
+    bus = smbus2.SMBus(1)
     drv2605 = DRV2605(i2c_dev=bus)
     drv2605.reset()
 
     drv2605.set_feedback_mode('LRA')
     drv2605.set_library('LRA')
 
     if enable_calibration:
```

