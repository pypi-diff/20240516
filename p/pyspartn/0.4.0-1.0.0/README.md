# Comparing `tmp/pyspartn-0.4.0.tar.gz` & `tmp/pyspartn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspartn-0.4.0.tar", last modified: Wed May  1 09:03:42 2024, max compression
+gzip compressed data, was "pyspartn-1.0.0.tar", last modified: Thu May 16 07:25:07 2024, max compression
```

## Comparing `pyspartn-0.4.0.tar` & `pyspartn-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.523066 pyspartn-0.4.0/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-25 22:03:47.000000 pyspartn-0.4.0/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-25 22:03:47.000000 pyspartn-0.4.0/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    24138 2024-05-01 09:03:42.522686 pyspartn-0.4.0/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    20628 2024-05-01 09:01:22.000000 pyspartn-0.4.0/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2446 2024-05-01 09:01:22.000000 pyspartn-0.4.0/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-01 09:03:42.523133 pyspartn-0.4.0/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.511465 pyspartn-0.4.0/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.514387 pyspartn-0.4.0/src/pyspartn/
--rw-r--r--   0 steve      (501) staff       (20)      598 2024-04-25 22:03:47.000000 pyspartn-0.4.0/src/pyspartn/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2024-05-01 09:01:22.000000 pyspartn-0.4.0/src/pyspartn/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      671 2024-04-25 22:03:47.000000 pyspartn-0.4.0/src/pyspartn/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     2441 2024-04-25 22:03:47.000000 pyspartn-0.4.0/src/pyspartn/socket_stream.py
--rw-r--r--   0 steve      (501) staff       (20)     8987 2024-05-01 09:01:22.000000 pyspartn-0.4.0/src/pyspartn/spartnhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    18499 2024-04-30 06:27:38.000000 pyspartn-0.4.0/src/pyspartn/spartnmessage.py
--rw-r--r--   0 steve      (501) staff       (20)    11496 2024-05-01 09:01:22.000000 pyspartn-0.4.0/src/pyspartn/spartnreader.py
--rw-r--r--   0 steve      (501) staff       (20)     4010 2024-04-26 07:17:19.000000 pyspartn-0.4.0/src/pyspartn/spartntables.py
--rw-r--r--   0 steve      (501) staff       (20)     9370 2024-05-01 09:01:22.000000 pyspartn-0.4.0/src/pyspartn/spartntypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    25860 2024-04-30 06:27:38.000000 pyspartn-0.4.0/src/pyspartn/spartntypes_get.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.521522 pyspartn-0.4.0/src/pyspartn.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    24138 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      576 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      134 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        9 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.520675 pyspartn-0.4.0/tests/
--rw-r--r--   0 steve      (501) staff       (20)     4043 2024-04-25 22:03:47.000000 pyspartn-0.4.0/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     8764 2024-05-01 09:01:22.000000 pyspartn-0.4.0/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)   207798 2024-05-01 09:01:22.000000 pyspartn-0.4.0/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 07:25:07.172824 pyspartn-1.0.0/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2024-05-07 14:54:46.000000 pyspartn-1.0.0/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2024-05-07 14:54:46.000000 pyspartn-1.0.0/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    24869 2024-05-16 07:25:07.172542 pyspartn-1.0.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    21351 2024-05-16 07:23:23.000000 pyspartn-1.0.0/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2608 2024-05-16 07:23:23.000000 pyspartn-1.0.0/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-16 07:25:07.172873 pyspartn-1.0.0/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 07:25:07.167408 pyspartn-1.0.0/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 07:25:07.169844 pyspartn-1.0.0/src/pyspartn/
+-rw-r--r--   0 steve      (501) staff       (20)      635 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      671 2024-05-07 14:54:46.000000 pyspartn-1.0.0/src/pyspartn/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     2521 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/socket_stream.py
+-rw-r--r--   0 steve      (501) staff       (20)     9403 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/spartnhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    20003 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/spartnmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)    11108 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/spartnreader.py
+-rw-r--r--   0 steve      (501) staff       (20)     5740 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/spartntables.py
+-rw-r--r--   0 steve      (501) staff       (20)     9533 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/spartntypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    27755 2024-05-16 07:23:23.000000 pyspartn-1.0.0/src/pyspartn/spartntypes_get.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 07:25:07.171661 pyspartn-1.0.0/src/pyspartn.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    24869 2024-05-16 07:25:07.000000 pyspartn-1.0.0/src/pyspartn.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      576 2024-05-16 07:25:07.000000 pyspartn-1.0.0/src/pyspartn.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-16 07:25:07.000000 pyspartn-1.0.0/src/pyspartn.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      134 2024-05-16 07:25:07.000000 pyspartn-1.0.0/src/pyspartn.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        9 2024-05-16 07:25:07.000000 pyspartn-1.0.0/src/pyspartn.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 07:25:07.171228 pyspartn-1.0.0/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     4659 2024-05-16 07:23:23.000000 pyspartn-1.0.0/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)     9007 2024-05-16 07:23:23.000000 pyspartn-1.0.0/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)   234707 2024-05-16 07:23:23.000000 pyspartn-1.0.0/tests/test_stream.py
```

### Comparing `pyspartn-0.4.0/LICENSE` & `pyspartn-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspartn-0.4.0/PKG-INFO` & `pyspartn-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.4.0
+Version: 1.0.0
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -32,15 +32,15 @@
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/semuconsulting/pyspartn
 Project-URL: documentation, https://www.semuconsulting.com/pyspartn/
 Project-URL: repository, https://github.com/semuconsulting/pyspartn
 Project-URL: changelog, https://github.com/semuconsulting/pyspartn/blob/master/RELEASE_NOTES.md
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
@@ -53,15 +53,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cryptography>=39.0.2
+Requires-Dist: cryptography>=42.0.0
 Provides-Extra: deploy
 Requires-Dist: build; extra == "deploy"
 Requires-Dist: pip; extra == "deploy"
 Requires-Dist: setuptools>=66.0; extra == "deploy"
 Requires-Dist: wheel; extra == "deploy"
 Provides-Extra: test
 Requires-Dist: bandit; extra == "test"
@@ -97,16 +97,14 @@
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy;, UBX &copy; (u-blox) and RTCM3 &copy; GNSS/GPS messages:
 - [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 - [pyrtcm](http://github.com/semuconsulting/pyrtcm)
 
 ## <a name="currentstatus">Current Status</a>
 
-**CURRENTLY IN BETA**
-
 ![Status](https://img.shields.io/pypi/status/pyspartn)
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyspartn?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
@@ -150,17 +148,15 @@
 python3 -m virtualenv env
 source env/bin/activate (or env\Scripts\activate on Windows)
 (env) python3 -m pip install --upgrade pyspartn
 ...
 deactivate
 ```
 
-*¹* On some 32-bit Linux platforms (e.g. Raspberry Pi OS 32), it may be necessary to [install Rust compiler support](https://www.rust-lang.org/tools/install) in order to install the `cryptography` library which `pyspartn` depends on to decrypt SPARTN messages (see [Discussion](https://github.com/semuconsulting/PyGPSClient/discussions/83#discussioncomment-6635558)):
-
-See [cryptography install README](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
+*¹* On some 32-bit Linux platforms (e.g. Raspberry Pi OS 32), it may be necessary to [install Rust compiler support](https://www.rust-lang.org/tools/install) in order to install the `cryptography` library which `pyspartn` depends on to decrypt SPARTN messages. See [cryptography install README](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
 
 
 For [Conda](https://docs.conda.io/en/latest/) users, `pyspartn` is also available from [conda-forge](https://github.com/conda-forge/pyspartn-feedstock):
 
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyspartn/badges/version.svg)](https://anaconda.org/conda-forge/pyspartn)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyspartn/badges/downloads.svg)](https://anaconda.org/conda-forge/pyspartn)
 
@@ -173,78 +169,80 @@
 
 ```
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
-or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
+or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams.
 
 Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
-stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
-spr = SPARTNReader(stream)
-(raw_data, parsed_data) = spr.read()
-print(parsed_data)
+with Serial('/dev/tty.usbmodem14101', 38400, timeout=3) as stream:
+   spr = SPARTNReader(stream)
+   raw_data, parsed_data = spr.read()
+   print(parsed_data)
 ```
 
 Example - File input (using iterator).
 ```python
 from pyspartn import SPARTNReader
-stream = open('spartndata.log', 'rb')
-spr = SPARTNReader(stream)
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with open('spartndata.log', 'rb') as stream:
+   spr = SPARTNReader(stream)
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
 import socket
 from pyspartn import SPARTNReader
-stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
-stream.connect(("localhost", 50007))
-spr = SPARTNReader(stream)
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as stream:
+   stream.connect(("localhost", 50007))
+   spr = SPARTNReader(stream)
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
-Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit `gnssTimetag` (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the UTC datetime on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the UTC datetime on which the datastream was originally created to the nearest half day. `pyspartn` can derive the requisite `basedate` from any 32-bit `gnssTimetag` for the same message subtype, but this is dependent on the datastream containing such 32-bit timetags. See examples below.
 
-The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
+The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need updating every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
-stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
-spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
+   spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 Example - Historical file input with decryption.
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader
-stream = open('spartndata.log', 'rb')
-spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+
+with open('spartndata.log', 'rb') as stream:
+   spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255, tzinfo=timezone.utc))
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
+
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and UTC `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
 Example - without payload decryption or decoding:
 
 ```python
 from pyspartn import SPARTNReader
@@ -256,62 +254,68 @@
 ```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader
 
 transport = b"\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80"
 msg = SPARTNReader.parse(
     transport,
     decode=1,
     key="6b30302427df05b4d98911ebff3a4d95",
-    basedate=datetime(2023, 6, 27, 22, 3, 0),
+    basedate=datetime(2023, 6, 27, 22, 3, 0, tzinfo=timezone.utc),
 )
 print(msg)
 ```
 ```
 <SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader, datadesc
-msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
+msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255, tzinfo=timezone.utc))
 print(msg)
 print(msg.identity)
 print(msg.gnssTimeTag)
 print(datadesc("SF005"), msg.SF005)
 print(datadesc("SF061a"), msg.SF061a_10_05)
 ```
 ```
 <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 'SPARTN-1X-HPAC-GPS'
 451165680
 ('Solution issue of update (SIOU)', 152)
 ('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
-Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
+Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. See [examples below](#iterating) for illustrations of how to iterate through grouped attributes.
+
+Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
+
+The `payload` attribute always contains the raw payload as bytes.
+
+#### <a name="iterating">Iterating Through Group Attributes</a>
+
+To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
 
 ```python
 vals = []
 for i in range(parsed_data.SF030 + 1):  # attribute or formula representing group size
     vals.append(getattr(parsed_data, f"SF032_{i+1:02d}"))
 print(vals)
 ```
 
-Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
-
-The `payload` attribute always contains the raw payload as bytes.
+See examples `parse_ocb.py`, `parse_hpac.py` and `parse_gad.py` for illustrations of how to convert parsed and decoded OCB, HPAC and GAD payloads into iterable data structures.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyspartn.spartnmessage.SPARTNMessage(**kwargs)
 ```
@@ -353,22 +357,23 @@
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
-1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the pygnssutils.GNSSMQTTClient class. **NB**: requires a valid ClientID for a
+1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from a binary SPARTN datastream.
+1. `spartn_decrypt.py` - illustrates how to decrypt and parse a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples below).
+1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the [`pygnssutils.GNSSMQTTClient`](https://github.com/semuconsulting/pygnssutils?tab=readme-ov-file#gnssmqttclient) class. **NB**: requires a valid ClientID for a
 SPARTN MQTT service e.g. u-blox Thingstream PointPerfect MQTT.
-1. `spartn_ntrip_client.py` - implements a simple SPARTN NTRIP client using the pygnssutils.GNSSNTRIPClient class. **NB**: requires a valid user and password for a
+1. `spartn_ntrip_client.py` - implements a simple SPARTN NTRIP client using the [`pygnssutils.GNSSNTRIPClient`](https://github.com/semuconsulting/pygnssutils?tab=readme-ov-file#gnssntripclient) class. **NB**: requires a valid user and password for a
 SPARTN NTRIP service e.g. u-blox Thingstream PointPerfect NTRIP.
-1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
-1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
-1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
+1. `parse_gad.py` - illustrates how to convert parsed GAD message types into WKT area polygon format for display on a map (see, for example, `gad_plot_map.png`).
+1. `parse_hpac.py` and `parse_ocb.py` - illustrate how to convert parsed HPAC and OCB message types into iterable data structures.
 
 ---
 ## <a name="troubleshooting">Troubleshooting</a>
 
 1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
 
    ```
```

### Comparing `pyspartn-0.4.0/README.md` & `pyspartn-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy;, UBX &copy; (u-blox) and RTCM3 &copy; GNSS/GPS messages:
 - [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 - [pyrtcm](http://github.com/semuconsulting/pyrtcm)
 
 ## <a name="currentstatus">Current Status</a>
 
-**CURRENTLY IN BETA**
-
 ![Status](https://img.shields.io/pypi/status/pyspartn)
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyspartn?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
@@ -76,17 +74,15 @@
 python3 -m virtualenv env
 source env/bin/activate (or env\Scripts\activate on Windows)
 (env) python3 -m pip install --upgrade pyspartn
 ...
 deactivate
 ```
 
-*¹* On some 32-bit Linux platforms (e.g. Raspberry Pi OS 32), it may be necessary to [install Rust compiler support](https://www.rust-lang.org/tools/install) in order to install the `cryptography` library which `pyspartn` depends on to decrypt SPARTN messages (see [Discussion](https://github.com/semuconsulting/PyGPSClient/discussions/83#discussioncomment-6635558)):
-
-See [cryptography install README](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
+*¹* On some 32-bit Linux platforms (e.g. Raspberry Pi OS 32), it may be necessary to [install Rust compiler support](https://www.rust-lang.org/tools/install) in order to install the `cryptography` library which `pyspartn` depends on to decrypt SPARTN messages. See [cryptography install README](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
 
 
 For [Conda](https://docs.conda.io/en/latest/) users, `pyspartn` is also available from [conda-forge](https://github.com/conda-forge/pyspartn-feedstock):
 
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyspartn/badges/version.svg)](https://anaconda.org/conda-forge/pyspartn)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyspartn/badges/downloads.svg)](https://anaconda.org/conda-forge/pyspartn)
 
@@ -99,78 +95,80 @@
 
 ```
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
-or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
+or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams.
 
 Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
-stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
-spr = SPARTNReader(stream)
-(raw_data, parsed_data) = spr.read()
-print(parsed_data)
+with Serial('/dev/tty.usbmodem14101', 38400, timeout=3) as stream:
+   spr = SPARTNReader(stream)
+   raw_data, parsed_data = spr.read()
+   print(parsed_data)
 ```
 
 Example - File input (using iterator).
 ```python
 from pyspartn import SPARTNReader
-stream = open('spartndata.log', 'rb')
-spr = SPARTNReader(stream)
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with open('spartndata.log', 'rb') as stream:
+   spr = SPARTNReader(stream)
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
 import socket
 from pyspartn import SPARTNReader
-stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
-stream.connect(("localhost", 50007))
-spr = SPARTNReader(stream)
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as stream:
+   stream.connect(("localhost", 50007))
+   spr = SPARTNReader(stream)
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
-Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit `gnssTimetag` (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the UTC datetime on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the UTC datetime on which the datastream was originally created to the nearest half day. `pyspartn` can derive the requisite `basedate` from any 32-bit `gnssTimetag` for the same message subtype, but this is dependent on the datastream containing such 32-bit timetags. See examples below.
 
-The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
+The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need updating every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
-stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
-spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
+   spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 Example - Historical file input with decryption.
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader
-stream = open('spartndata.log', 'rb')
-spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+
+with open('spartndata.log', 'rb') as stream:
+   spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255, tzinfo=timezone.utc))
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
+
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and UTC `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
 Example - without payload decryption or decoding:
 
 ```python
 from pyspartn import SPARTNReader
@@ -182,62 +180,68 @@
 ```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader
 
 transport = b"\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80"
 msg = SPARTNReader.parse(
     transport,
     decode=1,
     key="6b30302427df05b4d98911ebff3a4d95",
-    basedate=datetime(2023, 6, 27, 22, 3, 0),
+    basedate=datetime(2023, 6, 27, 22, 3, 0, tzinfo=timezone.utc),
 )
 print(msg)
 ```
 ```
 <SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader, datadesc
-msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
+msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255, tzinfo=timezone.utc))
 print(msg)
 print(msg.identity)
 print(msg.gnssTimeTag)
 print(datadesc("SF005"), msg.SF005)
 print(datadesc("SF061a"), msg.SF061a_10_05)
 ```
 ```
 <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 'SPARTN-1X-HPAC-GPS'
 451165680
 ('Solution issue of update (SIOU)', 152)
 ('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
-Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
+Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. See [examples below](#iterating) for illustrations of how to iterate through grouped attributes.
+
+Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
+
+The `payload` attribute always contains the raw payload as bytes.
+
+#### <a name="iterating">Iterating Through Group Attributes</a>
+
+To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
 
 ```python
 vals = []
 for i in range(parsed_data.SF030 + 1):  # attribute or formula representing group size
     vals.append(getattr(parsed_data, f"SF032_{i+1:02d}"))
 print(vals)
 ```
 
-Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
-
-The `payload` attribute always contains the raw payload as bytes.
+See examples `parse_ocb.py`, `parse_hpac.py` and `parse_gad.py` for illustrations of how to convert parsed and decoded OCB, HPAC and GAD payloads into iterable data structures.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyspartn.spartnmessage.SPARTNMessage(**kwargs)
 ```
@@ -279,22 +283,23 @@
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
-1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the pygnssutils.GNSSMQTTClient class. **NB**: requires a valid ClientID for a
+1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from a binary SPARTN datastream.
+1. `spartn_decrypt.py` - illustrates how to decrypt and parse a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples below).
+1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the [`pygnssutils.GNSSMQTTClient`](https://github.com/semuconsulting/pygnssutils?tab=readme-ov-file#gnssmqttclient) class. **NB**: requires a valid ClientID for a
 SPARTN MQTT service e.g. u-blox Thingstream PointPerfect MQTT.
-1. `spartn_ntrip_client.py` - implements a simple SPARTN NTRIP client using the pygnssutils.GNSSNTRIPClient class. **NB**: requires a valid user and password for a
+1. `spartn_ntrip_client.py` - implements a simple SPARTN NTRIP client using the [`pygnssutils.GNSSNTRIPClient`](https://github.com/semuconsulting/pygnssutils?tab=readme-ov-file#gnssntripclient) class. **NB**: requires a valid user and password for a
 SPARTN NTRIP service e.g. u-blox Thingstream PointPerfect NTRIP.
-1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
-1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
-1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
+1. `parse_gad.py` - illustrates how to convert parsed GAD message types into WKT area polygon format for display on a map (see, for example, `gad_plot_map.png`).
+1. `parse_hpac.py` and `parse_ocb.py` - illustrate how to convert parsed HPAC and OCB message types into iterable data structures.
 
 ---
 ## <a name="troubleshooting">Troubleshooting</a>
 
 1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
 
    ```
```

### Comparing `pyspartn-0.4.0/pyproject.toml` & `pyspartn-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pyspartn"
 authors = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 maintainers = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 description = "SPARTN protocol parser"
-version = "0.4.0"
+version = "1.0.0"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: MacOS X",
     "Environment :: Win32 (MS Windows)",
     "Environment :: X11 Applications",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: End Users/Desktop",
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: BSD License",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 
-dependencies = ["cryptography>=39.0.2"]
+dependencies = ["cryptography>=42.0.0"]
 
 [project.urls]
 homepage = "https://github.com/semuconsulting/pyspartn"
 documentation = "https://www.semuconsulting.com/pyspartn/"
 repository = "https://github.com/semuconsulting/pyspartn"
 changelog = "https://github.com/semuconsulting/pyspartn/blob/master/RELEASE_NOTES.md"
 
@@ -81,12 +81,18 @@
     useless-suppression,
     deprecated-pragma,
     use-symbolic-message-instead,
 """
 
 [tool.pytest.ini_options]
 minversion = "7.0"
-addopts = "--cov --cov-report html --cov-fail-under 85"
+addopts = "--cov --cov-report html --cov-fail-under 90"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 source = ["src"]
+
+[tool.coverage.report]
+exclude_also = [
+    # "if self.authInd > 1:", # no current test data
+    # "if authInd > 1:",      # no current test data
+]
```

### Comparing `pyspartn-0.4.0/src/pyspartn/__init__.py` & `pyspartn-1.0.0/src/pyspartn/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,10 +14,11 @@
     SPARTNStreamError,
     SPARTNTypeError,
 )
 from pyspartn.socket_stream import SocketStream
 from pyspartn.spartnhelpers import *
 from pyspartn.spartnmessage import SPARTNMessage
 from pyspartn.spartnreader import SPARTNReader
+from pyspartn.spartntables import *
 from pyspartn.spartntypes_core import *
 
 version = __version__  # pylint: disable=invalid-name
```

### Comparing `pyspartn-0.4.0/src/pyspartn/exceptions.py` & `pyspartn-1.0.0/src/pyspartn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.4.0/src/pyspartn/socket_stream.py` & `pyspartn-1.0.0/src/pyspartn/socket_stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,27 +76,28 @@
         while len(self._buffer) < num:
             if not self._recv():
                 return b""
         data = self._buffer[:num]
         self._buffer = self._buffer[num:]
         return bytes(data)
 
-    def readline(self) -> bytes:
-        """
-        Read bytes from buffer until LF reached.
-        NB: always check that return data terminator is LF.
+    # Not relevant for SPARTN message streams
+    # def readline(self) -> bytes:
+    #     """
+    #     Read bytes from buffer until LF reached.
+    #     NB: always check that return data terminator is LF.
 
-        :return: bytes
-        :rtype: bytes
-        """
+    #     :return: bytes
+    #     :rtype: bytes
+    #     """
 
-        line = b""
-        while True:
-            data = self.read(1)
-            if len(data) == 1:
-                line += data
-                if line[-1:] == b"\n":  # LF
-                    break
-            else:
-                break
+    #     line = b""
+    #     while True:
+    #         data = self.read(1)
+    #         if len(data) == 1:
+    #             line += data
+    #             if line[-1:] == b"\n":  # LF
+    #                 break
+    #         else:
+    #             break
 
-        return line
+    #     return line
```

### Comparing `pyspartn-0.4.0/src/pyspartn/spartnhelpers.py` & `pyspartn-1.0.0/src/pyspartn/spartnhelpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 Created on 10 Feb 2023
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 
-# pylint: disable=invalid-name
-
 from datetime import datetime, timedelta, timezone
 
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
 from pyspartn.exceptions import SPARTNMessageError
 from pyspartn.spartntypes_core import FL, IN, SPARTN_DATA_FIELDS, TIMEBASE
 
@@ -81,14 +79,15 @@
     :param str typ: field type (i.e. Integer, Bitmask, Float)
     :param float res: field resolution (i.e. scaling factor)
     :param float rngmin: field range minimum value
     :return: value
     :rtype: int
     :raises: SPARTNMessageError if end of bitfield
     """
+    # pylint: disable=too-many-arguments
 
     lbb = len(bitfield) * 8
     if position + length > lbb:
         raise SPARTNMessageError(
             f"Attribute size {length} exceeds remaining payload length {lbb - position}"
         )
 
@@ -133,33 +132,33 @@
             if crc & (1 << n):
                 crc ^= g
 
     # Return the CRC value
     return crc ^ xor_out
 
 
-def valid_crc(msg: bytes, crc: int, crcType: int) -> bool:
+def valid_crc(msg: bytes, crc: int, crctype: int) -> bool:
     """
     Validate message CRC.
 
     :param bytes msg: message to which CRC applies
     :param int crc: message CRC
     :param int cycType: crc type (0-3)
     """
 
-    if crcType == 0:
+    if crctype == 0:
         crcchk = crc_poly(msg, 8, 0x07)
-    elif crcType == 1:
+    elif crctype == 1:
         crcchk = crc_poly(msg, 16, 0x1021)
-    elif crcType == 2:
+    elif crctype == 2:
         crcchk = crc_poly(msg, 24, 0x864CFB)
-    elif crcType == 3:
+    elif crctype == 3:
         crcchk = crc_poly(msg, 32, 0x04C11DB7, crc=0xFFFFFFFF, xor_out=0xFFFFFFFF)
     else:
-        raise ValueError(f"Invalid crcType: {crcType} - should be 0-3")
+        raise ValueError(f"Invalid crcType: {crctype} - should be 0-3")
     return crc == crcchk
 
 
 def encrypt(pt: bytes, key: bytes, iv: bytes, mode: str = "CTR") -> tuple:
     """
     Encrypt payload
     The length of the plaintext data must be a multiple of
@@ -176,18 +175,18 @@
 
     if mode == "CTR":
         cipher = Cipher(algorithms.AES(key), modes.CTR(iv))
     else:
         cipher = Cipher(algorithms.AES(key), modes.CBC(iv))
 
     pad = 16 - len(pt) % 16
-    PADDING_BYTE = pad.to_bytes(1, "big")
+    pad_byte = pad.to_bytes(1, "big")
 
     encryptor = cipher.encryptor()
-    ct = encryptor.update(pt + (pad * PADDING_BYTE)) + encryptor.finalize()
+    ct = encryptor.update(pt + (pad * pad_byte)) + encryptor.finalize()
     return ct, pad
 
 
 def decrypt(ct: bytes, key: bytes, iv: bytes, mode: str = "CTR") -> bytes:
     """
     Decrypt payload
 
@@ -265,15 +264,15 @@
     To convert to a 32-bit timetag, calculate number of seconds since TIMEBASE:
 
     (2023-06-27 21:03:00 - 2010-01-01 00:00:00) = 425595780 seconds
 
     All timetag16 are given in their respective constellation timezone :
     UTC = GPS + 18s = GAL + 18s = QZSS + 18s = BEI + 4s = GLO - 10800s
 
-    Since all timetags are in GNSS constellation time and basedate is timezone-naive,
+    Since all timetags are in GNSS constellation time and basedate is UTC,
     we calculate three possible 32-bit timetags : basedate, basedate plus half a day,
     basedate minus half a day, so all constellations and basedate time reference are tried.
     We then select the unambiguous resolution the closest in time to the original basedate.
 
     :param int timetag16: 16-bit gnssTimeTag
     :param datetime basedate: original processing datetime accurate to 3 hours
     :return: 32-bit gnssTimeTag
@@ -292,14 +291,30 @@
         floor_halfday_timetag + secs_half_day,
     ]
 
     closest_time_tag = min(time_options, key=lambda x: abs(x - basedate_seconds))
     return closest_time_tag
 
 
+def naive2aware(dt: datetime, tz: timezone = timezone.utc) -> datetime:
+    """
+    Convert naive datetime to aware.
+
+    :param datetime dt: datetime
+    :param timezone tz: timezone (utc)
+    :return: datetime object with UTC timezone
+    :rtype: datetime
+    """
+
+    if isinstance(dt, datetime):
+        if dt.tzinfo is None:  # add tz data if naive
+            return dt.replace(tzinfo=tz)
+    return dt
+
+
 def enc2float(value: int, res: float, rngmin: float = 0) -> float:
     """
     Convert encoded floating point value to float.
 
     SPARTN protocol stores floating point numbers in
     encoded integer format.
```

### Comparing `pyspartn-0.4.0/src/pyspartn/spartnmessage.py` & `pyspartn-1.0.0/src/pyspartn/spartnmessage.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,50 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 
 # pylint: disable=invalid-name too-many-instance-attributes
 
-from datetime import datetime
+from datetime import datetime, timezone
 from os import getenv
 
 from pyspartn.exceptions import (
     ParameterError,
     SPARTNMessageError,
     SPARTNParseError,
     SPARTNTypeError,
 )
 from pyspartn.spartnhelpers import (
     bitsval,
     convert_timetag,
     decrypt,
     escapeall,
+    naive2aware,
     timetag2date,
     valid_crc,
 )
+from pyspartn.spartntables import (
+    CBBITMASKKEY,
+    CBBITMASKLEN,
+    PBBITMASKKEY,
+    PBBITMASKLEN,
+    SATBITMASKKEY,
+    SATBITMASKLEN,
+    SF087_ENUM,
+)
 from pyspartn.spartntypes_core import (
     CBBMLEN,
+    CBS,
     FL,
+    NA,
     NB,
     PBBMLEN,
+    PBS,
+    PRN,
     SPARTN_DATA_FIELDS,
     SPARTN_MSGIDS,
     SPARTN_PRE,
     STBMLEN,
     VALCRC,
 )
 from pyspartn.spartntypes_get import SPARTN_PAYLOADS_GET
@@ -51,15 +65,15 @@
 
     def __init__(
         self,
         transport: bytes = None,
         validate: int = VALCRC,
         decode: bool = False,
         key: str = None,
-        basedate: object = None,
+        basedate: object = datetime.now(timezone.utc),
     ):
         """
         Constructor.
 
         :param bytes transport: SPARTN message transport (None)
         :param bool validate: validate CRC (True)
         :param bool decode: decrypt and decode payloads (False)
@@ -79,19 +93,23 @@
         self._preamble = bitsval(self._transport, 0, 8)
         if self._preamble != SPARTN_PRE:  # not SPARTN
             raise SPARTNParseError(f"Unknown message preamble {self._preamble}")
 
         self._validate = validate
         self._decode = decode
         self._padding = 0
-        basedate = datetime.now() if basedate is None else basedate
+        self._prnmap = []  # maps group index to satellite PRN
+        self._pbsmap = []  # maps group index to phase bias type
+        self._cbsmap = []  # maps group index to code bias type
+        basedate = datetime.now(timezone.utc) if basedate is None else basedate
         if isinstance(basedate, int):  # 32-bit gnssTimeTag
             self._basedate = timetag2date(basedate)
         else:  # datetime
-            self._basedate = basedate
+            self._basedate = naive2aware(basedate)
+
         key = getenv("MQTTKEY", None) if key is None else key
         self._key = None if key is None else bytes.fromhex(key)
         self._iv = None
 
         if self._decode and self._key is None:
             raise ParameterError("Key must be provided if decoding is enabled")
 
@@ -165,30 +183,30 @@
         # decrypt payload if encrypted
         if self.eaf and self._decode:
             iv = self._get_iv()
             self._payload = decrypt(payload, self._key, iv)
         else:
             self._payload = payload
 
-        key = ""
+        anam = ""
         try:
             if self._decode:
                 pdict = (
                     self._get_dict()
                 )  # get payload definition dict for this message identity
                 if pdict is None:  # unknown (or not yet implemented) message identity
                     self._do_unknown()
                     return
-                for key in pdict:  # process each attribute in dict
-                    (offset, index) = self._set_attribute(offset, pdict, key, index)
+                for anam in pdict:  # process each attribute in dict
+                    (offset, index) = self._set_attribute(anam, pdict, offset, index)
                 self._padding = self.nData * 8 - offset  # byte alignment padding
         except Exception as err:
             raise SPARTNTypeError(
                 (
-                    f"Error processing attribute '{key}' "
+                    f"Error processing attribute '{anam}' "
                     f"in message type {self.identity}"
                 )
             ) from err
 
     def _get_iv(self) -> bytes:
         """
         Create 128-bit Encryption Initialisation Vector.
@@ -206,170 +224,188 @@
             (self.msgType << 121)  # TF002 7 bits
             + (self.nData << 111)  # TF003 10 bits
             + (self.msgSubtype << 107)  # TF007 4 bits
             + (timeTag << 75)  # TF009 32 bits
             + (self.solutionId << 68)  # TF010 7 bits
             + (self.solutionProcId << 64)  # TF011 4 bits
             + (self.encryptionId << 60)  # TF012 4 bits
-            + (self.encryptionSeq << 54)  # TF012 6 bits
+            + (self.encryptionSeq << 54)  # TF013 6 bits
             + 1  # padding to 128 bits
         )
         return iv.to_bytes(16, "big")
 
-    def _set_attribute(self, offset: int, pdict: dict, key: str, index: list) -> tuple:
+    def _set_attribute(self, anam: str, pdict: dict, offset: int, index: list) -> tuple:
         """
         Recursive routine to set individual, optional or grouped payload attributes.
 
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
-        if isinstance(att, tuple):  # attribute group
-            siz, _ = att
-            if isinstance(siz, tuple):  # conditional group of attributes
-                (offset, index) = self._set_attribute_optional(att, offset, index)
+        adef = pdict[anam]  # get attribute definition
+        if isinstance(adef, tuple):  # attribute group
+            gsiz, _ = adef
+            if isinstance(gsiz, tuple):  # conditional group of attributes
+                (offset, index) = self._set_attribute_optional(adef, offset, index)
             else:  # repeating group of attributes
-                (offset, index) = self._set_attribute_group(att, offset, index)
+                (offset, index) = self._set_attribute_group(adef, offset, index)
         else:  # single attribute
-            offset = self._set_attribute_single(att, offset, key, index)
+            offset = self._set_attribute_single(anam, offset, index)
 
         return (offset, index)
 
-    def _set_attribute_optional(self, attg: tuple, offset: int, index: list) -> tuple:
+    def _set_attribute_optional(self, adef: tuple, offset: int, index: list) -> tuple:
         """
         Process optional group of attributes, subject to condition being met:
         a) group is present if attribute value = specific value, otherwise absent
         b) group is present if attribute value is in specific range, otherwise absent
 
-        :param tuple attg: attribute group - tuple of ((attribute name, condition), group dict)
+        :param tuple adef: attribute definition - tuple of ((attribute name, condition), group dict)
         :param int offset: payload offset in bits
         :param list index: repeating group index array
         :return: (offset, index[])
         :rtype: tuple
         """
 
         pres = False
-        (numr, con), gdict = attg  # (attribute, condition), group dictionary
+        (anam, con), gdict = adef  # (attribute, condition), group dictionary
         # "+n" suffix signifies that one or more nested group indices
         # must be appended to name e.g. "DF379_01", "IDF023_03"
-        if "+" in numr:
-            numr, nestlevel = numr.split("+")
+        if "+" in anam:
+            anam, nestlevel = anam.split("+")
             for i in range(int(nestlevel)):
-                numr += f"_{index[i]:02d}"
+                anam += f"_{index[i]:02d}"
         if isinstance(con, int):  # present if attribute == value
-            pres = getattr(self, numr) == con
+            pres = getattr(self, anam) == con
         elif isinstance(con, list):  # present if attribute in range of values
-            pres = getattr(self, numr) in con
+            pres = getattr(self, anam) in con
 
-        # recursively process each group attribute,
-        # incrementing the payload offset as we go
-        if pres:
-            for key1 in gdict:
-                (offset, index) = self._set_attribute(offset, gdict, key1, index)
+        if pres:  # if the conditional element is present...
+            # recursively process each group attribute,
+            # incrementing the payload offset as we go
+            for anami in gdict:
+                (offset, index) = self._set_attribute(anami, gdict, offset, index)
 
         return (offset, index)
 
-    def _set_attribute_group(self, attg: tuple, offset: int, index: list) -> tuple:
+    def _set_attribute_group(self, adef: tuple, offset: int, index: list) -> tuple:
         """
         Process (nested) group of attributes. Group size (number of repeats)
         can be signified in a number of ways:
         a) size = fixed integer
         b) size = value of named attribute e.g. SF030
         c) size = number of bits set in named attribute e.g. SF011
 
-        :param tuple attg: attribute group - tuple of (size, group dict)
+        :param tuple adef: attribute definition - tuple of (attribute name, group dict)
         :param int offset: payload offset in bits
         :param list index: repeating group index array
         :return: (offset, index[])
         :rtype: tuple
         """
 
         index.append(0)
-        numr, gdict = attg  # size, group dictionary
+        anam, gdict = adef  # attribute signifying group size, group dictionary
 
         # derive or retrieve number of items in group
-        if isinstance(numr, int):  # repeats = fixed integer
-            rng = numr
-        elif isinstance(numr, str):  # repeats defined in named attribute
+        if isinstance(anam, int):  # repeats = fixed integer
+            gsiz = anam
+        elif isinstance(anam, str):  # repeats defined in named attribute
             # "+n" suffix signifies that one or more nested group indices
             # must be appended to name e.g. "DF379_01", "IDF023_03"
-            if "+" in numr:
-                numr, nestlevel = numr.split("+")
+            if "+" in anam:
+                anam, nestlevel = anam.split("+")
                 for i in range(int(nestlevel)):
-                    numr += f"_{index[i]:02d}"
-            if numr[0:3] == NB:  # repeats = num bits set
-                rng = bin(getattr(self, numr[3:])).count("1")
+                    anam += f"_{index[i]:02d}"
+            if anam[0:3] == NB:  # repeats = num bits set
+                gsiz = bin(getattr(self, anam[3:])).count("1")
             else:
-                rng = getattr(self, numr)  # repeats = attribute value
-                if numr in ("SF030", "SF071"):
-                    rng += 1
+                gsiz = getattr(self, anam)  # repeats = attribute value
+                if anam in ("SF030", "SF071"):
+                    gsiz += 1
 
         # recursively process each group attribute,
         # incrementing the payload offset and index as we go
-        for i in range(rng):
+        for i in range(gsiz):
             index[-1] = i + 1
-            for key1 in gdict:
-                (offset, index) = self._set_attribute(offset, gdict, key1, index)
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
         Set individual attribute value.
 
-        :param str att: attribute type string e.g. 'INT008'
+        :param str anam: attribute keyword
         :param int offset: payload offset in bits
-        :param str key: attribute keyword
         :param list index: repeating group index array
         :return: offset
         :rtype: int
         """
-        # pylint: disable=no-member
 
         # if attribute is part of a (nested) repeating group, suffix name with index
-        keyr = key
+        anami = anam
         for i in index:  # one index for each nested level
             if i > 0:
-                keyr += f"_{i:02d}"
+                anami += f"_{i:02d}"
 
         # get value of required number of bits at current payload offset
         # (attribute length, resolution, minimum, description)
-        attinfo = SPARTN_DATA_FIELDS[key]
+        attinfo = SPARTN_DATA_FIELDS[anam]
         attlen = attinfo[0]
         atttyp = attinfo[1]  # IN, EN, BM, FL
         if isinstance(attlen, str):  # variable length attribute
-            attlen = self._getvarlen(key, index)
+            attlen = self._getvarlen(anam, index)
         try:
-            if atttyp == FL:
+            if atttyp == PRN:
+                val = self._prnmap[index[-1] - 1]
+            elif atttyp == PBS:
+                val = self._pbsmap[index[-1] - 1]
+            elif atttyp == CBS:
+                val = self._cbsmap[index[-1] - 1]
+            elif atttyp == FL:
                 res = attinfo[2]  # resolution (i.e. scaling factor)
                 rngmin = attinfo[3]  # range minimum
                 val = bitsval(self._payload, offset, attlen, atttyp, res, rngmin)
             else:
                 val = bitsval(self._payload, offset, attlen, atttyp)
         except SPARTNMessageError as err:
             # print(self)
             raise err
 
-        setattr(self, keyr, val)
+        setattr(self, anami, val)
 
         offset += attlen
 
+        # if attribute represents bitmask, populate
+        # corresponding map table
+        if anam in SATBITMASKKEY.values():
+            self._prnmap = self._getbitmask(
+                index, STBMLEN, SATBITMASKKEY, SATBITMASKLEN
+            )  # satellite PRN
+        elif anam in PBBITMASKKEY.values():
+            self._pbsmap = self._getbitmask(
+                index, PBBMLEN, PBBITMASKKEY, PBBITMASKLEN
+            )  # phase bias type
+        elif anam in CBBITMASKKEY.values():
+            self._cbsmap = self._getbitmask(
+                index, CBBMLEN, CBBITMASKKEY, CBBITMASKLEN
+            )  # code bias type
+
         return offset
 
     def _get_dict(self) -> dict:
         """
         Get payload dictionary corresponding to message identity
         (or None if message type not defined)
 
@@ -388,72 +424,80 @@
         value of preceeding bits.
 
         :param str keyr: name of attribute
         :param list index: nested group index
         :return: length of attribute in bits
         :rtype: int
         """
-        # pylint: disable=no-member, too-many-branches
+
+        # pylint: disable=no-member
 
         # if within repeating group, append nested index
         if len(index) > 0:
             sfx = f"_{index[-1]:02d}"
         else:
             sfx = ""
         attl = 0
-        # satellite bitmasks
-        if key in ("SF011", "SF012", "SF093", "SF094", "SF095"):
-            sflen = getattr(self, STBMLEN + sfx)
-            if key == "SF011":  # GPS satellite mask
-                attl = [32, 44, 56, 64][sflen]
-            elif key == "SF012":  # GLONASS Satellite mask
-                attl = [24, 36, 48, 63][sflen]
-            elif key == "SF093":  # Galileo satellite mask
-                attl = [36, 45, 54, 64][sflen]
-            elif key == "SF094":  # BDS satellite mask
-                attl = [37, 46, 55, 64][sflen]
-            elif key == "SF095":  # QZSS satellite mask
-                attl = [10, 40, 48, 64][sflen]
-        # phase bias bitmasks
-        elif key in ("SF025", "SF026", "SF102", "SF103", "SF104"):
-            sflen = getattr(self, PBBMLEN + sfx)
-            if key == "SF025":  # GPS phase bias mask
-                attl = [6, 11][sflen]
-            elif key == "SF026":  # GLONASS phase bias mask
-                attl = [5, 9][sflen]
-            elif key == "SF102":  # Galileo phase bias mask
-                attl = [8, 15][sflen]
-            elif key == "SF103":  # BDS phase bias mask
-                attl = [8, 15][sflen]
-            elif key == "SF104":  # QZSS phase bias mask
-                attl = [6, 11][sflen]
-        # code bias bitmasks
-        elif key in ("SF027", "SF028", "SF105", "SF106", "SF107"):
-            sflen = getattr(self, CBBMLEN + sfx)
-            if key == "SF027":  # GPS code bias mask
-                attl = [6, 11][sflen]
-            elif key == "SF028":  # GLONASS code bias mask
-                attl = [5, 9][sflen]
-            elif key == "SF105":  # Galileo code bias mask
-                attl = [8, 15][sflen]
-            elif key == "SF106":  # BDS code bias mask
-                attl = [8, 15][sflen]
-            elif key == "SF107":  # QZSS code bias mask
-                attl = [6, 11][sflen]
+        if key in SATBITMASKKEY.values():  # satellite bitmasks
+            attl = SATBITMASKLEN[key][getattr(self, STBMLEN + sfx)]
+        elif key in PBBITMASKKEY.values():  # phase bias bitmasks
+            attl = PBBITMASKLEN[key][getattr(self, PBBMLEN + sfx)][0]
+        elif key in CBBITMASKKEY.values():  # code bias bitmasks
+            attl = CBBITMASKLEN[key][getattr(self, CBBMLEN + sfx)][0]
         elif key == "SF079":  # Grid node present mask
             attl = (getattr(self, f"SF075{sfx}") + 1) * (
                 getattr(self, f"SF076{sfx}") + 1
             )
         elif key == "SF088":  # Cryptographic Key length
-            attl = [96, 128, 192, 256, 512][self.SF087]
+            attl = SF087_ENUM[self.SF087]
         elif key == "SF092":  # Computed Authentication Data (CAD)
             attl = self.SF091
 
         return attl
 
+    def _getbitmask(self, index: list, bmlen: str, bmkeys: list, bmvals: list) -> list:
+        """
+        Map bitmask to values in repeating groups of satellite prn, phase bias
+        and code bias.
+
+        :param str index: group index
+        :param str bmlen: name of attribute containing bitmask length
+        :param list bmkeys: list of bitmask attribute names for each gnss
+        :param list bmvals: list of bitmask lengths and values
+        :return: list of values
+        :rtype: list
+        """
+
+        mode = PRN if bmlen == STBMLEN else PBS
+        bm = bmkeys[self.identity[-3:]]  # bitmask name for this gnss
+        if mode == PRN and "OCB" in self.identity:
+            # OCB PRN bitmasks are at root level
+            idx = ""
+        else:
+            # HPAC PRN and OCB phase/code bias bitmasks are nested one level deep
+            idx = f"_{index[0]:02d}"
+        bmi = bm + idx  # name of attribute containing bitmask
+        bml = bmlen + idx  # name of attribute containing bitmask length
+
+        bmval = getattr(self, bmi)  # value of bitmask
+        if mode == PRN:
+            bmlval = bmvals[bm][getattr(self, bml)]  # length of bitmask
+        else:
+            bmlval = bmvals[bm][0][getattr(self, bml)]  # length of bitmask
+        vals = []
+        for i in range(bmlval):  # check set bits from left to right
+            if bmval >> (bmlval - 1 - i) & 1:
+                if mode == PRN:
+                    val = i + 1
+                else:
+                    val = bmvals[bm][1].get(i, NA)
+                vals.append(val)
+        # print(f"\nDEBUG phase bias map = {bmval:0{bmlval}b} {vals}\n")
+        return vals
+
     def _do_unknown(self):
         """
         Handle unknown message type.
         """
 
     def __str__(self) -> str:
         """
@@ -471,15 +515,15 @@
                 if isinstance(val, bytes):
                     val = escapeall(val)
                 stg += att + "=" + str(val)
                 if i < len(self.__dict__) - 1:
                     stg += ", "
         if self.identity == "UNKNOWN":
             stg += ", Not_Yet_Implemented"
-        stg += ")>"
+        stg = stg.strip(" ,") + ")>"
 
         return stg
 
     def __repr__(self) -> str:
         """
         Machine readable representation.
         eval(repr(obj)) = obj
```

### Comparing `pyspartn-0.4.0/src/pyspartn/spartnreader.py` & `pyspartn-1.0.0/src/pyspartn/spartnreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,34 +38,28 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 
 # pylint: disable=invalid-name too-many-instance-attributes
 
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timezone
 from os import getenv
 from socket import socket
 
 from pyspartn.exceptions import (
     ParameterError,
     SPARTNMessageError,
     SPARTNParseError,
     SPARTNTypeError,
 )
 from pyspartn.socket_stream import SocketStream
-from pyspartn.spartnhelpers import bitsval, timetag2date, valid_crc
+from pyspartn.spartnhelpers import bitsval, naive2aware, timetag2date, valid_crc
 from pyspartn.spartnmessage import SPARTNMessage
-from pyspartn.spartntypes_core import (
-    ERRLOG,
-    ERRRAISE,
-    SPARTN_PREB,
-    TIMETAGSHIFT,
-    VALCRC,
-)
+from pyspartn.spartntypes_core import ERRLOG, ERRRAISE, SPARTN_PREB, VALCRC
 
 
 class SPARTNReader:
     """
     SPARTNReader class.
     """
 
@@ -106,15 +100,15 @@
         self._key = key
         # accumlated array of 32-bit gnssTimeTag from datastream
         self._timetags = {}
         basedate = datetime.now(timezone.utc) if basedate is None else basedate
         if isinstance(basedate, int):  # 32-bit gnssTimeTag
             self._basedate = timetag2date(basedate)
         else:  # datetime
-            self._basedate = basedate
+            self._basedate = naive2aware(basedate)
 
         if self._decode and self._key is None:
             raise ParameterError("Key must be provided if decoding is enabled")
 
     def __iter__(self):
         """Iterator."""
 
@@ -200,14 +194,15 @@
         gnssTimeTag = bitsval(payDesc, 5, gtlen)
         # store 32-bit timetag for this subtype for later use in decryption
         if timeTagtype == 1:
             self._timetags[msgSubtype] = gnssTimeTag
         # solutionId = bitsval(payDesc, gtlen + 5, 7)
         # solutionProcId = bitsval(payDesc, gtlen + 12, 4)
         authInd = 0
+        embAuthLen = 0
         if eaf:
             payDesc += self._read_bytes(2)
             # encryptionId = bitsval(payDesc, gtlen + 16, 4)
             # encryptionSeq = bitsval(payDesc, gtlen + 20, 6)
             authInd = bitsval(payDesc, gtlen + 26, 3)
             embAuthLen = bitsval(payDesc, gtlen + 29, 3)
         payload = self._read_bytes(nData)
@@ -232,29 +227,20 @@
         # validate CRC
         core = framestart + payDesc + payload + embAuth
         raw_data = preamble + core + crcb
         if self._validate & VALCRC:
             if not valid_crc(core, crc, crcType):
                 raise SPARTNParseError(f"Invalid CRC {crc}")
 
-        # use 32-bit timetag for this subtype from datastream if available,
-        # otherwise use value provided in arguments adjusted for UTC and leap second shift
-        shift = TIMETAGSHIFT.get(msgSubtype, 0)
-        if isinstance(self._basedate, datetime):
-            shift = timedelta(seconds=shift)
-        basedate = self._timetags.get(
-            msgSubtype,
-            self._basedate + shift,
-        )
         parsed_data = self.parse(
             raw_data,
             validate=self._validate,
             decode=self._decode,
             key=self._key,
-            basedate=basedate,
+            basedate=self._basedate,
         )
         return (raw_data, parsed_data)
 
     def _read_bytes(self, size: int) -> bytes:
         """
         Read a specified number of bytes from stream.
 
@@ -299,15 +285,15 @@
 
     @staticmethod
     def parse(
         message: bytes,
         validate: int = VALCRC,
         decode: bool = False,
         key: str = None,
-        basedate: object = datetime.now(),
+        basedate: object = datetime.now(timezone.utc),
     ) -> SPARTNMessage:
         """
         Parse SPARTN message to SPARTNMessage object.
 
         :param bytes message: SPARTN raw message bytes
         :param int validate: 0 = ignore invalid CRC, 1 = validate CRC (1)
         :param int decode: decode payload True/False
@@ -322,10 +308,10 @@
         if decode and key is None:
             raise ParameterError("Key must be provided if decoding is enabled")
 
         return SPARTNMessage(
             transport=message,
             decode=decode,
             key=key,
-            basedate=basedate,
+            basedate=naive2aware(basedate),
             validate=validate,
         )
```

### Comparing `pyspartn-0.4.0/src/pyspartn/spartntypes_core.py` & `pyspartn-1.0.0/src/pyspartn/spartntypes_core.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 Created on 10 Feb 2023
 
 Information Sourced from https://www.spartnformat.org/download/
 (available in the public domain) © 2021 u-blox AG. All rights reserved.
 
 :author: semuadmin
+:copyright: SEMU Consulting © 2023
+:license: BSD 3-Clause
 """
 
 # pylint: disable=line-too-long
 
 from datetime import datetime, timezone
 
 TIMEBASE = datetime(2010, 1, 1, 0, 0, tzinfo=timezone.utc)
@@ -18,36 +20,31 @@
 ERRLOG = 1
 ERRIGNORE = 0
 VALNONE = 0
 VALCRC = 1
 VALMSGID = 2
 SPARTN_PRE = 0x73
 SPARTN_PREB = b"s"
+NA = "N/A"
 
 # Attribute types
 IN = "IN"  # integer
 EN = "EN"  # enumeration
 BM = "BM"  # bitmask
 FL = "FL"  # float
+PRN = "PRN"  # PRN lookup value
+PBS = "PBS"  # phase bias value
+CBS = "CBS"  # code bias value
 
 # Transient attribute names used to store variable bitmask length flags
 NB = "NB_"
 STBMLEN = "SatBitmaskLen"
 PBBMLEN = "PhaseBiasBitmaskLen"
 CBBMLEN = "CodeBiasBitmaskLen"
 
-# UTC + leap second basedate shift for different constellations
-# relative to GPS (UTC + 18 leap seconds); valid as from 2017/1/1
-TIMETAGSHIFT = {
-    0: 0,  # GPS
-    1: 10782,  # GLO = GPS + 3600 * 3 - 18
-    2: 0,  # GAL = GPS
-    3: -14,  # BEI = GPS - 14
-    4: 0,  # QZS = GPS
-}
 
 # SPARTN message types
 SPARTN_MSGIDS = {
     0: "SPARTN-1X-OCB",  # Orbit, Clock, Bias
     (0, 0): "SPARTN-1X-OCB-GPS",
     (0, 1): "SPARTN-1X-OCB-GLO",
     (0, 2): "SPARTN-1X-OCB-GAL",
@@ -72,14 +69,17 @@
     (120, 2): "SPARTN-1X-PROP-SWIFT",
 }
 
 # Datafields used in message definitions
 # key (IN, BM, EN): (length in bits, type, resolution or n/a, description)
 # key (FL): (length in bits, type, resolution, range minimum, description)
 SPARTN_DATA_FIELDS = {
+    "PRN": (0, PRN, "n/a", "Satellite PRN"),  # attribute derived by pyspartn
+    "PhaseBias": (0, PBS, "n/a", "Phase Bias"),  # attribute derived by pyspartn
+    "CodeBias": (0, CBS, "n/a", "Code Bias"),  # attribute derived by pyspartn
     "SF005": (9, IN, 1, "Solution issue of update (SIOU)"),
     "SF008": (1, EN, "n/a", "Yaw present flag"),
     "SF009": (1, IN, 1, "Satellite reference datum"),
     "SF010": (1, IN, "n/a", "End of OCB set (EOS)"),
     STBMLEN: (2, IN, "n/a", "Length of satellite bitmask"),
     "SF011": ("34 to 66", BM, "Bitmask", "GPS Satellite mask"),
     "SF012": ("26 to 65", BM, "Bitmask", "GLONASS Satellite mask"),
@@ -165,14 +165,15 @@
     "SF079": ("N", BM, "Bitmask", "Grid node present mask"),
     "SF080": (12, FL, 0.25, -511.75, "Area average VTEC"),
     "SF081": (1, IN, 1, "VTEC size indicator"),
     "SF082": (7, FL, 0.25, -15.75, "Small VTEC residual "),
     "SF083": (11, FL, 0.25, -255.75, "Large VTEC residual "),
     "SF084": (20, IN, 1, "Customer Key ID"),
     "SF085": (4, EN, 1, "Encryption Type"),
+    "SF085a": (4, EN, 1, "Encryption Type"),
     "SF086": (6, IN, 1, "Week of Applicability"),
     "SF087": (4, IN, 1, "Key length"),
     "SF088": ("Key length (SF087)", IN, "1", "Cryptographic Key"),
     "SF089": (5, IN, 1, "Count of Message IDs"),
     "SF090": (4, EN, 1, "Group Authentication Type"),
     "SF091": (4, IN, 1, "Computed Authentication Data (CAD) Length"),
     "SF092": ("CAD length (SF091)", IN, 1, "Computed Authentication Data (CAD)"),
```

### Comparing `pyspartn-0.4.0/src/pyspartn/spartntypes_get.py` & `pyspartn-1.0.0/src/pyspartn/spartntypes_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,69 @@
 SPARTN Protocol core globals and constants
 
 Created on 10 Feb 2023
 
 Information Sourced from https://www.spartnformat.org/download/
 (available in the public domain) © 2021 u-blox AG. All rights reserved.
 
+Payload definitions are contained in a series of dictionaries.
+Repeating and conditional elements are defined as a tuple of
+(element size/presence designator, element dictionary). The element
+size/presence designator can take one of the following forms:
+
+*Repeating elements:*
+ - an integer representing the fixed size of the repeating element N.
+ - a string representing the name of a preceding attribute containing
+   the size of the repeating element N (note that in some cases the
+   attribute represents N - 1) e.g.
+
+.. code-block:: python
+
+  "group": (  # repeating group * (SF030 + 1)
+      "SF030",
+      {
+          "SF031": "Area ID",
+          etc ...
+      },
+  )
+
+*Conditional elements:*
+ - a tuple containing a string and either a single value or a list of values,
+   representing the name of a preceding attribute and the value(s) it must take
+   in order for the optional element to be present e.g.
+
+.. code-block:: python
+
+  "optSF041-12": (
+      ("SF041+1", [1, 2]),  # if SF041I in 1,2
+      {
+          "SF055": "Ionosphere quality",
+          etc ...
+      }
+  )
+
+An 'NB' prefix indicates that the element size is given by the number of set bits
+in the attribute, rather than its integer value e.g. 
+'NB + "SF011"' -> if SF011 = 0b0101101, the size of the repeating element is 4.
+
+A '+1' or '+2' suffix indicates that the attribute name must be suffixed
+with the specified number of nested element indices e.g. 'SF041+1' -> 'SF041_01'
+
+In some instances, the size of the repeating element must be derived from 
+multiple attributes. In these cases the element size is denoted by a composite
+attribute name which is calculated within `spartnmessage.py` e.g. 'PBBMLEN'
+
 :author: semuadmin
+:copyright: SEMU Consulting © 2023
+:license: BSD 3-Clause
 """
 
 # pylint: disable=too-many-lines, line-too-long
 
-from pyspartn.spartntypes_core import CBBMLEN, NB, PBBMLEN, STBMLEN
+from pyspartn.spartntypes_core import CBBMLEN, NB, PBBMLEN, PRN, STBMLEN
 
 OCB_HDR = {  # OCB Header
     "SF005": "Solution issue of update (SIOU)",
     "SF010": "End of set",
     "SF069": "Reserved",
     "SF008": "Yaw present flag",
     "SF009": "Satellite reference datum",
@@ -25,14 +74,15 @@
     "SF005": "Solution issue of update (SIOU)",
     "SF068": "Area issue of update (AIOU)",
     "SF069": "Reserved",
     "SF030": "Area count",  # NB: N - 1
 }
 
 OCB_SAT_FLAGS = {  # table 6.4
+    PRN: "Satellite PRN",
     "SF014O": "Orbit data present flag",
     "SF014C": "Clock data present flag",
     "SF014B": "Bias data present flag",
     "SF015": "Continuity indicator",
 }
 
 OCB_ORBIT_BLOCK = {  # part of table 6.5 Orbit Block
@@ -55,19 +105,25 @@
             "SF020CK": "Clock correction",
             "SF024": "User range error",
         },
     ),
 }
 
 PHAS_BIAS_BLOCK = {  # table 6.12 Phase Bias Block
+    "PhaseBias": "Phase Bias type",
     "SF023": "Fix flag",
     "SF015": "Continuity indicator",
     "SF020PB": "Phase bias correction",
 }
 
+CODE_BIAS_BLOCK = {  # tables 6.7 - 6.12
+    "CodeBias": "Code Bias type",
+    "SF029": "Code bias correction",
+}
+
 AREA_DATA_BLOCK = {  # table 6.15 Area Data Block
     "SF031": "Area ID",
     "SF039": "Number of grid points present",
     "SF040T": "Tropo blocks indicator",
     "SF040I": "Iono blocks indicator",
 }
 
@@ -135,17 +191,18 @@
     ),
 }
 
 ION_SAT_BLOCK = {  # table 6.20 Ionosphere Satellite Block
     "optSF041-12": (
         ("SF041+1", [1, 2]),  # if SF041I in 1,2
         {
+            PRN: "Satellite PRN",
             "SF055": "Ionosphere quality",
             "SF056": "Ionosphere polynomial coefficient size indicator",
-            "optSF064-0": (
+            "optSF056-0": (
                 ("SF056+2", 0),  # if SF056 = 0 table 6.21
                 {
                     "SF057": "Ionosphere coefficient C00",
                     "optSF054-12": (
                         ("SF054+1", [1, 2]),  # if SF054 in 1,2
                         {
                             "SF058a": "Ionosphere coefficient C01",
@@ -248,15 +305,15 @@
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF027": "GPS code bias mask",
                                 "groupSF027-BITS": (
                                     NB
                                     + "SF027+1",  # repeating group * num bits set in SF027
                                     {
-                                        "SF029": "Code bias correction",
+                                        **CODE_BIAS_BLOCK,
                                     },
                                 ),
                             },
                         ),
                     },
                 ),
             },
@@ -297,15 +354,15 @@
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF028": "GLONASScode bias mask",
                                 "groupSF028-BITS": (
                                     NB
                                     + "SF028+1",  # repeating group * num bits set in SF028
                                     {
-                                        "SF029": "Code bias correction",
+                                        **CODE_BIAS_BLOCK,
                                     },
                                 ),
                             },
                         ),
                     },
                 ),
             },
@@ -346,15 +403,15 @@
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF105": "GALILEO code bias mask",
                                 "groupSF105-BITS": (
                                     NB
                                     + "SF105+1",  # repeating group * num bits set in SF0105
                                     {
-                                        "SF029": "Code bias correction",
+                                        **CODE_BIAS_BLOCK,
                                     },
                                 ),
                             },
                         ),
                     },
                 ),
             },
@@ -395,15 +452,15 @@
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF106": "BEIDOU code bias mask",
                                 "groupSF106-BITS": (
                                     NB
                                     + "SF106+1",  # repeating group * num bits set in SF0106
                                     {
-                                        "SF029": "Code bias correction",
+                                        **CODE_BIAS_BLOCK,
                                     },
                                 ),
                             },
                         ),
                     },
                 ),
             },
@@ -444,15 +501,15 @@
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF107": "QZSS code bias mask",
                                 "groupSF107-BITS": (
                                     NB
                                     + "SF107+1",  # repeating group * num bits set in SF0107
                                     {
-                                        "SF029": "Code bias correction",
+                                        **CODE_BIAS_BLOCK,
                                     },
                                 ),
                             },
                         ),
                     },
                 ),
             },
@@ -647,15 +704,15 @@
     # ********************************************************************
     # EAS-DYN TODO not yet tested - no available test data source
     # ********************************************************************
     "SPARTN-1X-EAS-DYN": {
         "SF084": "Customer key ID",  # plain text
         "SF085": "Dynamic key encryption type",  # plain text
         "SF086": "Week of applicability",
-        "SF085": "Payload encryption type",
+        "SF085a": "Payload encryption type",
         "SF087": "Dynamic key length",
         "SF088": "Dynamic key",  # variable length
     },
     # ********************************************************************
     # EAS-GRP deprecated
     # ********************************************************************
     "SPARTN-1X-EAS-GRP": {},  # no current plans to implement
```

### Comparing `pyspartn-0.4.0/src/pyspartn.egg-info/PKG-INFO` & `pyspartn-1.0.0/src/pyspartn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.4.0
+Version: 1.0.0
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -32,15 +32,15 @@
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/semuconsulting/pyspartn
 Project-URL: documentation, https://www.semuconsulting.com/pyspartn/
 Project-URL: repository, https://github.com/semuconsulting/pyspartn
 Project-URL: changelog, https://github.com/semuconsulting/pyspartn/blob/master/RELEASE_NOTES.md
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
@@ -53,15 +53,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cryptography>=39.0.2
+Requires-Dist: cryptography>=42.0.0
 Provides-Extra: deploy
 Requires-Dist: build; extra == "deploy"
 Requires-Dist: pip; extra == "deploy"
 Requires-Dist: setuptools>=66.0; extra == "deploy"
 Requires-Dist: wheel; extra == "deploy"
 Provides-Extra: test
 Requires-Dist: bandit; extra == "test"
@@ -97,16 +97,14 @@
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy;, UBX &copy; (u-blox) and RTCM3 &copy; GNSS/GPS messages:
 - [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 - [pyrtcm](http://github.com/semuconsulting/pyrtcm)
 
 ## <a name="currentstatus">Current Status</a>
 
-**CURRENTLY IN BETA**
-
 ![Status](https://img.shields.io/pypi/status/pyspartn)
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyspartn?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
@@ -150,17 +148,15 @@
 python3 -m virtualenv env
 source env/bin/activate (or env\Scripts\activate on Windows)
 (env) python3 -m pip install --upgrade pyspartn
 ...
 deactivate
 ```
 
-*¹* On some 32-bit Linux platforms (e.g. Raspberry Pi OS 32), it may be necessary to [install Rust compiler support](https://www.rust-lang.org/tools/install) in order to install the `cryptography` library which `pyspartn` depends on to decrypt SPARTN messages (see [Discussion](https://github.com/semuconsulting/PyGPSClient/discussions/83#discussioncomment-6635558)):
-
-See [cryptography install README](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
+*¹* On some 32-bit Linux platforms (e.g. Raspberry Pi OS 32), it may be necessary to [install Rust compiler support](https://www.rust-lang.org/tools/install) in order to install the `cryptography` library which `pyspartn` depends on to decrypt SPARTN messages. See [cryptography install README](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
 
 
 For [Conda](https://docs.conda.io/en/latest/) users, `pyspartn` is also available from [conda-forge](https://github.com/conda-forge/pyspartn-feedstock):
 
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyspartn/badges/version.svg)](https://anaconda.org/conda-forge/pyspartn)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyspartn/badges/downloads.svg)](https://anaconda.org/conda-forge/pyspartn)
 
@@ -173,78 +169,80 @@
 
 ```
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
-or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
+or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams.
 
 Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
-stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
-spr = SPARTNReader(stream)
-(raw_data, parsed_data) = spr.read()
-print(parsed_data)
+with Serial('/dev/tty.usbmodem14101', 38400, timeout=3) as stream:
+   spr = SPARTNReader(stream)
+   raw_data, parsed_data = spr.read()
+   print(parsed_data)
 ```
 
 Example - File input (using iterator).
 ```python
 from pyspartn import SPARTNReader
-stream = open('spartndata.log', 'rb')
-spr = SPARTNReader(stream)
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with open('spartndata.log', 'rb') as stream:
+   spr = SPARTNReader(stream)
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
 import socket
 from pyspartn import SPARTNReader
-stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
-stream.connect(("localhost", 50007))
-spr = SPARTNReader(stream)
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as stream:
+   stream.connect(("localhost", 50007))
+   spr = SPARTNReader(stream)
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
-Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit `gnssTimetag` (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the UTC datetime on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the UTC datetime on which the datastream was originally created to the nearest half day. `pyspartn` can derive the requisite `basedate` from any 32-bit `gnssTimetag` for the same message subtype, but this is dependent on the datastream containing such 32-bit timetags. See examples below.
 
-The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
+The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need updating every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
-stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
-spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
+   spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
 ```
 
 Example - Historical file input with decryption.
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader
-stream = open('spartndata.log', 'rb')
-spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
-for (raw_data, parsed_data) in spr:
-   print(parsed_data)
+
+with open('spartndata.log', 'rb') as stream:
+   spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255, tzinfo=timezone.utc))
+   for raw_data, parsed_data in spr:
+      print(parsed_data)
+
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and UTC `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
 Example - without payload decryption or decoding:
 
 ```python
 from pyspartn import SPARTNReader
@@ -256,62 +254,68 @@
 ```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader
 
 transport = b"\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80"
 msg = SPARTNReader.parse(
     transport,
     decode=1,
     key="6b30302427df05b4d98911ebff3a4d95",
-    basedate=datetime(2023, 6, 27, 22, 3, 0),
+    basedate=datetime(2023, 6, 27, 22, 3, 0, tzinfo=timezone.utc),
 )
 print(msg)
 ```
 ```
 <SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspartn import SPARTNReader, datadesc
-msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
+msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255, tzinfo=timezone.utc))
 print(msg)
 print(msg.identity)
 print(msg.gnssTimeTag)
 print(datadesc("SF005"), msg.SF005)
 print(datadesc("SF061a"), msg.SF061a_10_05)
 ```
 ```
 <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 'SPARTN-1X-HPAC-GPS'
 451165680
 ('Solution issue of update (SIOU)', 152)
 ('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
-Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
+Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. See [examples below](#iterating) for illustrations of how to iterate through grouped attributes.
+
+Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
+
+The `payload` attribute always contains the raw payload as bytes.
+
+#### <a name="iterating">Iterating Through Group Attributes</a>
+
+To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
 
 ```python
 vals = []
 for i in range(parsed_data.SF030 + 1):  # attribute or formula representing group size
     vals.append(getattr(parsed_data, f"SF032_{i+1:02d}"))
 print(vals)
 ```
 
-Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
-
-The `payload` attribute always contains the raw payload as bytes.
+See examples `parse_ocb.py`, `parse_hpac.py` and `parse_gad.py` for illustrations of how to convert parsed and decoded OCB, HPAC and GAD payloads into iterable data structures.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyspartn.spartnmessage.SPARTNMessage(**kwargs)
 ```
@@ -353,22 +357,23 @@
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
-1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the pygnssutils.GNSSMQTTClient class. **NB**: requires a valid ClientID for a
+1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from a binary SPARTN datastream.
+1. `spartn_decrypt.py` - illustrates how to decrypt and parse a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples below).
+1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the [`pygnssutils.GNSSMQTTClient`](https://github.com/semuconsulting/pygnssutils?tab=readme-ov-file#gnssmqttclient) class. **NB**: requires a valid ClientID for a
 SPARTN MQTT service e.g. u-blox Thingstream PointPerfect MQTT.
-1. `spartn_ntrip_client.py` - implements a simple SPARTN NTRIP client using the pygnssutils.GNSSNTRIPClient class. **NB**: requires a valid user and password for a
+1. `spartn_ntrip_client.py` - implements a simple SPARTN NTRIP client using the [`pygnssutils.GNSSNTRIPClient`](https://github.com/semuconsulting/pygnssutils?tab=readme-ov-file#gnssntripclient) class. **NB**: requires a valid user and password for a
 SPARTN NTRIP service e.g. u-blox Thingstream PointPerfect NTRIP.
-1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
-1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
-1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
+1. `parse_gad.py` - illustrates how to convert parsed GAD message types into WKT area polygon format for display on a map (see, for example, `gad_plot_map.png`).
+1. `parse_hpac.py` and `parse_ocb.py` - illustrate how to convert parsed HPAC and OCB message types into iterable data structures.
 
 ---
 ## <a name="troubleshooting">Troubleshooting</a>
 
 1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
 
    ```
```

### Comparing `pyspartn-0.4.0/src/pyspartn.egg-info/SOURCES.txt` & `pyspartn-1.0.0/src/pyspartn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspartn-0.4.0/tests/test_socket.py` & `pyspartn-1.0.0/tests/test_socket.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,14 +34,28 @@
             + b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
             + b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
             + b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
         )
         self._stream = pool * round(4096 / len(pool))
         self._buffer = self._stream
 
+    def __enter__(self):
+        """
+        Context manager enter routine.
+        """
+
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        """
+        Context manager exit routine.
+        """
+
+        self.close()
+
     def recv(self, num: int) -> bytes:
         if self._timeout:
             raise TimeoutError
         if len(self._buffer) < num:
             self._buffer = self._buffer + self._stream
         buff = self._buffer[:num]
         self._buffer = self._buffer[num:]
@@ -55,56 +69,56 @@
     def tearDown(self):
         pass
 
     # *******************************************
     # Helper methods
     # *******************************************
 
-    # def testSocketStub(self):
-    #     EXPECTED_RESULTS = (
-    #         "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>",
-    #         "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>",
-    #         "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>",
-    #         "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>",
-    #     )
-    #     raw = None
-    #     stream = DummySocket()
-    #     spr = SPARTNReader(stream, bufsize=512)
-    #     buff = spr._stream.buffer  # test buffer getter method
-    #     i = 0
-    #     for raw, parsed in spr.iterate():
-    #         if raw is not None:
-    #             print(parsed)
-    #             self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
-    #             i += 1
-    #             if i >= 4:
-    #                 break
-    #     self.assertEqual(i, 4)
+    def testSocketStub(self):
+        EXPECTED_RESULTS = (
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181)>",
+        )
+        raw = None
+        with DummySocket() as stream:
+            spr = SPARTNReader(stream, bufsize=512)
+            buff = spr._stream.buffer  # test buffer getter method
+            i = 0
+            for raw, parsed in spr:
+                if raw is not None:
+                    # print(f'"{parsed}",')
+                    self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
+                    i += 1
+                    if i >= 4:
+                        break
+        self.assertEqual(i, 4)
 
     def testSocketIter(self):  # test for extended stream
         raw = None
-        stream = DummySocket()
-        spr = SPARTNReader(stream)
-        i = 0
-        for raw, parsed in spr:
-            if raw is None:
-                raise EOFError
-            i += 1
-            if i >= 123:
-                break
+        with DummySocket() as stream:
+            spr = SPARTNReader(stream)
+            i = 0
+            for raw, parsed in spr:
+                if raw is None:
+                    raise EOFError
+                i += 1
+                if i >= 123:
+                    break
         self.assertEqual(i, 123)
 
     def testSocketError(self):  # test for simulated socket timeout
         raw = None
-        stream = DummySocket(timeout=True)
-        spr = SPARTNReader(stream)
-        i = 0
-        for raw, parsed in spr:
-            i += 1
-            if i >= 4:
-                break
+        with DummySocket(timeout=True) as stream:
+            spr = SPARTNReader(stream)
+            i = 0
+            for raw, parsed in spr:
+                i += 1
+                if i >= 4:
+                    break
         self.assertEqual(i, 0)
 
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

### Comparing `pyspartn-0.4.0/tests/test_static.py` & `pyspartn-1.0.0/tests/test_static.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     convert_timetag,
     datadesc,
     date2timetag,
     decrypt,
     enc2float,
     encrypt,
     escapeall,
+    naive2aware,
     timetag2date,
     valid_crc,
 )
 from pyspartn.spartntypes_core import SPARTN_DATA_FIELDS, FL
 from pyspartn.spartntables import (
     SF015_ENUM,
     SF022_ENUM,
@@ -48,20 +49,14 @@
     SF091_ENUM,
     SF093_ENUM,
     SF094_ENUM,
     SF095_ENUM,
     SF096_ENUM,
     SF097_ENUM,
     SF098_ENUM,
-    SF102_ENUM,
-    SF103_ENUM,
-    SF104_ENUM,
-    SF105_ENUM,
-    SF106_ENUM,
-    SF107_ENUM,
 )
 
 
 class StaticTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         dirname = os.path.dirname(__file__)
@@ -258,21 +253,27 @@
             SF091_ENUM,
             SF093_ENUM,
             SF094_ENUM,
             SF095_ENUM,
             SF096_ENUM,
             SF097_ENUM,
             SF098_ENUM,
-            SF102_ENUM,
-            SF103_ENUM,
-            SF104_ENUM,
-            SF105_ENUM,
-            SF106_ENUM,
-            SF107_ENUM,
         ):
             i += len(tbl)
-        self.assertEqual(i, 141)
+        self.assertEqual(i, 115)
+
+    def testnaive2aware(self):
+        dt1 = datetime(2022, 3, 4, 12, 34, 54)
+        dt2 = datetime(2020, 3, 4, 10, 34, 54, tzinfo=timezone.utc)
+        dt3 = 452383965
+        self.assertEqual(
+            naive2aware(dt1), datetime(2022, 3, 4, 12, 34, 54, tzinfo=timezone.utc)
+        )
+        self.assertEqual(
+            naive2aware(dt2), datetime(2020, 3, 4, 10, 34, 54, tzinfo=timezone.utc)
+        )
+        self.assertEqual(naive2aware(dt3), 452383965)
 
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

### Comparing `pyspartn-0.4.0/tests/test_stream.py` & `pyspartn-1.0.0/tests/test_stream.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 import sys
 import unittest
 from io import StringIO
 from datetime import datetime, timezone
 
 from pyspartn.exceptions import SPARTNMessageError, SPARTNParseError, ParameterError
 from pyspartn.spartnreader import SPARTNReader, SPARTNMessage
+from pyspartn.spartnhelpers import date2timetag
 from pyspartn.spartntypes_core import ERRRAISE, ERRIGNORE, ERRLOG
 
 SPARTN_KEY = "930d847b779b126863c8b3b2766ae7cc"
 SPARTN_BASEDATE = datetime(2024, 4, 18, 20, 48, 29, 977255, tzinfo=timezone.utc)
+SPARTN_BASEDATE_INT = date2timetag(SPARTN_BASEDATE)
 
 
 class StreamTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         self.dirname = os.path.dirname(__file__)
         self.streamSPARTN = open(os.path.join(self.dirname, "spartn_mqtt.log"), "rb")
@@ -144,28 +146,59 @@
         self.catchio()
         spr = SPARTNReader(self.streamBADCRC, quitonerror=ERRLOG, errorhandler=igor)
         for raw, parsed in spr:
             pass
         output = self.restoreio()
         self.assertEqual(output, EXPECTED_OUTPUT)
 
+    def testHPACLOGnodecode(
+        self,
+    ):  # test SPARTN HPAC message no decode
+        EXPECTED_RESULT = [
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=478, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=31, authInd=1, embAuthLen=0, crc=8969842)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=478, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=32, authInd=1, embAuthLen=0, crc=114625)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=472, eaf=1, crcType=2, frameCrc=6, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=33, authInd=1, embAuthLen=0, crc=8980777)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=98, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=34, authInd=1, embAuthLen=0, crc=7396141)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=421, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=57, authInd=1, embAuthLen=0, crc=15138586)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=456, eaf=1, crcType=2, frameCrc=2, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=58, authInd=1, embAuthLen=0, crc=14979022)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=468, eaf=1, crcType=2, frameCrc=5, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=59, authInd=1, embAuthLen=0, crc=11322474)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=468, eaf=1, crcType=2, frameCrc=5, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=60, authInd=1, embAuthLen=0, crc=13756719)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=61, eaf=1, crcType=2, frameCrc=15, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=61, authInd=1, embAuthLen=0, crc=13417473)>",
+        ]
+        i = 0
+        with open(os.path.join(self.dirname, "spartnHPAC.log"), "rb") as stream:
+            spr = SPARTNReader(
+                stream,
+                quitonerror=ERRRAISE,
+                decode=False,
+            )
+
+            for raw, parsed in spr:
+                if raw is not None:
+                    # print(f'"{parsed}",')
+                    self.assertEqual(str(parsed), EXPECTED_RESULT[i])
+                    self.assertTrue(0 <= parsed._padding <= 8)
+                    i += 1
+        self.assertEqual(i, 10)
+
     def testHPACLOG(
         self,
     ):  # test decoding of SPARTN HPAC message
         EXPECTED_RESULT = [
-            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, SF061a_01_01=-0.8960000000000008, SF061b_01_01=-0.15200000000000102, SF055_01_02=1, SF056_01_02=1, SF060_01_02=-2.0, SF061a_01_02=0.6319999999999908, SF061b_01_02=-0.04000000000000625, SF055_01_03=3, SF056_01_03=1, SF060_01_03=-1.6800000000000068, SF061a_01_03=0.35999999999999943, SF061b_01_03=0.1280000000000001, SF055_01_04=3, SF056_01_04=1, SF060_01_04=27.439999999999998, SF061a_01_04=0.4719999999999942, SF061b_01_04=0.23999999999999488, SF055_01_05=5, SF056_01_05=1, SF060_01_05=24.560000000000002, SF061a_01_05=0.6640000000000015, SF061b_01_05=0.2079999999999984, SF055_01_06=5, SF056_01_06=1, SF060_01_06=16.480000000000018, SF061a_01_06=-0.936000000000007, SF061b_01_06=-0.23199999999999932, SF055_01_07=4, SF056_01_07=1, SF060_01_07=-8.639999999999986, SF061a_01_07=-1.872000000000007, SF061b_01_07=-0.24800000000000466, SF031_02=1, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.0, SF044_02=1, SF048_02=-0.21199999999999997, SF049a_02=-0.0020000000000000018, SF049b_02=0.0, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836738, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-9.120000000000005, SF061a_02_01=0.11199999999999477, SF061b_02_01=-0.14400000000000546, SF055_02_02=1, SF056_02_02=1, SF060_02_02=-3.319999999999993, SF061a_02_02=0.35199999999998965, SF061b_02_02=-0.06400000000000716, SF055_02_03=3, SF056_02_03=1, SF060_02_03=-1.1999999999999886, SF061a_02_03=-0.8320000000000078, SF061b_02_03=0.055999999999997385, SF055_02_04=4, SF056_02_04=1, SF060_02_04=23.920000000000016, SF061a_02_04=0.6479999999999961, SF061b_02_04=0.5039999999999907, SF055_02_05=5, SF056_02_05=1, SF060_02_05=20.680000000000007, SF061a_02_05=-0.17600000000000193, SF061b_02_05=0.47999999999998977, SF055_02_06=6, SF056_02_06=1, SF060_02_06=14.920000000000016, SF061a_02_06=0.8160000000000025, SF061b_02_06=1.0319999999999965, SF055_02_07=4, SF056_02_07=1, SF060_02_07=-1.8799999999999955, SF061a_02_07=-1.1440000000000055, SF061b_02_07=-0.2880000000000109, SF031_03=2, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=1, SF043_03=0.0, SF044_03=1, SF048_03=-0.21599999999999997, SF049a_03=0.0030000000000000027, SF049b_03=-0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF011_03=880836738, SF055_03_01=2, SF056_03_01=1, SF060_03_01=-10.359999999999957, SF061a_03_01=0.11999999999999034, SF061b_03_01=-0.09600000000000364, SF055_03_02=2, SF056_03_02=1, SF060_03_02=-3.5600000000000023, SF061a_03_02=0.23999999999999488, SF061b_03_02=0.007999999999995566, SF055_03_03=2, SF056_03_03=1, SF060_03_03=-0.8799999999999955, SF061a_03_03=-0.8160000000000025, SF061b_03_03=0.0799999999999983, SF055_03_04=2, SF056_03_04=1, SF060_03_04=26.400000000000034, SF061a_03_04=0.5759999999999934, SF061b_03_04=0.2560000000000002, SF055_03_05=4, SF056_03_05=1, SF060_03_05=25.04000000000002, SF061a_03_05=-0.22400000000000375, SF061b_03_05=0.38400000000000034, SF055_03_06=6, SF056_03_06=1, SF060_03_06=15.600000000000023, SF061a_03_06=-0.04800000000000182, SF061b_03_06=-0.3200000000000074, SF055_03_07=4, SF056_03_07=1, SF060_03_07=-4.519999999999982, SF061a_03_07=-0.960000000000008, SF061b_03_07=-0.27200000000000557, SF031_04=3, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.0, SF044_04=1, SF048_04=-0.20799999999999996, SF049a_04=-0.0020000000000000018, SF049b_04=0.0, SF054_04=1, SatBitmaskLen_04=0, SF011_04=880836610, SF055_04_01=1, SF056_04_01=1, SF060_04_01=-8.71999999999997, SF061a_04_01=0.11999999999999034, SF061b_04_01=-0.11200000000000898, SF055_04_02=1, SF056_04_02=1, SF060_04_02=-3.759999999999991, SF061a_04_02=0.28000000000000114, SF061b_04_02=-0.04000000000000625, SF055_04_03=4, SF056_04_03=1, SF060_04_03=0.4000000000000341, SF061a_04_03=-0.27200000000000557, SF061b_04_03=0.03999999999999204, SF055_04_04=4, SF056_04_04=1, SF060_04_04=20.840000000000032, SF061a_04_04=0.3439999999999941, SF061b_04_04=0.4959999999999951, SF055_04_05=4, SF056_04_05=1, SF060_04_05=17.680000000000007, SF061a_04_05=-0.32800000000000296, SF061b_04_05=0.5039999999999907, SF055_04_06=1, SF056_04_06=1, SF060_04_06=1.1200000000000045, SF061a_04_06=-0.4000000000000057, SF061b_04_06=-0.32800000000000296, SF031_05=4, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.0, SF044_05=1, SF048_05=-0.20799999999999996, SF049a_05=-0.0030000000000000027, SF049b_05=0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF011_05=880836610, SF055_05_01=2, SF056_05_01=1, SF060_05_01=-10.359999999999957, SF061a_05_01=0.43200000000000216, SF061b_05_01=-0.0799999999999983, SF055_05_02=3, SF056_05_02=1, SF060_05_02=-4.479999999999961, SF061a_05_02=0.1599999999999966, SF061b_05_02=-0.03200000000001069, SF055_05_03=2, SF056_05_03=1, SF060_05_03=2.640000000000043, SF061a_05_03=-0.7360000000000042, SF061b_05_03=0.14399999999999125, SF055_05_04=3, SF056_05_04=1, SF060_05_04=25.439999999999998, SF061a_05_04=0.6319999999999908, SF061b_05_04=0.2079999999999984, SF055_05_05=3, SF056_05_05=1, SF060_05_05=25.920000000000016, SF061a_05_05=-0.3760000000000048, SF061b_05_05=0.37599999999999056, SF055_05_06=3, SF056_05_06=1, SF060_05_06=-3.6399999999999864, SF061a_05_06=0.23999999999999488, SF061b_05_06=-0.35999999999999943, SF031_06=5, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.0, SF044_06=1, SF048_06=-0.18400000000000005, SF049a_06=-0.007000000000000006, SF049b_06=-0.0040000000000000036, SF054_06=1, SatBitmaskLen_06=0, SF011_06=880836610, SF055_06_01=2, SF056_06_01=1, SF060_06_01=-3.2799999999999727, SF061a_06_01=-0.2079999999999984, SF061b_06_01=-0.23199999999999932, SF055_06_02=4, SF056_06_02=1, SF060_06_02=0.4399999999999977, SF061a_06_02=-0.06400000000000716, SF061b_06_02=-0.03200000000001069, SF055_06_03=3, SF056_06_03=1, SF060_06_03=5.0400000000000205, SF061a_06_03=-0.1839999999999975, SF061b_06_03=-0.008000000000009777, SF055_06_04=3, SF056_06_04=1, SF060_06_04=23.680000000000007, SF061a_06_04=0.04800000000000182, SF061b_06_04=-0.08800000000000807, SF055_06_05=4, SF056_06_05=1, SF060_06_05=22.560000000000002, SF061a_06_05=-0.5440000000000111, SF061b_06_05=0.13599999999999568, SF055_06_06=2, SF056_06_06=1, SF060_06_06=8.520000000000039, SF061a_06_06=-0.48799999999999955, SF061b_06_06=-0.5520000000000067, SF031_07=6, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.0040000000000000036, SF044_07=1, SF048_07=-0.19599999999999995, SF049a_07=-0.0020000000000000018, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF011_07=880836610, SF055_07_01=2, SF056_07_01=1, SF060_07_01=-5.639999999999986, SF061a_07_01=-0.055999999999997385, SF061b_07_01=-0.35200000000000387, SF055_07_02=2, SF056_07_02=1, SF060_07_02=-0.839999999999975, SF061a_07_02=-0.27200000000000557, SF061b_07_02=-0.3760000000000048, SF055_07_03=2, SF056_07_03=1, SF060_07_03=6.8799999999999955, SF061a_07_03=-0.8080000000000069, SF061b_07_03=0.13599999999999568, SF055_07_04=3, SF056_07_04=1, SF060_07_04=23.920000000000016, SF061a_07_04=0.35199999999998965, SF061b_07_04=-0.02400000000000091, SF055_07_05=2, SF056_07_05=1, SF060_07_05=24.400000000000034, SF061a_07_05=-0.43200000000000216, SF061b_07_05=0.5120000000000005, SF055_07_06=1, SF056_07_06=1, SF060_07_06=4.520000000000039, SF061a_07_06=-0.3760000000000048, SF061b_07_06=-0.632000000000005, SF031_08=7, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.0, SF044_08=1, SF048_08=-0.20399999999999996, SF049a_08=-0.0050000000000000044, SF049b_08=-0.0010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF011_08=880836610, SF055_08_01=5, SF056_08_01=1, SF060_08_01=-8.319999999999993, SF061a_08_01=-0.5440000000000111, SF061b_08_01=0.007999999999995566, SF055_08_02=3, SF056_08_02=1, SF060_08_02=-2.6399999999999864, SF061a_08_02=-0.5120000000000005, SF061b_08_02=0.17600000000000193, SF055_08_03=2, SF056_08_03=1, SF060_08_03=7.560000000000002, SF061a_08_03=-1.0799999999999983, SF061b_08_03=0.3199999999999932, SF055_08_04=3, SF056_08_04=1, SF060_08_04=25.680000000000007, SF061a_08_04=0.23199999999999932, SF061b_08_04=0.29599999999999227, SF055_08_05=4, SF056_08_05=1, SF060_08_05=28.720000000000027, SF061a_08_05=-0.3359999999999985, SF061b_08_05=0.7439999999999998, SF055_08_06=4, SF056_08_06=1, SF060_08_06=-0.9199999999999591, SF061a_08_06=-0.30400000000000205, SF061b_08_06=-0.3920000000000101, SF031_09=8, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.0040000000000000036, SF044_09=1, SF048_09=-0.14400000000000002, SF049a_09=-0.009000000000000008, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF011_09=880836610, SF055_09_01=2, SF056_09_01=1, SF060_09_01=0.6800000000000068, SF061a_09_01=-1.3359999999999985, SF061b_09_01=-0.055999999999997385, SF055_09_02=2, SF056_09_02=1, SF060_09_02=2.9600000000000364, SF061a_09_02=-0.9200000000000017, SF061b_09_02=0.21599999999999397, SF055_09_03=2, SF056_09_03=1, SF060_09_03=6.2000000000000455, SF061a_09_03=-1.240000000000009, SF061b_09_03=0.0799999999999983, SF055_09_04=1, SF056_09_04=1, SF060_09_04=20.0, SF061a_09_04=-0.784000000000006, SF061b_09_04=0.1839999999999975, SF055_09_05=3, SF056_09_05=1, SF060_09_05=17.720000000000027, SF061a_09_05=-0.9280000000000115, SF061b_09_05=0.22399999999998954, SF055_09_06=2, SF056_09_06=1, SF060_09_06=17.0, SF061a_09_06=-2.1680000000000064, SF061b_09_06=-0.3920000000000101, SF031_10=9, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.0040000000000000036, SF044_10=1, SF048_10=-0.18799999999999994, SF049a_10=-0.0020000000000000018, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF011_10=880836610, SF055_10_01=1, SF056_10_01=1, SF060_10_01=-4.399999999999977, SF061a_10_01=-0.8320000000000078, SF061b_10_01=-0.5200000000000102, SF055_10_02=2, SF056_10_02=1, SF060_10_02=-0.4399999999999977, SF061a_10_02=-0.6560000000000059, SF061b_10_02=-0.2960000000000065, SF055_10_03=3, SF056_10_03=1, SF060_10_03=8.960000000000036, SF061a_10_03=-1.4399999999999977, SF061b_10_03=0.14399999999999125, SF055_10_04=2, SF056_10_04=1, SF060_10_04=21.960000000000036, SF061a_10_04=0.16799999999999216, SF061b_10_04=-0.04000000000000625, SF055_10_05=4, SF056_10_05=1, SF060_10_05=23.760000000000048, SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>",
-            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=478, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=31, authInd=1, embAuthLen=0, crc=8969842, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=10, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0040000000000000036, SF044_01=1, SF048_01=-0.19199999999999995, SF049a_01=-0.0030000000000000027, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836610, SF055_01_01=2, SF056_01_01=1, SF060_01_01=-6.279999999999973, SF061a_01_01=-0.5440000000000111, SF061b_01_01=0.0, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-1.3599999999999568, SF061a_01_02=-0.30400000000000205, SF061b_01_02=0.21599999999999397, SF055_01_03=2, SF056_01_03=1, SF060_01_03=11.319999999999993, SF061a_01_03=-1.2240000000000038, SF061b_01_03=0.30400000000000205, SF055_01_04=2, SF056_01_04=1, SF060_01_04=24.680000000000007, SF061a_01_04=0.1599999999999966, SF061b_01_04=0.37599999999999056, SF055_01_05=3, SF056_01_05=1, SF060_01_05=28.840000000000032, SF061a_01_05=-0.3359999999999985, SF061b_01_05=0.8960000000000008, SF055_01_06=3, SF056_01_06=1, SF060_01_06=2.5200000000000387, SF061a_01_06=-1.088000000000008, SF061b_01_06=-0.17600000000000193, SF031_02=11, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.09999999999999998, SF049a_02=-0.0050000000000000044, SF049b_02=-0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836610, SF055_02_01=2, SF056_02_01=1, SF060_02_01=6.160000000000025, SF061a_02_01=-1.2319999999999993, SF061b_02_01=-0.03200000000001069, SF055_02_02=1, SF056_02_02=1, SF060_02_02=6.600000000000023, SF061a_02_02=-0.9680000000000035, SF061b_02_02=0.06399999999999295, SF055_02_03=1, SF056_02_03=1, SF060_02_03=11.360000000000014, SF061a_02_03=-1.2480000000000047, SF061b_02_03=-0.1039999999999992, SF055_02_04=3, SF056_02_04=1, SF060_02_04=22.360000000000014, SF061a_02_04=-0.4720000000000084, SF061b_02_04=0.0799999999999983, SF055_02_05=2, SF056_02_05=1, SF060_02_05=20.439999999999998, SF061a_02_05=-0.9040000000000106, SF061b_02_05=0.43200000000000216, SF055_02_06=1, SF056_02_06=1, SF060_02_06=27.319999999999993, SF061a_02_06=-2.112000000000002, SF061b_02_06=-0.3440000000000083, SF031_03=12, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.008000000000000007, SF044_03=1, SF048_03=-0.10799999999999998, SF049a_03=-0.01100000000000001, SF049b_03=-0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF011_03=880836610, SF055_03_01=1, SF056_03_01=1, SF060_03_01=5.560000000000002, SF061a_03_01=-1.2000000000000028, SF061b_03_01=-0.1360000000000099, SF055_03_02=1, SF056_03_02=1, SF060_03_02=7.1200000000000045, SF061a_03_02=-0.8560000000000088, SF061b_03_02=0.0799999999999983, SF055_03_03=2, SF056_03_03=1, SF060_03_03=12.520000000000039, SF061a_03_03=-1.4720000000000084, SF061b_03_03=0.4479999999999933, SF055_03_04=1, SF056_03_04=1, SF060_03_04=23.04000000000002, SF061a_03_04=-0.4000000000000057, SF061b_03_04=0.15200000000000102, SF055_03_05=1, SF056_03_05=1, SF060_03_05=22.80000000000001, SF061a_03_05=-0.9519999999999982, SF061b_03_05=0.29599999999999227, SF055_03_06=2, SF056_03_06=1, SF060_03_06=23.80000000000001, SF061a_03_06=-1.9280000000000044, SF061b_03_06=-0.632000000000005, SF031_04=13, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=2, SF043_04=0.008000000000000007, SF044_04=1, SF048_04=-0.18000000000000005, SF049a_04=-0.006000000000000005, SF049b_04=-0.0030000000000000027, SF054_04=1, SatBitmaskLen_04=0, SF011_04=880836610, SF055_04_01=1, SF056_04_01=1, SF060_04_01=0.8400000000000318, SF061a_04_01=-0.6720000000000113, SF061b_04_01=-0.5120000000000005, SF055_04_02=2, SF056_04_02=1, SF060_04_02=3.319999999999993, SF061a_04_02=-0.3440000000000083, SF061b_04_02=-0.4399999999999977, SF055_04_03=3, SF056_04_03=1, SF060_04_03=13.920000000000016, SF061a_04_03=-1.568000000000005, SF061b_04_03=0.007999999999995566, SF055_04_04=4, SF056_04_04=1, SF060_04_04=21.24000000000001, SF061a_04_04=0.2079999999999984, SF061b_04_04=-0.1360000000000099, SF055_04_05=1, SF056_04_05=1, SF060_04_05=23.600000000000023, SF061a_04_05=-0.21600000000000819, SF061b_04_05=0.06399999999999295, SF055_04_06=2, SF056_04_06=1, SF060_04_06=16.439999999999998, SF061a_04_06=-1.4480000000000075, SF061b_04_06=-0.7360000000000042, SF031_05=14, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.008000000000000007, SF044_05=1, SF048_05=-0.18000000000000005, SF049a_05=-0.0050000000000000044, SF049b_05=0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF011_05=880836610, SF055_05_01=1, SF056_05_01=1, SF060_05_01=-2.0399999999999636, SF061a_05_01=-0.8000000000000114, SF061b_05_01=-0.4720000000000084, SF055_05_02=1, SF056_05_02=1, SF060_05_02=1.240000000000009, SF061a_05_02=-0.5600000000000023, SF061b_05_02=-0.3359999999999985, SF055_05_03=1, SF056_05_03=1, SF060_05_03=13.920000000000016, SF061a_05_03=-1.4879999999999995, SF061b_05_03=-0.04000000000000625, SF055_05_04=2, SF056_05_04=1, SF060_05_04=21.200000000000045, SF061a_05_04=0.35199999999998965, SF061b_05_04=0.09599999999998943, SF055_05_05=1, SF056_05_05=1, SF060_05_05=24.680000000000007, SF061a_05_05=-0.22400000000000375, SF061b_05_05=0.23999999999999488, SF055_05_06=2, SF056_05_06=1, SF060_05_06=11.640000000000043, SF061a_05_06=-1.3680000000000092, SF061b_05_06=-0.847999999999999, SF031_06=15, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.008000000000000007, SF044_06=1, SF048_06=-0.19999999999999996, SF049a_06=-0.0030000000000000027, SF049b_06=-0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF011_06=880836610, SF055_06_01=1, SF056_06_01=1, SF060_06_01=-5.079999999999984, SF061a_06_01=0.2879999999999967, SF061b_06_01=-0.5200000000000102, SF055_06_02=1, SF056_06_02=1, SF060_06_02=-1.0, SF061a_06_02=0.5039999999999907, SF061b_06_02=-0.4000000000000057, SF055_06_03=4, SF056_06_03=1, SF060_06_03=14.480000000000018, SF061a_06_03=-0.5919999999999987, SF061b_06_03=-0.04800000000000182, SF055_06_04=2, SF056_06_04=1, SF060_06_04=21.80000000000001, SF061a_06_04=1.3119999999999976, SF061b_06_04=0.06399999999999295, SF055_06_05=4, SF056_06_05=1, SF060_06_05=26.920000000000016, SF061a_06_05=0.887999999999991, SF061b_06_05=0.24799999999999045, SF055_06_06=1, SF056_06_06=1, SF060_06_06=6.0, SF061a_06_06=0.06399999999999295, SF061b_06_06=-0.8560000000000088, SF031_07=16, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.008000000000000007, SF044_07=1, SF048_07=-0.136, SF049a_07=0.01200000000000001, SF049b_07=-0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF011_07=880836610, SF055_07_01=1, SF056_07_01=1, SF060_07_01=10.640000000000043, SF061a_07_01=-0.3920000000000101, SF061b_07_01=-0.3680000000000092, SF055_07_02=1, SF056_07_02=1, SF060_07_02=10.840000000000032, SF061a_07_02=-0.0799999999999983, SF061b_07_02=-0.24800000000000466, SF055_07_03=1, SF056_07_03=1, SF060_07_03=18.319999999999993, SF061a_07_03=-1.1280000000000001, SF061b_07_03=0.22399999999998954, SF055_07_04=1, SF056_07_04=1, SF060_07_04=25.400000000000034, SF061a_07_04=0.32799999999998875, SF061b_07_04=-0.15200000000000102, SF055_07_05=1, SF056_07_05=1, SF060_07_05=26.04000000000002, SF061a_07_05=-0.07200000000000273, SF061b_07_05=0.015999999999991132, SF055_07_06=2, SF056_07_06=1, SF060_07_06=31.720000000000027, SF061a_07_06=-1.3359999999999985, SF061b_07_06=-0.9120000000000061, SF031_08=17, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.008000000000000007, SF044_08=1, SF048_08=-0.16400000000000003, SF049a_08=0.009000000000000008, SF049b_08=-0.006000000000000005, SF054_08=1, SatBitmaskLen_08=0, SF011_08=880836610, SF055_08_01=1, SF056_08_01=1, SF060_08_01=7.680000000000007, SF061a_08_01=-0.3760000000000048, SF061b_08_01=-0.48799999999999955, SF055_08_02=1, SF056_08_02=1, SF060_08_02=8.920000000000016, SF061a_08_02=0.007999999999995566, SF061b_08_02=-0.3440000000000083, SF055_08_03=2, SF056_08_03=1, SF060_08_03=20.480000000000018, SF061a_08_03=-1.1920000000000073, SF061b_08_03=0.367999999999995, SF055_08_04=1, SF056_08_04=1, SF060_08_04=24.680000000000007, SF061a_08_04=0.3359999999999985, SF061b_08_04=-0.07200000000000273, SF055_08_05=2, SF056_08_05=1, SF060_08_05=26.920000000000016, SF061a_08_05=0.07199999999998852, SF061b_08_05=0.21599999999999397, SF055_08_06=1, SF056_08_06=1, SF060_08_06=26.120000000000005, SF061a_08_06=-1.1280000000000001, SF061b_08_06=-0.8000000000000114, SF031_09=18, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.008000000000000007, SF044_09=1, SF048_09=-0.18000000000000005, SF049a_09=-0.010000000000000009, SF049b_09=-0.0020000000000000018, SF054_09=1, SatBitmaskLen_09=0, SF011_09=880836610, SF055_09_01=1, SF056_09_01=1, SF060_09_01=3.0400000000000205, SF061a_09_01=-0.21600000000000819, SF061b_09_01=-0.14400000000000546, SF055_09_02=2, SF056_09_02=1, SF060_09_02=5.28000000000003, SF061a_09_02=0.14399999999999125, SF061b_09_02=0.02400000000000091, SF055_09_03=4, SF056_09_03=1, SF060_09_03=20.08000000000004, SF061a_09_03=-1.3200000000000074, SF061b_09_03=0.5759999999999934, SF055_09_04=1, SF056_09_04=1, SF060_09_04=22.52000000000004, SF061a_09_04=0.6640000000000015, SF061b_09_04=0.2079999999999984, SF055_09_05=2, SF056_09_05=1, SF060_09_05=26.480000000000018, SF061a_09_05=0.30400000000000205, SF061b_09_05=0.45599999999998886, SF055_09_06=1, SF056_09_06=1, SF060_09_06=18.720000000000027, SF061a_09_06=-0.5280000000000058, SF061b_09_06=-0.5600000000000023, SF031_10=19, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=1, SF043_10=0.008000000000000007, SF044_10=1, SF048_10=-0.19599999999999995, SF049a_10=0.0, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF011_10=880836610, SF055_10_01=1, SF056_10_01=1, SF060_10_01=-5.439999999999998, SF061a_10_01=0.32799999999998875, SF061b_10_01=-0.5280000000000058, SF055_10_02=1, SF056_10_02=1, SF060_10_02=-2.0, SF061a_10_02=0.5279999999999916, SF061b_10_02=-0.3760000000000048, SF055_10_03=2, SF056_10_03=1, SF060_10_03=16.640000000000043, SF061a_10_03=-0.9759999999999991, SF061b_10_03=0.11199999999999477, SF055_10_04=1, SF056_10_04=1, SF060_10_04=18.04000000000002, SF061a_10_04=1.4639999999999986, SF061b_10_04=0.1039999999999992, SF055_10_05=1, SF056_10_05=1, SF060_10_05=23.960000000000036, SF061a_10_05=1.215999999999994, SF061b_10_05=0.2079999999999984, SF055_10_06=1, SF056_10_06=1, SF060_10_06=6.560000000000002, SF061a_10_06=0.06399999999999295, SF061b_10_06=-0.9280000000000115)>",
-            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=478, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=32, authInd=1, embAuthLen=0, crc=114625, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=20, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=0.0, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836610, SF055_01_01=1, SF056_01_01=1, SF060_01_01=11.04000000000002, SF061a_01_01=-0.28000000000000114, SF061b_01_01=-0.4480000000000075, SF055_01_02=1, SF056_01_02=1, SF060_01_02=10.640000000000043, SF061a_01_02=0.007999999999995566, SF061b_01_02=-0.3200000000000074, SF055_01_03=2, SF056_01_03=1, SF060_01_03=21.840000000000032, SF061a_01_03=-1.2079999999999984, SF061b_01_03=0.2639999999999958, SF055_01_04=1, SF056_01_04=1, SF060_01_04=24.400000000000034, SF061a_01_04=0.30400000000000205, SF061b_01_04=-0.14400000000000546, SF055_01_05=1, SF056_01_05=1, SF060_01_05=26.120000000000005, SF061a_01_05=0.03999999999999204, SF061b_01_05=0.07199999999998852, SF055_01_06=1, SF056_01_06=1, SF060_01_06=33.879999999999995, SF061a_01_06=-1.152000000000001, SF061b_01_06=-0.9440000000000026, SF031_02=21, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=3, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.16800000000000004, SF049a_02=-0.006000000000000005, SF049b_02=-0.01100000000000001, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836610, SF055_02_01=1, SF056_02_01=1, SF060_02_01=8.28000000000003, SF061a_02_01=-0.35200000000000387, SF061b_02_01=-0.416000000000011, SF055_02_02=1, SF056_02_02=1, SF060_02_02=8.680000000000007, SF061a_02_02=-0.016000000000005343, SF061b_02_02=-0.3119999999999976, SF055_02_03=3, SF056_02_03=1, SF060_02_03=23.560000000000002, SF061a_02_03=-1.0160000000000053, SF061b_02_03=0.23199999999999932, SF055_02_04=1, SF056_02_04=1, SF060_02_04=23.840000000000032, SF061a_02_04=0.27199999999999136, SF061b_02_04=-0.02400000000000091, SF055_02_05=2, SF056_02_05=1, SF060_02_05=26.720000000000027, SF061a_02_05=0.03999999999999204, SF061b_02_05=0.21599999999999397, SF055_02_06=1, SF056_02_06=1, SF060_02_06=28.08000000000004, SF061a_02_06=-0.9120000000000061, SF061b_02_06=-0.9120000000000061, SF031_03=22, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.17600000000000005, SF049a_03=0.007000000000000006, SF049b_03=-0.0030000000000000027, SF054_03=1, SatBitmaskLen_03=0, SF011_03=880836610, SF055_03_01=1, SF056_03_01=1, SF060_03_01=3.7200000000000273, SF061a_03_01=-0.21600000000000819, SF061b_03_01=-0.17600000000000193, SF055_03_02=1, SF056_03_02=1, SF060_03_02=5.0, SF061a_03_02=0.09599999999998943, SF061b_03_02=0.0, SF055_03_03=1, SF056_03_03=1, SF060_03_03=22.600000000000023, SF061a_03_03=-1.3760000000000048, SF061b_03_03=0.6239999999999952, SF055_03_04=1, SF056_03_04=1, SF060_03_04=20.920000000000016, SF061a_03_04=0.5439999999999969, SF061b_03_04=0.09599999999998943, SF055_03_05=2, SF056_03_05=1, SF060_03_05=25.600000000000023, SF061a_03_05=0.17600000000000193, SF061b_03_05=0.32799999999998875, SF055_03_06=1, SF056_03_06=1, SF060_03_06=20.840000000000032, SF061a_03_06=-0.5760000000000076, SF061b_03_06=-0.6880000000000024, SF031_04=23, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.01200000000000001, SF044_04=1, SF048_04=-0.19599999999999995, SF049a_04=-0.01100000000000001, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF011_04=880836610, SF055_04_01=1, SF056_04_01=1, SF060_04_01=2.920000000000016, SF061a_04_01=-0.15200000000000102, SF061b_04_01=-0.08800000000000807, SF055_04_02=1, SF056_04_02=1, SF060_04_02=5.160000000000025, SF061a_04_02=0.1280000000000001, SF061b_04_02=0.07199999999998852, SF055_04_03=2, SF056_04_03=1, SF060_04_03=26.120000000000005, SF061a_04_03=-1.3440000000000083, SF061b_04_03=0.48799999999999955, SF055_04_04=1, SF056_04_04=1, SF060_04_04=21.760000000000048, SF061a_04_04=0.6559999999999917, SF061b_04_04=0.24799999999999045, SF055_04_05=2, SF056_04_05=1, SF060_04_05=27.840000000000032, SF061a_04_05=0.3919999999999959, SF061b_04_05=0.4719999999999942, SF055_04_06=2, SF056_04_06=1, SF060_04_06=17.24000000000001, SF061a_04_06=-0.43200000000000216, SF061b_04_06=-0.5919999999999987, SF031_05=24, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.01200000000000001, SF044_05=1, SF048_05=-0.19599999999999995, SF049a_05=-0.0030000000000000027, SF049b_05=-0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF011_05=880836610, SF055_05_01=1, SF056_05_01=1, SF060_05_01=-2.7999999999999545, SF061a_05_01=0.08799999999999386, SF061b_05_01=-0.2079999999999984, SF055_05_02=1, SF056_05_02=1, SF060_05_02=0.28000000000002956, SF061a_05_02=0.367999999999995, SF061b_05_02=-0.02400000000000091, SF055_05_03=1, SF056_05_03=1, SF060_05_03=23.319999999999993, SF061a_05_03=-0.7680000000000007, SF061b_05_03=0.4159999999999968, SF055_05_04=1, SF056_05_04=1, SF060_05_04=18.52000000000004, SF061a_05_04=0.9039999999999964, SF061b_05_04=0.43200000000000216, SF055_05_05=1, SF056_05_05=1, SF060_05_05=25.400000000000034, SF061a_05_05=0.8160000000000025, SF061b_05_05=0.6640000000000015, SF055_05_06=1, SF056_05_06=1, SF060_05_06=9.04000000000002, SF061a_05_06=-0.04000000000000625, SF061b_05_06=-0.7280000000000086, SF031_06=25, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.18400000000000005, SF049a_06=-0.006000000000000005, SF049b_06=0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF011_06=880836610, SF055_06_01=1, SF056_06_01=1, SF060_06_01=-3.9599999999999795, SF061a_06_01=-0.06400000000000716, SF061b_06_01=-0.1600000000000108, SF055_06_02=1, SF056_06_02=1, SF060_06_02=-0.3599999999999568, SF061a_06_02=0.1599999999999966, SF061b_06_02=-0.04800000000000182, SF055_06_03=2, SF056_06_03=1, SF060_06_03=26.400000000000034, SF061a_06_03=-0.9680000000000035, SF061b_06_03=0.3359999999999985, SF055_06_04=1, SF056_06_04=1, SF060_06_04=19.879999999999995, SF061a_06_04=0.6159999999999997, SF061b_06_04=0.40800000000000125, SF055_06_05=1, SF056_06_05=1, SF060_06_05=27.960000000000036, SF061a_06_05=0.9359999999999928, SF061b_06_05=0.6319999999999908, SF055_06_06=1, SF056_06_06=1, SF060_06_06=5.600000000000023, SF061a_06_06=-0.2560000000000002, SF061b_06_06=-0.5840000000000032, SF031_07=26, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=3, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.17200000000000004, SF049a_07=0.0010000000000000009, SF049b_07=-0.007000000000000006, SF054_07=1, SatBitmaskLen_07=0, SF011_07=880836610, SF055_07_01=1, SF056_07_01=1, SF060_07_01=10.760000000000048, SF061a_07_01=-0.15200000000000102, SF061b_07_01=-1.0720000000000027, SF055_07_02=1, SF056_07_02=1, SF060_07_02=7.840000000000032, SF061a_07_02=0.24799999999999045, SF061b_07_02=-0.8239999999999981, SF055_07_03=2, SF056_07_03=1, SF060_07_03=21.840000000000032, SF061a_07_03=-1.0, SF061b_07_03=-0.016000000000005343, SF055_07_04=1, SF056_07_04=1, SF060_07_04=18.80000000000001, SF061a_07_04=0.8559999999999945, SF061b_07_04=-0.4399999999999977, SF055_07_05=2, SF056_07_05=1, SF060_07_05=20.24000000000001, SF061a_07_05=0.6239999999999952, SF061b_07_05=-0.21600000000000819, SF055_07_06=2, SF056_07_06=1, SF060_07_06=39.31999999999999, SF061a_07_06=-0.5600000000000023, SF061b_07_06=-1.5600000000000023, SF031_08=27, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.016000000000000014, SF044_08=1, SF048_08=-0.19199999999999995, SF049a_08=0.0030000000000000027, SF049b_08=0.0050000000000000044, SF054_08=1, SatBitmaskLen_08=0, SF011_08=880836610, SF055_08_01=1, SF056_08_01=1, SF060_08_01=6.439999999999998, SF061a_08_01=0.24799999999999045, SF061b_08_01=-0.7439999999999998, SF055_08_02=2, SF056_08_02=1, SF060_08_02=5.160000000000025, SF061a_08_02=0.5279999999999916, SF061b_08_02=-0.5440000000000111, SF055_08_03=2, SF056_08_03=1, SF060_08_03=21.80000000000001, SF061a_08_03=-0.7280000000000086, SF061b_08_03=0.08799999999999386, SF055_08_04=1, SF056_08_04=1, SF060_08_04=18.160000000000025, SF061a_08_04=0.695999999999998, SF061b_08_04=-0.3680000000000092, SF055_08_05=2, SF056_08_05=1, SF060_08_05=21.0, SF061a_08_05=0.5999999999999943, SF061b_08_05=-0.11200000000000898, SF055_08_06=2, SF056_08_06=1, SF060_08_06=31.24000000000001, SF061a_08_06=-0.1280000000000001, SF061b_08_06=-1.3760000000000048, SF031_09=28, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.01200000000000001, SF044_09=1, SF048_09=-0.18799999999999994, SF049a_09=-0.008000000000000007, SF049b_09=0.0020000000000000018, SF054_09=1, SatBitmaskLen_09=0, SF011_09=880836610, SF055_09_01=1, SF056_09_01=1, SF060_09_01=3.840000000000032, SF061a_09_01=0.40800000000000125, SF061b_09_01=-0.5919999999999987, SF055_09_02=1, SF056_09_02=1, SF060_09_02=3.240000000000009, SF061a_09_02=0.6479999999999961, SF061b_09_02=-0.5120000000000005, SF055_09_03=2, SF056_09_03=1, SF060_09_03=22.160000000000025, SF061a_09_03=-0.40800000000000125, SF061b_09_03=-0.016000000000005343, SF055_09_04=2, SF056_09_04=1, SF060_09_04=17.319999999999993, SF061a_09_04=0.7999999999999972, SF061b_09_04=-0.1280000000000001, SF055_09_05=2, SF056_09_05=1, SF060_09_05=20.840000000000032, SF061a_09_05=0.6159999999999997, SF061b_09_05=-0.02400000000000091, SF055_09_06=1, SF056_09_06=1, SF060_09_06=25.840000000000032, SF061a_09_06=0.1039999999999992, SF061b_09_06=-1.2800000000000011, SF031_10=29, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=4, SF043_10=0.01200000000000001, SF044_10=1, SF048_10=-0.18799999999999994, SF049a_10=0.045999999999999985, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=0, SF011_10=880836610, SF055_10_01=2, SF056_10_01=1, SF060_10_01=3.920000000000016, SF061a_10_01=0.6400000000000006, SF061b_10_01=-0.6720000000000113, SF055_10_02=1, SF056_10_02=1, SF060_10_02=4.240000000000009, SF061a_10_02=0.9200000000000017, SF061b_10_02=-0.5280000000000058, SF055_10_03=1, SF056_10_03=1, SF060_10_03=25.200000000000045, SF061a_10_03=-0.6800000000000068, SF061b_10_03=0.19999999999998863, SF055_10_04=2, SF056_10_04=1, SF060_10_04=19.04000000000002, SF061a_10_04=1.0079999999999956, SF061b_10_04=-0.4399999999999977, SF055_10_05=2, SF056_10_05=1, SF060_10_05=24.24000000000001, SF061a_10_05=0.9519999999999982, SF061b_10_05=-0.3440000000000083, SF055_10_06=2, SF056_10_06=1, SF060_10_06=22.760000000000048, SF061a_10_06=0.40800000000000125, SF061b_10_06=-1.1839999999999975)>",
-            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=472, eaf=1, crcType=2, frameCrc=6, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=33, authInd=1, embAuthLen=0, crc=8980777, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.18000000000000005, SF049a_01=-0.01200000000000001, SF049b_01=-0.006000000000000005, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836610, SF055_01_01=1, SF056_01_01=1, SF060_01_01=1.1200000000000045, SF061a_01_01=0.7519999999999953, SF061b_01_01=-0.695999999999998, SF055_01_02=1, SF056_01_02=1, SF060_01_02=2.2000000000000455, SF061a_01_02=0.8160000000000025, SF061b_01_02=-0.5760000000000076, SF055_01_03=4, SF056_01_03=1, SF060_01_03=25.400000000000034, SF061a_01_03=-0.12000000000000455, SF061b_01_03=-0.06400000000000716, SF055_01_04=2, SF056_01_04=1, SF060_01_04=17.480000000000018, SF061a_01_04=0.8079999999999927, SF061b_01_04=-0.4720000000000084, SF055_01_05=2, SF056_01_05=1, SF060_01_05=23.480000000000018, SF061a_01_05=0.8719999999999999, SF061b_01_05=-0.22400000000000375, SF055_01_06=2, SF056_01_06=1, SF060_01_06=17.439999999999998, SF061a_01_06=0.4399999999999977, SF061b_01_06=-1.2960000000000065, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.19599999999999995, SF049a_02=0.0050000000000000044, SF049b_02=0.0, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836610, SF055_02_01=2, SF056_02_01=1, SF060_02_01=-2.6399999999999864, SF061a_02_01=0.015999999999991132, SF061b_02_01=-0.15200000000000102, SF055_02_02=2, SF056_02_02=1, SF060_02_02=-0.39999999999997726, SF061a_02_02=0.1039999999999992, SF061b_02_02=0.04800000000000182, SF055_02_03=2, SF056_02_03=1, SF060_02_03=24.80000000000001, SF061a_02_03=-0.6880000000000024, SF061b_02_03=0.46399999999999864, SF055_02_04=1, SF056_02_04=1, SF060_02_04=16.160000000000025, SF061a_02_04=0.30400000000000205, SF061b_02_04=0.37599999999999056, SF055_02_05=2, SF056_02_05=1, SF060_02_05=22.760000000000048, SF061a_02_05=0.43200000000000216, SF061b_02_05=0.48799999999999955, SF055_02_06=2, SF056_02_06=1, SF060_02_06=10.439999999999998, SF061a_02_06=-0.1600000000000108, SF061b_02_06=-0.6480000000000103, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.016000000000000014, SF044_03=1, SF048_03=-0.18799999999999994, SF049a_03=-0.037000000000000005, SF049b_03=-0.006000000000000005, SF054_03=1, SatBitmaskLen_03=0, SF011_03=880836610, SF055_03_01=1, SF056_03_01=1, SF060_03_01=-3.919999999999959, SF061a_03_01=-0.12000000000000455, SF061b_03_01=-0.1600000000000108, SF055_03_02=1, SF056_03_02=1, SF060_03_02=-0.6800000000000068, SF061a_03_02=0.1599999999999966, SF061b_03_02=-0.016000000000005343, SF055_03_03=1, SF056_03_03=1, SF060_03_03=27.840000000000032, SF061a_03_03=-0.5200000000000102, SF061b_03_03=0.1839999999999975, SF055_03_04=1, SF056_03_04=1, SF060_03_04=18.760000000000048, SF061a_03_04=0.19199999999999307, SF061b_03_04=0.3119999999999976, SF055_03_05=2, SF056_03_05=1, SF060_03_05=27.08000000000004, SF061a_03_05=0.11999999999999034, SF061b_03_05=0.7920000000000016, SF055_03_06=1, SF056_03_06=1, SF060_03_06=5.8799999999999955, SF061a_03_06=-0.5600000000000023, SF061b_03_06=-0.632000000000005, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.128, SF049a_04=-0.013000000000000012, SF049b_04=0.0, SF054_04=1, SatBitmaskLen_04=0, SF011_04=880836608, SF055_04_01=1, SF056_04_01=1, SF060_04_01=11.120000000000005, SF061a_04_01=0.30400000000000205, SF061b_04_01=-1.3760000000000048, SF055_04_02=1, SF056_04_02=1, SF060_04_02=6.240000000000009, SF061a_04_02=0.5439999999999969, SF061b_04_02=-0.8400000000000034, SF055_04_03=2, SF056_04_03=1, SF060_04_03=25.0, SF061a_04_03=-0.5440000000000111, SF061b_04_03=-0.1360000000000099, SF055_04_04=3, SF056_04_04=1, SF060_04_04=15.600000000000023, SF061a_04_04=0.6640000000000015, SF061b_04_04=-0.38400000000000034, SF055_04_05=2, SF056_04_05=1, SF060_04_05=17.0, SF061a_04_05=0.8639999999999901, SF061b_04_05=-0.2560000000000002, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.14400000000000002, SF049a_05=-0.021999999999999992, SF049b_05=0.014000000000000012, SF054_05=1, SatBitmaskLen_05=0, SF011_05=880836610, SF055_05_01=2, SF056_05_01=1, SF060_05_01=4.560000000000002, SF061a_05_01=0.48799999999999955, SF061b_05_01=-0.9040000000000106, SF055_05_02=1, SF056_05_02=1, SF060_05_02=2.5200000000000387, SF061a_05_02=0.583999999999989, SF061b_05_02=-0.5600000000000023, SF055_05_03=3, SF056_05_03=1, SF060_05_03=24.960000000000036, SF061a_05_03=-0.632000000000005, SF061b_05_03=-0.09600000000000364, SF055_05_04=3, SF056_05_04=1, SF060_05_04=15.240000000000009, SF061a_05_04=0.4719999999999942, SF061b_05_04=-0.14400000000000546, SF055_05_05=3, SF056_05_05=1, SF060_05_05=17.760000000000048, SF061a_05_05=0.8399999999999892, SF061b_05_05=-0.016000000000005343, SF055_05_06=2, SF056_05_06=1, SF060_05_06=30.160000000000025, SF061a_05_06=0.3919999999999959, SF061b_05_06=-1.6880000000000024, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.016000000000000014, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0030000000000000027, SF049b_06=0.006000000000000005, SF054_06=1, SatBitmaskLen_06=0, SF011_06=880836610, SF055_06_01=1, SF056_06_01=1, SF060_06_01=-1.9599999999999795, SF061a_06_01=0.73599999999999, SF061b_06_01=-0.5760000000000076, SF055_06_02=1, SF056_06_02=1, SF060_06_02=-0.7599999999999909, SF061a_06_02=0.7199999999999989, SF061b_06_02=-0.4399999999999977, SF055_06_03=4, SF056_06_03=1, SF060_06_03=25.160000000000025, SF061a_06_03=-0.23199999999999932, SF061b_06_03=-0.2880000000000109, SF055_06_04=1, SF056_06_04=1, SF060_06_04=15.240000000000009, SF061a_06_04=0.30400000000000205, SF061b_06_04=-0.27200000000000557, SF055_06_05=1, SF056_06_05=1, SF060_06_05=21.480000000000018, SF061a_06_05=0.28000000000000114, SF061b_06_05=-0.11200000000000898, SF055_06_06=2, SF056_06_06=1, SF060_06_06=13.920000000000016, SF061a_06_06=0.7439999999999998, SF061b_06_06=-1.2000000000000028, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=4, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.15200000000000002, SF049a_07=-0.04500000000000001, SF049b_07=-0.015000000000000013, SF054_07=1, SatBitmaskLen_07=0, SF011_07=880836610, SF055_07_01=2, SF056_07_01=1, SF060_07_01=2.160000000000025, SF061a_07_01=-1.1680000000000064, SF061b_07_01=-0.1600000000000108, SF055_07_02=1, SF056_07_02=1, SF060_07_02=4.400000000000034, SF061a_07_02=-1.1039999999999992, SF061b_07_02=-0.02400000000000091, SF055_07_03=5, SF056_07_03=1, SF060_07_03=32.64000000000004, SF061a_07_03=-1.6000000000000014, SF061b_07_03=0.45599999999998886, SF055_07_04=4, SF056_07_04=1, SF060_07_04=22.120000000000005, SF061a_07_04=-1.720000000000006, SF061b_07_04=0.367999999999995, SF055_07_05=3, SF056_07_05=1, SF060_07_05=28.760000000000048, SF061a_07_05=-1.7360000000000042, SF061b_07_05=0.5679999999999978, SF055_07_06=1, SF056_07_06=1, SF060_07_06=14.480000000000018, SF061a_07_06=-1.3599999999999994, SF061b_07_06=-0.5280000000000058, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.016000000000000014, SF044_08=1, SF048_08=-0.16800000000000004, SF049a_08=-0.010000000000000009, SF049b_08=0.009000000000000008, SF054_08=1, SatBitmaskLen_08=0, SF011_08=880836610, SF055_08_01=1, SF056_08_01=1, SF060_08_01=1.080000000000041, SF061a_08_01=-1.3119999999999976, SF061b_08_01=-0.2960000000000065, SF055_08_02=1, SF056_08_02=1, SF060_08_02=3.8799999999999955, SF061a_08_02=-1.112000000000009, SF061b_08_02=-0.14400000000000546, SF055_08_03=4, SF056_08_03=1, SF060_08_03=34.28000000000003, SF061a_08_03=-2.2960000000000065, SF061b_08_03=-0.008000000000009777, SF055_08_04=1, SF056_08_04=1, SF060_08_04=23.28000000000003, SF061a_08_04=-1.5200000000000102, SF061b_08_04=0.1599999999999966, SF055_08_05=1, SF056_08_05=1, SF060_08_05=31.319999999999993, SF061a_08_05=-1.4320000000000022, SF061b_08_05=0.5279999999999916, SF055_08_06=1, SF056_08_06=1, SF060_08_06=11.560000000000002, SF061a_08_06=-1.5200000000000102, SF061b_08_06=-0.6880000000000024, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.15600000000000003, SF049a_09=0.0010000000000000009, SF049b_09=-0.0010000000000000009, SF054_09=1, SatBitmaskLen_09=0, SF011_09=880836610, SF055_09_01=2, SF056_09_01=1, SF060_09_01=-5.319999999999993, SF061a_09_01=1.0159999999999911, SF061b_09_01=-0.7199999999999989, SF055_09_02=2, SF056_09_02=1, SF060_09_02=-3.680000000000007, SF061a_09_02=0.8319999999999936, SF061b_09_02=-0.5040000000000049, SF055_09_03=5, SF056_09_03=1, SF060_09_03=22.640000000000043, SF061a_09_03=1.3999999999999915, SF061b_09_03=-0.19200000000000728, SF055_09_04=2, SF056_09_04=1, SF060_09_04=15.560000000000002, SF061a_09_04=-0.5040000000000049, SF061b_09_04=-0.30400000000000205, SF055_09_05=2, SF056_09_05=1, SF060_09_05=21.560000000000002, SF061a_09_05=-0.3760000000000048, SF061b_09_05=0.015999999999991132, SF055_09_06=2, SF056_09_06=1, SF060_09_06=9.680000000000007, SF061a_09_06=1.1039999999999992, SF061b_09_06=-1.152000000000001, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=4, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.14400000000000002, SF049a_10=0.04999999999999999, SF049b_10=-0.038000000000000006, SF054_10=1, SatBitmaskLen_10=0, SF011_10=880836610, SF055_10_01=1, SF056_10_01=1, SF060_10_01=6.080000000000041, SF061a_10_01=-1.1440000000000055, SF061b_10_01=-0.30400000000000205, SF055_10_02=1, SF056_10_02=1, SF060_10_02=8.680000000000007, SF061a_10_02=-1.328000000000003, SF061b_10_02=-0.23199999999999932, SF055_10_03=1, SF056_10_03=1, SF060_10_03=36.52000000000004, SF061a_10_03=-0.3359999999999985, SF061b_10_03=0.15200000000000102, SF055_10_04=2, SF056_10_04=1, SF060_10_04=31.08000000000004, SF061a_10_04=-3.2080000000000055, SF061b_10_04=0.1599999999999966, SF055_10_05=2, SF056_10_05=1, SF060_10_05=37.44, SF061a_10_05=-2.872000000000007, SF061b_10_05=0.2079999999999984, SF055_10_06=1, SF056_10_06=1, SF060_10_06=18.52000000000004, SF061a_10_06=-1.1839999999999975, SF061b_10_06=-0.632000000000005)>",
-            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=98, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=34, authInd=1, embAuthLen=0, crc=7396141, SF005=152, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.17600000000000005, SF049a_01=-0.017999999999999988, SF049b_01=0.0020000000000000018, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836610, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-10.439999999999998, SF061a_01_01=0.9679999999999893, SF061b_01_01=-0.07200000000000273, SF055_01_02=1, SF056_01_02=1, SF060_01_02=-6.279999999999973, SF061a_01_02=1.2079999999999984, SF061b_01_02=0.055999999999997385, SF055_01_03=3, SF056_01_03=1, SF060_01_03=17.28000000000003, SF061a_01_03=0.4239999999999924, SF061b_01_03=0.3439999999999941, SF055_01_04=2, SF056_01_04=1, SF060_01_04=15.640000000000043, SF061a_01_04=1.9839999999999947, SF061b_01_04=0.5279999999999916, SF055_01_05=1, SF056_01_05=1, SF060_01_05=24.319999999999993, SF061a_01_05=1.8559999999999945, SF061b_01_05=0.8079999999999927, SF055_01_06=1, SF056_01_06=1, SF060_01_06=-1.3199999999999932, SF061a_01_06=0.8160000000000025, SF061b_01_06=-0.45600000000000307, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.18799999999999994, SF049a_02=0.0010000000000000009, SF049b_02=0.0030000000000000027, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836610, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-8.359999999999957, SF061a_02_01=0.9440000000000026, SF061b_02_01=-0.07200000000000273, SF055_02_02=1, SF056_02_02=1, SF060_02_02=-3.599999999999966, SF061a_02_02=1.1359999999999957, SF061b_02_02=0.055999999999997385, SF055_02_03=4, SF056_02_03=1, SF060_02_03=16.920000000000016, SF061a_02_03=-0.960000000000008, SF061b_02_03=0.5120000000000005, SF055_02_04=1, SF056_02_04=1, SF060_02_04=20.480000000000018, SF061a_02_04=2.0319999999999965, SF061b_02_04=0.43200000000000216, SF055_02_05=4, SF056_02_05=1, SF060_02_05=28.80000000000001, SF061a_02_05=1.5600000000000023, SF061b_02_05=0.8160000000000025, SF055_02_06=1, SF056_02_06=1, SF060_02_06=0.28000000000002956, SF061a_02_06=0.9200000000000017, SF061b_02_06=-0.46399999999999864)>",
-            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=421, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=57, authInd=1, embAuthLen=0, crc=15138586, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF012_01=2627632, SF055_01_01=3, SF056_01_01=1, SF060_01_01=-18.519999999999982, SF061a_01_01=0.43200000000000216, SF061b_01_01=-0.3440000000000083, SF055_01_02=4, SF056_01_02=1, SF060_01_02=4.28000000000003, SF061a_01_02=-0.2400000000000091, SF061b_01_02=0.2560000000000002, SF055_01_03=3, SF056_01_03=1, SF060_01_03=-7.1200000000000045, SF061a_01_03=0.3919999999999959, SF061b_01_03=-0.24800000000000466, SF055_01_04=4, SF056_01_04=1, SF060_01_04=-19.71999999999997, SF061a_01_04=-1.1200000000000045, SF061b_01_04=-0.38400000000000034, SF055_01_05=4, SF056_01_05=1, SF060_01_05=-3.0399999999999636, SF061a_01_05=0.0799999999999983, SF061b_01_05=-0.016000000000005343, SF055_01_06=4, SF056_01_06=1, SF060_01_06=-15.279999999999973, SF061a_01_06=-0.9519999999999982, SF061b_01_06=-0.07200000000000273, SF031_02=1, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.0, SF044_02=1, SF048_02=-0.21199999999999997, SF049a_02=-0.0020000000000000018, SF049b_02=0.0, SF054_02=1, SatBitmaskLen_02=0, SF012_02=2627632, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-15.079999999999984, SF061a_02_01=-1.6000000000000014, SF061b_02_01=-0.2560000000000002, SF055_02_02=5, SF056_02_02=1, SF060_02_02=3.7600000000000477, SF061a_02_02=-0.1280000000000001, SF061b_02_02=0.07199999999998852, SF055_02_03=4, SF056_02_03=1, SF060_02_03=-6.359999999999957, SF061a_02_03=0.015999999999991132, SF061b_02_03=-0.27200000000000557, SF055_02_04=4, SF056_02_04=1, SF060_02_04=-10.560000000000002, SF061a_02_04=-2.6240000000000023, SF061b_02_04=-0.5600000000000023, SF055_02_05=3, SF056_02_05=1, SF060_02_05=-3.759999999999991, SF061a_02_05=0.5039999999999907, SF061b_02_05=-0.0799999999999983, SF055_02_06=3, SF056_02_06=1, SF060_02_06=-12.120000000000005, SF061a_02_06=-0.7280000000000086, SF061b_02_06=-0.055999999999997385, SF031_03=2, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=1, SF043_03=0.0, SF044_03=1, SF048_03=-0.21599999999999997, SF049a_03=0.0030000000000000027, SF049b_03=-0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF012_03=2627632, SF055_03_01=3, SF056_03_01=1, SF060_03_01=-17.680000000000007, SF061a_03_01=-1.8400000000000034, SF061b_03_01=-0.38400000000000034, SF055_03_02=2, SF056_03_02=1, SF060_03_02=6.2000000000000455, SF061a_03_02=-0.1360000000000099, SF061b_03_02=0.367999999999995, SF055_03_03=2, SF056_03_03=1, SF060_03_03=-9.239999999999952, SF061a_03_03=0.3999999999999915, SF061b_03_03=-0.38400000000000034, SF055_03_04=5, SF056_03_04=1, SF060_03_04=-14.319999999999993, SF061a_03_04=-2.720000000000006, SF061b_03_04=-0.4480000000000075, SF055_03_05=2, SF056_03_05=1, SF060_03_05=-4.239999999999952, SF061a_03_05=0.6319999999999908, SF061b_03_05=0.007999999999995566, SF055_03_06=2, SF056_03_06=1, SF060_03_06=-12.599999999999966, SF061a_03_06=-1.024000000000001, SF061b_03_06=-0.08800000000000807, SF031_04=3, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.0, SF044_04=1, SF048_04=-0.20799999999999996, SF049a_04=-0.0020000000000000018, SF049b_04=0.0, SF054_04=1, SatBitmaskLen_04=0, SF012_04=2101280, SF055_04_01=2, SF056_04_01=1, SF060_04_01=-10.71999999999997, SF061a_04_01=-0.16800000000000637, SF061b_04_01=-0.1280000000000001, SF055_04_02=2, SF056_04_02=1, SF060_04_02=-3.359999999999957, SF061a_04_02=-0.7040000000000077, SF061b_04_02=-0.06400000000000716, SF055_04_03=3, SF056_04_03=1, SF060_04_03=-3.7999999999999545, SF061a_04_03=0.6559999999999917, SF061b_04_03=-0.008000000000009777, SF031_05=4, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.0, SF044_05=1, SF048_05=-0.20799999999999996, SF049a_05=-0.0030000000000000027, SF049b_05=0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF012_05=2103328, SF055_05_01=1, SF056_05_01=1, SF060_05_01=-12.799999999999955, SF061a_05_01=0.02400000000000091, SF061b_05_01=-0.09600000000000364, SF055_05_02=3, SF056_05_02=1, SF060_05_02=-5.1200000000000045, SF061a_05_02=-1.112000000000009, SF061b_05_02=-0.1600000000000108, SF055_05_03=1, SF056_05_03=1, SF060_05_03=-9.839999999999975, SF061a_05_03=0.29599999999999227, SF061b_05_03=-0.3359999999999985, SF055_05_04=3, SF056_05_04=1, SF060_05_04=-3.8799999999999955, SF061a_05_04=0.7680000000000007, SF061b_05_04=0.07199999999998852, SF031_06=5, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.0, SF044_06=1, SF048_06=-0.18400000000000005, SF049a_06=-0.007000000000000006, SF049b_06=-0.0040000000000000036, SF054_06=1, SatBitmaskLen_06=0, SF012_06=528432, SF055_06_01=2, SF056_06_01=1, SF060_06_01=3.3600000000000136, SF061a_06_01=-0.21600000000000819, SF061b_06_01=-0.4399999999999977, SF055_06_02=3, SF056_06_02=1, SF060_06_02=4.600000000000023, SF061a_06_02=-0.6000000000000085, SF061b_06_02=-0.23199999999999932, SF055_06_03=4, SF056_06_03=1, SF060_06_03=-2.0399999999999636, SF061a_06_03=1.0719999999999885, SF061b_06_03=-0.0799999999999983, SF055_06_04=4, SF056_06_04=1, SF060_06_04=-6.919999999999959, SF061a_06_04=0.29599999999999227, SF061b_06_04=0.4159999999999968, SF031_07=6, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.0040000000000000036, SF044_07=1, SF048_07=-0.19599999999999995, SF049a_07=-0.0020000000000000018, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF012_07=528432, SF055_07_01=3, SF056_07_01=1, SF060_07_01=5.8799999999999955, SF061a_07_01=0.5039999999999907, SF061b_07_01=0.3999999999999915, SF055_07_02=4, SF056_07_02=1, SF060_07_02=2.080000000000041, SF061a_07_02=-0.7280000000000086, SF061b_07_02=-0.35200000000000387, SF055_07_03=4, SF056_07_03=1, SF060_07_03=-3.2799999999999727, SF061a_07_03=1.1679999999999922, SF061b_07_03=-0.11200000000000898, SF055_07_04=4, SF056_07_04=1, SF060_07_04=-6.680000000000007, SF061a_07_04=0.4719999999999942, SF061b_07_04=0.031999999999996476, SF031_08=7, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.0, SF044_08=1, SF048_08=-0.20399999999999996, SF049a_08=-0.0050000000000000044, SF049b_08=-0.0010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF012_08=3676208, SF055_08_01=3, SF056_08_01=1, SF060_08_01=-5.9599999999999795, SF061a_08_01=-0.3200000000000074, SF061b_08_01=-0.38400000000000034, SF055_08_02=3, SF056_08_02=1, SF060_08_02=-11.279999999999973, SF061a_08_02=-0.480000000000004, SF061b_08_02=0.0, SF055_08_03=4, SF056_08_03=1, SF060_08_03=14.920000000000016, SF061a_08_03=-0.5280000000000058, SF061b_08_03=0.40800000000000125, SF055_08_04=2, SF056_08_04=1, SF060_08_04=5.480000000000018, SF061a_08_04=-1.4320000000000022, SF061b_08_04=-0.2560000000000002, SF055_08_05=5, SF056_08_05=1, SF060_08_05=-2.1200000000000045, SF061a_08_05=-0.9040000000000106, SF061b_08_05=-0.28000000000000114, SF055_08_06=1, SF056_08_06=1, SF060_08_06=1.240000000000009, SF061a_08_06=-0.4399999999999977, SF061b_08_06=0.17600000000000193, SF055_08_07=3, SF056_08_07=1, SF060_08_07=-0.7599999999999909, SF061a_08_07=-0.847999999999999, SF061b_08_07=0.13599999999999568, SF031_09=8, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.0040000000000000036, SF044_09=1, SF048_09=-0.14400000000000002, SF049a_09=-0.009000000000000008, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF012_09=3674160, SF055_09_01=3, SF056_09_01=1, SF060_09_01=17.360000000000014, SF061a_09_01=-1.656000000000006, SF061b_09_01=0.1599999999999966, SF055_09_02=2, SF056_09_02=1, SF060_09_02=1.6000000000000227, SF061a_09_02=-0.8640000000000043, SF061b_09_02=0.6640000000000015, SF055_09_03=3, SF056_09_03=1, SF060_09_03=15.920000000000016, SF061a_09_03=-0.5760000000000076, SF061b_09_03=0.6159999999999997, SF055_09_04=2, SF056_09_04=1, SF060_09_04=27.400000000000034, SF061a_09_04=-1.8160000000000025, SF061b_09_04=0.3359999999999985, SF055_09_05=1, SF056_09_05=1, SF060_09_05=14.840000000000032, SF061a_09_05=-0.3200000000000074, SF061b_09_05=0.4959999999999951, SF055_09_06=3, SF056_09_06=1, SF060_09_06=8.840000000000032, SF061a_09_06=-0.7520000000000095, SF061b_09_06=0.519999999999996, SF031_10=9, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.0040000000000000036, SF044_10=1, SF048_10=-0.18799999999999994, SF049a_10=-0.0020000000000000018, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF012_10=3674160, SF055_10_01=2, SF056_10_01=1, SF060_10_01=3.4399999999999977, SF061a_10_01=-1.2160000000000082, SF061b_10_01=-0.6080000000000041, SF055_10_02=2, SF056_10_02=1, SF060_10_02=-6.71999999999997, SF061a_10_02=-0.8080000000000069, SF061b_10_02=-0.2079999999999984, SF055_10_03=3, SF056_10_03=1, SF060_10_03=14.0, SF061a_10_03=-0.8320000000000078, SF061b_10_03=0.15200000000000102, SF055_10_04=4, SF056_10_04=1, SF060_10_04=16.52000000000004, SF061a_10_04=-1.6000000000000014, SF061b_10_04=-0.4960000000000093, SF055_10_05=2, SF056_10_05=1, SF060_10_05=3.920000000000016, SF061a_10_05=-0.3760000000000048, SF061b_10_05=-0.21600000000000819, SF055_10_06=3, SF056_10_06=1, SF060_10_06=3.240000000000009, SF061a_10_06=-1.26400000000001, SF061b_10_06=-0.06400000000000716)>",
-            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=456, eaf=1, crcType=2, frameCrc=2, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=58, authInd=1, embAuthLen=0, crc=14979022, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=10, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0040000000000000036, SF044_01=1, SF048_01=-0.19199999999999995, SF049a_01=-0.0030000000000000027, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF012_01=3676208, SF055_01_01=3, SF056_01_01=1, SF060_01_01=-2.4399999999999977, SF061a_01_01=-1.1839999999999975, SF061b_01_01=-0.3680000000000092, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-9.319999999999993, SF061a_01_02=-0.6080000000000041, SF061b_01_02=0.09599999999998943, SF055_01_03=3, SF056_01_03=1, SF060_01_03=16.439999999999998, SF061a_01_03=-0.5919999999999987, SF061b_01_03=0.4959999999999951, SF055_01_04=3, SF056_01_04=1, SF060_01_04=11.080000000000041, SF061a_01_04=-1.3840000000000003, SF061b_01_04=-0.38400000000000034, SF055_01_05=5, SF056_01_05=1, SF060_01_05=2.2800000000000296, SF061a_01_05=-1.4720000000000084, SF061b_01_05=-0.3359999999999985, SF055_01_06=2, SF056_01_06=1, SF060_01_06=1.6000000000000227, SF061a_01_06=0.007999999999995566, SF061b_01_06=0.11199999999999477, SF055_01_07=4, SF056_01_07=1, SF060_01_07=1.9600000000000364, SF061a_01_07=-0.8239999999999981, SF061b_01_07=0.09599999999998943, SF031_02=11, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.09999999999999998, SF049a_02=-0.0050000000000000044, SF049b_02=-0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=0, SF012_02=3670064, SF055_02_01=2, SF056_02_01=1, SF060_02_01=23.840000000000032, SF061a_02_01=-1.7600000000000051, SF061b_02_01=0.17600000000000193, SF055_02_02=2, SF056_02_02=1, SF060_02_02=2.5600000000000023, SF061a_02_02=-0.8400000000000034, SF061b_02_02=0.7199999999999989, SF055_02_03=3, SF056_02_03=1, SF060_02_03=15.920000000000016, SF061a_02_03=-0.6159999999999997, SF061b_02_03=0.7920000000000016, SF055_02_04=2, SF056_02_04=1, SF060_02_04=14.640000000000043, SF061a_02_04=-0.2880000000000109, SF061b_02_04=0.37599999999999056, SF055_02_05=3, SF056_02_05=1, SF060_02_05=10.04000000000002, SF061a_02_05=-0.8400000000000034, SF061b_02_05=0.6640000000000015, SF031_03=12, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.008000000000000007, SF044_03=1, SF048_03=-0.10799999999999998, SF049a_03=-0.01100000000000001, SF049b_03=-0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF012_03=3670064, SF055_03_01=4, SF056_03_01=1, SF060_03_01=25.360000000000014, SF061a_03_01=-1.7520000000000024, SF061b_03_01=0.15200000000000102, SF055_03_02=1, SF056_03_02=1, SF060_03_02=7.520000000000039, SF061a_03_02=-0.7199999999999989, SF061b_03_02=0.671999999999997, SF055_03_03=1, SF056_03_03=1, SF060_03_03=21.680000000000007, SF061a_03_03=-0.7680000000000007, SF061b_03_03=0.8639999999999901, SF055_03_04=1, SF056_03_04=1, SF060_03_04=17.600000000000023, SF061a_03_04=-0.1600000000000108, SF061b_03_04=0.4399999999999977, SF055_03_05=1, SF056_03_05=1, SF060_03_05=15.360000000000014, SF061a_03_05=-1.112000000000009, SF061b_03_05=0.8639999999999901, SF031_04=13, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=2, SF043_04=0.008000000000000007, SF044_04=1, SF048_04=-0.18000000000000005, SF049a_04=-0.006000000000000005, SF049b_04=-0.0030000000000000027, SF054_04=1, SatBitmaskLen_04=0, SF012_04=3674160, SF055_04_01=1, SF056_04_01=1, SF060_04_01=11.800000000000011, SF061a_04_01=-1.7680000000000078, SF061b_04_01=-0.7360000000000042, SF055_04_02=2, SF056_04_02=1, SF060_04_02=-2.519999999999982, SF061a_04_02=-1.024000000000001, SF061b_04_02=-0.3200000000000074, SF055_04_03=2, SF056_04_03=1, SF060_04_03=15.120000000000005, SF061a_04_03=-0.6000000000000085, SF061b_04_03=0.1280000000000001, SF055_04_04=5, SF056_04_04=1, SF060_04_04=25.160000000000025, SF061a_04_04=-2.064000000000007, SF061b_04_04=-0.4720000000000084, SF055_04_05=1, SF056_04_05=1, SF060_04_05=6.319999999999993, SF061a_04_05=-0.32800000000000296, SF061b_04_05=-0.2560000000000002, SF055_04_06=1, SF056_04_06=1, SF060_04_06=7.720000000000027, SF061a_04_06=-1.240000000000009, SF061b_04_06=-0.0799999999999983, SF031_05=14, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.008000000000000007, SF044_05=1, SF048_05=-0.18000000000000005, SF049a_05=-0.0050000000000000044, SF049b_05=0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF012_05=3674160, SF055_05_01=1, SF056_05_01=1, SF060_05_01=8.04000000000002, SF061a_05_01=-1.6880000000000024, SF061b_05_01=-0.6640000000000015, SF055_05_02=1, SF056_05_02=1, SF060_05_02=-4.0, SF061a_05_02=-0.8719999999999999, SF061b_05_02=-0.40800000000000125, SF055_05_03=3, SF056_05_03=1, SF060_05_03=16.760000000000048, SF061a_05_03=-0.6000000000000085, SF061b_05_03=0.29599999999999227, SF055_05_04=1, SF056_05_04=1, SF060_05_04=23.80000000000001, SF061a_05_04=-2.7520000000000024, SF061b_05_04=-0.5280000000000058, SF055_05_05=2, SF056_05_05=1, SF060_05_05=4.760000000000048, SF061a_05_05=-0.24800000000000466, SF061b_05_05=-0.3440000000000083, SF055_05_06=3, SF056_05_06=1, SF060_05_06=7.439999999999998, SF061a_05_06=-1.3920000000000101, SF061b_05_06=-0.08800000000000807, SF031_06=15, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.008000000000000007, SF044_06=1, SF048_06=-0.19999999999999996, SF049a_06=-0.0030000000000000027, SF049b_06=-0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF012_06=3674160, SF055_06_01=2, SF056_06_01=1, SF060_06_01=5.0400000000000205, SF061a_06_01=-0.9840000000000089, SF061b_06_01=-0.2400000000000091, SF055_06_02=2, SF056_06_02=1, SF060_06_02=-4.479999999999961, SF061a_06_02=-0.3920000000000101, SF061b_06_02=0.16799999999999216, SF055_06_03=3, SF056_06_03=1, SF060_06_03=19.600000000000023, SF061a_06_03=-0.1600000000000108, SF061b_06_03=0.7279999999999944, SF055_06_04=4, SF056_06_04=1, SF060_06_04=19.439999999999998, SF061a_06_04=-1.416000000000011, SF061b_06_04=-0.2400000000000091, SF055_06_05=2, SF056_06_05=1, SF060_06_05=4.360000000000014, SF061a_06_05=0.2879999999999967, SF061b_06_05=0.14399999999999125, SF055_06_06=2, SF056_06_06=1, SF060_06_06=7.920000000000016, SF061a_06_06=-0.8080000000000069, SF061b_06_06=0.19199999999999307, SF031_07=16, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.008000000000000007, SF044_07=1, SF048_07=-0.136, SF049a_07=0.01200000000000001, SF049b_07=-0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF012_07=3670064, SF055_07_01=2, SF056_07_01=1, SF060_07_01=25.439999999999998, SF061a_07_01=-1.088000000000008, SF061b_07_01=-0.960000000000008, SF055_07_02=1, SF056_07_02=1, SF060_07_02=3.8799999999999955, SF061a_07_02=-0.2880000000000109, SF061b_07_02=-0.2400000000000091, SF055_07_03=2, SF056_07_03=1, SF060_07_03=17.400000000000034, SF061a_07_03=-0.008000000000009777, SF061b_07_03=-0.11200000000000898, SF055_07_04=1, SF056_07_04=1, SF060_07_04=12.319999999999993, SF061a_07_04=0.4239999999999924, SF061b_07_04=-0.5200000000000102, SF055_07_05=1, SF056_07_05=1, SF060_07_05=12.480000000000018, SF061a_07_05=-0.695999999999998, SF061b_07_05=0.015999999999991132, SF031_08=17, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.008000000000000007, SF044_08=1, SF048_08=-0.16400000000000003, SF049a_08=0.009000000000000008, SF049b_08=-0.006000000000000005, SF054_08=1, SatBitmaskLen_08=0, SF012_08=3670064, SF055_08_01=2, SF056_08_01=1, SF060_08_01=19.879999999999995, SF061a_08_01=-1.2560000000000002, SF061b_08_01=-0.6640000000000015, SF055_08_02=1, SF056_08_02=1, SF060_08_02=2.2000000000000455, SF061a_08_02=-0.2560000000000002, SF061b_08_02=-0.2960000000000065, SF055_08_03=2, SF056_08_03=1, SF060_08_03=17.560000000000002, SF061a_08_03=0.0, SF061b_08_03=0.11999999999999034, SF055_08_04=1, SF056_08_04=1, SF060_08_04=9.240000000000009, SF061a_08_04=0.35199999999998965, SF061b_08_04=-0.4399999999999977, SF055_08_05=1, SF056_08_05=1, SF060_08_05=12.560000000000002, SF061a_08_05=-0.7680000000000007, SF061b_08_05=-0.008000000000009777, SF031_09=18, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.008000000000000007, SF044_09=1, SF048_09=-0.18000000000000005, SF049a_09=-0.010000000000000009, SF049b_09=-0.0020000000000000018, SF054_09=1, SatBitmaskLen_09=0, SF012_09=3670128, SF055_09_01=4, SF056_09_01=1, SF060_09_01=22.439999999999998, SF061a_09_01=-0.7360000000000042, SF061b_09_01=-0.7199999999999989, SF055_09_02=3, SF056_09_02=1, SF060_09_02=7.680000000000007, SF061a_09_02=0.04800000000000182, SF061b_09_02=-0.35999999999999943, SF055_09_03=3, SF056_09_03=1, SF060_09_03=25.80000000000001, SF061a_09_03=0.2879999999999967, SF061b_09_03=0.1280000000000001, SF055_09_04=3, SF056_09_04=1, SF060_09_04=47.200000000000045, SF061a_09_04=0.8319999999999936, SF061b_09_04=-1.240000000000009, SF055_09_05=1, SF056_09_05=1, SF060_09_05=14.640000000000043, SF061a_09_05=1.0319999999999965, SF061b_09_05=-0.46399999999999864, SF055_09_06=4, SF056_09_06=1, SF060_09_06=20.0, SF061a_09_06=-0.22400000000000375, SF061b_09_06=-0.1839999999999975, SF031_10=19, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=1, SF043_10=0.008000000000000007, SF044_10=1, SF048_10=-0.19599999999999995, SF049a_10=0.0, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF012_10=3674224, SF055_10_01=2, SF056_10_01=1, SF060_10_01=7.360000000000014, SF061a_10_01=-0.695999999999998, SF061b_10_01=-0.3200000000000074, SF055_10_02=1, SF056_10_02=1, SF060_10_02=-3.599999999999966, SF061a_10_02=-0.38400000000000034, SF061b_10_02=0.1839999999999975, SF055_10_03=1, SF056_10_03=1, SF060_10_03=18.80000000000001, SF061a_10_03=0.2639999999999958, SF061b_10_03=0.7119999999999891, SF055_10_04=3, SF056_10_04=1, SF060_10_04=24.08000000000004, SF061a_10_04=-1.9280000000000044, SF061b_10_04=0.0, SF055_10_05=1, SF056_10_05=1, SF060_10_05=31.480000000000018, SF061a_10_05=0.9839999999999947, SF061b_10_05=-0.17600000000000193, SF055_10_06=1, SF056_10_06=1, SF060_10_06=3.480000000000018, SF061a_10_06=0.3919999999999959, SF061b_10_06=0.21599999999999397, SF055_10_07=2, SF056_10_07=1, SF060_10_07=10.240000000000009, SF061a_10_07=-0.936000000000007, SF061b_10_07=0.3199999999999932)>",
-            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=468, eaf=1, crcType=2, frameCrc=5, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=59, authInd=1, embAuthLen=0, crc=11322474, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=20, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=0.0, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF012_01=3670128, SF055_01_01=1, SF056_01_01=1, SF060_01_01=27.400000000000034, SF061a_01_01=-1.152000000000001, SF061b_01_01=-0.8800000000000097, SF055_01_02=1, SF056_01_02=1, SF060_01_02=4.080000000000041, SF061a_01_02=-0.09600000000000364, SF061b_01_02=-0.2560000000000002, SF055_01_03=1, SF056_01_03=1, SF060_01_03=17.08000000000004, SF061a_01_03=0.11999999999999034, SF061b_01_03=-0.008000000000009777, SF055_01_04=1, SF056_01_04=1, SF060_01_04=57.44, SF061a_01_04=-0.07200000000000273, SF061b_01_04=-1.7440000000000069, SF055_01_05=1, SF056_01_05=1, SF060_01_05=10.560000000000002, SF061a_01_05=0.3999999999999915, SF061b_01_05=-0.46399999999999864, SF055_01_06=1, SF056_01_06=1, SF060_01_06=14.160000000000025, SF061a_01_06=-0.5600000000000023, SF061b_01_06=0.07199999999998852, SF031_02=21, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=3, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.16800000000000004, SF049a_02=-0.006000000000000005, SF049b_02=-0.01100000000000001, SF054_02=1, SatBitmaskLen_02=0, SF012_02=3670128, SF055_02_01=1, SF056_02_01=1, SF060_02_01=22.08000000000004, SF061a_02_01=-0.8960000000000008, SF061b_02_01=-0.7680000000000007, SF055_02_02=1, SF056_02_02=1, SF060_02_02=2.400000000000034, SF061a_02_02=-0.1039999999999992, SF061b_02_02=-0.32800000000000296, SF055_02_03=1, SF056_02_03=1, SF060_02_03=17.24000000000001, SF061a_02_03=0.14399999999999125, SF061b_02_03=0.09599999999998943, SF055_02_04=3, SF056_02_04=1, SF060_02_04=46.920000000000016, SF061a_02_04=0.08799999999999386, SF061b_02_04=-1.6160000000000068, SF055_02_05=1, SF056_02_05=1, SF060_02_05=7.8799999999999955, SF061a_02_05=0.4399999999999977, SF061b_02_05=-0.4399999999999977, SF055_02_06=1, SF056_02_06=1, SF060_02_06=14.160000000000025, SF061a_02_06=-0.5679999999999978, SF061b_02_06=-0.09600000000000364, SF031_03=22, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.17600000000000005, SF049a_03=0.007000000000000006, SF049b_03=-0.0030000000000000027, SF054_03=1, SatBitmaskLen_03=0, SF012_03=3670128, SF055_03_01=1, SF056_03_01=1, SF060_03_01=23.879999999999995, SF061a_03_01=0.11199999999999477, SF061b_03_01=-1.0160000000000053, SF055_03_02=1, SF056_03_02=1, SF060_03_02=6.8799999999999955, SF061a_03_02=0.7199999999999989, SF061b_03_02=-0.45600000000000307, SF055_03_03=2, SF056_03_03=1, SF060_03_03=23.80000000000001, SF061a_03_03=1.0879999999999939, SF061b_03_03=-0.12000000000000455, SF055_03_04=2, SF056_03_04=1, SF060_03_04=45.920000000000016, SF061a_03_04=1.039999999999992, SF061b_03_04=-1.2480000000000047, SF055_03_05=1, SF056_03_05=1, SF060_03_05=11.879999999999995, SF061a_03_05=1.4479999999999933, SF061b_03_05=-0.5280000000000058, SF055_03_06=3, SF056_03_06=1, SF060_03_06=20.120000000000005, SF061a_03_06=0.1039999999999992, SF061b_03_06=-0.2560000000000002, SF031_04=23, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.01200000000000001, SF044_04=1, SF048_04=-0.19599999999999995, SF049a_04=-0.01100000000000001, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF012_04=3670112, SF055_04_01=1, SF056_04_01=1, SF060_04_01=18.319999999999993, SF061a_04_01=0.27199999999999136, SF061b_04_01=-0.9280000000000115, SF055_04_02=1, SF056_04_02=1, SF060_04_02=4.480000000000018, SF061a_04_02=0.7039999999999935, SF061b_04_02=-0.3440000000000083, SF055_04_03=1, SF056_04_03=1, SF060_04_03=23.400000000000034, SF061a_04_03=1.2560000000000002, SF061b_04_03=0.02400000000000091, SF055_04_04=2, SF056_04_04=1, SF060_04_04=38.960000000000036, SF061a_04_04=0.7680000000000007, SF061b_04_04=-1.1280000000000001, SF055_04_05=1, SF056_04_05=1, SF060_04_05=9.200000000000045, SF061a_04_05=1.4159999999999968, SF061b_04_05=-0.32800000000000296, SF031_05=24, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.01200000000000001, SF044_05=1, SF048_05=-0.19599999999999995, SF049a_05=-0.0030000000000000027, SF049b_05=-0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF012_05=3670128, SF055_05_01=1, SF056_05_01=1, SF060_05_01=9.28000000000003, SF061a_05_01=-0.35999999999999943, SF061b_05_01=-0.6880000000000024, SF055_05_02=1, SF056_05_02=1, SF060_05_02=-1.5199999999999818, SF061a_05_02=0.031999999999996476, SF061b_05_02=-0.04000000000000625, SF055_05_03=1, SF056_05_03=1, SF060_05_03=19.960000000000036, SF061a_05_03=0.5360000000000014, SF061b_05_03=0.5999999999999943, SF055_05_04=2, SF056_05_04=1, SF060_05_04=30.319999999999993, SF061a_05_04=0.2560000000000002, SF061b_05_04=-0.19200000000000728, SF055_05_05=1, SF056_05_05=1, SF060_05_05=3.4399999999999977, SF061a_05_05=0.6079999999999899, SF061b_05_05=0.06399999999999295, SF055_05_06=1, SF056_05_06=1, SF060_05_06=13.960000000000036, SF061a_05_06=-0.3680000000000092, SF061b_05_06=0.13599999999999568, SF031_06=25, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.18400000000000005, SF049a_06=-0.006000000000000005, SF049b_06=0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF012_06=3672176, SF055_06_01=1, SF056_06_01=1, SF060_06_01=6.240000000000009, SF061a_06_01=-0.09600000000000364, SF061b_06_01=-0.5919999999999987, SF055_06_02=1, SF056_06_02=1, SF060_06_02=-1.7999999999999545, SF061a_06_02=-0.008000000000009777, SF061b_06_02=-0.055999999999997385, SF055_06_03=1, SF056_06_03=1, SF060_06_03=22.400000000000034, SF061a_06_03=0.9200000000000017, SF061b_06_03=0.5120000000000005, SF055_06_04=1, SF056_06_04=1, SF060_06_04=9.240000000000009, SF061a_06_04=-0.2960000000000065, SF061b_06_04=-0.8640000000000043, SF055_06_05=3, SF056_06_05=1, SF060_06_05=30.760000000000048, SF061a_06_05=0.02400000000000091, SF061b_06_05=0.367999999999995, SF055_06_06=1, SF056_06_06=1, SF060_06_06=3.0400000000000205, SF061a_06_06=0.5039999999999907, SF061b_06_06=0.04800000000000182, SF055_06_07=1, SF056_06_07=1, SF060_06_07=14.920000000000016, SF061a_06_07=-0.40800000000000125, SF061b_06_07=0.09599999999998943, SF031_07=26, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=3, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.17200000000000004, SF049a_07=0.0010000000000000009, SF049b_07=-0.007000000000000006, SF054_07=1, SatBitmaskLen_07=0, SF012_07=3670128, SF055_07_01=2, SF056_07_01=1, SF060_07_01=21.0, SF061a_07_01=-1.2480000000000047, SF061b_07_01=-1.0160000000000053, SF055_07_02=1, SF056_07_02=1, SF060_07_02=-10.239999999999952, SF061a_07_02=-0.24800000000000466, SF061b_07_02=-0.30400000000000205, SF055_07_03=2, SF056_07_03=1, SF060_07_03=-0.39999999999997726, SF061a_07_03=0.2879999999999967, SF061b_07_03=0.1599999999999966, SF055_07_04=4, SF056_07_04=1, SF060_07_04=54.28000000000003, SF061a_07_04=-2.5520000000000067, SF061b_07_04=-1.5360000000000014, SF055_07_05=2, SF056_07_05=1, SF060_07_05=-5.519999999999982, SF061a_07_05=0.35999999999999943, SF061b_07_05=-0.45600000000000307, SF055_07_06=1, SF056_07_06=1, SF060_07_06=0.8400000000000318, SF061a_07_06=-0.695999999999998, SF061b_07_06=0.06399999999999295, SF031_08=27, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.016000000000000014, SF044_08=1, SF048_08=-0.19199999999999995, SF049a_08=0.0030000000000000027, SF049b_08=0.0050000000000000044, SF054_08=1, SatBitmaskLen_08=0, SF012_08=3670128, SF055_08_01=3, SF056_08_01=1, SF060_08_01=35.44, SF061a_08_01=-1.3680000000000092, SF061b_08_01=-0.6560000000000059, SF055_08_02=1, SF056_08_02=1, SF060_08_02=8.920000000000016, SF061a_08_02=-0.5840000000000032, SF061b_08_02=0.07199999999998852, SF055_08_03=2, SF056_08_03=1, SF060_08_03=21.439999999999998, SF061a_08_03=-0.35200000000000387, SF061b_08_03=0.32799999999998875, SF055_08_04=5, SF056_08_04=1, SF060_08_04=63.04000000000002, SF061a_08_04=-3.4240000000000066, SF061b_08_04=-1.6160000000000068, SF055_08_05=1, SF056_08_05=1, SF060_08_05=13.319999999999993, SF061a_08_05=-0.08800000000000807, SF061b_08_05=-0.1039999999999992, SF055_08_06=2, SF056_08_06=1, SF060_08_06=21.04000000000002, SF061a_08_06=-1.1680000000000064, SF061b_08_06=0.30400000000000205, SF031_09=28, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.01200000000000001, SF044_09=1, SF048_09=-0.18799999999999994, SF049a_09=-0.008000000000000007, SF049b_09=0.0020000000000000018, SF054_09=1, SatBitmaskLen_09=0, SF012_09=3670128, SF055_09_01=1, SF056_09_01=1, SF060_09_01=32.48000000000002, SF061a_09_01=-1.3599999999999994, SF061b_09_01=-0.632000000000005, SF055_09_02=1, SF056_09_02=1, SF060_09_02=9.080000000000041, SF061a_09_02=-0.6080000000000041, SF061b_09_02=0.06399999999999295, SF055_09_03=2, SF056_09_03=1, SF060_09_03=22.960000000000036, SF061a_09_03=-0.4960000000000093, SF061b_09_03=0.5039999999999907, SF055_09_04=3, SF056_09_04=1, SF060_09_04=57.44, SF061a_09_04=-2.3600000000000065, SF061b_09_04=-1.2960000000000065, SF055_09_05=1, SF056_09_05=1, SF060_09_05=12.680000000000007, SF061a_09_05=-0.17600000000000193, SF061b_09_05=-0.1360000000000099, SF055_09_06=2, SF056_09_06=1, SF060_09_06=22.360000000000014, SF061a_09_06=-1.1839999999999975, SF061b_09_06=0.48799999999999955, SF031_10=29, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=4, SF043_10=0.01200000000000001, SF044_10=1, SF048_10=-0.18799999999999994, SF049a_10=0.045999999999999985, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=0, SF012_10=3670128, SF055_10_01=3, SF056_10_01=1, SF060_10_01=17.0, SF061a_10_01=-0.17600000000000193, SF061b_10_01=-0.784000000000006, SF055_10_02=2, SF056_10_02=1, SF060_10_02=-2.680000000000007, SF061a_10_02=0.3999999999999915, SF061b_10_02=-0.1039999999999992, SF055_10_03=4, SF056_10_03=1, SF060_10_03=13.240000000000009, SF061a_10_03=0.5759999999999934, SF061b_10_03=0.007999999999995566, SF055_10_04=2, SF056_10_04=1, SF060_10_04=39.31999999999999, SF061a_10_04=-1.024000000000001, SF061b_10_04=-0.7760000000000105, SF055_10_05=1, SF056_10_05=1, SF060_10_05=0.7200000000000273, SF061a_10_05=0.7999999999999972, SF061b_10_05=-0.20000000000000284, SF055_10_06=1, SF056_10_06=1, SF060_10_06=11.879999999999995, SF061a_10_06=-0.17600000000000193, SF061b_10_06=0.13599999999999568)>",
-            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=468, eaf=1, crcType=2, frameCrc=5, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=60, authInd=1, embAuthLen=0, crc=13756719, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.18000000000000005, SF049a_01=-0.01200000000000001, SF049b_01=-0.006000000000000005, SF054_01=1, SatBitmaskLen_01=0, SF012_01=3670128, SF055_01_01=2, SF056_01_01=1, SF060_01_01=13.360000000000014, SF061a_01_01=0.0, SF061b_01_01=-0.8400000000000034, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-3.159999999999968, SF061a_01_02=0.4719999999999942, SF061b_01_02=-0.1360000000000099, SF055_01_03=3, SF056_01_03=1, SF060_01_03=13.800000000000011, SF061a_01_03=0.6079999999999899, SF061b_01_03=0.11999999999999034, SF055_01_04=4, SF056_01_04=1, SF060_01_04=35.360000000000014, SF061a_01_04=-1.6400000000000077, SF061b_01_04=-0.960000000000008, SF055_01_05=2, SF056_01_05=1, SF060_01_05=0.0, SF061a_01_05=0.6880000000000024, SF061b_01_05=-0.23199999999999932, SF055_01_06=1, SF056_01_06=1, SF060_01_06=11.920000000000016, SF061a_01_06=0.21599999999999397, SF061b_01_06=-0.08800000000000807, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.19599999999999995, SF049a_02=0.0050000000000000044, SF049b_02=0.0, SF054_02=1, SatBitmaskLen_02=0, SF012_02=3672176, SF055_02_01=2, SF056_02_01=1, SF060_02_01=10.840000000000032, SF061a_02_01=-0.04000000000000625, SF061b_02_01=-0.6159999999999997, SF055_02_02=2, SF056_02_02=1, SF060_02_02=-1.8799999999999955, SF061a_02_02=0.21599999999999397, SF061b_02_02=0.055999999999997385, SF055_02_03=2, SF056_02_03=1, SF060_02_03=17.120000000000005, SF061a_02_03=0.8319999999999936, SF061b_02_03=0.5600000000000023, SF055_02_04=3, SF056_02_04=1, SF060_02_04=16.04000000000002, SF061a_02_04=-0.3359999999999985, SF061b_02_04=-0.936000000000007, SF055_02_05=4, SF056_02_05=1, SF060_02_05=31.439999999999998, SF061a_02_05=-0.7120000000000033, SF061b_02_05=-0.6159999999999997, SF055_02_06=2, SF056_02_06=1, SF060_02_06=1.6000000000000227, SF061a_02_06=0.5519999999999925, SF061b_02_06=0.1599999999999966, SF055_02_07=4, SF056_02_07=1, SF060_02_07=14.360000000000014, SF061a_02_07=-0.27200000000000557, SF061b_02_07=0.32799999999998875, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.016000000000000014, SF044_03=1, SF048_03=-0.18799999999999994, SF049a_03=-0.037000000000000005, SF049b_03=-0.006000000000000005, SF054_03=1, SatBitmaskLen_03=0, SF012_03=3672176, SF055_03_01=1, SF056_03_01=1, SF060_03_01=6.439999999999998, SF061a_03_01=0.16799999999999216, SF061b_03_01=-0.5280000000000058, SF055_03_02=1, SF056_03_02=1, SF060_03_02=-2.079999999999984, SF061a_03_02=0.04800000000000182, SF061b_03_02=-0.1039999999999992, SF055_03_03=2, SF056_03_03=1, SF060_03_03=21.640000000000043, SF061a_03_03=0.7279999999999944, SF061b_03_03=0.8079999999999927, SF055_03_04=1, SF056_03_04=1, SF060_03_04=9.520000000000039, SF061a_03_04=0.16799999999999216, SF061b_03_04=-0.8320000000000078, SF055_03_05=5, SF056_03_05=1, SF060_03_05=31.400000000000034, SF061a_03_05=0.46399999999999864, SF061b_03_05=0.7439999999999998, SF055_03_06=1, SF056_03_06=1, SF060_03_06=1.9600000000000364, SF061a_03_06=0.6319999999999908, SF061b_03_06=0.08799999999999386, SF055_03_07=3, SF056_03_07=1, SF060_03_07=15.920000000000016, SF061a_03_07=0.015999999999991132, SF061b_03_07=0.2879999999999967, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.128, SF049a_04=-0.013000000000000012, SF049b_04=0.0, SF054_04=1, SatBitmaskLen_04=0, SF012_04=3670128, SF055_04_01=6, SF056_04_01=1, SF060_04_01=23.879999999999995, SF061a_04_01=-0.21600000000000819, SF061b_04_01=-0.9759999999999991, SF055_04_02=2, SF056_04_02=1, SF060_04_02=-10.359999999999957, SF061a_04_02=0.28000000000000114, SF061b_04_02=-0.4000000000000057, SF055_04_03=2, SF056_04_03=1, SF060_04_03=-2.919999999999959, SF061a_04_03=0.7759999999999962, SF061b_04_03=0.09599999999998943, SF055_04_04=5, SF056_04_04=1, SF060_04_04=72.72000000000003, SF061a_04_04=-5.648000000000003, SF061b_04_04=-0.5679999999999978, SF055_04_05=2, SF056_04_05=1, SF060_04_05=-7.639999999999986, SF061a_04_05=0.5360000000000014, SF061b_04_05=-0.3359999999999985, SF055_04_06=4, SF056_04_06=1, SF060_04_06=2.680000000000007, SF061a_04_06=-0.17600000000000193, SF061b_04_06=-0.07200000000000273, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.14400000000000002, SF049a_05=-0.021999999999999992, SF049b_05=0.014000000000000012, SF054_05=1, SatBitmaskLen_05=0, SF012_05=3670128, SF055_05_01=4, SF056_05_01=1, SF060_05_01=40.160000000000025, SF061a_05_01=-0.8960000000000008, SF061b_05_01=-0.9120000000000061, SF055_05_02=4, SF056_05_02=1, SF060_05_02=11.120000000000005, SF061a_05_02=-0.4000000000000057, SF061b_05_02=0.04800000000000182, SF055_05_03=4, SF056_05_03=1, SF060_05_03=22.52000000000004, SF061a_05_03=-0.14400000000000546, SF061b_05_03=0.4399999999999977, SF055_05_04=6, SF056_05_04=1, SF060_05_04=86.12, SF061a_05_04=-6.736000000000004, SF061b_05_04=-1.9280000000000044, SF055_05_05=3, SF056_05_05=1, SF060_05_05=13.879999999999995, SF061a_05_05=-0.22400000000000375, SF061b_05_05=-0.016000000000005343, SF055_05_06=4, SF056_05_06=1, SF060_05_06=25.760000000000048, SF061a_05_06=-0.8400000000000034, SF061b_05_06=0.1839999999999975, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.016000000000000014, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0030000000000000027, SF049b_06=0.006000000000000005, SF054_06=1, SatBitmaskLen_06=0, SF012_06=3670128, SF055_06_01=2, SF056_06_01=1, SF060_06_01=11.400000000000034, SF061a_06_01=0.5759999999999934, SF061b_06_01=-0.7280000000000086, SF055_06_02=2, SF056_06_02=1, SF060_06_02=-4.8799999999999955, SF061a_06_02=0.5759999999999934, SF061b_06_02=-0.06400000000000716, SF055_06_03=2, SF056_06_03=1, SF060_06_03=12.480000000000018, SF061a_06_03=0.47999999999998977, SF061b_06_03=0.23999999999999488, SF055_06_04=5, SF056_06_04=1, SF060_06_04=40.68000000000001, SF061a_06_04=-3.7040000000000077, SF061b_06_04=-1.2720000000000056, SF055_06_05=1, SF056_06_05=1, SF060_06_05=-2.0, SF061a_06_05=0.519999999999996, SF061b_06_05=-0.04000000000000625, SF055_06_06=5, SF056_06_06=1, SF060_06_06=11.120000000000005, SF061a_06_06=0.4399999999999977, SF061b_06_06=0.11999999999999034, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=4, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.15200000000000002, SF049a_07=-0.04500000000000001, SF049b_07=-0.015000000000000013, SF054_07=1, SatBitmaskLen_07=0, SF012_07=3670128, SF055_07_01=1, SF056_07_01=1, SF060_07_01=16.760000000000048, SF061a_07_01=-0.7360000000000042, SF061b_07_01=-0.9120000000000061, SF055_07_02=1, SF056_07_02=1, SF060_07_02=4.960000000000036, SF061a_07_02=-0.6480000000000103, SF061b_07_02=-0.3440000000000083, SF055_07_03=4, SF056_07_03=1, SF060_07_03=24.439999999999998, SF061a_07_03=-0.8400000000000034, SF061b_07_03=0.23199999999999932, SF055_07_04=4, SF056_07_04=1, SF060_07_04=40.120000000000005, SF061a_07_04=-2.0160000000000053, SF061b_07_04=-1.1839999999999975, SF055_07_05=2, SF056_07_05=1, SF060_07_05=7.960000000000036, SF061a_07_05=-0.7120000000000033, SF061b_07_05=-0.21600000000000819, SF055_07_06=1, SF056_07_06=1, SF060_07_06=22.24000000000001, SF061a_07_06=-0.7040000000000077, SF061b_07_06=-0.0799999999999983, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.016000000000000014, SF044_08=1, SF048_08=-0.16800000000000004, SF049a_08=-0.010000000000000009, SF049b_08=0.009000000000000008, SF054_08=1, SatBitmaskLen_08=0, SF012_08=3670128, SF055_08_01=1, SF056_08_01=1, SF060_08_01=12.600000000000023, SF061a_08_01=-0.6800000000000068, SF061b_08_01=-0.784000000000006, SF055_08_02=1, SF056_08_02=1, SF060_08_02=3.319999999999993, SF061a_08_02=-0.5520000000000067, SF061b_08_02=-0.30400000000000205, SF055_08_03=2, SF056_08_03=1, SF060_08_03=25.80000000000001, SF061a_08_03=-0.40800000000000125, SF061b_08_03=0.35199999999998965, SF055_08_04=2, SF056_08_04=1, SF060_08_04=36.80000000000001, SF061a_08_04=-0.9120000000000061, SF061b_08_04=-0.12000000000000455, SF055_08_05=1, SF056_08_05=1, SF060_08_05=6.960000000000036, SF061a_08_05=-0.4480000000000075, SF061b_08_05=-0.1600000000000108, SF055_08_06=2, SF056_08_06=1, SF060_08_06=21.640000000000043, SF061a_08_06=-0.695999999999998, SF061b_08_06=-0.1839999999999975, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.15600000000000003, SF049a_09=0.0010000000000000009, SF049b_09=-0.0010000000000000009, SF054_09=1, SatBitmaskLen_09=0, SF012_09=3670048, SF055_09_01=1, SF056_09_01=1, SF060_09_01=7.920000000000016, SF061a_09_01=0.8960000000000008, SF061b_09_01=-0.6240000000000094, SF055_09_02=4, SF056_09_02=1, SF060_09_02=-7.519999999999982, SF061a_09_02=0.7439999999999998, SF061b_09_02=0.0799999999999983, SF055_09_03=1, SF056_09_03=1, SF060_09_03=11.160000000000025, SF061a_09_03=0.367999999999995, SF061b_09_03=0.16799999999999216, SF055_09_04=3, SF056_09_04=1, SF060_09_04=-3.4399999999999977, SF061a_09_04=0.19999999999998863, SF061b_09_04=0.08799999999999386, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=4, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.14400000000000002, SF049a_10=0.04999999999999999, SF049b_10=-0.038000000000000006, SF054_10=1, SatBitmaskLen_10=0, SF012_10=3670128, SF055_10_01=1, SF056_10_01=1, SF060_10_01=17.760000000000048, SF061a_10_01=-0.22400000000000375, SF061b_10_01=-0.5679999999999978, SF055_10_02=1, SF056_10_02=1, SF060_10_02=6.0400000000000205, SF061a_10_02=-0.04800000000000182, SF061b_10_02=-0.14400000000000546, SF055_10_03=1, SF056_10_03=1, SF060_10_03=28.200000000000045, SF061a_10_03=-1.0480000000000018, SF061b_10_03=0.30400000000000205, SF055_10_04=2, SF056_10_04=1, SF060_10_04=46.879999999999995, SF061a_10_04=-2.768000000000008, SF061b_10_04=-2.216000000000001, SF055_10_05=1, SF056_10_05=1, SF060_10_05=10.439999999999998, SF061a_10_05=-0.7040000000000077, SF061b_10_05=-0.06400000000000716, SF055_10_06=1, SF056_10_06=1, SF060_10_06=23.840000000000032, SF061a_10_06=-0.1039999999999992, SF061b_10_06=0.0799999999999983)>",
-            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=61, eaf=1, crcType=2, frameCrc=15, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=61, authInd=1, embAuthLen=0, crc=13417473, SF005=152, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.17600000000000005, SF049a_01=-0.017999999999999988, SF049b_01=0.0020000000000000018, SF054_01=1, SatBitmaskLen_01=0, SF012_01=4144, SF055_01_01=5, SF056_01_01=1, SF060_01_01=26.960000000000036, SF061a_01_01=-1.6000000000000014, SF061b_01_01=-0.416000000000011, SF055_01_02=1, SF056_01_02=1, SF060_01_02=6.160000000000025, SF061a_01_02=0.73599999999999, SF061b_01_02=-0.07200000000000273, SF055_01_03=2, SF056_01_03=1, SF060_01_03=16.160000000000025, SF061a_01_03=-0.4960000000000093, SF061b_01_03=0.13599999999999568, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.18799999999999994, SF049a_02=0.0010000000000000009, SF049b_02=0.0030000000000000027, SF054_02=1, SatBitmaskLen_02=0, SF012_02=4144, SF055_02_01=5, SF056_02_01=1, SF060_02_01=23.920000000000016, SF061a_02_01=-0.5520000000000067, SF061b_02_01=-0.45600000000000307, SF055_02_02=1, SF056_02_02=1, SF060_02_02=7.680000000000007, SF061a_02_02=0.7599999999999909, SF061b_02_02=-0.09600000000000364, SF055_02_03=2, SF056_02_03=1, SF060_02_03=15.28000000000003, SF061a_02_03=-0.3920000000000101, SF061b_02_03=0.1280000000000001)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, PRN_01_01=3, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, SF061a_01_01=-0.8960000000000008, SF061b_01_01=-0.15200000000000102, PRN_01_02=4, SF055_01_02=1, SF056_01_02=1, SF060_01_02=-2.0, SF061a_01_02=0.6319999999999908, SF061b_01_02=-0.04000000000000625, PRN_01_03=6, SF055_01_03=3, SF056_01_03=1, SF060_01_03=-1.6800000000000068, SF061a_01_03=0.35999999999999943, SF061b_01_03=0.1280000000000001, PRN_01_04=9, SF055_01_04=3, SF056_01_04=1, SF060_01_04=27.439999999999998, SF061a_01_04=0.4719999999999942, SF061b_01_04=0.23999999999999488, PRN_01_05=17, SF055_01_05=5, SF056_01_05=1, SF060_01_05=24.560000000000002, SF061a_01_05=0.6640000000000015, SF061b_01_05=0.2079999999999984, PRN_01_06=25, SF055_01_06=5, SF056_01_06=1, SF060_01_06=16.480000000000018, SF061a_01_06=-0.936000000000007, SF061b_01_06=-0.23199999999999932, PRN_01_07=31, SF055_01_07=4, SF056_01_07=1, SF060_01_07=-8.639999999999986, SF061a_01_07=-1.872000000000007, SF061b_01_07=-0.24800000000000466, SF031_02=1, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.0, SF044_02=1, SF048_02=-0.21199999999999997, SF049a_02=-0.0020000000000000018, SF049b_02=0.0, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836738, PRN_02_01=3, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-9.120000000000005, SF061a_02_01=0.11199999999999477, SF061b_02_01=-0.14400000000000546, PRN_02_02=4, SF055_02_02=1, SF056_02_02=1, SF060_02_02=-3.319999999999993, SF061a_02_02=0.35199999999998965, SF061b_02_02=-0.06400000000000716, PRN_02_03=6, SF055_02_03=3, SF056_02_03=1, SF060_02_03=-1.1999999999999886, SF061a_02_03=-0.8320000000000078, SF061b_02_03=0.055999999999997385, PRN_02_04=9, SF055_02_04=4, SF056_02_04=1, SF060_02_04=23.920000000000016, SF061a_02_04=0.6479999999999961, SF061b_02_04=0.5039999999999907, PRN_02_05=17, SF055_02_05=5, SF056_02_05=1, SF060_02_05=20.680000000000007, SF061a_02_05=-0.17600000000000193, SF061b_02_05=0.47999999999998977, PRN_02_06=25, SF055_02_06=6, SF056_02_06=1, SF060_02_06=14.920000000000016, SF061a_02_06=0.8160000000000025, SF061b_02_06=1.0319999999999965, PRN_02_07=31, SF055_02_07=4, SF056_02_07=1, SF060_02_07=-1.8799999999999955, SF061a_02_07=-1.1440000000000055, SF061b_02_07=-0.2880000000000109, SF031_03=2, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=1, SF043_03=0.0, SF044_03=1, SF048_03=-0.21599999999999997, SF049a_03=0.0030000000000000027, SF049b_03=-0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF011_03=880836738, PRN_03_01=3, SF055_03_01=2, SF056_03_01=1, SF060_03_01=-10.359999999999957, SF061a_03_01=0.11999999999999034, SF061b_03_01=-0.09600000000000364, PRN_03_02=4, SF055_03_02=2, SF056_03_02=1, SF060_03_02=-3.5600000000000023, SF061a_03_02=0.23999999999999488, SF061b_03_02=0.007999999999995566, PRN_03_03=6, SF055_03_03=2, SF056_03_03=1, SF060_03_03=-0.8799999999999955, SF061a_03_03=-0.8160000000000025, SF061b_03_03=0.0799999999999983, PRN_03_04=9, SF055_03_04=2, SF056_03_04=1, SF060_03_04=26.400000000000034, SF061a_03_04=0.5759999999999934, SF061b_03_04=0.2560000000000002, PRN_03_05=17, SF055_03_05=4, SF056_03_05=1, SF060_03_05=25.04000000000002, SF061a_03_05=-0.22400000000000375, SF061b_03_05=0.38400000000000034, PRN_03_06=25, SF055_03_06=6, SF056_03_06=1, SF060_03_06=15.600000000000023, SF061a_03_06=-0.04800000000000182, SF061b_03_06=-0.3200000000000074, PRN_03_07=31, SF055_03_07=4, SF056_03_07=1, SF060_03_07=-4.519999999999982, SF061a_03_07=-0.960000000000008, SF061b_03_07=-0.27200000000000557, SF031_04=3, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.0, SF044_04=1, SF048_04=-0.20799999999999996, SF049a_04=-0.0020000000000000018, SF049b_04=0.0, SF054_04=1, SatBitmaskLen_04=0, SF011_04=880836610, PRN_04_01=3, SF055_04_01=1, SF056_04_01=1, SF060_04_01=-8.71999999999997, SF061a_04_01=0.11999999999999034, SF061b_04_01=-0.11200000000000898, PRN_04_02=4, SF055_04_02=1, SF056_04_02=1, SF060_04_02=-3.759999999999991, SF061a_04_02=0.28000000000000114, SF061b_04_02=-0.04000000000000625, PRN_04_03=6, SF055_04_03=4, SF056_04_03=1, SF060_04_03=0.4000000000000341, SF061a_04_03=-0.27200000000000557, SF061b_04_03=0.03999999999999204, PRN_04_04=9, SF055_04_04=4, SF056_04_04=1, SF060_04_04=20.840000000000032, SF061a_04_04=0.3439999999999941, SF061b_04_04=0.4959999999999951, PRN_04_05=17, SF055_04_05=4, SF056_04_05=1, SF060_04_05=17.680000000000007, SF061a_04_05=-0.32800000000000296, SF061b_04_05=0.5039999999999907, PRN_04_06=31, SF055_04_06=1, SF056_04_06=1, SF060_04_06=1.1200000000000045, SF061a_04_06=-0.4000000000000057, SF061b_04_06=-0.32800000000000296, SF031_05=4, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.0, SF044_05=1, SF048_05=-0.20799999999999996, SF049a_05=-0.0030000000000000027, SF049b_05=0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF011_05=880836610, PRN_05_01=3, SF055_05_01=2, SF056_05_01=1, SF060_05_01=-10.359999999999957, SF061a_05_01=0.43200000000000216, SF061b_05_01=-0.0799999999999983, PRN_05_02=4, SF055_05_02=3, SF056_05_02=1, SF060_05_02=-4.479999999999961, SF061a_05_02=0.1599999999999966, SF061b_05_02=-0.03200000000001069, PRN_05_03=6, SF055_05_03=2, SF056_05_03=1, SF060_05_03=2.640000000000043, SF061a_05_03=-0.7360000000000042, SF061b_05_03=0.14399999999999125, PRN_05_04=9, SF055_05_04=3, SF056_05_04=1, SF060_05_04=25.439999999999998, SF061a_05_04=0.6319999999999908, SF061b_05_04=0.2079999999999984, PRN_05_05=17, SF055_05_05=3, SF056_05_05=1, SF060_05_05=25.920000000000016, SF061a_05_05=-0.3760000000000048, SF061b_05_05=0.37599999999999056, PRN_05_06=31, SF055_05_06=3, SF056_05_06=1, SF060_05_06=-3.6399999999999864, SF061a_05_06=0.23999999999999488, SF061b_05_06=-0.35999999999999943, SF031_06=5, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.0, SF044_06=1, SF048_06=-0.18400000000000005, SF049a_06=-0.007000000000000006, SF049b_06=-0.0040000000000000036, SF054_06=1, SatBitmaskLen_06=0, SF011_06=880836610, PRN_06_01=3, SF055_06_01=2, SF056_06_01=1, SF060_06_01=-3.2799999999999727, SF061a_06_01=-0.2079999999999984, SF061b_06_01=-0.23199999999999932, PRN_06_02=4, SF055_06_02=4, SF056_06_02=1, SF060_06_02=0.4399999999999977, SF061a_06_02=-0.06400000000000716, SF061b_06_02=-0.03200000000001069, PRN_06_03=6, SF055_06_03=3, SF056_06_03=1, SF060_06_03=5.0400000000000205, SF061a_06_03=-0.1839999999999975, SF061b_06_03=-0.008000000000009777, PRN_06_04=9, SF055_06_04=3, SF056_06_04=1, SF060_06_04=23.680000000000007, SF061a_06_04=0.04800000000000182, SF061b_06_04=-0.08800000000000807, PRN_06_05=17, SF055_06_05=4, SF056_06_05=1, SF060_06_05=22.560000000000002, SF061a_06_05=-0.5440000000000111, SF061b_06_05=0.13599999999999568, PRN_06_06=31, SF055_06_06=2, SF056_06_06=1, SF060_06_06=8.520000000000039, SF061a_06_06=-0.48799999999999955, SF061b_06_06=-0.5520000000000067, SF031_07=6, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.0040000000000000036, SF044_07=1, SF048_07=-0.19599999999999995, SF049a_07=-0.0020000000000000018, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF011_07=880836610, PRN_07_01=3, SF055_07_01=2, SF056_07_01=1, SF060_07_01=-5.639999999999986, SF061a_07_01=-0.055999999999997385, SF061b_07_01=-0.35200000000000387, PRN_07_02=4, SF055_07_02=2, SF056_07_02=1, SF060_07_02=-0.839999999999975, SF061a_07_02=-0.27200000000000557, SF061b_07_02=-0.3760000000000048, PRN_07_03=6, SF055_07_03=2, SF056_07_03=1, SF060_07_03=6.8799999999999955, SF061a_07_03=-0.8080000000000069, SF061b_07_03=0.13599999999999568, PRN_07_04=9, SF055_07_04=3, SF056_07_04=1, SF060_07_04=23.920000000000016, SF061a_07_04=0.35199999999998965, SF061b_07_04=-0.02400000000000091, PRN_07_05=17, SF055_07_05=2, SF056_07_05=1, SF060_07_05=24.400000000000034, SF061a_07_05=-0.43200000000000216, SF061b_07_05=0.5120000000000005, PRN_07_06=31, SF055_07_06=1, SF056_07_06=1, SF060_07_06=4.520000000000039, SF061a_07_06=-0.3760000000000048, SF061b_07_06=-0.632000000000005, SF031_08=7, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.0, SF044_08=1, SF048_08=-0.20399999999999996, SF049a_08=-0.0050000000000000044, SF049b_08=-0.0010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF011_08=880836610, PRN_08_01=3, SF055_08_01=5, SF056_08_01=1, SF060_08_01=-8.319999999999993, SF061a_08_01=-0.5440000000000111, SF061b_08_01=0.007999999999995566, PRN_08_02=4, SF055_08_02=3, SF056_08_02=1, SF060_08_02=-2.6399999999999864, SF061a_08_02=-0.5120000000000005, SF061b_08_02=0.17600000000000193, PRN_08_03=6, SF055_08_03=2, SF056_08_03=1, SF060_08_03=7.560000000000002, SF061a_08_03=-1.0799999999999983, SF061b_08_03=0.3199999999999932, PRN_08_04=9, SF055_08_04=3, SF056_08_04=1, SF060_08_04=25.680000000000007, SF061a_08_04=0.23199999999999932, SF061b_08_04=0.29599999999999227, PRN_08_05=17, SF055_08_05=4, SF056_08_05=1, SF060_08_05=28.720000000000027, SF061a_08_05=-0.3359999999999985, SF061b_08_05=0.7439999999999998, PRN_08_06=31, SF055_08_06=4, SF056_08_06=1, SF060_08_06=-0.9199999999999591, SF061a_08_06=-0.30400000000000205, SF061b_08_06=-0.3920000000000101, SF031_09=8, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.0040000000000000036, SF044_09=1, SF048_09=-0.14400000000000002, SF049a_09=-0.009000000000000008, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF011_09=880836610, PRN_09_01=3, SF055_09_01=2, SF056_09_01=1, SF060_09_01=0.6800000000000068, SF061a_09_01=-1.3359999999999985, SF061b_09_01=-0.055999999999997385, PRN_09_02=4, SF055_09_02=2, SF056_09_02=1, SF060_09_02=2.9600000000000364, SF061a_09_02=-0.9200000000000017, SF061b_09_02=0.21599999999999397, PRN_09_03=6, SF055_09_03=2, SF056_09_03=1, SF060_09_03=6.2000000000000455, SF061a_09_03=-1.240000000000009, SF061b_09_03=0.0799999999999983, PRN_09_04=9, SF055_09_04=1, SF056_09_04=1, SF060_09_04=20.0, SF061a_09_04=-0.784000000000006, SF061b_09_04=0.1839999999999975, PRN_09_05=17, SF055_09_05=3, SF056_09_05=1, SF060_09_05=17.720000000000027, SF061a_09_05=-0.9280000000000115, SF061b_09_05=0.22399999999998954, PRN_09_06=31, SF055_09_06=2, SF056_09_06=1, SF060_09_06=17.0, SF061a_09_06=-2.1680000000000064, SF061b_09_06=-0.3920000000000101, SF031_10=9, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.0040000000000000036, SF044_10=1, SF048_10=-0.18799999999999994, SF049a_10=-0.0020000000000000018, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF011_10=880836610, PRN_10_01=3, SF055_10_01=1, SF056_10_01=1, SF060_10_01=-4.399999999999977, SF061a_10_01=-0.8320000000000078, SF061b_10_01=-0.5200000000000102, PRN_10_02=4, SF055_10_02=2, SF056_10_02=1, SF060_10_02=-0.4399999999999977, SF061a_10_02=-0.6560000000000059, SF061b_10_02=-0.2960000000000065, PRN_10_03=6, SF055_10_03=3, SF056_10_03=1, SF060_10_03=8.960000000000036, SF061a_10_03=-1.4399999999999977, SF061b_10_03=0.14399999999999125, PRN_10_04=9, SF055_10_04=2, SF056_10_04=1, SF060_10_04=21.960000000000036, SF061a_10_04=0.16799999999999216, SF061b_10_04=-0.04000000000000625, PRN_10_05=17, SF055_10_05=4, SF056_10_05=1, SF060_10_05=23.760000000000048, SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, PRN_10_06=31, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=478, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=31, authInd=1, embAuthLen=0, crc=8969842, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=10, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0040000000000000036, SF044_01=1, SF048_01=-0.19199999999999995, SF049a_01=-0.0030000000000000027, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836610, PRN_01_01=3, SF055_01_01=2, SF056_01_01=1, SF060_01_01=-6.279999999999973, SF061a_01_01=-0.5440000000000111, SF061b_01_01=0.0, PRN_01_02=4, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-1.3599999999999568, SF061a_01_02=-0.30400000000000205, SF061b_01_02=0.21599999999999397, PRN_01_03=6, SF055_01_03=2, SF056_01_03=1, SF060_01_03=11.319999999999993, SF061a_01_03=-1.2240000000000038, SF061b_01_03=0.30400000000000205, PRN_01_04=9, SF055_01_04=2, SF056_01_04=1, SF060_01_04=24.680000000000007, SF061a_01_04=0.1599999999999966, SF061b_01_04=0.37599999999999056, PRN_01_05=17, SF055_01_05=3, SF056_01_05=1, SF060_01_05=28.840000000000032, SF061a_01_05=-0.3359999999999985, SF061b_01_05=0.8960000000000008, PRN_01_06=31, SF055_01_06=3, SF056_01_06=1, SF060_01_06=2.5200000000000387, SF061a_01_06=-1.088000000000008, SF061b_01_06=-0.17600000000000193, SF031_02=11, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.09999999999999998, SF049a_02=-0.0050000000000000044, SF049b_02=-0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836610, PRN_02_01=3, SF055_02_01=2, SF056_02_01=1, SF060_02_01=6.160000000000025, SF061a_02_01=-1.2319999999999993, SF061b_02_01=-0.03200000000001069, PRN_02_02=4, SF055_02_02=1, SF056_02_02=1, SF060_02_02=6.600000000000023, SF061a_02_02=-0.9680000000000035, SF061b_02_02=0.06399999999999295, PRN_02_03=6, SF055_02_03=1, SF056_02_03=1, SF060_02_03=11.360000000000014, SF061a_02_03=-1.2480000000000047, SF061b_02_03=-0.1039999999999992, PRN_02_04=9, SF055_02_04=3, SF056_02_04=1, SF060_02_04=22.360000000000014, SF061a_02_04=-0.4720000000000084, SF061b_02_04=0.0799999999999983, PRN_02_05=17, SF055_02_05=2, SF056_02_05=1, SF060_02_05=20.439999999999998, SF061a_02_05=-0.9040000000000106, SF061b_02_05=0.43200000000000216, PRN_02_06=31, SF055_02_06=1, SF056_02_06=1, SF060_02_06=27.319999999999993, SF061a_02_06=-2.112000000000002, SF061b_02_06=-0.3440000000000083, SF031_03=12, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.008000000000000007, SF044_03=1, SF048_03=-0.10799999999999998, SF049a_03=-0.01100000000000001, SF049b_03=-0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF011_03=880836610, PRN_03_01=3, SF055_03_01=1, SF056_03_01=1, SF060_03_01=5.560000000000002, SF061a_03_01=-1.2000000000000028, SF061b_03_01=-0.1360000000000099, PRN_03_02=4, SF055_03_02=1, SF056_03_02=1, SF060_03_02=7.1200000000000045, SF061a_03_02=-0.8560000000000088, SF061b_03_02=0.0799999999999983, PRN_03_03=6, SF055_03_03=2, SF056_03_03=1, SF060_03_03=12.520000000000039, SF061a_03_03=-1.4720000000000084, SF061b_03_03=0.4479999999999933, PRN_03_04=9, SF055_03_04=1, SF056_03_04=1, SF060_03_04=23.04000000000002, SF061a_03_04=-0.4000000000000057, SF061b_03_04=0.15200000000000102, PRN_03_05=17, SF055_03_05=1, SF056_03_05=1, SF060_03_05=22.80000000000001, SF061a_03_05=-0.9519999999999982, SF061b_03_05=0.29599999999999227, PRN_03_06=31, SF055_03_06=2, SF056_03_06=1, SF060_03_06=23.80000000000001, SF061a_03_06=-1.9280000000000044, SF061b_03_06=-0.632000000000005, SF031_04=13, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=2, SF043_04=0.008000000000000007, SF044_04=1, SF048_04=-0.18000000000000005, SF049a_04=-0.006000000000000005, SF049b_04=-0.0030000000000000027, SF054_04=1, SatBitmaskLen_04=0, SF011_04=880836610, PRN_04_01=3, SF055_04_01=1, SF056_04_01=1, SF060_04_01=0.8400000000000318, SF061a_04_01=-0.6720000000000113, SF061b_04_01=-0.5120000000000005, PRN_04_02=4, SF055_04_02=2, SF056_04_02=1, SF060_04_02=3.319999999999993, SF061a_04_02=-0.3440000000000083, SF061b_04_02=-0.4399999999999977, PRN_04_03=6, SF055_04_03=3, SF056_04_03=1, SF060_04_03=13.920000000000016, SF061a_04_03=-1.568000000000005, SF061b_04_03=0.007999999999995566, PRN_04_04=9, SF055_04_04=4, SF056_04_04=1, SF060_04_04=21.24000000000001, SF061a_04_04=0.2079999999999984, SF061b_04_04=-0.1360000000000099, PRN_04_05=17, SF055_04_05=1, SF056_04_05=1, SF060_04_05=23.600000000000023, SF061a_04_05=-0.21600000000000819, SF061b_04_05=0.06399999999999295, PRN_04_06=31, SF055_04_06=2, SF056_04_06=1, SF060_04_06=16.439999999999998, SF061a_04_06=-1.4480000000000075, SF061b_04_06=-0.7360000000000042, SF031_05=14, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.008000000000000007, SF044_05=1, SF048_05=-0.18000000000000005, SF049a_05=-0.0050000000000000044, SF049b_05=0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF011_05=880836610, PRN_05_01=3, SF055_05_01=1, SF056_05_01=1, SF060_05_01=-2.0399999999999636, SF061a_05_01=-0.8000000000000114, SF061b_05_01=-0.4720000000000084, PRN_05_02=4, SF055_05_02=1, SF056_05_02=1, SF060_05_02=1.240000000000009, SF061a_05_02=-0.5600000000000023, SF061b_05_02=-0.3359999999999985, PRN_05_03=6, SF055_05_03=1, SF056_05_03=1, SF060_05_03=13.920000000000016, SF061a_05_03=-1.4879999999999995, SF061b_05_03=-0.04000000000000625, PRN_05_04=9, SF055_05_04=2, SF056_05_04=1, SF060_05_04=21.200000000000045, SF061a_05_04=0.35199999999998965, SF061b_05_04=0.09599999999998943, PRN_05_05=17, SF055_05_05=1, SF056_05_05=1, SF060_05_05=24.680000000000007, SF061a_05_05=-0.22400000000000375, SF061b_05_05=0.23999999999999488, PRN_05_06=31, SF055_05_06=2, SF056_05_06=1, SF060_05_06=11.640000000000043, SF061a_05_06=-1.3680000000000092, SF061b_05_06=-0.847999999999999, SF031_06=15, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.008000000000000007, SF044_06=1, SF048_06=-0.19999999999999996, SF049a_06=-0.0030000000000000027, SF049b_06=-0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF011_06=880836610, PRN_06_01=3, SF055_06_01=1, SF056_06_01=1, SF060_06_01=-5.079999999999984, SF061a_06_01=0.2879999999999967, SF061b_06_01=-0.5200000000000102, PRN_06_02=4, SF055_06_02=1, SF056_06_02=1, SF060_06_02=-1.0, SF061a_06_02=0.5039999999999907, SF061b_06_02=-0.4000000000000057, PRN_06_03=6, SF055_06_03=4, SF056_06_03=1, SF060_06_03=14.480000000000018, SF061a_06_03=-0.5919999999999987, SF061b_06_03=-0.04800000000000182, PRN_06_04=9, SF055_06_04=2, SF056_06_04=1, SF060_06_04=21.80000000000001, SF061a_06_04=1.3119999999999976, SF061b_06_04=0.06399999999999295, PRN_06_05=17, SF055_06_05=4, SF056_06_05=1, SF060_06_05=26.920000000000016, SF061a_06_05=0.887999999999991, SF061b_06_05=0.24799999999999045, PRN_06_06=31, SF055_06_06=1, SF056_06_06=1, SF060_06_06=6.0, SF061a_06_06=0.06399999999999295, SF061b_06_06=-0.8560000000000088, SF031_07=16, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.008000000000000007, SF044_07=1, SF048_07=-0.136, SF049a_07=0.01200000000000001, SF049b_07=-0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF011_07=880836610, PRN_07_01=3, SF055_07_01=1, SF056_07_01=1, SF060_07_01=10.640000000000043, SF061a_07_01=-0.3920000000000101, SF061b_07_01=-0.3680000000000092, PRN_07_02=4, SF055_07_02=1, SF056_07_02=1, SF060_07_02=10.840000000000032, SF061a_07_02=-0.0799999999999983, SF061b_07_02=-0.24800000000000466, PRN_07_03=6, SF055_07_03=1, SF056_07_03=1, SF060_07_03=18.319999999999993, SF061a_07_03=-1.1280000000000001, SF061b_07_03=0.22399999999998954, PRN_07_04=9, SF055_07_04=1, SF056_07_04=1, SF060_07_04=25.400000000000034, SF061a_07_04=0.32799999999998875, SF061b_07_04=-0.15200000000000102, PRN_07_05=17, SF055_07_05=1, SF056_07_05=1, SF060_07_05=26.04000000000002, SF061a_07_05=-0.07200000000000273, SF061b_07_05=0.015999999999991132, PRN_07_06=31, SF055_07_06=2, SF056_07_06=1, SF060_07_06=31.720000000000027, SF061a_07_06=-1.3359999999999985, SF061b_07_06=-0.9120000000000061, SF031_08=17, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.008000000000000007, SF044_08=1, SF048_08=-0.16400000000000003, SF049a_08=0.009000000000000008, SF049b_08=-0.006000000000000005, SF054_08=1, SatBitmaskLen_08=0, SF011_08=880836610, PRN_08_01=3, SF055_08_01=1, SF056_08_01=1, SF060_08_01=7.680000000000007, SF061a_08_01=-0.3760000000000048, SF061b_08_01=-0.48799999999999955, PRN_08_02=4, SF055_08_02=1, SF056_08_02=1, SF060_08_02=8.920000000000016, SF061a_08_02=0.007999999999995566, SF061b_08_02=-0.3440000000000083, PRN_08_03=6, SF055_08_03=2, SF056_08_03=1, SF060_08_03=20.480000000000018, SF061a_08_03=-1.1920000000000073, SF061b_08_03=0.367999999999995, PRN_08_04=9, SF055_08_04=1, SF056_08_04=1, SF060_08_04=24.680000000000007, SF061a_08_04=0.3359999999999985, SF061b_08_04=-0.07200000000000273, PRN_08_05=17, SF055_08_05=2, SF056_08_05=1, SF060_08_05=26.920000000000016, SF061a_08_05=0.07199999999998852, SF061b_08_05=0.21599999999999397, PRN_08_06=31, SF055_08_06=1, SF056_08_06=1, SF060_08_06=26.120000000000005, SF061a_08_06=-1.1280000000000001, SF061b_08_06=-0.8000000000000114, SF031_09=18, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.008000000000000007, SF044_09=1, SF048_09=-0.18000000000000005, SF049a_09=-0.010000000000000009, SF049b_09=-0.0020000000000000018, SF054_09=1, SatBitmaskLen_09=0, SF011_09=880836610, PRN_09_01=3, SF055_09_01=1, SF056_09_01=1, SF060_09_01=3.0400000000000205, SF061a_09_01=-0.21600000000000819, SF061b_09_01=-0.14400000000000546, PRN_09_02=4, SF055_09_02=2, SF056_09_02=1, SF060_09_02=5.28000000000003, SF061a_09_02=0.14399999999999125, SF061b_09_02=0.02400000000000091, PRN_09_03=6, SF055_09_03=4, SF056_09_03=1, SF060_09_03=20.08000000000004, SF061a_09_03=-1.3200000000000074, SF061b_09_03=0.5759999999999934, PRN_09_04=9, SF055_09_04=1, SF056_09_04=1, SF060_09_04=22.52000000000004, SF061a_09_04=0.6640000000000015, SF061b_09_04=0.2079999999999984, PRN_09_05=17, SF055_09_05=2, SF056_09_05=1, SF060_09_05=26.480000000000018, SF061a_09_05=0.30400000000000205, SF061b_09_05=0.45599999999998886, PRN_09_06=31, SF055_09_06=1, SF056_09_06=1, SF060_09_06=18.720000000000027, SF061a_09_06=-0.5280000000000058, SF061b_09_06=-0.5600000000000023, SF031_10=19, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=1, SF043_10=0.008000000000000007, SF044_10=1, SF048_10=-0.19599999999999995, SF049a_10=0.0, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF011_10=880836610, PRN_10_01=3, SF055_10_01=1, SF056_10_01=1, SF060_10_01=-5.439999999999998, SF061a_10_01=0.32799999999998875, SF061b_10_01=-0.5280000000000058, PRN_10_02=4, SF055_10_02=1, SF056_10_02=1, SF060_10_02=-2.0, SF061a_10_02=0.5279999999999916, SF061b_10_02=-0.3760000000000048, PRN_10_03=6, SF055_10_03=2, SF056_10_03=1, SF060_10_03=16.640000000000043, SF061a_10_03=-0.9759999999999991, SF061b_10_03=0.11199999999999477, PRN_10_04=9, SF055_10_04=1, SF056_10_04=1, SF060_10_04=18.04000000000002, SF061a_10_04=1.4639999999999986, SF061b_10_04=0.1039999999999992, PRN_10_05=17, SF055_10_05=1, SF056_10_05=1, SF060_10_05=23.960000000000036, SF061a_10_05=1.215999999999994, SF061b_10_05=0.2079999999999984, PRN_10_06=31, SF055_10_06=1, SF056_10_06=1, SF060_10_06=6.560000000000002, SF061a_10_06=0.06399999999999295, SF061b_10_06=-0.9280000000000115)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=478, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=32, authInd=1, embAuthLen=0, crc=114625, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=20, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=0.0, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836610, PRN_01_01=3, SF055_01_01=1, SF056_01_01=1, SF060_01_01=11.04000000000002, SF061a_01_01=-0.28000000000000114, SF061b_01_01=-0.4480000000000075, PRN_01_02=4, SF055_01_02=1, SF056_01_02=1, SF060_01_02=10.640000000000043, SF061a_01_02=0.007999999999995566, SF061b_01_02=-0.3200000000000074, PRN_01_03=6, SF055_01_03=2, SF056_01_03=1, SF060_01_03=21.840000000000032, SF061a_01_03=-1.2079999999999984, SF061b_01_03=0.2639999999999958, PRN_01_04=9, SF055_01_04=1, SF056_01_04=1, SF060_01_04=24.400000000000034, SF061a_01_04=0.30400000000000205, SF061b_01_04=-0.14400000000000546, PRN_01_05=17, SF055_01_05=1, SF056_01_05=1, SF060_01_05=26.120000000000005, SF061a_01_05=0.03999999999999204, SF061b_01_05=0.07199999999998852, PRN_01_06=31, SF055_01_06=1, SF056_01_06=1, SF060_01_06=33.879999999999995, SF061a_01_06=-1.152000000000001, SF061b_01_06=-0.9440000000000026, SF031_02=21, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=3, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.16800000000000004, SF049a_02=-0.006000000000000005, SF049b_02=-0.01100000000000001, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836610, PRN_02_01=3, SF055_02_01=1, SF056_02_01=1, SF060_02_01=8.28000000000003, SF061a_02_01=-0.35200000000000387, SF061b_02_01=-0.416000000000011, PRN_02_02=4, SF055_02_02=1, SF056_02_02=1, SF060_02_02=8.680000000000007, SF061a_02_02=-0.016000000000005343, SF061b_02_02=-0.3119999999999976, PRN_02_03=6, SF055_02_03=3, SF056_02_03=1, SF060_02_03=23.560000000000002, SF061a_02_03=-1.0160000000000053, SF061b_02_03=0.23199999999999932, PRN_02_04=9, SF055_02_04=1, SF056_02_04=1, SF060_02_04=23.840000000000032, SF061a_02_04=0.27199999999999136, SF061b_02_04=-0.02400000000000091, PRN_02_05=17, SF055_02_05=2, SF056_02_05=1, SF060_02_05=26.720000000000027, SF061a_02_05=0.03999999999999204, SF061b_02_05=0.21599999999999397, PRN_02_06=31, SF055_02_06=1, SF056_02_06=1, SF060_02_06=28.08000000000004, SF061a_02_06=-0.9120000000000061, SF061b_02_06=-0.9120000000000061, SF031_03=22, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.17600000000000005, SF049a_03=0.007000000000000006, SF049b_03=-0.0030000000000000027, SF054_03=1, SatBitmaskLen_03=0, SF011_03=880836610, PRN_03_01=3, SF055_03_01=1, SF056_03_01=1, SF060_03_01=3.7200000000000273, SF061a_03_01=-0.21600000000000819, SF061b_03_01=-0.17600000000000193, PRN_03_02=4, SF055_03_02=1, SF056_03_02=1, SF060_03_02=5.0, SF061a_03_02=0.09599999999998943, SF061b_03_02=0.0, PRN_03_03=6, SF055_03_03=1, SF056_03_03=1, SF060_03_03=22.600000000000023, SF061a_03_03=-1.3760000000000048, SF061b_03_03=0.6239999999999952, PRN_03_04=9, SF055_03_04=1, SF056_03_04=1, SF060_03_04=20.920000000000016, SF061a_03_04=0.5439999999999969, SF061b_03_04=0.09599999999998943, PRN_03_05=17, SF055_03_05=2, SF056_03_05=1, SF060_03_05=25.600000000000023, SF061a_03_05=0.17600000000000193, SF061b_03_05=0.32799999999998875, PRN_03_06=31, SF055_03_06=1, SF056_03_06=1, SF060_03_06=20.840000000000032, SF061a_03_06=-0.5760000000000076, SF061b_03_06=-0.6880000000000024, SF031_04=23, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.01200000000000001, SF044_04=1, SF048_04=-0.19599999999999995, SF049a_04=-0.01100000000000001, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF011_04=880836610, PRN_04_01=3, SF055_04_01=1, SF056_04_01=1, SF060_04_01=2.920000000000016, SF061a_04_01=-0.15200000000000102, SF061b_04_01=-0.08800000000000807, PRN_04_02=4, SF055_04_02=1, SF056_04_02=1, SF060_04_02=5.160000000000025, SF061a_04_02=0.1280000000000001, SF061b_04_02=0.07199999999998852, PRN_04_03=6, SF055_04_03=2, SF056_04_03=1, SF060_04_03=26.120000000000005, SF061a_04_03=-1.3440000000000083, SF061b_04_03=0.48799999999999955, PRN_04_04=9, SF055_04_04=1, SF056_04_04=1, SF060_04_04=21.760000000000048, SF061a_04_04=0.6559999999999917, SF061b_04_04=0.24799999999999045, PRN_04_05=17, SF055_04_05=2, SF056_04_05=1, SF060_04_05=27.840000000000032, SF061a_04_05=0.3919999999999959, SF061b_04_05=0.4719999999999942, PRN_04_06=31, SF055_04_06=2, SF056_04_06=1, SF060_04_06=17.24000000000001, SF061a_04_06=-0.43200000000000216, SF061b_04_06=-0.5919999999999987, SF031_05=24, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.01200000000000001, SF044_05=1, SF048_05=-0.19599999999999995, SF049a_05=-0.0030000000000000027, SF049b_05=-0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF011_05=880836610, PRN_05_01=3, SF055_05_01=1, SF056_05_01=1, SF060_05_01=-2.7999999999999545, SF061a_05_01=0.08799999999999386, SF061b_05_01=-0.2079999999999984, PRN_05_02=4, SF055_05_02=1, SF056_05_02=1, SF060_05_02=0.28000000000002956, SF061a_05_02=0.367999999999995, SF061b_05_02=-0.02400000000000091, PRN_05_03=6, SF055_05_03=1, SF056_05_03=1, SF060_05_03=23.319999999999993, SF061a_05_03=-0.7680000000000007, SF061b_05_03=0.4159999999999968, PRN_05_04=9, SF055_05_04=1, SF056_05_04=1, SF060_05_04=18.52000000000004, SF061a_05_04=0.9039999999999964, SF061b_05_04=0.43200000000000216, PRN_05_05=17, SF055_05_05=1, SF056_05_05=1, SF060_05_05=25.400000000000034, SF061a_05_05=0.8160000000000025, SF061b_05_05=0.6640000000000015, PRN_05_06=31, SF055_05_06=1, SF056_05_06=1, SF060_05_06=9.04000000000002, SF061a_05_06=-0.04000000000000625, SF061b_05_06=-0.7280000000000086, SF031_06=25, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.18400000000000005, SF049a_06=-0.006000000000000005, SF049b_06=0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF011_06=880836610, PRN_06_01=3, SF055_06_01=1, SF056_06_01=1, SF060_06_01=-3.9599999999999795, SF061a_06_01=-0.06400000000000716, SF061b_06_01=-0.1600000000000108, PRN_06_02=4, SF055_06_02=1, SF056_06_02=1, SF060_06_02=-0.3599999999999568, SF061a_06_02=0.1599999999999966, SF061b_06_02=-0.04800000000000182, PRN_06_03=6, SF055_06_03=2, SF056_06_03=1, SF060_06_03=26.400000000000034, SF061a_06_03=-0.9680000000000035, SF061b_06_03=0.3359999999999985, PRN_06_04=9, SF055_06_04=1, SF056_06_04=1, SF060_06_04=19.879999999999995, SF061a_06_04=0.6159999999999997, SF061b_06_04=0.40800000000000125, PRN_06_05=17, SF055_06_05=1, SF056_06_05=1, SF060_06_05=27.960000000000036, SF061a_06_05=0.9359999999999928, SF061b_06_05=0.6319999999999908, PRN_06_06=31, SF055_06_06=1, SF056_06_06=1, SF060_06_06=5.600000000000023, SF061a_06_06=-0.2560000000000002, SF061b_06_06=-0.5840000000000032, SF031_07=26, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=3, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.17200000000000004, SF049a_07=0.0010000000000000009, SF049b_07=-0.007000000000000006, SF054_07=1, SatBitmaskLen_07=0, SF011_07=880836610, PRN_07_01=3, SF055_07_01=1, SF056_07_01=1, SF060_07_01=10.760000000000048, SF061a_07_01=-0.15200000000000102, SF061b_07_01=-1.0720000000000027, PRN_07_02=4, SF055_07_02=1, SF056_07_02=1, SF060_07_02=7.840000000000032, SF061a_07_02=0.24799999999999045, SF061b_07_02=-0.8239999999999981, PRN_07_03=6, SF055_07_03=2, SF056_07_03=1, SF060_07_03=21.840000000000032, SF061a_07_03=-1.0, SF061b_07_03=-0.016000000000005343, PRN_07_04=9, SF055_07_04=1, SF056_07_04=1, SF060_07_04=18.80000000000001, SF061a_07_04=0.8559999999999945, SF061b_07_04=-0.4399999999999977, PRN_07_05=17, SF055_07_05=2, SF056_07_05=1, SF060_07_05=20.24000000000001, SF061a_07_05=0.6239999999999952, SF061b_07_05=-0.21600000000000819, PRN_07_06=31, SF055_07_06=2, SF056_07_06=1, SF060_07_06=39.31999999999999, SF061a_07_06=-0.5600000000000023, SF061b_07_06=-1.5600000000000023, SF031_08=27, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.016000000000000014, SF044_08=1, SF048_08=-0.19199999999999995, SF049a_08=0.0030000000000000027, SF049b_08=0.0050000000000000044, SF054_08=1, SatBitmaskLen_08=0, SF011_08=880836610, PRN_08_01=3, SF055_08_01=1, SF056_08_01=1, SF060_08_01=6.439999999999998, SF061a_08_01=0.24799999999999045, SF061b_08_01=-0.7439999999999998, PRN_08_02=4, SF055_08_02=2, SF056_08_02=1, SF060_08_02=5.160000000000025, SF061a_08_02=0.5279999999999916, SF061b_08_02=-0.5440000000000111, PRN_08_03=6, SF055_08_03=2, SF056_08_03=1, SF060_08_03=21.80000000000001, SF061a_08_03=-0.7280000000000086, SF061b_08_03=0.08799999999999386, PRN_08_04=9, SF055_08_04=1, SF056_08_04=1, SF060_08_04=18.160000000000025, SF061a_08_04=0.695999999999998, SF061b_08_04=-0.3680000000000092, PRN_08_05=17, SF055_08_05=2, SF056_08_05=1, SF060_08_05=21.0, SF061a_08_05=0.5999999999999943, SF061b_08_05=-0.11200000000000898, PRN_08_06=31, SF055_08_06=2, SF056_08_06=1, SF060_08_06=31.24000000000001, SF061a_08_06=-0.1280000000000001, SF061b_08_06=-1.3760000000000048, SF031_09=28, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.01200000000000001, SF044_09=1, SF048_09=-0.18799999999999994, SF049a_09=-0.008000000000000007, SF049b_09=0.0020000000000000018, SF054_09=1, SatBitmaskLen_09=0, SF011_09=880836610, PRN_09_01=3, SF055_09_01=1, SF056_09_01=1, SF060_09_01=3.840000000000032, SF061a_09_01=0.40800000000000125, SF061b_09_01=-0.5919999999999987, PRN_09_02=4, SF055_09_02=1, SF056_09_02=1, SF060_09_02=3.240000000000009, SF061a_09_02=0.6479999999999961, SF061b_09_02=-0.5120000000000005, PRN_09_03=6, SF055_09_03=2, SF056_09_03=1, SF060_09_03=22.160000000000025, SF061a_09_03=-0.40800000000000125, SF061b_09_03=-0.016000000000005343, PRN_09_04=9, SF055_09_04=2, SF056_09_04=1, SF060_09_04=17.319999999999993, SF061a_09_04=0.7999999999999972, SF061b_09_04=-0.1280000000000001, PRN_09_05=17, SF055_09_05=2, SF056_09_05=1, SF060_09_05=20.840000000000032, SF061a_09_05=0.6159999999999997, SF061b_09_05=-0.02400000000000091, PRN_09_06=31, SF055_09_06=1, SF056_09_06=1, SF060_09_06=25.840000000000032, SF061a_09_06=0.1039999999999992, SF061b_09_06=-1.2800000000000011, SF031_10=29, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=4, SF043_10=0.01200000000000001, SF044_10=1, SF048_10=-0.18799999999999994, SF049a_10=0.045999999999999985, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=0, SF011_10=880836610, PRN_10_01=3, SF055_10_01=2, SF056_10_01=1, SF060_10_01=3.920000000000016, SF061a_10_01=0.6400000000000006, SF061b_10_01=-0.6720000000000113, PRN_10_02=4, SF055_10_02=1, SF056_10_02=1, SF060_10_02=4.240000000000009, SF061a_10_02=0.9200000000000017, SF061b_10_02=-0.5280000000000058, PRN_10_03=6, SF055_10_03=1, SF056_10_03=1, SF060_10_03=25.200000000000045, SF061a_10_03=-0.6800000000000068, SF061b_10_03=0.19999999999998863, PRN_10_04=9, SF055_10_04=2, SF056_10_04=1, SF060_10_04=19.04000000000002, SF061a_10_04=1.0079999999999956, SF061b_10_04=-0.4399999999999977, PRN_10_05=17, SF055_10_05=2, SF056_10_05=1, SF060_10_05=24.24000000000001, SF061a_10_05=0.9519999999999982, SF061b_10_05=-0.3440000000000083, PRN_10_06=31, SF055_10_06=2, SF056_10_06=1, SF060_10_06=22.760000000000048, SF061a_10_06=0.40800000000000125, SF061b_10_06=-1.1839999999999975)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=472, eaf=1, crcType=2, frameCrc=6, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=33, authInd=1, embAuthLen=0, crc=8980777, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.18000000000000005, SF049a_01=-0.01200000000000001, SF049b_01=-0.006000000000000005, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836610, PRN_01_01=3, SF055_01_01=1, SF056_01_01=1, SF060_01_01=1.1200000000000045, SF061a_01_01=0.7519999999999953, SF061b_01_01=-0.695999999999998, PRN_01_02=4, SF055_01_02=1, SF056_01_02=1, SF060_01_02=2.2000000000000455, SF061a_01_02=0.8160000000000025, SF061b_01_02=-0.5760000000000076, PRN_01_03=6, SF055_01_03=4, SF056_01_03=1, SF060_01_03=25.400000000000034, SF061a_01_03=-0.12000000000000455, SF061b_01_03=-0.06400000000000716, PRN_01_04=9, SF055_01_04=2, SF056_01_04=1, SF060_01_04=17.480000000000018, SF061a_01_04=0.8079999999999927, SF061b_01_04=-0.4720000000000084, PRN_01_05=17, SF055_01_05=2, SF056_01_05=1, SF060_01_05=23.480000000000018, SF061a_01_05=0.8719999999999999, SF061b_01_05=-0.22400000000000375, PRN_01_06=31, SF055_01_06=2, SF056_01_06=1, SF060_01_06=17.439999999999998, SF061a_01_06=0.4399999999999977, SF061b_01_06=-1.2960000000000065, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.19599999999999995, SF049a_02=0.0050000000000000044, SF049b_02=0.0, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836610, PRN_02_01=3, SF055_02_01=2, SF056_02_01=1, SF060_02_01=-2.6399999999999864, SF061a_02_01=0.015999999999991132, SF061b_02_01=-0.15200000000000102, PRN_02_02=4, SF055_02_02=2, SF056_02_02=1, SF060_02_02=-0.39999999999997726, SF061a_02_02=0.1039999999999992, SF061b_02_02=0.04800000000000182, PRN_02_03=6, SF055_02_03=2, SF056_02_03=1, SF060_02_03=24.80000000000001, SF061a_02_03=-0.6880000000000024, SF061b_02_03=0.46399999999999864, PRN_02_04=9, SF055_02_04=1, SF056_02_04=1, SF060_02_04=16.160000000000025, SF061a_02_04=0.30400000000000205, SF061b_02_04=0.37599999999999056, PRN_02_05=17, SF055_02_05=2, SF056_02_05=1, SF060_02_05=22.760000000000048, SF061a_02_05=0.43200000000000216, SF061b_02_05=0.48799999999999955, PRN_02_06=31, SF055_02_06=2, SF056_02_06=1, SF060_02_06=10.439999999999998, SF061a_02_06=-0.1600000000000108, SF061b_02_06=-0.6480000000000103, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.016000000000000014, SF044_03=1, SF048_03=-0.18799999999999994, SF049a_03=-0.037000000000000005, SF049b_03=-0.006000000000000005, SF054_03=1, SatBitmaskLen_03=0, SF011_03=880836610, PRN_03_01=3, SF055_03_01=1, SF056_03_01=1, SF060_03_01=-3.919999999999959, SF061a_03_01=-0.12000000000000455, SF061b_03_01=-0.1600000000000108, PRN_03_02=4, SF055_03_02=1, SF056_03_02=1, SF060_03_02=-0.6800000000000068, SF061a_03_02=0.1599999999999966, SF061b_03_02=-0.016000000000005343, PRN_03_03=6, SF055_03_03=1, SF056_03_03=1, SF060_03_03=27.840000000000032, SF061a_03_03=-0.5200000000000102, SF061b_03_03=0.1839999999999975, PRN_03_04=9, SF055_03_04=1, SF056_03_04=1, SF060_03_04=18.760000000000048, SF061a_03_04=0.19199999999999307, SF061b_03_04=0.3119999999999976, PRN_03_05=17, SF055_03_05=2, SF056_03_05=1, SF060_03_05=27.08000000000004, SF061a_03_05=0.11999999999999034, SF061b_03_05=0.7920000000000016, PRN_03_06=31, SF055_03_06=1, SF056_03_06=1, SF060_03_06=5.8799999999999955, SF061a_03_06=-0.5600000000000023, SF061b_03_06=-0.632000000000005, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.128, SF049a_04=-0.013000000000000012, SF049b_04=0.0, SF054_04=1, SatBitmaskLen_04=0, SF011_04=880836608, PRN_04_01=3, SF055_04_01=1, SF056_04_01=1, SF060_04_01=11.120000000000005, SF061a_04_01=0.30400000000000205, SF061b_04_01=-1.3760000000000048, PRN_04_02=4, SF055_04_02=1, SF056_04_02=1, SF060_04_02=6.240000000000009, SF061a_04_02=0.5439999999999969, SF061b_04_02=-0.8400000000000034, PRN_04_03=6, SF055_04_03=2, SF056_04_03=1, SF060_04_03=25.0, SF061a_04_03=-0.5440000000000111, SF061b_04_03=-0.1360000000000099, PRN_04_04=9, SF055_04_04=3, SF056_04_04=1, SF060_04_04=15.600000000000023, SF061a_04_04=0.6640000000000015, SF061b_04_04=-0.38400000000000034, PRN_04_05=17, SF055_04_05=2, SF056_04_05=1, SF060_04_05=17.0, SF061a_04_05=0.8639999999999901, SF061b_04_05=-0.2560000000000002, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.14400000000000002, SF049a_05=-0.021999999999999992, SF049b_05=0.014000000000000012, SF054_05=1, SatBitmaskLen_05=0, SF011_05=880836610, PRN_05_01=3, SF055_05_01=2, SF056_05_01=1, SF060_05_01=4.560000000000002, SF061a_05_01=0.48799999999999955, SF061b_05_01=-0.9040000000000106, PRN_05_02=4, SF055_05_02=1, SF056_05_02=1, SF060_05_02=2.5200000000000387, SF061a_05_02=0.583999999999989, SF061b_05_02=-0.5600000000000023, PRN_05_03=6, SF055_05_03=3, SF056_05_03=1, SF060_05_03=24.960000000000036, SF061a_05_03=-0.632000000000005, SF061b_05_03=-0.09600000000000364, PRN_05_04=9, SF055_05_04=3, SF056_05_04=1, SF060_05_04=15.240000000000009, SF061a_05_04=0.4719999999999942, SF061b_05_04=-0.14400000000000546, PRN_05_05=17, SF055_05_05=3, SF056_05_05=1, SF060_05_05=17.760000000000048, SF061a_05_05=0.8399999999999892, SF061b_05_05=-0.016000000000005343, PRN_05_06=31, SF055_05_06=2, SF056_05_06=1, SF060_05_06=30.160000000000025, SF061a_05_06=0.3919999999999959, SF061b_05_06=-1.6880000000000024, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.016000000000000014, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0030000000000000027, SF049b_06=0.006000000000000005, SF054_06=1, SatBitmaskLen_06=0, SF011_06=880836610, PRN_06_01=3, SF055_06_01=1, SF056_06_01=1, SF060_06_01=-1.9599999999999795, SF061a_06_01=0.73599999999999, SF061b_06_01=-0.5760000000000076, PRN_06_02=4, SF055_06_02=1, SF056_06_02=1, SF060_06_02=-0.7599999999999909, SF061a_06_02=0.7199999999999989, SF061b_06_02=-0.4399999999999977, PRN_06_03=6, SF055_06_03=4, SF056_06_03=1, SF060_06_03=25.160000000000025, SF061a_06_03=-0.23199999999999932, SF061b_06_03=-0.2880000000000109, PRN_06_04=9, SF055_06_04=1, SF056_06_04=1, SF060_06_04=15.240000000000009, SF061a_06_04=0.30400000000000205, SF061b_06_04=-0.27200000000000557, PRN_06_05=17, SF055_06_05=1, SF056_06_05=1, SF060_06_05=21.480000000000018, SF061a_06_05=0.28000000000000114, SF061b_06_05=-0.11200000000000898, PRN_06_06=31, SF055_06_06=2, SF056_06_06=1, SF060_06_06=13.920000000000016, SF061a_06_06=0.7439999999999998, SF061b_06_06=-1.2000000000000028, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=4, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.15200000000000002, SF049a_07=-0.04500000000000001, SF049b_07=-0.015000000000000013, SF054_07=1, SatBitmaskLen_07=0, SF011_07=880836610, PRN_07_01=3, SF055_07_01=2, SF056_07_01=1, SF060_07_01=2.160000000000025, SF061a_07_01=-1.1680000000000064, SF061b_07_01=-0.1600000000000108, PRN_07_02=4, SF055_07_02=1, SF056_07_02=1, SF060_07_02=4.400000000000034, SF061a_07_02=-1.1039999999999992, SF061b_07_02=-0.02400000000000091, PRN_07_03=6, SF055_07_03=5, SF056_07_03=1, SF060_07_03=32.64000000000004, SF061a_07_03=-1.6000000000000014, SF061b_07_03=0.45599999999998886, PRN_07_04=9, SF055_07_04=4, SF056_07_04=1, SF060_07_04=22.120000000000005, SF061a_07_04=-1.720000000000006, SF061b_07_04=0.367999999999995, PRN_07_05=17, SF055_07_05=3, SF056_07_05=1, SF060_07_05=28.760000000000048, SF061a_07_05=-1.7360000000000042, SF061b_07_05=0.5679999999999978, PRN_07_06=31, SF055_07_06=1, SF056_07_06=1, SF060_07_06=14.480000000000018, SF061a_07_06=-1.3599999999999994, SF061b_07_06=-0.5280000000000058, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.016000000000000014, SF044_08=1, SF048_08=-0.16800000000000004, SF049a_08=-0.010000000000000009, SF049b_08=0.009000000000000008, SF054_08=1, SatBitmaskLen_08=0, SF011_08=880836610, PRN_08_01=3, SF055_08_01=1, SF056_08_01=1, SF060_08_01=1.080000000000041, SF061a_08_01=-1.3119999999999976, SF061b_08_01=-0.2960000000000065, PRN_08_02=4, SF055_08_02=1, SF056_08_02=1, SF060_08_02=3.8799999999999955, SF061a_08_02=-1.112000000000009, SF061b_08_02=-0.14400000000000546, PRN_08_03=6, SF055_08_03=4, SF056_08_03=1, SF060_08_03=34.28000000000003, SF061a_08_03=-2.2960000000000065, SF061b_08_03=-0.008000000000009777, PRN_08_04=9, SF055_08_04=1, SF056_08_04=1, SF060_08_04=23.28000000000003, SF061a_08_04=-1.5200000000000102, SF061b_08_04=0.1599999999999966, PRN_08_05=17, SF055_08_05=1, SF056_08_05=1, SF060_08_05=31.319999999999993, SF061a_08_05=-1.4320000000000022, SF061b_08_05=0.5279999999999916, PRN_08_06=31, SF055_08_06=1, SF056_08_06=1, SF060_08_06=11.560000000000002, SF061a_08_06=-1.5200000000000102, SF061b_08_06=-0.6880000000000024, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.15600000000000003, SF049a_09=0.0010000000000000009, SF049b_09=-0.0010000000000000009, SF054_09=1, SatBitmaskLen_09=0, SF011_09=880836610, PRN_09_01=3, SF055_09_01=2, SF056_09_01=1, SF060_09_01=-5.319999999999993, SF061a_09_01=1.0159999999999911, SF061b_09_01=-0.7199999999999989, PRN_09_02=4, SF055_09_02=2, SF056_09_02=1, SF060_09_02=-3.680000000000007, SF061a_09_02=0.8319999999999936, SF061b_09_02=-0.5040000000000049, PRN_09_03=6, SF055_09_03=5, SF056_09_03=1, SF060_09_03=22.640000000000043, SF061a_09_03=1.3999999999999915, SF061b_09_03=-0.19200000000000728, PRN_09_04=9, SF055_09_04=2, SF056_09_04=1, SF060_09_04=15.560000000000002, SF061a_09_04=-0.5040000000000049, SF061b_09_04=-0.30400000000000205, PRN_09_05=17, SF055_09_05=2, SF056_09_05=1, SF060_09_05=21.560000000000002, SF061a_09_05=-0.3760000000000048, SF061b_09_05=0.015999999999991132, PRN_09_06=31, SF055_09_06=2, SF056_09_06=1, SF060_09_06=9.680000000000007, SF061a_09_06=1.1039999999999992, SF061b_09_06=-1.152000000000001, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=4, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.14400000000000002, SF049a_10=0.04999999999999999, SF049b_10=-0.038000000000000006, SF054_10=1, SatBitmaskLen_10=0, SF011_10=880836610, PRN_10_01=3, SF055_10_01=1, SF056_10_01=1, SF060_10_01=6.080000000000041, SF061a_10_01=-1.1440000000000055, SF061b_10_01=-0.30400000000000205, PRN_10_02=4, SF055_10_02=1, SF056_10_02=1, SF060_10_02=8.680000000000007, SF061a_10_02=-1.328000000000003, SF061b_10_02=-0.23199999999999932, PRN_10_03=6, SF055_10_03=1, SF056_10_03=1, SF060_10_03=36.52000000000004, SF061a_10_03=-0.3359999999999985, SF061b_10_03=0.15200000000000102, PRN_10_04=9, SF055_10_04=2, SF056_10_04=1, SF060_10_04=31.08000000000004, SF061a_10_04=-3.2080000000000055, SF061b_10_04=0.1599999999999966, PRN_10_05=17, SF055_10_05=2, SF056_10_05=1, SF060_10_05=37.44, SF061a_10_05=-2.872000000000007, SF061b_10_05=0.2079999999999984, PRN_10_06=31, SF055_10_06=1, SF056_10_06=1, SF060_10_06=18.52000000000004, SF061a_10_06=-1.1839999999999975, SF061b_10_06=-0.632000000000005)>",
+            "<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=98, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=34, authInd=1, embAuthLen=0, crc=7396141, SF005=152, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.17600000000000005, SF049a_01=-0.017999999999999988, SF049b_01=0.0020000000000000018, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836610, PRN_01_01=3, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-10.439999999999998, SF061a_01_01=0.9679999999999893, SF061b_01_01=-0.07200000000000273, PRN_01_02=4, SF055_01_02=1, SF056_01_02=1, SF060_01_02=-6.279999999999973, SF061a_01_02=1.2079999999999984, SF061b_01_02=0.055999999999997385, PRN_01_03=6, SF055_01_03=3, SF056_01_03=1, SF060_01_03=17.28000000000003, SF061a_01_03=0.4239999999999924, SF061b_01_03=0.3439999999999941, PRN_01_04=9, SF055_01_04=2, SF056_01_04=1, SF060_01_04=15.640000000000043, SF061a_01_04=1.9839999999999947, SF061b_01_04=0.5279999999999916, PRN_01_05=17, SF055_01_05=1, SF056_01_05=1, SF060_01_05=24.319999999999993, SF061a_01_05=1.8559999999999945, SF061b_01_05=0.8079999999999927, PRN_01_06=31, SF055_01_06=1, SF056_01_06=1, SF060_01_06=-1.3199999999999932, SF061a_01_06=0.8160000000000025, SF061b_01_06=-0.45600000000000307, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.18799999999999994, SF049a_02=0.0010000000000000009, SF049b_02=0.0030000000000000027, SF054_02=1, SatBitmaskLen_02=0, SF011_02=880836610, PRN_02_01=3, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-8.359999999999957, SF061a_02_01=0.9440000000000026, SF061b_02_01=-0.07200000000000273, PRN_02_02=4, SF055_02_02=1, SF056_02_02=1, SF060_02_02=-3.599999999999966, SF061a_02_02=1.1359999999999957, SF061b_02_02=0.055999999999997385, PRN_02_03=6, SF055_02_03=4, SF056_02_03=1, SF060_02_03=16.920000000000016, SF061a_02_03=-0.960000000000008, SF061b_02_03=0.5120000000000005, PRN_02_04=9, SF055_02_04=1, SF056_02_04=1, SF060_02_04=20.480000000000018, SF061a_02_04=2.0319999999999965, SF061b_02_04=0.43200000000000216, PRN_02_05=17, SF055_02_05=4, SF056_02_05=1, SF060_02_05=28.80000000000001, SF061a_02_05=1.5600000000000023, SF061b_02_05=0.8160000000000025, PRN_02_06=31, SF055_02_06=1, SF056_02_06=1, SF060_02_06=0.28000000000002956, SF061a_02_06=0.9200000000000017, SF061b_02_06=-0.46399999999999864)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=421, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=57, authInd=1, embAuthLen=0, crc=15138586, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF012_01=2627632, PRN_01_01=3, SF055_01_01=3, SF056_01_01=1, SF060_01_01=-18.519999999999982, SF061a_01_01=0.43200000000000216, SF061b_01_01=-0.3440000000000083, PRN_01_02=5, SF055_01_02=4, SF056_01_02=1, SF060_01_02=4.28000000000003, SF061a_01_02=-0.2400000000000091, SF061b_01_02=0.2560000000000002, PRN_01_03=12, SF055_01_03=3, SF056_01_03=1, SF060_01_03=-7.1200000000000045, SF061a_01_03=0.3919999999999959, SF061b_01_03=-0.24800000000000466, PRN_01_04=13, SF055_01_04=4, SF056_01_04=1, SF060_01_04=-19.71999999999997, SF061a_01_04=-1.1200000000000045, SF061b_01_04=-0.38400000000000034, PRN_01_05=19, SF055_01_05=4, SF056_01_05=1, SF060_01_05=-3.0399999999999636, SF061a_01_05=0.0799999999999983, SF061b_01_05=-0.016000000000005343, PRN_01_06=20, SF055_01_06=4, SF056_01_06=1, SF060_01_06=-15.279999999999973, SF061a_01_06=-0.9519999999999982, SF061b_01_06=-0.07200000000000273, SF031_02=1, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.0, SF044_02=1, SF048_02=-0.21199999999999997, SF049a_02=-0.0020000000000000018, SF049b_02=0.0, SF054_02=1, SatBitmaskLen_02=0, SF012_02=2627632, PRN_02_01=3, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-15.079999999999984, SF061a_02_01=-1.6000000000000014, SF061b_02_01=-0.2560000000000002, PRN_02_02=5, SF055_02_02=5, SF056_02_02=1, SF060_02_02=3.7600000000000477, SF061a_02_02=-0.1280000000000001, SF061b_02_02=0.07199999999998852, PRN_02_03=12, SF055_02_03=4, SF056_02_03=1, SF060_02_03=-6.359999999999957, SF061a_02_03=0.015999999999991132, SF061b_02_03=-0.27200000000000557, PRN_02_04=13, SF055_02_04=4, SF056_02_04=1, SF060_02_04=-10.560000000000002, SF061a_02_04=-2.6240000000000023, SF061b_02_04=-0.5600000000000023, PRN_02_05=19, SF055_02_05=3, SF056_02_05=1, SF060_02_05=-3.759999999999991, SF061a_02_05=0.5039999999999907, SF061b_02_05=-0.0799999999999983, PRN_02_06=20, SF055_02_06=3, SF056_02_06=1, SF060_02_06=-12.120000000000005, SF061a_02_06=-0.7280000000000086, SF061b_02_06=-0.055999999999997385, SF031_03=2, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=1, SF043_03=0.0, SF044_03=1, SF048_03=-0.21599999999999997, SF049a_03=0.0030000000000000027, SF049b_03=-0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF012_03=2627632, PRN_03_01=3, SF055_03_01=3, SF056_03_01=1, SF060_03_01=-17.680000000000007, SF061a_03_01=-1.8400000000000034, SF061b_03_01=-0.38400000000000034, PRN_03_02=5, SF055_03_02=2, SF056_03_02=1, SF060_03_02=6.2000000000000455, SF061a_03_02=-0.1360000000000099, SF061b_03_02=0.367999999999995, PRN_03_03=12, SF055_03_03=2, SF056_03_03=1, SF060_03_03=-9.239999999999952, SF061a_03_03=0.3999999999999915, SF061b_03_03=-0.38400000000000034, PRN_03_04=13, SF055_03_04=5, SF056_03_04=1, SF060_03_04=-14.319999999999993, SF061a_03_04=-2.720000000000006, SF061b_03_04=-0.4480000000000075, PRN_03_05=19, SF055_03_05=2, SF056_03_05=1, SF060_03_05=-4.239999999999952, SF061a_03_05=0.6319999999999908, SF061b_03_05=0.007999999999995566, PRN_03_06=20, SF055_03_06=2, SF056_03_06=1, SF060_03_06=-12.599999999999966, SF061a_03_06=-1.024000000000001, SF061b_03_06=-0.08800000000000807, SF031_04=3, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.0, SF044_04=1, SF048_04=-0.20799999999999996, SF049a_04=-0.0020000000000000018, SF049b_04=0.0, SF054_04=1, SatBitmaskLen_04=0, SF012_04=2101280, PRN_04_01=3, SF055_04_01=2, SF056_04_01=1, SF060_04_01=-10.71999999999997, SF061a_04_01=-0.16800000000000637, SF061b_04_01=-0.1280000000000001, PRN_04_02=12, SF055_04_02=2, SF056_04_02=1, SF060_04_02=-3.359999999999957, SF061a_04_02=-0.7040000000000077, SF061b_04_02=-0.06400000000000716, PRN_04_03=19, SF055_04_03=3, SF056_04_03=1, SF060_04_03=-3.7999999999999545, SF061a_04_03=0.6559999999999917, SF061b_04_03=-0.008000000000009777, SF031_05=4, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.0, SF044_05=1, SF048_05=-0.20799999999999996, SF049a_05=-0.0030000000000000027, SF049b_05=0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF012_05=2103328, PRN_05_01=3, SF055_05_01=1, SF056_05_01=1, SF060_05_01=-12.799999999999955, SF061a_05_01=0.02400000000000091, SF061b_05_01=-0.09600000000000364, PRN_05_02=12, SF055_05_02=3, SF056_05_02=1, SF060_05_02=-5.1200000000000045, SF061a_05_02=-1.112000000000009, SF061b_05_02=-0.1600000000000108, PRN_05_03=13, SF055_05_03=1, SF056_05_03=1, SF060_05_03=-9.839999999999975, SF061a_05_03=0.29599999999999227, SF061b_05_03=-0.3359999999999985, PRN_05_04=19, SF055_05_04=3, SF056_05_04=1, SF060_05_04=-3.8799999999999955, SF061a_05_04=0.7680000000000007, SF061b_05_04=0.07199999999998852, SF031_06=5, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.0, SF044_06=1, SF048_06=-0.18400000000000005, SF049a_06=-0.007000000000000006, SF049b_06=-0.0040000000000000036, SF054_06=1, SatBitmaskLen_06=0, SF012_06=528432, PRN_06_01=5, SF055_06_01=2, SF056_06_01=1, SF060_06_01=3.3600000000000136, SF061a_06_01=-0.21600000000000819, SF061b_06_01=-0.4399999999999977, PRN_06_02=12, SF055_06_02=3, SF056_06_02=1, SF060_06_02=4.600000000000023, SF061a_06_02=-0.6000000000000085, SF061b_06_02=-0.23199999999999932, PRN_06_03=19, SF055_06_03=4, SF056_06_03=1, SF060_06_03=-2.0399999999999636, SF061a_06_03=1.0719999999999885, SF061b_06_03=-0.0799999999999983, PRN_06_04=20, SF055_06_04=4, SF056_06_04=1, SF060_06_04=-6.919999999999959, SF061a_06_04=0.29599999999999227, SF061b_06_04=0.4159999999999968, SF031_07=6, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.0040000000000000036, SF044_07=1, SF048_07=-0.19599999999999995, SF049a_07=-0.0020000000000000018, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF012_07=528432, PRN_07_01=5, SF055_07_01=3, SF056_07_01=1, SF060_07_01=5.8799999999999955, SF061a_07_01=0.5039999999999907, SF061b_07_01=0.3999999999999915, PRN_07_02=12, SF055_07_02=4, SF056_07_02=1, SF060_07_02=2.080000000000041, SF061a_07_02=-0.7280000000000086, SF061b_07_02=-0.35200000000000387, PRN_07_03=19, SF055_07_03=4, SF056_07_03=1, SF060_07_03=-3.2799999999999727, SF061a_07_03=1.1679999999999922, SF061b_07_03=-0.11200000000000898, PRN_07_04=20, SF055_07_04=4, SF056_07_04=1, SF060_07_04=-6.680000000000007, SF061a_07_04=0.4719999999999942, SF061b_07_04=0.031999999999996476, SF031_08=7, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.0, SF044_08=1, SF048_08=-0.20399999999999996, SF049a_08=-0.0050000000000000044, SF049b_08=-0.0010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF012_08=3676208, PRN_08_01=3, SF055_08_01=3, SF056_08_01=1, SF060_08_01=-5.9599999999999795, SF061a_08_01=-0.3200000000000074, SF061b_08_01=-0.38400000000000034, PRN_08_02=4, SF055_08_02=3, SF056_08_02=1, SF060_08_02=-11.279999999999973, SF061a_08_02=-0.480000000000004, SF061b_08_02=0.0, PRN_08_03=5, SF055_08_03=4, SF056_08_03=1, SF060_08_03=14.920000000000016, SF061a_08_03=-0.5280000000000058, SF061b_08_03=0.40800000000000125, PRN_08_04=12, SF055_08_04=2, SF056_08_04=1, SF060_08_04=5.480000000000018, SF061a_08_04=-1.4320000000000022, SF061b_08_04=-0.2560000000000002, PRN_08_05=13, SF055_08_05=5, SF056_08_05=1, SF060_08_05=-2.1200000000000045, SF061a_08_05=-0.9040000000000106, SF061b_08_05=-0.28000000000000114, PRN_08_06=19, SF055_08_06=1, SF056_08_06=1, SF060_08_06=1.240000000000009, SF061a_08_06=-0.4399999999999977, SF061b_08_06=0.17600000000000193, PRN_08_07=20, SF055_08_07=3, SF056_08_07=1, SF060_08_07=-0.7599999999999909, SF061a_08_07=-0.847999999999999, SF061b_08_07=0.13599999999999568, SF031_09=8, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.0040000000000000036, SF044_09=1, SF048_09=-0.14400000000000002, SF049a_09=-0.009000000000000008, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF012_09=3674160, PRN_09_01=3, SF055_09_01=3, SF056_09_01=1, SF060_09_01=17.360000000000014, SF061a_09_01=-1.656000000000006, SF061b_09_01=0.1599999999999966, PRN_09_02=4, SF055_09_02=2, SF056_09_02=1, SF060_09_02=1.6000000000000227, SF061a_09_02=-0.8640000000000043, SF061b_09_02=0.6640000000000015, PRN_09_03=5, SF055_09_03=3, SF056_09_03=1, SF060_09_03=15.920000000000016, SF061a_09_03=-0.5760000000000076, SF061b_09_03=0.6159999999999997, PRN_09_04=12, SF055_09_04=2, SF056_09_04=1, SF060_09_04=27.400000000000034, SF061a_09_04=-1.8160000000000025, SF061b_09_04=0.3359999999999985, PRN_09_05=19, SF055_09_05=1, SF056_09_05=1, SF060_09_05=14.840000000000032, SF061a_09_05=-0.3200000000000074, SF061b_09_05=0.4959999999999951, PRN_09_06=20, SF055_09_06=3, SF056_09_06=1, SF060_09_06=8.840000000000032, SF061a_09_06=-0.7520000000000095, SF061b_09_06=0.519999999999996, SF031_10=9, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.0040000000000000036, SF044_10=1, SF048_10=-0.18799999999999994, SF049a_10=-0.0020000000000000018, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF012_10=3674160, PRN_10_01=3, SF055_10_01=2, SF056_10_01=1, SF060_10_01=3.4399999999999977, SF061a_10_01=-1.2160000000000082, SF061b_10_01=-0.6080000000000041, PRN_10_02=4, SF055_10_02=2, SF056_10_02=1, SF060_10_02=-6.71999999999997, SF061a_10_02=-0.8080000000000069, SF061b_10_02=-0.2079999999999984, PRN_10_03=5, SF055_10_03=3, SF056_10_03=1, SF060_10_03=14.0, SF061a_10_03=-0.8320000000000078, SF061b_10_03=0.15200000000000102, PRN_10_04=12, SF055_10_04=4, SF056_10_04=1, SF060_10_04=16.52000000000004, SF061a_10_04=-1.6000000000000014, SF061b_10_04=-0.4960000000000093, PRN_10_05=19, SF055_10_05=2, SF056_10_05=1, SF060_10_05=3.920000000000016, SF061a_10_05=-0.3760000000000048, SF061b_10_05=-0.21600000000000819, PRN_10_06=20, SF055_10_06=3, SF056_10_06=1, SF060_10_06=3.240000000000009, SF061a_10_06=-1.26400000000001, SF061b_10_06=-0.06400000000000716)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=456, eaf=1, crcType=2, frameCrc=2, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=58, authInd=1, embAuthLen=0, crc=14979022, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=10, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0040000000000000036, SF044_01=1, SF048_01=-0.19199999999999995, SF049a_01=-0.0030000000000000027, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF012_01=3676208, PRN_01_01=3, SF055_01_01=3, SF056_01_01=1, SF060_01_01=-2.4399999999999977, SF061a_01_01=-1.1839999999999975, SF061b_01_01=-0.3680000000000092, PRN_01_02=4, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-9.319999999999993, SF061a_01_02=-0.6080000000000041, SF061b_01_02=0.09599999999998943, PRN_01_03=5, SF055_01_03=3, SF056_01_03=1, SF060_01_03=16.439999999999998, SF061a_01_03=-0.5919999999999987, SF061b_01_03=0.4959999999999951, PRN_01_04=12, SF055_01_04=3, SF056_01_04=1, SF060_01_04=11.080000000000041, SF061a_01_04=-1.3840000000000003, SF061b_01_04=-0.38400000000000034, PRN_01_05=13, SF055_01_05=5, SF056_01_05=1, SF060_01_05=2.2800000000000296, SF061a_01_05=-1.4720000000000084, SF061b_01_05=-0.3359999999999985, PRN_01_06=19, SF055_01_06=2, SF056_01_06=1, SF060_01_06=1.6000000000000227, SF061a_01_06=0.007999999999995566, SF061b_01_06=0.11199999999999477, PRN_01_07=20, SF055_01_07=4, SF056_01_07=1, SF060_01_07=1.9600000000000364, SF061a_01_07=-0.8239999999999981, SF061b_01_07=0.09599999999998943, SF031_02=11, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.09999999999999998, SF049a_02=-0.0050000000000000044, SF049b_02=-0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=0, SF012_02=3670064, PRN_02_01=3, SF055_02_01=2, SF056_02_01=1, SF060_02_01=23.840000000000032, SF061a_02_01=-1.7600000000000051, SF061b_02_01=0.17600000000000193, PRN_02_02=4, SF055_02_02=2, SF056_02_02=1, SF060_02_02=2.5600000000000023, SF061a_02_02=-0.8400000000000034, SF061b_02_02=0.7199999999999989, PRN_02_03=5, SF055_02_03=3, SF056_02_03=1, SF060_02_03=15.920000000000016, SF061a_02_03=-0.6159999999999997, SF061b_02_03=0.7920000000000016, PRN_02_04=19, SF055_02_04=2, SF056_02_04=1, SF060_02_04=14.640000000000043, SF061a_02_04=-0.2880000000000109, SF061b_02_04=0.37599999999999056, PRN_02_05=20, SF055_02_05=3, SF056_02_05=1, SF060_02_05=10.04000000000002, SF061a_02_05=-0.8400000000000034, SF061b_02_05=0.6640000000000015, SF031_03=12, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.008000000000000007, SF044_03=1, SF048_03=-0.10799999999999998, SF049a_03=-0.01100000000000001, SF049b_03=-0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF012_03=3670064, PRN_03_01=3, SF055_03_01=4, SF056_03_01=1, SF060_03_01=25.360000000000014, SF061a_03_01=-1.7520000000000024, SF061b_03_01=0.15200000000000102, PRN_03_02=4, SF055_03_02=1, SF056_03_02=1, SF060_03_02=7.520000000000039, SF061a_03_02=-0.7199999999999989, SF061b_03_02=0.671999999999997, PRN_03_03=5, SF055_03_03=1, SF056_03_03=1, SF060_03_03=21.680000000000007, SF061a_03_03=-0.7680000000000007, SF061b_03_03=0.8639999999999901, PRN_03_04=19, SF055_03_04=1, SF056_03_04=1, SF060_03_04=17.600000000000023, SF061a_03_04=-0.1600000000000108, SF061b_03_04=0.4399999999999977, PRN_03_05=20, SF055_03_05=1, SF056_03_05=1, SF060_03_05=15.360000000000014, SF061a_03_05=-1.112000000000009, SF061b_03_05=0.8639999999999901, SF031_04=13, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=2, SF043_04=0.008000000000000007, SF044_04=1, SF048_04=-0.18000000000000005, SF049a_04=-0.006000000000000005, SF049b_04=-0.0030000000000000027, SF054_04=1, SatBitmaskLen_04=0, SF012_04=3674160, PRN_04_01=3, SF055_04_01=1, SF056_04_01=1, SF060_04_01=11.800000000000011, SF061a_04_01=-1.7680000000000078, SF061b_04_01=-0.7360000000000042, PRN_04_02=4, SF055_04_02=2, SF056_04_02=1, SF060_04_02=-2.519999999999982, SF061a_04_02=-1.024000000000001, SF061b_04_02=-0.3200000000000074, PRN_04_03=5, SF055_04_03=2, SF056_04_03=1, SF060_04_03=15.120000000000005, SF061a_04_03=-0.6000000000000085, SF061b_04_03=0.1280000000000001, PRN_04_04=12, SF055_04_04=5, SF056_04_04=1, SF060_04_04=25.160000000000025, SF061a_04_04=-2.064000000000007, SF061b_04_04=-0.4720000000000084, PRN_04_05=19, SF055_04_05=1, SF056_04_05=1, SF060_04_05=6.319999999999993, SF061a_04_05=-0.32800000000000296, SF061b_04_05=-0.2560000000000002, PRN_04_06=20, SF055_04_06=1, SF056_04_06=1, SF060_04_06=7.720000000000027, SF061a_04_06=-1.240000000000009, SF061b_04_06=-0.0799999999999983, SF031_05=14, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.008000000000000007, SF044_05=1, SF048_05=-0.18000000000000005, SF049a_05=-0.0050000000000000044, SF049b_05=0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF012_05=3674160, PRN_05_01=3, SF055_05_01=1, SF056_05_01=1, SF060_05_01=8.04000000000002, SF061a_05_01=-1.6880000000000024, SF061b_05_01=-0.6640000000000015, PRN_05_02=4, SF055_05_02=1, SF056_05_02=1, SF060_05_02=-4.0, SF061a_05_02=-0.8719999999999999, SF061b_05_02=-0.40800000000000125, PRN_05_03=5, SF055_05_03=3, SF056_05_03=1, SF060_05_03=16.760000000000048, SF061a_05_03=-0.6000000000000085, SF061b_05_03=0.29599999999999227, PRN_05_04=12, SF055_05_04=1, SF056_05_04=1, SF060_05_04=23.80000000000001, SF061a_05_04=-2.7520000000000024, SF061b_05_04=-0.5280000000000058, PRN_05_05=19, SF055_05_05=2, SF056_05_05=1, SF060_05_05=4.760000000000048, SF061a_05_05=-0.24800000000000466, SF061b_05_05=-0.3440000000000083, PRN_05_06=20, SF055_05_06=3, SF056_05_06=1, SF060_05_06=7.439999999999998, SF061a_05_06=-1.3920000000000101, SF061b_05_06=-0.08800000000000807, SF031_06=15, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.008000000000000007, SF044_06=1, SF048_06=-0.19999999999999996, SF049a_06=-0.0030000000000000027, SF049b_06=-0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF012_06=3674160, PRN_06_01=3, SF055_06_01=2, SF056_06_01=1, SF060_06_01=5.0400000000000205, SF061a_06_01=-0.9840000000000089, SF061b_06_01=-0.2400000000000091, PRN_06_02=4, SF055_06_02=2, SF056_06_02=1, SF060_06_02=-4.479999999999961, SF061a_06_02=-0.3920000000000101, SF061b_06_02=0.16799999999999216, PRN_06_03=5, SF055_06_03=3, SF056_06_03=1, SF060_06_03=19.600000000000023, SF061a_06_03=-0.1600000000000108, SF061b_06_03=0.7279999999999944, PRN_06_04=12, SF055_06_04=4, SF056_06_04=1, SF060_06_04=19.439999999999998, SF061a_06_04=-1.416000000000011, SF061b_06_04=-0.2400000000000091, PRN_06_05=19, SF055_06_05=2, SF056_06_05=1, SF060_06_05=4.360000000000014, SF061a_06_05=0.2879999999999967, SF061b_06_05=0.14399999999999125, PRN_06_06=20, SF055_06_06=2, SF056_06_06=1, SF060_06_06=7.920000000000016, SF061a_06_06=-0.8080000000000069, SF061b_06_06=0.19199999999999307, SF031_07=16, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.008000000000000007, SF044_07=1, SF048_07=-0.136, SF049a_07=0.01200000000000001, SF049b_07=-0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF012_07=3670064, PRN_07_01=3, SF055_07_01=2, SF056_07_01=1, SF060_07_01=25.439999999999998, SF061a_07_01=-1.088000000000008, SF061b_07_01=-0.960000000000008, PRN_07_02=4, SF055_07_02=1, SF056_07_02=1, SF060_07_02=3.8799999999999955, SF061a_07_02=-0.2880000000000109, SF061b_07_02=-0.2400000000000091, PRN_07_03=5, SF055_07_03=2, SF056_07_03=1, SF060_07_03=17.400000000000034, SF061a_07_03=-0.008000000000009777, SF061b_07_03=-0.11200000000000898, PRN_07_04=19, SF055_07_04=1, SF056_07_04=1, SF060_07_04=12.319999999999993, SF061a_07_04=0.4239999999999924, SF061b_07_04=-0.5200000000000102, PRN_07_05=20, SF055_07_05=1, SF056_07_05=1, SF060_07_05=12.480000000000018, SF061a_07_05=-0.695999999999998, SF061b_07_05=0.015999999999991132, SF031_08=17, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.008000000000000007, SF044_08=1, SF048_08=-0.16400000000000003, SF049a_08=0.009000000000000008, SF049b_08=-0.006000000000000005, SF054_08=1, SatBitmaskLen_08=0, SF012_08=3670064, PRN_08_01=3, SF055_08_01=2, SF056_08_01=1, SF060_08_01=19.879999999999995, SF061a_08_01=-1.2560000000000002, SF061b_08_01=-0.6640000000000015, PRN_08_02=4, SF055_08_02=1, SF056_08_02=1, SF060_08_02=2.2000000000000455, SF061a_08_02=-0.2560000000000002, SF061b_08_02=-0.2960000000000065, PRN_08_03=5, SF055_08_03=2, SF056_08_03=1, SF060_08_03=17.560000000000002, SF061a_08_03=0.0, SF061b_08_03=0.11999999999999034, PRN_08_04=19, SF055_08_04=1, SF056_08_04=1, SF060_08_04=9.240000000000009, SF061a_08_04=0.35199999999998965, SF061b_08_04=-0.4399999999999977, PRN_08_05=20, SF055_08_05=1, SF056_08_05=1, SF060_08_05=12.560000000000002, SF061a_08_05=-0.7680000000000007, SF061b_08_05=-0.008000000000009777, SF031_09=18, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.008000000000000007, SF044_09=1, SF048_09=-0.18000000000000005, SF049a_09=-0.010000000000000009, SF049b_09=-0.0020000000000000018, SF054_09=1, SatBitmaskLen_09=0, SF012_09=3670128, PRN_09_01=3, SF055_09_01=4, SF056_09_01=1, SF060_09_01=22.439999999999998, SF061a_09_01=-0.7360000000000042, SF061b_09_01=-0.7199999999999989, PRN_09_02=4, SF055_09_02=3, SF056_09_02=1, SF060_09_02=7.680000000000007, SF061a_09_02=0.04800000000000182, SF061b_09_02=-0.35999999999999943, PRN_09_03=5, SF055_09_03=3, SF056_09_03=1, SF060_09_03=25.80000000000001, SF061a_09_03=0.2879999999999967, SF061b_09_03=0.1280000000000001, PRN_09_04=18, SF055_09_04=3, SF056_09_04=1, SF060_09_04=47.200000000000045, SF061a_09_04=0.8319999999999936, SF061b_09_04=-1.240000000000009, PRN_09_05=19, SF055_09_05=1, SF056_09_05=1, SF060_09_05=14.640000000000043, SF061a_09_05=1.0319999999999965, SF061b_09_05=-0.46399999999999864, PRN_09_06=20, SF055_09_06=4, SF056_09_06=1, SF060_09_06=20.0, SF061a_09_06=-0.22400000000000375, SF061b_09_06=-0.1839999999999975, SF031_10=19, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=1, SF043_10=0.008000000000000007, SF044_10=1, SF048_10=-0.19599999999999995, SF049a_10=0.0, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF012_10=3674224, PRN_10_01=3, SF055_10_01=2, SF056_10_01=1, SF060_10_01=7.360000000000014, SF061a_10_01=-0.695999999999998, SF061b_10_01=-0.3200000000000074, PRN_10_02=4, SF055_10_02=1, SF056_10_02=1, SF060_10_02=-3.599999999999966, SF061a_10_02=-0.38400000000000034, SF061b_10_02=0.1839999999999975, PRN_10_03=5, SF055_10_03=1, SF056_10_03=1, SF060_10_03=18.80000000000001, SF061a_10_03=0.2639999999999958, SF061b_10_03=0.7119999999999891, PRN_10_04=12, SF055_10_04=3, SF056_10_04=1, SF060_10_04=24.08000000000004, SF061a_10_04=-1.9280000000000044, SF061b_10_04=0.0, PRN_10_05=18, SF055_10_05=1, SF056_10_05=1, SF060_10_05=31.480000000000018, SF061a_10_05=0.9839999999999947, SF061b_10_05=-0.17600000000000193, PRN_10_06=19, SF055_10_06=1, SF056_10_06=1, SF060_10_06=3.480000000000018, SF061a_10_06=0.3919999999999959, SF061b_10_06=0.21599999999999397, PRN_10_07=20, SF055_10_07=2, SF056_10_07=1, SF060_10_07=10.240000000000009, SF061a_10_07=-0.936000000000007, SF061b_10_07=0.3199999999999932)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=468, eaf=1, crcType=2, frameCrc=5, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=59, authInd=1, embAuthLen=0, crc=11322474, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=20, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=0.0, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF012_01=3670128, PRN_01_01=3, SF055_01_01=1, SF056_01_01=1, SF060_01_01=27.400000000000034, SF061a_01_01=-1.152000000000001, SF061b_01_01=-0.8800000000000097, PRN_01_02=4, SF055_01_02=1, SF056_01_02=1, SF060_01_02=4.080000000000041, SF061a_01_02=-0.09600000000000364, SF061b_01_02=-0.2560000000000002, PRN_01_03=5, SF055_01_03=1, SF056_01_03=1, SF060_01_03=17.08000000000004, SF061a_01_03=0.11999999999999034, SF061b_01_03=-0.008000000000009777, PRN_01_04=18, SF055_01_04=1, SF056_01_04=1, SF060_01_04=57.44, SF061a_01_04=-0.07200000000000273, SF061b_01_04=-1.7440000000000069, PRN_01_05=19, SF055_01_05=1, SF056_01_05=1, SF060_01_05=10.560000000000002, SF061a_01_05=0.3999999999999915, SF061b_01_05=-0.46399999999999864, PRN_01_06=20, SF055_01_06=1, SF056_01_06=1, SF060_01_06=14.160000000000025, SF061a_01_06=-0.5600000000000023, SF061b_01_06=0.07199999999998852, SF031_02=21, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=3, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.16800000000000004, SF049a_02=-0.006000000000000005, SF049b_02=-0.01100000000000001, SF054_02=1, SatBitmaskLen_02=0, SF012_02=3670128, PRN_02_01=3, SF055_02_01=1, SF056_02_01=1, SF060_02_01=22.08000000000004, SF061a_02_01=-0.8960000000000008, SF061b_02_01=-0.7680000000000007, PRN_02_02=4, SF055_02_02=1, SF056_02_02=1, SF060_02_02=2.400000000000034, SF061a_02_02=-0.1039999999999992, SF061b_02_02=-0.32800000000000296, PRN_02_03=5, SF055_02_03=1, SF056_02_03=1, SF060_02_03=17.24000000000001, SF061a_02_03=0.14399999999999125, SF061b_02_03=0.09599999999998943, PRN_02_04=18, SF055_02_04=3, SF056_02_04=1, SF060_02_04=46.920000000000016, SF061a_02_04=0.08799999999999386, SF061b_02_04=-1.6160000000000068, PRN_02_05=19, SF055_02_05=1, SF056_02_05=1, SF060_02_05=7.8799999999999955, SF061a_02_05=0.4399999999999977, SF061b_02_05=-0.4399999999999977, PRN_02_06=20, SF055_02_06=1, SF056_02_06=1, SF060_02_06=14.160000000000025, SF061a_02_06=-0.5679999999999978, SF061b_02_06=-0.09600000000000364, SF031_03=22, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.17600000000000005, SF049a_03=0.007000000000000006, SF049b_03=-0.0030000000000000027, SF054_03=1, SatBitmaskLen_03=0, SF012_03=3670128, PRN_03_01=3, SF055_03_01=1, SF056_03_01=1, SF060_03_01=23.879999999999995, SF061a_03_01=0.11199999999999477, SF061b_03_01=-1.0160000000000053, PRN_03_02=4, SF055_03_02=1, SF056_03_02=1, SF060_03_02=6.8799999999999955, SF061a_03_02=0.7199999999999989, SF061b_03_02=-0.45600000000000307, PRN_03_03=5, SF055_03_03=2, SF056_03_03=1, SF060_03_03=23.80000000000001, SF061a_03_03=1.0879999999999939, SF061b_03_03=-0.12000000000000455, PRN_03_04=18, SF055_03_04=2, SF056_03_04=1, SF060_03_04=45.920000000000016, SF061a_03_04=1.039999999999992, SF061b_03_04=-1.2480000000000047, PRN_03_05=19, SF055_03_05=1, SF056_03_05=1, SF060_03_05=11.879999999999995, SF061a_03_05=1.4479999999999933, SF061b_03_05=-0.5280000000000058, PRN_03_06=20, SF055_03_06=3, SF056_03_06=1, SF060_03_06=20.120000000000005, SF061a_03_06=0.1039999999999992, SF061b_03_06=-0.2560000000000002, SF031_04=23, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.01200000000000001, SF044_04=1, SF048_04=-0.19599999999999995, SF049a_04=-0.01100000000000001, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF012_04=3670112, PRN_04_01=3, SF055_04_01=1, SF056_04_01=1, SF060_04_01=18.319999999999993, SF061a_04_01=0.27199999999999136, SF061b_04_01=-0.9280000000000115, PRN_04_02=4, SF055_04_02=1, SF056_04_02=1, SF060_04_02=4.480000000000018, SF061a_04_02=0.7039999999999935, SF061b_04_02=-0.3440000000000083, PRN_04_03=5, SF055_04_03=1, SF056_04_03=1, SF060_04_03=23.400000000000034, SF061a_04_03=1.2560000000000002, SF061b_04_03=0.02400000000000091, PRN_04_04=18, SF055_04_04=2, SF056_04_04=1, SF060_04_04=38.960000000000036, SF061a_04_04=0.7680000000000007, SF061b_04_04=-1.1280000000000001, PRN_04_05=19, SF055_04_05=1, SF056_04_05=1, SF060_04_05=9.200000000000045, SF061a_04_05=1.4159999999999968, SF061b_04_05=-0.32800000000000296, SF031_05=24, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.01200000000000001, SF044_05=1, SF048_05=-0.19599999999999995, SF049a_05=-0.0030000000000000027, SF049b_05=-0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF012_05=3670128, PRN_05_01=3, SF055_05_01=1, SF056_05_01=1, SF060_05_01=9.28000000000003, SF061a_05_01=-0.35999999999999943, SF061b_05_01=-0.6880000000000024, PRN_05_02=4, SF055_05_02=1, SF056_05_02=1, SF060_05_02=-1.5199999999999818, SF061a_05_02=0.031999999999996476, SF061b_05_02=-0.04000000000000625, PRN_05_03=5, SF055_05_03=1, SF056_05_03=1, SF060_05_03=19.960000000000036, SF061a_05_03=0.5360000000000014, SF061b_05_03=0.5999999999999943, PRN_05_04=18, SF055_05_04=2, SF056_05_04=1, SF060_05_04=30.319999999999993, SF061a_05_04=0.2560000000000002, SF061b_05_04=-0.19200000000000728, PRN_05_05=19, SF055_05_05=1, SF056_05_05=1, SF060_05_05=3.4399999999999977, SF061a_05_05=0.6079999999999899, SF061b_05_05=0.06399999999999295, PRN_05_06=20, SF055_05_06=1, SF056_05_06=1, SF060_05_06=13.960000000000036, SF061a_05_06=-0.3680000000000092, SF061b_05_06=0.13599999999999568, SF031_06=25, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=1, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.18400000000000005, SF049a_06=-0.006000000000000005, SF049b_06=0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF012_06=3672176, PRN_06_01=3, SF055_06_01=1, SF056_06_01=1, SF060_06_01=6.240000000000009, SF061a_06_01=-0.09600000000000364, SF061b_06_01=-0.5919999999999987, PRN_06_02=4, SF055_06_02=1, SF056_06_02=1, SF060_06_02=-1.7999999999999545, SF061a_06_02=-0.008000000000009777, SF061b_06_02=-0.055999999999997385, PRN_06_03=5, SF055_06_03=1, SF056_06_03=1, SF060_06_03=22.400000000000034, SF061a_06_03=0.9200000000000017, SF061b_06_03=0.5120000000000005, PRN_06_04=13, SF055_06_04=1, SF056_06_04=1, SF060_06_04=9.240000000000009, SF061a_06_04=-0.2960000000000065, SF061b_06_04=-0.8640000000000043, PRN_06_05=18, SF055_06_05=3, SF056_06_05=1, SF060_06_05=30.760000000000048, SF061a_06_05=0.02400000000000091, SF061b_06_05=0.367999999999995, PRN_06_06=19, SF055_06_06=1, SF056_06_06=1, SF060_06_06=3.0400000000000205, SF061a_06_06=0.5039999999999907, SF061b_06_06=0.04800000000000182, PRN_06_07=20, SF055_06_07=1, SF056_06_07=1, SF060_06_07=14.920000000000016, SF061a_06_07=-0.40800000000000125, SF061b_06_07=0.09599999999998943, SF031_07=26, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=3, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.17200000000000004, SF049a_07=0.0010000000000000009, SF049b_07=-0.007000000000000006, SF054_07=1, SatBitmaskLen_07=0, SF012_07=3670128, PRN_07_01=3, SF055_07_01=2, SF056_07_01=1, SF060_07_01=21.0, SF061a_07_01=-1.2480000000000047, SF061b_07_01=-1.0160000000000053, PRN_07_02=4, SF055_07_02=1, SF056_07_02=1, SF060_07_02=-10.239999999999952, SF061a_07_02=-0.24800000000000466, SF061b_07_02=-0.30400000000000205, PRN_07_03=5, SF055_07_03=2, SF056_07_03=1, SF060_07_03=-0.39999999999997726, SF061a_07_03=0.2879999999999967, SF061b_07_03=0.1599999999999966, PRN_07_04=18, SF055_07_04=4, SF056_07_04=1, SF060_07_04=54.28000000000003, SF061a_07_04=-2.5520000000000067, SF061b_07_04=-1.5360000000000014, PRN_07_05=19, SF055_07_05=2, SF056_07_05=1, SF060_07_05=-5.519999999999982, SF061a_07_05=0.35999999999999943, SF061b_07_05=-0.45600000000000307, PRN_07_06=20, SF055_07_06=1, SF056_07_06=1, SF060_07_06=0.8400000000000318, SF061a_07_06=-0.695999999999998, SF061b_07_06=0.06399999999999295, SF031_08=27, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.016000000000000014, SF044_08=1, SF048_08=-0.19199999999999995, SF049a_08=0.0030000000000000027, SF049b_08=0.0050000000000000044, SF054_08=1, SatBitmaskLen_08=0, SF012_08=3670128, PRN_08_01=3, SF055_08_01=3, SF056_08_01=1, SF060_08_01=35.44, SF061a_08_01=-1.3680000000000092, SF061b_08_01=-0.6560000000000059, PRN_08_02=4, SF055_08_02=1, SF056_08_02=1, SF060_08_02=8.920000000000016, SF061a_08_02=-0.5840000000000032, SF061b_08_02=0.07199999999998852, PRN_08_03=5, SF055_08_03=2, SF056_08_03=1, SF060_08_03=21.439999999999998, SF061a_08_03=-0.35200000000000387, SF061b_08_03=0.32799999999998875, PRN_08_04=18, SF055_08_04=5, SF056_08_04=1, SF060_08_04=63.04000000000002, SF061a_08_04=-3.4240000000000066, SF061b_08_04=-1.6160000000000068, PRN_08_05=19, SF055_08_05=1, SF056_08_05=1, SF060_08_05=13.319999999999993, SF061a_08_05=-0.08800000000000807, SF061b_08_05=-0.1039999999999992, PRN_08_06=20, SF055_08_06=2, SF056_08_06=1, SF060_08_06=21.04000000000002, SF061a_08_06=-1.1680000000000064, SF061b_08_06=0.30400000000000205, SF031_09=28, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.01200000000000001, SF044_09=1, SF048_09=-0.18799999999999994, SF049a_09=-0.008000000000000007, SF049b_09=0.0020000000000000018, SF054_09=1, SatBitmaskLen_09=0, SF012_09=3670128, PRN_09_01=3, SF055_09_01=1, SF056_09_01=1, SF060_09_01=32.48000000000002, SF061a_09_01=-1.3599999999999994, SF061b_09_01=-0.632000000000005, PRN_09_02=4, SF055_09_02=1, SF056_09_02=1, SF060_09_02=9.080000000000041, SF061a_09_02=-0.6080000000000041, SF061b_09_02=0.06399999999999295, PRN_09_03=5, SF055_09_03=2, SF056_09_03=1, SF060_09_03=22.960000000000036, SF061a_09_03=-0.4960000000000093, SF061b_09_03=0.5039999999999907, PRN_09_04=18, SF055_09_04=3, SF056_09_04=1, SF060_09_04=57.44, SF061a_09_04=-2.3600000000000065, SF061b_09_04=-1.2960000000000065, PRN_09_05=19, SF055_09_05=1, SF056_09_05=1, SF060_09_05=12.680000000000007, SF061a_09_05=-0.17600000000000193, SF061b_09_05=-0.1360000000000099, PRN_09_06=20, SF055_09_06=2, SF056_09_06=1, SF060_09_06=22.360000000000014, SF061a_09_06=-1.1839999999999975, SF061b_09_06=0.48799999999999955, SF031_10=29, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=4, SF043_10=0.01200000000000001, SF044_10=1, SF048_10=-0.18799999999999994, SF049a_10=0.045999999999999985, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=0, SF012_10=3670128, PRN_10_01=3, SF055_10_01=3, SF056_10_01=1, SF060_10_01=17.0, SF061a_10_01=-0.17600000000000193, SF061b_10_01=-0.784000000000006, PRN_10_02=4, SF055_10_02=2, SF056_10_02=1, SF060_10_02=-2.680000000000007, SF061a_10_02=0.3999999999999915, SF061b_10_02=-0.1039999999999992, PRN_10_03=5, SF055_10_03=4, SF056_10_03=1, SF060_10_03=13.240000000000009, SF061a_10_03=0.5759999999999934, SF061b_10_03=0.007999999999995566, PRN_10_04=18, SF055_10_04=2, SF056_10_04=1, SF060_10_04=39.31999999999999, SF061a_10_04=-1.024000000000001, SF061b_10_04=-0.7760000000000105, PRN_10_05=19, SF055_10_05=1, SF056_10_05=1, SF060_10_05=0.7200000000000273, SF061a_10_05=0.7999999999999972, SF061b_10_05=-0.20000000000000284, PRN_10_06=20, SF055_10_06=1, SF056_10_06=1, SF060_10_06=11.879999999999995, SF061a_10_06=-0.17600000000000193, SF061b_10_06=0.13599999999999568)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=468, eaf=1, crcType=2, frameCrc=5, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=60, authInd=1, embAuthLen=0, crc=13756719, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.18000000000000005, SF049a_01=-0.01200000000000001, SF049b_01=-0.006000000000000005, SF054_01=1, SatBitmaskLen_01=0, SF012_01=3670128, PRN_01_01=3, SF055_01_01=2, SF056_01_01=1, SF060_01_01=13.360000000000014, SF061a_01_01=0.0, SF061b_01_01=-0.8400000000000034, PRN_01_02=4, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-3.159999999999968, SF061a_01_02=0.4719999999999942, SF061b_01_02=-0.1360000000000099, PRN_01_03=5, SF055_01_03=3, SF056_01_03=1, SF060_01_03=13.800000000000011, SF061a_01_03=0.6079999999999899, SF061b_01_03=0.11999999999999034, PRN_01_04=18, SF055_01_04=4, SF056_01_04=1, SF060_01_04=35.360000000000014, SF061a_01_04=-1.6400000000000077, SF061b_01_04=-0.960000000000008, PRN_01_05=19, SF055_01_05=2, SF056_01_05=1, SF060_01_05=0.0, SF061a_01_05=0.6880000000000024, SF061b_01_05=-0.23199999999999932, PRN_01_06=20, SF055_01_06=1, SF056_01_06=1, SF060_01_06=11.920000000000016, SF061a_01_06=0.21599999999999397, SF061b_01_06=-0.08800000000000807, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.19599999999999995, SF049a_02=0.0050000000000000044, SF049b_02=0.0, SF054_02=1, SatBitmaskLen_02=0, SF012_02=3672176, PRN_02_01=3, SF055_02_01=2, SF056_02_01=1, SF060_02_01=10.840000000000032, SF061a_02_01=-0.04000000000000625, SF061b_02_01=-0.6159999999999997, PRN_02_02=4, SF055_02_02=2, SF056_02_02=1, SF060_02_02=-1.8799999999999955, SF061a_02_02=0.21599999999999397, SF061b_02_02=0.055999999999997385, PRN_02_03=5, SF055_02_03=2, SF056_02_03=1, SF060_02_03=17.120000000000005, SF061a_02_03=0.8319999999999936, SF061b_02_03=0.5600000000000023, PRN_02_04=13, SF055_02_04=3, SF056_02_04=1, SF060_02_04=16.04000000000002, SF061a_02_04=-0.3359999999999985, SF061b_02_04=-0.936000000000007, PRN_02_05=18, SF055_02_05=4, SF056_02_05=1, SF060_02_05=31.439999999999998, SF061a_02_05=-0.7120000000000033, SF061b_02_05=-0.6159999999999997, PRN_02_06=19, SF055_02_06=2, SF056_02_06=1, SF060_02_06=1.6000000000000227, SF061a_02_06=0.5519999999999925, SF061b_02_06=0.1599999999999966, PRN_02_07=20, SF055_02_07=4, SF056_02_07=1, SF060_02_07=14.360000000000014, SF061a_02_07=-0.27200000000000557, SF061b_02_07=0.32799999999998875, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.016000000000000014, SF044_03=1, SF048_03=-0.18799999999999994, SF049a_03=-0.037000000000000005, SF049b_03=-0.006000000000000005, SF054_03=1, SatBitmaskLen_03=0, SF012_03=3672176, PRN_03_01=3, SF055_03_01=1, SF056_03_01=1, SF060_03_01=6.439999999999998, SF061a_03_01=0.16799999999999216, SF061b_03_01=-0.5280000000000058, PRN_03_02=4, SF055_03_02=1, SF056_03_02=1, SF060_03_02=-2.079999999999984, SF061a_03_02=0.04800000000000182, SF061b_03_02=-0.1039999999999992, PRN_03_03=5, SF055_03_03=2, SF056_03_03=1, SF060_03_03=21.640000000000043, SF061a_03_03=0.7279999999999944, SF061b_03_03=0.8079999999999927, PRN_03_04=13, SF055_03_04=1, SF056_03_04=1, SF060_03_04=9.520000000000039, SF061a_03_04=0.16799999999999216, SF061b_03_04=-0.8320000000000078, PRN_03_05=18, SF055_03_05=5, SF056_03_05=1, SF060_03_05=31.400000000000034, SF061a_03_05=0.46399999999999864, SF061b_03_05=0.7439999999999998, PRN_03_06=19, SF055_03_06=1, SF056_03_06=1, SF060_03_06=1.9600000000000364, SF061a_03_06=0.6319999999999908, SF061b_03_06=0.08799999999999386, PRN_03_07=20, SF055_03_07=3, SF056_03_07=1, SF060_03_07=15.920000000000016, SF061a_03_07=0.015999999999991132, SF061b_03_07=0.2879999999999967, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.128, SF049a_04=-0.013000000000000012, SF049b_04=0.0, SF054_04=1, SatBitmaskLen_04=0, SF012_04=3670128, PRN_04_01=3, SF055_04_01=6, SF056_04_01=1, SF060_04_01=23.879999999999995, SF061a_04_01=-0.21600000000000819, SF061b_04_01=-0.9759999999999991, PRN_04_02=4, SF055_04_02=2, SF056_04_02=1, SF060_04_02=-10.359999999999957, SF061a_04_02=0.28000000000000114, SF061b_04_02=-0.4000000000000057, PRN_04_03=5, SF055_04_03=2, SF056_04_03=1, SF060_04_03=-2.919999999999959, SF061a_04_03=0.7759999999999962, SF061b_04_03=0.09599999999998943, PRN_04_04=18, SF055_04_04=5, SF056_04_04=1, SF060_04_04=72.72000000000003, SF061a_04_04=-5.648000000000003, SF061b_04_04=-0.5679999999999978, PRN_04_05=19, SF055_04_05=2, SF056_04_05=1, SF060_04_05=-7.639999999999986, SF061a_04_05=0.5360000000000014, SF061b_04_05=-0.3359999999999985, PRN_04_06=20, SF055_04_06=4, SF056_04_06=1, SF060_04_06=2.680000000000007, SF061a_04_06=-0.17600000000000193, SF061b_04_06=-0.07200000000000273, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.14400000000000002, SF049a_05=-0.021999999999999992, SF049b_05=0.014000000000000012, SF054_05=1, SatBitmaskLen_05=0, SF012_05=3670128, PRN_05_01=3, SF055_05_01=4, SF056_05_01=1, SF060_05_01=40.160000000000025, SF061a_05_01=-0.8960000000000008, SF061b_05_01=-0.9120000000000061, PRN_05_02=4, SF055_05_02=4, SF056_05_02=1, SF060_05_02=11.120000000000005, SF061a_05_02=-0.4000000000000057, SF061b_05_02=0.04800000000000182, PRN_05_03=5, SF055_05_03=4, SF056_05_03=1, SF060_05_03=22.52000000000004, SF061a_05_03=-0.14400000000000546, SF061b_05_03=0.4399999999999977, PRN_05_04=18, SF055_05_04=6, SF056_05_04=1, SF060_05_04=86.12, SF061a_05_04=-6.736000000000004, SF061b_05_04=-1.9280000000000044, PRN_05_05=19, SF055_05_05=3, SF056_05_05=1, SF060_05_05=13.879999999999995, SF061a_05_05=-0.22400000000000375, SF061b_05_05=-0.016000000000005343, PRN_05_06=20, SF055_05_06=4, SF056_05_06=1, SF060_05_06=25.760000000000048, SF061a_05_06=-0.8400000000000034, SF061b_05_06=0.1839999999999975, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.016000000000000014, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0030000000000000027, SF049b_06=0.006000000000000005, SF054_06=1, SatBitmaskLen_06=0, SF012_06=3670128, PRN_06_01=3, SF055_06_01=2, SF056_06_01=1, SF060_06_01=11.400000000000034, SF061a_06_01=0.5759999999999934, SF061b_06_01=-0.7280000000000086, PRN_06_02=4, SF055_06_02=2, SF056_06_02=1, SF060_06_02=-4.8799999999999955, SF061a_06_02=0.5759999999999934, SF061b_06_02=-0.06400000000000716, PRN_06_03=5, SF055_06_03=2, SF056_06_03=1, SF060_06_03=12.480000000000018, SF061a_06_03=0.47999999999998977, SF061b_06_03=0.23999999999999488, PRN_06_04=18, SF055_06_04=5, SF056_06_04=1, SF060_06_04=40.68000000000001, SF061a_06_04=-3.7040000000000077, SF061b_06_04=-1.2720000000000056, PRN_06_05=19, SF055_06_05=1, SF056_06_05=1, SF060_06_05=-2.0, SF061a_06_05=0.519999999999996, SF061b_06_05=-0.04000000000000625, PRN_06_06=20, SF055_06_06=5, SF056_06_06=1, SF060_06_06=11.120000000000005, SF061a_06_06=0.4399999999999977, SF061b_06_06=0.11999999999999034, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=4, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.15200000000000002, SF049a_07=-0.04500000000000001, SF049b_07=-0.015000000000000013, SF054_07=1, SatBitmaskLen_07=0, SF012_07=3670128, PRN_07_01=3, SF055_07_01=1, SF056_07_01=1, SF060_07_01=16.760000000000048, SF061a_07_01=-0.7360000000000042, SF061b_07_01=-0.9120000000000061, PRN_07_02=4, SF055_07_02=1, SF056_07_02=1, SF060_07_02=4.960000000000036, SF061a_07_02=-0.6480000000000103, SF061b_07_02=-0.3440000000000083, PRN_07_03=5, SF055_07_03=4, SF056_07_03=1, SF060_07_03=24.439999999999998, SF061a_07_03=-0.8400000000000034, SF061b_07_03=0.23199999999999932, PRN_07_04=18, SF055_07_04=4, SF056_07_04=1, SF060_07_04=40.120000000000005, SF061a_07_04=-2.0160000000000053, SF061b_07_04=-1.1839999999999975, PRN_07_05=19, SF055_07_05=2, SF056_07_05=1, SF060_07_05=7.960000000000036, SF061a_07_05=-0.7120000000000033, SF061b_07_05=-0.21600000000000819, PRN_07_06=20, SF055_07_06=1, SF056_07_06=1, SF060_07_06=22.24000000000001, SF061a_07_06=-0.7040000000000077, SF061b_07_06=-0.0799999999999983, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.016000000000000014, SF044_08=1, SF048_08=-0.16800000000000004, SF049a_08=-0.010000000000000009, SF049b_08=0.009000000000000008, SF054_08=1, SatBitmaskLen_08=0, SF012_08=3670128, PRN_08_01=3, SF055_08_01=1, SF056_08_01=1, SF060_08_01=12.600000000000023, SF061a_08_01=-0.6800000000000068, SF061b_08_01=-0.784000000000006, PRN_08_02=4, SF055_08_02=1, SF056_08_02=1, SF060_08_02=3.319999999999993, SF061a_08_02=-0.5520000000000067, SF061b_08_02=-0.30400000000000205, PRN_08_03=5, SF055_08_03=2, SF056_08_03=1, SF060_08_03=25.80000000000001, SF061a_08_03=-0.40800000000000125, SF061b_08_03=0.35199999999998965, PRN_08_04=18, SF055_08_04=2, SF056_08_04=1, SF060_08_04=36.80000000000001, SF061a_08_04=-0.9120000000000061, SF061b_08_04=-0.12000000000000455, PRN_08_05=19, SF055_08_05=1, SF056_08_05=1, SF060_08_05=6.960000000000036, SF061a_08_05=-0.4480000000000075, SF061b_08_05=-0.1600000000000108, PRN_08_06=20, SF055_08_06=2, SF056_08_06=1, SF060_08_06=21.640000000000043, SF061a_08_06=-0.695999999999998, SF061b_08_06=-0.1839999999999975, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.15600000000000003, SF049a_09=0.0010000000000000009, SF049b_09=-0.0010000000000000009, SF054_09=1, SatBitmaskLen_09=0, SF012_09=3670048, PRN_09_01=3, SF055_09_01=1, SF056_09_01=1, SF060_09_01=7.920000000000016, SF061a_09_01=0.8960000000000008, SF061b_09_01=-0.6240000000000094, PRN_09_02=4, SF055_09_02=4, SF056_09_02=1, SF060_09_02=-7.519999999999982, SF061a_09_02=0.7439999999999998, SF061b_09_02=0.0799999999999983, PRN_09_03=5, SF055_09_03=1, SF056_09_03=1, SF060_09_03=11.160000000000025, SF061a_09_03=0.367999999999995, SF061b_09_03=0.16799999999999216, PRN_09_04=19, SF055_09_04=3, SF056_09_04=1, SF060_09_04=-3.4399999999999977, SF061a_09_04=0.19999999999998863, SF061b_09_04=0.08799999999999386, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=4, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.14400000000000002, SF049a_10=0.04999999999999999, SF049b_10=-0.038000000000000006, SF054_10=1, SatBitmaskLen_10=0, SF012_10=3670128, PRN_10_01=3, SF055_10_01=1, SF056_10_01=1, SF060_10_01=17.760000000000048, SF061a_10_01=-0.22400000000000375, SF061b_10_01=-0.5679999999999978, PRN_10_02=4, SF055_10_02=1, SF056_10_02=1, SF060_10_02=6.0400000000000205, SF061a_10_02=-0.04800000000000182, SF061b_10_02=-0.14400000000000546, PRN_10_03=5, SF055_10_03=1, SF056_10_03=1, SF060_10_03=28.200000000000045, SF061a_10_03=-1.0480000000000018, SF061b_10_03=0.30400000000000205, PRN_10_04=18, SF055_10_04=2, SF056_10_04=1, SF060_10_04=46.879999999999995, SF061a_10_04=-2.768000000000008, SF061b_10_04=-2.216000000000001, PRN_10_05=19, SF055_10_05=1, SF056_10_05=1, SF060_10_05=10.439999999999998, SF061a_10_05=-0.7040000000000077, SF061b_10_05=-0.06400000000000716, PRN_10_06=20, SF055_10_06=1, SF056_10_06=1, SF060_10_06=23.840000000000032, SF061a_10_06=-0.1039999999999992, SF061b_10_06=0.0799999999999983)>",
+            "<SPARTN(SPARTN-1X-HPAC-GLO, msgType=1, nData=61, eaf=1, crcType=2, frameCrc=15, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=61, authInd=1, embAuthLen=0, crc=13417473, SF005=152, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.17600000000000005, SF049a_01=-0.017999999999999988, SF049b_01=0.0020000000000000018, SF054_01=1, SatBitmaskLen_01=0, SF012_01=4144, PRN_01_01=12, SF055_01_01=5, SF056_01_01=1, SF060_01_01=26.960000000000036, SF061a_01_01=-1.6000000000000014, SF061b_01_01=-0.416000000000011, PRN_01_02=19, SF055_01_02=1, SF056_01_02=1, SF060_01_02=6.160000000000025, SF061a_01_02=0.73599999999999, SF061b_01_02=-0.07200000000000273, PRN_01_03=20, SF055_01_03=2, SF056_01_03=1, SF060_01_03=16.160000000000025, SF061a_01_03=-0.4960000000000093, SF061b_01_03=0.13599999999999568, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.18799999999999994, SF049a_02=0.0010000000000000009, SF049b_02=0.0030000000000000027, SF054_02=1, SatBitmaskLen_02=0, SF012_02=4144, PRN_02_01=12, SF055_02_01=5, SF056_02_01=1, SF060_02_01=23.920000000000016, SF061a_02_01=-0.5520000000000067, SF061b_02_01=-0.45600000000000307, PRN_02_02=19, SF055_02_02=1, SF056_02_02=1, SF060_02_02=7.680000000000007, SF061a_02_02=0.7599999999999909, SF061b_02_02=-0.09600000000000364, PRN_02_03=20, SF055_02_03=2, SF056_02_03=1, SF060_02_03=15.28000000000003, SF061a_02_03=-0.3920000000000101, SF061b_02_03=0.1280000000000001)>",
         ]
         i = 0
         with open(os.path.join(self.dirname, "spartnHPAC.log"), "rb") as stream:
             spr = SPARTNReader(
                 stream,
                 quitonerror=ERRRAISE,
                 decode=True,
@@ -177,14 +210,39 @@
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertEqual(str(parsed), EXPECTED_RESULT[i])
                     self.assertTrue(0 <= parsed._padding <= 8)
                     i += 1
         self.assertEqual(i, 10)
 
+    def testGADLOGnodecode(
+        self,
+    ):  # test PARTN GAD message no decode
+        EXPECTED_RESULT = [
+            "<SPARTN(SPARTN-1X-GAD, msgType=2, nData=191, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=0, gnssTimeTag=28080, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=34, authInd=1, embAuthLen=0, crc=1303268)>",
+            "<SPARTN(SPARTN-1X-GAD, msgType=2, nData=62, eaf=1, crcType=2, frameCrc=1, msgSubtype=0, timeTagtype=0, gnssTimeTag=28080, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=35, authInd=1, embAuthLen=0, crc=15938608)>",
+            "<SPARTN(SPARTN-1X-GAD, msgType=2, nData=191, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=0, gnssTimeTag=28110, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=36, authInd=1, embAuthLen=0, crc=9218824)>",
+            "<SPARTN(SPARTN-1X-GAD, msgType=2, nData=62, eaf=1, crcType=2, frameCrc=1, msgSubtype=0, timeTagtype=0, gnssTimeTag=28110, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=37, authInd=1, embAuthLen=0, crc=11512563)>",
+        ]
+        i = 0
+        with open(os.path.join(self.dirname, "spartnGAD.log"), "rb") as stream:
+            spr = SPARTNReader(
+                stream,
+                quitonerror=ERRRAISE,
+                decode=False,
+            )
+
+            for raw, parsed in spr:
+                if raw is not None:
+                    # print(f'"{parsed}",')
+                    self.assertEqual(str(parsed), EXPECTED_RESULT[i])
+                    self.assertTrue(0 <= parsed._padding <= 8)
+                    i += 1
+        self.assertEqual(i, 4)
+
     def testGADLOG(
         self,
     ):  # test decoding of SPARTN GAD message
         EXPECTED_RESULT = [
             "<SPARTN(SPARTN-1X-GAD, msgType=2, nData=191, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=0, gnssTimeTag=28080, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=34, authInd=1, embAuthLen=0, crc=1303268, SF005=152, SF068=1, SF069=0, SF030=31, SF031_01=0, SF032_01=71.30000000000001, SF033_01=12.5, SF034_01=4, SF035_01=6, SF036_01=0.8, SF037_01=3.2, SF031_02=1, SF032_02=68.20000000000002, SF033_02=10.5, SF034_02=2, SF035_02=7, SF036_02=1.7000000000000002, SF037_02=1.6, SF031_03=2, SF032_03=68.30000000000001, SF033_03=21.700000000000017, SF034_03=7, SF035_03=5, SF036_03=0.5, SF037_03=1.7000000000000002, SF031_04=3, SF032_04=65.20000000000002, SF033_04=4.300000000000011, SF034_04=7, SF035_04=5, SF036_04=0.5, SF037_04=2.9000000000000004, SF031_05=4, SF032_05=64.9, SF033_05=18.80000000000001, SF034_05=7, SF035_05=5, SF036_05=0.5, SF037_05=2.6, SF031_06=5, SF032_06=61.80000000000001, SF033_06=4.300000000000011, SF034_06=7, SF035_06=7, SF036_06=0.6, SF037_06=1.0, SF031_07=6, SF032_07=61.80000000000001, SF033_07=11.300000000000011, SF034_07=7, SF035_07=5, SF036_07=0.6, SF037_07=1.5000000000000002, SF031_08=7, SF032_08=61.5, SF033_08=18.80000000000001, SF034_08=2, SF035_08=6, SF036_08=1.9000000000000001, SF037_08=1.8000000000000003, SF031_09=8, SF032_09=59.599999999999994, SF033_09=-9.0, SF034_09=7, SF035_09=7, SF036_09=0.7000000000000001, SF037_09=1.2000000000000002, SF031_10=9, SF032_10=57.70000000000002, SF033_10=7.700000000000017, SF034_10=7, SF035_10=6, SF036_10=0.5, SF037_10=1.6, SF031_11=10, SF032_11=57.900000000000006, SF033_11=17.30000000000001, SF034_11=5, SF035_11=5, SF036_11=0.8, SF037_11=2.2, SF031_12=11, SF032_12=54.80000000000001, SF033_12=-11.199999999999989, SF034_12=6, SF035_12=6, SF036_12=0.6, SF037_12=1.0, SF031_13=12, SF032_13=54.80000000000001, SF033_13=-5.399999999999977, SF034_13=6, SF035_13=7, SF036_13=0.6, SF037_13=1.2000000000000002, SF031_14=13, SF032_14=54.5, SF033_14=3.0, SF034_14=6, SF035_14=7, SF036_14=0.6, SF037_14=1.1, SF031_15=14, SF032_15=54.30000000000001, SF033_15=10.700000000000017, SF034_15=3, SF035_15=7, SF036_15=1.1, SF037_15=0.7000000000000001, SF031_16=15, SF032_16=54.30000000000001, SF033_16=15.600000000000023, SF034_16=6, SF035_16=7, SF036_16=0.5, SF037_16=1.2000000000000002, SF031_17=16, SF032_17=51.30000000000001, SF033_17=-6.099999999999994, SF034_17=2, SF035_17=6, SF036_17=1.3000000000000003, SF037_17=1.1, SF031_18=17, SF032_18=51.30000000000001, SF033_18=0.5, SF034_18=5, SF035_18=6, SF036_18=0.5, SF037_18=1.1, SF031_19=18, SF032_19=51.099999999999994, SF033_19=6.700000000000017, SF034_19=2, SF035_19=7, SF036_19=1.1, SF037_19=1.2000000000000002, SF031_20=19, SF032_20=51.5, SF033_20=15.100000000000023, SF034_20=3, SF035_20=6, SF036_20=0.9, SF037_20=1.3000000000000003, SF031_21=20, SF032_21=49.099999999999994, SF033_21=-5.299999999999983, SF034_21=6, SF035_21=5, SF036_21=0.6, SF037_21=1.5000000000000002, SF031_22=21, SF032_22=49.099999999999994, SF033_22=2.200000000000017, SF034_22=4, SF035_22=5, SF036_22=0.8, SF037_22=0.9, SF031_23=22, SF032_23=49.099999999999994, SF033_23=6.700000000000017, SF034_23=4, SF035_23=7, SF036_23=0.8, SF037_23=0.9, SF031_24=23, SF032_24=49.0, SF033_24=13.0, SF034_24=3, SF035_24=4, SF036_24=1.1, SF037_24=1.3000000000000003, SF031_25=24, SF032_25=48.900000000000006, SF033_25=18.200000000000017, SF034_25=6, SF035_25=4, SF036_25=0.5, SF037_25=1.1, SF031_26=25, SF032_26=47.400000000000006, SF033_26=22.200000000000017, SF034_26=6, SF035_26=5, SF036_26=0.4, SF037_26=1.5000000000000002, SF031_27=26, SF032_27=44.30000000000001, SF033_27=-9.599999999999994, SF034_27=7, SF035_27=7, SF036_27=0.6, SF037_27=1.0, SF031_28=27, SF032_28=45.70000000000002, SF033_28=-2.5999999999999943, SF034_28=6, SF035_28=4, SF036_28=0.8, SF037_28=1.1, SF031_29=28, SF032_29=46.0, SF033_29=1.4000000000000057, SF034_29=7, SF035_29=5, SF036_29=0.7000000000000001, SF037_29=1.0, SF031_30=29, SF032_30=46.0, SF033_30=6.400000000000006, SF034_30=4, SF035_30=7, SF036_30=0.8, SF037_30=0.6, SF031_31=30, SF032_31=46.0, SF033_31=10.600000000000023, SF034_31=3, SF035_31=2, SF036_31=0.9, SF037_31=2.3000000000000003, SF031_32=31, SF032_32=46.099999999999994, SF033_32=15.200000000000017, SF034_32=6, SF035_32=6, SF036_32=0.5, SF037_32=1.2000000000000002)>",
             "<SPARTN(SPARTN-1X-GAD, msgType=2, nData=62, eaf=1, crcType=2, frameCrc=1, msgSubtype=0, timeTagtype=0, gnssTimeTag=28080, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=35, authInd=1, embAuthLen=0, crc=15938608, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=32, SF032_01=45.20000000000002, SF033_01=22.400000000000006, SF034_01=2, SF035_01=7, SF036_01=1.1, SF037_01=1.1, SF031_02=33, SF032_02=40.30000000000001, SF033_02=-9.899999999999977, SF034_02=2, SF035_02=6, SF036_02=2.3000000000000003, SF037_02=1.2000000000000002, SF031_03=34, SF032_03=41.20000000000002, SF033_03=-2.6999999999999886, SF034_03=6, SF035_03=6, SF036_03=0.8, SF037_03=0.9, SF031_04=35, SF032_04=43.400000000000006, SF033_04=10.300000000000011, SF034_04=2, SF035_04=7, SF036_04=1.7000000000000002, SF037_04=1.2000000000000002, SF031_05=36, SF032_05=43.20000000000002, SF033_05=18.700000000000017, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=2.3000000000000003, SF031_06=37, SF032_06=43.20000000000002, SF033_06=23.30000000000001, SF034_06=6, SF035_06=3, SF036_06=0.6, SF037_06=1.7000000000000002, SF031_07=38, SF032_07=40.20000000000002, SF033_07=12.100000000000023, SF034_07=2, SF035_07=6, SF036_07=1.9000000000000001, SF037_07=1.1, SF031_08=39, SF032_08=39.70000000000002, SF033_08=18.700000000000017, SF034_08=3, SF035_08=3, SF036_08=1.3000000000000003, SF037_08=2.3000000000000003, SF031_09=40, SF032_09=49.80000000000001, SF033_09=22.600000000000023, SF034_09=5, SF035_09=7, SF036_09=0.5, SF037_09=1.1, SF031_10=41, SF032_10=52.0, SF033_10=22.900000000000006, SF034_10=6, SF035_10=5, SF036_10=0.4, SF037_10=1.7000000000000002)>",
             "<SPARTN(SPARTN-1X-GAD, msgType=2, nData=191, eaf=1, crcType=2, frameCrc=14, msgSubtype=0, timeTagtype=0, gnssTimeTag=28110, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=36, authInd=1, embAuthLen=0, crc=9218824, SF005=153, SF068=1, SF069=0, SF030=31, SF031_01=0, SF032_01=71.30000000000001, SF033_01=12.5, SF034_01=4, SF035_01=6, SF036_01=0.8, SF037_01=3.2, SF031_02=1, SF032_02=68.20000000000002, SF033_02=10.5, SF034_02=2, SF035_02=7, SF036_02=1.7000000000000002, SF037_02=1.6, SF031_03=2, SF032_03=68.30000000000001, SF033_03=21.700000000000017, SF034_03=7, SF035_03=5, SF036_03=0.5, SF037_03=1.7000000000000002, SF031_04=3, SF032_04=65.20000000000002, SF033_04=4.300000000000011, SF034_04=7, SF035_04=5, SF036_04=0.5, SF037_04=2.9000000000000004, SF031_05=4, SF032_05=64.9, SF033_05=18.80000000000001, SF034_05=7, SF035_05=5, SF036_05=0.5, SF037_05=2.6, SF031_06=5, SF032_06=61.80000000000001, SF033_06=4.300000000000011, SF034_06=7, SF035_06=7, SF036_06=0.6, SF037_06=1.0, SF031_07=6, SF032_07=61.80000000000001, SF033_07=11.300000000000011, SF034_07=7, SF035_07=5, SF036_07=0.6, SF037_07=1.5000000000000002, SF031_08=7, SF032_08=61.5, SF033_08=18.80000000000001, SF034_08=2, SF035_08=6, SF036_08=1.9000000000000001, SF037_08=1.8000000000000003, SF031_09=8, SF032_09=59.599999999999994, SF033_09=-9.0, SF034_09=7, SF035_09=7, SF036_09=0.7000000000000001, SF037_09=1.2000000000000002, SF031_10=9, SF032_10=57.70000000000002, SF033_10=7.700000000000017, SF034_10=7, SF035_10=6, SF036_10=0.5, SF037_10=1.6, SF031_11=10, SF032_11=57.900000000000006, SF033_11=17.30000000000001, SF034_11=5, SF035_11=5, SF036_11=0.8, SF037_11=2.2, SF031_12=11, SF032_12=54.80000000000001, SF033_12=-11.199999999999989, SF034_12=6, SF035_12=6, SF036_12=0.6, SF037_12=1.0, SF031_13=12, SF032_13=54.80000000000001, SF033_13=-5.399999999999977, SF034_13=6, SF035_13=7, SF036_13=0.6, SF037_13=1.2000000000000002, SF031_14=13, SF032_14=54.5, SF033_14=3.0, SF034_14=6, SF035_14=7, SF036_14=0.6, SF037_14=1.1, SF031_15=14, SF032_15=54.30000000000001, SF033_15=10.700000000000017, SF034_15=3, SF035_15=7, SF036_15=1.1, SF037_15=0.7000000000000001, SF031_16=15, SF032_16=54.30000000000001, SF033_16=15.600000000000023, SF034_16=6, SF035_16=7, SF036_16=0.5, SF037_16=1.2000000000000002, SF031_17=16, SF032_17=51.30000000000001, SF033_17=-6.099999999999994, SF034_17=2, SF035_17=6, SF036_17=1.3000000000000003, SF037_17=1.1, SF031_18=17, SF032_18=51.30000000000001, SF033_18=0.5, SF034_18=5, SF035_18=6, SF036_18=0.5, SF037_18=1.1, SF031_19=18, SF032_19=51.099999999999994, SF033_19=6.700000000000017, SF034_19=2, SF035_19=7, SF036_19=1.1, SF037_19=1.2000000000000002, SF031_20=19, SF032_20=51.5, SF033_20=15.100000000000023, SF034_20=3, SF035_20=6, SF036_20=0.9, SF037_20=1.3000000000000003, SF031_21=20, SF032_21=49.099999999999994, SF033_21=-5.299999999999983, SF034_21=6, SF035_21=5, SF036_21=0.6, SF037_21=1.5000000000000002, SF031_22=21, SF032_22=49.099999999999994, SF033_22=2.200000000000017, SF034_22=4, SF035_22=5, SF036_22=0.8, SF037_22=0.9, SF031_23=22, SF032_23=49.099999999999994, SF033_23=6.700000000000017, SF034_23=4, SF035_23=7, SF036_23=0.8, SF037_23=0.9, SF031_24=23, SF032_24=49.0, SF033_24=13.0, SF034_24=3, SF035_24=4, SF036_24=1.1, SF037_24=1.3000000000000003, SF031_25=24, SF032_25=48.900000000000006, SF033_25=18.200000000000017, SF034_25=6, SF035_25=4, SF036_25=0.5, SF037_25=1.1, SF031_26=25, SF032_26=47.400000000000006, SF033_26=22.200000000000017, SF034_26=6, SF035_26=5, SF036_26=0.4, SF037_26=1.5000000000000002, SF031_27=26, SF032_27=44.30000000000001, SF033_27=-9.599999999999994, SF034_27=7, SF035_27=7, SF036_27=0.6, SF037_27=1.0, SF031_28=27, SF032_28=45.70000000000002, SF033_28=-2.5999999999999943, SF034_28=6, SF035_28=4, SF036_28=0.8, SF037_28=1.1, SF031_29=28, SF032_29=46.0, SF033_29=1.4000000000000057, SF034_29=7, SF035_29=5, SF036_29=0.7000000000000001, SF037_29=1.0, SF031_30=29, SF032_30=46.0, SF033_30=6.400000000000006, SF034_30=4, SF035_30=7, SF036_30=0.8, SF037_30=0.6, SF031_31=30, SF032_31=46.0, SF033_31=10.600000000000023, SF034_31=3, SF035_31=2, SF036_31=0.9, SF037_31=2.3000000000000003, SF031_32=31, SF032_32=46.099999999999994, SF033_32=15.200000000000017, SF034_32=6, SF035_32=6, SF036_32=0.5, SF037_32=1.2000000000000002)>",
@@ -193,39 +251,72 @@
         i = 0
         with open(os.path.join(self.dirname, "spartnGAD.log"), "rb") as stream:
             spr = SPARTNReader(
                 stream,
                 quitonerror=ERRRAISE,
                 decode=True,
                 key=SPARTN_KEY,
-                basedate=SPARTN_BASEDATE,
+                basedate=SPARTN_BASEDATE_INT,
             )
 
             for raw, parsed in spr:
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertEqual(str(parsed), EXPECTED_RESULT[i])
                     self.assertTrue(0 <= parsed._padding <= 8)
                     i += 1
         self.assertEqual(i, 4)
 
+    def testOCBLOGnodecode(
+        self,
+    ):  # test SPARTN OCB GPS message no decode
+        EXPECTED_RESULT = [
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=30, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=0, gnssTimeTag=28075, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=37, authInd=1, embAuthLen=0, crc=4342523)>",
+            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=33, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=0, gnssTimeTag=38857, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=28, authInd=1, embAuthLen=0, crc=4143853)>",
+            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=36, eaf=1, crcType=2, frameCrc=11, msgSubtype=3, timeTagtype=0, gnssTimeTag=28061, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=60, authInd=1, embAuthLen=0, crc=13197342)>",
+            "<SPARTN(SPARTN-1X-OCB-GAL, msgType=0, nData=34, eaf=1, crcType=2, frameCrc=3, msgSubtype=2, timeTagtype=0, gnssTimeTag=28075, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=28, authInd=1, embAuthLen=0, crc=5329954)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=180, eaf=1, crcType=2, frameCrc=9, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=38, authInd=1, embAuthLen=0, crc=11341296)>",
+            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=152, eaf=1, crcType=2, frameCrc=2, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=29, authInd=1, embAuthLen=0, crc=1087652)>",
+            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=220, eaf=1, crcType=2, frameCrc=0, msgSubtype=3, timeTagtype=1, gnssTimeTag=451165666, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=61, authInd=1, embAuthLen=0, crc=14343958)>",
+            "<SPARTN(SPARTN-1X-OCB-GAL, msgType=0, nData=191, eaf=1, crcType=2, frameCrc=11, msgSubtype=2, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=29, authInd=1, embAuthLen=0, crc=5207238)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=30, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=0, gnssTimeTag=28085, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=39, authInd=1, embAuthLen=0, crc=11321430)>",
+            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=33, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=0, gnssTimeTag=38867, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=517021)>",
+        ]
+
+        # test using datetime as basedate
+        i = 0
+        with open(os.path.join(self.dirname, "spartnOCB.log"), "rb") as stream:
+            spr = SPARTNReader(
+                stream,
+                quitonerror=ERRRAISE,
+                decode=False,
+            )
+
+            for raw, parsed in spr:
+                if raw is not None:
+                    # print(f'"{parsed}",')
+                    self.assertEqual(str(parsed), EXPECTED_RESULT[i])
+                    self.assertTrue(0 <= parsed._padding <= 8)
+                    i += 1
+        self.assertEqual(i, 10)
+
     def testOCBLOG(
         self,
     ):  # test decoding of SPARTN OCB GPS message
         EXPECTED_RESULT = (
-            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=30, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=0, gnssTimeTag=28075, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=37, authInd=1, embAuthLen=0, crc=4342523, SF005=151, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=880836738, SF013_01=0, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=4.727999999999998, SF024_01=1, SF013_02=0, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=2.0459999999999994, SF024_02=1, SF013_03=0, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=2.622, SF024_03=1, SF013_04=0, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=2.823999999999998, SF024_04=1, SF013_05=0, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=-1.0020000000000007, SF024_05=2, SF013_06=0, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=3.6099999999999994, SF024_06=1, SF013_07=0, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-1.3600000000000012, SF024_07=1)>",
-            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=33, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=0, gnssTimeTag=38857, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=28, authInd=1, embAuthLen=0, crc=4143853, SF005=151, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=3676272, SF013_01=0, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=-0.0259999999999998, SF024_01=3, SF013_02=0, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=1.8780000000000001, SF024_02=2, SF013_03=0, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=1.9819999999999993, SF024_03=2, SF013_04=0, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=1.9279999999999973, SF024_04=2, SF013_05=0, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=2.2959999999999994, SF024_05=1, SF013_06=0, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=-1.7960000000000012, SF024_06=3, SF013_07=0, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-0.8880000000000017, SF024_07=2, SF013_08=0, SF014O_08=0, SF014C_08=1, SF014B_08=0, SF015_08=7, SF022_08=7, SF020CK_08=7.311999999999998, SF024_08=1)>",
-            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=36, eaf=1, crcType=2, frameCrc=11, msgSubtype=3, timeTagtype=0, gnssTimeTag=28061, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=60, authInd=1, embAuthLen=0, crc=13197342, SF005=151, SF010=0, SF069=0, SF008=0, SF009=0, SF097=0, SatBitmaskLen=1, SF094=212025376, SF013_01=0, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=2.849999999999998, SF024_01=1, SF013_02=0, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=3.565999999999999, SF024_02=3, SF013_03=0, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=5.654, SF024_03=1, SF013_04=0, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=0.39000000000000057, SF024_04=1, SF013_05=0, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=-0.8080000000000016, SF024_05=2, SF013_06=0, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=-3.612000000000002, SF024_06=4, SF013_07=0, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-1.9200000000000017, SF024_07=2, SF013_08=0, SF014O_08=0, SF014C_08=1, SF014B_08=0, SF015_08=7, SF022_08=7, SF020CK_08=-6.6800000000000015, SF024_08=4)>",
-            "<SPARTN(SPARTN-1X-OCB-GAL, msgType=0, nData=34, eaf=1, crcType=2, frameCrc=3, msgSubtype=2, timeTagtype=0, gnssTimeTag=28075, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=28, authInd=1, embAuthLen=0, crc=5329954, SF005=151, SF010=1, SF069=0, SF008=0, SF009=0, SF096=1, SatBitmaskLen=0, SF093=9405731848, SF013_01=0, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=3.0700000000000003, SF024_01=1, SF013_02=0, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=3.724, SF024_02=1, SF013_03=0, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=1.9499999999999993, SF024_03=1, SF013_04=0, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=1.7680000000000007, SF024_04=1, SF013_05=0, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=6, SF020CK_05=3.1419999999999995, SF024_05=1, SF013_06=0, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=-1.7940000000000005, SF024_06=1, SF013_07=0, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-2.902000000000001, SF024_07=1, SF013_08=0, SF014O_08=0, SF014C_08=1, SF014B_08=0, SF015_08=3, SF022_08=3, SF020CK_08=-1.886000000000001, SF024_08=1)>",
-            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=180, eaf=1, crcType=2, frameCrc=9, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=38, authInd=1, embAuthLen=0, crc=11341296, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=880836738, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF018_01=47, SF020R_01=0.0259999999999998, SF020A_01=0.597999999999999, SF020C_01=0.31799999999999784, SF022_01=7, SF020CK_01=4.745999999999999, SF024_01=1, PhaseBiasBitmaskLen_01=0, SF025_01=60, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.347999999999999, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.347999999999999, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.6539999999999999, CodeBiasBitmaskLen_01=0, SF027_01=60, SF029_01_01=-2.0, SF029_01_02=-0.05999999999999872, SF029_01_03=0.03999999999999915, SF029_01_04=-2.1799999999999997, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF018_02=31, SF020R_02=-0.724000000000002, SF020A_02=-0.3200000000000003, SF020C_02=-0.1180000000000021, SF022_02=7, SF020CK_02=2.0500000000000007, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF025_02=60, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=1.0879999999999974, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=1.0879999999999974, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=0.8999999999999986, CodeBiasBitmaskLen_02=0, SF027_02=60, SF029_02_01=-2.219999999999999, SF029_02_02=-1.3599999999999994, SF029_02_03=-1.5599999999999987, SF029_02_04=-0.28000000000000114, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF018_03=119, SF020R_03=-0.18599999999999994, SF020A_03=1.541999999999998, SF020C_03=0.023999999999997357, SF022_03=7, SF020CK_03=2.6099999999999994, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF025_03=60, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=-0.1440000000000019, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=-0.1440000000000019, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=-0.2959999999999994, CodeBiasBitmaskLen_03=0, SF027_03=60, SF029_03_01=0.3200000000000003, SF029_03_02=2.4800000000000004, SF029_03_03=2.719999999999999, SF029_03_04=0.6799999999999997, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF018_04=27, SF020R_04=0.019999999999999574, SF020A_04=0.04400000000000048, SF020C_04=-0.7100000000000009, SF022_04=7, SF020CK_04=2.8359999999999985, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF025_04=60, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=-0.06800000000000139, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=-0.06800000000000139, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=0.0779999999999994, CodeBiasBitmaskLen_04=0, SF027_04=60, SF029_04_01=-0.17999999999999972, SF029_04_02=1.0599999999999987, SF029_04_03=0.8999999999999986, SF029_04_04=-0.9200000000000017, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF018_05=93, SF020R_05=-0.21199999999999974, SF020A_05=1.6359999999999992, SF020C_05=0.7419999999999973, SF022_05=7, SF020CK_05=-1.0040000000000013, SF024_05=2, PhaseBiasBitmaskLen_05=0, SF025_05=56, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.12599999999999767, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=0.12599999999999767, CodeBiasBitmaskLen_05=0, SF027_05=56, SF029_05_01=-0.379999999999999, SF029_05_02=-1.3000000000000007, SF029_05_03=-1.3599999999999994, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF018_06=50, SF020R_06=-0.12600000000000122, SF020A_06=-3.1560000000000006, SF020C_06=0.6419999999999995, SF022_06=7, SF020CK_06=3.5700000000000003, SF024_06=1, PhaseBiasBitmaskLen_06=0, SF025_06=60, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=0.029999999999997584, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=0.029999999999997584, SF023_06_04=1, SF015_06_04=7, SF020PB_06_04=-0.0400000000000027, CodeBiasBitmaskLen_06=0, SF027_06=60, SF029_06_01=-0.14000000000000057, SF029_06_02=2.0, SF029_06_03=2.0599999999999987, SF029_06_04=0.14000000000000057, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF018_07=51, SF020R_07=0.03200000000000003, SF020A_07=-0.8060000000000009, SF020C_07=0.2940000000000005, SF022_07=7, SF020CK_07=-1.3420000000000005, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF025_07=56, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=0.0259999999999998, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=0.0259999999999998, CodeBiasBitmaskLen_07=0, SF027_07=56, SF029_07_01=-0.9200000000000017, SF029_07_02=-2.039999999999999, SF029_07_03=-1.9800000000000004)>",
-            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=152, eaf=1, crcType=2, frameCrc=2, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=29, authInd=1, embAuthLen=0, crc=1087652, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=3676272, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF019_01=91, SF020R_01=-0.39800000000000146, SF020A_01=-0.3240000000000016, SF020C_01=1.2360000000000007, SF022_01=7, SF020CK_01=0.0, SF024_01=3, PhaseBiasBitmaskLen_01=0, SF026_01=24, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.5479999999999983, CodeBiasBitmaskLen_01=0, SF028_01=24, SF029_01_01=-1.4200000000000017, SF029_01_02=-1.8000000000000007, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF019_02=91, SF020R_02=-0.25800000000000267, SF020A_02=-2.4380000000000006, SF020C_02=0.18999999999999773, SF022_02=7, SF020CK_02=1.8619999999999983, SF024_02=2, PhaseBiasBitmaskLen_02=0, SF026_02=24, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.3279999999999994, CodeBiasBitmaskLen_02=0, SF028_02=24, SF029_02_01=-1.0800000000000018, SF029_02_02=-1.7199999999999989, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF019_03=91, SF020R_03=0.8959999999999972, SF020A_03=2.6720000000000006, SF020C_03=-0.8240000000000016, SF022_03=7, SF020CK_03=1.9699999999999989, SF024_03=2, PhaseBiasBitmaskLen_03=0, SF026_03=24, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.3359999999999985, CodeBiasBitmaskLen_03=0, SF028_03=24, SF029_03_01=-2.0199999999999996, SF029_03_02=-1.9600000000000009, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF019_04=91, SF020R_04=0.6280000000000001, SF020A_04=-4.564000000000002, SF020C_04=1.0479999999999983, SF022_04=7, SF020CK_04=1.9100000000000001, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF026_04=24, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.3539999999999992, CodeBiasBitmaskLen_04=0, SF028_04=24, SF029_04_01=-1.2600000000000016, SF029_04_02=-0.5399999999999991, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF019_05=91, SF020R_05=0.3460000000000001, SF020A_05=-0.10800000000000054, SF020C_05=1.041999999999998, SF022_05=7, SF020CK_05=2.2880000000000003, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF026_05=24, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.3019999999999996, CodeBiasBitmaskLen_05=0, SF028_05=24, SF029_05_01=-0.7600000000000016, SF029_05_02=-0.5800000000000018, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF019_06=91, SF020R_06=0.1720000000000006, SF020A_06=1.6999999999999993, SF020C_06=0.7859999999999978, SF022_06=7, SF020CK_06=-1.758000000000001, SF024_06=3, PhaseBiasBitmaskLen_06=0, SF026_06=24, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=-0.8320000000000007, CodeBiasBitmaskLen_06=0, SF028_06=24, SF029_06_01=2.280000000000001, SF029_06_02=2.84, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF019_07=91, SF020R_07=0.8260000000000005, SF020A_07=1.413999999999998, SF020C_07=-0.008000000000002672, SF022_07=7, SF020CK_07=-0.9300000000000015, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF026_07=24, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.13600000000000279, CodeBiasBitmaskLen_07=0, SF028_07=24, SF029_07_01=0.33999999999999986, SF029_07_02=0.33999999999999986, SF013_08=0, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=7, SF019_08=91, SF020R_08=-0.5500000000000007, SF020A_08=-0.7620000000000005, SF020C_08=2.2439999999999998, SF022_08=7, SF020CK_08=7.327999999999999, SF024_08=2, PhaseBiasBitmaskLen_08=0, SF026_08=24, SF023_08_01=1, SF015_08_01=7, SF020PB_08_01=0.0, SF023_08_02=1, SF015_08_02=7, SF020PB_08_02=0.19599999999999795, CodeBiasBitmaskLen_08=0, SF028_08=24, SF029_08_01=-0.4400000000000013, SF029_08_02=1.4800000000000004)>",
-            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=220, eaf=1, crcType=2, frameCrc=0, msgSubtype=3, timeTagtype=1, gnssTimeTag=451165666, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=61, authInd=1, embAuthLen=0, crc=14343958, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF097=0, SatBitmaskLen=1, SF094=212025376, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF100_01=95, SF020R_01=0.038000000000000256, SF020A_01=0.3099999999999987, SF020C_01=-0.14000000000000057, SF022_01=7, SF020CK_01=2.969999999999999, SF024_01=1, PhaseBiasBitmaskLen_01=0, SF103_01=232, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.46799999999999997, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.4559999999999995, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.0, CodeBiasBitmaskLen_01=0, SF106_01=232, SF029_01_01=-1.379999999999999, SF029_01_02=-2.780000000000001, SF029_01_03=-2.780000000000001, SF029_01_04=-1.379999999999999, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF100_02=95, SF020R_02=-0.10600000000000165, SF020A_02=-0.07400000000000162, SF020C_02=0.16000000000000014, SF022_02=7, SF020CK_02=3.5700000000000003, SF024_02=3, PhaseBiasBitmaskLen_02=0, SF103_02=232, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.8399999999999999, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=0.8200000000000003, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=0.0, CodeBiasBitmaskLen_02=0, SF106_02=232, SF029_02_01=-1.740000000000002, SF029_02_02=-4.120000000000001, SF029_02_03=-4.120000000000001, SF029_02_04=-1.740000000000002, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF100_03=95, SF020R_03=0.04400000000000048, SF020A_03=-0.35400000000000276, SF020C_03=0.3059999999999974, SF022_03=7, SF020CK_03=5.611999999999998, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF103_03=232, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.16399999999999793, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=0.16000000000000014, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=0.0, CodeBiasBitmaskLen_03=0, SF106_03=232, SF029_03_01=-0.17999999999999972, SF029_03_02=-6.280000000000001, SF029_03_03=-6.280000000000001, SF029_03_04=-0.17999999999999972, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF100_04=95, SF020R_04=0.32399999999999807, SF020A_04=-0.4360000000000017, SF020C_04=0.541999999999998, SF022_04=7, SF020CK_04=0.41600000000000037, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF103_04=232, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.5459999999999994, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=0.532, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=0.0, CodeBiasBitmaskLen_04=0, SF106_04=232, SF029_04_01=-2.1999999999999993, SF029_04_02=-4.6, SF029_04_03=-4.6, SF029_04_04=-2.1999999999999993, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF100_05=95, SF020R_05=-0.012000000000000455, SF020A_05=-0.08800000000000097, SF020C_05=0.03399999999999892, SF022_05=7, SF020CK_05=-0.7840000000000007, SF024_05=2, PhaseBiasBitmaskLen_05=0, SF103_05=232, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=-0.04400000000000048, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=-0.04200000000000159, SF023_05_04=1, SF015_05_04=7, SF020PB_05_04=0.0, CodeBiasBitmaskLen_05=0, SF106_05=232, SF029_05_01=0.0799999999999983, SF029_05_02=-2.3200000000000003, SF029_05_03=-2.3200000000000003, SF029_05_04=0.0799999999999983, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF100_06=95, SF020R_06=0.1039999999999992, SF020A_06=-0.31200000000000117, SF020C_06=0.047999999999998266, SF022_06=7, SF020CK_06=-3.6060000000000016, SF024_06=4, PhaseBiasBitmaskLen_06=0, SF103_06=232, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=-0.2920000000000016, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=-0.2840000000000025, SF023_06_04=1, SF015_06_04=7, SF020PB_06_04=0.0, CodeBiasBitmaskLen_06=0, SF106_06=232, SF029_06_01=0.620000000000001, SF029_06_02=1.0, SF029_06_03=1.0, SF029_06_04=0.620000000000001, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF100_07=95, SF020R_07=-0.054000000000002046, SF020A_07=-0.019999999999999574, SF020C_07=-0.028000000000002245, SF022_07=7, SF020CK_07=-1.8980000000000015, SF024_07=2, PhaseBiasBitmaskLen_07=0, SF103_07=232, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=0.6899999999999977, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=0.6720000000000006, SF023_07_04=1, SF015_07_04=7, SF020PB_07_04=0.0, CodeBiasBitmaskLen_07=0, SF106_07=232, SF029_07_01=-0.9600000000000009, SF029_07_02=1.0799999999999983, SF029_07_03=1.0799999999999983, SF029_07_04=-0.9600000000000009, SF013_08=0, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=7, SF100_08=95, SF020R_08=-0.0660000000000025, SF020A_08=0.4079999999999977, SF020C_08=-0.20000000000000284, SF022_08=7, SF020CK_08=-6.618000000000002, SF024_08=3, PhaseBiasBitmaskLen_08=0, SF103_08=232, SF023_08_01=1, SF015_08_01=7, SF020PB_08_01=0.0, SF023_08_02=1, SF015_08_02=7, SF020PB_08_02=1.2739999999999974, SF023_08_03=1, SF015_08_03=7, SF020PB_08_03=1.2419999999999973, SF023_08_04=1, SF015_08_04=7, SF020PB_08_04=0.0, CodeBiasBitmaskLen_08=0, SF106_08=232, SF029_08_01=-2.240000000000002, SF029_08_02=7.699999999999999, SF029_08_03=7.699999999999999, SF029_08_04=-2.240000000000002)>",
-            "<SPARTN(SPARTN-1X-OCB-GAL, msgType=0, nData=191, eaf=1, crcType=2, frameCrc=11, msgSubtype=2, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=29, authInd=1, embAuthLen=0, crc=5207238, SF005=152, SF010=1, SF069=0, SF008=0, SF009=0, SF096=1, SatBitmaskLen=0, SF093=9405731848, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF099_01=56, SF020R_01=0.2699999999999996, SF020A_01=-0.3420000000000023, SF020C_01=-0.11200000000000188, SF022_01=7, SF020CK_01=3.073999999999998, SF024_01=1, PhaseBiasBitmaskLen_01=0, SF102_01=224, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=1.1799999999999997, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=1.0159999999999982, CodeBiasBitmaskLen_01=0, SF105_01=224, SF029_01_01=-2.6000000000000014, SF029_01_02=-1.7199999999999989, SF029_01_03=-1.8599999999999994, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF099_02=58, SF020R_02=0.12199999999999989, SF020A_02=0.08999999999999986, SF020C_02=-0.0400000000000027, SF022_02=7, SF020CK_02=3.727999999999998, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF102_02=224, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.9719999999999978, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=0.8379999999999974, CodeBiasBitmaskLen_02=0, SF105_02=224, SF029_02_01=-2.1400000000000006, SF029_02_02=-0.7800000000000011, SF029_02_03=-0.9200000000000017, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF099_03=58, SF020R_03=0.12399999999999878, SF020A_03=-0.30799999999999983, SF020C_03=0.28800000000000026, SF022_03=7, SF020CK_03=1.9540000000000006, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF102_03=224, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=1.041999999999998, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=0.8140000000000001, CodeBiasBitmaskLen_03=0, SF105_03=224, SF029_03_01=-3.6400000000000006, SF029_03_02=-4.379999999999999, SF029_03_03=-4.440000000000001, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF099_04=58, SF020R_04=-0.02400000000000091, SF020A_04=0.09600000000000009, SF020C_04=0.05999999999999872, SF022_04=7, SF020CK_04=1.7539999999999978, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF102_04=224, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.38599999999999923, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=0.3119999999999976, CodeBiasBitmaskLen_04=0, SF105_04=224, SF029_04_01=-0.4200000000000017, SF029_04_02=1.0, SF029_04_03=0.8999999999999986, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF099_05=58, SF020R_05=0.42799999999999727, SF020A_05=-0.6740000000000013, SF020C_05=0.129999999999999, SF022_05=6, SF020CK_05=3.129999999999999, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF102_05=224, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.08399999999999963, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=0.03599999999999781, CodeBiasBitmaskLen_05=0, SF105_05=224, SF029_05_01=-0.10000000000000142, SF029_05_02=1.4400000000000013, SF029_05_03=1.3399999999999999, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF099_06=58, SF020R_06=0.12399999999999878, SF020A_06=-0.5940000000000012, SF020C_06=0.8840000000000003, SF022_06=7, SF020CK_06=-1.774000000000001, SF024_06=1, PhaseBiasBitmaskLen_06=0, SF102_06=224, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=0.2940000000000005, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=0.16199999999999903, CodeBiasBitmaskLen_06=0, SF105_06=224, SF029_06_01=-0.6400000000000006, SF029_06_02=-1.3599999999999994, SF029_06_03=-1.5800000000000018, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF099_07=58, SF020R_07=-0.1680000000000028, SF020A_07=-0.3520000000000003, SF020C_07=0.07000000000000028, SF022_07=7, SF020CK_07=-2.9240000000000013, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF102_07=224, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.04800000000000182, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=-0.1440000000000019, CodeBiasBitmaskLen_07=0, SF105_07=224, SF029_07_01=0.620000000000001, SF029_07_02=-0.240000000000002, SF029_07_03=-0.33999999999999986, SF013_08=0, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=4, SF099_08=58, SF020R_08=-0.2900000000000027, SF020A_08=-0.03400000000000247, SF020C_08=0.09399999999999764, SF022_08=4, SF020CK_08=-1.9120000000000008, SF024_08=1, PhaseBiasBitmaskLen_08=0, SF102_08=224, SF023_08_01=1, SF015_08_01=4, SF020PB_08_01=0.0, SF023_08_02=1, SF015_08_02=4, SF020PB_08_02=0.07399999999999807, SF023_08_03=1, SF015_08_03=4, SF020PB_08_03=-0.038000000000000256, CodeBiasBitmaskLen_08=0, SF105_08=224, SF029_08_01=-0.120000000000001, SF029_08_02=-0.7600000000000016, SF029_08_03=-0.9200000000000017)>",
-            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=30, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=0, gnssTimeTag=28085, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=39, authInd=1, embAuthLen=0, crc=11321430, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=880836738, SF013_01=0, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=4.745999999999999, SF024_01=1, SF013_02=0, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=2.0500000000000007, SF024_02=1, SF013_03=0, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=2.6099999999999994, SF024_03=1, SF013_04=0, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=2.8359999999999985, SF024_04=1, SF013_05=0, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=-1.0040000000000013, SF024_05=1, SF013_06=0, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=3.5700000000000003, SF024_06=1, SF013_07=0, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-1.3420000000000005, SF024_07=1)>",
-            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=33, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=0, gnssTimeTag=38867, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=517021, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=3676272, SF013_01=0, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=0.0, SF024_01=2, SF013_02=0, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=1.8619999999999983, SF024_02=1, SF013_03=0, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=1.9699999999999989, SF024_03=2, SF013_04=0, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=1.9100000000000001, SF024_04=1, SF013_05=0, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=2.2880000000000003, SF024_05=1, SF013_06=0, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=-1.758000000000001, SF024_06=3, SF013_07=0, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-0.9300000000000015, SF024_07=2, SF013_08=0, SF014O_08=0, SF014C_08=1, SF014B_08=0, SF015_08=7, SF022_08=7, SF020CK_08=7.327999999999999, SF024_08=2)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=30, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=0, gnssTimeTag=28075, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=37, authInd=1, embAuthLen=0, crc=4342523, SF005=151, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=880836738, SF013_01=0, PRN_01=3, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=4.727999999999998, SF024_01=1, SF013_02=0, PRN_02=4, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=2.0459999999999994, SF024_02=1, SF013_03=0, PRN_03=6, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=2.622, SF024_03=1, SF013_04=0, PRN_04=9, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=2.823999999999998, SF024_04=1, SF013_05=0, PRN_05=17, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=-1.0020000000000007, SF024_05=2, SF013_06=0, PRN_06=25, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=3.6099999999999994, SF024_06=1, SF013_07=0, PRN_07=31, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-1.3600000000000012, SF024_07=1)>",
+            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=33, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=0, gnssTimeTag=38857, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=28, authInd=1, embAuthLen=0, crc=4143853, SF005=151, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=3676272, SF013_01=0, PRN_01=3, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=-0.0259999999999998, SF024_01=3, SF013_02=0, PRN_02=4, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=1.8780000000000001, SF024_02=2, SF013_03=0, PRN_03=5, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=1.9819999999999993, SF024_03=2, SF013_04=0, PRN_04=12, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=1.9279999999999973, SF024_04=2, SF013_05=0, PRN_05=13, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=2.2959999999999994, SF024_05=1, SF013_06=0, PRN_06=18, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=-1.7960000000000012, SF024_06=3, SF013_07=0, PRN_07=19, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-0.8880000000000017, SF024_07=2, SF013_08=0, PRN_08=20, SF014O_08=0, SF014C_08=1, SF014B_08=0, SF015_08=7, SF022_08=7, SF020CK_08=7.311999999999998, SF024_08=1)>",
+            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=36, eaf=1, crcType=2, frameCrc=11, msgSubtype=3, timeTagtype=0, gnssTimeTag=28061, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=60, authInd=1, embAuthLen=0, crc=13197342, SF005=151, SF010=0, SF069=0, SF008=0, SF009=0, SF097=0, SatBitmaskLen=1, SF094=212025376, SF013_01=0, PRN_01=19, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=2.849999999999998, SF024_01=1, SF013_02=0, PRN_02=20, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=3.565999999999999, SF024_02=3, SF013_03=0, PRN_03=23, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=5.654, SF024_03=1, SF013_04=0, PRN_04=25, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=0.39000000000000057, SF024_04=1, SF013_05=0, PRN_05=29, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=-0.8080000000000016, SF024_05=2, SF013_06=0, PRN_06=30, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=-3.612000000000002, SF024_06=4, SF013_07=0, PRN_07=32, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-1.9200000000000017, SF024_07=2, SF013_08=0, PRN_08=41, SF014O_08=0, SF014C_08=1, SF014B_08=0, SF015_08=7, SF022_08=7, SF020CK_08=-6.6800000000000015, SF024_08=4)>",
+            "<SPARTN(SPARTN-1X-OCB-GAL, msgType=0, nData=34, eaf=1, crcType=2, frameCrc=3, msgSubtype=2, timeTagtype=0, gnssTimeTag=28075, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=28, authInd=1, embAuthLen=0, crc=5329954, SF005=151, SF010=1, SF069=0, SF008=0, SF009=0, SF096=1, SatBitmaskLen=0, SF093=9405731848, SF013_01=0, PRN_01=3, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=3.0700000000000003, SF024_01=1, SF013_02=0, PRN_02=7, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=3.724, SF024_02=1, SF013_03=0, PRN_03=8, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=1.9499999999999993, SF024_03=1, SF013_04=0, PRN_04=13, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=1.7680000000000007, SF024_04=1, SF013_05=0, PRN_05=15, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=6, SF020CK_05=3.1419999999999995, SF024_05=1, SF013_06=0, PRN_06=24, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=-1.7940000000000005, SF024_06=1, SF013_07=0, PRN_07=26, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-2.902000000000001, SF024_07=1, SF013_08=0, PRN_08=33, SF014O_08=0, SF014C_08=1, SF014B_08=0, SF015_08=3, SF022_08=3, SF020CK_08=-1.886000000000001, SF024_08=1)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=180, eaf=1, crcType=2, frameCrc=9, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=38, authInd=1, embAuthLen=0, crc=11341296, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=880836738, SF013_01=0, PRN_01=3, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF018_01=47, SF020R_01=0.0259999999999998, SF020A_01=0.597999999999999, SF020C_01=0.31799999999999784, SF022_01=7, SF020CK_01=4.745999999999999, SF024_01=1, PhaseBiasBitmaskLen_01=0, SF025_01=60, PhaseBias_01_01=L1C, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, PhaseBias_01_02=L2W, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.347999999999999, PhaseBias_01_03=L2L, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.347999999999999, PhaseBias_01_04=L5Q, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.6539999999999999, CodeBiasBitmaskLen_01=0, SF027_01=60, CodeBias_01_01=C1C, SF029_01_01=-2.0, CodeBias_01_02=C2W, SF029_01_02=-0.05999999999999872, CodeBias_01_03=C2L, SF029_01_03=0.03999999999999915, CodeBias_01_04=C5Q, SF029_01_04=-2.1799999999999997, SF013_02=0, PRN_02=4, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF018_02=31, SF020R_02=-0.724000000000002, SF020A_02=-0.3200000000000003, SF020C_02=-0.1180000000000021, SF022_02=7, SF020CK_02=2.0500000000000007, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF025_02=60, PhaseBias_02_01=L1C, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, PhaseBias_02_02=L2W, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=1.0879999999999974, PhaseBias_02_03=L2L, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=1.0879999999999974, PhaseBias_02_04=L5Q, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=0.8999999999999986, CodeBiasBitmaskLen_02=0, SF027_02=60, CodeBias_02_01=C1C, SF029_02_01=-2.219999999999999, CodeBias_02_02=C2W, SF029_02_02=-1.3599999999999994, CodeBias_02_03=C2L, SF029_02_03=-1.5599999999999987, CodeBias_02_04=C5Q, SF029_02_04=-0.28000000000000114, SF013_03=0, PRN_03=6, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF018_03=119, SF020R_03=-0.18599999999999994, SF020A_03=1.541999999999998, SF020C_03=0.023999999999997357, SF022_03=7, SF020CK_03=2.6099999999999994, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF025_03=60, PhaseBias_03_01=L1C, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, PhaseBias_03_02=L2W, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=-0.1440000000000019, PhaseBias_03_03=L2L, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=-0.1440000000000019, PhaseBias_03_04=L5Q, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=-0.2959999999999994, CodeBiasBitmaskLen_03=0, SF027_03=60, CodeBias_03_01=C1C, SF029_03_01=0.3200000000000003, CodeBias_03_02=C2W, SF029_03_02=2.4800000000000004, CodeBias_03_03=C2L, SF029_03_03=2.719999999999999, CodeBias_03_04=C5Q, SF029_03_04=0.6799999999999997, SF013_04=0, PRN_04=9, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF018_04=27, SF020R_04=0.019999999999999574, SF020A_04=0.04400000000000048, SF020C_04=-0.7100000000000009, SF022_04=7, SF020CK_04=2.8359999999999985, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF025_04=60, PhaseBias_04_01=L1C, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, PhaseBias_04_02=L2W, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=-0.06800000000000139, PhaseBias_04_03=L2L, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=-0.06800000000000139, PhaseBias_04_04=L5Q, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=0.0779999999999994, CodeBiasBitmaskLen_04=0, SF027_04=60, CodeBias_04_01=C1C, SF029_04_01=-0.17999999999999972, CodeBias_04_02=C2W, SF029_04_02=1.0599999999999987, CodeBias_04_03=C2L, SF029_04_03=0.8999999999999986, CodeBias_04_04=C5Q, SF029_04_04=-0.9200000000000017, SF013_05=0, PRN_05=17, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF018_05=93, SF020R_05=-0.21199999999999974, SF020A_05=1.6359999999999992, SF020C_05=0.7419999999999973, SF022_05=7, SF020CK_05=-1.0040000000000013, SF024_05=2, PhaseBiasBitmaskLen_05=0, SF025_05=56, PhaseBias_05_01=L1C, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, PhaseBias_05_02=L2W, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.12599999999999767, PhaseBias_05_03=L2L, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=0.12599999999999767, CodeBiasBitmaskLen_05=0, SF027_05=56, CodeBias_05_01=C1C, SF029_05_01=-0.379999999999999, CodeBias_05_02=C2W, SF029_05_02=-1.3000000000000007, CodeBias_05_03=C2L, SF029_05_03=-1.3599999999999994, SF013_06=0, PRN_06=25, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF018_06=50, SF020R_06=-0.12600000000000122, SF020A_06=-3.1560000000000006, SF020C_06=0.6419999999999995, SF022_06=7, SF020CK_06=3.5700000000000003, SF024_06=1, PhaseBiasBitmaskLen_06=0, SF025_06=60, PhaseBias_06_01=L1C, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, PhaseBias_06_02=L2W, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=0.029999999999997584, PhaseBias_06_03=L2L, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=0.029999999999997584, PhaseBias_06_04=L5Q, SF023_06_04=1, SF015_06_04=7, SF020PB_06_04=-0.0400000000000027, CodeBiasBitmaskLen_06=0, SF027_06=60, CodeBias_06_01=C1C, SF029_06_01=-0.14000000000000057, CodeBias_06_02=C2W, SF029_06_02=2.0, CodeBias_06_03=C2L, SF029_06_03=2.0599999999999987, CodeBias_06_04=C5Q, SF029_06_04=0.14000000000000057, SF013_07=0, PRN_07=31, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF018_07=51, SF020R_07=0.03200000000000003, SF020A_07=-0.8060000000000009, SF020C_07=0.2940000000000005, SF022_07=7, SF020CK_07=-1.3420000000000005, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF025_07=56, PhaseBias_07_01=L1C, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, PhaseBias_07_02=L2W, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=0.0259999999999998, PhaseBias_07_03=L2L, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=0.0259999999999998, CodeBiasBitmaskLen_07=0, SF027_07=56, CodeBias_07_01=C1C, SF029_07_01=-0.9200000000000017, CodeBias_07_02=C2W, SF029_07_02=-2.039999999999999, CodeBias_07_03=C2L, SF029_07_03=-1.9800000000000004)>",
+            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=152, eaf=1, crcType=2, frameCrc=2, msgSubtype=1, timeTagtype=1, gnssTimeTag=451176462, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=29, authInd=1, embAuthLen=0, crc=1087652, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=3676272, SF013_01=0, PRN_01=3, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF019_01=91, SF020R_01=-0.39800000000000146, SF020A_01=-0.3240000000000016, SF020C_01=1.2360000000000007, SF022_01=7, SF020CK_01=0.0, SF024_01=3, PhaseBiasBitmaskLen_01=0, SF026_01=24, PhaseBias_01_01=L1C, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, PhaseBias_01_02=L2C, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.5479999999999983, CodeBiasBitmaskLen_01=0, SF028_01=24, CodeBias_01_01=C1C, SF029_01_01=-1.4200000000000017, CodeBias_01_02=C2C, SF029_01_02=-1.8000000000000007, SF013_02=0, PRN_02=4, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF019_02=91, SF020R_02=-0.25800000000000267, SF020A_02=-2.4380000000000006, SF020C_02=0.18999999999999773, SF022_02=7, SF020CK_02=1.8619999999999983, SF024_02=2, PhaseBiasBitmaskLen_02=0, SF026_02=24, PhaseBias_02_01=L1C, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, PhaseBias_02_02=L2C, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.3279999999999994, CodeBiasBitmaskLen_02=0, SF028_02=24, CodeBias_02_01=C1C, SF029_02_01=-1.0800000000000018, CodeBias_02_02=C2C, SF029_02_02=-1.7199999999999989, SF013_03=0, PRN_03=5, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF019_03=91, SF020R_03=0.8959999999999972, SF020A_03=2.6720000000000006, SF020C_03=-0.8240000000000016, SF022_03=7, SF020CK_03=1.9699999999999989, SF024_03=2, PhaseBiasBitmaskLen_03=0, SF026_03=24, PhaseBias_03_01=L1C, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, PhaseBias_03_02=L2C, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.3359999999999985, CodeBiasBitmaskLen_03=0, SF028_03=24, CodeBias_03_01=C1C, SF029_03_01=-2.0199999999999996, CodeBias_03_02=C2C, SF029_03_02=-1.9600000000000009, SF013_04=0, PRN_04=12, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF019_04=91, SF020R_04=0.6280000000000001, SF020A_04=-4.564000000000002, SF020C_04=1.0479999999999983, SF022_04=7, SF020CK_04=1.9100000000000001, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF026_04=24, PhaseBias_04_01=L1C, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, PhaseBias_04_02=L2C, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.3539999999999992, CodeBiasBitmaskLen_04=0, SF028_04=24, CodeBias_04_01=C1C, SF029_04_01=-1.2600000000000016, CodeBias_04_02=C2C, SF029_04_02=-0.5399999999999991, SF013_05=0, PRN_05=13, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF019_05=91, SF020R_05=0.3460000000000001, SF020A_05=-0.10800000000000054, SF020C_05=1.041999999999998, SF022_05=7, SF020CK_05=2.2880000000000003, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF026_05=24, PhaseBias_05_01=L1C, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, PhaseBias_05_02=L2C, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.3019999999999996, CodeBiasBitmaskLen_05=0, SF028_05=24, CodeBias_05_01=C1C, SF029_05_01=-0.7600000000000016, CodeBias_05_02=C2C, SF029_05_02=-0.5800000000000018, SF013_06=0, PRN_06=18, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF019_06=91, SF020R_06=0.1720000000000006, SF020A_06=1.6999999999999993, SF020C_06=0.7859999999999978, SF022_06=7, SF020CK_06=-1.758000000000001, SF024_06=3, PhaseBiasBitmaskLen_06=0, SF026_06=24, PhaseBias_06_01=L1C, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, PhaseBias_06_02=L2C, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=-0.8320000000000007, CodeBiasBitmaskLen_06=0, SF028_06=24, CodeBias_06_01=C1C, SF029_06_01=2.280000000000001, CodeBias_06_02=C2C, SF029_06_02=2.84, SF013_07=0, PRN_07=19, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF019_07=91, SF020R_07=0.8260000000000005, SF020A_07=1.413999999999998, SF020C_07=-0.008000000000002672, SF022_07=7, SF020CK_07=-0.9300000000000015, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF026_07=24, PhaseBias_07_01=L1C, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, PhaseBias_07_02=L2C, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.13600000000000279, CodeBiasBitmaskLen_07=0, SF028_07=24, CodeBias_07_01=C1C, SF029_07_01=0.33999999999999986, CodeBias_07_02=C2C, SF029_07_02=0.33999999999999986, SF013_08=0, PRN_08=20, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=7, SF019_08=91, SF020R_08=-0.5500000000000007, SF020A_08=-0.7620000000000005, SF020C_08=2.2439999999999998, SF022_08=7, SF020CK_08=7.327999999999999, SF024_08=2, PhaseBiasBitmaskLen_08=0, SF026_08=24, PhaseBias_08_01=L1C, SF023_08_01=1, SF015_08_01=7, SF020PB_08_01=0.0, PhaseBias_08_02=L2C, SF023_08_02=1, SF015_08_02=7, SF020PB_08_02=0.19599999999999795, CodeBiasBitmaskLen_08=0, SF028_08=24, CodeBias_08_01=C1C, SF029_08_01=-0.4400000000000013, CodeBias_08_02=C2C, SF029_08_02=1.4800000000000004)>",
+            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=220, eaf=1, crcType=2, frameCrc=0, msgSubtype=3, timeTagtype=1, gnssTimeTag=451165666, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=61, authInd=1, embAuthLen=0, crc=14343958, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF097=0, SatBitmaskLen=1, SF094=212025376, SF013_01=0, PRN_01=19, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF100_01=95, SF020R_01=0.038000000000000256, SF020A_01=0.3099999999999987, SF020C_01=-0.14000000000000057, SF022_01=7, SF020CK_01=2.969999999999999, SF024_01=1, PhaseBiasBitmaskLen_01=0, SF103_01=232, PhaseBias_01_01=L2I, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, PhaseBias_01_02=L5P, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.46799999999999997, PhaseBias_01_03=L7I, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.4559999999999995, PhaseBias_01_04=L1P, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.0, CodeBiasBitmaskLen_01=0, SF106_01=232, CodeBias_01_01=C2I, SF029_01_01=-1.379999999999999, CodeBias_01_02=C5P, SF029_01_02=-2.780000000000001, CodeBias_01_03=C7I, SF029_01_03=-2.780000000000001, CodeBias_01_04=C1P, SF029_01_04=-1.379999999999999, SF013_02=0, PRN_02=20, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF100_02=95, SF020R_02=-0.10600000000000165, SF020A_02=-0.07400000000000162, SF020C_02=0.16000000000000014, SF022_02=7, SF020CK_02=3.5700000000000003, SF024_02=3, PhaseBiasBitmaskLen_02=0, SF103_02=232, PhaseBias_02_01=L2I, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, PhaseBias_02_02=L5P, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.8399999999999999, PhaseBias_02_03=L7I, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=0.8200000000000003, PhaseBias_02_04=L1P, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=0.0, CodeBiasBitmaskLen_02=0, SF106_02=232, CodeBias_02_01=C2I, SF029_02_01=-1.740000000000002, CodeBias_02_02=C5P, SF029_02_02=-4.120000000000001, CodeBias_02_03=C7I, SF029_02_03=-4.120000000000001, CodeBias_02_04=C1P, SF029_02_04=-1.740000000000002, SF013_03=0, PRN_03=23, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF100_03=95, SF020R_03=0.04400000000000048, SF020A_03=-0.35400000000000276, SF020C_03=0.3059999999999974, SF022_03=7, SF020CK_03=5.611999999999998, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF103_03=232, PhaseBias_03_01=L2I, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, PhaseBias_03_02=L5P, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.16399999999999793, PhaseBias_03_03=L7I, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=0.16000000000000014, PhaseBias_03_04=L1P, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=0.0, CodeBiasBitmaskLen_03=0, SF106_03=232, CodeBias_03_01=C2I, SF029_03_01=-0.17999999999999972, CodeBias_03_02=C5P, SF029_03_02=-6.280000000000001, CodeBias_03_03=C7I, SF029_03_03=-6.280000000000001, CodeBias_03_04=C1P, SF029_03_04=-0.17999999999999972, SF013_04=0, PRN_04=25, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF100_04=95, SF020R_04=0.32399999999999807, SF020A_04=-0.4360000000000017, SF020C_04=0.541999999999998, SF022_04=7, SF020CK_04=0.41600000000000037, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF103_04=232, PhaseBias_04_01=L2I, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, PhaseBias_04_02=L5P, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.5459999999999994, PhaseBias_04_03=L7I, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=0.532, PhaseBias_04_04=L1P, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=0.0, CodeBiasBitmaskLen_04=0, SF106_04=232, CodeBias_04_01=C2I, SF029_04_01=-2.1999999999999993, CodeBias_04_02=C5P, SF029_04_02=-4.6, CodeBias_04_03=C7I, SF029_04_03=-4.6, CodeBias_04_04=C1P, SF029_04_04=-2.1999999999999993, SF013_05=0, PRN_05=29, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF100_05=95, SF020R_05=-0.012000000000000455, SF020A_05=-0.08800000000000097, SF020C_05=0.03399999999999892, SF022_05=7, SF020CK_05=-0.7840000000000007, SF024_05=2, PhaseBiasBitmaskLen_05=0, SF103_05=232, PhaseBias_05_01=L2I, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, PhaseBias_05_02=L5P, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=-0.04400000000000048, PhaseBias_05_03=L7I, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=-0.04200000000000159, PhaseBias_05_04=L1P, SF023_05_04=1, SF015_05_04=7, SF020PB_05_04=0.0, CodeBiasBitmaskLen_05=0, SF106_05=232, CodeBias_05_01=C2I, SF029_05_01=0.0799999999999983, CodeBias_05_02=C5P, SF029_05_02=-2.3200000000000003, CodeBias_05_03=C7I, SF029_05_03=-2.3200000000000003, CodeBias_05_04=C1P, SF029_05_04=0.0799999999999983, SF013_06=0, PRN_06=30, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF100_06=95, SF020R_06=0.1039999999999992, SF020A_06=-0.31200000000000117, SF020C_06=0.047999999999998266, SF022_06=7, SF020CK_06=-3.6060000000000016, SF024_06=4, PhaseBiasBitmaskLen_06=0, SF103_06=232, PhaseBias_06_01=L2I, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, PhaseBias_06_02=L5P, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=-0.2920000000000016, PhaseBias_06_03=L7I, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=-0.2840000000000025, PhaseBias_06_04=L1P, SF023_06_04=1, SF015_06_04=7, SF020PB_06_04=0.0, CodeBiasBitmaskLen_06=0, SF106_06=232, CodeBias_06_01=C2I, SF029_06_01=0.620000000000001, CodeBias_06_02=C5P, SF029_06_02=1.0, CodeBias_06_03=C7I, SF029_06_03=1.0, CodeBias_06_04=C1P, SF029_06_04=0.620000000000001, SF013_07=0, PRN_07=32, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF100_07=95, SF020R_07=-0.054000000000002046, SF020A_07=-0.019999999999999574, SF020C_07=-0.028000000000002245, SF022_07=7, SF020CK_07=-1.8980000000000015, SF024_07=2, PhaseBiasBitmaskLen_07=0, SF103_07=232, PhaseBias_07_01=L2I, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, PhaseBias_07_02=L5P, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=0.6899999999999977, PhaseBias_07_03=L7I, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=0.6720000000000006, PhaseBias_07_04=L1P, SF023_07_04=1, SF015_07_04=7, SF020PB_07_04=0.0, CodeBiasBitmaskLen_07=0, SF106_07=232, CodeBias_07_01=C2I, SF029_07_01=-0.9600000000000009, CodeBias_07_02=C5P, SF029_07_02=1.0799999999999983, CodeBias_07_03=C7I, SF029_07_03=1.0799999999999983, CodeBias_07_04=C1P, SF029_07_04=-0.9600000000000009, SF013_08=0, PRN_08=41, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=7, SF100_08=95, SF020R_08=-0.0660000000000025, SF020A_08=0.4079999999999977, SF020C_08=-0.20000000000000284, SF022_08=7, SF020CK_08=-6.618000000000002, SF024_08=3, PhaseBiasBitmaskLen_08=0, SF103_08=232, PhaseBias_08_01=L2I, SF023_08_01=1, SF015_08_01=7, SF020PB_08_01=0.0, PhaseBias_08_02=L5P, SF023_08_02=1, SF015_08_02=7, SF020PB_08_02=1.2739999999999974, PhaseBias_08_03=L7I, SF023_08_03=1, SF015_08_03=7, SF020PB_08_03=1.2419999999999973, PhaseBias_08_04=L1P, SF023_08_04=1, SF015_08_04=7, SF020PB_08_04=0.0, CodeBiasBitmaskLen_08=0, SF106_08=232, CodeBias_08_01=C2I, SF029_08_01=-2.240000000000002, CodeBias_08_02=C5P, SF029_08_02=7.699999999999999, CodeBias_08_03=C7I, SF029_08_03=7.699999999999999, CodeBias_08_04=C1P, SF029_08_04=-2.240000000000002)>",
+            "<SPARTN(SPARTN-1X-OCB-GAL, msgType=0, nData=191, eaf=1, crcType=2, frameCrc=11, msgSubtype=2, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=29, authInd=1, embAuthLen=0, crc=5207238, SF005=152, SF010=1, SF069=0, SF008=0, SF009=0, SF096=1, SatBitmaskLen=0, SF093=9405731848, SF013_01=0, PRN_01=3, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF099_01=56, SF020R_01=0.2699999999999996, SF020A_01=-0.3420000000000023, SF020C_01=-0.11200000000000188, SF022_01=7, SF020CK_01=3.073999999999998, SF024_01=1, PhaseBiasBitmaskLen_01=0, SF102_01=224, PhaseBias_01_01=L1C, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, PhaseBias_01_02=L5Q, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=1.1799999999999997, PhaseBias_01_03=L7Q, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=1.0159999999999982, CodeBiasBitmaskLen_01=0, SF105_01=224, CodeBias_01_01=C1C, SF029_01_01=-2.6000000000000014, CodeBias_01_02=C5Q, SF029_01_02=-1.7199999999999989, CodeBias_01_03=C7Q, SF029_01_03=-1.8599999999999994, SF013_02=0, PRN_02=7, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF099_02=58, SF020R_02=0.12199999999999989, SF020A_02=0.08999999999999986, SF020C_02=-0.0400000000000027, SF022_02=7, SF020CK_02=3.727999999999998, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF102_02=224, PhaseBias_02_01=L1C, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, PhaseBias_02_02=L5Q, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.9719999999999978, PhaseBias_02_03=L7Q, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=0.8379999999999974, CodeBiasBitmaskLen_02=0, SF105_02=224, CodeBias_02_01=C1C, SF029_02_01=-2.1400000000000006, CodeBias_02_02=C5Q, SF029_02_02=-0.7800000000000011, CodeBias_02_03=C7Q, SF029_02_03=-0.9200000000000017, SF013_03=0, PRN_03=8, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF099_03=58, SF020R_03=0.12399999999999878, SF020A_03=-0.30799999999999983, SF020C_03=0.28800000000000026, SF022_03=7, SF020CK_03=1.9540000000000006, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF102_03=224, PhaseBias_03_01=L1C, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, PhaseBias_03_02=L5Q, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=1.041999999999998, PhaseBias_03_03=L7Q, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=0.8140000000000001, CodeBiasBitmaskLen_03=0, SF105_03=224, CodeBias_03_01=C1C, SF029_03_01=-3.6400000000000006, CodeBias_03_02=C5Q, SF029_03_02=-4.379999999999999, CodeBias_03_03=C7Q, SF029_03_03=-4.440000000000001, SF013_04=0, PRN_04=13, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF099_04=58, SF020R_04=-0.02400000000000091, SF020A_04=0.09600000000000009, SF020C_04=0.05999999999999872, SF022_04=7, SF020CK_04=1.7539999999999978, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF102_04=224, PhaseBias_04_01=L1C, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, PhaseBias_04_02=L5Q, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.38599999999999923, PhaseBias_04_03=L7Q, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=0.3119999999999976, CodeBiasBitmaskLen_04=0, SF105_04=224, CodeBias_04_01=C1C, SF029_04_01=-0.4200000000000017, CodeBias_04_02=C5Q, SF029_04_02=1.0, CodeBias_04_03=C7Q, SF029_04_03=0.8999999999999986, SF013_05=0, PRN_05=15, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF099_05=58, SF020R_05=0.42799999999999727, SF020A_05=-0.6740000000000013, SF020C_05=0.129999999999999, SF022_05=6, SF020CK_05=3.129999999999999, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF102_05=224, PhaseBias_05_01=L1C, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, PhaseBias_05_02=L5Q, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.08399999999999963, PhaseBias_05_03=L7Q, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=0.03599999999999781, CodeBiasBitmaskLen_05=0, SF105_05=224, CodeBias_05_01=C1C, SF029_05_01=-0.10000000000000142, CodeBias_05_02=C5Q, SF029_05_02=1.4400000000000013, CodeBias_05_03=C7Q, SF029_05_03=1.3399999999999999, SF013_06=0, PRN_06=24, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF099_06=58, SF020R_06=0.12399999999999878, SF020A_06=-0.5940000000000012, SF020C_06=0.8840000000000003, SF022_06=7, SF020CK_06=-1.774000000000001, SF024_06=1, PhaseBiasBitmaskLen_06=0, SF102_06=224, PhaseBias_06_01=L1C, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, PhaseBias_06_02=L5Q, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=0.2940000000000005, PhaseBias_06_03=L7Q, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=0.16199999999999903, CodeBiasBitmaskLen_06=0, SF105_06=224, CodeBias_06_01=C1C, SF029_06_01=-0.6400000000000006, CodeBias_06_02=C5Q, SF029_06_02=-1.3599999999999994, CodeBias_06_03=C7Q, SF029_06_03=-1.5800000000000018, SF013_07=0, PRN_07=26, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF099_07=58, SF020R_07=-0.1680000000000028, SF020A_07=-0.3520000000000003, SF020C_07=0.07000000000000028, SF022_07=7, SF020CK_07=-2.9240000000000013, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF102_07=224, PhaseBias_07_01=L1C, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, PhaseBias_07_02=L5Q, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.04800000000000182, PhaseBias_07_03=L7Q, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=-0.1440000000000019, CodeBiasBitmaskLen_07=0, SF105_07=224, CodeBias_07_01=C1C, SF029_07_01=0.620000000000001, CodeBias_07_02=C5Q, SF029_07_02=-0.240000000000002, CodeBias_07_03=C7Q, SF029_07_03=-0.33999999999999986, SF013_08=0, PRN_08=33, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=4, SF099_08=58, SF020R_08=-0.2900000000000027, SF020A_08=-0.03400000000000247, SF020C_08=0.09399999999999764, SF022_08=4, SF020CK_08=-1.9120000000000008, SF024_08=1, PhaseBiasBitmaskLen_08=0, SF102_08=224, PhaseBias_08_01=L1C, SF023_08_01=1, SF015_08_01=4, SF020PB_08_01=0.0, PhaseBias_08_02=L5Q, SF023_08_02=1, SF015_08_02=4, SF020PB_08_02=0.07399999999999807, PhaseBias_08_03=L7Q, SF023_08_03=1, SF015_08_03=4, SF020PB_08_03=-0.038000000000000256, CodeBiasBitmaskLen_08=0, SF105_08=224, CodeBias_08_01=C1C, SF029_08_01=-0.120000000000001, CodeBias_08_02=C5Q, SF029_08_02=-0.7600000000000016, CodeBias_08_03=C7Q, SF029_08_03=-0.9200000000000017)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=30, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=0, gnssTimeTag=28085, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=39, authInd=1, embAuthLen=0, crc=11321430, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=880836738, SF013_01=0, PRN_01=3, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=4.745999999999999, SF024_01=1, SF013_02=0, PRN_02=4, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=2.0500000000000007, SF024_02=1, SF013_03=0, PRN_03=6, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=2.6099999999999994, SF024_03=1, SF013_04=0, PRN_04=9, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=2.8359999999999985, SF024_04=1, SF013_05=0, PRN_05=17, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=-1.0040000000000013, SF024_05=1, SF013_06=0, PRN_06=25, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=3.5700000000000003, SF024_06=1, SF013_07=0, PRN_07=31, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-1.3420000000000005, SF024_07=1)>",
+            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=33, eaf=1, crcType=2, frameCrc=3, msgSubtype=1, timeTagtype=0, gnssTimeTag=38867, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=517021, SF005=152, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=3676272, SF013_01=0, PRN_01=3, SF014O_01=0, SF014C_01=1, SF014B_01=0, SF015_01=7, SF022_01=7, SF020CK_01=0.0, SF024_01=2, SF013_02=0, PRN_02=4, SF014O_02=0, SF014C_02=1, SF014B_02=0, SF015_02=7, SF022_02=7, SF020CK_02=1.8619999999999983, SF024_02=1, SF013_03=0, PRN_03=5, SF014O_03=0, SF014C_03=1, SF014B_03=0, SF015_03=7, SF022_03=7, SF020CK_03=1.9699999999999989, SF024_03=2, SF013_04=0, PRN_04=12, SF014O_04=0, SF014C_04=1, SF014B_04=0, SF015_04=7, SF022_04=7, SF020CK_04=1.9100000000000001, SF024_04=1, SF013_05=0, PRN_05=13, SF014O_05=0, SF014C_05=1, SF014B_05=0, SF015_05=7, SF022_05=7, SF020CK_05=2.2880000000000003, SF024_05=1, SF013_06=0, PRN_06=18, SF014O_06=0, SF014C_06=1, SF014B_06=0, SF015_06=7, SF022_06=7, SF020CK_06=-1.758000000000001, SF024_06=3, SF013_07=0, PRN_07=19, SF014O_07=0, SF014C_07=1, SF014B_07=0, SF015_07=7, SF022_07=7, SF020CK_07=-0.9300000000000015, SF024_07=2, SF013_08=0, PRN_08=20, SF014O_08=0, SF014C_08=1, SF014B_08=0, SF015_08=7, SF022_08=7, SF020CK_08=7.327999999999999, SF024_08=2)>",
         )
 
         # test using datetime as basedate
         i = 0
         with open(os.path.join(self.dirname, "spartnOCB.log"), "rb") as stream:
             spr = SPARTNReader(
                 stream,
@@ -343,39 +434,39 @@
             "rb",
         ) as stream:
             spr = SPARTNReader(
                 stream,
                 quitonerror=ERRRAISE,
                 decode=True,
                 key="930d847b779b126863c8b3b2766ae7cc",
-                basedate=datetime(2024, 4, 28, 23, 50, 40),
+                basedate=datetime(2024, 4, 28, 23, 50, 40, tzinfo=timezone.utc),
             )
 
             for raw, parsed in spr:
                 i += 1
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertTrue(0 <= parsed._padding <= 8)
 
         self.assertEqual(i, 99)
 
     def testspartnntrip(
         self,
     ):  # test decryption of datastream from SPARTN NTRIP caster containing unencrypted messages (eaf=0)
         EXPECTED_RESULT = [
-            "<SPARTN(SPARTN-1X-HPAC-BEI, msgType=1, nData=369, eaf=0, crcType=2, frameCrc=14, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=4347676, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.16800000000000004, SF049a_01=-0.0010000000000000009, SF049b_01=-0.015999999999999986, SF054_01=1, SatBitmaskLen_01=0, SF094_01=32768, SF055_01_01=1, SF056_01_01=1, SF060_01_01=8.960000000000036, SF061a_01_01=0.1599999999999966, SF061b_01_01=0.3999999999999915, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.10399999999999998, SF049a_02=0.0020000000000000018, SF049b_02=0.007000000000000006, SF054_02=1, SatBitmaskLen_02=1, SF094_02=184554500, SF055_02_01=3, SF056_02_01=1, SF060_02_01=9.800000000000011, SF061a_02_01=-0.38400000000000034, SF061b_02_01=-0.4399999999999977, SF055_02_02=4, SF056_02_02=1, SF060_02_02=28.480000000000018, SF061a_02_02=-0.4720000000000084, SF061b_02_02=0.37599999999999056, SF055_02_03=3, SF056_02_03=1, SF060_02_03=3.5200000000000387, SF061a_02_03=-0.24800000000000466, SF061b_02_03=0.0799999999999983, SF055_02_04=4, SF056_02_04=1, SF060_02_04=27.640000000000043, SF061a_02_04=-1.0080000000000098, SF061b_02_04=0.3359999999999985, SF055_02_05=2, SF056_02_05=1, SF060_02_05=22.319999999999993, SF061a_02_05=0.37599999999999056, SF061b_02_05=-0.6080000000000041, SF055_02_06=4, SF056_02_06=1, SF060_02_06=15.760000000000048, SF061a_02_06=0.1039999999999992, SF061b_02_06=0.22399999999998954, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.09599999999999997, SF049a_03=-0.033, SF049b_03=-0.009000000000000008, SF054_03=1, SatBitmaskLen_03=1, SF094_03=184550404, SF055_03_01=1, SF056_03_01=1, SF060_03_01=7.28000000000003, SF061a_03_01=-0.4480000000000075, SF061b_03_01=-0.26400000000001, SF055_03_02=5, SF056_03_02=1, SF060_03_02=30.52000000000004, SF061a_03_02=0.07199999999998852, SF061b_03_02=0.30400000000000205, SF055_03_03=1, SF056_03_03=1, SF060_03_03=3.5600000000000023, SF061a_03_03=-0.0799999999999983, SF061b_03_03=-0.03200000000001069, SF055_03_04=2, SF056_03_04=1, SF060_03_04=17.319999999999993, SF061a_03_04=0.30400000000000205, SF061b_03_04=-0.6159999999999997, SF055_03_05=1, SF056_03_05=1, SF060_03_05=17.760000000000048, SF061a_03_05=0.28000000000000114, SF061b_03_05=0.3359999999999985, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.09999999999999998, SF049a_04=0.0010000000000000009, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=1, SF094_04=50335748, SF055_04_01=4, SF056_04_01=1, SF060_04_01=28.08000000000004, SF061a_04_01=0.02400000000000091, SF061b_04_01=-1.784000000000006, SF055_04_02=4, SF056_04_02=1, SF060_04_02=13.480000000000018, SF061a_04_02=0.35199999999998965, SF061b_04_02=-2.3600000000000065, SF055_04_03=5, SF056_04_03=1, SF060_04_03=32.160000000000025, SF061a_04_03=-0.2560000000000002, SF061b_04_03=-1.7360000000000042, SF055_04_04=4, SF056_04_04=1, SF060_04_04=20.480000000000018, SF061a_04_04=0.5519999999999925, SF061b_04_04=-1.9680000000000035, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.132, SF049a_05=-0.0040000000000000036, SF049b_05=0.01100000000000001, SF054_05=1, SatBitmaskLen_05=1, SF094_05=50335748, SF055_05_01=1, SF056_05_01=1, SF060_05_01=19.439999999999998, SF061a_05_01=1.3119999999999976, SF061b_05_01=-0.35999999999999943, SF055_05_02=1, SF056_05_02=1, SF060_05_02=3.080000000000041, SF061a_05_02=1.583999999999989, SF061b_05_02=-0.9680000000000035, SF055_05_03=4, SF056_05_03=1, SF060_05_03=23.760000000000048, SF061a_05_03=0.8239999999999981, SF061b_05_03=-0.48799999999999955, SF055_05_04=3, SF056_05_04=1, SF060_05_04=10.720000000000027, SF061a_05_04=1.7920000000000016, SF061b_05_04=-0.7120000000000033, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0020000000000000018, SF049b_06=-0.013000000000000012, SF054_06=1, SatBitmaskLen_06=0, SF094_06=98304, SF055_06_01=5, SF056_06_01=1, SF060_06_01=32.44, SF061a_06_01=-0.0799999999999983, SF061b_06_01=0.5759999999999934, SF055_06_02=1, SF056_06_02=1, SF060_06_02=8.640000000000043, SF061a_06_02=0.2560000000000002, SF061b_06_02=0.24799999999999045, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=2, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=0.0010000000000000009, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=1, SF094_07=184550404, SF055_07_01=1, SF056_07_01=1, SF060_07_01=12.04000000000002, SF061a_07_01=1.0959999999999894, SF061b_07_01=-0.2400000000000091, SF055_07_02=1, SF056_07_02=1, SF060_07_02=32.04000000000002, SF061a_07_02=0.5919999999999987, SF061b_07_02=0.6400000000000006, SF055_07_03=1, SF056_07_03=1, SF060_07_03=6.240000000000009, SF061a_07_03=1.2719999999999914, SF061b_07_03=0.19999999999998863, SF055_07_04=4, SF056_07_04=1, SF060_07_04=21.640000000000043, SF061a_07_04=1.176000000000002, SF061b_07_04=0.14399999999999125, SF055_07_05=2, SF056_07_05=1, SF060_07_05=18.480000000000018, SF061a_07_05=1.3519999999999897, SF061b_07_05=0.15200000000000102, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.07199999999999995, SF049a_08=0.006000000000000005, SF049b_08=0.016000000000000014, SF054_08=1, SatBitmaskLen_08=1, SF094_08=184550404, SF055_08_01=2, SF056_08_01=1, SF060_08_01=11.520000000000039, SF061a_08_01=1.024000000000001, SF061b_08_01=0.015999999999991132, SF055_08_02=2, SF056_08_02=1, SF060_08_02=35.879999999999995, SF061a_08_02=0.5360000000000014, SF061b_08_02=0.9119999999999919, SF055_08_03=2, SF056_08_03=1, SF060_08_03=7.160000000000025, SF061a_08_03=1.1039999999999992, SF061b_08_03=0.16799999999999216, SF055_08_04=4, SF056_08_04=1, SF060_08_04=20.480000000000018, SF061a_08_04=0.7599999999999909, SF061b_08_04=-0.6480000000000103, SF055_08_05=1, SF056_08_05=1, SF060_08_05=20.04000000000002, SF061a_08_05=1.5360000000000014, SF061b_08_05=0.5600000000000023, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.17600000000000005, SF049a_09=-0.01899999999999999, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF094_09=98304, SF055_09_01=3, SF056_09_01=1, SF060_09_01=34.04000000000002, SF061a_09_01=-0.2960000000000065, SF061b_09_01=0.21599999999999397, SF055_09_02=1, SF056_09_02=1, SF060_09_02=7.840000000000032, SF061a_09_02=0.32799999999998875, SF061b_09_02=0.30400000000000205, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=3, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.124, SF049a_10=0.010000000000000009, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=1, SF094_10=184550404, SF055_10_01=1, SF056_10_01=1, SF060_10_01=7.8799999999999955, SF061a_10_01=1.2800000000000011, SF061b_10_01=0.08799999999999386, SF055_10_02=1, SF056_10_02=1, SF060_10_02=30.200000000000045, SF061a_10_02=1.063999999999993, SF061b_10_02=0.9119999999999919, SF055_10_03=1, SF056_10_03=1, SF060_10_03=2.0400000000000205, SF061a_10_03=1.2959999999999923, SF061b_10_03=0.4159999999999968, SF055_10_04=1, SF056_10_04=1, SF060_10_04=16.0, SF061a_10_04=1.519999999999996, SF061b_10_04=-0.6800000000000068, SF055_10_05=1, SF056_10_05=1, SF060_10_05=14.400000000000034, SF061a_10_05=1.2079999999999984, SF061b_10_05=0.5039999999999907)>",
-            "<SPARTN(SPARTN-1X-HPAC-BEI, msgType=1, nData=101, eaf=0, crcType=2, frameCrc=7, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=3165361, SF005=354, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.008000000000000007, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=-0.008000000000000007, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=1, SF094_01=184554500, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-9.680000000000007, SF061a_01_01=-0.7920000000000016, SF061b_01_01=-0.5679999999999978, SF055_01_02=2, SF056_01_02=1, SF060_01_02=15.560000000000002, SF061a_01_02=-0.5120000000000005, SF061b_01_02=0.1839999999999975, SF055_01_03=1, SF056_01_03=1, SF060_01_03=-12.079999999999984, SF061a_01_03=-0.43200000000000216, SF061b_01_03=-0.24800000000000466, SF055_01_04=3, SF056_01_04=1, SF060_01_04=10.360000000000014, SF061a_01_04=-1.5360000000000014, SF061b_01_04=-0.1600000000000108, SF055_01_05=1, SF056_01_05=1, SF060_01_05=5.1200000000000045, SF061a_01_05=0.27199999999999136, SF061b_01_05=-0.8640000000000043, SF055_01_06=1, SF056_01_06=1, SF060_01_06=3.8799999999999955, SF061a_01_06=-0.06400000000000716, SF061b_01_06=0.1599999999999966, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.16400000000000003, SF049a_02=-0.0010000000000000009, SF049b_02=0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=1, SF094_02=184554500, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-11.560000000000002, SF061a_02_01=-0.632000000000005, SF061b_02_01=-0.5440000000000111, SF055_02_02=3, SF056_02_02=1, SF060_02_02=14.360000000000014, SF061a_02_02=-0.6400000000000006, SF061b_02_02=0.16799999999999216, SF055_02_03=1, SF056_02_03=1, SF060_02_03=-13.239999999999952, SF061a_02_03=-0.45600000000000307, SF061b_02_03=-0.2880000000000109, SF055_02_04=2, SF056_02_04=1, SF060_02_04=7.0, SF061a_02_04=-1.4639999999999986, SF061b_02_04=-0.08800000000000807, SF055_02_05=2, SF056_02_05=1, SF060_02_05=4.8799999999999955, SF061a_02_05=-0.008000000000009777, SF061b_02_05=-0.847999999999999, SF055_02_06=1, SF056_02_06=1, SF060_02_06=3.7200000000000273, SF061a_02_06=-0.1600000000000108, SF061b_02_06=0.1039999999999992)>",
-            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=536, eaf=0, crcType=2, frameCrc=14, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=4199949, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.15200000000000002, SF049a_01=-0.0020000000000000018, SF049b_01=-0.0040000000000000036, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412539457, SF055_01_01=1, SF056_01_01=1, SF060_01_01=3.160000000000025, SF061a_01_01=0.43200000000000216, SF061b_01_01=0.1599999999999966, SF055_01_02=2, SF056_01_02=1, SF060_01_02=0.6800000000000068, SF061a_01_02=0.19199999999999307, SF061b_01_02=0.08799999999999386, SF055_01_03=4, SF056_01_03=1, SF060_01_03=-0.7999999999999545, SF061a_01_03=1.0480000000000018, SF061b_01_03=0.1039999999999992, SF055_01_04=1, SF056_01_04=1, SF060_01_04=7.360000000000014, SF061a_01_04=1.4959999999999951, SF061b_01_04=-0.1360000000000099, SF055_01_05=3, SF056_01_05=1, SF060_01_05=-0.3599999999999568, SF061a_01_05=0.23999999999999488, SF061b_01_05=-0.1600000000000108, SF055_01_06=4, SF056_01_06=1, SF060_01_06=17.04000000000002, SF061a_01_06=-0.38400000000000034, SF061b_01_06=-0.6240000000000094, SF055_01_07=4, SF056_01_07=1, SF060_01_07=24.80000000000001, SF061a_01_07=-1.0480000000000018, SF061b_01_07=-0.32800000000000296, SF055_01_08=4, SF056_01_08=1, SF060_01_08=13.680000000000007, SF061a_01_08=0.847999999999999, SF061b_01_08=0.4479999999999933, SF031_02=1, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.0, SF044_02=1, SF048_02=-0.128, SF049a_02=0.0010000000000000009, SF049b_02=-0.0030000000000000027, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412539457, SF055_02_01=5, SF056_02_01=1, SF060_02_01=-1.2399999999999523, SF061a_02_01=2.3359999999999985, SF061b_02_01=0.0, SF055_02_02=4, SF056_02_02=1, SF060_02_02=-2.839999999999975, SF061a_02_02=2.128, SF061b_02_02=-0.1600000000000108, SF055_02_03=4, SF056_02_03=1, SF060_02_03=-3.7199999999999704, SF061a_02_03=0.2079999999999984, SF061b_02_03=0.14399999999999125, SF055_02_04=5, SF056_02_04=1, SF060_02_04=2.4399999999999977, SF061a_02_04=2.304000000000002, SF061b_02_04=-0.35999999999999943, SF055_02_05=4, SF056_02_05=1, SF060_02_05=-1.5600000000000023, SF061a_02_05=0.4959999999999951, SF061b_02_05=-0.04800000000000182, SF055_02_06=1, SF056_02_06=1, SF060_02_06=20.400000000000034, SF061a_02_06=0.14399999999999125, SF061b_02_06=-0.35200000000000387, SF055_02_07=5, SF056_02_07=1, SF060_02_07=27.120000000000005, SF061a_02_07=0.19999999999998863, SF061b_02_07=0.04800000000000182, SF055_02_08=4, SF056_02_08=1, SF060_02_08=10.680000000000007, SF061a_02_08=0.19199999999999307, SF061b_02_08=0.3999999999999915, SF031_03=2, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=1, SF043_03=0.0, SF044_03=1, SF048_03=-0.14800000000000002, SF049a_03=-0.015000000000000013, SF049b_03=0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4412539457, SF055_03_01=5, SF056_03_01=1, SF060_03_01=-0.5600000000000023, SF061a_03_01=2.7039999999999935, SF061b_03_01=0.0799999999999983, SF055_03_02=5, SF056_03_02=1, SF060_03_02=-2.0399999999999636, SF061a_03_02=2.1999999999999886, SF061b_03_02=0.08799999999999386, SF055_03_03=4, SF056_03_03=1, SF060_03_03=-1.3999999999999773, SF061a_03_03=0.1039999999999992, SF061b_03_03=0.03999999999999204, SF055_03_04=5, SF056_03_04=1, SF060_03_04=1.6400000000000432, SF061a_03_04=1.3119999999999976, SF061b_03_04=-0.03200000000001069, SF055_03_05=5, SF056_03_05=1, SF060_03_05=-2.0, SF061a_03_05=0.27199999999999136, SF061b_03_05=-0.08800000000000807, SF055_03_06=4, SF056_03_06=1, SF060_03_06=14.400000000000034, SF061a_03_06=0.2879999999999967, SF061b_03_06=-0.7680000000000007, SF055_03_07=4, SF056_03_07=1, SF060_03_07=26.80000000000001, SF061a_03_07=-0.7280000000000086, SF061b_03_07=-0.2079999999999984, SF055_03_08=1, SF056_03_08=1, SF060_03_08=13.760000000000048, SF061a_03_08=0.07199999999998852, SF061b_03_08=0.367999999999995, SF031_04=3, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.0, SF044_04=1, SF048_04=-0.124, SF049a_04=0.0030000000000000027, SF049b_04=-0.0010000000000000009, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412539457, SF055_04_01=4, SF056_04_01=1, SF060_04_01=1.3600000000000136, SF061a_04_01=-1.480000000000004, SF061b_04_01=0.2079999999999984, SF055_04_02=4, SF056_04_02=1, SF060_04_02=-1.599999999999966, SF061a_04_02=-1.328000000000003, SF061b_04_02=0.24799999999999045, SF055_04_03=4, SF056_04_03=1, SF060_04_03=-4.359999999999957, SF061a_04_03=2.7920000000000016, SF061b_04_03=0.3359999999999985, SF055_04_04=4, SF056_04_04=1, SF060_04_04=9.920000000000016, SF061a_04_04=0.1039999999999992, SF061b_04_04=0.15200000000000102, SF055_04_05=4, SF056_04_05=1, SF060_04_05=-0.9199999999999591, SF061a_04_05=3.1119999999999948, SF061b_04_05=0.0799999999999983, SF055_04_06=5, SF056_04_06=1, SF060_04_06=27.80000000000001, SF061a_04_06=1.3199999999999932, SF061b_04_06=-0.784000000000006, SF055_04_07=5, SF056_04_07=1, SF060_04_07=29.439999999999998, SF061a_04_07=0.4959999999999951, SF061b_04_07=0.8399999999999892, SF055_04_08=3, SF056_04_08=1, SF060_04_08=11.879999999999995, SF061a_04_08=1.1359999999999957, SF061b_04_08=0.5999999999999943, SF031_05=4, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.0, SF044_05=1, SF048_05=-0.14, SF049a_05=0.0020000000000000018, SF049b_05=-0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412539457, SF055_05_01=4, SF056_05_01=1, SF060_05_01=6.1200000000000045, SF061a_05_01=-0.1039999999999992, SF061b_05_01=0.37599999999999056, SF055_05_02=5, SF056_05_02=1, SF060_05_02=1.4399999999999977, SF061a_05_02=-1.6720000000000041, SF061b_05_02=0.21599999999999397, SF055_05_03=4, SF056_05_03=1, SF060_05_03=0.040000000000020464, SF061a_05_03=2.5519999999999925, SF061b_05_03=0.4239999999999924, SF055_05_04=2, SF056_05_04=1, SF060_05_04=10.319999999999993, SF061a_05_04=0.46399999999999864, SF061b_05_04=0.04800000000000182, SF055_05_05=3, SF056_05_05=1, SF060_05_05=1.0, SF061a_05_05=3.087999999999994, SF061b_05_05=0.24799999999999045, SF055_05_06=5, SF056_05_06=1, SF060_05_06=20.720000000000027, SF061a_05_06=1.3599999999999994, SF061b_05_06=-0.2560000000000002, SF055_05_07=4, SF056_05_07=1, SF060_05_07=35.0, SF061a_05_07=0.4719999999999942, SF061b_05_07=0.367999999999995, SF055_05_08=3, SF056_05_08=1, SF060_05_08=20.28000000000003, SF061a_05_08=1.5360000000000014, SF061b_05_08=0.6239999999999952, SF031_06=5, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.0, SF044_06=1, SF048_06=-0.08799999999999997, SF049a_06=-0.01899999999999999, SF049b_06=-0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538881, SF055_06_01=2, SF056_06_01=1, SF060_06_01=5.600000000000023, SF061a_06_01=0.14399999999999125, SF061b_06_01=0.28000000000000114, SF055_06_02=3, SF056_06_02=1, SF060_06_02=3.2000000000000455, SF061a_06_02=0.24799999999999045, SF061b_06_02=0.29599999999999227, SF055_06_03=4, SF056_06_03=1, SF060_06_03=0.20000000000004547, SF061a_06_03=-0.7439999999999998, SF061b_06_03=0.35999999999999943, SF055_06_04=2, SF056_06_04=1, SF060_06_04=12.360000000000014, SF061a_06_04=0.2639999999999958, SF061b_06_04=-0.02400000000000091, SF055_06_05=4, SF056_06_05=1, SF060_06_05=0.5600000000000023, SF061a_06_05=-1.720000000000006, SF061b_06_05=0.23999999999999488, SF055_06_06=4, SF056_06_06=1, SF060_06_06=8.720000000000027, SF061a_06_06=1.2239999999999895, SF061b_06_06=0.43200000000000216, SF031_07=6, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.0, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=-0.015999999999999986, SF049b_07=-0.006000000000000005, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538881, SF055_07_01=3, SF056_07_01=1, SF060_07_01=7.319999999999993, SF061a_07_01=-0.03200000000001069, SF061b_07_01=0.19999999999998863, SF055_07_02=1, SF056_07_02=1, SF060_07_02=5.0, SF061a_07_02=0.11999999999999034, SF061b_07_02=0.24799999999999045, SF055_07_03=2, SF056_07_03=1, SF060_07_03=2.2000000000000455, SF061a_07_03=-0.480000000000004, SF061b_07_03=0.3359999999999985, SF055_07_04=1, SF056_07_04=1, SF060_07_04=12.760000000000048, SF061a_07_04=0.13599999999999568, SF061b_07_04=0.055999999999997385, SF055_07_05=2, SF056_07_05=1, SF060_07_05=2.080000000000041, SF061a_07_05=-0.9920000000000044, SF061b_07_05=0.015999999999991132, SF055_07_06=4, SF056_07_06=1, SF060_07_06=13.160000000000025, SF061a_07_06=0.9919999999999902, SF061b_07_06=0.6319999999999908, SF031_08=7, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.0, SF044_08=1, SF048_08=-0.14, SF049a_08=-0.023999999999999994, SF049b_08=-0.0010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF093_08=117571585, SF055_08_01=3, SF056_08_01=1, SF060_08_01=-8.839999999999975, SF061a_08_01=-0.7199999999999989, SF061b_08_01=-0.23199999999999932, SF055_08_02=4, SF056_08_02=1, SF060_08_02=-10.759999999999991, SF061a_08_02=-1.5520000000000067, SF061b_08_02=-0.1039999999999992, SF055_08_03=1, SF056_08_03=1, SF060_08_03=-2.8799999999999955, SF061a_08_03=-0.4960000000000093, SF061b_08_03=-0.3760000000000048, SF055_08_04=4, SF056_08_04=1, SF060_08_04=-12.479999999999961, SF061a_08_04=-1.240000000000009, SF061b_08_04=-0.1839999999999975, SF055_08_05=2, SF056_08_05=1, SF060_08_05=4.360000000000014, SF061a_08_05=0.5919999999999987, SF061b_08_05=0.3359999999999985, SF031_09=8, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.0040000000000000036, SF044_09=1, SF048_09=-0.14400000000000002, SF049a_09=0.0010000000000000009, SF049b_09=0.0, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, SF055_09_01=1, SF056_09_01=1, SF060_09_01=13.400000000000034, SF061a_09_01=-0.2400000000000091, SF061b_09_01=0.09599999999998943, SF055_09_02=2, SF056_09_02=1, SF060_09_02=11.520000000000039, SF061a_09_02=-0.35200000000000387, SF061b_09_02=-0.016000000000005343, SF055_09_03=1, SF056_09_03=1, SF060_09_03=8.0, SF061a_09_03=-0.5440000000000111, SF061b_09_03=0.14399999999999125, SF055_09_04=2, SF056_09_04=1, SF060_09_04=22.640000000000043, SF061a_09_04=-0.08800000000000807, SF061b_09_04=-0.2880000000000109, SF055_09_05=2, SF056_09_05=1, SF060_09_05=11.640000000000043, SF061a_09_05=-1.4000000000000057, SF061b_09_05=-0.1600000000000108, SF055_09_06=4, SF056_09_06=1, SF060_09_06=20.0, SF061a_09_06=-3.8160000000000025, SF061b_09_06=0.015999999999991132, SF031_10=9, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=1, SF043_10=0.0040000000000000036, SF044_10=1, SF048_10=-0.09199999999999997, SF049a_10=0.007000000000000006, SF049b_10=-0.0010000000000000009, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538881, SF055_10_01=2, SF056_10_01=1, SF060_10_01=9.160000000000025, SF061a_10_01=-0.30400000000000205, SF061b_10_01=-0.17600000000000193, SF055_10_02=2, SF056_10_02=1, SF060_10_02=6.720000000000027, SF061a_10_02=-0.4960000000000093, SF061b_10_02=-0.20000000000000284, SF055_10_03=2, SF056_10_03=1, SF060_10_03=4.8799999999999955, SF061a_10_03=-0.6159999999999997, SF061b_10_03=-0.15200000000000102, SF055_10_04=2, SF056_10_04=1, SF060_10_04=14.240000000000009, SF061a_10_04=0.031999999999996476, SF061b_10_04=-0.416000000000011, SF055_10_05=1, SF056_10_05=1, SF060_10_05=5.800000000000011, SF061a_10_05=-0.7120000000000033, SF061b_10_05=-0.38400000000000034, SF055_10_06=2, SF056_10_06=1, SF060_10_06=17.24000000000001, SF061a_10_06=-2.896000000000008, SF061b_10_06=-0.3119999999999976)>",
-            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=465, eaf=0, crcType=2, frameCrc=0, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=8229442, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=10, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.0040000000000000036, SF044_01=1, SF048_01=-0.11199999999999999, SF049a_01=0.016000000000000014, SF049b_01=-0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538881, SF055_01_01=3, SF056_01_01=1, SF060_01_01=-2.5600000000000023, SF061a_01_01=-0.8719999999999999, SF061b_01_01=-0.14400000000000546, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-5.639999999999986, SF061a_01_02=-0.7520000000000095, SF061b_01_02=-0.21600000000000819, SF055_01_03=4, SF056_01_03=1, SF060_01_03=-6.0, SF061a_01_03=-0.9519999999999982, SF061b_01_03=-0.09600000000000364, SF055_01_04=1, SF056_01_04=1, SF060_01_04=-0.4399999999999977, SF061a_01_04=-0.5600000000000023, SF061b_01_04=-0.35200000000000387, SF055_01_05=2, SF056_01_05=1, SF060_01_05=-8.599999999999966, SF061a_01_05=-0.8320000000000078, SF061b_01_05=-0.3119999999999976, SF055_01_06=5, SF056_01_06=1, SF060_01_06=5.720000000000027, SF061a_01_06=-1.6640000000000015, SF061b_01_06=0.35199999999998965, SF031_02=11, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.0040000000000000036, SF044_02=1, SF048_02=-0.18799999999999994, SF049a_02=0.013000000000000012, SF049b_02=-0.0050000000000000044, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538881, SF055_02_01=2, SF056_02_01=1, SF060_02_01=14.319999999999993, SF061a_02_01=-0.3440000000000083, SF061b_02_01=0.03999999999999204, SF055_02_02=2, SF056_02_02=1, SF060_02_02=13.080000000000041, SF061a_02_02=-0.416000000000011, SF061b_02_02=0.055999999999997385, SF055_02_03=1, SF056_02_03=1, SF060_02_03=9.840000000000032, SF061a_02_03=-0.5600000000000023, SF061b_02_03=0.14399999999999125, SF055_02_04=2, SF056_02_04=1, SF060_02_04=24.319999999999993, SF061a_02_04=-0.3680000000000092, SF061b_02_04=-0.2560000000000002, SF055_02_05=1, SF056_02_05=1, SF060_02_05=18.0, SF061a_02_05=-1.2319999999999993, SF061b_02_05=-0.20000000000000284, SF055_02_06=5, SF056_02_06=1, SF060_02_06=31.80000000000001, SF061a_02_06=-1.9920000000000044, SF061b_02_06=0.06399999999999295, SF031_03=12, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.008000000000000007, SF044_03=1, SF048_03=-0.14, SF049a_03=0.008000000000000007, SF049b_03=0.016000000000000014, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4378984449, SF055_03_01=5, SF056_03_01=1, SF060_03_01=13.960000000000036, SF061a_03_01=0.43200000000000216, SF061b_03_01=0.43200000000000216, SF055_03_02=5, SF056_03_02=1, SF060_03_02=12.439999999999998, SF061a_03_02=0.19999999999998863, SF061b_03_02=0.40800000000000125, SF055_03_03=3, SF056_03_03=1, SF060_03_03=22.80000000000001, SF061a_03_03=-0.43200000000000216, SF061b_03_03=-0.2560000000000002, SF055_03_04=3, SF056_03_04=1, SF060_03_04=16.160000000000025, SF061a_03_04=-1.2240000000000038, SF061b_03_04=-0.3920000000000101, SF055_03_05=4, SF056_03_05=1, SF060_03_05=33.04000000000002, SF061a_03_05=-2.5120000000000076, SF061b_03_05=0.055999999999997385, SF031_04=13, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.008000000000000007, SF044_04=1, SF048_04=-0.09599999999999997, SF049a_04=0.0020000000000000018, SF049b_04=-0.0030000000000000027, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538881, SF055_04_01=1, SF056_04_01=1, SF060_04_01=11.080000000000041, SF061a_04_01=-0.3680000000000092, SF061b_04_01=-0.16800000000000637, SF055_04_02=1, SF056_04_02=1, SF060_04_02=9.200000000000045, SF061a_04_02=-0.4399999999999977, SF061b_04_02=-0.20000000000000284, SF055_04_03=2, SF056_04_03=1, SF060_04_03=7.560000000000002, SF061a_04_03=-0.5760000000000076, SF061b_04_03=-0.08800000000000807, SF055_04_04=1, SF056_04_04=1, SF060_04_04=16.80000000000001, SF061a_04_04=-0.0799999999999983, SF061b_04_04=-0.480000000000004, SF055_04_05=2, SF056_04_05=1, SF060_04_05=10.600000000000023, SF061a_04_05=-0.8719999999999999, SF061b_04_05=-0.3440000000000083, SF055_04_06=4, SF056_04_06=1, SF060_04_06=28.879999999999995, SF061a_04_06=-2.608000000000004, SF061b_04_06=-0.5600000000000023, SF031_05=14, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.008000000000000007, SF044_05=1, SF048_05=-0.12, SF049a_05=0.006000000000000005, SF049b_05=0.0, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538881, SF055_05_01=4, SF056_05_01=1, SF060_05_01=10.28000000000003, SF061a_05_01=-0.43200000000000216, SF061b_05_01=-0.16800000000000637, SF055_05_02=2, SF056_05_02=1, SF060_05_02=7.960000000000036, SF061a_05_02=-0.2960000000000065, SF061b_05_02=-0.2079999999999984, SF055_05_03=1, SF056_05_03=1, SF060_05_03=6.8799999999999955, SF061a_05_03=-0.6000000000000085, SF061b_05_03=-0.09600000000000364, SF055_05_04=1, SF056_05_04=1, SF060_05_04=13.920000000000016, SF061a_05_04=-0.03200000000001069, SF061b_05_04=-0.4720000000000084, SF055_05_05=1, SF056_05_05=1, SF060_05_05=8.0, SF061a_05_05=-0.8400000000000034, SF061b_05_05=-0.5919999999999987, SF055_05_06=4, SF056_05_06=1, SF060_05_06=25.879999999999995, SF061a_05_06=-2.6400000000000077, SF061b_05_06=-0.6240000000000094, SF031_06=15, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.008000000000000007, SF044_06=1, SF048_06=-0.15200000000000002, SF049a_06=0.009000000000000008, SF049b_06=-0.007000000000000006, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538880, SF055_06_01=1, SF056_06_01=1, SF060_06_01=7.28000000000003, SF061a_06_01=0.14399999999999125, SF061b_06_01=0.3199999999999932, SF055_06_02=1, SF056_06_02=1, SF060_06_02=4.400000000000034, SF061a_06_02=0.09599999999998943, SF061b_06_02=0.21599999999999397, SF055_06_03=2, SF056_06_03=1, SF060_06_03=4.160000000000025, SF061a_06_03=-0.35999999999999943, SF061b_06_03=0.38400000000000034, SF055_06_04=2, SF056_06_04=1, SF060_06_04=9.120000000000005, SF061a_06_04=0.35199999999998965, SF061b_06_04=0.16799999999999216, SF055_06_05=2, SF056_06_05=1, SF060_06_05=2.319999999999993, SF061a_06_05=-0.19200000000000728, SF061b_06_05=0.04800000000000182, SF031_07=16, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.008000000000000007, SF044_07=1, SF048_07=-0.15200000000000002, SF049a_07=0.0020000000000000018, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4546756608, SF055_07_01=1, SF056_07_01=1, SF060_07_01=19.439999999999998, SF061a_07_01=-1.024000000000001, SF061b_07_01=-0.6480000000000103, SF055_07_02=4, SF056_07_02=1, SF060_07_02=62.24000000000001, SF061a_07_02=0.22399999999998954, SF061b_07_02=-0.20000000000000284, SF055_07_03=1, SF056_07_03=1, SF060_07_03=18.08000000000004, SF061a_07_03=-1.1039999999999992, SF061b_07_03=-0.6720000000000113, SF055_07_04=1, SF056_07_04=1, SF060_07_04=15.920000000000016, SF061a_07_04=-1.240000000000009, SF061b_07_04=-0.4480000000000075, SF055_07_05=1, SF056_07_05=1, SF060_07_05=27.480000000000018, SF061a_07_05=-0.8800000000000097, SF061b_07_05=-0.9840000000000089, SF055_07_06=1, SF056_07_06=1, SF060_07_06=23.360000000000014, SF061a_07_06=-1.6800000000000068, SF061b_07_06=-1.0, SF031_08=17, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.008000000000000007, SF044_08=1, SF048_08=-0.11599999999999999, SF049a_08=-0.0040000000000000036, SF049b_08=0.006000000000000005, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4546756608, SF055_08_01=1, SF056_08_01=1, SF060_08_01=15.120000000000005, SF061a_08_01=-0.9519999999999982, SF061b_08_01=-0.6159999999999997, SF055_08_02=1, SF056_08_02=1, SF060_08_02=59.960000000000036, SF061a_08_02=0.28000000000000114, SF061b_08_02=-0.3760000000000048, SF055_08_03=1, SF056_08_03=1, SF060_08_03=13.640000000000043, SF061a_08_03=-0.9519999999999982, SF061b_08_03=-0.6640000000000015, SF055_08_04=1, SF056_08_04=1, SF060_08_04=12.240000000000009, SF061a_08_04=-1.088000000000008, SF061b_08_04=-0.5919999999999987, SF055_08_05=2, SF056_08_05=1, SF060_08_05=21.08000000000004, SF061a_08_05=-0.7920000000000016, SF061b_08_05=-0.9759999999999991, SF055_08_06=1, SF056_08_06=1, SF060_08_06=16.52000000000004, SF061a_08_06=-1.5840000000000032, SF061b_08_06=-0.9759999999999991, SF031_09=18, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.008000000000000007, SF044_09=1, SF048_09=-0.132, SF049a_09=0.006000000000000005, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, SF055_09_01=1, SF056_09_01=1, SF060_09_01=8.879999999999995, SF061a_09_01=0.3119999999999976, SF061b_09_01=0.5759999999999934, SF055_09_02=1, SF056_09_02=1, SF060_09_02=7.0400000000000205, SF061a_09_02=0.21599999999999397, SF061b_09_02=0.4719999999999942, SF055_09_03=1, SF056_09_03=1, SF060_09_03=6.28000000000003, SF061a_09_03=-0.3119999999999976, SF061b_09_03=0.5999999999999943, SF055_09_04=1, SF056_09_04=1, SF060_09_04=12.360000000000014, SF061a_09_04=0.5759999999999934, SF061b_09_04=0.23199999999999932, SF055_09_05=2, SF056_09_05=1, SF060_09_05=8.600000000000023, SF061a_09_05=-0.016000000000005343, SF061b_09_05=0.1599999999999966, SF055_09_06=2, SF056_09_06=1, SF060_09_06=31.0, SF061a_09_06=-1.9200000000000017, SF061b_09_06=0.35199999999998965, SF031_10=19, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.008000000000000007, SF044_10=1, SF048_10=-0.15200000000000002, SF049a_10=0.0030000000000000027, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538880, SF055_10_01=1, SF056_10_01=1, SF060_10_01=6.560000000000002, SF061a_10_01=0.1839999999999975, SF061b_10_01=0.30400000000000205, SF055_10_02=1, SF056_10_02=1, SF060_10_02=3.9600000000000364, SF061a_10_02=0.11999999999999034, SF061b_10_02=0.2560000000000002, SF055_10_03=1, SF056_10_03=1, SF060_10_03=4.560000000000002, SF061a_10_03=-0.12000000000000455, SF061b_10_03=0.37599999999999056, SF055_10_04=1, SF056_10_04=1, SF060_10_04=8.080000000000041, SF061a_10_04=0.3199999999999932, SF061b_10_04=0.16799999999999216, SF055_10_05=1, SF056_10_05=1, SF060_10_05=2.8799999999999955, SF061a_10_05=-0.28000000000000114, SF061b_10_05=0.007999999999995566)>",
-            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=459, eaf=0, crcType=2, frameCrc=15, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=10010485, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=20, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.14800000000000002, SF049a_01=-0.0010000000000000009, SF049b_01=0.007000000000000006, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4546756608, SF055_01_01=1, SF056_01_01=1, SF060_01_01=21.08000000000004, SF061a_01_01=-0.8239999999999981, SF061b_01_01=-0.6720000000000113, SF055_01_02=5, SF056_01_02=1, SF060_01_02=62.08000000000004, SF061a_01_02=-0.06400000000000716, SF061b_01_02=-0.5280000000000058, SF055_01_03=1, SF056_01_03=1, SF060_01_03=19.840000000000032, SF061a_01_03=-0.8960000000000008, SF061b_01_03=-0.6880000000000024, SF055_01_04=1, SF056_01_04=1, SF060_01_04=18.360000000000014, SF061a_01_04=-1.0799999999999983, SF061b_01_04=-0.5840000000000032, SF055_01_05=1, SF056_01_05=1, SF060_01_05=28.28000000000003, SF061a_01_05=-0.6640000000000015, SF061b_01_05=-0.9840000000000089, SF055_01_06=1, SF056_01_06=1, SF060_01_06=26.160000000000025, SF061a_01_06=-1.3840000000000003, SF061b_01_06=-1.0160000000000053, SF031_02=21, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.124, SF049a_02=0.010000000000000009, SF049b_02=-0.009000000000000008, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4546756608, SF055_02_01=1, SF056_02_01=1, SF060_02_01=16.960000000000036, SF061a_02_01=-0.847999999999999, SF061b_02_01=-0.6640000000000015, SF055_02_02=1, SF056_02_02=1, SF060_02_02=59.44, SF061a_02_02=-0.02400000000000091, SF061b_02_02=-0.22400000000000375, SF055_02_03=1, SF056_02_03=1, SF060_02_03=15.520000000000039, SF061a_02_03=-0.8560000000000088, SF061b_02_03=-0.7280000000000086, SF055_02_04=1, SF056_02_04=1, SF060_02_04=14.680000000000007, SF061a_02_04=-1.13600000000001, SF061b_02_04=-0.48799999999999955, SF055_02_05=1, SF056_02_05=1, SF060_02_05=22.08000000000004, SF061a_02_05=-0.5600000000000023, SF061b_02_05=-1.1280000000000001, SF055_02_06=1, SF056_02_06=1, SF060_02_06=19.720000000000027, SF061a_02_06=-1.4399999999999977, SF061b_02_06=-1.088000000000008, SF031_03=22, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.14400000000000002, SF049a_03=0.0050000000000000044, SF049b_03=-0.0030000000000000027, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4345430017, SF055_03_01=1, SF056_03_01=1, SF060_03_01=7.640000000000043, SF061a_03_01=0.24799999999999045, SF061b_03_01=0.5519999999999925, SF055_03_02=1, SF056_03_02=1, SF060_03_02=6.080000000000041, SF061a_03_02=-0.1360000000000099, SF061b_03_02=0.6319999999999908, SF055_03_03=1, SF056_03_03=1, SF060_03_03=10.800000000000011, SF061a_03_03=0.47999999999998977, SF061b_03_03=0.24799999999999045, SF055_03_04=1, SF056_03_04=1, SF060_03_04=8.680000000000007, SF061a_03_04=-0.12000000000000455, SF061b_03_04=0.21599999999999397, SF055_03_05=2, SF056_03_05=1, SF060_03_05=35.64000000000004, SF061a_03_05=-1.9120000000000061, SF061b_03_05=0.17600000000000193, SF031_04=23, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=2, SF043_04=0.01200000000000001, SF044_04=1, SF048_04=-0.14, SF049a_04=-0.0040000000000000036, SF049b_04=0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538881, SF055_04_01=1, SF056_04_01=1, SF060_04_01=10.680000000000007, SF061a_04_01=0.30400000000000205, SF061b_04_01=0.5120000000000005, SF055_04_02=1, SF056_04_02=1, SF060_04_02=8.600000000000023, SF061a_04_02=0.21599999999999397, SF061b_04_02=0.3999999999999915, SF055_04_03=1, SF056_04_03=1, SF060_04_03=9.760000000000048, SF061a_04_03=-0.15200000000000102, SF061b_04_03=0.6079999999999899, SF055_04_04=1, SF056_04_04=1, SF060_04_04=12.360000000000014, SF061a_04_04=0.38400000000000034, SF061b_04_04=0.3359999999999985, SF055_04_05=1, SF056_04_05=1, SF060_04_05=9.640000000000043, SF061a_04_05=-0.1360000000000099, SF061b_04_05=0.15200000000000102, SF055_04_06=3, SF056_04_06=1, SF060_04_06=37.76000000000005, SF061a_04_06=-1.7280000000000015, SF061b_04_06=0.519999999999996, SF031_05=24, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=2, SF043_05=0.01200000000000001, SF044_05=1, SF048_05=-0.124, SF049a_05=-0.01999999999999999, SF049b_05=-0.01100000000000001, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538880, SF055_05_01=2, SF056_05_01=1, SF060_05_01=6.400000000000034, SF061a_05_01=0.46399999999999864, SF061b_05_01=0.2079999999999984, SF055_05_02=1, SF056_05_02=1, SF060_05_02=4.1200000000000045, SF061a_05_02=0.367999999999995, SF061b_05_02=0.09599999999998943, SF055_05_03=3, SF056_05_03=1, SF060_05_03=5.240000000000009, SF061a_05_03=0.08799999999999386, SF061b_05_03=0.1599999999999966, SF055_05_04=1, SF056_05_04=1, SF060_05_04=7.319999999999993, SF061a_05_04=0.7039999999999935, SF061b_05_04=-0.04000000000000625, SF055_05_05=1, SF056_05_05=1, SF060_05_05=3.6000000000000227, SF061a_05_05=-0.008000000000009777, SF061b_05_05=-0.22400000000000375, SF031_06=25, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.14, SF049a_06=-0.032, SF049b_06=-0.0030000000000000027, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538880, SF055_06_01=1, SF056_06_01=1, SF060_06_01=6.800000000000011, SF061a_06_01=0.3199999999999932, SF061b_06_01=0.13599999999999568, SF055_06_02=1, SF056_06_02=1, SF060_06_02=4.0400000000000205, SF061a_06_02=0.2560000000000002, SF061b_06_02=0.055999999999997385, SF055_06_03=1, SF056_06_03=1, SF060_06_03=6.080000000000041, SF061a_06_03=-0.17600000000000193, SF061b_06_03=0.16799999999999216, SF055_06_04=1, SF056_06_04=1, SF060_06_04=6.319999999999993, SF061a_06_04=0.4719999999999942, SF061b_06_04=-0.008000000000009777, SF055_06_05=1, SF056_06_05=1, SF060_06_05=2.5200000000000387, SF061a_06_05=-0.17600000000000193, SF061b_06_05=-0.14400000000000546, SF031_07=26, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=3, SF043_07=0.01200000000000001, SF044_07=1, SF048_07=-0.124, SF049a_07=-0.0020000000000000018, SF049b_07=0.014000000000000012, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538880, SF055_07_01=1, SF056_07_01=1, SF060_07_01=15.240000000000009, SF061a_07_01=0.4239999999999924, SF061b_07_01=-1.9120000000000061, SF055_07_02=1, SF056_07_02=1, SF060_07_02=14.720000000000027, SF061a_07_02=0.32799999999998875, SF061b_07_02=-1.960000000000008, SF055_07_03=2, SF056_07_03=1, SF060_07_03=13.400000000000034, SF061a_07_03=0.04800000000000182, SF061b_07_03=-1.8320000000000078, SF055_07_04=1, SF056_07_04=1, SF060_07_04=23.920000000000016, SF061a_07_04=0.3199999999999932, SF061b_07_04=-2.328000000000003, SF055_07_05=2, SF056_07_05=1, SF060_07_05=26.439999999999998, SF061a_07_05=-0.6720000000000113, SF061b_07_05=-2.4000000000000057, SF031_08=27, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=3, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.14800000000000002, SF049a_08=-0.0020000000000000018, SF049b_08=0.010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4412538881, SF055_08_01=1, SF056_08_01=1, SF060_08_01=14.240000000000009, SF061a_08_01=1.4080000000000013, SF061b_08_01=-0.1839999999999975, SF055_08_02=1, SF056_08_02=1, SF060_08_02=13.319999999999993, SF061a_08_02=1.3519999999999897, SF061b_08_02=-0.26400000000001, SF055_08_03=2, SF056_08_03=1, SF060_08_03=12.879999999999995, SF061a_08_03=1.0719999999999885, SF061b_08_03=-0.008000000000009777, SF055_08_04=1, SF056_08_04=1, SF060_08_04=20.400000000000034, SF061a_08_04=1.5279999999999916, SF061b_08_04=-0.6720000000000113, SF055_08_05=2, SF056_08_05=1, SF060_08_05=21.600000000000023, SF061a_08_05=0.8160000000000025, SF061b_08_05=-0.6800000000000068, SF055_08_06=4, SF056_08_06=1, SF060_08_06=47.24000000000001, SF061a_08_06=-0.1600000000000108, SF061b_08_06=0.03999999999999204, SF031_09=28, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.01200000000000001, SF044_09=1, SF048_09=-0.09199999999999997, SF049a_09=-0.0040000000000000036, SF049b_09=0.015000000000000013, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, SF055_09_01=1, SF056_09_01=1, SF060_09_01=13.760000000000048, SF061a_09_01=1.3279999999999887, SF061b_09_01=-0.16800000000000637, SF055_09_02=1, SF056_09_02=1, SF060_09_02=12.439999999999998, SF061a_09_02=1.2879999999999967, SF061b_09_02=-0.23199999999999932, SF055_09_03=1, SF056_09_03=1, SF060_09_03=13.0, SF061a_09_03=1.024000000000001, SF061b_09_03=-0.008000000000009777, SF055_09_04=1, SF056_09_04=1, SF060_09_04=17.80000000000001, SF061a_09_04=1.543999999999997, SF061b_09_04=-0.6880000000000024, SF055_09_05=1, SF056_09_05=1, SF060_09_05=18.879999999999995, SF061a_09_05=0.7680000000000007, SF061b_09_05=-0.695999999999998, SF055_09_06=3, SF056_09_06=1, SF060_09_06=46.960000000000036, SF061a_09_06=-0.32800000000000296, SF061b_09_06=-0.04000000000000625, SF031_10=29, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.01200000000000001, SF044_10=1, SF048_10=-0.14, SF049a_10=0.016000000000000014, SF049b_10=0.010000000000000009, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4546756608, SF055_10_01=1, SF056_10_01=1, SF060_10_01=13.680000000000007, SF061a_10_01=0.5519999999999925, SF061b_10_01=-0.19200000000000728, SF055_10_02=3, SF056_10_02=1, SF060_10_02=56.68000000000001, SF061a_10_02=0.8399999999999892, SF061b_10_02=0.7999999999999972, SF055_10_03=1, SF056_10_03=1, SF060_10_03=12.04000000000002, SF061a_10_03=0.4719999999999942, SF061b_10_03=-0.3119999999999976, SF055_10_04=1, SF056_10_04=1, SF060_10_04=13.080000000000041, SF061a_10_04=-0.2560000000000002, SF061b_10_04=-0.04000000000000625, SF055_10_05=2, SF056_10_05=1, SF060_10_05=16.439999999999998, SF061a_10_05=0.8160000000000025, SF061b_10_05=-0.4720000000000084, SF055_10_06=1, SF056_10_06=1, SF060_10_06=16.640000000000043, SF061a_10_06=-0.1600000000000108, SF061b_10_06=-0.3440000000000083)>",
-            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=448, eaf=0, crcType=2, frameCrc=13, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=7076377, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.16800000000000004, SF049a_01=-0.0010000000000000009, SF049b_01=-0.015999999999999986, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538880, SF055_01_01=2, SF056_01_01=1, SF060_01_01=12.920000000000016, SF061a_01_01=0.5039999999999907, SF061b_01_01=-0.19200000000000728, SF055_01_02=2, SF056_01_02=1, SF060_01_02=11.160000000000025, SF061a_01_02=0.4239999999999924, SF061b_01_02=-0.22400000000000375, SF055_01_03=2, SF056_01_03=1, SF060_01_03=12.800000000000011, SF061a_01_03=0.19999999999998863, SF061b_01_03=0.055999999999997385, SF055_01_04=1, SF056_01_04=1, SF060_01_04=14.720000000000027, SF061a_01_04=0.6079999999999899, SF061b_01_04=-0.3680000000000092, SF055_01_05=4, SF056_01_05=1, SF060_01_05=13.920000000000016, SF061a_01_05=0.055999999999997385, SF061b_01_05=-0.6159999999999997, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.10399999999999998, SF049a_02=0.0020000000000000018, SF049b_02=0.007000000000000006, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538880, SF055_02_01=2, SF056_02_01=1, SF060_02_01=5.080000000000041, SF061a_02_01=0.28000000000000114, SF061b_02_01=0.1839999999999975, SF055_02_02=2, SF056_02_02=1, SF060_02_02=3.1200000000000045, SF061a_02_02=0.23199999999999932, SF061b_02_02=0.0799999999999983, SF055_02_03=4, SF056_02_03=1, SF060_02_03=5.080000000000041, SF061a_02_03=-0.06400000000000716, SF061b_02_03=0.13599999999999568, SF055_02_04=3, SF056_02_04=1, SF060_02_04=5.760000000000048, SF061a_02_04=0.5039999999999907, SF061b_02_04=-0.04800000000000182, SF055_02_05=2, SF056_02_05=1, SF060_02_05=4.240000000000009, SF061a_02_05=-0.1280000000000001, SF061b_02_05=-0.2560000000000002, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.09599999999999997, SF049a_03=-0.033, SF049b_03=-0.009000000000000008, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4412538880, SF055_03_01=1, SF056_03_01=1, SF060_03_01=5.960000000000036, SF061a_03_01=0.48799999999999955, SF061b_03_01=0.11199999999999477, SF055_03_02=2, SF056_03_02=1, SF060_03_02=3.4399999999999977, SF061a_03_02=0.30400000000000205, SF061b_03_02=0.055999999999997385, SF055_03_03=4, SF056_03_03=1, SF060_03_03=5.640000000000043, SF061a_03_03=1.9279999999999973, SF061b_03_03=0.2639999999999958, SF055_03_04=1, SF056_03_04=1, SF060_03_04=5.0400000000000205, SF061a_03_04=0.7599999999999909, SF061b_03_04=-0.02400000000000091, SF055_03_05=1, SF056_03_05=1, SF060_03_05=2.5600000000000023, SF061a_03_05=0.09599999999998943, SF061b_03_05=-0.1360000000000099, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.09999999999999998, SF049a_04=0.0010000000000000009, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538880, SF055_04_01=1, SF056_04_01=1, SF060_04_01=14.480000000000018, SF061a_04_01=0.13599999999999568, SF061b_04_01=-2.0320000000000036, SF055_04_02=2, SF056_04_02=1, SF060_04_02=14.080000000000041, SF061a_04_02=0.15200000000000102, SF061b_04_02=-2.0960000000000036, SF055_04_03=1, SF056_04_03=1, SF060_04_03=13.560000000000002, SF061a_04_03=0.09599999999998943, SF061b_04_03=-1.9200000000000017, SF055_04_04=3, SF056_04_04=1, SF060_04_04=23.720000000000027, SF061a_04_04=-0.008000000000009777, SF061b_04_04=-2.504000000000005, SF055_04_05=2, SF056_04_05=1, SF060_04_05=29.160000000000025, SF061a_04_05=-0.35999999999999943, SF061b_04_05=-2.608000000000004, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.132, SF049a_05=-0.0040000000000000036, SF049b_05=0.01100000000000001, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538881, SF055_05_01=2, SF056_05_01=1, SF060_05_01=7.600000000000023, SF061a_05_01=1.5519999999999925, SF061b_05_01=-0.20000000000000284, SF055_05_02=2, SF056_05_02=1, SF060_05_02=6.760000000000048, SF061a_05_02=1.5519999999999925, SF061b_05_02=-0.2560000000000002, SF055_05_03=3, SF056_05_03=1, SF060_05_03=7.520000000000039, SF061a_05_03=1.2879999999999967, SF061b_05_03=0.0, SF055_05_04=2, SF056_05_04=1, SF060_05_04=13.439999999999998, SF061a_05_04=1.4399999999999977, SF061b_05_04=-0.5760000000000076, SF055_05_05=3, SF056_05_05=1, SF060_05_05=17.400000000000034, SF061a_05_05=0.73599999999999, SF061b_05_05=-0.9440000000000026, SF055_05_06=4, SF056_05_06=1, SF060_05_06=47.84000000000003, SF061a_05_06=0.02400000000000091, SF061b_05_06=0.14399999999999125, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0020000000000000018, SF049b_06=-0.013000000000000012, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4546756608, SF055_06_01=1, SF056_06_01=1, SF060_06_01=11.080000000000041, SF061a_06_01=0.45599999999998886, SF061b_06_01=-0.23199999999999932, SF055_06_02=4, SF056_06_02=1, SF060_06_02=60.68000000000001, SF061a_06_02=0.4719999999999942, SF061b_06_02=0.519999999999996, SF055_06_03=1, SF056_06_03=1, SF060_06_03=9.400000000000034, SF061a_06_03=0.519999999999996, SF061b_06_03=-0.26400000000001, SF055_06_04=2, SF056_06_04=1, SF060_06_04=11.800000000000011, SF061a_06_04=0.3359999999999985, SF061b_06_04=-0.17600000000000193, SF055_06_05=1, SF056_06_05=1, SF060_06_05=12.080000000000041, SF061a_06_05=0.7199999999999989, SF061b_06_05=-0.4399999999999977, SF055_06_06=2, SF056_06_06=1, SF060_06_06=12.680000000000007, SF061a_06_06=0.2560000000000002, SF061b_06_06=-0.6159999999999997, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=2, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=0.0010000000000000009, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538880, SF055_07_01=1, SF056_07_01=1, SF060_07_01=15.720000000000027, SF061a_07_01=1.039999999999992, SF061b_07_01=-0.09600000000000364, SF055_07_02=1, SF056_07_02=1, SF060_07_02=13.720000000000027, SF061a_07_02=1.024000000000001, SF061b_07_02=-0.09600000000000364, SF055_07_03=1, SF056_07_03=1, SF060_07_03=17.04000000000002, SF061a_07_03=0.8799999999999955, SF061b_07_03=-0.1280000000000001, SF055_07_04=1, SF056_07_04=1, SF060_07_04=15.319999999999993, SF061a_07_04=1.0719999999999885, SF061b_07_04=-0.21600000000000819, SF055_07_05=1, SF056_07_05=1, SF060_07_05=15.120000000000005, SF061a_07_05=0.8079999999999927, SF061b_07_05=-0.45600000000000307, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.07199999999999995, SF049a_08=0.006000000000000005, SF049b_08=0.016000000000000014, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4412538880, SF055_08_01=1, SF056_08_01=1, SF060_08_01=15.520000000000039, SF061a_08_01=1.0559999999999974, SF061b_08_01=-0.03200000000001069, SF055_08_02=1, SF056_08_02=1, SF060_08_02=13.080000000000041, SF061a_08_02=1.0, SF061b_08_02=-0.16800000000000637, SF055_08_03=1, SF056_08_03=1, SF060_08_03=16.52000000000004, SF061a_08_03=0.8559999999999945, SF061b_08_03=-0.1039999999999992, SF055_08_04=1, SF056_08_04=1, SF060_08_04=14.160000000000025, SF061a_08_04=1.1039999999999992, SF061b_08_04=-0.2560000000000002, SF055_08_05=1, SF056_08_05=1, SF060_08_05=13.28000000000003, SF061a_08_05=0.671999999999997, SF061b_08_05=-0.30400000000000205, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.17600000000000005, SF049a_09=-0.01899999999999999, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4546756608, SF055_09_01=1, SF056_09_01=1, SF060_09_01=9.0, SF061a_09_01=0.5600000000000023, SF061b_09_01=-0.1600000000000108, SF055_09_02=3, SF056_09_02=1, SF060_09_02=61.160000000000025, SF061a_09_02=-0.480000000000004, SF061b_09_02=0.6640000000000015, SF055_09_03=1, SF056_09_03=1, SF060_09_03=7.080000000000041, SF061a_09_03=0.671999999999997, SF061b_09_03=-0.28000000000000114, SF055_09_04=2, SF056_09_04=1, SF060_09_04=10.160000000000025, SF061a_09_04=0.4959999999999951, SF061b_09_04=-0.1280000000000001, SF055_09_05=2, SF056_09_05=1, SF060_09_05=9.360000000000014, SF061a_09_05=0.6559999999999917, SF061b_09_05=-0.5600000000000023, SF055_09_06=2, SF056_09_06=1, SF060_09_06=10.520000000000039, SF061a_09_06=0.6400000000000006, SF061b_09_06=-0.6480000000000103, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=3, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.124, SF049a_10=0.010000000000000009, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538888, SF055_10_01=1, SF056_10_01=1, SF060_10_01=12.080000000000041, SF061a_10_01=0.9200000000000017, SF061b_10_01=-0.11200000000000898, SF055_10_02=1, SF056_10_02=1, SF060_10_02=10.160000000000025, SF061a_10_02=0.9039999999999964, SF061b_10_02=-0.08800000000000807, SF055_10_03=1, SF056_10_03=1, SF060_10_03=13.640000000000043, SF061a_10_03=0.8239999999999981, SF061b_10_03=-0.2079999999999984, SF055_10_04=1, SF056_10_04=1, SF060_10_04=11.560000000000002, SF061a_10_04=0.8319999999999936, SF061b_10_04=-0.2560000000000002, SF055_10_05=1, SF056_10_05=1, SF060_10_05=11.400000000000034, SF061a_10_05=0.9839999999999947, SF061b_10_05=-0.3359999999999985, SF055_10_06=5, SF056_10_06=1, SF060_10_06=68.76000000000005, SF061a_10_06=-4.496000000000002, SF061b_10_06=-3.5520000000000067)>",
-            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=87, eaf=0, crcType=2, frameCrc=2, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=5702700, SF005=354, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.008000000000000007, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=-0.008000000000000007, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538880, SF055_01_01=2, SF056_01_01=1, SF060_01_01=-4.0, SF061a_01_01=0.24799999999999045, SF061b_01_01=-0.20000000000000284, SF055_01_02=1, SF056_01_02=1, SF060_01_02=-6.9599999999999795, SF061a_01_02=0.1839999999999975, SF061b_01_02=-0.2400000000000091, SF055_01_03=1, SF056_01_03=1, SF060_01_03=-5.639999999999986, SF061a_01_03=-0.06400000000000716, SF061b_01_03=-0.26400000000001, SF055_01_04=2, SF056_01_04=1, SF060_01_04=-4.0, SF061a_01_04=0.5759999999999934, SF061b_01_04=-0.3359999999999985, SF055_01_05=1, SF056_01_05=1, SF060_01_05=-9.439999999999998, SF061a_01_05=-0.07200000000000273, SF061b_01_05=-0.4720000000000084, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.16400000000000003, SF049a_02=-0.0010000000000000009, SF049b_02=0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538880, SF055_02_01=2, SF056_02_01=1, SF060_02_01=-3.599999999999966, SF061a_02_01=0.19999999999998863, SF061b_02_01=-0.20000000000000284, SF055_02_02=1, SF056_02_02=1, SF060_02_02=-6.839999999999975, SF061a_02_02=0.09599999999998943, SF061b_02_02=-0.30400000000000205, SF055_02_03=1, SF056_02_03=1, SF060_02_03=-6.079999999999984, SF061a_02_03=-0.1360000000000099, SF061b_02_03=-0.27200000000000557, SF055_02_04=1, SF056_02_04=1, SF060_02_04=-3.1200000000000045, SF061a_02_04=0.45599999999998886, SF061b_02_04=-0.35999999999999943, SF055_02_05=1, SF056_02_05=1, SF060_02_05=-9.879999999999995, SF061a_02_05=-0.03200000000001069, SF061b_02_05=-0.480000000000004)>",
-            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=180, eaf=0, crcType=2, frameCrc=4, msgSubtype=0, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=736926, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=882933762, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF018_01=45, SF020R_01=0.13599999999999923, SF020A_01=-1.426000000000002, SF020C_01=0.045999999999999375, SF022_01=7, SF020CK_01=6.782, SF024_01=2, PhaseBiasBitmaskLen_01=0, SF025_01=60, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.6660000000000004, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.6660000000000004, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.6359999999999992, CodeBiasBitmaskLen_01=0, SF027_01=60, SF029_01_01=-2.280000000000001, SF029_01_02=-0.35999999999999943, SF029_01_03=-0.240000000000002, SF029_01_04=-2.4800000000000004, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF018_02=189, SF020R_02=-0.652000000000001, SF020A_02=-0.07000000000000028, SF020C_02=0.1039999999999992, SF022_02=7, SF020CK_02=3.041999999999998, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF025_02=60, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=1.5879999999999974, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=1.5879999999999974, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=1.6039999999999992, CodeBiasBitmaskLen_02=0, SF027_02=60, SF029_02_01=-3.1400000000000006, SF029_02_02=-2.280000000000001, SF029_02_03=-2.460000000000001, SF029_02_04=-1.1999999999999993, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF018_03=48, SF020R_03=-0.23200000000000287, SF020A_03=1.9899999999999984, SF020C_03=-0.0020000000000024443, SF022_03=7, SF020CK_03=1.8399999999999999, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF025_03=60, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=-0.23799999999999955, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=-0.23799999999999955, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=-0.272000000000002, CodeBiasBitmaskLen_03=0, SF027_03=60, SF029_03_01=0.5999999999999979, SF029_03_02=2.84, SF029_03_03=3.099999999999998, SF029_03_04=0.9199999999999982, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF018_04=5, SF020R_04=0.14399999999999835, SF020A_04=0.27399999999999736, SF020C_04=0.2759999999999998, SF022_04=7, SF020CK_04=2.8959999999999972, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF025_04=60, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=-0.17800000000000082, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=-0.17800000000000082, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=-0.1620000000000026, CodeBiasBitmaskLen_04=0, SF027_04=60, SF029_04_01=0.16000000000000014, SF029_04_02=1.4400000000000013, SF029_04_03=1.2800000000000011, SF029_04_04=-0.6000000000000014, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=6, SF018_05=108, SF020R_05=-0.7500000000000018, SF020A_05=-0.6400000000000006, SF020C_05=0.2560000000000002, SF022_05=6, SF020CK_05=-1.7180000000000017, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF025_05=60, SF023_05_01=1, SF015_05_01=6, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=6, SF020PB_05_02=0.27199999999999847, SF023_05_03=1, SF015_05_03=6, SF020PB_05_03=0.27199999999999847, SF023_05_04=1, SF015_05_04=6, SF020PB_05_04=0.6219999999999999, CodeBiasBitmaskLen_05=0, SF027_05=60, SF029_05_01=-0.120000000000001, SF029_05_02=-0.08000000000000185, SF029_05_03=-0.1999999999999993, SF029_05_04=1.5399999999999991, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF018_06=44, SF020R_06=-0.18599999999999994, SF020A_06=0.6459999999999972, SF020C_06=-0.24399999999999977, SF022_06=7, SF020CK_06=-1.3300000000000018, SF024_06=3, PhaseBiasBitmaskLen_06=0, SF025_06=56, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=-0.03400000000000247, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=-0.03400000000000247, CodeBiasBitmaskLen_06=0, SF027_06=56, SF029_06_01=0.16000000000000014, SF029_06_02=-0.7800000000000011, SF029_06_03=-0.8399999999999999, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF018_07=32, SF020R_07=0.11199999999999832, SF020A_07=-0.48600000000000065, SF020C_07=0.4659999999999975, SF022_07=7, SF020CK_07=-1.474000000000002, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF025_07=56, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=0.2579999999999991, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=0.2579999999999991, CodeBiasBitmaskLen_07=0, SF027_07=56, SF029_07_01=-0.9200000000000017, SF029_07_02=-2.0199999999999996, SF029_07_03=-1.9800000000000004)>",
-            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=152, eaf=0, crcType=2, frameCrc=15, msgSubtype=1, timeTagtype=1, gnssTimeTag=452211642, solutionId=5, solutionProcId=11, crc=7233776, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=8618373, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF019_01=89, SF020R_01=0.2839999999999989, SF020A_01=2.2779999999999987, SF020C_01=-1.910000000000002, SF022_01=7, SF020CK_01=-3.4040000000000017, SF024_01=2, PhaseBiasBitmaskLen_01=0, SF026_01=24, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=-0.5800000000000018, CodeBiasBitmaskLen_01=0, SF028_01=24, SF029_01_01=1.120000000000001, SF029_01_02=1.9199999999999982, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF019_02=89, SF020R_02=0.129999999999999, SF020A_02=0.6459999999999972, SF020C_02=0.8780000000000001, SF022_02=7, SF020CK_02=-0.7900000000000009, SF024_02=2, PhaseBiasBitmaskLen_02=0, SF026_02=24, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.4480000000000004, CodeBiasBitmaskLen_02=0, SF028_02=24, SF029_02_01=-0.6799999999999997, SF029_02_02=-0.5599999999999987, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF019_03=89, SF020R_03=-0.013999999999999346, SF020A_03=3.0159999999999982, SF020C_03=0.8580000000000005, SF022_03=7, SF020CK_03=4.366, SF024_03=2, PhaseBiasBitmaskLen_03=0, SF026_03=24, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.34199999999999875, CodeBiasBitmaskLen_03=0, SF028_03=24, SF029_03_01=-1.6000000000000014, SF029_03_02=-2.400000000000002, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF019_04=89, SF020R_04=0.7519999999999989, SF020A_04=6.013999999999999, SF020C_04=-3.1860000000000017, SF022_04=7, SF020CK_04=5.2940000000000005, SF024_04=2, PhaseBiasBitmaskLen_04=0, SF026_04=24, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.19399999999999906, CodeBiasBitmaskLen_04=0, SF028_04=24, SF029_04_01=-0.5599999999999987, SF029_04_02=-0.9600000000000009, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF019_05=89, SF020R_05=0.01799999999999713, SF020A_05=-5.796000000000001, SF020C_05=-0.1460000000000008, SF022_05=7, SF020CK_05=1.1119999999999983, SF024_05=2, PhaseBiasBitmaskLen_05=0, SF026_05=24, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=-0.1460000000000008, CodeBiasBitmaskLen_05=0, SF028_05=24, SF029_05_01=-0.5199999999999996, SF029_05_02=-0.10000000000000142, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=6, SF019_06=89, SF020R_06=0.5339999999999989, SF020A_06=-0.5640000000000018, SF020C_06=0.6739999999999995, SF022_06=6, SF020CK_06=-1.838000000000001, SF024_06=1, PhaseBiasBitmaskLen_06=0, SF026_06=24, SF023_06_01=1, SF015_06_01=6, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=6, SF020PB_06_02=-0.15000000000000213, CodeBiasBitmaskLen_06=0, SF028_06=24, SF029_06_01=0.03999999999999915, SF029_06_02=-0.03999999999999915, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF019_07=89, SF020R_07=1.4540000000000006, SF020A_07=-1.5180000000000007, SF020C_07=-1.200000000000001, SF022_07=7, SF020CK_07=-2.694000000000001, SF024_07=4, PhaseBiasBitmaskLen_07=0, SF026_07=24, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.7660000000000018, CodeBiasBitmaskLen_07=0, SF028_07=24, SF029_07_01=2.919999999999998, SF029_07_02=2.1799999999999997, SF013_08=0, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=7, SF019_08=89, SF020R_08=0.597999999999999, SF020A_08=0.15399999999999991, SF020C_08=0.5239999999999974, SF022_08=7, SF020CK_08=-1.6560000000000006, SF024_08=2, PhaseBiasBitmaskLen_08=0, SF026_08=24, SF023_08_01=1, SF015_08_01=7, SF020PB_08_01=0.0, SF023_08_02=1, SF015_08_02=7, SF020PB_08_02=-0.5660000000000007, CodeBiasBitmaskLen_08=0, SF028_08=24, SF029_08_01=1.379999999999999, SF029_08_02=1.259999999999998)>",
-            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=193, eaf=0, crcType=2, frameCrc=3, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=6801214, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF097=0, SatBitmaskLen=1, SF094=184555012, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF100_01=95, SF020R_01=0.24599999999999866, SF020A_01=0.20599999999999952, SF020C_01=-0.28000000000000114, SF022_01=7, SF020CK_01=2.9399999999999977, SF024_01=3, PhaseBiasBitmaskLen_01=0, SF103_01=232, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.7999999999999972, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.7799999999999976, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.0, CodeBiasBitmaskLen_01=0, SF106_01=232, SF029_01_01=-1.1799999999999997, SF029_01_02=-2.620000000000001, SF029_01_03=-2.620000000000001, SF029_01_04=-1.1799999999999997, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF100_02=95, SF020R_02=0.3379999999999974, SF020A_02=-0.08200000000000074, SF020C_02=-0.4380000000000006, SF022_02=7, SF020CK_02=4.047999999999998, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF103_02=232, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.7680000000000007, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=0.7479999999999976, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=0.0, CodeBiasBitmaskLen_02=0, SF106_02=232, SF029_02_01=-1.4000000000000021, SF029_02_02=-4.0, SF029_02_03=-4.0, SF029_02_04=-1.4000000000000021, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF100_03=95, SF020R_03=-0.240000000000002, SF020A_03=0.029999999999997584, SF020C_03=-0.34800000000000253, SF022_03=7, SF020CK_03=4.07, SF024_03=3, PhaseBiasBitmaskLen_03=0, SF103_03=232, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.6899999999999977, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=0.6720000000000006, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=0.0, CodeBiasBitmaskLen_03=0, SF106_03=232, SF029_03_01=-1.0199999999999996, SF029_03_02=-5.32, SF029_03_03=-5.32, SF029_03_04=-1.0199999999999996, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF100_04=95, SF020R_04=-0.1460000000000008, SF020A_04=0.2539999999999978, SF020C_04=0.347999999999999, SF022_04=7, SF020CK_04=-3.0100000000000016, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF103_04=232, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=-0.1479999999999997, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=-0.1460000000000008, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=0.0, CodeBiasBitmaskLen_04=0, SF106_04=232, SF029_04_01=0.14000000000000057, SF029_04_02=-0.26000000000000156, SF029_04_03=-0.26000000000000156, SF029_04_04=0.14000000000000057, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF100_05=95, SF020R_05=-0.15399999999999991, SF020A_05=-0.26399999999999935, SF020C_05=-0.2140000000000022, SF022_05=7, SF020CK_05=-5.328000000000001, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF103_05=232, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.8580000000000005, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=0.8359999999999985, SF023_05_04=1, SF015_05_04=7, SF020PB_05_04=0.0, CodeBiasBitmaskLen_05=0, SF106_05=232, SF029_05_01=-0.40000000000000213, SF029_05_02=6.140000000000001, SF029_05_03=6.140000000000001, SF029_05_04=-0.40000000000000213, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF100_06=95, SF020R_06=-0.38000000000000256, SF020A_06=-0.28800000000000026, SF020C_06=0.045999999999999375, SF022_06=7, SF020CK_06=-4.3580000000000005, SF024_06=2, PhaseBiasBitmaskLen_06=0, SF103_06=232, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=0.7880000000000003, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=0.7680000000000007, SF023_06_04=1, SF015_06_04=7, SF020PB_06_04=0.0, CodeBiasBitmaskLen_06=0, SF106_06=232, SF029_06_01=-1.4800000000000004, SF029_06_02=2.259999999999998, SF029_06_03=2.259999999999998, SF029_06_04=-1.4800000000000004, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF100_07=95, SF020R_07=0.1319999999999979, SF020A_07=0.3739999999999988, SF020C_07=0.4259999999999984, SF022_07=7, SF020CK_07=-1.6240000000000006, SF024_07=3, PhaseBiasBitmaskLen_07=0, SF103_07=232, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.0779999999999994, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=-0.07600000000000051, SF023_07_04=1, SF015_07_04=7, SF020PB_07_04=0.0, CodeBiasBitmaskLen_07=0, SF106_07=232, SF029_07_01=0.7800000000000011, SF029_07_02=0.33999999999999986, SF029_07_03=0.33999999999999986, SF029_07_04=0.7800000000000011)>",
+            "<SPARTN(SPARTN-1X-HPAC-BEI, msgType=1, nData=369, eaf=0, crcType=2, frameCrc=14, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=4347676, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.16800000000000004, SF049a_01=-0.0010000000000000009, SF049b_01=-0.015999999999999986, SF054_01=1, SatBitmaskLen_01=0, SF094_01=32768, PRN_01_01=22, SF055_01_01=1, SF056_01_01=1, SF060_01_01=8.960000000000036, SF061a_01_01=0.1599999999999966, SF061b_01_01=0.3999999999999915, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.10399999999999998, SF049a_02=0.0020000000000000018, SF049b_02=0.007000000000000006, SF054_02=1, SatBitmaskLen_02=1, SF094_02=184554500, PRN_02_01=19, SF055_02_01=3, SF056_02_01=1, SF060_02_01=9.800000000000011, SF061a_02_01=-0.38400000000000034, SF061b_02_01=-0.4399999999999977, PRN_02_02=21, SF055_02_02=4, SF056_02_02=1, SF060_02_02=28.480000000000018, SF061a_02_02=-0.4720000000000084, SF061b_02_02=0.37599999999999056, PRN_02_03=22, SF055_02_03=3, SF056_02_03=1, SF060_02_03=3.5200000000000387, SF061a_02_03=-0.24800000000000466, SF061b_02_03=0.0799999999999983, PRN_02_04=34, SF055_02_04=4, SF056_02_04=1, SF060_02_04=27.640000000000043, SF061a_02_04=-1.0080000000000098, SF061b_02_04=0.3359999999999985, PRN_02_05=36, SF055_02_05=2, SF056_02_05=1, SF060_02_05=22.319999999999993, SF061a_02_05=0.37599999999999056, SF061b_02_05=-0.6080000000000041, PRN_02_06=44, SF055_02_06=4, SF056_02_06=1, SF060_02_06=15.760000000000048, SF061a_02_06=0.1039999999999992, SF061b_02_06=0.22399999999998954, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.09599999999999997, SF049a_03=-0.033, SF049b_03=-0.009000000000000008, SF054_03=1, SatBitmaskLen_03=1, SF094_03=184550404, PRN_03_01=19, SF055_03_01=1, SF056_03_01=1, SF060_03_01=7.28000000000003, SF061a_03_01=-0.4480000000000075, SF061b_03_01=-0.26400000000001, PRN_03_02=21, SF055_03_02=5, SF056_03_02=1, SF060_03_02=30.52000000000004, SF061a_03_02=0.07199999999998852, SF061b_03_02=0.30400000000000205, PRN_03_03=22, SF055_03_03=1, SF056_03_03=1, SF060_03_03=3.5600000000000023, SF061a_03_03=-0.0799999999999983, SF061b_03_03=-0.03200000000001069, PRN_03_04=36, SF055_03_04=2, SF056_03_04=1, SF060_03_04=17.319999999999993, SF061a_03_04=0.30400000000000205, SF061b_03_04=-0.6159999999999997, PRN_03_05=44, SF055_03_05=1, SF056_03_05=1, SF060_03_05=17.760000000000048, SF061a_03_05=0.28000000000000114, SF061b_03_05=0.3359999999999985, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.09999999999999998, SF049a_04=0.0010000000000000009, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=1, SF094_04=50335748, PRN_04_01=21, SF055_04_01=4, SF056_04_01=1, SF060_04_01=28.08000000000004, SF061a_04_01=0.02400000000000091, SF061b_04_01=-1.784000000000006, PRN_04_02=22, SF055_04_02=4, SF056_04_02=1, SF060_04_02=13.480000000000018, SF061a_04_02=0.35199999999998965, SF061b_04_02=-2.3600000000000065, PRN_04_03=34, SF055_04_03=5, SF056_04_03=1, SF060_04_03=32.160000000000025, SF061a_04_03=-0.2560000000000002, SF061b_04_03=-1.7360000000000042, PRN_04_04=44, SF055_04_04=4, SF056_04_04=1, SF060_04_04=20.480000000000018, SF061a_04_04=0.5519999999999925, SF061b_04_04=-1.9680000000000035, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.132, SF049a_05=-0.0040000000000000036, SF049b_05=0.01100000000000001, SF054_05=1, SatBitmaskLen_05=1, SF094_05=50335748, PRN_05_01=21, SF055_05_01=1, SF056_05_01=1, SF060_05_01=19.439999999999998, SF061a_05_01=1.3119999999999976, SF061b_05_01=-0.35999999999999943, PRN_05_02=22, SF055_05_02=1, SF056_05_02=1, SF060_05_02=3.080000000000041, SF061a_05_02=1.583999999999989, SF061b_05_02=-0.9680000000000035, PRN_05_03=34, SF055_05_03=4, SF056_05_03=1, SF060_05_03=23.760000000000048, SF061a_05_03=0.8239999999999981, SF061b_05_03=-0.48799999999999955, PRN_05_04=44, SF055_05_04=3, SF056_05_04=1, SF060_05_04=10.720000000000027, SF061a_05_04=1.7920000000000016, SF061b_05_04=-0.7120000000000033, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0020000000000000018, SF049b_06=-0.013000000000000012, SF054_06=1, SatBitmaskLen_06=0, SF094_06=98304, PRN_06_01=21, SF055_06_01=5, SF056_06_01=1, SF060_06_01=32.44, SF061a_06_01=-0.0799999999999983, SF061b_06_01=0.5759999999999934, PRN_06_02=22, SF055_06_02=1, SF056_06_02=1, SF060_06_02=8.640000000000043, SF061a_06_02=0.2560000000000002, SF061b_06_02=0.24799999999999045, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=2, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=0.0010000000000000009, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=1, SF094_07=184550404, PRN_07_01=19, SF055_07_01=1, SF056_07_01=1, SF060_07_01=12.04000000000002, SF061a_07_01=1.0959999999999894, SF061b_07_01=-0.2400000000000091, PRN_07_02=21, SF055_07_02=1, SF056_07_02=1, SF060_07_02=32.04000000000002, SF061a_07_02=0.5919999999999987, SF061b_07_02=0.6400000000000006, PRN_07_03=22, SF055_07_03=1, SF056_07_03=1, SF060_07_03=6.240000000000009, SF061a_07_03=1.2719999999999914, SF061b_07_03=0.19999999999998863, PRN_07_04=36, SF055_07_04=4, SF056_07_04=1, SF060_07_04=21.640000000000043, SF061a_07_04=1.176000000000002, SF061b_07_04=0.14399999999999125, PRN_07_05=44, SF055_07_05=2, SF056_07_05=1, SF060_07_05=18.480000000000018, SF061a_07_05=1.3519999999999897, SF061b_07_05=0.15200000000000102, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.07199999999999995, SF049a_08=0.006000000000000005, SF049b_08=0.016000000000000014, SF054_08=1, SatBitmaskLen_08=1, SF094_08=184550404, PRN_08_01=19, SF055_08_01=2, SF056_08_01=1, SF060_08_01=11.520000000000039, SF061a_08_01=1.024000000000001, SF061b_08_01=0.015999999999991132, PRN_08_02=21, SF055_08_02=2, SF056_08_02=1, SF060_08_02=35.879999999999995, SF061a_08_02=0.5360000000000014, SF061b_08_02=0.9119999999999919, PRN_08_03=22, SF055_08_03=2, SF056_08_03=1, SF060_08_03=7.160000000000025, SF061a_08_03=1.1039999999999992, SF061b_08_03=0.16799999999999216, PRN_08_04=36, SF055_08_04=4, SF056_08_04=1, SF060_08_04=20.480000000000018, SF061a_08_04=0.7599999999999909, SF061b_08_04=-0.6480000000000103, PRN_08_05=44, SF055_08_05=1, SF056_08_05=1, SF060_08_05=20.04000000000002, SF061a_08_05=1.5360000000000014, SF061b_08_05=0.5600000000000023, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.17600000000000005, SF049a_09=-0.01899999999999999, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF094_09=98304, PRN_09_01=21, SF055_09_01=3, SF056_09_01=1, SF060_09_01=34.04000000000002, SF061a_09_01=-0.2960000000000065, SF061b_09_01=0.21599999999999397, PRN_09_02=22, SF055_09_02=1, SF056_09_02=1, SF060_09_02=7.840000000000032, SF061a_09_02=0.32799999999998875, SF061b_09_02=0.30400000000000205, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=3, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.124, SF049a_10=0.010000000000000009, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=1, SF094_10=184550404, PRN_10_01=19, SF055_10_01=1, SF056_10_01=1, SF060_10_01=7.8799999999999955, SF061a_10_01=1.2800000000000011, SF061b_10_01=0.08799999999999386, PRN_10_02=21, SF055_10_02=1, SF056_10_02=1, SF060_10_02=30.200000000000045, SF061a_10_02=1.063999999999993, SF061b_10_02=0.9119999999999919, PRN_10_03=22, SF055_10_03=1, SF056_10_03=1, SF060_10_03=2.0400000000000205, SF061a_10_03=1.2959999999999923, SF061b_10_03=0.4159999999999968, PRN_10_04=36, SF055_10_04=1, SF056_10_04=1, SF060_10_04=16.0, SF061a_10_04=1.519999999999996, SF061b_10_04=-0.6800000000000068, PRN_10_05=44, SF055_10_05=1, SF056_10_05=1, SF060_10_05=14.400000000000034, SF061a_10_05=1.2079999999999984, SF061b_10_05=0.5039999999999907)>",
+            "<SPARTN(SPARTN-1X-HPAC-BEI, msgType=1, nData=101, eaf=0, crcType=2, frameCrc=7, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=3165361, SF005=354, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.008000000000000007, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=-0.008000000000000007, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=1, SF094_01=184554500, PRN_01_01=19, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-9.680000000000007, SF061a_01_01=-0.7920000000000016, SF061b_01_01=-0.5679999999999978, PRN_01_02=21, SF055_01_02=2, SF056_01_02=1, SF060_01_02=15.560000000000002, SF061a_01_02=-0.5120000000000005, SF061b_01_02=0.1839999999999975, PRN_01_03=22, SF055_01_03=1, SF056_01_03=1, SF060_01_03=-12.079999999999984, SF061a_01_03=-0.43200000000000216, SF061b_01_03=-0.24800000000000466, PRN_01_04=34, SF055_01_04=3, SF056_01_04=1, SF060_01_04=10.360000000000014, SF061a_01_04=-1.5360000000000014, SF061b_01_04=-0.1600000000000108, PRN_01_05=36, SF055_01_05=1, SF056_01_05=1, SF060_01_05=5.1200000000000045, SF061a_01_05=0.27199999999999136, SF061b_01_05=-0.8640000000000043, PRN_01_06=44, SF055_01_06=1, SF056_01_06=1, SF060_01_06=3.8799999999999955, SF061a_01_06=-0.06400000000000716, SF061b_01_06=0.1599999999999966, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.16400000000000003, SF049a_02=-0.0010000000000000009, SF049b_02=0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=1, SF094_02=184554500, PRN_02_01=19, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-11.560000000000002, SF061a_02_01=-0.632000000000005, SF061b_02_01=-0.5440000000000111, PRN_02_02=21, SF055_02_02=3, SF056_02_02=1, SF060_02_02=14.360000000000014, SF061a_02_02=-0.6400000000000006, SF061b_02_02=0.16799999999999216, PRN_02_03=22, SF055_02_03=1, SF056_02_03=1, SF060_02_03=-13.239999999999952, SF061a_02_03=-0.45600000000000307, SF061b_02_03=-0.2880000000000109, PRN_02_04=34, SF055_02_04=2, SF056_02_04=1, SF060_02_04=7.0, SF061a_02_04=-1.4639999999999986, SF061b_02_04=-0.08800000000000807, PRN_02_05=36, SF055_02_05=2, SF056_02_05=1, SF060_02_05=4.8799999999999955, SF061a_02_05=-0.008000000000009777, SF061b_02_05=-0.847999999999999, PRN_02_06=44, SF055_02_06=1, SF056_02_06=1, SF060_02_06=3.7200000000000273, SF061a_02_06=-0.1600000000000108, SF061b_02_06=0.1039999999999992)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=536, eaf=0, crcType=2, frameCrc=14, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=4199949, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.15200000000000002, SF049a_01=-0.0020000000000000018, SF049b_01=-0.0040000000000000036, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412539457, PRN_01_01=4, SF055_01_01=1, SF056_01_01=1, SF060_01_01=3.160000000000025, SF061a_01_01=0.43200000000000216, SF061b_01_01=0.1599999999999966, PRN_01_02=10, SF055_01_02=2, SF056_01_02=1, SF060_01_02=0.6800000000000068, SF061a_01_02=0.19199999999999307, SF061b_01_02=0.08799999999999386, PRN_01_03=11, SF055_01_03=4, SF056_01_03=1, SF060_01_03=-0.7999999999999545, SF061a_01_03=1.0480000000000018, SF061b_01_03=0.1039999999999992, PRN_01_04=12, SF055_01_04=1, SF056_01_04=1, SF060_01_04=7.360000000000014, SF061a_01_04=1.4959999999999951, SF061b_01_04=-0.1360000000000099, PRN_01_05=19, SF055_01_05=3, SF056_01_05=1, SF060_01_05=-0.3599999999999568, SF061a_01_05=0.23999999999999488, SF061b_01_05=-0.1600000000000108, PRN_01_06=27, SF055_01_06=4, SF056_01_06=1, SF060_01_06=17.04000000000002, SF061a_01_06=-0.38400000000000034, SF061b_01_06=-0.6240000000000094, PRN_01_07=30, SF055_01_07=4, SF056_01_07=1, SF060_01_07=24.80000000000001, SF061a_01_07=-1.0480000000000018, SF061b_01_07=-0.32800000000000296, PRN_01_08=36, SF055_01_08=4, SF056_01_08=1, SF060_01_08=13.680000000000007, SF061a_01_08=0.847999999999999, SF061b_01_08=0.4479999999999933, SF031_02=1, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.0, SF044_02=1, SF048_02=-0.128, SF049a_02=0.0010000000000000009, SF049b_02=-0.0030000000000000027, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412539457, PRN_02_01=4, SF055_02_01=5, SF056_02_01=1, SF060_02_01=-1.2399999999999523, SF061a_02_01=2.3359999999999985, SF061b_02_01=0.0, PRN_02_02=10, SF055_02_02=4, SF056_02_02=1, SF060_02_02=-2.839999999999975, SF061a_02_02=2.128, SF061b_02_02=-0.1600000000000108, PRN_02_03=11, SF055_02_03=4, SF056_02_03=1, SF060_02_03=-3.7199999999999704, SF061a_02_03=0.2079999999999984, SF061b_02_03=0.14399999999999125, PRN_02_04=12, SF055_02_04=5, SF056_02_04=1, SF060_02_04=2.4399999999999977, SF061a_02_04=2.304000000000002, SF061b_02_04=-0.35999999999999943, PRN_02_05=19, SF055_02_05=4, SF056_02_05=1, SF060_02_05=-1.5600000000000023, SF061a_02_05=0.4959999999999951, SF061b_02_05=-0.04800000000000182, PRN_02_06=27, SF055_02_06=1, SF056_02_06=1, SF060_02_06=20.400000000000034, SF061a_02_06=0.14399999999999125, SF061b_02_06=-0.35200000000000387, PRN_02_07=30, SF055_02_07=5, SF056_02_07=1, SF060_02_07=27.120000000000005, SF061a_02_07=0.19999999999998863, SF061b_02_07=0.04800000000000182, PRN_02_08=36, SF055_02_08=4, SF056_02_08=1, SF060_02_08=10.680000000000007, SF061a_02_08=0.19199999999999307, SF061b_02_08=0.3999999999999915, SF031_03=2, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=1, SF043_03=0.0, SF044_03=1, SF048_03=-0.14800000000000002, SF049a_03=-0.015000000000000013, SF049b_03=0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4412539457, PRN_03_01=4, SF055_03_01=5, SF056_03_01=1, SF060_03_01=-0.5600000000000023, SF061a_03_01=2.7039999999999935, SF061b_03_01=0.0799999999999983, PRN_03_02=10, SF055_03_02=5, SF056_03_02=1, SF060_03_02=-2.0399999999999636, SF061a_03_02=2.1999999999999886, SF061b_03_02=0.08799999999999386, PRN_03_03=11, SF055_03_03=4, SF056_03_03=1, SF060_03_03=-1.3999999999999773, SF061a_03_03=0.1039999999999992, SF061b_03_03=0.03999999999999204, PRN_03_04=12, SF055_03_04=5, SF056_03_04=1, SF060_03_04=1.6400000000000432, SF061a_03_04=1.3119999999999976, SF061b_03_04=-0.03200000000001069, PRN_03_05=19, SF055_03_05=5, SF056_03_05=1, SF060_03_05=-2.0, SF061a_03_05=0.27199999999999136, SF061b_03_05=-0.08800000000000807, PRN_03_06=27, SF055_03_06=4, SF056_03_06=1, SF060_03_06=14.400000000000034, SF061a_03_06=0.2879999999999967, SF061b_03_06=-0.7680000000000007, PRN_03_07=30, SF055_03_07=4, SF056_03_07=1, SF060_03_07=26.80000000000001, SF061a_03_07=-0.7280000000000086, SF061b_03_07=-0.2079999999999984, PRN_03_08=36, SF055_03_08=1, SF056_03_08=1, SF060_03_08=13.760000000000048, SF061a_03_08=0.07199999999998852, SF061b_03_08=0.367999999999995, SF031_04=3, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.0, SF044_04=1, SF048_04=-0.124, SF049a_04=0.0030000000000000027, SF049b_04=-0.0010000000000000009, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412539457, PRN_04_01=4, SF055_04_01=4, SF056_04_01=1, SF060_04_01=1.3600000000000136, SF061a_04_01=-1.480000000000004, SF061b_04_01=0.2079999999999984, PRN_04_02=10, SF055_04_02=4, SF056_04_02=1, SF060_04_02=-1.599999999999966, SF061a_04_02=-1.328000000000003, SF061b_04_02=0.24799999999999045, PRN_04_03=11, SF055_04_03=4, SF056_04_03=1, SF060_04_03=-4.359999999999957, SF061a_04_03=2.7920000000000016, SF061b_04_03=0.3359999999999985, PRN_04_04=12, SF055_04_04=4, SF056_04_04=1, SF060_04_04=9.920000000000016, SF061a_04_04=0.1039999999999992, SF061b_04_04=0.15200000000000102, PRN_04_05=19, SF055_04_05=4, SF056_04_05=1, SF060_04_05=-0.9199999999999591, SF061a_04_05=3.1119999999999948, SF061b_04_05=0.0799999999999983, PRN_04_06=27, SF055_04_06=5, SF056_04_06=1, SF060_04_06=27.80000000000001, SF061a_04_06=1.3199999999999932, SF061b_04_06=-0.784000000000006, PRN_04_07=30, SF055_04_07=5, SF056_04_07=1, SF060_04_07=29.439999999999998, SF061a_04_07=0.4959999999999951, SF061b_04_07=0.8399999999999892, PRN_04_08=36, SF055_04_08=3, SF056_04_08=1, SF060_04_08=11.879999999999995, SF061a_04_08=1.1359999999999957, SF061b_04_08=0.5999999999999943, SF031_05=4, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.0, SF044_05=1, SF048_05=-0.14, SF049a_05=0.0020000000000000018, SF049b_05=-0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412539457, PRN_05_01=4, SF055_05_01=4, SF056_05_01=1, SF060_05_01=6.1200000000000045, SF061a_05_01=-0.1039999999999992, SF061b_05_01=0.37599999999999056, PRN_05_02=10, SF055_05_02=5, SF056_05_02=1, SF060_05_02=1.4399999999999977, SF061a_05_02=-1.6720000000000041, SF061b_05_02=0.21599999999999397, PRN_05_03=11, SF055_05_03=4, SF056_05_03=1, SF060_05_03=0.040000000000020464, SF061a_05_03=2.5519999999999925, SF061b_05_03=0.4239999999999924, PRN_05_04=12, SF055_05_04=2, SF056_05_04=1, SF060_05_04=10.319999999999993, SF061a_05_04=0.46399999999999864, SF061b_05_04=0.04800000000000182, PRN_05_05=19, SF055_05_05=3, SF056_05_05=1, SF060_05_05=1.0, SF061a_05_05=3.087999999999994, SF061b_05_05=0.24799999999999045, PRN_05_06=27, SF055_05_06=5, SF056_05_06=1, SF060_05_06=20.720000000000027, SF061a_05_06=1.3599999999999994, SF061b_05_06=-0.2560000000000002, PRN_05_07=30, SF055_05_07=4, SF056_05_07=1, SF060_05_07=35.0, SF061a_05_07=0.4719999999999942, SF061b_05_07=0.367999999999995, PRN_05_08=36, SF055_05_08=3, SF056_05_08=1, SF060_05_08=20.28000000000003, SF061a_05_08=1.5360000000000014, SF061b_05_08=0.6239999999999952, SF031_06=5, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.0, SF044_06=1, SF048_06=-0.08799999999999997, SF049a_06=-0.01899999999999999, SF049b_06=-0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538881, PRN_06_01=4, SF055_06_01=2, SF056_06_01=1, SF060_06_01=5.600000000000023, SF061a_06_01=0.14399999999999125, SF061b_06_01=0.28000000000000114, PRN_06_02=10, SF055_06_02=3, SF056_06_02=1, SF060_06_02=3.2000000000000455, SF061a_06_02=0.24799999999999045, SF061b_06_02=0.29599999999999227, PRN_06_03=11, SF055_06_03=4, SF056_06_03=1, SF060_06_03=0.20000000000004547, SF061a_06_03=-0.7439999999999998, SF061b_06_03=0.35999999999999943, PRN_06_04=12, SF055_06_04=2, SF056_06_04=1, SF060_06_04=12.360000000000014, SF061a_06_04=0.2639999999999958, SF061b_06_04=-0.02400000000000091, PRN_06_05=19, SF055_06_05=4, SF056_06_05=1, SF060_06_05=0.5600000000000023, SF061a_06_05=-1.720000000000006, SF061b_06_05=0.23999999999999488, PRN_06_06=36, SF055_06_06=4, SF056_06_06=1, SF060_06_06=8.720000000000027, SF061a_06_06=1.2239999999999895, SF061b_06_06=0.43200000000000216, SF031_07=6, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.0, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=-0.015999999999999986, SF049b_07=-0.006000000000000005, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538881, PRN_07_01=4, SF055_07_01=3, SF056_07_01=1, SF060_07_01=7.319999999999993, SF061a_07_01=-0.03200000000001069, SF061b_07_01=0.19999999999998863, PRN_07_02=10, SF055_07_02=1, SF056_07_02=1, SF060_07_02=5.0, SF061a_07_02=0.11999999999999034, SF061b_07_02=0.24799999999999045, PRN_07_03=11, SF055_07_03=2, SF056_07_03=1, SF060_07_03=2.2000000000000455, SF061a_07_03=-0.480000000000004, SF061b_07_03=0.3359999999999985, PRN_07_04=12, SF055_07_04=1, SF056_07_04=1, SF060_07_04=12.760000000000048, SF061a_07_04=0.13599999999999568, SF061b_07_04=0.055999999999997385, PRN_07_05=19, SF055_07_05=2, SF056_07_05=1, SF060_07_05=2.080000000000041, SF061a_07_05=-0.9920000000000044, SF061b_07_05=0.015999999999991132, PRN_07_06=36, SF055_07_06=4, SF056_07_06=1, SF060_07_06=13.160000000000025, SF061a_07_06=0.9919999999999902, SF061b_07_06=0.6319999999999908, SF031_08=7, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.0, SF044_08=1, SF048_08=-0.14, SF049a_08=-0.023999999999999994, SF049b_08=-0.0010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF093_08=117571585, PRN_08_01=10, SF055_08_01=3, SF056_08_01=1, SF060_08_01=-8.839999999999975, SF061a_08_01=-0.7199999999999989, SF061b_08_01=-0.23199999999999932, PRN_08_02=11, SF055_08_02=4, SF056_08_02=1, SF060_08_02=-10.759999999999991, SF061a_08_02=-1.5520000000000067, SF061b_08_02=-0.1039999999999992, PRN_08_03=12, SF055_08_03=1, SF056_08_03=1, SF060_08_03=-2.8799999999999955, SF061a_08_03=-0.4960000000000093, SF061b_08_03=-0.3760000000000048, PRN_08_04=19, SF055_08_04=4, SF056_08_04=1, SF060_08_04=-12.479999999999961, SF061a_08_04=-1.240000000000009, SF061b_08_04=-0.1839999999999975, PRN_08_05=36, SF055_08_05=2, SF056_08_05=1, SF060_08_05=4.360000000000014, SF061a_08_05=0.5919999999999987, SF061b_08_05=0.3359999999999985, SF031_09=8, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.0040000000000000036, SF044_09=1, SF048_09=-0.14400000000000002, SF049a_09=0.0010000000000000009, SF049b_09=0.0, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, PRN_09_01=4, SF055_09_01=1, SF056_09_01=1, SF060_09_01=13.400000000000034, SF061a_09_01=-0.2400000000000091, SF061b_09_01=0.09599999999998943, PRN_09_02=10, SF055_09_02=2, SF056_09_02=1, SF060_09_02=11.520000000000039, SF061a_09_02=-0.35200000000000387, SF061b_09_02=-0.016000000000005343, PRN_09_03=11, SF055_09_03=1, SF056_09_03=1, SF060_09_03=8.0, SF061a_09_03=-0.5440000000000111, SF061b_09_03=0.14399999999999125, PRN_09_04=12, SF055_09_04=2, SF056_09_04=1, SF060_09_04=22.640000000000043, SF061a_09_04=-0.08800000000000807, SF061b_09_04=-0.2880000000000109, PRN_09_05=19, SF055_09_05=2, SF056_09_05=1, SF060_09_05=11.640000000000043, SF061a_09_05=-1.4000000000000057, SF061b_09_05=-0.1600000000000108, PRN_09_06=36, SF055_09_06=4, SF056_09_06=1, SF060_09_06=20.0, SF061a_09_06=-3.8160000000000025, SF061b_09_06=0.015999999999991132, SF031_10=9, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=1, SF043_10=0.0040000000000000036, SF044_10=1, SF048_10=-0.09199999999999997, SF049a_10=0.007000000000000006, SF049b_10=-0.0010000000000000009, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538881, PRN_10_01=4, SF055_10_01=2, SF056_10_01=1, SF060_10_01=9.160000000000025, SF061a_10_01=-0.30400000000000205, SF061b_10_01=-0.17600000000000193, PRN_10_02=10, SF055_10_02=2, SF056_10_02=1, SF060_10_02=6.720000000000027, SF061a_10_02=-0.4960000000000093, SF061b_10_02=-0.20000000000000284, PRN_10_03=11, SF055_10_03=2, SF056_10_03=1, SF060_10_03=4.8799999999999955, SF061a_10_03=-0.6159999999999997, SF061b_10_03=-0.15200000000000102, PRN_10_04=12, SF055_10_04=2, SF056_10_04=1, SF060_10_04=14.240000000000009, SF061a_10_04=0.031999999999996476, SF061b_10_04=-0.416000000000011, PRN_10_05=19, SF055_10_05=1, SF056_10_05=1, SF060_10_05=5.800000000000011, SF061a_10_05=-0.7120000000000033, SF061b_10_05=-0.38400000000000034, PRN_10_06=36, SF055_10_06=2, SF056_10_06=1, SF060_10_06=17.24000000000001, SF061a_10_06=-2.896000000000008, SF061b_10_06=-0.3119999999999976)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=465, eaf=0, crcType=2, frameCrc=0, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=8229442, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=10, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.0040000000000000036, SF044_01=1, SF048_01=-0.11199999999999999, SF049a_01=0.016000000000000014, SF049b_01=-0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538881, PRN_01_01=4, SF055_01_01=3, SF056_01_01=1, SF060_01_01=-2.5600000000000023, SF061a_01_01=-0.8719999999999999, SF061b_01_01=-0.14400000000000546, PRN_01_02=10, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-5.639999999999986, SF061a_01_02=-0.7520000000000095, SF061b_01_02=-0.21600000000000819, PRN_01_03=11, SF055_01_03=4, SF056_01_03=1, SF060_01_03=-6.0, SF061a_01_03=-0.9519999999999982, SF061b_01_03=-0.09600000000000364, PRN_01_04=12, SF055_01_04=1, SF056_01_04=1, SF060_01_04=-0.4399999999999977, SF061a_01_04=-0.5600000000000023, SF061b_01_04=-0.35200000000000387, PRN_01_05=19, SF055_01_05=2, SF056_01_05=1, SF060_01_05=-8.599999999999966, SF061a_01_05=-0.8320000000000078, SF061b_01_05=-0.3119999999999976, PRN_01_06=36, SF055_01_06=5, SF056_01_06=1, SF060_01_06=5.720000000000027, SF061a_01_06=-1.6640000000000015, SF061b_01_06=0.35199999999998965, SF031_02=11, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.0040000000000000036, SF044_02=1, SF048_02=-0.18799999999999994, SF049a_02=0.013000000000000012, SF049b_02=-0.0050000000000000044, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538881, PRN_02_01=4, SF055_02_01=2, SF056_02_01=1, SF060_02_01=14.319999999999993, SF061a_02_01=-0.3440000000000083, SF061b_02_01=0.03999999999999204, PRN_02_02=10, SF055_02_02=2, SF056_02_02=1, SF060_02_02=13.080000000000041, SF061a_02_02=-0.416000000000011, SF061b_02_02=0.055999999999997385, PRN_02_03=11, SF055_02_03=1, SF056_02_03=1, SF060_02_03=9.840000000000032, SF061a_02_03=-0.5600000000000023, SF061b_02_03=0.14399999999999125, PRN_02_04=12, SF055_02_04=2, SF056_02_04=1, SF060_02_04=24.319999999999993, SF061a_02_04=-0.3680000000000092, SF061b_02_04=-0.2560000000000002, PRN_02_05=19, SF055_02_05=1, SF056_02_05=1, SF060_02_05=18.0, SF061a_02_05=-1.2319999999999993, SF061b_02_05=-0.20000000000000284, PRN_02_06=36, SF055_02_06=5, SF056_02_06=1, SF060_02_06=31.80000000000001, SF061a_02_06=-1.9920000000000044, SF061b_02_06=0.06399999999999295, SF031_03=12, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.008000000000000007, SF044_03=1, SF048_03=-0.14, SF049a_03=0.008000000000000007, SF049b_03=0.016000000000000014, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4378984449, PRN_03_01=4, SF055_03_01=5, SF056_03_01=1, SF060_03_01=13.960000000000036, SF061a_03_01=0.43200000000000216, SF061b_03_01=0.43200000000000216, PRN_03_02=10, SF055_03_02=5, SF056_03_02=1, SF060_03_02=12.439999999999998, SF061a_03_02=0.19999999999998863, SF061b_03_02=0.40800000000000125, PRN_03_03=12, SF055_03_03=3, SF056_03_03=1, SF060_03_03=22.80000000000001, SF061a_03_03=-0.43200000000000216, SF061b_03_03=-0.2560000000000002, PRN_03_04=19, SF055_03_04=3, SF056_03_04=1, SF060_03_04=16.160000000000025, SF061a_03_04=-1.2240000000000038, SF061b_03_04=-0.3920000000000101, PRN_03_05=36, SF055_03_05=4, SF056_03_05=1, SF060_03_05=33.04000000000002, SF061a_03_05=-2.5120000000000076, SF061b_03_05=0.055999999999997385, SF031_04=13, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.008000000000000007, SF044_04=1, SF048_04=-0.09599999999999997, SF049a_04=0.0020000000000000018, SF049b_04=-0.0030000000000000027, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538881, PRN_04_01=4, SF055_04_01=1, SF056_04_01=1, SF060_04_01=11.080000000000041, SF061a_04_01=-0.3680000000000092, SF061b_04_01=-0.16800000000000637, PRN_04_02=10, SF055_04_02=1, SF056_04_02=1, SF060_04_02=9.200000000000045, SF061a_04_02=-0.4399999999999977, SF061b_04_02=-0.20000000000000284, PRN_04_03=11, SF055_04_03=2, SF056_04_03=1, SF060_04_03=7.560000000000002, SF061a_04_03=-0.5760000000000076, SF061b_04_03=-0.08800000000000807, PRN_04_04=12, SF055_04_04=1, SF056_04_04=1, SF060_04_04=16.80000000000001, SF061a_04_04=-0.0799999999999983, SF061b_04_04=-0.480000000000004, PRN_04_05=19, SF055_04_05=2, SF056_04_05=1, SF060_04_05=10.600000000000023, SF061a_04_05=-0.8719999999999999, SF061b_04_05=-0.3440000000000083, PRN_04_06=36, SF055_04_06=4, SF056_04_06=1, SF060_04_06=28.879999999999995, SF061a_04_06=-2.608000000000004, SF061b_04_06=-0.5600000000000023, SF031_05=14, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.008000000000000007, SF044_05=1, SF048_05=-0.12, SF049a_05=0.006000000000000005, SF049b_05=0.0, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538881, PRN_05_01=4, SF055_05_01=4, SF056_05_01=1, SF060_05_01=10.28000000000003, SF061a_05_01=-0.43200000000000216, SF061b_05_01=-0.16800000000000637, PRN_05_02=10, SF055_05_02=2, SF056_05_02=1, SF060_05_02=7.960000000000036, SF061a_05_02=-0.2960000000000065, SF061b_05_02=-0.2079999999999984, PRN_05_03=11, SF055_05_03=1, SF056_05_03=1, SF060_05_03=6.8799999999999955, SF061a_05_03=-0.6000000000000085, SF061b_05_03=-0.09600000000000364, PRN_05_04=12, SF055_05_04=1, SF056_05_04=1, SF060_05_04=13.920000000000016, SF061a_05_04=-0.03200000000001069, SF061b_05_04=-0.4720000000000084, PRN_05_05=19, SF055_05_05=1, SF056_05_05=1, SF060_05_05=8.0, SF061a_05_05=-0.8400000000000034, SF061b_05_05=-0.5919999999999987, PRN_05_06=36, SF055_05_06=4, SF056_05_06=1, SF060_05_06=25.879999999999995, SF061a_05_06=-2.6400000000000077, SF061b_05_06=-0.6240000000000094, SF031_06=15, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.008000000000000007, SF044_06=1, SF048_06=-0.15200000000000002, SF049a_06=0.009000000000000008, SF049b_06=-0.007000000000000006, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538880, PRN_06_01=4, SF055_06_01=1, SF056_06_01=1, SF060_06_01=7.28000000000003, SF061a_06_01=0.14399999999999125, SF061b_06_01=0.3199999999999932, PRN_06_02=10, SF055_06_02=1, SF056_06_02=1, SF060_06_02=4.400000000000034, SF061a_06_02=0.09599999999998943, SF061b_06_02=0.21599999999999397, PRN_06_03=11, SF055_06_03=2, SF056_06_03=1, SF060_06_03=4.160000000000025, SF061a_06_03=-0.35999999999999943, SF061b_06_03=0.38400000000000034, PRN_06_04=12, SF055_06_04=2, SF056_06_04=1, SF060_06_04=9.120000000000005, SF061a_06_04=0.35199999999998965, SF061b_06_04=0.16799999999999216, PRN_06_05=19, SF055_06_05=2, SF056_06_05=1, SF060_06_05=2.319999999999993, SF061a_06_05=-0.19200000000000728, SF061b_06_05=0.04800000000000182, SF031_07=16, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.008000000000000007, SF044_07=1, SF048_07=-0.15200000000000002, SF049a_07=0.0020000000000000018, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4546756608, PRN_07_01=4, SF055_07_01=1, SF056_07_01=1, SF060_07_01=19.439999999999998, SF061a_07_01=-1.024000000000001, SF061b_07_01=-0.6480000000000103, PRN_07_02=9, SF055_07_02=4, SF056_07_02=1, SF060_07_02=62.24000000000001, SF061a_07_02=0.22399999999998954, SF061b_07_02=-0.20000000000000284, PRN_07_03=10, SF055_07_03=1, SF056_07_03=1, SF060_07_03=18.08000000000004, SF061a_07_03=-1.1039999999999992, SF061b_07_03=-0.6720000000000113, PRN_07_04=11, SF055_07_04=1, SF056_07_04=1, SF060_07_04=15.920000000000016, SF061a_07_04=-1.240000000000009, SF061b_07_04=-0.4480000000000075, PRN_07_05=12, SF055_07_05=1, SF056_07_05=1, SF060_07_05=27.480000000000018, SF061a_07_05=-0.8800000000000097, SF061b_07_05=-0.9840000000000089, PRN_07_06=19, SF055_07_06=1, SF056_07_06=1, SF060_07_06=23.360000000000014, SF061a_07_06=-1.6800000000000068, SF061b_07_06=-1.0, SF031_08=17, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.008000000000000007, SF044_08=1, SF048_08=-0.11599999999999999, SF049a_08=-0.0040000000000000036, SF049b_08=0.006000000000000005, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4546756608, PRN_08_01=4, SF055_08_01=1, SF056_08_01=1, SF060_08_01=15.120000000000005, SF061a_08_01=-0.9519999999999982, SF061b_08_01=-0.6159999999999997, PRN_08_02=9, SF055_08_02=1, SF056_08_02=1, SF060_08_02=59.960000000000036, SF061a_08_02=0.28000000000000114, SF061b_08_02=-0.3760000000000048, PRN_08_03=10, SF055_08_03=1, SF056_08_03=1, SF060_08_03=13.640000000000043, SF061a_08_03=-0.9519999999999982, SF061b_08_03=-0.6640000000000015, PRN_08_04=11, SF055_08_04=1, SF056_08_04=1, SF060_08_04=12.240000000000009, SF061a_08_04=-1.088000000000008, SF061b_08_04=-0.5919999999999987, PRN_08_05=12, SF055_08_05=2, SF056_08_05=1, SF060_08_05=21.08000000000004, SF061a_08_05=-0.7920000000000016, SF061b_08_05=-0.9759999999999991, PRN_08_06=19, SF055_08_06=1, SF056_08_06=1, SF060_08_06=16.52000000000004, SF061a_08_06=-1.5840000000000032, SF061b_08_06=-0.9759999999999991, SF031_09=18, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.008000000000000007, SF044_09=1, SF048_09=-0.132, SF049a_09=0.006000000000000005, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, PRN_09_01=4, SF055_09_01=1, SF056_09_01=1, SF060_09_01=8.879999999999995, SF061a_09_01=0.3119999999999976, SF061b_09_01=0.5759999999999934, PRN_09_02=10, SF055_09_02=1, SF056_09_02=1, SF060_09_02=7.0400000000000205, SF061a_09_02=0.21599999999999397, SF061b_09_02=0.4719999999999942, PRN_09_03=11, SF055_09_03=1, SF056_09_03=1, SF060_09_03=6.28000000000003, SF061a_09_03=-0.3119999999999976, SF061b_09_03=0.5999999999999943, PRN_09_04=12, SF055_09_04=1, SF056_09_04=1, SF060_09_04=12.360000000000014, SF061a_09_04=0.5759999999999934, SF061b_09_04=0.23199999999999932, PRN_09_05=19, SF055_09_05=2, SF056_09_05=1, SF060_09_05=8.600000000000023, SF061a_09_05=-0.016000000000005343, SF061b_09_05=0.1599999999999966, PRN_09_06=36, SF055_09_06=2, SF056_09_06=1, SF060_09_06=31.0, SF061a_09_06=-1.9200000000000017, SF061b_09_06=0.35199999999998965, SF031_10=19, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.008000000000000007, SF044_10=1, SF048_10=-0.15200000000000002, SF049a_10=0.0030000000000000027, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538880, PRN_10_01=4, SF055_10_01=1, SF056_10_01=1, SF060_10_01=6.560000000000002, SF061a_10_01=0.1839999999999975, SF061b_10_01=0.30400000000000205, PRN_10_02=10, SF055_10_02=1, SF056_10_02=1, SF060_10_02=3.9600000000000364, SF061a_10_02=0.11999999999999034, SF061b_10_02=0.2560000000000002, PRN_10_03=11, SF055_10_03=1, SF056_10_03=1, SF060_10_03=4.560000000000002, SF061a_10_03=-0.12000000000000455, SF061b_10_03=0.37599999999999056, PRN_10_04=12, SF055_10_04=1, SF056_10_04=1, SF060_10_04=8.080000000000041, SF061a_10_04=0.3199999999999932, SF061b_10_04=0.16799999999999216, PRN_10_05=19, SF055_10_05=1, SF056_10_05=1, SF060_10_05=2.8799999999999955, SF061a_10_05=-0.28000000000000114, SF061b_10_05=0.007999999999995566)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=459, eaf=0, crcType=2, frameCrc=15, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=10010485, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=20, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.14800000000000002, SF049a_01=-0.0010000000000000009, SF049b_01=0.007000000000000006, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4546756608, PRN_01_01=4, SF055_01_01=1, SF056_01_01=1, SF060_01_01=21.08000000000004, SF061a_01_01=-0.8239999999999981, SF061b_01_01=-0.6720000000000113, PRN_01_02=9, SF055_01_02=5, SF056_01_02=1, SF060_01_02=62.08000000000004, SF061a_01_02=-0.06400000000000716, SF061b_01_02=-0.5280000000000058, PRN_01_03=10, SF055_01_03=1, SF056_01_03=1, SF060_01_03=19.840000000000032, SF061a_01_03=-0.8960000000000008, SF061b_01_03=-0.6880000000000024, PRN_01_04=11, SF055_01_04=1, SF056_01_04=1, SF060_01_04=18.360000000000014, SF061a_01_04=-1.0799999999999983, SF061b_01_04=-0.5840000000000032, PRN_01_05=12, SF055_01_05=1, SF056_01_05=1, SF060_01_05=28.28000000000003, SF061a_01_05=-0.6640000000000015, SF061b_01_05=-0.9840000000000089, PRN_01_06=19, SF055_01_06=1, SF056_01_06=1, SF060_01_06=26.160000000000025, SF061a_01_06=-1.3840000000000003, SF061b_01_06=-1.0160000000000053, SF031_02=21, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.124, SF049a_02=0.010000000000000009, SF049b_02=-0.009000000000000008, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4546756608, PRN_02_01=4, SF055_02_01=1, SF056_02_01=1, SF060_02_01=16.960000000000036, SF061a_02_01=-0.847999999999999, SF061b_02_01=-0.6640000000000015, PRN_02_02=9, SF055_02_02=1, SF056_02_02=1, SF060_02_02=59.44, SF061a_02_02=-0.02400000000000091, SF061b_02_02=-0.22400000000000375, PRN_02_03=10, SF055_02_03=1, SF056_02_03=1, SF060_02_03=15.520000000000039, SF061a_02_03=-0.8560000000000088, SF061b_02_03=-0.7280000000000086, PRN_02_04=11, SF055_02_04=1, SF056_02_04=1, SF060_02_04=14.680000000000007, SF061a_02_04=-1.13600000000001, SF061b_02_04=-0.48799999999999955, PRN_02_05=12, SF055_02_05=1, SF056_02_05=1, SF060_02_05=22.08000000000004, SF061a_02_05=-0.5600000000000023, SF061b_02_05=-1.1280000000000001, PRN_02_06=19, SF055_02_06=1, SF056_02_06=1, SF060_02_06=19.720000000000027, SF061a_02_06=-1.4399999999999977, SF061b_02_06=-1.088000000000008, SF031_03=22, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.14400000000000002, SF049a_03=0.0050000000000000044, SF049b_03=-0.0030000000000000027, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4345430017, PRN_03_01=4, SF055_03_01=1, SF056_03_01=1, SF060_03_01=7.640000000000043, SF061a_03_01=0.24799999999999045, SF061b_03_01=0.5519999999999925, PRN_03_02=11, SF055_03_02=1, SF056_03_02=1, SF060_03_02=6.080000000000041, SF061a_03_02=-0.1360000000000099, SF061b_03_02=0.6319999999999908, PRN_03_03=12, SF055_03_03=1, SF056_03_03=1, SF060_03_03=10.800000000000011, SF061a_03_03=0.47999999999998977, SF061b_03_03=0.24799999999999045, PRN_03_04=19, SF055_03_04=1, SF056_03_04=1, SF060_03_04=8.680000000000007, SF061a_03_04=-0.12000000000000455, SF061b_03_04=0.21599999999999397, PRN_03_05=36, SF055_03_05=2, SF056_03_05=1, SF060_03_05=35.64000000000004, SF061a_03_05=-1.9120000000000061, SF061b_03_05=0.17600000000000193, SF031_04=23, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=2, SF043_04=0.01200000000000001, SF044_04=1, SF048_04=-0.14, SF049a_04=-0.0040000000000000036, SF049b_04=0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538881, PRN_04_01=4, SF055_04_01=1, SF056_04_01=1, SF060_04_01=10.680000000000007, SF061a_04_01=0.30400000000000205, SF061b_04_01=0.5120000000000005, PRN_04_02=10, SF055_04_02=1, SF056_04_02=1, SF060_04_02=8.600000000000023, SF061a_04_02=0.21599999999999397, SF061b_04_02=0.3999999999999915, PRN_04_03=11, SF055_04_03=1, SF056_04_03=1, SF060_04_03=9.760000000000048, SF061a_04_03=-0.15200000000000102, SF061b_04_03=0.6079999999999899, PRN_04_04=12, SF055_04_04=1, SF056_04_04=1, SF060_04_04=12.360000000000014, SF061a_04_04=0.38400000000000034, SF061b_04_04=0.3359999999999985, PRN_04_05=19, SF055_04_05=1, SF056_04_05=1, SF060_04_05=9.640000000000043, SF061a_04_05=-0.1360000000000099, SF061b_04_05=0.15200000000000102, PRN_04_06=36, SF055_04_06=3, SF056_04_06=1, SF060_04_06=37.76000000000005, SF061a_04_06=-1.7280000000000015, SF061b_04_06=0.519999999999996, SF031_05=24, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=2, SF043_05=0.01200000000000001, SF044_05=1, SF048_05=-0.124, SF049a_05=-0.01999999999999999, SF049b_05=-0.01100000000000001, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538880, PRN_05_01=4, SF055_05_01=2, SF056_05_01=1, SF060_05_01=6.400000000000034, SF061a_05_01=0.46399999999999864, SF061b_05_01=0.2079999999999984, PRN_05_02=10, SF055_05_02=1, SF056_05_02=1, SF060_05_02=4.1200000000000045, SF061a_05_02=0.367999999999995, SF061b_05_02=0.09599999999998943, PRN_05_03=11, SF055_05_03=3, SF056_05_03=1, SF060_05_03=5.240000000000009, SF061a_05_03=0.08799999999999386, SF061b_05_03=0.1599999999999966, PRN_05_04=12, SF055_05_04=1, SF056_05_04=1, SF060_05_04=7.319999999999993, SF061a_05_04=0.7039999999999935, SF061b_05_04=-0.04000000000000625, PRN_05_05=19, SF055_05_05=1, SF056_05_05=1, SF060_05_05=3.6000000000000227, SF061a_05_05=-0.008000000000009777, SF061b_05_05=-0.22400000000000375, SF031_06=25, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.14, SF049a_06=-0.032, SF049b_06=-0.0030000000000000027, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538880, PRN_06_01=4, SF055_06_01=1, SF056_06_01=1, SF060_06_01=6.800000000000011, SF061a_06_01=0.3199999999999932, SF061b_06_01=0.13599999999999568, PRN_06_02=10, SF055_06_02=1, SF056_06_02=1, SF060_06_02=4.0400000000000205, SF061a_06_02=0.2560000000000002, SF061b_06_02=0.055999999999997385, PRN_06_03=11, SF055_06_03=1, SF056_06_03=1, SF060_06_03=6.080000000000041, SF061a_06_03=-0.17600000000000193, SF061b_06_03=0.16799999999999216, PRN_06_04=12, SF055_06_04=1, SF056_06_04=1, SF060_06_04=6.319999999999993, SF061a_06_04=0.4719999999999942, SF061b_06_04=-0.008000000000009777, PRN_06_05=19, SF055_06_05=1, SF056_06_05=1, SF060_06_05=2.5200000000000387, SF061a_06_05=-0.17600000000000193, SF061b_06_05=-0.14400000000000546, SF031_07=26, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=3, SF043_07=0.01200000000000001, SF044_07=1, SF048_07=-0.124, SF049a_07=-0.0020000000000000018, SF049b_07=0.014000000000000012, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538880, PRN_07_01=4, SF055_07_01=1, SF056_07_01=1, SF060_07_01=15.240000000000009, SF061a_07_01=0.4239999999999924, SF061b_07_01=-1.9120000000000061, PRN_07_02=10, SF055_07_02=1, SF056_07_02=1, SF060_07_02=14.720000000000027, SF061a_07_02=0.32799999999998875, SF061b_07_02=-1.960000000000008, PRN_07_03=11, SF055_07_03=2, SF056_07_03=1, SF060_07_03=13.400000000000034, SF061a_07_03=0.04800000000000182, SF061b_07_03=-1.8320000000000078, PRN_07_04=12, SF055_07_04=1, SF056_07_04=1, SF060_07_04=23.920000000000016, SF061a_07_04=0.3199999999999932, SF061b_07_04=-2.328000000000003, PRN_07_05=19, SF055_07_05=2, SF056_07_05=1, SF060_07_05=26.439999999999998, SF061a_07_05=-0.6720000000000113, SF061b_07_05=-2.4000000000000057, SF031_08=27, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=3, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.14800000000000002, SF049a_08=-0.0020000000000000018, SF049b_08=0.010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4412538881, PRN_08_01=4, SF055_08_01=1, SF056_08_01=1, SF060_08_01=14.240000000000009, SF061a_08_01=1.4080000000000013, SF061b_08_01=-0.1839999999999975, PRN_08_02=10, SF055_08_02=1, SF056_08_02=1, SF060_08_02=13.319999999999993, SF061a_08_02=1.3519999999999897, SF061b_08_02=-0.26400000000001, PRN_08_03=11, SF055_08_03=2, SF056_08_03=1, SF060_08_03=12.879999999999995, SF061a_08_03=1.0719999999999885, SF061b_08_03=-0.008000000000009777, PRN_08_04=12, SF055_08_04=1, SF056_08_04=1, SF060_08_04=20.400000000000034, SF061a_08_04=1.5279999999999916, SF061b_08_04=-0.6720000000000113, PRN_08_05=19, SF055_08_05=2, SF056_08_05=1, SF060_08_05=21.600000000000023, SF061a_08_05=0.8160000000000025, SF061b_08_05=-0.6800000000000068, PRN_08_06=36, SF055_08_06=4, SF056_08_06=1, SF060_08_06=47.24000000000001, SF061a_08_06=-0.1600000000000108, SF061b_08_06=0.03999999999999204, SF031_09=28, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.01200000000000001, SF044_09=1, SF048_09=-0.09199999999999997, SF049a_09=-0.0040000000000000036, SF049b_09=0.015000000000000013, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, PRN_09_01=4, SF055_09_01=1, SF056_09_01=1, SF060_09_01=13.760000000000048, SF061a_09_01=1.3279999999999887, SF061b_09_01=-0.16800000000000637, PRN_09_02=10, SF055_09_02=1, SF056_09_02=1, SF060_09_02=12.439999999999998, SF061a_09_02=1.2879999999999967, SF061b_09_02=-0.23199999999999932, PRN_09_03=11, SF055_09_03=1, SF056_09_03=1, SF060_09_03=13.0, SF061a_09_03=1.024000000000001, SF061b_09_03=-0.008000000000009777, PRN_09_04=12, SF055_09_04=1, SF056_09_04=1, SF060_09_04=17.80000000000001, SF061a_09_04=1.543999999999997, SF061b_09_04=-0.6880000000000024, PRN_09_05=19, SF055_09_05=1, SF056_09_05=1, SF060_09_05=18.879999999999995, SF061a_09_05=0.7680000000000007, SF061b_09_05=-0.695999999999998, PRN_09_06=36, SF055_09_06=3, SF056_09_06=1, SF060_09_06=46.960000000000036, SF061a_09_06=-0.32800000000000296, SF061b_09_06=-0.04000000000000625, SF031_10=29, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.01200000000000001, SF044_10=1, SF048_10=-0.14, SF049a_10=0.016000000000000014, SF049b_10=0.010000000000000009, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4546756608, PRN_10_01=4, SF055_10_01=1, SF056_10_01=1, SF060_10_01=13.680000000000007, SF061a_10_01=0.5519999999999925, SF061b_10_01=-0.19200000000000728, PRN_10_02=9, SF055_10_02=3, SF056_10_02=1, SF060_10_02=56.68000000000001, SF061a_10_02=0.8399999999999892, SF061b_10_02=0.7999999999999972, PRN_10_03=10, SF055_10_03=1, SF056_10_03=1, SF060_10_03=12.04000000000002, SF061a_10_03=0.4719999999999942, SF061b_10_03=-0.3119999999999976, PRN_10_04=11, SF055_10_04=1, SF056_10_04=1, SF060_10_04=13.080000000000041, SF061a_10_04=-0.2560000000000002, SF061b_10_04=-0.04000000000000625, PRN_10_05=12, SF055_10_05=2, SF056_10_05=1, SF060_10_05=16.439999999999998, SF061a_10_05=0.8160000000000025, SF061b_10_05=-0.4720000000000084, PRN_10_06=19, SF055_10_06=1, SF056_10_06=1, SF060_10_06=16.640000000000043, SF061a_10_06=-0.1600000000000108, SF061b_10_06=-0.3440000000000083)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=448, eaf=0, crcType=2, frameCrc=13, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=7076377, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.16800000000000004, SF049a_01=-0.0010000000000000009, SF049b_01=-0.015999999999999986, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538880, PRN_01_01=4, SF055_01_01=2, SF056_01_01=1, SF060_01_01=12.920000000000016, SF061a_01_01=0.5039999999999907, SF061b_01_01=-0.19200000000000728, PRN_01_02=10, SF055_01_02=2, SF056_01_02=1, SF060_01_02=11.160000000000025, SF061a_01_02=0.4239999999999924, SF061b_01_02=-0.22400000000000375, PRN_01_03=11, SF055_01_03=2, SF056_01_03=1, SF060_01_03=12.800000000000011, SF061a_01_03=0.19999999999998863, SF061b_01_03=0.055999999999997385, PRN_01_04=12, SF055_01_04=1, SF056_01_04=1, SF060_01_04=14.720000000000027, SF061a_01_04=0.6079999999999899, SF061b_01_04=-0.3680000000000092, PRN_01_05=19, SF055_01_05=4, SF056_01_05=1, SF060_01_05=13.920000000000016, SF061a_01_05=0.055999999999997385, SF061b_01_05=-0.6159999999999997, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.10399999999999998, SF049a_02=0.0020000000000000018, SF049b_02=0.007000000000000006, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538880, PRN_02_01=4, SF055_02_01=2, SF056_02_01=1, SF060_02_01=5.080000000000041, SF061a_02_01=0.28000000000000114, SF061b_02_01=0.1839999999999975, PRN_02_02=10, SF055_02_02=2, SF056_02_02=1, SF060_02_02=3.1200000000000045, SF061a_02_02=0.23199999999999932, SF061b_02_02=0.0799999999999983, PRN_02_03=11, SF055_02_03=4, SF056_02_03=1, SF060_02_03=5.080000000000041, SF061a_02_03=-0.06400000000000716, SF061b_02_03=0.13599999999999568, PRN_02_04=12, SF055_02_04=3, SF056_02_04=1, SF060_02_04=5.760000000000048, SF061a_02_04=0.5039999999999907, SF061b_02_04=-0.04800000000000182, PRN_02_05=19, SF055_02_05=2, SF056_02_05=1, SF060_02_05=4.240000000000009, SF061a_02_05=-0.1280000000000001, SF061b_02_05=-0.2560000000000002, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.09599999999999997, SF049a_03=-0.033, SF049b_03=-0.009000000000000008, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4412538880, PRN_03_01=4, SF055_03_01=1, SF056_03_01=1, SF060_03_01=5.960000000000036, SF061a_03_01=0.48799999999999955, SF061b_03_01=0.11199999999999477, PRN_03_02=10, SF055_03_02=2, SF056_03_02=1, SF060_03_02=3.4399999999999977, SF061a_03_02=0.30400000000000205, SF061b_03_02=0.055999999999997385, PRN_03_03=11, SF055_03_03=4, SF056_03_03=1, SF060_03_03=5.640000000000043, SF061a_03_03=1.9279999999999973, SF061b_03_03=0.2639999999999958, PRN_03_04=12, SF055_03_04=1, SF056_03_04=1, SF060_03_04=5.0400000000000205, SF061a_03_04=0.7599999999999909, SF061b_03_04=-0.02400000000000091, PRN_03_05=19, SF055_03_05=1, SF056_03_05=1, SF060_03_05=2.5600000000000023, SF061a_03_05=0.09599999999998943, SF061b_03_05=-0.1360000000000099, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.09999999999999998, SF049a_04=0.0010000000000000009, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538880, PRN_04_01=4, SF055_04_01=1, SF056_04_01=1, SF060_04_01=14.480000000000018, SF061a_04_01=0.13599999999999568, SF061b_04_01=-2.0320000000000036, PRN_04_02=10, SF055_04_02=2, SF056_04_02=1, SF060_04_02=14.080000000000041, SF061a_04_02=0.15200000000000102, SF061b_04_02=-2.0960000000000036, PRN_04_03=11, SF055_04_03=1, SF056_04_03=1, SF060_04_03=13.560000000000002, SF061a_04_03=0.09599999999998943, SF061b_04_03=-1.9200000000000017, PRN_04_04=12, SF055_04_04=3, SF056_04_04=1, SF060_04_04=23.720000000000027, SF061a_04_04=-0.008000000000009777, SF061b_04_04=-2.504000000000005, PRN_04_05=19, SF055_04_05=2, SF056_04_05=1, SF060_04_05=29.160000000000025, SF061a_04_05=-0.35999999999999943, SF061b_04_05=-2.608000000000004, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.132, SF049a_05=-0.0040000000000000036, SF049b_05=0.01100000000000001, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538881, PRN_05_01=4, SF055_05_01=2, SF056_05_01=1, SF060_05_01=7.600000000000023, SF061a_05_01=1.5519999999999925, SF061b_05_01=-0.20000000000000284, PRN_05_02=10, SF055_05_02=2, SF056_05_02=1, SF060_05_02=6.760000000000048, SF061a_05_02=1.5519999999999925, SF061b_05_02=-0.2560000000000002, PRN_05_03=11, SF055_05_03=3, SF056_05_03=1, SF060_05_03=7.520000000000039, SF061a_05_03=1.2879999999999967, SF061b_05_03=0.0, PRN_05_04=12, SF055_05_04=2, SF056_05_04=1, SF060_05_04=13.439999999999998, SF061a_05_04=1.4399999999999977, SF061b_05_04=-0.5760000000000076, PRN_05_05=19, SF055_05_05=3, SF056_05_05=1, SF060_05_05=17.400000000000034, SF061a_05_05=0.73599999999999, SF061b_05_05=-0.9440000000000026, PRN_05_06=36, SF055_05_06=4, SF056_05_06=1, SF060_05_06=47.84000000000003, SF061a_05_06=0.02400000000000091, SF061b_05_06=0.14399999999999125, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0020000000000000018, SF049b_06=-0.013000000000000012, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4546756608, PRN_06_01=4, SF055_06_01=1, SF056_06_01=1, SF060_06_01=11.080000000000041, SF061a_06_01=0.45599999999998886, SF061b_06_01=-0.23199999999999932, PRN_06_02=9, SF055_06_02=4, SF056_06_02=1, SF060_06_02=60.68000000000001, SF061a_06_02=0.4719999999999942, SF061b_06_02=0.519999999999996, PRN_06_03=10, SF055_06_03=1, SF056_06_03=1, SF060_06_03=9.400000000000034, SF061a_06_03=0.519999999999996, SF061b_06_03=-0.26400000000001, PRN_06_04=11, SF055_06_04=2, SF056_06_04=1, SF060_06_04=11.800000000000011, SF061a_06_04=0.3359999999999985, SF061b_06_04=-0.17600000000000193, PRN_06_05=12, SF055_06_05=1, SF056_06_05=1, SF060_06_05=12.080000000000041, SF061a_06_05=0.7199999999999989, SF061b_06_05=-0.4399999999999977, PRN_06_06=19, SF055_06_06=2, SF056_06_06=1, SF060_06_06=12.680000000000007, SF061a_06_06=0.2560000000000002, SF061b_06_06=-0.6159999999999997, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=2, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=0.0010000000000000009, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538880, PRN_07_01=4, SF055_07_01=1, SF056_07_01=1, SF060_07_01=15.720000000000027, SF061a_07_01=1.039999999999992, SF061b_07_01=-0.09600000000000364, PRN_07_02=10, SF055_07_02=1, SF056_07_02=1, SF060_07_02=13.720000000000027, SF061a_07_02=1.024000000000001, SF061b_07_02=-0.09600000000000364, PRN_07_03=11, SF055_07_03=1, SF056_07_03=1, SF060_07_03=17.04000000000002, SF061a_07_03=0.8799999999999955, SF061b_07_03=-0.1280000000000001, PRN_07_04=12, SF055_07_04=1, SF056_07_04=1, SF060_07_04=15.319999999999993, SF061a_07_04=1.0719999999999885, SF061b_07_04=-0.21600000000000819, PRN_07_05=19, SF055_07_05=1, SF056_07_05=1, SF060_07_05=15.120000000000005, SF061a_07_05=0.8079999999999927, SF061b_07_05=-0.45600000000000307, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.07199999999999995, SF049a_08=0.006000000000000005, SF049b_08=0.016000000000000014, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4412538880, PRN_08_01=4, SF055_08_01=1, SF056_08_01=1, SF060_08_01=15.520000000000039, SF061a_08_01=1.0559999999999974, SF061b_08_01=-0.03200000000001069, PRN_08_02=10, SF055_08_02=1, SF056_08_02=1, SF060_08_02=13.080000000000041, SF061a_08_02=1.0, SF061b_08_02=-0.16800000000000637, PRN_08_03=11, SF055_08_03=1, SF056_08_03=1, SF060_08_03=16.52000000000004, SF061a_08_03=0.8559999999999945, SF061b_08_03=-0.1039999999999992, PRN_08_04=12, SF055_08_04=1, SF056_08_04=1, SF060_08_04=14.160000000000025, SF061a_08_04=1.1039999999999992, SF061b_08_04=-0.2560000000000002, PRN_08_05=19, SF055_08_05=1, SF056_08_05=1, SF060_08_05=13.28000000000003, SF061a_08_05=0.671999999999997, SF061b_08_05=-0.30400000000000205, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.17600000000000005, SF049a_09=-0.01899999999999999, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4546756608, PRN_09_01=4, SF055_09_01=1, SF056_09_01=1, SF060_09_01=9.0, SF061a_09_01=0.5600000000000023, SF061b_09_01=-0.1600000000000108, PRN_09_02=9, SF055_09_02=3, SF056_09_02=1, SF060_09_02=61.160000000000025, SF061a_09_02=-0.480000000000004, SF061b_09_02=0.6640000000000015, PRN_09_03=10, SF055_09_03=1, SF056_09_03=1, SF060_09_03=7.080000000000041, SF061a_09_03=0.671999999999997, SF061b_09_03=-0.28000000000000114, PRN_09_04=11, SF055_09_04=2, SF056_09_04=1, SF060_09_04=10.160000000000025, SF061a_09_04=0.4959999999999951, SF061b_09_04=-0.1280000000000001, PRN_09_05=12, SF055_09_05=2, SF056_09_05=1, SF060_09_05=9.360000000000014, SF061a_09_05=0.6559999999999917, SF061b_09_05=-0.5600000000000023, PRN_09_06=19, SF055_09_06=2, SF056_09_06=1, SF060_09_06=10.520000000000039, SF061a_09_06=0.6400000000000006, SF061b_09_06=-0.6480000000000103, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=3, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.124, SF049a_10=0.010000000000000009, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538888, PRN_10_01=4, SF055_10_01=1, SF056_10_01=1, SF060_10_01=12.080000000000041, SF061a_10_01=0.9200000000000017, SF061b_10_01=-0.11200000000000898, PRN_10_02=10, SF055_10_02=1, SF056_10_02=1, SF060_10_02=10.160000000000025, SF061a_10_02=0.9039999999999964, SF061b_10_02=-0.08800000000000807, PRN_10_03=11, SF055_10_03=1, SF056_10_03=1, SF060_10_03=13.640000000000043, SF061a_10_03=0.8239999999999981, SF061b_10_03=-0.2079999999999984, PRN_10_04=12, SF055_10_04=1, SF056_10_04=1, SF060_10_04=11.560000000000002, SF061a_10_04=0.8319999999999936, SF061b_10_04=-0.2560000000000002, PRN_10_05=19, SF055_10_05=1, SF056_10_05=1, SF060_10_05=11.400000000000034, SF061a_10_05=0.9839999999999947, SF061b_10_05=-0.3359999999999985, PRN_10_06=33, SF055_10_06=5, SF056_10_06=1, SF060_10_06=68.76000000000005, SF061a_10_06=-4.496000000000002, SF061b_10_06=-3.5520000000000067)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=87, eaf=0, crcType=2, frameCrc=2, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=5702700, SF005=354, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.008000000000000007, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=-0.008000000000000007, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538880, PRN_01_01=4, SF055_01_01=2, SF056_01_01=1, SF060_01_01=-4.0, SF061a_01_01=0.24799999999999045, SF061b_01_01=-0.20000000000000284, PRN_01_02=10, SF055_01_02=1, SF056_01_02=1, SF060_01_02=-6.9599999999999795, SF061a_01_02=0.1839999999999975, SF061b_01_02=-0.2400000000000091, PRN_01_03=11, SF055_01_03=1, SF056_01_03=1, SF060_01_03=-5.639999999999986, SF061a_01_03=-0.06400000000000716, SF061b_01_03=-0.26400000000001, PRN_01_04=12, SF055_01_04=2, SF056_01_04=1, SF060_01_04=-4.0, SF061a_01_04=0.5759999999999934, SF061b_01_04=-0.3359999999999985, PRN_01_05=19, SF055_01_05=1, SF056_01_05=1, SF060_01_05=-9.439999999999998, SF061a_01_05=-0.07200000000000273, SF061b_01_05=-0.4720000000000084, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.16400000000000003, SF049a_02=-0.0010000000000000009, SF049b_02=0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538880, PRN_02_01=4, SF055_02_01=2, SF056_02_01=1, SF060_02_01=-3.599999999999966, SF061a_02_01=0.19999999999998863, SF061b_02_01=-0.20000000000000284, PRN_02_02=10, SF055_02_02=1, SF056_02_02=1, SF060_02_02=-6.839999999999975, SF061a_02_02=0.09599999999998943, SF061b_02_02=-0.30400000000000205, PRN_02_03=11, SF055_02_03=1, SF056_02_03=1, SF060_02_03=-6.079999999999984, SF061a_02_03=-0.1360000000000099, SF061b_02_03=-0.27200000000000557, PRN_02_04=12, SF055_02_04=1, SF056_02_04=1, SF060_02_04=-3.1200000000000045, SF061a_02_04=0.45599999999998886, SF061b_02_04=-0.35999999999999943, PRN_02_05=19, SF055_02_05=1, SF056_02_05=1, SF060_02_05=-9.879999999999995, SF061a_02_05=-0.03200000000001069, SF061b_02_05=-0.480000000000004)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=180, eaf=0, crcType=2, frameCrc=4, msgSubtype=0, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=736926, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=882933762, SF013_01=0, PRN_01=3, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF018_01=45, SF020R_01=0.13599999999999923, SF020A_01=-1.426000000000002, SF020C_01=0.045999999999999375, SF022_01=7, SF020CK_01=6.782, SF024_01=2, PhaseBiasBitmaskLen_01=0, SF025_01=60, PhaseBias_01_01=L1C, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, PhaseBias_01_02=L2W, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.6660000000000004, PhaseBias_01_03=L2L, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.6660000000000004, PhaseBias_01_04=L5Q, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.6359999999999992, CodeBiasBitmaskLen_01=0, SF027_01=60, CodeBias_01_01=C1C, SF029_01_01=-2.280000000000001, CodeBias_01_02=C2W, SF029_01_02=-0.35999999999999943, CodeBias_01_03=C2L, SF029_01_03=-0.240000000000002, CodeBias_01_04=C5Q, SF029_01_04=-2.4800000000000004, SF013_02=0, PRN_02=4, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF018_02=189, SF020R_02=-0.652000000000001, SF020A_02=-0.07000000000000028, SF020C_02=0.1039999999999992, SF022_02=7, SF020CK_02=3.041999999999998, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF025_02=60, PhaseBias_02_01=L1C, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, PhaseBias_02_02=L2W, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=1.5879999999999974, PhaseBias_02_03=L2L, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=1.5879999999999974, PhaseBias_02_04=L5Q, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=1.6039999999999992, CodeBiasBitmaskLen_02=0, SF027_02=60, CodeBias_02_01=C1C, SF029_02_01=-3.1400000000000006, CodeBias_02_02=C2W, SF029_02_02=-2.280000000000001, CodeBias_02_03=C2L, SF029_02_03=-2.460000000000001, CodeBias_02_04=C5Q, SF029_02_04=-1.1999999999999993, SF013_03=0, PRN_03=6, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF018_03=48, SF020R_03=-0.23200000000000287, SF020A_03=1.9899999999999984, SF020C_03=-0.0020000000000024443, SF022_03=7, SF020CK_03=1.8399999999999999, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF025_03=60, PhaseBias_03_01=L1C, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, PhaseBias_03_02=L2W, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=-0.23799999999999955, PhaseBias_03_03=L2L, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=-0.23799999999999955, PhaseBias_03_04=L5Q, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=-0.272000000000002, CodeBiasBitmaskLen_03=0, SF027_03=60, CodeBias_03_01=C1C, SF029_03_01=0.5999999999999979, CodeBias_03_02=C2W, SF029_03_02=2.84, CodeBias_03_03=C2L, SF029_03_03=3.099999999999998, CodeBias_03_04=C5Q, SF029_03_04=0.9199999999999982, SF013_04=0, PRN_04=9, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF018_04=5, SF020R_04=0.14399999999999835, SF020A_04=0.27399999999999736, SF020C_04=0.2759999999999998, SF022_04=7, SF020CK_04=2.8959999999999972, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF025_04=60, PhaseBias_04_01=L1C, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, PhaseBias_04_02=L2W, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=-0.17800000000000082, PhaseBias_04_03=L2L, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=-0.17800000000000082, PhaseBias_04_04=L5Q, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=-0.1620000000000026, CodeBiasBitmaskLen_04=0, SF027_04=60, CodeBias_04_01=C1C, SF029_04_01=0.16000000000000014, CodeBias_04_02=C2W, SF029_04_02=1.4400000000000013, CodeBias_04_03=C2L, SF029_04_03=1.2800000000000011, CodeBias_04_04=C5Q, SF029_04_04=-0.6000000000000014, SF013_05=0, PRN_05=11, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=6, SF018_05=108, SF020R_05=-0.7500000000000018, SF020A_05=-0.6400000000000006, SF020C_05=0.2560000000000002, SF022_05=6, SF020CK_05=-1.7180000000000017, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF025_05=60, PhaseBias_05_01=L1C, SF023_05_01=1, SF015_05_01=6, SF020PB_05_01=0.0, PhaseBias_05_02=L2W, SF023_05_02=1, SF015_05_02=6, SF020PB_05_02=0.27199999999999847, PhaseBias_05_03=L2L, SF023_05_03=1, SF015_05_03=6, SF020PB_05_03=0.27199999999999847, PhaseBias_05_04=L5Q, SF023_05_04=1, SF015_05_04=6, SF020PB_05_04=0.6219999999999999, CodeBiasBitmaskLen_05=0, SF027_05=60, CodeBias_05_01=C1C, SF029_05_01=-0.120000000000001, CodeBias_05_02=C2W, SF029_05_02=-0.08000000000000185, CodeBias_05_03=C2L, SF029_05_03=-0.1999999999999993, CodeBias_05_04=C5Q, SF029_05_04=1.5399999999999991, SF013_06=0, PRN_06=17, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF018_06=44, SF020R_06=-0.18599999999999994, SF020A_06=0.6459999999999972, SF020C_06=-0.24399999999999977, SF022_06=7, SF020CK_06=-1.3300000000000018, SF024_06=3, PhaseBiasBitmaskLen_06=0, SF025_06=56, PhaseBias_06_01=L1C, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, PhaseBias_06_02=L2W, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=-0.03400000000000247, PhaseBias_06_03=L2L, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=-0.03400000000000247, CodeBiasBitmaskLen_06=0, SF027_06=56, CodeBias_06_01=C1C, SF029_06_01=0.16000000000000014, CodeBias_06_02=C2W, SF029_06_02=-0.7800000000000011, CodeBias_06_03=C2L, SF029_06_03=-0.8399999999999999, SF013_07=0, PRN_07=31, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF018_07=32, SF020R_07=0.11199999999999832, SF020A_07=-0.48600000000000065, SF020C_07=0.4659999999999975, SF022_07=7, SF020CK_07=-1.474000000000002, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF025_07=56, PhaseBias_07_01=L1C, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, PhaseBias_07_02=L2W, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=0.2579999999999991, PhaseBias_07_03=L2L, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=0.2579999999999991, CodeBiasBitmaskLen_07=0, SF027_07=56, CodeBias_07_01=C1C, SF029_07_01=-0.9200000000000017, CodeBias_07_02=C2W, SF029_07_02=-2.0199999999999996, CodeBias_07_03=C2L, SF029_07_03=-1.9800000000000004)>",
+            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=152, eaf=0, crcType=2, frameCrc=15, msgSubtype=1, timeTagtype=1, gnssTimeTag=452211642, solutionId=5, solutionProcId=11, crc=7233776, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=8618373, SF013_01=0, PRN_01=1, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF019_01=89, SF020R_01=0.2839999999999989, SF020A_01=2.2779999999999987, SF020C_01=-1.910000000000002, SF022_01=7, SF020CK_01=-3.4040000000000017, SF024_01=2, PhaseBiasBitmaskLen_01=0, SF026_01=24, PhaseBias_01_01=L1C, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, PhaseBias_01_02=L2C, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=-0.5800000000000018, CodeBiasBitmaskLen_01=0, SF028_01=24, CodeBias_01_01=C1C, SF029_01_01=1.120000000000001, CodeBias_01_02=C2C, SF029_01_02=1.9199999999999982, SF013_02=0, PRN_02=7, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF019_02=89, SF020R_02=0.129999999999999, SF020A_02=0.6459999999999972, SF020C_02=0.8780000000000001, SF022_02=7, SF020CK_02=-0.7900000000000009, SF024_02=2, PhaseBiasBitmaskLen_02=0, SF026_02=24, PhaseBias_02_01=L1C, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, PhaseBias_02_02=L2C, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.4480000000000004, CodeBiasBitmaskLen_02=0, SF028_02=24, CodeBias_02_01=C1C, SF029_02_01=-0.6799999999999997, CodeBias_02_02=C2C, SF029_02_02=-0.5599999999999987, SF013_03=0, PRN_03=8, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF019_03=89, SF020R_03=-0.013999999999999346, SF020A_03=3.0159999999999982, SF020C_03=0.8580000000000005, SF022_03=7, SF020CK_03=4.366, SF024_03=2, PhaseBiasBitmaskLen_03=0, SF026_03=24, PhaseBias_03_01=L1C, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, PhaseBias_03_02=L2C, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.34199999999999875, CodeBiasBitmaskLen_03=0, SF028_03=24, CodeBias_03_01=C1C, SF029_03_01=-1.6000000000000014, CodeBias_03_02=C2C, SF029_03_02=-2.400000000000002, SF013_04=0, PRN_04=9, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF019_04=89, SF020R_04=0.7519999999999989, SF020A_04=6.013999999999999, SF020C_04=-3.1860000000000017, SF022_04=7, SF020CK_04=5.2940000000000005, SF024_04=2, PhaseBiasBitmaskLen_04=0, SF026_04=24, PhaseBias_04_01=L1C, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, PhaseBias_04_02=L2C, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.19399999999999906, CodeBiasBitmaskLen_04=0, SF028_04=24, CodeBias_04_01=C1C, SF029_04_01=-0.5599999999999987, CodeBias_04_02=C2C, SF029_04_02=-0.9600000000000009, SF013_05=0, PRN_05=16, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF019_05=89, SF020R_05=0.01799999999999713, SF020A_05=-5.796000000000001, SF020C_05=-0.1460000000000008, SF022_05=7, SF020CK_05=1.1119999999999983, SF024_05=2, PhaseBiasBitmaskLen_05=0, SF026_05=24, PhaseBias_05_01=L1C, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, PhaseBias_05_02=L2C, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=-0.1460000000000008, CodeBiasBitmaskLen_05=0, SF028_05=24, CodeBias_05_01=C1C, SF029_05_01=-0.5199999999999996, CodeBias_05_02=C2C, SF029_05_02=-0.10000000000000142, SF013_06=0, PRN_06=17, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=6, SF019_06=89, SF020R_06=0.5339999999999989, SF020A_06=-0.5640000000000018, SF020C_06=0.6739999999999995, SF022_06=6, SF020CK_06=-1.838000000000001, SF024_06=1, PhaseBiasBitmaskLen_06=0, SF026_06=24, PhaseBias_06_01=L1C, SF023_06_01=1, SF015_06_01=6, SF020PB_06_01=0.0, PhaseBias_06_02=L2C, SF023_06_02=1, SF015_06_02=6, SF020PB_06_02=-0.15000000000000213, CodeBiasBitmaskLen_06=0, SF028_06=24, CodeBias_06_01=C1C, SF029_06_01=0.03999999999999915, CodeBias_06_02=C2C, SF029_06_02=-0.03999999999999915, SF013_07=0, PRN_07=22, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF019_07=89, SF020R_07=1.4540000000000006, SF020A_07=-1.5180000000000007, SF020C_07=-1.200000000000001, SF022_07=7, SF020CK_07=-2.694000000000001, SF024_07=4, PhaseBiasBitmaskLen_07=0, SF026_07=24, PhaseBias_07_01=L1C, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, PhaseBias_07_02=L2C, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.7660000000000018, CodeBiasBitmaskLen_07=0, SF028_07=24, CodeBias_07_01=C1C, SF029_07_01=2.919999999999998, CodeBias_07_02=C2C, SF029_07_02=2.1799999999999997, SF013_08=0, PRN_08=24, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=7, SF019_08=89, SF020R_08=0.597999999999999, SF020A_08=0.15399999999999991, SF020C_08=0.5239999999999974, SF022_08=7, SF020CK_08=-1.6560000000000006, SF024_08=2, PhaseBiasBitmaskLen_08=0, SF026_08=24, PhaseBias_08_01=L1C, SF023_08_01=1, SF015_08_01=7, SF020PB_08_01=0.0, PhaseBias_08_02=L2C, SF023_08_02=1, SF015_08_02=7, SF020PB_08_02=-0.5660000000000007, CodeBiasBitmaskLen_08=0, SF028_08=24, CodeBias_08_01=C1C, SF029_08_01=1.379999999999999, CodeBias_08_02=C2C, SF029_08_02=1.259999999999998)>",
+            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=193, eaf=0, crcType=2, frameCrc=3, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=6801214, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF097=0, SatBitmaskLen=1, SF094=184555012, SF013_01=0, PRN_01=19, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF100_01=95, SF020R_01=0.24599999999999866, SF020A_01=0.20599999999999952, SF020C_01=-0.28000000000000114, SF022_01=7, SF020CK_01=2.9399999999999977, SF024_01=3, PhaseBiasBitmaskLen_01=0, SF103_01=232, PhaseBias_01_01=L2I, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, PhaseBias_01_02=L5P, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.7999999999999972, PhaseBias_01_03=L7I, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.7799999999999976, PhaseBias_01_04=L1P, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.0, CodeBiasBitmaskLen_01=0, SF106_01=232, CodeBias_01_01=C2I, SF029_01_01=-1.1799999999999997, CodeBias_01_02=C5P, SF029_01_02=-2.620000000000001, CodeBias_01_03=C7I, SF029_01_03=-2.620000000000001, CodeBias_01_04=C1P, SF029_01_04=-1.1799999999999997, SF013_02=0, PRN_02=21, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF100_02=95, SF020R_02=0.3379999999999974, SF020A_02=-0.08200000000000074, SF020C_02=-0.4380000000000006, SF022_02=7, SF020CK_02=4.047999999999998, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF103_02=232, PhaseBias_02_01=L2I, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, PhaseBias_02_02=L5P, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.7680000000000007, PhaseBias_02_03=L7I, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=0.7479999999999976, PhaseBias_02_04=L1P, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=0.0, CodeBiasBitmaskLen_02=0, SF106_02=232, CodeBias_02_01=C2I, SF029_02_01=-1.4000000000000021, CodeBias_02_02=C5P, SF029_02_02=-4.0, CodeBias_02_03=C7I, SF029_02_03=-4.0, CodeBias_02_04=C1P, SF029_02_04=-1.4000000000000021, SF013_03=0, PRN_03=22, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF100_03=95, SF020R_03=-0.240000000000002, SF020A_03=0.029999999999997584, SF020C_03=-0.34800000000000253, SF022_03=7, SF020CK_03=4.07, SF024_03=3, PhaseBiasBitmaskLen_03=0, SF103_03=232, PhaseBias_03_01=L2I, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, PhaseBias_03_02=L5P, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.6899999999999977, PhaseBias_03_03=L7I, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=0.6720000000000006, PhaseBias_03_04=L1P, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=0.0, CodeBiasBitmaskLen_03=0, SF106_03=232, CodeBias_03_01=C2I, SF029_03_01=-1.0199999999999996, CodeBias_03_02=C5P, SF029_03_02=-5.32, CodeBias_03_03=C7I, SF029_03_03=-5.32, CodeBias_03_04=C1P, SF029_03_04=-1.0199999999999996, SF013_04=0, PRN_04=34, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF100_04=95, SF020R_04=-0.1460000000000008, SF020A_04=0.2539999999999978, SF020C_04=0.347999999999999, SF022_04=7, SF020CK_04=-3.0100000000000016, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF103_04=232, PhaseBias_04_01=L2I, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, PhaseBias_04_02=L5P, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=-0.1479999999999997, PhaseBias_04_03=L7I, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=-0.1460000000000008, PhaseBias_04_04=L1P, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=0.0, CodeBiasBitmaskLen_04=0, SF106_04=232, CodeBias_04_01=C2I, SF029_04_01=0.14000000000000057, CodeBias_04_02=C5P, SF029_04_02=-0.26000000000000156, CodeBias_04_03=C7I, SF029_04_03=-0.26000000000000156, CodeBias_04_04=C1P, SF029_04_04=0.14000000000000057, SF013_05=0, PRN_05=36, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF100_05=95, SF020R_05=-0.15399999999999991, SF020A_05=-0.26399999999999935, SF020C_05=-0.2140000000000022, SF022_05=7, SF020CK_05=-5.328000000000001, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF103_05=232, PhaseBias_05_01=L2I, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, PhaseBias_05_02=L5P, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.8580000000000005, PhaseBias_05_03=L7I, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=0.8359999999999985, PhaseBias_05_04=L1P, SF023_05_04=1, SF015_05_04=7, SF020PB_05_04=0.0, CodeBiasBitmaskLen_05=0, SF106_05=232, CodeBias_05_01=C2I, SF029_05_01=-0.40000000000000213, CodeBias_05_02=C5P, SF029_05_02=6.140000000000001, CodeBias_05_03=C7I, SF029_05_03=6.140000000000001, CodeBias_05_04=C1P, SF029_05_04=-0.40000000000000213, SF013_06=0, PRN_06=37, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF100_06=95, SF020R_06=-0.38000000000000256, SF020A_06=-0.28800000000000026, SF020C_06=0.045999999999999375, SF022_06=7, SF020CK_06=-4.3580000000000005, SF024_06=2, PhaseBiasBitmaskLen_06=0, SF103_06=232, PhaseBias_06_01=L2I, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, PhaseBias_06_02=L5P, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=0.7880000000000003, PhaseBias_06_03=L7I, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=0.7680000000000007, PhaseBias_06_04=L1P, SF023_06_04=1, SF015_06_04=7, SF020PB_06_04=0.0, CodeBiasBitmaskLen_06=0, SF106_06=232, CodeBias_06_01=C2I, SF029_06_01=-1.4800000000000004, CodeBias_06_02=C5P, SF029_06_02=2.259999999999998, CodeBias_06_03=C7I, SF029_06_03=2.259999999999998, CodeBias_06_04=C1P, SF029_06_04=-1.4800000000000004, SF013_07=0, PRN_07=44, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF100_07=95, SF020R_07=0.1319999999999979, SF020A_07=0.3739999999999988, SF020C_07=0.4259999999999984, SF022_07=7, SF020CK_07=-1.6240000000000006, SF024_07=3, PhaseBiasBitmaskLen_07=0, SF103_07=232, PhaseBias_07_01=L2I, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, PhaseBias_07_02=L5P, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.0779999999999994, PhaseBias_07_03=L7I, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=-0.07600000000000051, PhaseBias_07_04=L1P, SF023_07_04=1, SF015_07_04=7, SF020PB_07_04=0.0, CodeBiasBitmaskLen_07=0, SF106_07=232, CodeBias_07_01=C2I, SF029_07_01=0.7800000000000011, CodeBias_07_02=C5P, SF029_07_02=0.33999999999999986, CodeBias_07_03=C7I, SF029_07_03=0.33999999999999986, CodeBias_07_04=C1P, SF029_07_04=0.7800000000000011)>",
         ]
         i = 0
         with open(
             os.path.join(self.dirname, "spartnntrip_20240430192807.log"),
             "rb",
         ) as stream:
             spr = SPARTNReader(
```

