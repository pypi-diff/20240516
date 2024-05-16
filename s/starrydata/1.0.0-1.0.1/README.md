# Comparing `tmp/starrydata-1.0.0.tar.gz` & `tmp/starrydata-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrydata-1.0.0.tar", last modified: Thu May 16 03:26:53 2024, max compression
+gzip compressed data, was "starrydata-1.0.1.tar", last modified: Thu May 16 03:37:33 2024, max compression
```

## Comparing `starrydata-1.0.0.tar` & `starrydata-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:26:53.070180 starrydata-1.0.0/
--rw-r--r--   0 matotomoya   (501) staff       (20)     1073 2023-12-12 10:27:13.000000 starrydata-1.0.0/LICENSE
--rw-r--r--   0 matotomoya   (501) staff       (20)     2427 2024-05-16 03:26:53.069891 starrydata-1.0.0/PKG-INFO
--rw-r--r--   0 matotomoya   (501) staff       (20)     1835 2024-05-16 03:24:29.000000 starrydata-1.0.0/README.md
--rw-r--r--   0 matotomoya   (501) staff       (20)      576 2024-05-16 03:26:50.000000 starrydata-1.0.0/pyproject.toml
--rw-r--r--   0 matotomoya   (501) staff       (20)       38 2024-05-16 03:26:53.070246 starrydata-1.0.0/setup.cfg
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:26:53.067365 starrydata-1.0.0/src/
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:26:53.068548 starrydata-1.0.0/src/starrydata/
--rw-r--r--   0 matotomoya   (501) staff       (20)        0 2024-05-15 03:36:37.000000 starrydata-1.0.0/src/starrydata/__init__.py
--rw-r--r--   0 matotomoya   (501) staff       (20)     5740 2024-05-15 06:22:44.000000 starrydata-1.0.0/src/starrydata/dataset.py
--rw-r--r--   0 matotomoya   (501) staff       (20)     4914 2024-05-12 10:10:09.000000 starrydata-1.0.0/src/starrydata/test_dataset.py
-drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:26:53.069613 starrydata-1.0.0/src/starrydata.egg-info/
--rw-r--r--   0 matotomoya   (501) staff       (20)     2427 2024-05-16 03:26:53.000000 starrydata-1.0.0/src/starrydata.egg-info/PKG-INFO
--rw-r--r--   0 matotomoya   (501) staff       (20)      305 2024-05-16 03:26:53.000000 starrydata-1.0.0/src/starrydata.egg-info/SOURCES.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)        1 2024-05-16 03:26:53.000000 starrydata-1.0.0/src/starrydata.egg-info/dependency_links.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)       21 2024-05-16 03:26:53.000000 starrydata-1.0.0/src/starrydata.egg-info/requires.txt
--rw-r--r--   0 matotomoya   (501) staff       (20)       11 2024-05-16 03:26:53.000000 starrydata-1.0.0/src/starrydata.egg-info/top_level.txt
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:37:33.878953 starrydata-1.0.1/
+-rw-r--r--   0 matotomoya   (501) staff       (20)     1073 2023-12-12 10:27:13.000000 starrydata-1.0.1/LICENSE
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2214 2024-05-16 03:37:33.878683 starrydata-1.0.1/PKG-INFO
+-rw-r--r--   0 matotomoya   (501) staff       (20)     1622 2024-05-16 03:36:49.000000 starrydata-1.0.1/README.md
+-rw-r--r--   0 matotomoya   (501) staff       (20)      576 2024-05-16 03:37:31.000000 starrydata-1.0.1/pyproject.toml
+-rw-r--r--   0 matotomoya   (501) staff       (20)       38 2024-05-16 03:37:33.879016 starrydata-1.0.1/setup.cfg
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:37:33.876284 starrydata-1.0.1/src/
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:37:33.877433 starrydata-1.0.1/src/starrydata/
+-rw-r--r--   0 matotomoya   (501) staff       (20)        0 2024-05-15 03:36:37.000000 starrydata-1.0.1/src/starrydata/__init__.py
+-rw-r--r--   0 matotomoya   (501) staff       (20)     5740 2024-05-15 06:22:44.000000 starrydata-1.0.1/src/starrydata/dataset.py
+-rw-r--r--   0 matotomoya   (501) staff       (20)     4914 2024-05-12 10:10:09.000000 starrydata-1.0.1/src/starrydata/test_dataset.py
+drwxr-xr-x   0 matotomoya   (501) staff       (20)        0 2024-05-16 03:37:33.878408 starrydata-1.0.1/src/starrydata.egg-info/
+-rw-r--r--   0 matotomoya   (501) staff       (20)     2214 2024-05-16 03:37:33.000000 starrydata-1.0.1/src/starrydata.egg-info/PKG-INFO
+-rw-r--r--   0 matotomoya   (501) staff       (20)      305 2024-05-16 03:37:33.000000 starrydata-1.0.1/src/starrydata.egg-info/SOURCES.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)        1 2024-05-16 03:37:33.000000 starrydata-1.0.1/src/starrydata.egg-info/dependency_links.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)       21 2024-05-16 03:37:33.000000 starrydata-1.0.1/src/starrydata.egg-info/requires.txt
+-rw-r--r--   0 matotomoya   (501) staff       (20)       11 2024-05-16 03:37:33.000000 starrydata-1.0.1/src/starrydata.egg-info/top_level.txt
```

### Comparing `starrydata-1.0.0/LICENSE` & `starrydata-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrydata-1.0.0/PKG-INFO` & `starrydata-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrydata
-Version: 1.0.0
+Version: 1.0.1
 Summary: Starrydata Python useful tools 
 Author-email: MATO Tomoya <tomoya.matou@gmail.com>
 Project-URL: Homepage, https://github.com/starrydata/starrydata-python-library
 Project-URL: Issues, https://github.com/starrydata/starrydata-python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,20 +23,14 @@
 
 You can install Starrydata from PyPI using the following command:
 
 ```sh
 pip install starrydata
 ```
 
