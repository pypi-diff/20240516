# Comparing `tmp/GOES-3.4.1.tar.gz` & `tmp/goes-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GOES-3.4.1.tar", last modified: Mon Apr  8 04:35:02 2024, max compression
+gzip compressed data, was "goes-3.4.2.tar", last modified: Thu May 16 02:20:13 2024, max compression
```

## Comparing `GOES-3.4.1.tar` & `goes-3.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/GOES/
--rw-rw-r--   0 joao      (1000) joao      (1000)      549 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/__init__.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/GOES/downloads/
--rw-rw-r--   0 joao      (1000) joao      (1000)       70 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/downloads/__init__.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14842 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/downloads/download_data.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/GOES/processing/
--rw-rw-r--   0 joao      (1000) joao      (1000)       73 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/processing/__init__.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    68451 2024-04-08 04:28:31.000000 GOES-3.4.1/GOES/processing/processing_data.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-04-08 04:35:02.917894 GOES-3.4.1/GOES.egg-info/
--rw-r--r--   0 joao      (1000) joao      (1000)     2655 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)      304 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/SOURCES.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/dependency_links.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       46 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/requires.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        5 2024-04-08 04:35:02.000000 GOES-3.4.1/GOES.egg-info/top_level.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)     1535 2024-04-08 04:28:31.000000 GOES-3.4.1/LICENSE
--rw-r--r--   0 joao      (1000) joao      (1000)     2655 2024-04-08 04:35:02.917894 GOES-3.4.1/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)     1979 2024-04-08 04:28:31.000000 GOES-3.4.1/README.md
--rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-04-08 04:35:02.917894 GOES-3.4.1/setup.cfg
--rw-rw-r--   0 joao      (1000) joao      (1000)      867 2024-04-08 04:28:31.000000 GOES-3.4.1/setup.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-16 02:20:13.391471 goes-3.4.2/
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-16 02:20:13.387472 goes-3.4.2/GOES/
+-rw-r--r--   0 joao      (1000) joao      (1000)      616 2024-05-16 01:10:40.000000 goes-3.4.2/GOES/__init__.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-16 02:20:13.391471 goes-3.4.2/GOES/downloads/
+-rw-r--r--   0 joao      (1000) joao      (1000)       70 2024-05-16 01:10:48.000000 goes-3.4.2/GOES/downloads/__init__.py
+-rw-r--r--   0 joao      (1000) joao      (1000)    26171 2024-05-16 01:11:56.000000 goes-3.4.2/GOES/downloads/download_data.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-16 02:20:13.391471 goes-3.4.2/GOES/processing/
+-rw-r--r--   0 joao      (1000) joao      (1000)       73 2024-05-16 01:41:04.000000 goes-3.4.2/GOES/processing/__init__.py
+-rw-r--r--   0 joao      (1000) joao      (1000)    68451 2024-05-16 01:08:08.000000 goes-3.4.2/GOES/processing/processing_data.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-16 02:20:13.391471 goes-3.4.2/GOES.egg-info/
+-rw-r--r--   0 joao      (1000) joao      (1000)     2646 2024-05-16 02:20:13.000000 goes-3.4.2/GOES.egg-info/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)      304 2024-05-16 02:20:13.000000 goes-3.4.2/GOES.egg-info/SOURCES.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-05-16 02:20:13.000000 goes-3.4.2/GOES.egg-info/dependency_links.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       46 2024-05-16 02:20:13.000000 goes-3.4.2/GOES.egg-info/requires.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        5 2024-05-16 02:20:13.000000 goes-3.4.2/GOES.egg-info/top_level.txt
+-rw-r--r--   0 joao      (1000) joao      (1000)     1535 2024-05-16 01:08:08.000000 goes-3.4.2/LICENSE
+-rw-r--r--   0 joao      (1000) joao      (1000)     2646 2024-05-16 02:20:13.391471 goes-3.4.2/PKG-INFO
+-rw-r--r--   0 joao      (1000) joao      (1000)     1970 2024-05-16 01:53:31.000000 goes-3.4.2/README.md
+-rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-05-16 02:20:13.391471 goes-3.4.2/setup.cfg
+-rw-r--r--   0 joao      (1000) joao      (1000)      867 2024-05-16 01:13:23.000000 goes-3.4.2/setup.py
```

### Comparing `GOES-3.4.1/GOES/__init__.py` & `goes-3.4.2/GOES/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 name = "GOES"
 from .downloads.download_data import *
 from .processing.processing_data import *
 __all__ = ['show_products','download_file', 'download',
+           'show_products_from_google_cloud', 'get_data_to_colab',
            'GOES', 'open_dataset', 'open_mfdataset',
            'get_lonlat','get_lonlatcorner','corner_size_to_center_size',
            'midpoint_in_x','midpoint_in_y','calculate_corners',
            'find_pixel_of_coordinate',
            'cosine_of_solar_zenith_angle',
            'find_pixels_of_region','create_gridmap',
            'locate_files','accumulate_in_gridmap']
