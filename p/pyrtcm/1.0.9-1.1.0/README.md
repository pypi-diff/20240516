# Comparing `tmp/pyrtcm-1.0.9.tar.gz` & `tmp/pyrtcm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtcm-1.0.9.tar", last modified: Tue Jun  6 06:36:03 2023, max compression
+gzip compressed data, was "pyrtcm-1.1.0.tar", last modified: Thu May 16 08:57:22 2024, max compression
```

## Comparing `pyrtcm-1.0.9.tar` & `pyrtcm-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:36:03.164466 pyrtcm-1.0.9/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2023-02-07 10:54:51.000000 pyrtcm-1.0.9/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2023-02-07 10:54:51.000000 pyrtcm-1.0.9/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    16256 2023-06-06 06:36:03.164292 pyrtcm-1.0.9/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    13216 2023-06-06 06:33:44.000000 pyrtcm-1.0.9/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2416 2023-06-06 06:33:44.000000 pyrtcm-1.0.9/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-06-06 06:36:03.164513 pyrtcm-1.0.9/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:36:03.160541 pyrtcm-1.0.9/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:36:03.162568 pyrtcm-1.0.9/src/pyrtcm/
--rw-r--r--   0 steve      (501) staff       (20)      600 2023-06-06 06:33:44.000000 pyrtcm-1.0.9/src/pyrtcm/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2023-06-06 06:33:44.000000 pyrtcm-1.0.9/src/pyrtcm/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      734 2023-03-23 18:20:24.000000 pyrtcm-1.0.9/src/pyrtcm/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)    10588 2023-06-06 06:33:44.000000 pyrtcm-1.0.9/src/pyrtcm/rtcmhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    11393 2023-06-06 06:33:44.000000 pyrtcm-1.0.9/src/pyrtcm/rtcmmessage.py
--rw-r--r--   0 steve      (501) staff       (20)    10051 2023-06-06 06:33:44.000000 pyrtcm-1.0.9/src/pyrtcm/rtcmreader.py
--rw-r--r--   0 steve      (501) staff       (20)     5924 2023-03-23 18:20:24.000000 pyrtcm-1.0.9/src/pyrtcm/rtcmtables.py
--rw-r--r--   0 steve      (501) staff       (20)    34696 2023-03-27 07:03:50.000000 pyrtcm-1.0.9/src/pyrtcm/rtcmtypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    47149 2023-06-06 06:33:44.000000 pyrtcm-1.0.9/src/pyrtcm/rtcmtypes_get.py
--rw-r--r--   0 steve      (501) staff       (20)     2465 2023-03-23 18:20:24.000000 pyrtcm-1.0.9/src/pyrtcm/socket_stream.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:36:03.163319 pyrtcm-1.0.9/src/pyrtcm.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    16256 2023-06-06 06:36:03.000000 pyrtcm-1.0.9/src/pyrtcm.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      587 2023-06-06 06:36:03.000000 pyrtcm-1.0.9/src/pyrtcm.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-06-06 06:36:03.000000 pyrtcm-1.0.9/src/pyrtcm.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      113 2023-06-06 06:36:03.000000 pyrtcm-1.0.9/src/pyrtcm.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        7 2023-06-06 06:36:03.000000 pyrtcm-1.0.9/src/pyrtcm.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-06 06:36:03.163967 pyrtcm-1.0.9/tests/
--rw-r--r--   0 steve      (501) staff       (20)      996 2023-03-23 18:20:24.000000 pyrtcm-1.0.9/tests/test_definitions.py
--rw-r--r--   0 steve      (501) staff       (20)     5980 2023-03-27 17:42:09.000000 pyrtcm-1.0.9/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     8397 2023-04-03 09:09:35.000000 pyrtcm-1.0.9/tests/test_specialcases.py
--rw-r--r--   0 steve      (501) staff       (20)     7066 2023-03-27 17:33:30.000000 pyrtcm-1.0.9/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)    69287 2023-03-27 17:27:10.000000 pyrtcm-1.0.9/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.851837 pyrtcm-1.1.0/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    17908 2024-05-16 08:57:22.851451 pyrtcm-1.1.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    14397 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2426 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-16 08:57:22.851888 pyrtcm-1.1.0/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.845620 pyrtcm-1.1.0/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.848469 pyrtcm-1.1.0/src/pyrtcm/
+-rw-r--r--   0 steve      (501) staff       (20)      600 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/src/pyrtcm/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      734 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/src/pyrtcm/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     8961 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    14502 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)     9459 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmreader.py
+-rw-r--r--   0 steve      (501) staff       (20)     3564 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmtables.py
+-rw-r--r--   0 steve      (501) staff       (20)    41265 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmtypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    65495 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmtypes_get.py
+-rw-r--r--   0 steve      (501) staff       (20)     2508 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/src/pyrtcm/socket_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.850456 pyrtcm-1.1.0/src/pyrtcm.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    17908 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      560 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      113 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        7 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.850023 pyrtcm-1.1.0/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     1008 2024-05-08 07:05:03.000000 pyrtcm-1.1.0/tests/test_definitions.py
+-rw-r--r--   0 steve      (501) staff       (20)     6032 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)    24603 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)   195338 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/tests/test_stream.py
```

### Comparing `pyrtcm-1.0.9/LICENSE` & `pyrtcm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtcm-1.0.9/PKG-INFO` & `pyrtcm-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtcm
-Version: 1.0.9
+Version: 1.1.0
 Summary: RTCM3 protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2022, SEMU Consulting
         All rights reserved.