-If you want to install from the PyPI test repository for testing purposes, use the following command:
-
-```sh
-pip install --index-url https://test.pypi.org/simple/ --no-deps starrydata
-```
-
 ## Usage
 
 Below is an example of how to use Starrydata.
 
 ### Downloading a Dataset
 
 To download a specific dataset, use the `Dataset` class. Here is an example of how to download and load a dataset into a pandas DataFrame:
@@ -67,12 +61,9 @@
 2. Create a new branch (`git checkout -b feature-branch`)
 3. Commit your changes (`git commit -am 'Add new feature'`)
 4. Push the branch (`git push origin feature-branch`)
 5. Create a pull request
 
 ## License
 
-This project is licensed under the MIT License. See the [LICENSE file](LICENSE) for more details.
-
----
+This project is licensed under the MIT License. See the [LICENSE file](https://github.com/starrydata/starrydata-python-library?tab=MIT-1-ov-file#readme) for more details.
 
-For questions or support, please contact [support@example.com](mailto:support@example.com).
```

### Comparing `starrydata-1.0.0/README.md` & `starrydata-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,102 +14,89 @@
 000000d0: 6374 732e 0a0a 2323 2049 6e73 7461 6c6c  cts...## Install
 000000e0: 6174 696f 6e0a 0a59 6f75 2063 616e 2069  ation..You can i
 000000f0: 6e73 7461 6c6c 2053 7461 7272 7964 6174  nstall Starrydat
 00000100: 6120 6672 6f6d 2050 7950 4920 7573 696e  a from PyPI usin
 00000110: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
 00000120: 636f 6d6d 616e 643a 0a0a 6060 6073 680a  command:..```sh.
 00000130: 7069 7020 696e 7374 616c 6c20 7374 6172  pip install star
-00000140: 7279 6461 7461 0a60 6060 0a0a 4966 2079  rydata.```..If y
-00000150: 6f75 2077 616e 7420 746f 2069 6e73 7461  ou want to insta
-00000160: 6c6c 2066 726f 6d20 7468 6520 5079 5049  ll from the PyPI
-00000170: 2074 6573 7420 7265 706f 7369 746f 7279   test repository
-00000180: 2066 6f72 2074 6573 7469 6e67 2070 7572   for testing pur
-00000190: 706f 7365 732c 2075 7365 2074 6865 2066  poses, use the f
-000001a0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-000001b0: 3a0a 0a60 6060 7368 0a70 6970 2069 6e73  :..```sh.pip ins
-000001c0: 7461 6c6c 202d 2d69 6e64 6578 2d75 726c  tall --index-url
-000001d0: 2068 7474 7073 3a2f 2f74 6573 742e 7079   https://test.py
-000001e0: 7069 2e6f 7267 2f73 696d 706c 652f 202d  pi.org/simple/ -
-000001f0: 2d6e 6f2d 6465 7073 2073 7461 7272 7964  -no-deps starryd
-00000200: 6174 610a 6060 600a 0a23 2320 5573 6167  ata.```..## Usag
-00000210: 650a 0a42 656c 6f77 2069 7320 616e 2065  e..Below is an e
-00000220: 7861 6d70 6c65 206f 6620 686f 7720 746f  xample of how to
-00000230: 2075 7365 2053 7461 7272 7964 6174 612e   use Starrydata.
-00000240: 0a0a 2323 2320 446f 776e 6c6f 6164 696e  ..### Downloadin
-00000250: 6720 6120 4461 7461 7365 740a 0a54 6f20  g a Dataset..To 
-00000260: 646f 776e 6c6f 6164 2061 2073 7065 6369  download a speci
-00000270: 6669 6320 6461 7461 7365 742c 2075 7365  fic dataset, use
-00000280: 2074 6865 2060 4461 7461 7365 7460 2063   the `Dataset` c
-00000290: 6c61 7373 2e20 4865 7265 2069 7320 616e  lass. Here is an
-000002a0: 2065 7861 6d70 6c65 206f 6620 686f 7720   example of how 
-000002b0: 746f 2064 6f77 6e6c 6f61 6420 616e 6420  to download and 
-000002c0: 6c6f 6164 2061 2064 6174 6173 6574 2069  load a dataset i
-000002d0: 6e74 6f20 6120 7061 6e64 6173 2044 6174  nto a pandas Dat
-000002e0: 6146 7261 6d65 3a0a 0a60 6060 7079 7468  aFrame:..```pyth
-000002f0: 6f6e 0a66 726f 6d20 7374 6172 7279 6461  on.from starryda
-00000300: 7461 2069 6d70 6f72 7420 4461 7461 7365  ta import Datase
-00000310: 740a 696d 706f 7274 2070 616e 6461 7320  t.import pandas 
-00000320: 6173 2070 640a 0a23 2049 6e69 7469 616c  as pd..# Initial
-00000330: 697a 6520 7468 6520 4461 7461 7365 7420  ize the Dataset 
-00000340: 6f62 6a65 6374 2077 6974 6820 6120 7370  object with a sp
-00000350: 6563 6966 6963 2064 6174 650a 6461 7461  ecific date.data
-00000360: 7365 7420 3d20 4461 7461 7365 7428 6461  set = Dataset(da
-00000370: 7465 3d22 3230 3234 3035 3135 2229 0a0a  te="20240515")..
-00000380: 2320 4c6f 6164 2074 6865 2064 6174 6173  # Load the datas
-00000390: 6574 2069 6e74 6f20 6120 7061 6e64 6173  et into a pandas
-000003a0: 2044 6174 6146 7261 6d65 0a64 6620 3d20   DataFrame.df = 
-000003b0: 7064 2e72 6561 645f 6373 7628 6461 7461  pd.read_csv(data
-000003c0: 7365 742e 616c 6c5f 6375 7276 6573 290a  set.all_curves).
-000003d0: 0a23 2044 6973 706c 6179 2074 6865 2044  .# Display the D
-000003e0: 6174 6146 7261 6d65 0a70 7269 6e74 2864  ataFrame.print(d
-000003f0: 6629 0a60 6060 0a0a 2323 2044 6f63 756d  f).```..## Docum
-00000400: 656e 7461 7469 6f6e 0a0a 466f 7220 6d6f  entation..For mo
-00000410: 7265 2064 6574 6169 6c65 6420 646f 6375  re detailed docu
-00000420: 6d65 6e74 6174 696f 6e20 616e 6420 7573  mentation and us
-00000430: 6167 6520 6578 616d 706c 6573 2c20 706c  age examples, pl
-00000440: 6561 7365 2072 6566 6572 2074 6f20 7468  ease refer to th
-00000450: 6520 5b6f 6666 6963 6961 6c20 646f 6375  e [official docu
-00000460: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-00000470: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000480: 6563 742f 7374 6172 7279 6461 7461 2f29  ect/starrydata/)
-00000490: 2e0a 0a23 2320 436f 6e74 7269 6275 7469  ...## Contributi
-000004a0: 6e67 0a0a 4275 6720 7265 706f 7274 7320  ng..Bug reports 
-000004b0: 616e 6420 6665 6174 7572 6520 7265 7175  and feature requ
-000004c0: 6573 7473 2061 7265 2077 656c 636f 6d65  ests are welcome
-000004d0: 2061 7420 7468 6520 5b47 6974 4875 6220   at the [GitHub 
-000004e0: 7265 706f 7369 746f 7279 5d28 6874 7470  repository](http
-000004f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000500: 7461 7272 7964 6174 612f 7374 6172 7279  tarrydata/starry
-00000510: 6461 7461 2d70 7974 686f 6e2d 6c69 6272  data-python-libr
-00000520: 6172 792f 292e 2043 6f6e 7472 6962 7574  ary/). Contribut
-00000530: 696f 6e73 2074 6f20 7468 6520 636f 6465  ions to the code
-00000540: 6261 7365 2061 7265 2061 6c73 6f20 6170  base are also ap
-00000550: 7072 6563 6961 7465 642e 2046 6f6c 6c6f  preciated. Follo
-00000560: 7720 7468 6573 6520 7374 6570 7320 746f  w these steps to
-00000570: 2063 6f6e 7472 6962 7574 653a 0a0a 312e   contribute:..1.
-00000580: 2046 6f72 6b20 7468 6520 7265 706f 7369   Fork the reposi
-00000590: 746f 7279 0a32 2e20 4372 6561 7465 2061  tory.2. Create a
-000005a0: 206e 6577 2062 7261 6e63 6820 2860 6769   new branch (`gi
-000005b0: 7420 6368 6563 6b6f 7574 202d 6220 6665  t checkout -b fe
-000005c0: 6174 7572 652d 6272 616e 6368 6029 0a33  ature-branch`).3
-000005d0: 2e20 436f 6d6d 6974 2079 6f75 7220 6368  . Commit your ch
-000005e0: 616e 6765 7320 2860 6769 7420 636f 6d6d  anges (`git comm
-000005f0: 6974 202d 616d 2027 4164 6420 6e65 7720  it -am 'Add new 
-00000600: 6665 6174 7572 6527 6029 0a34 2e20 5075  feature'`).4. Pu
-00000610: 7368 2074 6865 2062 7261 6e63 6820 2860  sh the branch (`
-00000620: 6769 7420 7075 7368 206f 7269 6769 6e20  git push origin 
-00000630: 6665 6174 7572 652d 6272 616e 6368 6029  feature-branch`)
-00000640: 0a35 2e20 4372 6561 7465 2061 2070 756c  .5. Create a pul
-00000650: 6c20 7265 7175 6573 740a 0a23 2320 4c69  l request..## Li
-00000660: 6365 6e73 650a 0a54 6869 7320 7072 6f6a  cense..This proj
-00000670: 6563 7420 6973 206c 6963 656e 7365 6420  ect is licensed 
-00000680: 756e 6465 7220 7468 6520 4d49 5420 4c69  under the MIT Li
-00000690: 6365 6e73 652e 2053 6565 2074 6865 205b  cense. See the [
-000006a0: 4c49 4345 4e53 4520 6669 6c65 5d28 4c49  LICENSE file](LI
-000006b0: 4345 4e53 4529 2066 6f72 206d 6f72 6520  CENSE) for more 
-000006c0: 6465 7461 696c 732e 0a0a 2d2d 2d0a 0a46  details...---..F
-000006d0: 6f72 2071 7565 7374 696f 6e73 206f 7220  or questions or 
-000006e0: 7375 7070 6f72 742c 2070 6c65 6173 6520  support, please 
-000006f0: 636f 6e74 6163 7420 5b73 7570 706f 7274  contact [support
-00000700: 4065 7861 6d70 6c65 2e63 6f6d 5d28 6d61  @example.com](ma
-00000710: 696c 746f 3a73 7570 706f 7274 4065 7861  ilto:support@exa
-00000720: 6d70 6c65 2e63 6f6d 292e 0a              mple.com)..
+00000140: 7279 6461 7461 0a60 6060 0a0a 2323 2055  rydata.```..## U
+00000150: 7361 6765 0a0a 4265 6c6f 7720 6973 2061  sage..Below is a
+00000160: 6e20 6578 616d 706c 6520 6f66 2068 6f77  n example of how
+00000170: 2074 6f20 7573 6520 5374 6172 7279 6461   to use Starryda
+00000180: 7461 2e0a 0a23 2323 2044 6f77 6e6c 6f61  ta...### Downloa
+00000190: 6469 6e67 2061 2044 6174 6173 6574 0a0a  ding a Dataset..
+000001a0: 546f 2064 6f77 6e6c 6f61 6420 6120 7370  To download a sp
+000001b0: 6563 6966 6963 2064 6174 6173 6574 2c20  ecific dataset, 
+000001c0: 7573 6520 7468 6520 6044 6174 6173 6574  use the `Dataset
+000001d0: 6020 636c 6173 732e 2048 6572 6520 6973  ` class. Here is
+000001e0: 2061 6e20 6578 616d 706c 6520 6f66 2068   an example of h
+000001f0: 6f77 2074 6f20 646f 776e 6c6f 6164 2061  ow to download a
+00000200: 6e64 206c 6f61 6420 6120 6461 7461 7365  nd load a datase
+00000210: 7420 696e 746f 2061 2070 616e 6461 7320  t into a pandas 
+00000220: 4461 7461 4672 616d 653a 0a0a 6060 6070  DataFrame:..```p
+00000230: 7974 686f 6e0a 6672 6f6d 2073 7461 7272  ython.from starr
+00000240: 7964 6174 6120 696d 706f 7274 2044 6174  ydata import Dat
+00000250: 6173 6574 0a69 6d70 6f72 7420 7061 6e64  aset.import pand
+00000260: 6173 2061 7320 7064 0a0a 2320 496e 6974  as as pd..# Init
+00000270: 6961 6c69 7a65 2074 6865 2044 6174 6173  ialize the Datas
+00000280: 6574 206f 626a 6563 7420 7769 7468 2061  et object with a
+00000290: 2073 7065 6369 6669 6320 6461 7465 0a64   specific date.d
+000002a0: 6174 6173 6574 203d 2044 6174 6173 6574  ataset = Dataset
+000002b0: 2864 6174 653d 2232 3032 3430 3531 3522  (date="20240515"
+000002c0: 290a 0a23 204c 6f61 6420 7468 6520 6461  )..# Load the da
+000002d0: 7461 7365 7420 696e 746f 2061 2070 616e  taset into a pan
+000002e0: 6461 7320 4461 7461 4672 616d 650a 6466  das DataFrame.df
+000002f0: 203d 2070 642e 7265 6164 5f63 7376 2864   = pd.read_csv(d
+00000300: 6174 6173 6574 2e61 6c6c 5f63 7572 7665  ataset.all_curve
+00000310: 7329 0a0a 2320 4469 7370 6c61 7920 7468  s)..# Display th
+00000320: 6520 4461 7461 4672 616d 650a 7072 696e  e DataFrame.prin
+00000330: 7428 6466 290a 6060 600a 0a23 2320 446f  t(df).```..## Do
+00000340: 6375 6d65 6e74 6174 696f 6e0a 0a46 6f72  cumentation..For
+00000350: 206d 6f72 6520 6465 7461 696c 6564 2064   more detailed d
+00000360: 6f63 756d 656e 7461 7469 6f6e 2061 6e64  ocumentation and
+00000370: 2075 7361 6765 2065 7861 6d70 6c65 732c   usage examples,
+00000380: 2070 6c65 6173 6520 7265 6665 7220 746f   please refer to
+00000390: 2074 6865 205b 6f66 6669 6369 616c 2064   the [official d
+000003a0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+000003b0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000003c0: 726f 6a65 6374 2f73 7461 7272 7964 6174  roject/starrydat
+000003d0: 612f 292e 0a0a 2323 2043 6f6e 7472 6962  a/)...## Contrib
+000003e0: 7574 696e 670a 0a42 7567 2072 6570 6f72  uting..Bug repor
+000003f0: 7473 2061 6e64 2066 6561 7475 7265 2072  ts and feature r
+00000400: 6571 7565 7374 7320 6172 6520 7765 6c63  equests are welc
+00000410: 6f6d 6520 6174 2074 6865 205b 4769 7448  ome at the [GitH
+00000420: 7562 2072 6570 6f73 6974 6f72 795d 2868  ub repository](h
+00000430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000440: 6d2f 7374 6172 7279 6461 7461 2f73 7461  m/starrydata/sta
+00000450: 7272 7964 6174 612d 7079 7468 6f6e 2d6c  rrydata-python-l
+00000460: 6962 7261 7279 2f29 2e20 436f 6e74 7269  ibrary/). Contri
+00000470: 6275 7469 6f6e 7320 746f 2074 6865 2063  butions to the c
+00000480: 6f64 6562 6173 6520 6172 6520 616c 736f  odebase are also
+00000490: 2061 7070 7265 6369 6174 6564 2e20 466f   appreciated. Fo
+000004a0: 6c6c 6f77 2074 6865 7365 2073 7465 7073  llow these steps
+000004b0: 2074 6f20 636f 6e74 7269 6275 7465 3a0a   to contribute:.
+000004c0: 0a31 2e20 466f 726b 2074 6865 2072 6570  .1. Fork the rep
+000004d0: 6f73 6974 6f72 790a 322e 2043 7265 6174  ository.2. Creat
+000004e0: 6520 6120 6e65 7720 6272 616e 6368 2028  e a new branch (
+000004f0: 6067 6974 2063 6865 636b 6f75 7420 2d62  `git checkout -b
+00000500: 2066 6561 7475 7265 2d62 7261 6e63 6860   feature-branch`
+00000510: 290a 332e 2043 6f6d 6d69 7420 796f 7572  ).3. Commit your
+00000520: 2063 6861 6e67 6573 2028 6067 6974 2063   changes (`git c
+00000530: 6f6d 6d69 7420 2d61 6d20 2741 6464 206e  ommit -am 'Add n
+00000540: 6577 2066 6561 7475 7265 2760 290a 342e  ew feature'`).4.
+00000550: 2050 7573 6820 7468 6520 6272 616e 6368   Push the branch
+00000560: 2028 6067 6974 2070 7573 6820 6f72 6967   (`git push orig
+00000570: 696e 2066 6561 7475 7265 2d62 7261 6e63  in feature-branc
+00000580: 6860 290a 352e 2043 7265 6174 6520 6120  h`).5. Create a 
+00000590: 7075 6c6c 2072 6571 7565 7374 0a0a 2323  pull request..##
+000005a0: 204c 6963 656e 7365 0a0a 5468 6973 2070   License..This p
+000005b0: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
+000005c0: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
+000005d0: 204c 6963 656e 7365 2e20 5365 6520 7468   License. See th
+000005e0: 6520 5b4c 4943 454e 5345 2066 696c 655d  e [LICENSE file]
+000005f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000600: 636f 6d2f 7374 6172 7279 6461 7461 2f73  com/starrydata/s
+00000610: 7461 7272 7964 6174 612d 7079 7468 6f6e  tarrydata-python
+00000620: 2d6c 6962 7261 7279 3f74 6162 3d4d 4954  -library?tab=MIT
+00000630: 2d31 2d6f 762d 6669 6c65 2372 6561 646d  -1-ov-file#readm
+00000640: 6529 2066 6f72 206d 6f72 6520 6465 7461  e) for more deta
+00000650: 696c 732e 0a0a                           ils...
```

### Comparing `starrydata-1.0.0/pyproject.toml` & `starrydata-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "starrydata"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="MATO Tomoya", email="tomoya.matou@gmail.com" },
 ]
 description = "Starrydata Python useful tools "
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `starrydata-1.0.0/src/starrydata/dataset.py` & `starrydata-1.0.1/src/starrydata/dataset.py`

 * *Files identical despite different names*