-__version__ = '3.4.1'
+__version__ = '3.4.2'
```

### Comparing `GOES-3.4.1/GOES/downloads/download_data.py` & `goes-3.4.2/GOES/downloads/download_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------------------------------------------------------------
 '''
 Description: Downloads GOES-16/17/18 data from amazon
 Author: Joao Henry Huaman Chinchay
 E-mail: joaohenry23@gmail.com
 Created date: Mar 23, 2020
-Modification date: Apr 07, 2024
+Modification date: May 15, 2024
 '''
 #-----------------------------------------------------------------------------------------------------------------------------------
 import numpy as np
 import s3fs
 from datetime import *
 import requests
 import os
+import subprocess
 
 from urllib3.util.retry import Retry
 from requests.adapters import HTTPAdapter
 
 #-----------------------------------------------------------------------------------------------------------------------------------
 def show_products():
 
@@ -370,8 +371,291 @@
         DateTimeIniLoop = DateTimeIniLoop + timedelta(minutes=60)
 
     Downloaded_files.sort()
 
     return Downloaded_files;
 
 #-----------------------------------------------------------------------------------------------------------------------------------
+def show_products_from_google_cloud(Satellite):
+
+    '''
+
+    Lists the products of GOES-16, GOES-17 and GOES-18 available in the Google Cloud.
+
+    Parameters
+    ----------
+    Satellite : str
+        Indicates serie of GOES, the options are 'goes16', 'goes17' and 'goes18'
+
+    '''
+
+    if 'COLAB_GPU' in os.environ:
+
+        if Satellite == 'goes16':
+            Sat = '16'
+        elif Satellite == 'goes17':
+            Sat = '17'
+        elif Satellite == 'goes18':
+            Sat = '18'
+        server = 'gs://gcp-public-data-goes-{}/'.format(Sat)
+        #list_gc = !gsutil ls -d $server
+        list_gc = subprocess.run(['gsutil','ls','-d',server], capture_output=True, text=True).stdout
+        list_gc = list(list_gc.split('\n'))[:-1]
+        print('Products of {} available in Google Cloud:'.format(Satellite))
+        for folder in list_gc:
+            if folder[-1] == '/':
+                print('  {}'.format(folder[len(server):-1]))
+
+    else:
+        print('\n  This function only works in Colab\n')
+
+#-----------------------------------------------------------------------------------------------------------------------------------
+def get_data_to_colab(Satellite, Product, DateTimeIni=None, DateTimeFin=None, domain=None, channel=None, path_out='/content/', size_format='Decimal'):
+
+    '''
+
+    Copy data of GOES-16, GOES-17 and GOES-18 from the Google Cloud to colab folder.
+
+    Parameters
+    ----------
+    Satellite : str
+        Indicates serie of GOES, the options are 'goes16', 'goes17' and 'goes18'
+
+
+    Product : str
+        Indicates the instrument and level of product. The products
+        can be list using: GOES.show_products()
+
+
+    DateTimeIni : str
+        String that indicates the initial datetime. Its structure
+        must be yyyymmdd-HHMMSS
+        Example:
+            DateTimeIni='20180520-183000'
+
+
+    DateTimeFin : str
+        String that indicates the final datetime. Its structure
+        must be yyyymmdd-HHMMSS
+        Example:
+            DateTimeFin='20180520-183000'
+
+
+    domain : str
+        This parameter just is necessary with Mesoescale products.
+        The options are:
+            M1 : Mesoscale 1
+            M2 : Mesoscale 2
+
+
+    channel : list
+        This parameter just is necessary with ABI-L1b-Rad and ABI-L2-CMIP products.
+        List indicates the channel or channels that will be download.
+        The channels can be mentioned individually as elements of the list
+        or as a sequence of channels separated by a hyphen ('-').
+        Example:
+            channel = ['02','08','09','10','11','13']
+            channel = ['02','08-11','13']
+
+
+    path_out : str, optional, default '/content/'
+        Optional string that indicates the folder where data will be download.
+        The default value is folder where python was open.
+
+
+    size_format: str, optional, default 'Decimal'
+        It defines how is print the size of file.
+        Options are:
+            'Decimal' : divide file size (in bytes) by (1000*1000) 
+            'Binary' : divide file size (in bytes) by (1024*1024)
+
+
+    Return
+    ------
+    Download_files : list
+        List with the downloaded files (path+filename).
+
+    '''
+
+    if 'COLAB_GPU' in os.environ:
+
+        # ----------------------------------------
+        if size_format == 'Binary':
+            dsize = 1024*1024
+        else:
+            dsize = 1000*1000
+
+        # ---------- Satellite -------------------
+        try:
+            assert Satellite == 'goes16' or Satellite == 'goes17' or Satellite == 'goes18'
+        except AssertionError:
+            print('\nSatellite should be goes16, goes17 or goes18\n')
+            return
+        else:
+            if Satellite == 'goes16':
+                Sat = '16'
+            elif Satellite == 'goes17':
+                Sat = '17'
+            elif Satellite == 'goes18':
+                Sat = '18'
+
+        # ---------- Product and Domain -------------------
+        if Product[-1] == 'M':
+            try:
+                assert domain == 'M1' or domain == 'M2'
+            except AssertionError:
+                print("\nProduct domain is mesoscale so you need define domain='M1' or domain='M2'\n")
+                return
+            else:
+                if domain == 'M1':
+                    Product2 = Product+'1'
+                elif domain == 'M2':
+                    Product2 = Product+'2'
+        else:
+            Product2 = Product
+
+        # ---------- DateTimeIni -------------------
+        try:
+            assert DateTimeIni != None
+        except AssertionError:
+            print('\nYou must define initial DateTimeIni\n')
+            return
+        else:
+            DateTimeIni = datetime.strptime(DateTimeIni, '%Y%m%d-%H%M%S')
+
+        # ---------- DateTimeFin -------------------
+        if DateTimeFin == None :
+            DateTimeFin = DateTimeIni
+        else:
+            DateTimeFin = datetime.strptime(DateTimeFin, '%Y%m%d-%H%M%S')
+
+        # ---------- channel -------------------
+
+        if Product[:-1] in ['ABI-L1b-Rad','ABI-L2-CMIP']:
+
+            try:
+                assert channel != None
+            except AssertionError:
+                print('\nYou must define channel or channels\n')
+                return
+            else:
+
+                try:
+                    #assert isinstance(channel, list) == True
+                    assert isinstance(channel, type([])) == True
+                except AssertionError:
+                    print('\nChannel must be a list\n')
+                    return
+                else:
+                    ChannelList = []
+                    for item in channel:
+
+                        try:
+                            #assert isinstance(item, str) == True
+                            assert isinstance(item, type('Hola Joao')) == True
+                        except AssertionError:
+                            print('\nEach elements of channel must have string format\n')
+                            return
+                        else:
+
+                            try:
+                                assert len(item) == 2 or len(item) == 5
+                            except AssertionError:
+                                print('\nElement of channel must be string with two or five characters\n')
+                                return
+                            else:
+                                if len(item) == 2 :
+                                    ChannelList.append(item)
+                                elif len(item) == 5 :
+                                    ChIni, ChEnd = item.split('-')
+                                    for Chn in range(int(ChIni),int(ChEnd)+1):
+                                        ChannelList.append('{:02d}'.format(Chn))
+
+
+        Downloaded_files = []
+
+        # ---------- Loop -------------------
+        DateTimeIniLoop = DateTimeIni.replace(minute=0)
+        DateTimeFinLoop = DateTimeFin.replace(minute=0)+timedelta(minutes=60)
+        while DateTimeIniLoop < DateTimeFinLoop :
+
+            DateTimeFolder = DateTimeIniLoop.strftime('%Y/%j/%H/')
+
+            server = 'gs://gcp-public-data-goes-'+Sat+'/'+Product+'/'+DateTimeFolder
+            #list_gc = !gsutil ls $server
+            list_gc = subprocess.run(['gsutil','ls',server], capture_output=True, text=True).stdout
+            list_gc = list(list_gc.split('\n'))[:-1]
+
+            ListFiles = np.array(list_gc)
+
+            for line in ListFiles:
+                if Product[:-1] in ['ABI-L1b-Rad','ABI-L2-CMIP']:
+                    NameFile = line.split('/')[-1]
+                    ChannelFile = NameFile.split('_')[1][-2:]
+                    DateTimeFile = datetime.strptime(NameFile[NameFile.find('_s')+2:NameFile.find('_e')-1], '%Y%j%H%M%S')
+
+                    if Product2 in NameFile    and    ChannelFile in ChannelList    and    DateTimeIni <= DateTimeFile <= DateTimeFin:
+
+                        NameOut = NameFile
+
+                        if os.path.isfile(path_out+NameFile) == True:
+                            #size_in_server = !gsutil du $line
+                            #size_in_server = int(size_in_server[0].split()[0])
+                            size_in_server = subprocess.run(['gsutil','du',line], capture_output=True, text=True).stdout
+                            size_in_server = int(size_in_server.split(' ')[0])
+                            size_in_folder = os.path.getsize(path_out+NameFile)
+                            if size_in_server == size_in_folder:
+                                print('{} already exists.'.format(NameFile))
+                            else:
+                                #!gsutil -q cp $line $path_out
+                                subprocess.run(['gsutil','-q','cp',line,path_out])
+                                size = os.path.getsize(path_out+NameFile)/dsize #
+                                print('{} {:.1f}MB [Replaced]'.format(NameFile,size))
+                        else:
+                            #!gsutil -q cp $line $path_out
+                            subprocess.run(['gsutil','-q','cp',line,path_out])
+                            size = os.path.getsize(path_out+NameFile)/dsize #
+                            print('{} {:.1f}MB'.format(NameFile,size))
+
+                        Downloaded_files.append(path_out+NameOut)
+
+                else:
+                    NameFile = line.split('/')[-1]
+                    DateTimeFile = datetime.strptime(NameFile[NameFile.find('_s')+2:NameFile.find('_e')-1], '%Y%j%H%M%S')
+
+                    if Product2 in NameFile    and    DateTimeIni <= DateTimeFile <= DateTimeFin:
+
+                        NameOut = NameFile
+
+                        if os.path.isfile(path_out+NameFile) == True:
+                            #size_in_server = !gsutil du $line
+                            #size_in_server = int(size_in_server[0].split()[0])
+                            size_in_server = subprocess.run(['gsutil','du',line], capture_output=True, text=True).stdout
+                            size_in_server = int(size_in_server.split(' ')[0])
+                            size_in_folder = os.path.getsize(path_out+NameFile)
+                            if size_in_server == size_in_folder:
+                                print('{} already exists.'.format(NameFile))
+                            else:
+                                #!gsutil -q cp $line $path_out
+                                subprocess.run(['gsutil','-q','cp',line,path_out])
+                                size = os.path.getsize(path_out+NameFile)/dsize #
+                                print('{} {:.1f}MB [Replaced]'.format(NameFile,size))
+
+                        else:
+                            #!gsutil -q cp $line $path_out
+                            subprocess.run(['gsutil','-q','cp',line,path_out])
+                            size = os.path.getsize(path_out+NameFile)/dsize #
+                            print('{} {:.1f}MB'.format(NameFile,size))
+
+                        Downloaded_files.append(path_out+NameOut)
+
+            DateTimeIniLoop = DateTimeIniLoop + timedelta(minutes=60)
+
+        Downloaded_files.sort()
+
+        return Downloaded_files;
+
+    else:
+        print('\n  This function only work in Colab\n')
+
+#-----------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `GOES-3.4.1/GOES/processing/processing_data.py` & `goes-3.4.2/GOES/processing/processing_data.py`

 * *Files identical despite different names*