@@ -45,23 +45,35 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Provides-Extra: deploy
+Requires-Dist: build; extra == "deploy"
+Requires-Dist: pip; extra == "deploy"
+Requires-Dist: setuptools>=66.0; extra == "deploy"
+Requires-Dist: wheel; extra == "deploy"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: bandit; extra == "test"
+Requires-Dist: black; extra == "test"
+Requires-Dist: pylint; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: Sphinx; extra == "test"
+Requires-Dist: sphinx-rtd-theme; extra == "test"
 
 # pyrtcm
 
 [Current Status](#currentstatus) |
 [Installation](#installation) |
 [Reading](#reading) |
 [Parsing](#parsing) |
@@ -78,66 +90,75 @@
 [RTCM STANDARD 10403.n DIFFERENTIAL GNSS (GLOBAL NAVIGATION SATELLITE SYSTEMS) SERVICES – VERSION 3](https://rtcm.myshopify.com/collections/differential-global-navigation-satellite-dgnss-standards/products/rtcm-10403-3-differential-gnss-global-navigation-satellite-systems-services-version-3-amendment-2-may-20-2021).
 
 The `pyrtcm` homepage is located at [https://github.com/semuconsulting/pyrtcm](https://github.com/semuconsulting/pyrtcm).
 
 This is an independent project and we have no affiliation whatsoever with the Radio Technical Commission for Maritime Services.
 
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy; and UBX &copy; (u-blox) GNSS/GPS messages:
-- [pyubx2](http://github.com/semuconsulting/pyubx2) (**FYI** installing `pyubx2` via pip also installs `pynmeagps` and `pyrtcm`)
+- [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 
 ## <a name="currentstatus">Current Status</a>
 
 ![Status](https://img.shields.io/pypi/status/pyrtcm)
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyrtcm?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyrtcm/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyrtcm)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyrtcm)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyrtcm)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyrtcm.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyrtcm)
 
-Parses RTCM3 messages into their constituent data fields. Refer to the `RTCM_MSGIDS` dictionary in [`rtcmtypes_core.py`](https://github.com/semuconsulting/pyrtcm/blob/main/src/pyrtcm/rtcmtypes_core.py) for a list of message types currently implemented. Additional message types can be readily added - see [Extensibility](#extensibility)).
+Parses RTCM3 messages into their constituent data fields - `DF002`, `DF003`, etc. Refer to the `RTCM_MSGIDS` dictionary in [`rtcmtypes_core.py`](https://github.com/semuconsulting/pyrtcm/blob/main/src/pyrtcm/rtcmtypes_core.py#L695) for a list of message types currently implemented. Additional message types can be readily added - see [Extensibility](#extensibility).
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyrtcm](https://www.semuconsulting.com/pyrtcm).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyrtcm/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyrtcm/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyrtcm/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, post a message to one of the [pyrtcm Discussions](https://github.com/semuconsulting/pyrtcm/discussions) channels.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyrtcm` is compatible with Python >=3.8 and has no third-party library dependencies.
 
-In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
-`python3` or `pip3`, depending on your particular environment.
+In the following, `python3` & `pip` refer to the Python 3 executables. You may need to type 
+`python` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pyrtcm.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pyrtcm.svg?style=flat)](https://pypi.org/project/pyrtcm/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pyrtcm.svg?style=flat)
 
 The recommended way to install the latest version of `pyrtcm` is with
 [pip](http://pypi.python.org/pypi/pip/):
 
 ```shell
-python -m pip install --upgrade pyrtcm
+python3 -m pip install --upgrade pyrtcm
 ```
 
 If required, `pyrtcm` can also be installed into a virtual environment, e.g.:
 
 ```shell
 python3 -m pip install --user --upgrade virtualenv
 python3 -m virtualenv env
 source env/bin/activate (or env\Scripts\activate on Windows)
 (env) python3 -m pip install --upgrade pyrtcm
 ...
 deactivate
 ```
 
+For [Conda](https://docs.conda.io/en/latest/) users, `pyrtcm` is also available from [conda-forge](https://github.com/conda-forge/pyrtcm-feedstock):
+
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyrtcm/badges/version.svg)](https://anaconda.org/conda-forge/pyrtcm)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyrtcm/badges/downloads.svg)](https://anaconda.org/conda-forge/pyrtcm)
+
+```shell
+conda install -c conda-forge pyrtcm
+```
+
 ---
 ## <a name="reading">Reading (Streaming)</a>
 
 ```
 class pyrtcm.rtcmreader.RTCMReader(stream, **kwargs)
 ```
 
@@ -145,147 +166,173 @@
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyrtcm` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual RTCM messages can then be read using the `RTCMReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `RTCMMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `RTCMReader` also implements an iterator.
 
 Example -  Serial input:
 ```python
->>> from serial import Serial
->>> from pyrtcm import RTCMReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>> rtr = RTCMReader(stream)
->>> (raw_data, parsed_data) = rtr.read()
->>> print(parsed_data)
- <RTCM(1077, DF002=1077, DF003=0, GNSSEpoch=204137001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=760738918298550272, NSat=10, DF395=1073807360, NSig=2, DF396=1044459, DF397_01(005)=75, DF397_02(007)=75, DF397_03(009)=81, ..., DF404_19(030,1C)=0.0, DF404_20(030,2L)=0.0)>,
+from serial import Serial
+from pyrtcm import RTCMReader
+with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
+  rtr = RTCMReader(stream)
+  raw_data, parsed_data = rtr.read()
+  print(parsed_data)
+```
+```
+"<RTCM(1077, DF002=1077, DF003=0, DF004=204137001, DF393=1, DF409=0, DF001_7=0, ..., DF404_15=-9556, DF404_16=-2148, DF404_17=-2174)>",     
 ```
 
 Example - File input (using iterator).
 ```python
->>> from pyrtcm import RTCMReader
->>> stream = open('rtcmdata.log', 'rb')
->>> rtr = RTCMReader(stream)
->>> for (raw_data, parsed_data) in rtr: print(parsed_data)
-...
+from pyrtcm import RTCMReader
+with open('rtcmdata.log', 'rb') as stream:
+  rtr = RTCMReader(stream)
+  for raw_data, parsed_data in rtr:
+    print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
->>> import socket
->>> from pyrtcm import RTCMReader
->>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
->>> stream.connect(("localhost", 50007))
->>> rtr = RTCMReader(stream)
->>> for (raw_data, parsed_data) in rtr: print(parsed_data)
+import socket
+from pyrtcm import RTCMReader
+with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as stream:
+  stream.connect(("localhost", 50007))
+  rtr = RTCMReader(stream)
+  for raw_data, parsed_data in rtr:
+    print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual RTCM messages using the static `RTCMReader.parse(data)` function, which takes a bytes array containing a binary RTCM message and returns a `RTCMMessage` object.
 
 **NB:** Once instantiated, an `RTCMMessage` object is immutable.
 
 Example:
 ```python
->>> from pyrtcm import RTCMReader
->>> msg = RTCMReader.parse(b"\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7")
->>> print(msg)
+from pyrtcm import RTCMReader
+msg = RTCMReader.parse(b"\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7")
+print(msg)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
 ```
 
-The `RTCMMessage` object exposes different public attributes depending on its message type or 'identity'. Attributes are defined as data fields ("DF002", "DF003", etc.) e.g. the `1005` message contains the following data fields:
+The `RTCMMessage` object exposes different public attributes depending on its message type or 'identity'. Attributes are defined as data fields (`DF002`, `DF003`, etc.) e.g. the `1097` multiple signal message (MSM) contains the following data fields:
 
 ```python
->>> print(msg)
-<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
->>> msg.identity
-'1005'
->>> msg.DF024
-1
+print(msg)
+print(msg.identity)
+print(msg.DF248)
+print(msg.DF404_07)
+```
+```
+"<RTCM(1097, DF002=1097, DF003=0, DF248=204137001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=216181732825628672, NSat=5, DF395=1073872896, NSig=2, DF396=1023, NCell=10, PRN_01=007, PRN_02=008, PRN_03=021, PRN_04=027, ..., DF404_07=5534, DF404_08=5545, DF404_09=-7726, DF404_10=-7733)>",             
+'1097'
+204137001
+5534
 ```
 
+Attributes within repeating groups are parsed with a two-digit suffix (`DF419_01`, `DF419_02`, etc. See [example below](#iterating) for an illustration of how to iterate through grouped attributes).
+
 Helper methods are available to interpret the individual datafields:
 
 ```python
->>> from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
->>> dfname = "DF012"
->>> RTCM_DATA_FIELDS[dfname]
+from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
+dfname = "DF012"
+print(RTCM_DATA_FIELDS[dfname])
+print(datasiz(dfname))
+print(datascale(dfname))
+print(datadesc(dfname))
+```
+```
 (INT20, 0.0001, "GPS L1 PhaseRange - L1 Pseudorange")
->>> datasiz(dfname) # size in bits
 20
->>> datascale(dfname) # scaling factor
 0.0001
->>> datadesc(dfname) # description
 'GPS L1 PhaseRange - L1 Pseudorange'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
-Attributes within repeating groups are parsed with a two-digit suffix ("DF030_01", "DF030_02", etc.). 
+#### <a name="iterating">Iterating Through Group Attributes</a>
 
-**Tip:** To iterate through a repeating group of attributes (*e.g., DF406 (GNSS signal fine PhaseRange)*) as a list, the following construct can be used:
+To iterate through a group of one or more repeating attributes in a given `RTCMMessage` object, the following construct can be used (in this illustration, repeating attributes CELLPRN, CELLSIG, DF405, DF406, DF407, DF408, DF420 and DF404 are extracted from an MSM 1077 message `msg` and collated in the array `msmarray`):
 
+```python
+msmarray = []
+for i in range(msg.NCell): # msg = MSM 1077, number of cells = NCell
+  vals = []
+  for attr in ("CELLPRN", "CELLSIG", "DF405", "DF406", "DF407", "DF408", "DF420", "DF404"):
+    val = getattr(msg, f"{attr}_{i+1:02d}")
+    vals.append(val)
+  msmarray.append(vals)
+print(msmarray)
 ```
-df406group = [] # list of DF406 ((GNSS signal fine PhaseRange) values from repeating group in MSM 1077 message
-for i in range(msg.NCell):
-    df406 = getattr(msg, f"DF406_{i+1:02}")
-    df406group.append(df406)
+```shell
+[['005', '1C', 0.00014309026300907135, 0.00014193402603268623, 341, 45.0, 0, -0.9231], ..., ['030', '2L', -0.00030865520238876343, -0.00030898721888661385, 341, 41.0, 0, -0.2174]]
 ```
 
-Attributes within MSM NSAT and NCELL repeating groups can optionally be labelled with their corresponding satellite PRN and signal ID when the `__str__()` method is invoked, by setting the keyword argument `labelmsm` to True (e.g. `DF405_10(014,2C)` signifies that the 10th item in the DF405 group refers to satellite PRN 014, signal ID 2C).
+The following dedicated helper methods are available to parse selected RTCM3 message types into a series of iterable data arrays:
+- `parse_msm` - for MSM message types (e.g. 1077, 1125, etc.).
+- `parse_4076_201` - for 4076_201 SSR (harmonic coefficients) message types.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyrtcm.rtcmmessage.RTCMMessage(**kwargs)
 ```
 
 You can create an `RTCMMessage` object by calling the constructor with the following keyword arguments:
 1. payload as bytes
 
 Example:
 
 ```python
->>> from pyrtcm import RTCMMessage
->>> msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
->>> print(msg)
+from pyrtcm import RTCMMessage
+msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
+print(msg)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `RTCMMessage` class implements a `serialize()` method to convert a `RTCMMessage` object to a bytes array suitable for writing to an output stream.
 
 e.g. to create and send a `1005` message type:
 
 ```python
->>> from serial import Serial
->>> serialOut = Serial('COM7', 38400, timeout=5)
->>> from pyrtcm import RTCMMessage
->>> msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
->>> print(msg)
+from serial import Serial
+from pyrtcm import RTCMMessage
+serialOut = Serial('COM7', 38400, timeout=5)
+msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
+print(msg)
+output = msg.serialize()
+print(output)
+serialOut.write(output)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
->>> output = msg.serialize()
->>> output
 b'\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7'
->>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
-1. `rtcmserial.py` - illustrates how to stream RTCM data from serial/UART port.
+1. `rtcmpoller.py` - illustrates how to read and display RTCM messages 'concurrently' with other tasks using threads and queues. This represents a useful generic pattern for many end user applications.
 1. `rtcmfile.py` - illustrates how to stream RTCM data from binary log file.
-1. `rtcmsocket.py` illustrates how to implement a TCP Socket reader for RTCM messages using RTCMReader iterator functionality.
-1. `rtcmbuild.py` - illustrates how to construct RTCM payload from constituent datafields.
-1. `ntripclient.py` - illustrates a simple [NTRIP](https://en.wikipedia.org/wiki/Networked_Transport_of_RTCM_via_Internet_Protocol) client using pyrtcm to parse the RTCM3 output.
+1. `rtcmsocket.py` - illustrates how to implement a TCP Socket reader for RTCM messages using RTCMReader iterator functionality.
+1. `msmparser.py` - illustrates how to parse RTCM3 MSM (multiple signal messages) into a series of iterable data arrays keyed on satellite PRN and signal ID.
+1. `rtcm_ntrip_client.py` - illustrates a simple [NTRIP](https://en.wikipedia.org/wiki/Networked_Transport_of_RTCM_via_Internet_Protocol) client using pyrtcm to parse the RTCM3 output.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
 The RTCM protocol is principally defined in the modules `rtcmtypes_core.py` and `rtcmtypes_get.py` as a series of dictionaries. RTCM uses a series of pre-defined data fields ("DF002", DF003" etc.), each of which has a designated data type (UINT32, etc.). Message payload definitions must conform to the following rules:
 
 ```
@@ -314,15 +361,15 @@
 ```
 gnssdump -h
 ```
 
 ---
 ## <a name="gui">Graphical Client</a>
 
-A python/tkinter graphical GPS client which supports NMEA, UBX and RTCM3 protocols is available at: 
+A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3, NTRIP and SPARTN protocols is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
 
 ---
 ## <a name="author">Author & License Information</a>
 
 semuadmin@semuconsulting.com
```

### Comparing `pyrtcm-1.0.9/README.md` & `pyrtcm-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,66 +17,75 @@
 [RTCM STANDARD 10403.n DIFFERENTIAL GNSS (GLOBAL NAVIGATION SATELLITE SYSTEMS) SERVICES – VERSION 3](https://rtcm.myshopify.com/collections/differential-global-navigation-satellite-dgnss-standards/products/rtcm-10403-3-differential-gnss-global-navigation-satellite-systems-services-version-3-amendment-2-may-20-2021).
 
 The `pyrtcm` homepage is located at [https://github.com/semuconsulting/pyrtcm](https://github.com/semuconsulting/pyrtcm).
 
 This is an independent project and we have no affiliation whatsoever with the Radio Technical Commission for Maritime Services.
 
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy; and UBX &copy; (u-blox) GNSS/GPS messages:
-- [pyubx2](http://github.com/semuconsulting/pyubx2) (**FYI** installing `pyubx2` via pip also installs `pynmeagps` and `pyrtcm`)
+- [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 
 ## <a name="currentstatus">Current Status</a>
 
 ![Status](https://img.shields.io/pypi/status/pyrtcm)
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyrtcm?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyrtcm/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyrtcm)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyrtcm)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyrtcm)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyrtcm.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyrtcm)
 
-Parses RTCM3 messages into their constituent data fields. Refer to the `RTCM_MSGIDS` dictionary in [`rtcmtypes_core.py`](https://github.com/semuconsulting/pyrtcm/blob/main/src/pyrtcm/rtcmtypes_core.py) for a list of message types currently implemented. Additional message types can be readily added - see [Extensibility](#extensibility)).
+Parses RTCM3 messages into their constituent data fields - `DF002`, `DF003`, etc. Refer to the `RTCM_MSGIDS` dictionary in [`rtcmtypes_core.py`](https://github.com/semuconsulting/pyrtcm/blob/main/src/pyrtcm/rtcmtypes_core.py#L695) for a list of message types currently implemented. Additional message types can be readily added - see [Extensibility](#extensibility).
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyrtcm](https://www.semuconsulting.com/pyrtcm).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyrtcm/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyrtcm/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyrtcm/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, post a message to one of the [pyrtcm Discussions](https://github.com/semuconsulting/pyrtcm/discussions) channels.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyrtcm` is compatible with Python >=3.8 and has no third-party library dependencies.
 
-In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
-`python3` or `pip3`, depending on your particular environment.
+In the following, `python3` & `pip` refer to the Python 3 executables. You may need to type 
+`python` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pyrtcm.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pyrtcm.svg?style=flat)](https://pypi.org/project/pyrtcm/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pyrtcm.svg?style=flat)
 
 The recommended way to install the latest version of `pyrtcm` is with
 [pip](http://pypi.python.org/pypi/pip/):
 
 ```shell
-python -m pip install --upgrade pyrtcm
+python3 -m pip install --upgrade pyrtcm
 ```
 
 If required, `pyrtcm` can also be installed into a virtual environment, e.g.:
 
 ```shell
 python3 -m pip install --user --upgrade virtualenv
 python3 -m virtualenv env
 source env/bin/activate (or env\Scripts\activate on Windows)
 (env) python3 -m pip install --upgrade pyrtcm
 ...
 deactivate
 ```
 
+For [Conda](https://docs.conda.io/en/latest/) users, `pyrtcm` is also available from [conda-forge](https://github.com/conda-forge/pyrtcm-feedstock):
+
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyrtcm/badges/version.svg)](https://anaconda.org/conda-forge/pyrtcm)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyrtcm/badges/downloads.svg)](https://anaconda.org/conda-forge/pyrtcm)
+
+```shell
+conda install -c conda-forge pyrtcm
+```
+
 ---
 ## <a name="reading">Reading (Streaming)</a>
 
 ```
 class pyrtcm.rtcmreader.RTCMReader(stream, **kwargs)
 ```
 
@@ -84,147 +93,173 @@
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyrtcm` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual RTCM messages can then be read using the `RTCMReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `RTCMMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `RTCMReader` also implements an iterator.
 
 Example -  Serial input:
 ```python
->>> from serial import Serial
->>> from pyrtcm import RTCMReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>> rtr = RTCMReader(stream)
->>> (raw_data, parsed_data) = rtr.read()
->>> print(parsed_data)
- <RTCM(1077, DF002=1077, DF003=0, GNSSEpoch=204137001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=760738918298550272, NSat=10, DF395=1073807360, NSig=2, DF396=1044459, DF397_01(005)=75, DF397_02(007)=75, DF397_03(009)=81, ..., DF404_19(030,1C)=0.0, DF404_20(030,2L)=0.0)>,
+from serial import Serial
+from pyrtcm import RTCMReader
+with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
+  rtr = RTCMReader(stream)
+  raw_data, parsed_data = rtr.read()
+  print(parsed_data)
+```
+```
+"<RTCM(1077, DF002=1077, DF003=0, DF004=204137001, DF393=1, DF409=0, DF001_7=0, ..., DF404_15=-9556, DF404_16=-2148, DF404_17=-2174)>",     
 ```
 
 Example - File input (using iterator).
 ```python
->>> from pyrtcm import RTCMReader
->>> stream = open('rtcmdata.log', 'rb')
->>> rtr = RTCMReader(stream)
->>> for (raw_data, parsed_data) in rtr: print(parsed_data)
-...
+from pyrtcm import RTCMReader
+with open('rtcmdata.log', 'rb') as stream:
+  rtr = RTCMReader(stream)
+  for raw_data, parsed_data in rtr:
+    print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
->>> import socket
->>> from pyrtcm import RTCMReader
->>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
->>> stream.connect(("localhost", 50007))
->>> rtr = RTCMReader(stream)
->>> for (raw_data, parsed_data) in rtr: print(parsed_data)
+import socket
+from pyrtcm import RTCMReader
+with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as stream:
+  stream.connect(("localhost", 50007))
+  rtr = RTCMReader(stream)
+  for raw_data, parsed_data in rtr:
+    print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual RTCM messages using the static `RTCMReader.parse(data)` function, which takes a bytes array containing a binary RTCM message and returns a `RTCMMessage` object.
 
 **NB:** Once instantiated, an `RTCMMessage` object is immutable.
 
 Example:
 ```python
->>> from pyrtcm import RTCMReader
->>> msg = RTCMReader.parse(b"\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7")
->>> print(msg)
+from pyrtcm import RTCMReader
+msg = RTCMReader.parse(b"\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7")
+print(msg)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
 ```
 
-The `RTCMMessage` object exposes different public attributes depending on its message type or 'identity'. Attributes are defined as data fields ("DF002", "DF003", etc.) e.g. the `1005` message contains the following data fields:
+The `RTCMMessage` object exposes different public attributes depending on its message type or 'identity'. Attributes are defined as data fields (`DF002`, `DF003`, etc.) e.g. the `1097` multiple signal message (MSM) contains the following data fields:
 
 ```python
->>> print(msg)
-<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
->>> msg.identity
-'1005'
->>> msg.DF024
-1
+print(msg)
+print(msg.identity)
+print(msg.DF248)
+print(msg.DF404_07)
 ```
+```
+"<RTCM(1097, DF002=1097, DF003=0, DF248=204137001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=216181732825628672, NSat=5, DF395=1073872896, NSig=2, DF396=1023, NCell=10, PRN_01=007, PRN_02=008, PRN_03=021, PRN_04=027, ..., DF404_07=5534, DF404_08=5545, DF404_09=-7726, DF404_10=-7733)>",             
+'1097'
+204137001
+5534
+```
+
+Attributes within repeating groups are parsed with a two-digit suffix (`DF419_01`, `DF419_02`, etc. See [example below](#iterating) for an illustration of how to iterate through grouped attributes).
 
 Helper methods are available to interpret the individual datafields:
 
 ```python
->>> from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
->>> dfname = "DF012"
->>> RTCM_DATA_FIELDS[dfname]
+from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
+dfname = "DF012"
+print(RTCM_DATA_FIELDS[dfname])
+print(datasiz(dfname))
+print(datascale(dfname))
+print(datadesc(dfname))
+```
+```
 (INT20, 0.0001, "GPS L1 PhaseRange - L1 Pseudorange")
->>> datasiz(dfname) # size in bits
 20
->>> datascale(dfname) # scaling factor
 0.0001
->>> datadesc(dfname) # description
 'GPS L1 PhaseRange - L1 Pseudorange'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
-Attributes within repeating groups are parsed with a two-digit suffix ("DF030_01", "DF030_02", etc.). 
+#### <a name="iterating">Iterating Through Group Attributes</a>
 
-**Tip:** To iterate through a repeating group of attributes (*e.g., DF406 (GNSS signal fine PhaseRange)*) as a list, the following construct can be used:
+To iterate through a group of one or more repeating attributes in a given `RTCMMessage` object, the following construct can be used (in this illustration, repeating attributes CELLPRN, CELLSIG, DF405, DF406, DF407, DF408, DF420 and DF404 are extracted from an MSM 1077 message `msg` and collated in the array `msmarray`):
 
+```python
+msmarray = []
+for i in range(msg.NCell): # msg = MSM 1077, number of cells = NCell
+  vals = []
+  for attr in ("CELLPRN", "CELLSIG", "DF405", "DF406", "DF407", "DF408", "DF420", "DF404"):
+    val = getattr(msg, f"{attr}_{i+1:02d}")
+    vals.append(val)
+  msmarray.append(vals)
+print(msmarray)
 ```
-df406group = [] # list of DF406 ((GNSS signal fine PhaseRange) values from repeating group in MSM 1077 message
-for i in range(msg.NCell):
-    df406 = getattr(msg, f"DF406_{i+1:02}")
-    df406group.append(df406)
+```shell
+[['005', '1C', 0.00014309026300907135, 0.00014193402603268623, 341, 45.0, 0, -0.9231], ..., ['030', '2L', -0.00030865520238876343, -0.00030898721888661385, 341, 41.0, 0, -0.2174]]
 ```
 
-Attributes within MSM NSAT and NCELL repeating groups can optionally be labelled with their corresponding satellite PRN and signal ID when the `__str__()` method is invoked, by setting the keyword argument `labelmsm` to True (e.g. `DF405_10(014,2C)` signifies that the 10th item in the DF405 group refers to satellite PRN 014, signal ID 2C).
+The following dedicated helper methods are available to parse selected RTCM3 message types into a series of iterable data arrays:
+- `parse_msm` - for MSM message types (e.g. 1077, 1125, etc.).
+- `parse_4076_201` - for 4076_201 SSR (harmonic coefficients) message types.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyrtcm.rtcmmessage.RTCMMessage(**kwargs)
 ```
 
 You can create an `RTCMMessage` object by calling the constructor with the following keyword arguments:
 1. payload as bytes
 
 Example:
 
 ```python
->>> from pyrtcm import RTCMMessage
->>> msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
->>> print(msg)
+from pyrtcm import RTCMMessage
+msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
+print(msg)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `RTCMMessage` class implements a `serialize()` method to convert a `RTCMMessage` object to a bytes array suitable for writing to an output stream.
 
 e.g. to create and send a `1005` message type:
 
 ```python
->>> from serial import Serial
->>> serialOut = Serial('COM7', 38400, timeout=5)
->>> from pyrtcm import RTCMMessage
->>> msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
->>> print(msg)
+from serial import Serial
+from pyrtcm import RTCMMessage
+serialOut = Serial('COM7', 38400, timeout=5)
+msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
+print(msg)
+output = msg.serialize()
+print(output)
+serialOut.write(output)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
->>> output = msg.serialize()
->>> output
 b'\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7'
->>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
-1. `rtcmserial.py` - illustrates how to stream RTCM data from serial/UART port.
+1. `rtcmpoller.py` - illustrates how to read and display RTCM messages 'concurrently' with other tasks using threads and queues. This represents a useful generic pattern for many end user applications.
 1. `rtcmfile.py` - illustrates how to stream RTCM data from binary log file.
-1. `rtcmsocket.py` illustrates how to implement a TCP Socket reader for RTCM messages using RTCMReader iterator functionality.
-1. `rtcmbuild.py` - illustrates how to construct RTCM payload from constituent datafields.
-1. `ntripclient.py` - illustrates a simple [NTRIP](https://en.wikipedia.org/wiki/Networked_Transport_of_RTCM_via_Internet_Protocol) client using pyrtcm to parse the RTCM3 output.
+1. `rtcmsocket.py` - illustrates how to implement a TCP Socket reader for RTCM messages using RTCMReader iterator functionality.
+1. `msmparser.py` - illustrates how to parse RTCM3 MSM (multiple signal messages) into a series of iterable data arrays keyed on satellite PRN and signal ID.
+1. `rtcm_ntrip_client.py` - illustrates a simple [NTRIP](https://en.wikipedia.org/wiki/Networked_Transport_of_RTCM_via_Internet_Protocol) client using pyrtcm to parse the RTCM3 output.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
 The RTCM protocol is principally defined in the modules `rtcmtypes_core.py` and `rtcmtypes_get.py` as a series of dictionaries. RTCM uses a series of pre-defined data fields ("DF002", DF003" etc.), each of which has a designated data type (UINT32, etc.). Message payload definitions must conform to the following rules:
 
 ```
@@ -253,15 +288,15 @@
 ```
 gnssdump -h
 ```
 
 ---
 ## <a name="gui">Graphical Client</a>
 
-A python/tkinter graphical GPS client which supports NMEA, UBX and RTCM3 protocols is available at: 
+A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3, NTRIP and SPARTN protocols is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
 
 ---
 ## <a name="author">Author & License Information</a>
 
 semuadmin@semuconsulting.com
```

### Comparing `pyrtcm-1.0.9/pyproject.toml` & `pyrtcm-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 [build-system]
 requires = ["setuptools>=66.0.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pyrtcm"
-authors = [
-    {name = "semuadmin", email = "semuadmin@semuconsulting.com"},
-]
-maintainers = [
-  {name = "semuadmin", email = "semuadmin@semuconsulting.com"}
-]
+authors = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
+maintainers = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 description = "RTCM3 protocol parser"
-version = "1.0.9"
-license = {file = "LICENSE"}
+version = "1.1.0"
+license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "Environment :: MacOS X",
     "Environment :: Win32 (MS Windows)",
@@ -26,36 +22,31 @@
     "Intended Audience :: Science/Research",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: BSD License",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: GIS",
-    ]
-
-dependencies = [
 ]
 
+dependencies = []
+
 [project.urls]
 homepage = "https://github.com/semuconsulting/pyrtcm"
 documentation = "https://www.semuconsulting.com/pyrtcm/"
 repository = "https://github.com/semuconsulting/pyrtcm"
 changelog = "https://github.com/semuconsulting/pyrtcm/blob/master/RELEASE_NOTES.md"
 
 [project.optional-dependencies]
-deploy = [
-    "build",
-    "pip",
-    "setuptools >= 66.0",
-    "wheel"
-]
+deploy = ["build", "pip", "setuptools >= 66.0", "wheel"]
 test = [
     "bandit",
     "black",
     "pylint",
     "pytest",
     "pytest-cov",
     "Sphinx",
@@ -90,12 +81,12 @@
     useless-suppression,
     deprecated-pragma,
     use-symbolic-message-instead,
 """
 
 [tool.pytest.ini_options]
 minversion = "7.0"
-addopts = "--cov --cov-report term-missing --cov-fail-under 95"
+addopts = "--cov --cov-report html --cov-fail-under 98"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `pyrtcm-1.0.9/src/pyrtcm/__init__.py` & `pyrtcm-1.1.0/src/pyrtcm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrtcm-1.0.9/src/pyrtcm/exceptions.py` & `pyrtcm-1.1.0/src/pyrtcm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyrtcm-1.0.9/src/pyrtcm/rtcmhelpers.py` & `pyrtcm-1.1.0/src/pyrtcm/rtcmhelpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,38 +4,18 @@
 
 Created on 14 Feb 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
 from datetime import datetime, timedelta
 
-from pyrtcm.exceptions import RTCMTypeError
-from pyrtcm.rtcmtables import (
-    BEIDOU_PRN_MAP,
-    BEIDOU_SIG_MAP,
-    GALILEO_PRN_MAP,
-    GALILEO_SIG_MAP,
-    GLONASS_PRN_MAP,
-    GLONASS_SIG_MAP,
-    GPS_PRN_MAP,
-    GPS_SIG_MAP,
-    IRNSS_PRN_MAP,
-    IRNSS_SIG_MAP,
-    QZSS_PRN_MAP,
-    QZSS_SIG_MAP,
-    SBAS_PRN_MAP,
-    SBAS_SIG_MAP,
-)
-from pyrtcm.rtcmtypes_core import RTCM_DATA_FIELDS, RTCM_MSGIDS
-
-SCALEDP = 8
+from pyrtcm.rtcmtypes_core import COEFFS, GNSSMAP, RTCM_DATA_FIELDS
 
 
 def att2idx(att: str) -> int:
     """
     Get integer index corresponding to grouped attribute.
 
     e.g. DF389_06 -> 6; DF406_103 -> 103
@@ -94,34 +74,19 @@
     if typ == "INT" and (bitfield & msb):  # 2's compliment -ve int
         val = val - (1 << siz)
     if typ in ("CHA", "UTF"):  # ASCII or UTF-8 character
         val = chr(val)
     # apply any scaling factor
     else:
         if scale not in (0, 1):
-            val = round(val * scale, SCALEDP)
+            val *= scale
 
     return val
 
 
-def num_setbits(val: int) -> int:
-    """
-    Get number of set bits in integer.
-
-    :param int val: integer value
-    :return: number of bits set
-    :rtype: int
-    """
-
-    i = 0
-    for x in bin(val)[2:]:
-        i += int(x)
-    return i
-
-
 def calc_crc24q(message: bytes) -> int:
     """
     Perform CRC24Q cyclic redundancy check.
 
     If the message includes the appended CRC bytes, the
     function will return 0 if the message is valid.
     If the message excludes the appended CRC bytes, the
@@ -129,22 +94,22 @@
 
     :param bytes message: message
     :return: CRC or 0
     :rtype: int
 
     """
 
-    POLY = 0x1864CFB
+    poly = 0x1864CFB
     crc = 0
     for octet in message:
         crc ^= octet << 16
         for _ in range(8):
             crc <<= 1
             if crc & 0x1000000:
-                crc ^= POLY
+                crc ^= poly
     return crc & 0xFFFFFF
 
 
 def crc2bytes(message: bytes) -> bytes:
     """
     Generate CRC as 3 bytes, suitable for
     constructing RTCM message transport.
@@ -287,139 +252,103 @@
         for col in range(0, colw, 4):
             hextbl += f"{rawl[col : col + 4]} "
         hextbl += f" | {bytes.fromhex(rawl)} |\n"
 
     return hextbl
 
 
-def sat2prn(msg: object) -> dict:
+def escapeall(val: bytes) -> str:
     """
-    Map MSM sat to satellite PRN for a given RTCM3 MSM message.
-
-    Returns a dict mapping the satellite PRN corresponding to each
-    item in the MSM NSAT repeating group e.g. DF397_01, DF397_02, etc.
+    Escape all byte characters e.g. b'\\\\x73' rather than b`s`
 
-    :param RTCMMessage msg: RTCM3 MSM message e.g. 1077
-    :return: dict of {cell: prn} values
-    :rtype: dict
-    :raises: RTCMTypeError if not MSM message type
+    :param bytes val: bytes
+    :return: string of escaped bytes
+    :rtype: str
     """
 
-    try:
-        prnmap, _ = id2prnsigmap(msg.identity)
-
-        sats = {}
-        nsat = 0
-        for idx in range(1, 65):
-            if msg.DF394 & 2 ** (64 - idx):
-                nsat += 1
-                sats[nsat] = prnmap[idx]
-
-        return sats
-
-    except (TypeError, KeyError, AttributeError) as err:
-        raise RTCMTypeError(
-            "Invalid RTCM3 message type - must be MSM message."
-        ) from err
+    return "b'{}'".format("".join(f"\\x{b:02x}" for b in val))
 
 
-def cell2prn(msg: object) -> dict:
+def parse_msm(msg: object) -> tuple:
     """
-    Map MSM cell to satellite PRN and signal ID for a given RTCM3 MSM message.
-
-    Returns a dict mapping the satellite PRN and signal ID corresponding to each
-    item in the MSM NCELL repeating group e.g. DF405_01, DF406_02, etc.
+    Parse individual MSM message into iterable data arrays.
 
-    DF394 bitmask indicates which satellites are present.
-    DF395 bitmask indicates which signals are present.
-    DF396 bitmask maps satellite to signal.
-
-    :param RTCMMessage msg: RTCM3 MSM message e.g. 1077
-    :return: dict of {cell: (prn, sig)} values
-    :rtype: dict
-    :raises: RTCMTypeError if not MSM message type
+    :param RTCMMessage msg: RTCM MSM Message
+    :return: tuple of (metadata, sat data array, cell data array)
+    :rtype: tuple
     """
 
-    try:
-        prnmap, sigmap = id2prnsigmap(msg.identity)
-
-        sats = []
-        nsat = 0
-        for idx in range(1, 65):
-            if msg.DF394 & 2 ** (64 - idx):
-                sats.append(prnmap[idx])
-                nsat += 1
-
-        sigs = []
-        nsig = 0
-        for idx in range(1, 33):
-            if msg.DF395 & 2 ** (32 - idx):
-                sigs.append(sigmap[idx])
-                nsig += 1
+    if not msg.ismsm:
+        return None
 
-        ncells = int(nsat * nsig)
+    meta = {}
+    gmap = GNSSMAP[msg.identity[0:3]]
+    meta["identity"] = msg.identity
+    meta["gnss"] = gmap[0]
+    meta["station"] = msg.DF003
+    meta["epoch"] = getattr(msg, gmap[1])
+    meta["sats"] = msg.NSat
+    meta["cells"] = msg.NCell
+    msmsats = []
+    for i in range(1, msg.NSat + 1):  # iterate through satellites
+        sats = {}
+        for attr in ["PRN", "DF397", "DF398", "DF399", "DF419", "ExtSatInfo"]:
+            if hasattr(msg, f"{attr}_{i:02d}"):
+                sats[attr] = getattr(msg, f"{attr}_{i:02d}")
+        msmsats.append(sats)
+    msmcells = []
+    for i in range(1, msg.NCell + 1):  # iterate through cells (satellite/signal)
         cells = {}
-        ncell = idx = 0
-        for sat in range(nsat):
-            for sig in range(nsig):
-                idx += 1
-                if msg.DF396 & 2 ** (ncells - idx):
-                    ncell += 1
-                    cells[ncell] = (sats[sat], sigs[sig])
+        for attr in [
+            "CELLPRN",
+            "CELLSIG",
+            "DF400",
+            "DF401",
+            "DF402",
+            "DF403",
+            "DF404",
+            "DF405",
+            "DF406",
+            "DF407",
+            "DF408",
+            "DF420",
+        ]:
+            if hasattr(msg, f"{attr}_{i:02d}"):
+                cells[attr] = getattr(msg, f"{attr}_{i:02d}")
+        msmcells.append(cells)
+
+    return (meta, msmsats, msmcells)
 
-        return cells
 
-    except (TypeError, KeyError, AttributeError) as err:
-        raise RTCMTypeError(
-            "Invalid RTCM3 message type - must be MSM message."
-        ) from err
-
-
-def id2prnsigmap(ident: str) -> tuple:
+def parse_4076_201(msg: object):
     """
-    Map RTCM3 message identity to MSM satellite PRN and signal ID maps.
+    Parse individual 4076_201 message into iterable data arrays.
 
-    :param str ident: RTCM3 MSM message identity e.g. "1077"
-    :return: tuple of (PRNMAP, SIGMAP)
-    :rtype: tuple
-    :raises: KeyError if ident unknown
+    :param RTCMMessage parsed: parsed 4076_201 message
+    :return: dict of {metadata, [cosine coefficients], [sine coefficients]} for each layer
+    :rtype: dict
     """
 
-    gnss = RTCM_MSGIDS[ident][0:3]
-    if gnss == "GPS":
-        PRNMAP = GPS_PRN_MAP
-        SIGMAP = GPS_SIG_MAP
-    elif gnss == "GLO":
-        PRNMAP = GLONASS_PRN_MAP
-        SIGMAP = GLONASS_SIG_MAP
-    elif gnss == "GAL":
-        PRNMAP = GALILEO_PRN_MAP
-        SIGMAP = GALILEO_SIG_MAP
-    elif gnss == "SBA":
-        PRNMAP = SBAS_PRN_MAP
-        SIGMAP = SBAS_SIG_MAP
-    elif gnss == "QZS":
-        PRNMAP = QZSS_PRN_MAP
-        SIGMAP = QZSS_SIG_MAP
-    elif gnss == "Bei":
-        PRNMAP = BEIDOU_PRN_MAP
-        SIGMAP = BEIDOU_SIG_MAP
-    elif gnss == "IRN":
-        PRNMAP = IRNSS_PRN_MAP
-        SIGMAP = IRNSS_SIG_MAP
-    else:
-        PRNMAP = None
-        SIGMAP = None
-
-    return (PRNMAP, SIGMAP)
-
+    if msg.identity != "4076_201":
+        return None
 
-def escapeall(val: bytes) -> str:
-    """
-    Escape all byte characters e.g. b'\\\\x73' rather than b`s`
+    hmc = {}
+    # for each ionospheric layer
+    for lyr in range(msg.IDF035 + 1):  # number of ionospheric layers
+        hmc[lyr] = {}
+        hmc[lyr]["Layer Height"] = getattr(msg, f"IDF036_{lyr+1:02d}")
+        # for each coefficient (cosine & sine)
+        for field, coeff in COEFFS.values():
+            hmc[lyr][coeff] = []
+            i = 0
+            eof = False
+            # for each coefficient value
+            while not eof:
+                try:
+                    hmc[lyr][coeff].append(
+                        getattr(msg, f"{field}_{lyr+1:02d}_{i+1:02d}")
+                    )
+                    i += 1
+                except AttributeError:
+                    eof = True
 
-    :param bytes val: bytes
-    :return: string of escaped bytes
-    :rtype: str
-    """
-
-    return "b'{}'".format("".join(f"\\x{b:02x}" for b in val))
+    return hmc
```

### Comparing `pyrtcm-1.0.9/src/pyrtcm/rtcmmessage.py` & `pyrtcm-1.1.0/src/pyrtcm/rtcmmessage.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,70 +3,61 @@
 
 Created on 14 Feb 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
-# pylint: disable=invalid-name
 
 import pyrtcm.exceptions as rte
 import pyrtcm.rtcmtypes_get as rtg
-from pyrtcm.rtcmhelpers import (
-    att2idx,
-    att2name,
-    attsiz,
-    bits2val,
-    cell2prn,
-    crc2bytes,
-    escapeall,
-    len2bytes,
-    num_setbits,
-    sat2prn,
-)
+from pyrtcm.rtcmhelpers import attsiz, bits2val, crc2bytes, escapeall, len2bytes
+from pyrtcm.rtcmtables import PRNSIGMAP
 from pyrtcm.rtcmtypes_core import (
-    ATT_NCELL,
-    ATT_NSAT,
-    BOOL_GROUPS,
+    CELPRN,
+    CELSIG,
+    NA,
     NCELL,
-    NL1CA,
-    NL1P,
-    NL2CA,
-    NL2P,
+    NHARMCOEFFC,
+    NHARMCOEFFS,
     NSAT,
     NSIG,
+    PRN,
     RTCM_DATA_FIELDS,
     RTCM_HDR,
     RTCM_MSGIDS,
 )
 
+BOOL = "B"
+
 
 class RTCMMessage:
     """RTCM Message Class."""
 
-    def __init__(self, **kwargs):
+    def __init__(self, payload: bytes = None, scaling: bool = True, labelmsm: int = 1):
         """Constructor.
 
-        :param bytes payload: (kwarg) message payload (mandatory)
-        :param bool scaling: (kwarg) whether to apply attribute scaling True/False (True)
-        :param bool labelmsm: (kwarg) whether to label MSM NSAT and NCELL attributes (True)
+        :param bytes payload: message payload (mandatory)
+        :param bool scaling: whether to apply attribute scaling True/False (True)
+        :param int labelmsm: MSM NSAT and NCELL attribute label (1 = RINEX, 2 = freq)
         :raises: RTCMMessageError
         """
-        # pylint: disable=unused-argument
 
         # object is mutable during initialisation only
         super().__setattr__("_immutable", False)
 
-        self._payload = kwargs.get("payload", None)
+        self._payload = payload
         if self._payload is None:
             raise rte.RTCMMessageError("Payload must be specified")
         self._payblen = len(self._payload) * 8  # length of payload in bits
-        self._scaling = int(kwargs.get("scaling", True))
-        self._labelmsm = int(kwargs.get("labelmsm", True))
+        self._scaling = scaling
+        self._labelmsm = labelmsm
         self._unknown = False
+        self._satmap = None
+        self._cellmap = None
         self._do_attributes()
 
         self._immutable = True  # once initialised, object is immutable
 
     def _do_attributes(self):
         """
         Populate RTCMMessage attributes from payload.
@@ -74,164 +65,257 @@
         :raises: RTCMTypeError
         """
 
         offset = 0  # payload offset in bits
         index = []  # array of (nested) group indices
 
         try:
-            pdict = (
-                self._get_dict()
-            )  # get payload definition dict for this message identity
+            # get payload definition dict for this message identity
+            pdict = self._get_dict()
             if pdict is None:  # unknown (or not yet implemented) message identity
                 self._do_unknown()
                 return
-            for key in pdict:  # process each attribute in dict
-                (offset, index) = self._set_attribute(offset, pdict, key, index)
+            for anam in pdict:  # process each attribute in dict
+                (offset, index) = self._set_attribute(anam, pdict, offset, index)
 
         except Exception as err:
             raise rte.RTCMTypeError(
                 (
-                    f"Error processing attribute '{key}' "
+                    f"Error processing attribute '{anam}' "
                     f"in message type {self.identity} {err}"
                 )
             ) from err
 
-    def _set_attribute(self, offset: int, pdict: dict, key: str, index: list) -> tuple:
+    def _set_attribute(self, anam: str, pdict: dict, offset: int, index: list) -> tuple:
         """
-        Recursive routine to set individual or grouped payload attributes.
+        Recursive routine to set individual, conditional or grouped payload attributes.
 
-        :param int offset: payload offset in bits
+        :param str anam: attribute name
         :param dict pdict: dict representing payload definition
-        :param str key: attribute keyword
+        :param int offset: payload offset in bits
         :param list index: repeating group index array
         :return: (offset, index[])
         :rtype: tuple
 
         """
 
-        att = pdict[key]  # get attribute type
-        if isinstance(att, tuple):  # repeating group of attributes
-            (offset, index) = self._set_attribute_group(att, offset, index)
+        adef = pdict[anam]  # get attribute definition
+        if isinstance(adef, tuple):  # attribute group
+            gtyp, _ = adef
+            if isinstance(gtyp, tuple):  # conditional group of attributes
+                (offset, index) = self._set_attribute_optional(adef, offset, index)
+            else:  # repeating group of attributes
+                (offset, index) = self._set_attribute_group(adef, offset, index)
         else:  # single attribute
-            offset = self._set_attribute_single(att, offset, key, index)
+            offset = self._set_attribute_single(anam, offset, index)
 
         return (offset, index)
 
-    def _set_attribute_group(self, att: tuple, offset: int, index: list) -> tuple:
+    def _set_attribute_optional(self, adef: tuple, offset: int, index: list) -> tuple:
+        """
+        Process conditional group of attributes - group is present if attribute value
+        = specific value, otherwise absent.
+
+        :param tuple adef: attribute definition - tuple of ((attribute name, condition), group dict)
+        :param int offset: payload offset in bits
+        :param list index: repeating group index array
+        :return: (offset, index[])
+        :rtype: tuple
+        """
+
+        (anam, con), gdict = adef  # (attribute name, condition), group dictionary
+        # "+n" suffix signifies that one or more nested group indices
+        # must be appended to name e.g. "DF379_01", "IDF023_03"
+        # if "+" in anam:
+        #     anam, nestlevel = anam.split("+")
+        #     for i in range(int(nestlevel)):
+        #        anam += f"_{index[i]:02d}"
+
+        if getattr(self, anam) == con:  # if condition is met...
+            # recursively process each group attribute,
+            # incrementing the payload offset as we go
+            for anamg in gdict:
+                (offset, index) = self._set_attribute(anamg, gdict, offset, index)
+
+        return (offset, index)
+
+    def _set_attribute_group(self, adef: tuple, offset: int, index: list) -> tuple:
         """
         Process (nested) group of attributes.
 
-        :param tuple att: attribute group - tuple of (num repeats, attribute dict)
+        :param tuple adef: attribute definition - tuple of (attr name, attribute dict)
         :param int offset: payload offset in bits
         :param list index: repeating group index array
         :return: (offset, index[])
         :rtype: tuple
 
         """
 
-        numr, attd = att  # number of repeats, attribute dictionary
+        anam, gdict = adef  # attribute signifying group size, group dictionary
         # derive or retrieve number of items in group
-        if isinstance(numr, int):  # fixed number of repeats
-            rng = numr
+        if isinstance(anam, int):  # fixed number of repeats
+            gsiz = anam
         else:  # number of repeats is defined in named attribute
-            # if attribute is within a group
-            # append group index to name e.g. "DF379_01"
-            if numr == "DF379":
-                numr += f"_{index[-1]:02d}"
-            rng = getattr(self, numr)
+            # "+n" suffix signifies that one or more nested group indices
+            # must be appended to name e.g. "DF379_01", "IDF023_03"
+            if "+" in anam:
+                anam, nestlevel = anam.split("+")
+                for i in range(int(nestlevel)):
+                    anam += f"_{index[i]:02d}"
+            gsiz = getattr(self, anam)
+            if anam == "IDF035":  # 4076_201 range is N-1
+                gsiz += 1
 
         index.append(0)  # add a (nested) group index level
         # recursively process each group attribute,
         # incrementing the payload offset and index as we go
-        for i in range(rng):
+        for i in range(gsiz):
             index[-1] = i + 1
-            for key1 in attd:
-                (offset, index) = self._set_attribute(offset, attd, key1, index)
+            for anamg in gdict:
+                (offset, index) = self._set_attribute(anamg, gdict, offset, index)
 
         index.pop()  # remove this (nested) group index
 
         return (offset, index)
 
     def _set_attribute_single(
         self,
-        att: object,
+        anam: str,
         offset: int,
-        key: str,
         index: list,
     ) -> int:
         """
         Set individual attribute value, applying scaling where appropriate.
 
-        :param str att: attribute type string e.g. 'INT008'
+        :param str anam: attribute name
         :param int offset: payload offset in bits
-        :param str key: attribute keyword
         :param list index: repeating group index array
         :return: offset
         :rtype: int
 
         """
-        # pylint: disable=no-member
+
+        # pylint: disable=invalid-name
 
         # if attribute is part of a (nested) repeating group, suffix name with index
-        keyr = key
-        for i in index:  # one index for each nested level (unless it's a boolean group)
-            if i > 0 and keyr not in BOOL_GROUPS:
-                keyr += f"_{i:02d}"
+        anami = anam
+        for i in index:  # one index for each nested level
+            if i > 0:
+                anami += f"_{i:02d}"
 
         # get value of required number of bits at current payload offset
-        att, scale, _ = RTCM_DATA_FIELDS[key]
+        atyp, ares, _ = RTCM_DATA_FIELDS[anam]
         if not self._scaling:
-            scale = 0
-        if key == "DF396":  # this MSM attribute has variable length
-            atts = getattr(self, NSAT) * getattr(self, NSIG)
+            ares = 0
+        if anam == "DF396":  # this MSM attribute has variable length
+            asiz = getattr(self, NSAT) * getattr(self, NSIG)
+        else:
+            asiz = attsiz(atyp)
+        if atyp == PRN:
+            val = self._satmap[index[0]]
+        elif atyp == CELPRN:
+            val = self._cellmap[index[0]][0]
+        elif atyp == CELSIG:
+            val = self._cellmap[index[0]][1]
         else:
-            atts = attsiz(att)
-        bitfield = self._getbits(offset, atts)
-        val = bits2val(att, scale, bitfield)
+            bitfield = self._getbits(offset, asiz)
+            val = bits2val(atyp, ares, bitfield)
 
-        setattr(self, keyr, val)
-        offset += atts
+        setattr(self, anami, val)
+        offset += asiz
 
         # add special attributes to keep track of
-        # MSM / 1230 message group sizes
+        # MSM message group sizes
         # NB: This is predicated on MSM payload dictionaries
         # always having attributes DF394, DF395 and DF396
         # in that order
-        if key == "DF394":  # num of satellites in MSM message
-            setattr(self, NSAT, num_setbits(bitfield))
-        if key == "DF395":  # num of signals in MSM message
-            setattr(self, NSIG, num_setbits(bitfield))
-        if key == "DF396":  # num of cells in MSM message
-            setattr(self, NCELL, num_setbits(bitfield))
-        if key == "DF422":  # bitmask of bias entries in 1230 message
-            setattr(self, NL1CA, (bitfield & 8) >> 3)  # MSB
-            setattr(self, NL1P, (bitfield & 4) >> 2)
-            setattr(self, NL2CA, (bitfield & 2) >> 1)
-            setattr(self, NL2P, bitfield & 1)  # LSB
+        if anam in ("DF394", "DF395", "DF396"):
+            nbits = bin(bitfield).count("1")  # number of bits set
+            if anam == "DF394":  # num of satellites in MSM message
+                setattr(self, NSAT, nbits)
+            elif anam == "DF395":  # num of signals in MSM message
+                setattr(self, NSIG, nbits)
+            elif anam == "DF396":  # num of cells in MSM message
+                setattr(self, NCELL, nbits)
+                # populate NSAT and NCELL mapping dictionaries
+                self._getsatcellmaps()
+
+        # add special coefficient attributes for message 4076_201
+        if anam == "IDF038":
+            i = index[0]
+            N = getattr(self, f"IDF037_{i:02d}") + 1
+            M = getattr(self, f"IDF038_{i:02d}") + 1
+            nc = int(((N + 1) * (N + 2) / 2) - ((N - M) * (N - M + 1) / 2))
+            ns = int(nc - (N + 1))
+            # ncs = (N + 1) * (N + 1) - (N - M) * (N - M + 1)
+            # print(f"DEBUG nc {nc} ns {ns} ncs {ncs} nc+ns {nc+ns}")
+            setattr(self, NHARMCOEFFC, nc)
+            setattr(self, NHARMCOEFFS, ns)
 
         return offset
 
+    def _getsatcellmaps(self):
+        """
+        Map group indices to satellite PRN & signal ID values via
+        bitmasks DF394, DF395 and DF396.
+        """
+
+        prnmap, sigmap = PRNSIGMAP[str(self.identity)[0:3]]
+        sigcode = 0 if self._labelmsm == 2 else 1
+
+        sats = {}
+        nsat = 0
+        for idx in range(1, 65):
+            if getattr(self, "DF394") >> (64 - idx) & 1:
+                nsat += 1
+                sats[nsat] = prnmap.get(idx, NA)
+
+        sigs = []
+        nsig = 0
+        for idx in range(1, 33):
+            if getattr(self, "DF395") >> (32 - idx) & 1:
+                sgc = sigmap.get(idx, NA)
+                fqc = sgc[1] if sigcode else sgc[0]
+                sigs.append(fqc)
+                nsig += 1
+
+        ncells = int(nsat * nsig)
+        cells = {}
+        ncell = idx = 0
+        for sat in range(nsat):
+            for sig in range(nsig):
+                idx += 1
+                if getattr(self, "DF396") >> (ncells - idx) & 1:
+                    ncell += 1
+                    cells[ncell] = (sats[sat + 1], sigs[sig])
+
+        self._satmap = sats
+        self._cellmap = cells
+
     def _getbits(self, position: int, length: int) -> int:
         """
-        Get unisgned integer value of masked bits in bytes.
+        Get unsigned integer value of masked bits in bytes.
 
         :param int position: position in bitfield, from leftmost bit
         :param int length: length of masked bits
         :return: value
         :rtype: int
         """
 
+        if length == 0:
+            return 0
         if position + length > self._payblen:
             raise rte.RTCMMessageError(
-                f"Attribute size {length} exceeds remaining payload length {self._payblen - position}"
+                f"Attribute size {length} exceeds remaining "
+                + f"payload length {self._payblen - position}"
             )
 
         return int.from_bytes(self._payload, "big") >> (
             self._payblen - position - length
-        ) & (2**length - 1)
+        ) & ((2 << length - 1) - 1)
 
     def _get_dict(self) -> dict:
         """
         Get payload dictionary corresponding to message identity
         (or None if message type not defined)
 
         :return: dictionary representing payload definition
@@ -252,43 +336,22 @@
         """
         Human readable representation.
 
         :return: human readable representation
         :rtype: str
         """
 
-        # if MSM message and labelmsm flag is set,
-        # label NSAT and NCELL group attributes with
-        # corresponding satellite PRN and signal ID
-        is_msm = False
-        if not self._unknown:
-            if self._labelmsm and "MSM" in RTCM_MSGIDS[self.identity]:
-                sats = sat2prn(self)
-                cells = cell2prn(self)
-                is_msm = True
-
         stg = f"<RTCM({self.identity}, "
         for i, att in enumerate(self.__dict__):
             if att[0] != "_":  # only show public attributes
                 val = self.__dict__[att]
                 # escape all byte chars
                 if isinstance(val, bytes):
                     val = escapeall(val)
-                # label MSM NSAT and NCELL group attributes
-                lbl = ""
-                if is_msm:
-                    aname = att2name(att)
-                    if aname in ATT_NSAT:
-                        prn = sats[att2idx(att)]
-                        lbl = f"({prn})"
-                    if aname in ATT_NCELL:
-                        prn, sig = cells[att2idx(att)]
-                        lbl = f"({prn},{sig})"
-
-                stg += att + lbl + "=" + str(val)
+                stg += att + "=" + str(val)
                 if i < len(self.__dict__) - 1:
                     stg += ", "
         if self._unknown:
             stg += ", Not_Yet_Implemented"
         stg += ")>"
 
         return stg
@@ -339,20 +402,40 @@
         """
         Getter for identity.
 
         :return: message identity e.g. "1005"
         :rtype: str
         """
 
-        return str(self._payload[0] << 4 | self._payload[1] >> 4)
+        mid = self._payload[0] << 4 | self._payload[1] >> 4
+
+        if mid == 4076:  # proprietary IGS SSR message type
+            subtype = (self._payload[1] & 0x1) << 7 | self._payload[2] >> 1
+            mid = f"{mid}_{subtype:03d}"
+
+        return str(mid)
 
     @property
     def payload(self) -> bytes:
         """
         Payload getter - returns the raw payload bytes.
 
         :return: raw payload as bytes
         :rtype: bytes
 
         """
 
         return self._payload
+
+    @property
+    def ismsm(self) -> bool:
+        """
+        Check if message is Multiple Signal Message (MSM) type.
+
+        :return: True/False
+        :rtype: bool
+        """
+
+        try:
+            return "MSM" in RTCM_MSGIDS[self.identity]
+        except KeyError:
+            return False
```

### Comparing `pyrtcm-1.0.9/src/pyrtcm/rtcmreader.py` & `pyrtcm-1.1.0/src/pyrtcm/rtcmreader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 RTCMReader class.
 
 Reads and parses individual RTCM3 messages from any stream
 which supports a read(n) -> bytes method.
 
 RTCM3 transport layer bit format:
-+-------+--------+--------+--------+----------------+--------+
-| 0xd3  | 000000 | length |  type  |    content     |  crc   |
-+-------+--------+--------+--------+----------------+--------+
-|<- 8 ->|<- 6 -->|<- 10 ->|<- 12 ->|<-- variable -->|<- 24 ->|
-|                         |<- payload; length x 8 ->|        |
+
++--------+--------+---------+---------+----------------+---------+
+|  0xd3  | 000000 | length  |  type   |    content     |   crc   |
++========+========+=========+=========+================+=========+
+| 8 bits | 6 bits | 10 bits | 12 bits |    variable    | 24 bits |
++--------+--------+---------+---------+----------------+---------+
+|                           |   payload; length x 8    |         |
++--------+--------+---------+---------+----------------+---------+
 
 Returns both the raw binary data (as bytes) and the parsed data
 (as RTCMMessage object).
 
 Created on 14 Feb 2022
 
 :author: semuadmin
@@ -31,37 +34,45 @@
 
 
 class RTCMReader:
     """
     rtcmReader class.
     """
 
-    def __init__(self, datastream, **kwargs):
+    def __init__(
+        self,
+        datastream,
+        validate: int = rtt.VALCKSUM,
+        quitonerror: int = rtt.ERR_LOG,
+        scaling: bool = True,
+        labelmsm: int = 1,
+        bufsize: int = 4096,
+        errorhandler: object = None,
+    ):  # pylint: disable=too-many-arguments
         """Constructor.
 
         :param datastream stream: input data stream
-        :param int quitonerror: (kwarg) 0 = ignore,  1 = log and continue, 2 = (re)raise (1)
-        :param int errorhandler: (kwarg) error handling object or function (None)
-        :param int validate: (kwarg) 0 = ignore invalid checksum, 1 = validate checksum (1)
-        :param bool scaling: (kwarg) apply attribute scaling True/False (True)
-        :param bool labelmsm: (kwarg) whether to label MSM NSAT and NCELL attributes (True)
-        :param int bufsize: (kwarg) socket recv buffer size (4096)
+        :param int validate: 0 = ignore invalid checksum, 1 = validate checksum (1)
+        :param int quitonerror: 0 = ignore,  1 = log and continue, 2 = (re)raise (1)
+        :param bool scaling: apply attribute scaling True/False (True)
+        :param int labelmsm: MSM NSAT and NCELL attribute label (1 = RINEX, 2 = freq)
+        :param int bufsize: socket recv buffer size (4096)
+        :param object errorhandler: error handling object or function (None)
         :raises: RTCMStreamError (if mode is invalid)
         """
 
-        bufsize = int(kwargs.get("bufsize", 4096))
         if isinstance(datastream, socket):
             self._stream = SocketStream(datastream, bufsize=bufsize)
         else:
             self._stream = datastream
-        self._quitonerror = int(kwargs.get("quitonerror", rtt.ERR_LOG))
-        self._errorhandler = kwargs.get("errorhandler", None)
-        self._validate = int(kwargs.get("validate", rtt.VALCKSUM))
-        self._scaling = int(kwargs.get("scaling", True))
-        self._labelmsm = int(kwargs.get("labelmsm", True))
+        self._quitonerror = quitonerror
+        self._errorhandler = errorhandler
+        self._validate = validate
+        self._scaling = scaling
+        self._labelmsm = labelmsm
 
     def __iter__(self):
         """Iterator."""
 
         return self
 
     def __next__(self) -> tuple:
@@ -93,15 +104,15 @@
         parsing = True
 
         try:
             while parsing:  # loop until end of valid message or EOF
                 raw_data = None
                 parsed_data = None
                 byte1 = self._read_bytes(1)  # read the first byte
-                # if not rtcm, NMEA or RTCM3, discard and continue
+                # if not UBX, NMEA or RTCM3, discard and continue
                 if byte1 not in (b"\xb5", b"\x24", b"\xd3"):
                     continue
                 byte2 = self._read_bytes(1)
                 bytehdr = byte1 + byte2
                 # if it's a UBX message (b'\xb5\x62'), ignore it
                 if bytehdr == rtt.UBX_HDR:
                     (raw_data, parsed_data) = self._parse_ubx(bytehdr)
@@ -140,22 +151,21 @@
         :param bytes hdr: UBX header (b'\xb5\x62')
         :return: tuple of (raw_data as bytes, parsed_data as UBXMessage or None)
         :rtype: tuple
         """
 
         # read the rest of the UBX message from the buffer
         byten = self._read_bytes(4)
-        clsid = byten[0:1]
-        msgid = byten[1:2]
+        msgid = byten[0:2]
         lenb = byten[2:4]
         leni = int.from_bytes(lenb, "little", signed=False)
         byten = self._read_bytes(leni + 2)
         plb = byten[0:leni]
         cksum = byten[leni : leni + 2]
-        raw_data = hdr + clsid + msgid + lenb + plb + cksum
+        raw_data = hdr + msgid + lenb + plb + cksum
         parsed_data = None
         return (raw_data, parsed_data)
 
     def _parse_nmea(self, hdr: bytes) -> tuple:
         """
         Parse remainder of NMEA message.
 
@@ -171,15 +181,14 @@
         return (raw_data, parsed_data)
 
     def _parse_rtcm3(self, hdr: bytes) -> tuple:
         """
         Parse any RTCM3 data in the stream.
 
         :param bytes hdr: first 2 bytes of RTCM3 header
-        :param bool validate: (kwarg) validate CRC Y/N
         :return: tuple of (raw_data as bytes, parsed_stub as RTCMMessage)
         :rtype: tuple
         """
 
         hdr3 = self._read_bytes(1)
         size = (hdr[1] << 8) | hdr3[0]
         payload = self._read_bytes(size)
@@ -235,60 +244,44 @@
         if self._quitonerror == rtt.ERR_LOG:
             # pass to error handler if there is one
             if self._errorhandler is None:
                 print(err)
             else:
                 self._errorhandler(err)
 
-    def iterate(self, **kwargs) -> tuple:
-        """
-        DEPRECATED - WILL BE REMOVED IN VERSION >=1.0.6
-        USE STANDARD ITERATOR INSTEAD
-        Invoke the iterator within an exception handling framework.
-
-        :return: tuple of (raw_data as bytes, parsed_data as RTCMMessage)
-        :rtype: tuple
-        :raises: RTCM... Error (if quitonerror is set and stream is invalid)
-        """
-
-        while True:
-            try:
-                yield next(self)  # invoke the iterator
-            except StopIteration:
-                break
-
     @property
     def datastream(self) -> object:
         """
         Getter for stream.
 
         :return: data stream
         :rtype: object
         """
 
         return self._stream
 
     @staticmethod
-    def parse(message: bytes, **kwargs) -> object:
+    def parse(
+        message: bytes,
+        validate: int = rtt.VALCKSUM,
+        scaling: bool = True,
+        labelmsm: int = 1,
+    ) -> "RTCMMessage":
         """
         Parse RTCM message to RTCMMessage object.
 
         :param bytes message: RTCM raw message bytes
-        :param int validate: (kwargs) 0 = don't validate CRC, 1 = validate CRC (1)
-        :param bool scaling: (kwargs) apply attribute scaling True/False (True)
-        :param bool labelmsm: (kwarg) whether to label MSM NSAT and NCELL attributes (True)
+        :param int validate: 0 = don't validate CRC, 1 = validate CRC (1)
+        :param bool scaling: apply attribute scaling True/False (True)
+        :param int labelmsm: MSM NSAT and NCELL attribute label (1 = RINEX, 2 = freq)
         :return: RTCMMessage object
         :rtype: RTCMMessage
         :raises: RTCMParseError (if data stream contains invalid data or unknown message type)
         """
-        # pylint: disable=unused-argument
 
-        validate = kwargs.get("validate", rtt.VALCKSUM)
-        scaling = int(kwargs.get("scaling", True))
-        labelmsm = int(kwargs.get("labelmsm", True))
         if validate & rtt.VALCKSUM:
             if calc_crc24q(message):
                 raise rte.RTCMParseError(
                     f"RTCM3 message invalid - failed CRC: {message[-3:]}"
                 )
         payload = message[3:-3]
         return RTCMMessage(payload=payload, scaling=scaling, labelmsm=labelmsm)
```

### Comparing `pyrtcm-1.0.9/src/pyrtcm/rtcmtypes_core.py` & `pyrtcm-1.1.0/src/pyrtcm/rtcmtypes_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,46 +2,62 @@
 RTCM Protocol core globals and constants
 
 Created on 14 Feb 2022
 
 Information sourced from RTCM STANDARD 10403.3 © 2016 RTCM
 
 :author: semuadmin
+:copyright: SEMU Consulting © 2022
+:license: BSD 3-Clause
 """
+
 # pylint: disable=line-too-long
 
-NMEA_HDR = [b"\x24\x47", b"\x24\x50"]
+NMEA_HDR = [
+    b"$V",
+    b"$M",
+    b"$P",
+    b"$B",
+    b"$D",
+    b"$I",
+    b"$L",
+    b"$G",
+    b"$F",
+    b"$S",
+    b"$H",
+    b"$R",
+    b"$E",
+    b"$Y",
+    b"$A",
+    b"$C",
+    b"$Z",
+    b"$T",
+    b"$W",
+]
 UBX_HDR = b"\xb5\x62"
 RTCM_HDR = b"\xd3"
 NMEA_PROTOCOL = 1
 UBX_PROTOCOL = 2
 RTCM3_PROTOCOL = 4
 GET = 0
 SET = 1
 POLL = 2
 VALNONE = 0
 VALCKSUM = 1
-RTCM3_PROTOCOL = 4
 ERR_RAISE = 2
 ERR_LOG = 1
 ERR_IGNORE = 0
+NA = "N/A"
 
 NSAT = "NSat"
 NSIG = "NSig"
 NCELL = "NCell"
-NL1CA = "_NL1CA"
-NL1P = "_NL1P"
-NL2CA = "_NL2CA"
-NL2P = "_NL2P"
-# Number of Residuals groups in MT1023 and MT1024
-NRES = 16
-# list of 'group' attributes which have
-# an occurrence of 0 or 1
-BOOL_GROUPS = ("DF423", "DF424", "DF425", "DF426")
-
+NRES = 16  # number of Residuals groups in MT1023 and MT1024
+NHARMCOEFFC = "_NHarmCoeffC"  # number of cosine harmonic coefficients in 4076
+NHARMCOEFFS = "_NHarmCoeffS"  # number of sine harmonic coefficients in 4076
 
 # Power of 2 scaling constants
 P2_P4 = 16  # 2**4
 P2_4 = 0.0625  # 2**-4
 P2_5 = 0.03125  # 2**-5
 P2_6 = 0.015625  # 2**-6
 P2_10 = 0.0009765625  # 2**-10
@@ -74,15 +90,15 @@
 BIT6 = "BIT006"  # 6 bit bit field
 BIT7 = "BIT007"  # 7 bit bit field
 BIT8 = "BIT008"  # 8 bit bit field
 BIT10 = "BIT010"  # 10 bit bit field
 BIT12 = "BIT012"  # 12 bit bit field
 BIT32 = "BIT032"  # 32 bit bit field
 BIT64 = "BIT064"  # 64 bit bit field
-BITX = "BIT999"  # variable bit field TODO check against usage
+BITX = "BIT999"  # variable bit field
 CHAR8 = "CHA008"  # 8 bit characters, ISO 8859-1 (not limited to ASCII)
 INT6 = "INT006"  # 6 bit 2’s complement integer
 INT8 = "INT008"  # 8 bit 2’s complement integer
 INT9 = "INT009"  # 9 bit 2’s complement integer
 INT10 = "INT010"  # 10 bit 2’s complement integer
 INT11 = "INT011"  # 11 bit 2’s complement integer
 INT12 = "INT012"  # 12 bit 2’s complement integer
@@ -135,27 +151,32 @@
 INTS5 = "SNT005"  # 5 bit sign-magnitude integer
 INTS11 = "SNT011"  # 11 bit sign-magnitude integer
 INTS22 = "SNT022"  # 22 bit sign-magnitude integer
 INTS24 = "SNT024"  # 24 bit sign-magnitude integer
 INTS27 = "SNT027"  # 27 bit sign-magnitude integer
 INTS32 = "SNT032"  # 32 bit sign-magnitude integer
 UTF8 = "UTF008"  # Unicode UTF-8 Code Unit
-
+PRN = "PRN000"  # Derived satellite PRN
+CELPRN = "CPR000"  # Derived cell PRN
+CELSIG = "CSG000"  # Derived cell Signal ID
 
 # ****************************************************
 # THESE ARE THE RTCM PROTOCOL DATA FIELDS
 #
 # DF key: (data_type, scale_factor, description)
 # scale_factor of 0 means N/A (no scaling)
 #
 # NOTICE 1: These values are provided in semicircles;
 #           multiply by π to use in orbit computations
 #
 # ****************************************************
 RTCM_DATA_FIELDS = {
+    "PRN": (PRN, 0, "Derived satellite PRN"),
+    "CELLPRN": (CELPRN, 0, "Derived satellite PRN"),
+    "CELLSIG": (CELSIG, 0, "Derived satellite Signal ID"),
     "DF001": (BIT1, 0, "Reserved Field"),
     "DF001_1": (BIT1, 0, "Reserved 1 bit"),
     "DF001_2": (BIT2, 0, "Reserved 2 bits"),
     "DF001_3": (BIT3, 0, "Reserved 3 bits"),
     "DF001_7": (BIT7, 0, "Reserved 7 bits"),
     "DF002": (UINT12, 0, "Message Number"),
     "DF003": (UINT12, 0, "Reference Station ID"),
@@ -234,36 +255,72 @@
     "DF072": (UINT4, 0, "Subnetwork ID"),
     "DF073": (UINT8, 0, "RESERVED for Provider ID"),
     "DF074": (BIT2, 0, "GPS Ambiguity Status Flag"),
     "DF075": (UINT3, 0, "GPS Non Sync Count"),
     "DF076": (UINT10, 0, "GPS Week number"),
     "DF077": (BIT4, 0, "GPS SV Acc. (URA)"),
     "DF078": (BIT2, 1, "GPS CODE ON L2"),
-    "DF079": (INT14, P2_43, "GPS IDOT"),  # see NOTICE 1 above
-    "DF080": (UINT8, 1, "GPS IODE"),
-    "DF081": (UINT16, P2_P4, "GPS toc"),
-    "DF082": (INT8, P2_55, "GPS af2"),
-    "DF083": (INT16, P2_43, "GPS af1"),
-    "DF084": (INT22, P2_31, "GPS af0"),
-    "DF085": (UINT10, 1, "GPS IODC"),
-    "DF086": (INT16, P2_5, "GPS Crs"),
-    "DF087": (INT16, P2_43, "GPS ∆n"),  # see NOTICE 1 above
-    "DF088": (INT32, P2_31, "GPS M0"),  # see NOTICE 1 above
-    "DF089": (INT16, P2_29, "GPS Cuc"),
+    "DF079": (INT14, P2_43, "GPS IDOT (Issue of Data, Time)"),  # see NOTICE 1 above
+    "DF080": (UINT8, 1, "GPS IODE (Issue of Data, Ephemeris)"),
+    "DF081": (UINT16, P2_P4, "GPS toc (Reference Time, Clock)"),
+    "DF082": (INT8, P2_55, "GPS af2 (Clock correction drift rate)"),
+    "DF083": (INT16, P2_43, "GPS af1 (Clock correction drift)"),
+    "DF084": (INT22, P2_31, "GPS af0 (Clock correction bias)"),
+    "DF085": (UINT10, 1, "GPS IODC (Issue of Data, Clock)"),
+    "DF086": (
+        INT16,
+        P2_5,
+        "GPS Crs (Amplitude of sine harmonic correction term to the orbit radius)",
+    ),
+    "DF087": (
+        INT16,
+        P2_43,
+        "GPS ∆n (Mean motion difference from computed value)",
+    ),  # see NOTICE 1 above
+    "DF088": (INT32, P2_31, "GPS M0 (Mean Anomaly)"),  # see NOTICE 1 above
+    "DF089": (
+        INT16,
+        P2_29,
+        "GPS Cuc (Amplitude of cosine harmonic correction term to argument of latitude)",
+    ),
     "DF090": (UINT32, P2_33, "GPS e (Eccentricity)"),
-    "DF091": (INT16, P2_29, "GPS Cus"),
-    "DF092": (UINT32, P2_19, "GPS A½"),
-    "DF093": (UINT16, P2_P4, "GPS toe"),
-    "DF094": (INT16, P2_29, "GPS Cic"),
-    "DF095": (INT32, P2_31, "GPS Ω0"),  # see NOTICE 1 above
-    "DF096": (INT16, P2_29, "GPS Cis"),
-    "DF097": (INT32, P2_31, "GPS i0"),  # see NOTICE 1 above
-    "DF098": (INT16, P2_5, "GPS Crc"),
+    "DF091": (
+        INT16,
+        P2_29,
+        "GPS Cus (Amplitude of sine harmonic correction term to argument of latitude)",
+    ),
+    "DF092": (UINT32, P2_19, "GPS A½ (Square root of Semi-major Axis)"),
+    "DF093": (UINT16, P2_P4, "GPS toe (Reference Time, Ephemeris)"),
+    "DF094": (
+        INT16,
+        P2_29,
+        "GPS Cic (Amplitude of cosine harmonic correction term to angle of inclination)",
+    ),
+    "DF095": (
+        INT32,
+        P2_31,
+        "GPS Ω0 (Longitude of Ascending Node)",
+    ),  # see NOTICE 1 above
+    "DF096": (
+        INT16,
+        P2_29,
+        "GPS Cis (Amplitude of sine harmonic correction term to angle of inclination)",
+    ),
+    "DF097": (INT32, P2_31, "GPS i0 (Inclination)"),  # see NOTICE 1 above
+    "DF098": (
+        INT16,
+        P2_5,
+        "GPS Crc (Amplitude of cosine harmonic correction term to orbit radius)",
+    ),
     "DF099": (INT32, P2_31, "GPS ω (Argument of Perigee)"),  # see NOTICE 1 above
-    "DF100": (INT24, P2_43, "GPS ΩDOT (Rate of Right Ascension)"),  # see NOTICE 1 above
+    "DF100": (
+        INT24,
+        P2_43,
+        "GPS ΩDOT (Rate of Change of Right Ascension)",
+    ),  # see NOTICE 1 above
     "DF101": (INT8, P2_31, "GPS tGD"),
     "DF102": (UINT6, 1, "GPS SV HEALTH"),
     "DF103": (BIT1, 1, "GPS L2 P data flag"),
     "DF104": (BIT1, 0, "GLONASS almanac health"),
     "DF105": (BIT1, 0, "GLONASS almanac health availability indicator"),
     "DF106": (BIT2, 0, "GLONASS P1"),
     "DF107": (BIT12, 0, "GLONASS tk"),
@@ -406,14 +463,15 @@
     "DF240": (UINT20, 1, "GPS FKP Epoch Time"),
     "DF241": (UINT17, 1, "GLONASS FKP Epoch Time"),
     "DF242": (INT12, 0.01, "N0: Geometric Gradient in North (ppm)"),
     "DF243": (INT12, 0.01, "E0: Geometric gradient in east (ppm)"),
     "DF244": (INT14, 0.01, "NI: Ionospheric gradient in north  (ppm)"),
     "DF245": (INT14, 0.01, "EI: Ionospheric gradient in east  (ppm)"),
     # 'DF246-DF251': RESERVED,
+    "DF248": (UINT30, 1, "Galileo Epoch Time (TOW)"),
     "DF252": (UINT6, 0, "Galileo Satellite ID"),
     "DF286": (BIT8, 0, "Galileo SISA (E1,E5b"),
     "DF287": (BIT2, 0, "Galileo E1-B Signal Health Status"),
     "DF288": (BIT1, 0, "Galileo E1-B Data Validity Status"),
     "DF289": (UINT12, 1, "Galileo Week Number"),
     "DF290": (UINT10, 1, "Galileo IODnav"),
     "DF291": (BIT8, 0, "Galileo SV SISA"),
@@ -514,15 +572,18 @@
     "DF415": (UINT4, 1, "SSR Solution ID"),
     "DF416": (UINT3, 1, "GLONASS Day Of Week"),
     "DF417": (BIT1, 0, "GNSS Smoothing Type Indicator"),
     "DF418": (BIT3, 0, "GNSS Smoothing Interval"),
     "DF419": (UINT4, 1, "GLONASS Satellite Frequency Channel Number"),
     "DF420": (BIT1, 0, "Half-cycle ambiguity indicator"),
     "DF421": (BIT1, 0, "GLONASS Code-Phase Bias Indicator"),
-    "DF422": (BIT4, 0, "GLONASS FDMA Signals Mask"),
+    "DF422_1": (BIT1, 0, "GLONASS FDMA Signals Mask L1 C/A"),
+    "DF422_2": (BIT1, 0, "GLONASS FDMA Signals Mask L1 P"),
+    "DF422_3": (BIT1, 0, "GLONASS FDMA Signals Mask L2 C/A"),
+    "DF422_4": (BIT1, 0, "GLONASS FDMA Signals Mask L2 P"),
     "DF423": (INT16, 0.02, "GLONASS L1 C/A Code-Phase Bias"),
     "DF424": (INT16, 0.02, "GLONASS L1 P Code-Phase Bias"),
     "DF425": (INT16, 0.02, "GLONASS L2 C/A Code-Phase Bias"),
     "DF426": (INT16, 0.02, "GLONASS L2 P Code-Phase Bias"),
     "DF427": (UINT30, 1, "BeiDou Epoch Time (TOW)"),
     "DF428": (UINT30, 1, "QZSS Epoch Time (TOW)"),
     "DF429": (UINT4, 1, "QZSS Satellite ID"),
@@ -546,15 +607,15 @@
     "DF447": (INT16, P2_5, "QZSS Crc"),
     "DF448": (INT32, P2_31, "QZSS ω (Argument of Perigee)"),
     "DF449": (INT24, P2_43, "QZSS ΩDOT (Rate of Right Ascension)"),
     "DF450": (INT14, P2_43, "QZSS i0-DOT"),
     "DF451": (BIT2, 1, "QZSS Codes on L2 Channel"),
     "DF452": (UINT10, 1, "QZSS Week Number"),
     "DF453": (UINT4, 0, "QZSS URA"),
-    "DF454": (UINT16, 1, "QZSS SV health"),
+    "DF454": (UINT6, 1, "QZSS SV health"),
     "DF455": (INT8, P2_31, "QZSS TGD"),
     "DF456": (UINT10, 1, "QZSS IODC"),
     "DF457": (BIT1, 1, "QZSS Fit Interval"),
     "DF488": (UINT6, 0, "BDS Satellite ID"),
     "DF489": (UINT13, 1, "BDS Week Number"),
     "DF490": (BIT4, 1, "BDS URAI"),
     "DF491": (INT14, P2_43, "BDS IDOT"),
@@ -609,16 +670,58 @@
     "DF540": (INT32, P2_31, "NAVIC/IRNSS Ω0 (Long of Ascending Node)"),
     "DF541": (INT32, P2_31, "NAVIC/IRNSS ω (Argument of perigee)"),
     "DF542": (INT22, P2_41, "NAVIC/IRNSS ΩDOT (Rate of Right Ascension)"),
     "DF543": (INT32, P2_31, "NAVIC/IRNSS i0 (Inclination)"),
     "DF544": (BIT2, 1, "NAVIC/IRNSS 2 spare bits after IDOT"),
     "DF545": (BIT2, 1, "NAVIC/IRNSS 2 spare bits after i0"),
     "DF546": (UINT30, 1, "NAVIC/IRNSS Epoch Time (TOW)"),
-    "GNSSSpecific": (UINT4, 0, "Extended Satellite Information"),
-    "GNSSEpoch": (UINT30, 0, "GNSS Epoch Time"),
+    "ExtSatInfo": (UINT4, 0, "Extended Satellite Information"),
+    # IGS SSR data types, used in 4076 messages
+    # https://files.igs.org/pub/data/format/igs_ssr_v1.pdf
+    "IDF001": (UINT3, 1, "IGM/IM Version"),
+    "IDF002": (UINT8, 1, "IGS Message Number"),
+    "IDF003": (UINT20, 1, "SSR Epoch Time 1s"),
+    "IDF004": (BIT4, 1, "SSR Update Interval"),
+    "IDF005": (BIT1, 1, "SSR Multiple Message Indicator"),
+    "IDF006": (BIT1, 1, "Global/Regional CRS Indicator"),
+    "IDF007": (UINT4, 1, "IOD SSR"),
+    "IDF008": (UINT16, 1, "SSR Provider ID"),
+    "IDF009": (UINT4, 1, "SSR Solution ID"),
+    "IDF010": (UINT6, 1, "No. of Satellites"),
+    "IDF011": (UINT6, 1, "GNSS Satellite ID"),
+    "IDF012": (BIT8, 1, "GNSS IOD"),
+    "IDF013": (INT22, 0.1, "Delta Orbit Radial"),
+    "IDF014": (INT20, 0.4, "Delta Orbit Along-Track"),
+    "IDF015": (INT20, 0.4, "Delta Orbit Cross-Track"),
+    "IDF016": (INT21, 0.001, "Dot Orbit Delta Radial"),
+    "IDF017": (INT19, 0.004, "Dot Orbit Delta Along-Track"),
+    "IDF018": (INT19, 0.004, "Dot Orbit Delta Cross-Track"),
+    "IDF019": (INT22, 0.1, "Delta Clock C0"),
+    "IDF020": (INT21, 0.001, "Delta Clock C1"),
+    "IDF021": (INT27, 0.00002, "Delta Clock C2"),
+    "IDF022": (INT22, 0.1, "High Rate Clock Correction"),
+    "IDF023": (UINT5, 1, "No. of Biases Processed"),
+    "IDF024": (UINT5, 1, "GNSS Signal and Tracking Mode Identifier"),
+    "IDF025": (INT14, 0.01, "Code Bias"),
+    "IDF026": (UINT9, 1 / 256, "Yaw Angle"),
+    "IDF027": (INT8, 1 / 8192, "Yaw Rate"),
+    "IDF028": (INT20, 0.0001, "Phase Bias"),
+    "IDF029": (BIT1, 1, "Signal Integer Indicator"),
+    "IDF030": (BIT2, 1, "Signals Wide-Lane Integer Indicator"),
+    "IDF031": (UINT4, 1, "Signal Discontinuity Counter"),
+    "IDF032": (BIT1, 1, "Dispersive Bias Consistency Indicator"),
+    "IDF033": (BIT1, 1, "MW Consistency Indicator"),
+    "IDF034": (BIT6, 1, "SSR URA"),
+    "IDF035": (UINT2, 1, "Number of Ionospheric Layers"),
+    "IDF036": (UINT8, 10, "Height of Ionospheric Layer"),
+    "IDF037": (UINT4, 1, "Spherical Harmonics Degree"),
+    "IDF038": (UINT4, 1, "Spherical Harmonics Order"),
+    "IDF039": (INT16, 0.005, "Spherical Harmonic Coefficient C"),
+    "IDF040": (INT16, 0.005, "Spherical Harmonic Coefficient S"),
+    "IDF041": (UINT9, 0.05, "VTEC Quality Indicator"),
 }
 
 # ***************************************************************************
 # THESE ARE THE RTCM PROTOCOL CORE MESSAGE IDENTITIES
 # Payloads for each of these identities are defined in the rtcmtypes_* modules
 # ***************************************************************************
 RTCM_MSGIDS = {
@@ -745,49 +848,103 @@
     "1135": "IRNSS MSM5",
     "1136": "IRNSS MSM6",
     "1137": "IRNSS MSM7",
     # "1138-1229":"Reserved MSM",
     "1230": "GLONASS L1 and L2 Code-Phase Biases",
     # "1240-1263": "SSR Messages"
     #
-    # Proprietary messages have not yet been implemented
+    # NB: Only those proprietary messages with public
+    # domain definitions have been implemented.
     #
     # "4001-4095":"Proprietary Messages",
-    "4072": "Mitsubishi Electric Corp",
-    "4073": "Unicore Communications Inc",
-    "4075": "Alberding GmbH",
-    "4076": "International GNSS Service (IGS)",
-    "4077": "Hemisphere GNSS Inc.",
-    "4078": "ComNav Technology Ltd.",
-    "4079": "SubCarrier Systems Corp. (SCSC) The makers of SNIP",
-    "4080": "NavCom Technology, Inc.",
-    "4081": "Seoul National University GNSS Lab",
-    "4082": "Cooperative Research Centre for Spatial Information",
-    "4083": "German Aerospace Center, Institute of Communications and Navigation (DLR)",
-    "4084": "Geodetics, Inc.",
-    "4085": "European GNSS Supervisory Authority",
-    "4086": "inPosition GmbH",
-    "4087": "Fugro",
-    "4088": "IfEN GmbH",
-    "4089": "Septentrio Satellite Navigation",
-    "4090": "Geo++",
-    "4091": "Topcon Positioning Systems",
-    "4092": "Leica Geosystems",
-    "4093": "NovAtel Inc.",
-    "4094": "Trimble Navigation Ltd.",
-    "4095": "Ashtech",
+    # "4072": "Mitsubishi Electric Corp",
+    # "4073": "Unicore Communications Inc",
+    # "4075": "Alberding GmbH",
+    # "4076": "International GNSS Service (IGS)",
+    "4076_021": "GPS SSR Orbit Correction",
+    "4076_022": "GPS SSR Clock Correction",
+    "4076_023": "GPS SSR Combined Orbit and Clock Correction",
+    "4076_024": "GPS SSR High Rate Clock Correction",
+    "4076_025": "GPS SSR Code Bias",
+    "4076_026": "GPS SSR Phase Bias",
+    "4076_027": "GPS SSR URA",
+    # "4076_028-040": "Reserved for GPS",
+    "4076_041": "GLONASS SSR Orbit Correction",
+    "4076_042": "GLONASS SSR Clock Correction",
+    "4076_043": "GLONASS SSR Combined Orbit and Clock Correction",
+    "4076_044": "GLONASS SSR High Rate Clock Correction",
+    "4076_045": "GLONASS SSR Code Bias",
+    "4076_046": "GLONASS SSR Phase Bias",
+    "4076_047": "GLONASS SSR URA",
+    # "4076_048-060": "Reserved for GLONASS",
+    "4076_061": "Galileo SSR Orbit Correction",
+    "4076_062": "Galileo SSR Clock Correction",
+    "4076_063": "Galileo SSR Combined Orbit and Clock Correction",
+    "4076_064": "Galileo SSR High Rate Clock Correction",
+    "4076_065": "Galileo SSR Code Bias",
+    "4076_066": "Galileo SSR Phase Bias",
+    "4076_067": "Galileo SSR URA",
+    # "4076_068-080": "Reserved for Galileo",
+    "4076_081": "QZSS SSR Orbit Correction",
+    "4076_082": "QZSS SSR Clock Correction",
+    "4076_083": "QZSS SSR Combined Orbit and Clock Correction",
+    "4076_084": "QZSS SSR High Rate Clock Correction",
+    "4076_085": "QZSS SSR Code Bias",
+    "4076_086": "QZSS SSR Phase Bias",
+    "4076_087": "QZSS SSR URA",
+    # "4076_088-100": "Reserved for QZSS",
+    "4076_101": "BeiDou SSR Orbit Correction",
+    "4076_102": "BeiDou SSR Clock Correction",
+    "4076_103": "BeiDou SSR Combined Orbit and Clock Correction",
+    "4076_104": "BeiDou SSR High Rate Clock Correction",
+    "4076_105": "BeiDou SSR Code Bias",
+    "4076_106": "BeiDou SSR Phase Bias",
+    "4076_107": "BeiDou SSR URA",
+    # "4076_108-120": "Reserved for BeiDou",
+    "4076_121": "SBAS SSR Orbit Correction",
+    "4076_122": "SBAS SSR Clock Correction",
+    "4076_123": "SBAS SSR Combined Orbit and Clock Correction",
+    "4076_124": "SBAS SSR High Rate Clock Correction",
+    "4076_125": "SBAS SSR Code Bias",
+    "4076_126": "SBAS SSR Phase Bias",
+    "4076_127": "SBAS SSR URA",
+    # "4076_128-140": "Reserved for SBAS",
+    # "4076_141-160": "Reserved for NavIC/IRNSS",
+    # "4076_161-200": "Reserved",
+    "4076_201": "GNSS SSR Ionosphere VTEC Spherical Harmonics",
+    # "4077": "Hemisphere GNSS Inc.",
+    # "4078": "ComNav Technology Ltd.",
+    # "4079": "SubCarrier Systems Corp. (SCSC) The makers of SNIP",
+    # "4080": "NavCom Technology, Inc.",
+    # "4081": "Seoul National University GNSS Lab",
+    # "4082": "Cooperative Research Centre for Spatial Information",
+    # "4083": "German Aerospace Center, Institute of Communications and Navigation (DLR)",
+    # "4084": "Geodetics, Inc.",
+    # "4085": "European GNSS Supervisory Authority",
+    # "4086": "inPosition GmbH",
+    # "4087": "Fugro",
+    # "4088": "IfEN GmbH",
+    # "4089": "Septentrio Satellite Navigation",
+    # "4090": "Geo++",
+    # "4091": "Topcon Positioning Systems",
+    # "4092": "Leica Geosystems",
+    # "4093": "NovAtel Inc.",
+    # "4094": "Trimble Navigation Ltd.",
+    # "4095": "Ashtech",
 }
 
-# list of MSM attributes to label if `labelmsm` kwarg is True
-ATT_NSAT = ["DF397", "DF398", "DF399", "GNSSSpecific"]
-ATT_NCELL = [
-    "DF400",
-    "DF401",
-    "DF402",
-    "DF403",
-    "DF404",
-    "DF405",
-    "DF406",
-    "DF407",
-    "DF408",
-    "DF420",
-]
+# map of MSM msg identity to GNSS name, epoch attribute name
+GNSSMAP = {
+    "107": ("GPS", "DF004"),
+    "108": ("GLONASS", "DF034"),
+    "109": ("GALILEO", "DF248"),
+    "110": ("SBAS", "DF004"),
+    "111": ("QZSS", "DF428"),
+    "112": ("BEIDOU", "DF427"),
+    "113": ("NAVIC", "DF546"),
+}
+
+# map of 4076_201 coefficients
+COEFFS = {
+    0: ("IDF039", "Cosine Coefficients"),
+    1: ("IDF040", "Sine Coefficients"),
+}
```

### Comparing `pyrtcm-1.0.9/src/pyrtcm/socket_stream.py` & `pyrtcm-1.1.0/src/pyrtcm/socket_stream.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,37 +20,39 @@
 
 
 class SocketStream:
     """
     socket stream class.
     """
 
-    def __init__(self, sock: socket, **kwargs):
+    def __init__(self, sock: socket, bufsize: int = 4096):
         """
         Constructor.
 
         :param sock socket: socket object
-        :param int bufsize: (kwarg) internal buffer size (4096)
+        :param int bufsize: internal buffer size (4096)
         """
 
         self._socket = sock
-        self._bufsize = kwargs.get("bufsize", 4096)
+        self._bufsize = bufsize
         self._buffer = bytearray()
         self._recv()  # populate initial buffer
 
     def _recv(self) -> bool:
         """
         Read bytes from socket into internal buffer.
 
         :return: return code (0 = failure, 1 = success)
         :rtype: bool
         """
 
         try:
             data = self._socket.recv(self._bufsize)
+            if len(data) == 0:
+                return False
             self._buffer += data
         except (OSError, TimeoutError):
             return False
         return True
 
     @property
     def buffer(self) -> bytearray:
```

### Comparing `pyrtcm-1.0.9/src/pyrtcm.egg-info/PKG-INFO` & `pyrtcm-1.1.0/src/pyrtcm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtcm
-Version: 1.0.9
+Version: 1.1.0
 Summary: RTCM3 protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2022, SEMU Consulting
         All rights reserved.
@@ -45,23 +45,35 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Provides-Extra: deploy
+Requires-Dist: build; extra == "deploy"
+Requires-Dist: pip; extra == "deploy"
+Requires-Dist: setuptools>=66.0; extra == "deploy"
+Requires-Dist: wheel; extra == "deploy"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: bandit; extra == "test"
+Requires-Dist: black; extra == "test"
+Requires-Dist: pylint; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: Sphinx; extra == "test"
+Requires-Dist: sphinx-rtd-theme; extra == "test"
 
 # pyrtcm
 
 [Current Status](#currentstatus) |
 [Installation](#installation) |
 [Reading](#reading) |
 [Parsing](#parsing) |
@@ -78,66 +90,75 @@
 [RTCM STANDARD 10403.n DIFFERENTIAL GNSS (GLOBAL NAVIGATION SATELLITE SYSTEMS) SERVICES – VERSION 3](https://rtcm.myshopify.com/collections/differential-global-navigation-satellite-dgnss-standards/products/rtcm-10403-3-differential-gnss-global-navigation-satellite-systems-services-version-3-amendment-2-may-20-2021).
 
 The `pyrtcm` homepage is located at [https://github.com/semuconsulting/pyrtcm](https://github.com/semuconsulting/pyrtcm).
 
 This is an independent project and we have no affiliation whatsoever with the Radio Technical Commission for Maritime Services.
 
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy; and UBX &copy; (u-blox) GNSS/GPS messages:
-- [pyubx2](http://github.com/semuconsulting/pyubx2) (**FYI** installing `pyubx2` via pip also installs `pynmeagps` and `pyrtcm`)
+- [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 
 ## <a name="currentstatus">Current Status</a>
 
 ![Status](https://img.shields.io/pypi/status/pyrtcm)
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyrtcm?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyrtcm/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyrtcm)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyrtcm)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyrtcm)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyrtcm.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyrtcm)
 
-Parses RTCM3 messages into their constituent data fields. Refer to the `RTCM_MSGIDS` dictionary in [`rtcmtypes_core.py`](https://github.com/semuconsulting/pyrtcm/blob/main/src/pyrtcm/rtcmtypes_core.py) for a list of message types currently implemented. Additional message types can be readily added - see [Extensibility](#extensibility)).
+Parses RTCM3 messages into their constituent data fields - `DF002`, `DF003`, etc. Refer to the `RTCM_MSGIDS` dictionary in [`rtcmtypes_core.py`](https://github.com/semuconsulting/pyrtcm/blob/main/src/pyrtcm/rtcmtypes_core.py#L695) for a list of message types currently implemented. Additional message types can be readily added - see [Extensibility](#extensibility).
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyrtcm](https://www.semuconsulting.com/pyrtcm).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyrtcm/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyrtcm/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyrtcm/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, post a message to one of the [pyrtcm Discussions](https://github.com/semuconsulting/pyrtcm/discussions) channels.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyrtcm` is compatible with Python >=3.8 and has no third-party library dependencies.
 
-In the following, `python` & `pip` refer to the Python 3 executables. You may need to type 
-`python3` or `pip3`, depending on your particular environment.
+In the following, `python3` & `pip` refer to the Python 3 executables. You may need to type 
+`python` or `pip3`, depending on your particular environment.
 
 ![Python version](https://img.shields.io/pypi/pyversions/pyrtcm.svg?style=flat)
 [![PyPI version](https://img.shields.io/pypi/v/pyrtcm.svg?style=flat)](https://pypi.org/project/pyrtcm/)
 ![PyPI downloads](https://img.shields.io/pypi/dm/pyrtcm.svg?style=flat)
 
 The recommended way to install the latest version of `pyrtcm` is with
 [pip](http://pypi.python.org/pypi/pip/):
 
 ```shell
-python -m pip install --upgrade pyrtcm
+python3 -m pip install --upgrade pyrtcm
 ```
 
 If required, `pyrtcm` can also be installed into a virtual environment, e.g.:
 
 ```shell
 python3 -m pip install --user --upgrade virtualenv
 python3 -m virtualenv env
 source env/bin/activate (or env\Scripts\activate on Windows)
 (env) python3 -m pip install --upgrade pyrtcm
 ...
 deactivate
 ```
 
+For [Conda](https://docs.conda.io/en/latest/) users, `pyrtcm` is also available from [conda-forge](https://github.com/conda-forge/pyrtcm-feedstock):
+
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyrtcm/badges/version.svg)](https://anaconda.org/conda-forge/pyrtcm)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyrtcm/badges/downloads.svg)](https://anaconda.org/conda-forge/pyrtcm)
+
+```shell
+conda install -c conda-forge pyrtcm
+```
+
 ---
 ## <a name="reading">Reading (Streaming)</a>
 
 ```
 class pyrtcm.rtcmreader.RTCMReader(stream, **kwargs)
 ```
 
@@ -145,147 +166,173 @@
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyrtcm` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual RTCM messages can then be read using the `RTCMReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `RTCMMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `RTCMReader` also implements an iterator.
 
 Example -  Serial input:
 ```python
->>> from serial import Serial
->>> from pyrtcm import RTCMReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>> rtr = RTCMReader(stream)
->>> (raw_data, parsed_data) = rtr.read()
->>> print(parsed_data)
- <RTCM(1077, DF002=1077, DF003=0, GNSSEpoch=204137001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=760738918298550272, NSat=10, DF395=1073807360, NSig=2, DF396=1044459, DF397_01(005)=75, DF397_02(007)=75, DF397_03(009)=81, ..., DF404_19(030,1C)=0.0, DF404_20(030,2L)=0.0)>,
+from serial import Serial
+from pyrtcm import RTCMReader
+with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
+  rtr = RTCMReader(stream)
+  raw_data, parsed_data = rtr.read()
+  print(parsed_data)
+```
+```
+"<RTCM(1077, DF002=1077, DF003=0, DF004=204137001, DF393=1, DF409=0, DF001_7=0, ..., DF404_15=-9556, DF404_16=-2148, DF404_17=-2174)>",     
 ```
 
 Example - File input (using iterator).
 ```python
->>> from pyrtcm import RTCMReader
->>> stream = open('rtcmdata.log', 'rb')
->>> rtr = RTCMReader(stream)
->>> for (raw_data, parsed_data) in rtr: print(parsed_data)
-...
+from pyrtcm import RTCMReader
+with open('rtcmdata.log', 'rb') as stream:
+  rtr = RTCMReader(stream)
+  for raw_data, parsed_data in rtr:
+    print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
->>> import socket
->>> from pyrtcm import RTCMReader
->>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
->>> stream.connect(("localhost", 50007))
->>> rtr = RTCMReader(stream)
->>> for (raw_data, parsed_data) in rtr: print(parsed_data)
+import socket
+from pyrtcm import RTCMReader
+with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as stream:
+  stream.connect(("localhost", 50007))
+  rtr = RTCMReader(stream)
+  for raw_data, parsed_data in rtr:
+    print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual RTCM messages using the static `RTCMReader.parse(data)` function, which takes a bytes array containing a binary RTCM message and returns a `RTCMMessage` object.
 
 **NB:** Once instantiated, an `RTCMMessage` object is immutable.
 
 Example:
 ```python
->>> from pyrtcm import RTCMReader
->>> msg = RTCMReader.parse(b"\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7")
->>> print(msg)
+from pyrtcm import RTCMReader
+msg = RTCMReader.parse(b"\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7")
+print(msg)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
 ```
 
-The `RTCMMessage` object exposes different public attributes depending on its message type or 'identity'. Attributes are defined as data fields ("DF002", "DF003", etc.) e.g. the `1005` message contains the following data fields:
+The `RTCMMessage` object exposes different public attributes depending on its message type or 'identity'. Attributes are defined as data fields (`DF002`, `DF003`, etc.) e.g. the `1097` multiple signal message (MSM) contains the following data fields:
 
 ```python
->>> print(msg)
-<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
->>> msg.identity
-'1005'
->>> msg.DF024
-1
+print(msg)
+print(msg.identity)
+print(msg.DF248)
+print(msg.DF404_07)
+```
+```
+"<RTCM(1097, DF002=1097, DF003=0, DF248=204137001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=216181732825628672, NSat=5, DF395=1073872896, NSig=2, DF396=1023, NCell=10, PRN_01=007, PRN_02=008, PRN_03=021, PRN_04=027, ..., DF404_07=5534, DF404_08=5545, DF404_09=-7726, DF404_10=-7733)>",             
+'1097'
+204137001
+5534
 ```
 
+Attributes within repeating groups are parsed with a two-digit suffix (`DF419_01`, `DF419_02`, etc. See [example below](#iterating) for an illustration of how to iterate through grouped attributes).
+
 Helper methods are available to interpret the individual datafields:
 
 ```python
->>> from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
->>> dfname = "DF012"
->>> RTCM_DATA_FIELDS[dfname]
+from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
+dfname = "DF012"
+print(RTCM_DATA_FIELDS[dfname])
+print(datasiz(dfname))
+print(datascale(dfname))
+print(datadesc(dfname))
+```
+```
 (INT20, 0.0001, "GPS L1 PhaseRange - L1 Pseudorange")
->>> datasiz(dfname) # size in bits
 20
->>> datascale(dfname) # scaling factor
 0.0001
->>> datadesc(dfname) # description
 'GPS L1 PhaseRange - L1 Pseudorange'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
-Attributes within repeating groups are parsed with a two-digit suffix ("DF030_01", "DF030_02", etc.). 
+#### <a name="iterating">Iterating Through Group Attributes</a>
 
-**Tip:** To iterate through a repeating group of attributes (*e.g., DF406 (GNSS signal fine PhaseRange)*) as a list, the following construct can be used:
+To iterate through a group of one or more repeating attributes in a given `RTCMMessage` object, the following construct can be used (in this illustration, repeating attributes CELLPRN, CELLSIG, DF405, DF406, DF407, DF408, DF420 and DF404 are extracted from an MSM 1077 message `msg` and collated in the array `msmarray`):
 
+```python
+msmarray = []
+for i in range(msg.NCell): # msg = MSM 1077, number of cells = NCell
+  vals = []
+  for attr in ("CELLPRN", "CELLSIG", "DF405", "DF406", "DF407", "DF408", "DF420", "DF404"):
+    val = getattr(msg, f"{attr}_{i+1:02d}")
+    vals.append(val)
+  msmarray.append(vals)
+print(msmarray)
 ```
-df406group = [] # list of DF406 ((GNSS signal fine PhaseRange) values from repeating group in MSM 1077 message
-for i in range(msg.NCell):
-    df406 = getattr(msg, f"DF406_{i+1:02}")
-    df406group.append(df406)
+```shell
+[['005', '1C', 0.00014309026300907135, 0.00014193402603268623, 341, 45.0, 0, -0.9231], ..., ['030', '2L', -0.00030865520238876343, -0.00030898721888661385, 341, 41.0, 0, -0.2174]]
 ```
 
-Attributes within MSM NSAT and NCELL repeating groups can optionally be labelled with their corresponding satellite PRN and signal ID when the `__str__()` method is invoked, by setting the keyword argument `labelmsm` to True (e.g. `DF405_10(014,2C)` signifies that the 10th item in the DF405 group refers to satellite PRN 014, signal ID 2C).
+The following dedicated helper methods are available to parse selected RTCM3 message types into a series of iterable data arrays:
+- `parse_msm` - for MSM message types (e.g. 1077, 1125, etc.).
+- `parse_4076_201` - for 4076_201 SSR (harmonic coefficients) message types.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyrtcm.rtcmmessage.RTCMMessage(**kwargs)
 ```
 
 You can create an `RTCMMessage` object by calling the constructor with the following keyword arguments:
 1. payload as bytes
 
 Example:
 
 ```python
->>> from pyrtcm import RTCMMessage
->>> msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
->>> print(msg)
+from pyrtcm import RTCMMessage
+msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
+print(msg)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `RTCMMessage` class implements a `serialize()` method to convert a `RTCMMessage` object to a bytes array suitable for writing to an output stream.
 
 e.g. to create and send a `1005` message type:
 
 ```python
->>> from serial import Serial
->>> serialOut = Serial('COM7', 38400, timeout=5)
->>> from pyrtcm import RTCMMessage
->>> msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
->>> print(msg)
+from serial import Serial
+from pyrtcm import RTCMMessage
+serialOut = Serial('COM7', 38400, timeout=5)
+msg = RTCMMessage(payload=b">\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH ")
+print(msg)
+output = msg.serialize()
+print(output)
+serialOut.write(output)
+```
+```
 <RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>
->>> output = msg.serialize()
->>> output
 b'\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7'
->>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
-1. `rtcmserial.py` - illustrates how to stream RTCM data from serial/UART port.
+1. `rtcmpoller.py` - illustrates how to read and display RTCM messages 'concurrently' with other tasks using threads and queues. This represents a useful generic pattern for many end user applications.
 1. `rtcmfile.py` - illustrates how to stream RTCM data from binary log file.
-1. `rtcmsocket.py` illustrates how to implement a TCP Socket reader for RTCM messages using RTCMReader iterator functionality.
-1. `rtcmbuild.py` - illustrates how to construct RTCM payload from constituent datafields.
-1. `ntripclient.py` - illustrates a simple [NTRIP](https://en.wikipedia.org/wiki/Networked_Transport_of_RTCM_via_Internet_Protocol) client using pyrtcm to parse the RTCM3 output.
+1. `rtcmsocket.py` - illustrates how to implement a TCP Socket reader for RTCM messages using RTCMReader iterator functionality.
+1. `msmparser.py` - illustrates how to parse RTCM3 MSM (multiple signal messages) into a series of iterable data arrays keyed on satellite PRN and signal ID.
+1. `rtcm_ntrip_client.py` - illustrates a simple [NTRIP](https://en.wikipedia.org/wiki/Networked_Transport_of_RTCM_via_Internet_Protocol) client using pyrtcm to parse the RTCM3 output.
 
 ---
 ## <a name="extensibility">Extensibility</a>
 
 The RTCM protocol is principally defined in the modules `rtcmtypes_core.py` and `rtcmtypes_get.py` as a series of dictionaries. RTCM uses a series of pre-defined data fields ("DF002", DF003" etc.), each of which has a designated data type (UINT32, etc.). Message payload definitions must conform to the following rules:
 
 ```
@@ -314,15 +361,15 @@
 ```
 gnssdump -h
 ```
 
 ---
 ## <a name="gui">Graphical Client</a>
 
-A python/tkinter graphical GPS client which supports NMEA, UBX and RTCM3 protocols is available at: 
+A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3, NTRIP and SPARTN protocols is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
 
 ---
 ## <a name="author">Author & License Information</a>
 
 semuadmin@semuconsulting.com
```

### Comparing `pyrtcm-1.0.9/src/pyrtcm.egg-info/SOURCES.txt` & `pyrtcm-1.1.0/src/pyrtcm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,10 +15,9 @@
 src/pyrtcm.egg-info/PKG-INFO
 src/pyrtcm.egg-info/SOURCES.txt
 src/pyrtcm.egg-info/dependency_links.txt
 src/pyrtcm.egg-info/requires.txt
 src/pyrtcm.egg-info/top_level.txt
 tests/test_definitions.py
 tests/test_socket.py
-tests/test_specialcases.py
 tests/test_static.py
 tests/test_stream.py
```

### Comparing `pyrtcm-1.0.9/tests/test_definitions.py` & `pyrtcm-1.1.0/tests/test_definitions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Test for errors in datafield and payload definitions
 
 Created on 19 Feb 2022
 
 @author: semuadmin
 """
+
 # pylint: disable=line-too-long, invalid-name, missing-docstring, no-member
 
 import os
 import sys
 import unittest
 
 ROOT = os.path.join(os.path.dirname(os.path.abspath(__file__)), "..")
@@ -25,13 +26,13 @@
         pass
 
     def testpayloaddfs(
         self,
     ):  # test all payload datafields are defined in RTCM_DATA_FIELDS
         for _, pdict in RTCM_PAYLOADS_GET.items():
             for df, _ in pdict.items():
-                if df[0:5] != "group":
+                if df[0:3] not in ("gro", "opt"):
                     self.assertIn(df, RTCM_DATA_FIELDS)
 
     def testdfres(self):  # test all resolution values are int or float
         for _, (_, res, _) in RTCM_DATA_FIELDS.items():
             self.assertIsInstance(res, (int, float))
```

### Comparing `pyrtcm-1.0.9/tests/test_socket.py` & `pyrtcm-1.1.0/tests/test_socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,35 +62,35 @@
 
     # *******************************************
     # Helper methods
     # *******************************************
 
     def testSocketStub(self):
         EXPECTED_RESULTS = (
-            "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108, DF364=0, DF027=3975521.4643)>",
-            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
+            "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108000005, DF364=0, DF027=3975521.4643)>",
+            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.802800001, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
             "<RTCM(1065, DF002=1065, DF386=12345, DF391=3, DF388=0, DF413=1, DF414=1, DF415=1, DF387=2, DF384_01=23, DF379_01=2, DF381_01_01=4, DF383_01_01=0.07, DF381_01_02=2, DF383_01_02=0.09, DF384_02=26, DF379_02=1, DF381_02_01=3, DF383_02_01=0.05)>",
-            "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108, DF364=0, DF027=3975521.4643)>",
-            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
+            "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108000005, DF364=0, DF027=3975521.4643)>",
+            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.802800001, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
             "<RTCM(1065, DF002=1065, DF386=12345, DF391=3, DF388=0, DF413=1, DF414=1, DF415=1, DF387=2, DF384_01=23, DF379_01=2, DF381_01_01=4, DF383_01_01=0.07, DF381_01_02=2, DF383_01_02=0.09, DF384_02=26, DF379_02=1, DF381_02_01=3, DF383_02_01=0.05)>",
-            "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108, DF364=0, DF027=3975521.4643)>",
-            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
+            "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108000005, DF364=0, DF027=3975521.4643)>",
+            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.802800001, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
             "<RTCM(1065, DF002=1065, DF386=12345, DF391=3, DF388=0, DF413=1, DF414=1, DF415=1, DF387=2, DF384_01=23, DF379_01=2, DF381_01_01=4, DF383_01_01=0.07, DF381_01_02=2, DF383_01_02=0.09, DF384_02=26, DF379_02=1, DF381_02_01=3, DF383_02_01=0.05)>",
-            "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108, DF364=0, DF027=3975521.4643)>",
-            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.8028, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
+            "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108000005, DF364=0, DF027=3975521.4643)>",
+            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.802800001, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
             "<RTCM(1065, DF002=1065, DF386=12345, DF391=3, DF388=0, DF413=1, DF414=1, DF415=1, DF387=2, DF384_01=23, DF379_01=2, DF381_01_01=4, DF383_01_01=0.07, DF381_01_02=2, DF383_01_02=0.09, DF384_02=26, DF379_02=1, DF381_02_01=3, DF383_02_01=0.05)>",
         )
         raw = None
         stream = DummySocket()
         rtr = RTCMReader(stream, bufsize=512)
         buff = rtr._stream.buffer  # test buffer getter method
         i = 0
         for raw, parsed in rtr:
             if raw is not None:
-                # print(parsed)
+                # print(f'"{parsed},"')
                 self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
                 i += 1
                 if i >= 12:
                     break
         self.assertEqual(i, 12)
 
     def testSocketIter(self):  # test for extended stream
```