### Comparing `starrydata-1.0.0/src/starrydata/test_dataset.py` & `starrydata-1.0.1/src/starrydata/test_dataset.py`

 * *Files identical despite different names*

### Comparing `starrydata-1.0.0/src/starrydata.egg-info/PKG-INFO` & `starrydata-1.0.1/src/starrydata.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrydata
-Version: 1.0.0
+Version: 1.0.1
 Summary: Starrydata Python useful tools 
 Author-email: MATO Tomoya <tomoya.matou@gmail.com>
 Project-URL: Homepage, https://github.com/starrydata/starrydata-python-library
 Project-URL: Issues, https://github.com/starrydata/starrydata-python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,20 +23,14 @@
 
 You can install Starrydata from PyPI using the following command:
 
 ```sh
 pip install starrydata
 ```
 
-If you want to install from the PyPI test repository for testing purposes, use the following command:
-
-```sh
-pip install --index-url https://test.pypi.org/simple/ --no-deps starrydata
-```
-
 ## Usage
 
 Below is an example of how to use Starrydata.
 
 ### Downloading a Dataset
 
 To download a specific dataset, use the `Dataset` class. Here is an example of how to download and load a dataset into a pandas DataFrame:
@@ -67,12 +61,9 @@
 2. Create a new branch (`git checkout -b feature-branch`)
 3. Commit your changes (`git commit -am 'Add new feature'`)
 4. Push the branch (`git push origin feature-branch`)
 5. Create a pull request
 
 ## License
 
-This project is licensed under the MIT License. See the [LICENSE file](LICENSE) for more details.
-
----
+This project is licensed under the MIT License. See the [LICENSE file](https://github.com/starrydata/starrydata-python-library?tab=MIT-1-ov-file#readme) for more details.
 
-For questions or support, please contact [support@example.com](mailto:support@example.com).
```