### Comparing `GOES-3.4.1/GOES.egg-info/PKG-INFO` & `goes-3.4.2/GOES.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GOES
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python package to download and manipulate GOES-16/17/18 data.
 Home-page: https://github.com/joaohenry23/GOES
 Author: Joao Henry Huamán Chinchay
 Author-email: joaohenry23@gmail.com
 License: BSD 3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -17,21 +17,21 @@
 Requires-Dist: cftime>1.1
 Requires-Dist: requests
 Requires-Dist: s3fs
 Requires-Dist: pyproj
 Requires-Dist: netCDF4
 
 # GOES
-[![pypi](https://img.shields.io/badge/pypi%20-%203.4.1%20-%20dodgerblue)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
+[![Static Badge](https://img.shields.io/badge/pypi-3.4.2-jade)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/doi/10.5281/zenodo.4556211)
 
 Python package to download and manipulate GOES-16/17/18 data.
 <br><br>
 
 # Version
-3.4.1
+3.4.2
 <br><br>
 If you have already installed the GOES package, update it to the latest version.
 <br><br>
 
 # Requirements
 The main packages required are:
 - [numpy](https://numpy.org/)
```

### Comparing `GOES-3.4.1/LICENSE` & `goes-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GOES-3.4.1/PKG-INFO` & `goes-3.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GOES
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python package to download and manipulate GOES-16/17/18 data.
 Home-page: https://github.com/joaohenry23/GOES
 Author: Joao Henry Huamán Chinchay
 Author-email: joaohenry23@gmail.com
 License: BSD 3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -17,21 +17,21 @@
 Requires-Dist: cftime>1.1
 Requires-Dist: requests
 Requires-Dist: s3fs
 Requires-Dist: pyproj
 Requires-Dist: netCDF4
 
 # GOES
-[![pypi](https://img.shields.io/badge/pypi%20-%203.4.1%20-%20dodgerblue)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
+[![Static Badge](https://img.shields.io/badge/pypi-3.4.2-jade)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/doi/10.5281/zenodo.4556211)
 
 Python package to download and manipulate GOES-16/17/18 data.
 <br><br>
 
 # Version
-3.4.1
+3.4.2
 <br><br>
 If you have already installed the GOES package, update it to the latest version.
 <br><br>
 
 # Requirements
 The main packages required are:
 - [numpy](https://numpy.org/)
```

### Comparing `GOES-3.4.1/README.md` & `goes-3.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GOES
-[![pypi](https://img.shields.io/badge/pypi%20-%203.4.1%20-%20dodgerblue)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
+[![Static Badge](https://img.shields.io/badge/pypi-3.4.2-jade)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/doi/10.5281/zenodo.4556211)
 
 Python package to download and manipulate GOES-16/17/18 data.
 <br><br>
 
 # Version
-3.4.1
+3.4.2
 <br><br>
 If you have already installed the GOES package, update it to the latest version.
 <br><br>
 
 # Requirements
 The main packages required are:
 - [numpy](https://numpy.org/)
```

### Comparing `GOES-3.4.1/setup.py` & `goes-3.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
    long_description = fh.read()
 
 setuptools.setup(
    name="GOES",
-   version="3.4.1",
+   version="3.4.2",
    author="Joao Henry Huamán Chinchay",
    author_email="joaohenry23@gmail.com",
    description="Python package to download and manipulate GOES-16/17/18 data.",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://github.com/joaohenry23/GOES",
    license='BSD 3-Clause',
```

