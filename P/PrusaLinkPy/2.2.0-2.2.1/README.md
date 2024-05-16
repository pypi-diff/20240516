# Comparing `tmp/prusalinkpy-2.2.0.tar.gz` & `tmp/prusalinkpy-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusalinkpy-2.2.0.tar", last modified: Mon May 13 14:23:26 2024, max compression
+gzip compressed data, was "prusalinkpy-2.2.1.tar", last modified: Thu May 16 14:10:14 2024, max compression
```

## Comparing `prusalinkpy-2.2.0.tar` & `prusalinkpy-2.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:23:26.819156 prusalinkpy-2.2.0/
--rw-rw-rw-   0        0        0     1075 2023-05-15 15:07:17.000000 prusalinkpy-2.2.0/LICENSE
--rw-rw-rw-   0        0        0    15045 2024-05-13 14:23:26.819156 prusalinkpy-2.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 14:23:26.789161 prusalinkpy-2.2.0/PrusaLinkPy/
--rw-rw-rw-   0        0        0    10059 2024-05-13 14:15:23.000000 prusalinkpy-2.2.0/PrusaLinkPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:23:26.819156 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/
--rw-rw-rw-   0        0        0    15045 2024-05-13 14:23:26.000000 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-13 14:23:26.000000 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:23:26.000000 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-13 14:23:26.000000 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13119 2024-05-13 14:22:01.000000 prusalinkpy-2.2.0/README.md
--rw-rw-rw-   0        0        0      691 2024-05-13 14:20:46.000000 prusalinkpy-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 14:23:26.819156 prusalinkpy-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      206 2024-05-13 14:20:35.000000 prusalinkpy-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:23:26.809212 prusalinkpy-2.2.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 prusalinkpy-2.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 prusalinkpy-2.2.0/tests/test_PrusaLinkPy.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:10:14.138127 prusalinkpy-2.2.1/
+-rw-rw-rw-   0        0        0     1075 2023-05-15 15:07:17.000000 prusalinkpy-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0    15932 2024-05-16 14:10:14.136127 prusalinkpy-2.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 14:10:14.109100 prusalinkpy-2.2.1/PrusaLinkPy/
+-rw-rw-rw-   0        0        0    10377 2024-05-16 14:06:32.000000 prusalinkpy-2.2.1/PrusaLinkPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:10:14.135059 prusalinkpy-2.2.1/PrusaLinkPy.egg-info/
+-rw-rw-rw-   0        0        0    15932 2024-05-16 14:10:14.000000 prusalinkpy-2.2.1/PrusaLinkPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-16 14:10:14.000000 prusalinkpy-2.2.1/PrusaLinkPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:10:14.000000 prusalinkpy-2.2.1/PrusaLinkPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-16 14:10:14.000000 prusalinkpy-2.2.1/PrusaLinkPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14006 2024-05-16 14:06:58.000000 prusalinkpy-2.2.1/README.md
+-rw-rw-rw-   0        0        0      691 2024-05-16 14:07:08.000000 prusalinkpy-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:10:14.138641 prusalinkpy-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      206 2024-05-16 14:07:04.000000 prusalinkpy-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:10:14.133993 prusalinkpy-2.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 prusalinkpy-2.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 prusalinkpy-2.2.1/tests/test_PrusaLinkPy.py
```

### Comparing `prusalinkpy-2.2.0/LICENSE` & `prusalinkpy-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prusalinkpy-2.2.0/PKG-INFO` & `prusalinkpy-2.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrusaLinkPy
-Version: 2.2.0
+Version: 2.2.1
 Summary: A library to interface with the PrusaLink API
 Author: Guillaume RICO
 Author-email: Guillaume RICO <guillaume.rico@alpesmesures.fr>
 License: Copyright (c) 2023 Guillaume RICO
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -35,14 +35,22 @@
 License-File: LICENSE
 
 
 PrusaLinkPy is a library to use the Prusa Link API.
 
 The library makes it easy to use the prusa API in python. The library is based on Request.
 
+Installation :
+
+    pip install PyPrusaLink
+    
+Update :
+
+    pip install PyPrusaLink -U
+
 Example of use :
 
     # Library import
     import PrusaLinkPy
     
     # Printer instantiation
     # IP : 192.168.0.123
@@ -70,101 +78,107 @@
     
 
 The library changed its name in May 2024. Before it was called prusaLink.
 Prusa staff asked me to leave them the name.
 
 # Change Log 
 
+## 2.2.1 :
+
+Tab correction
+
 ## 2.2 :
 
   Version made by [enrgarci](https://github.com/enrgarci)
  - Update README.md
- - Modified delete_job() to fix request from get to delete
+ - Modified [delete_job()](#prusalinkpydelete_job) to fix request from get to delete
  - added :
-
- * pause_print
- * resume_print
- * stop_print
+   - [pause_print()](#prusalinkpypause_print)
+   - [resume_print()](#prusalinkpyresume_print)
+   - [stop_print()](#prusalinkpystop_print)
 
 ## 2.1.1 :
 
  - Update README.md
  - added :
-
- * get_transfer
- * get_settings
+   - get_transfer
+   - get_settings
  
 ## 2.1.0 :
 
  - Update README.md
  - added :
-
- * delete
- * get_status
- * get_storage
- * delete_job
+   - delete
+   - [get_status()](#prusalinkpyget_status)
+   - [get_storage()](#prusalinkpyget_storage)
+   - [delete_job()](#prusalinkpydelete_job)
  
 ## 2.0.1 :
 
- - Bug correction on put_gcode
+ - Bug correction on [put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath-printafterupload--false-overwrite--false)
  
 ## 2.0.0 :
 
  - Support firmware 5.1.0
  - Added : 
-
- * get_files
- * put_gcode
- * exists_gcode
+   - [get_files(remoteDir)](#prusalinkpyget_files-remotedir--)
+   - [put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath-printafterupload--false-overwrite--false)
+   - [exists_gcode(remotePath)](#prusalinkpyexists_gcoderemotepath)
  
 ## 1.0.0 :
 
  - First Release
 
 # Installing PrusaLinkPy and Supported Versions
 
 PrusaLinkPy is available on pip :
 
     python -m pip install PrusaLinkPy
 
-PrusaLinkPy officially supports Python 3.9+ with Prusa MINI printer firmware 5.1.0.
+PrusaLinkPy officially supports Python 3.9+ with Prusa printers (MINI, MK4 or XL) firmware 5.1.0.
 
 
 # API Reference
 
 ## Low Level Functions
 
 [get_version()](#prusalinkpyget_version)
 
 [get_printer()](#prusalinkpyget_printer)
 
 [get_job()](#prusalinkpyget_job)
 
-[delete_job()](#prusalinkpydelete_job)
-
 [get_status()](#prusalinkpyget_status)
 
 [get_storage()](#prusalinkpyget_storage)
 
 [get_files(remoteDir)](#prusalinkpyget_files-remotedir--)
 
 [delete(remotePath)](#prusalinkpydeleteremotepath)
 
 [post_gcode(remotePath)](#prusalinkpyput_post_gcode)
 
-[put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath)
+[put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath-printafterupload--false-overwrite--false)
 
 [exists_gcode(remotePath)](#prusalinkpyexists_gcoderemotepath)
 
 [pause_print()](#prusalinkpypause_print)
 
 [resume_print()](#prusalinkpyresume_print)
 
 [stop_print()](#prusalinkpystop_print)
 
+Not documented :
+ * get_transfer
+ * get_settings
+
+For compatibility with old versions :
+
+[delete_job()](#prusalinkpydelete_job)
+
 ## High Level Functions 
 
 [get_recursive_files(remoteDir)](#prusalinkpyget_recursive_files-remotedir--)
 
 
 # User Guide
```

### Comparing `prusalinkpy-2.2.0/PrusaLinkPy/__init__.py` & `prusalinkpy-2.2.1/PrusaLinkPy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -248,61 +248,60 @@
         if "{" in ret.text :
             for filejson in ret.json()['files'][0]['children'] :
                 print("Delete file : " + filejson["path"])
                 self.delete( filejson["path"])
         else :
             return ret
 
-	def pause_print(self) :
-		"""
-		
-			Pause job.
-			None if no active job.
-			
-		"""
-		r = None
-		job_info = self.get_job()
-		# Check if response is json
-		if "{" in job_info.text :
-			if "id" in job_info.json():
-				id = str(job_info.json()['id'])
-				r = requests.put('http://' + self.host + ':' + self.port + '/api/v1/job/'+ id + '/pause', headers=self.headers)
-		return r
+    def pause_print(self) :
+        """
+        
+            Pause job.
+            None if no active job.
+            
+        """
+        r = None
+        job_info = self.get_job()
+        # Check if response is json
+        if "{" in job_info.text :
+            if "id" in job_info.json():
+                id = str(job_info.json()['id'])
+                r = requests.put('http://' + self.host + ':' + self.port + '/api/v1/job/'+ id + '/pause', headers=self.headers)
+        return r
 
-	def resume_print(self) :
-		"""
-		
-			Resume current job.
-			None if no active job.
-			
-		"""
-		r = None
-		job_info = self.get_job()
-		# Check if response is json 
-		if "{" in job_info.text :
-			if "id" in job_info.json():
-				id = str(job_info.json()['id'])
-				r = requests.put('http://' + self.host + ':' + self.port + '/api/v1/job/'+ id + '/resume', headers=self.headers)
-		return r
-	
-	def stop_print(self) :
-		"""
-		
-			Stop current job.
-			None if no active job
-			
-		"""
-		r = None
-		job_info = self.get_job()
-		# Check if response is json 
-		if "{" in job_info.text :
-			if "id" in job_info.json():
-				id = str(job_info.json()['id'])
-				r = requests.delete('http://' + self.host + ':' + self.port + '/api/v1/job/'+ str(id), headers=self.headers)
-		return r
+    def resume_print(self) :
+        """
         
+            Resume current job.
+            None if no active job.
+            
+        """
+        r = None
+        job_info = self.get_job()
+        # Check if response is json 
+        if "{" in job_info.text :
+            if "id" in job_info.json():
+                id = str(job_info.json()['id'])
+                r = requests.put('http://' + self.host + ':' + self.port + '/api/v1/job/'+ id + '/resume', headers=self.headers)
+        return r
+    
+    def stop_print(self) :
+        """
         
+            Stop current job.
+            None if no active job
+            
+        """
+        r = None
+        job_info = self.get_job()
+        # Check if response is json 
+        if "{" in job_info.text :
+            if "id" in job_info.json():
+                id = str(job_info.json()['id'])
+                r = requests.delete('http://' + self.host + ':' + self.port + '/api/v1/job/'+ str(id), headers=self.headers)
+        return r
+
 # Utilisation :
 # import PrusaLinkPy
 # prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM", port=8017)
 # prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.1.211", "44Da9wHhThmzFFJ")
 # obj = prusaMini.get_version()
```

### Comparing `prusalinkpy-2.2.0/PrusaLinkPy.egg-info/PKG-INFO` & `prusalinkpy-2.2.1/PrusaLinkPy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrusaLinkPy
-Version: 2.2.0
+Version: 2.2.1
 Summary: A library to interface with the PrusaLink API
 Author: Guillaume RICO
 Author-email: Guillaume RICO <guillaume.rico@alpesmesures.fr>
 License: Copyright (c) 2023 Guillaume RICO
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -35,14 +35,22 @@
 License-File: LICENSE
 
 
 PrusaLinkPy is a library to use the Prusa Link API.
 
 The library makes it easy to use the prusa API in python. The library is based on Request.
 
+Installation :
+
+    pip install PyPrusaLink
+    
+Update :
+
+    pip install PyPrusaLink -U
+
 Example of use :
 
     # Library import
     import PrusaLinkPy
     
     # Printer instantiation
     # IP : 192.168.0.123
@@ -70,101 +78,107 @@
     
 
 The library changed its name in May 2024. Before it was called prusaLink.
 Prusa staff asked me to leave them the name.
 
 # Change Log 
 
+## 2.2.1 :
+
+Tab correction
+
 ## 2.2 :
 
   Version made by [enrgarci](https://github.com/enrgarci)
  - Update README.md
- - Modified delete_job() to fix request from get to delete
+ - Modified [delete_job()](#prusalinkpydelete_job) to fix request from get to delete
  - added :
-
- * pause_print
- * resume_print
- * stop_print
+   - [pause_print()](#prusalinkpypause_print)
+   - [resume_print()](#prusalinkpyresume_print)
+   - [stop_print()](#prusalinkpystop_print)
 
 ## 2.1.1 :
 
  - Update README.md
  - added :
-
- * get_transfer
- * get_settings
+   - get_transfer
+   - get_settings
  
 ## 2.1.0 :
 
  - Update README.md
  - added :
-
- * delete
- * get_status
- * get_storage
- * delete_job
+   - delete
+   - [get_status()](#prusalinkpyget_status)
+   - [get_storage()](#prusalinkpyget_storage)
+   - [delete_job()](#prusalinkpydelete_job)
  
 ## 2.0.1 :
 
- - Bug correction on put_gcode
+ - Bug correction on [put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath-printafterupload--false-overwrite--false)
  
 ## 2.0.0 :
 
  - Support firmware 5.1.0
  - Added : 
-
- * get_files
- * put_gcode
- * exists_gcode
+   - [get_files(remoteDir)](#prusalinkpyget_files-remotedir--)
+   - [put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath-printafterupload--false-overwrite--false)
+   - [exists_gcode(remotePath)](#prusalinkpyexists_gcoderemotepath)
  
 ## 1.0.0 :
 
  - First Release
 
 # Installing PrusaLinkPy and Supported Versions
 
 PrusaLinkPy is available on pip :
 
     python -m pip install PrusaLinkPy
 
-PrusaLinkPy officially supports Python 3.9+ with Prusa MINI printer firmware 5.1.0.
+PrusaLinkPy officially supports Python 3.9+ with Prusa printers (MINI, MK4 or XL) firmware 5.1.0.
 
 
 # API Reference
 
 ## Low Level Functions
 
 [get_version()](#prusalinkpyget_version)
 
 [get_printer()](#prusalinkpyget_printer)
 
 [get_job()](#prusalinkpyget_job)
 
-[delete_job()](#prusalinkpydelete_job)
-
 [get_status()](#prusalinkpyget_status)
 
 [get_storage()](#prusalinkpyget_storage)
 
 [get_files(remoteDir)](#prusalinkpyget_files-remotedir--)
 
 [delete(remotePath)](#prusalinkpydeleteremotepath)
 
 [post_gcode(remotePath)](#prusalinkpyput_post_gcode)
 
-[put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath)
+[put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath-printafterupload--false-overwrite--false)
 
 [exists_gcode(remotePath)](#prusalinkpyexists_gcoderemotepath)
 
 [pause_print()](#prusalinkpypause_print)
 
 [resume_print()](#prusalinkpyresume_print)
 
 [stop_print()](#prusalinkpystop_print)
 
+Not documented :
+ * get_transfer
+ * get_settings
+
+For compatibility with old versions :
+
+[delete_job()](#prusalinkpydelete_job)
+
 ## High Level Functions 
 
 [get_recursive_files(remoteDir)](#prusalinkpyget_recursive_files-remotedir--)
 
 
 # User Guide
```

### Comparing `prusalinkpy-2.2.0/README.md` & `prusalinkpy-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,818 +3,874 @@
 00000020: 6520 7468 6520 5072 7573 6120 4c69 6e6b  e the Prusa Link
 00000030: 2041 5049 2e0d 0a0d 0a54 6865 206c 6962   API.....The lib
 00000040: 7261 7279 206d 616b 6573 2069 7420 6561  rary makes it ea
 00000050: 7379 2074 6f20 7573 6520 7468 6520 7072  sy to use the pr
 00000060: 7573 6120 4150 4920 696e 2070 7974 686f  usa API in pytho
 00000070: 6e2e 2054 6865 206c 6962 7261 7279 2069  n. The library i
 00000080: 7320 6261 7365 6420 6f6e 2052 6571 7565  s based on Reque
-00000090: 7374 2e0d 0a0d 0a45 7861 6d70 6c65 206f  st.....Example o
-000000a0: 6620 7573 6520 3a0d 0a0d 0a20 2020 2023  f use :....    #
-000000b0: 204c 6962 7261 7279 2069 6d70 6f72 740d   Library import.
-000000c0: 0a20 2020 2069 6d70 6f72 7420 5072 7573  .    import Prus
-000000d0: 614c 696e 6b50 790d 0a20 2020 200d 0a20  aLinkPy..    .. 
-000000e0: 2020 2023 2050 7269 6e74 6572 2069 6e73     # Printer ins
-000000f0: 7461 6e74 6961 7469 6f6e 0d0a 2020 2020  tantiation..    
-00000100: 2320 4950 203a 2031 3932 2e31 3638 2e30  # IP : 192.168.0
-00000110: 2e31 3233 0d0a 2020 2020 2320 4150 4920  .123..    # API 
-00000120: 4b45 5920 3a20 386f 6a48 4b48 474e 7541  KEY : 8ojHKHGNuA
-00000130: 4841 3262 4d0d 0a20 2020 2070 7275 7361  HA2bM..    prusa
-00000140: 4d69 6e69 203d 2050 7275 7361 4c69 6e6b  Mini = PrusaLink
-00000150: 5079 2e50 7275 7361 4c69 6e6b 5079 2822  Py.PrusaLinkPy("
-00000160: 3139 322e 3136 382e 302e 3132 3322 2c20  192.168.0.123", 
-00000170: 2238 6f6a 484b 4847 4e75 4148 4132 624d  "8ojHKHGNuAHA2bM
-00000180: 2229 0d0a 2020 2020 0d0a 2020 2020 2320  ")..    ..    # 
-00000190: 4765 7420 6265 6420 7465 6d70 6572 6174  Get bed temperat
-000001a0: 7572 650d 0a20 2020 2067 6574 5072 696e  ure..    getPrin
-000001b0: 7420 3d20 7072 7573 614d 696e 692e 6765  t = prusaMini.ge
-000001c0: 745f 7072 696e 7465 7228 290d 0a20 2020  t_printer()..   
-000001d0: 200d 0a20 2020 2023 2044 6973 706c 6179   ..    # Display
-000001e0: 2062 6564 2074 656d 7065 7261 7475 7265   bed temperature
-000001f0: 0d0a 2020 2020 7072 696e 7428 6765 7450  ..    print(getP
-00000200: 7269 6e74 2e6a 736f 6e28 295b 2274 656c  rint.json()["tel
-00000210: 656d 6574 7279 225d 5b22 7465 6d70 2d62  emetry"]["temp-b
-00000220: 6564 225d 290d 0a20 2020 200d 0a20 2020  ed"])..    ..   
-00000230: 2023 2044 656c 6574 6520 6120 6669 6c65   # Delete a file
-00000240: 7320 6f6e 2055 5342 2064 7269 7665 203a  s on USB drive :
-00000250: 0d0a 2020 2020 7072 7573 614d 696e 692e  ..    prusaMini.
-00000260: 6465 6c65 7465 2822 2f35 4833 304d 5f7e  delete("/5H30M_~
-00000270: 312e 4743 4f22 290d 0a20 2020 200d 0a20  1.GCO")..    .. 
-00000280: 2020 2023 2054 7261 6e73 6665 7272 696e     # Transferrin
-00000290: 6720 6120 6669 6c65 2074 6f20 7468 6520  g a file to the 
-000002a0: 7072 696e 7465 720d 0a20 2020 2069 6620  printer..    if 
-000002b0: 6e6f 7420 7072 7573 614d 696e 692e 6578  not prusaMini.ex
-000002c0: 6973 7473 5f67 636f 6465 2827 464f 4c44  ists_gcode('FOLD
-000002d0: 4552 2f74 6573 742e 6763 6f64 6527 2920  ER/test.gcode') 
-000002e0: 3a0d 0a20 2020 2020 2020 2070 7275 7361  :..        prusa
-000002f0: 4d69 6e69 2e70 7574 5f67 636f 6465 2827  Mini.put_gcode('
-00000300: 433a 2f41 4d2f 7465 7374 2e67 636f 6465  C:/AM/test.gcode
-00000310: 272c 2027 464f 4c44 4552 2f74 6573 742e  ', 'FOLDER/test.
-00000320: 6763 6f64 6527 290d 0a20 2020 200d 0a20  gcode')..    .. 
-00000330: 2020 2023 204c 6973 7420 6669 6c65 7320     # List files 
-00000340: 6f6e 2055 5342 2044 7269 7665 203a 0d0a  on USB Drive :..
-00000350: 2020 2020 7072 7573 614d 696e 692e 6765      prusaMini.ge
-00000360: 745f 6669 6c65 7328 292e 6a73 6f6e 2829  t_files().json()
-00000370: 5b22 6368 696c 6472 656e 225d 0d0a 2020  ["children"]..  
-00000380: 2020 0d0a 2020 2020 2320 5072 696e 7420    ..    # Print 
-00000390: 7468 6973 2066 696c 6520 0d0a 2020 2020  this file ..    
-000003a0: 7072 7573 614d 696e 692e 706f 7374 5f70  prusaMini.post_p
-000003b0: 7269 6e74 5f67 636f 6465 2827 2f75 7362  rint_gcode('/usb
-000003c0: 2f74 6573 742e 6763 6f64 6527 290d 0a20  /test.gcode').. 
-000003d0: 2020 200d 0a0d 0a54 6865 206c 6962 7261     ....The libra
-000003e0: 7279 2063 6861 6e67 6564 2069 7473 206e  ry changed its n
-000003f0: 616d 6520 696e 204d 6179 2032 3032 342e  ame in May 2024.
-00000400: 2042 6566 6f72 6520 6974 2077 6173 2063   Before it was c
-00000410: 616c 6c65 6420 7072 7573 614c 696e 6b2e  alled prusaLink.
-00000420: 0d0a 5072 7573 6120 7374 6166 6620 6173  ..Prusa staff as
-00000430: 6b65 6420 6d65 2074 6f20 6c65 6176 6520  ked me to leave 
-00000440: 7468 656d 2074 6865 206e 616d 652e 0d0a  them the name...
-00000450: 0d0a 2320 4368 616e 6765 204c 6f67 200d  ..# Change Log .
-00000460: 0a0d 0a23 2320 322e 3220 3a0d 0a0d 0a20  ...## 2.2 :.... 
-00000470: 2056 6572 7369 6f6e 206d 6164 6520 6279   Version made by
-00000480: 205b 656e 7267 6172 6369 5d28 6874 7470   [enrgarci](http
-00000490: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-000004a0: 6e72 6761 7263 6929 0d0a 202d 2055 7064  nrgarci).. - Upd
-000004b0: 6174 6520 5245 4144 4d45 2e6d 640d 0a20  ate README.md.. 
-000004c0: 2d20 4d6f 6469 6669 6564 2064 656c 6574  - Modified delet
-000004d0: 655f 6a6f 6228 2920 746f 2066 6978 2072  e_job() to fix r
-000004e0: 6571 7565 7374 2066 726f 6d20 6765 7420  equest from get 
-000004f0: 746f 2064 656c 6574 650d 0a20 2d20 6164  to delete.. - ad
-00000500: 6465 6420 3a0d 0a0d 0a20 2a20 7061 7573  ded :.... * paus
-00000510: 655f 7072 696e 740d 0a20 2a20 7265 7375  e_print.. * resu
-00000520: 6d65 5f70 7269 6e74 0d0a 202a 2073 746f  me_print.. * sto
-00000530: 705f 7072 696e 740d 0a0d 0a23 2320 322e  p_print....## 2.
-00000540: 312e 3120 3a0d 0a0d 0a20 2d20 5570 6461  1.1 :.... - Upda
-00000550: 7465 2052 4541 444d 452e 6d64 0d0a 202d  te README.md.. -
-00000560: 2061 6464 6564 203a 0d0a 0d0a 202a 2067   added :.... * g
-00000570: 6574 5f74 7261 6e73 6665 720d 0a20 2a20  et_transfer.. * 
-00000580: 6765 745f 7365 7474 696e 6773 0d0a 200d  get_settings.. .
-00000590: 0a23 2320 322e 312e 3020 3a0d 0a0d 0a20  .## 2.1.0 :.... 
-000005a0: 2d20 5570 6461 7465 2052 4541 444d 452e  - Update README.
-000005b0: 6d64 0d0a 202d 2061 6464 6564 203a 0d0a  md.. - added :..
-000005c0: 0d0a 202a 2064 656c 6574 650d 0a20 2a20  .. * delete.. * 
-000005d0: 6765 745f 7374 6174 7573 0d0a 202a 2067  get_status.. * g
-000005e0: 6574 5f73 746f 7261 6765 0d0a 202a 2064  et_storage.. * d
-000005f0: 656c 6574 655f 6a6f 620d 0a20 0d0a 2323  elete_job.. ..##
-00000600: 2032 2e30 2e31 203a 0d0a 0d0a 202d 2042   2.0.1 :.... - B
-00000610: 7567 2063 6f72 7265 6374 696f 6e20 6f6e  ug correction on
-00000620: 2070 7574 5f67 636f 6465 0d0a 200d 0a23   put_gcode.. ..#
-00000630: 2320 322e 302e 3020 3a0d 0a0d 0a20 2d20  # 2.0.0 :.... - 
-00000640: 5375 7070 6f72 7420 6669 726d 7761 7265  Support firmware
-00000650: 2035 2e31 2e30 0d0a 202d 2041 6464 6564   5.1.0.. - Added
-00000660: 203a 200d 0a0d 0a20 2a20 6765 745f 6669   : .... * get_fi
-00000670: 6c65 730d 0a20 2a20 7075 745f 6763 6f64  les.. * put_gcod
-00000680: 650d 0a20 2a20 6578 6973 7473 5f67 636f  e.. * exists_gco
-00000690: 6465 0d0a 200d 0a23 2320 312e 302e 3020  de.. ..## 1.0.0 
-000006a0: 3a0d 0a0d 0a20 2d20 4669 7273 7420 5265  :.... - First Re
-000006b0: 6c65 6173 650d 0a0d 0a23 2049 6e73 7461  lease....# Insta
-000006c0: 6c6c 696e 6720 5072 7573 614c 696e 6b50  lling PrusaLinkP
-000006d0: 7920 616e 6420 5375 7070 6f72 7465 6420  y and Supported 
-000006e0: 5665 7273 696f 6e73 0d0a 0d0a 5072 7573  Versions....Prus
-000006f0: 614c 696e 6b50 7920 6973 2061 7661 696c  aLinkPy is avail
-00000700: 6162 6c65 206f 6e20 7069 7020 3a0d 0a0d  able on pip :...
-00000710: 0a20 2020 2070 7974 686f 6e20 2d6d 2070  .    python -m p
-00000720: 6970 2069 6e73 7461 6c6c 2050 7275 7361  ip install Prusa
-00000730: 4c69 6e6b 5079 0d0a 0d0a 5072 7573 614c  LinkPy....PrusaL
-00000740: 696e 6b50 7920 6f66 6669 6369 616c 6c79  inkPy officially
-00000750: 2073 7570 706f 7274 7320 5079 7468 6f6e   supports Python
-00000760: 2033 2e39 2b20 7769 7468 2050 7275 7361   3.9+ with Prusa
-00000770: 204d 494e 4920 7072 696e 7465 7220 6669   MINI printer fi
-00000780: 726d 7761 7265 2035 2e31 2e30 2e0d 0a0d  rmware 5.1.0....
-00000790: 0a0d 0a23 2041 5049 2052 6566 6572 656e  ...# API Referen
-000007a0: 6365 0d0a 0d0a 2323 204c 6f77 204c 6576  ce....## Low Lev
-000007b0: 656c 2046 756e 6374 696f 6e73 0d0a 0d0a  el Functions....
-000007c0: 5b67 6574 5f76 6572 7369 6f6e 2829 5d28  [get_version()](
-000007d0: 2370 7275 7361 6c69 6e6b 7079 6765 745f  #prusalinkpyget_
-000007e0: 7665 7273 696f 6e29 0d0a 0d0a 5b67 6574  version)....[get
-000007f0: 5f70 7269 6e74 6572 2829 5d28 2370 7275  _printer()](#pru
-00000800: 7361 6c69 6e6b 7079 6765 745f 7072 696e  salinkpyget_prin
-00000810: 7465 7229 0d0a 0d0a 5b67 6574 5f6a 6f62  ter)....[get_job
-00000820: 2829 5d28 2370 7275 7361 6c69 6e6b 7079  ()](#prusalinkpy
-00000830: 6765 745f 6a6f 6229 0d0a 0d0a 5b64 656c  get_job)....[del
-00000840: 6574 655f 6a6f 6228 295d 2823 7072 7573  ete_job()](#prus
-00000850: 616c 696e 6b70 7964 656c 6574 655f 6a6f  alinkpydelete_jo
-00000860: 6229 0d0a 0d0a 5b67 6574 5f73 7461 7475  b)....[get_statu
-00000870: 7328 295d 2823 7072 7573 616c 696e 6b70  s()](#prusalinkp
-00000880: 7967 6574 5f73 7461 7475 7329 0d0a 0d0a  yget_status)....
-00000890: 5b67 6574 5f73 746f 7261 6765 2829 5d28  [get_storage()](
-000008a0: 2370 7275 7361 6c69 6e6b 7079 6765 745f  #prusalinkpyget_
-000008b0: 7374 6f72 6167 6529 0d0a 0d0a 5b67 6574  storage)....[get
-000008c0: 5f66 696c 6573 2872 656d 6f74 6544 6972  _files(remoteDir
-000008d0: 295d 2823 7072 7573 616c 696e 6b70 7967  )](#prusalinkpyg
-000008e0: 6574 5f66 696c 6573 2d72 656d 6f74 6564  et_files-remoted
-000008f0: 6972 2d2d 290d 0a0d 0a5b 6465 6c65 7465  ir--)....[delete
-00000900: 2872 656d 6f74 6550 6174 6829 5d28 2370  (remotePath)](#p
-00000910: 7275 7361 6c69 6e6b 7079 6465 6c65 7465  rusalinkpydelete
-00000920: 7265 6d6f 7465 7061 7468 290d 0a0d 0a5b  remotepath)....[
-00000930: 706f 7374 5f67 636f 6465 2872 656d 6f74  post_gcode(remot
-00000940: 6550 6174 6829 5d28 2370 7275 7361 6c69  ePath)](#prusali
-00000950: 6e6b 7079 7075 745f 706f 7374 5f67 636f  nkpyput_post_gco
-00000960: 6465 290d 0a0d 0a5b 7075 745f 6763 6f64  de)....[put_gcod
-00000970: 6528 6669 6c65 5061 7468 4c6f 6361 6c2c  e(filePathLocal,
-00000980: 2072 656d 6f74 6544 6972 2c20 7072 696e   remoteDir, prin
-00000990: 7441 6674 6572 5570 6c6f 6164 203d 2046  tAfterUpload = F
-000009a0: 616c 7365 2c20 6f76 6572 7772 6974 6520  alse, overwrite 
-000009b0: 3d20 4661 6c73 6529 5d28 2370 7275 7361  = False)](#prusa
-000009c0: 6c69 6e6b 7079 7075 745f 6763 6f64 6572  linkpyput_gcoder
-000009d0: 656d 6f74 6570 6174 6829 0d0a 0d0a 5b65  emotepath)....[e
-000009e0: 7869 7374 735f 6763 6f64 6528 7265 6d6f  xists_gcode(remo
-000009f0: 7465 5061 7468 295d 2823 7072 7573 616c  tePath)](#prusal
-00000a00: 696e 6b70 7965 7869 7374 735f 6763 6f64  inkpyexists_gcod
-00000a10: 6572 656d 6f74 6570 6174 6829 0d0a 0d0a  eremotepath)....
-00000a20: 5b70 6175 7365 5f70 7269 6e74 2829 5d28  [pause_print()](
-00000a30: 2370 7275 7361 6c69 6e6b 7079 7061 7573  #prusalinkpypaus
-00000a40: 655f 7072 696e 7429 0d0a 0d0a 5b72 6573  e_print)....[res
-00000a50: 756d 655f 7072 696e 7428 295d 2823 7072  ume_print()](#pr
-00000a60: 7573 616c 696e 6b70 7972 6573 756d 655f  usalinkpyresume_
-00000a70: 7072 696e 7429 0d0a 0d0a 5b73 746f 705f  print)....[stop_
-00000a80: 7072 696e 7428 295d 2823 7072 7573 616c  print()](#prusal
-00000a90: 696e 6b70 7973 746f 705f 7072 696e 7429  inkpystop_print)
-00000aa0: 0d0a 0d0a 2323 2048 6967 6820 4c65 7665  ....## High Leve
-00000ab0: 6c20 4675 6e63 7469 6f6e 7320 0d0a 0d0a  l Functions ....
-00000ac0: 5b67 6574 5f72 6563 7572 7369 7665 5f66  [get_recursive_f
-00000ad0: 696c 6573 2872 656d 6f74 6544 6972 295d  iles(remoteDir)]
-00000ae0: 2823 7072 7573 616c 696e 6b70 7967 6574  (#prusalinkpyget
-00000af0: 5f72 6563 7572 7369 7665 5f66 696c 6573  _recursive_files
-00000b00: 2d72 656d 6f74 6564 6972 2d2d 290d 0a0d  -remotedir--)...
-00000b10: 0a0d 0a23 2055 7365 7220 4775 6964 650d  ...# User Guide.
-00000b20: 0a0d 0a23 2320 5072 7573 614c 696e 6b50  ...## PrusaLinkP
-00000b30: 792e 6765 745f 7665 7273 696f 6e28 290d  y.get_version().
-00000b40: 0a0d 0a52 6561 6420 7665 7273 696f 6e20  ...Read version 
-00000b50: 3a0d 0a0d 0a0d 0a20 2020 2069 6d70 6f72  :......    impor
-00000b60: 7420 5072 7573 614c 696e 6b50 790d 0a20  t PrusaLinkPy.. 
-00000b70: 2020 2070 7275 7361 4d69 6e69 203d 2050     prusaMini = P
-00000b80: 7275 7361 4c69 6e6b 5079 2e50 7275 7361  rusaLinkPy.Prusa
-00000b90: 4c69 6e6b 5079 2822 3139 322e 3136 382e  LinkPy("192.168.
-00000ba0: 302e 3132 3322 2c20 2238 6f6a 484b 4847  0.123", "8ojHKHG
-00000bb0: 4e75 4148 4132 624d 222c 2070 6f72 743d  NuAHA2bM", port=
-00000bc0: 3830 3137 290d 0a20 2020 206f 626a 203d  8017)..    obj =
-00000bd0: 2070 7275 7361 4d69 6e69 2e67 6574 5f76   prusaMini.get_v
-00000be0: 6572 7369 6f6e 2829 0d0a 2020 2020 6f62  ersion()..    ob
-00000bf0: 6a2e 6a73 6f6e 2829 0d0a 2020 2020 0d0a  j.json()..    ..
-00000c00: 5265 7475 726e 2073 6f6d 6574 6869 6e67  Return something
-00000c10: 206c 696b 6520 3a0d 0a0d 0a20 2020 207b   like :....    {
-00000c20: 0d0a 2020 2020 2020 2020 2761 7069 273a  ..        'api':
-00000c30: 2027 322e 302e 3027 2c20 0d0a 2020 2020   '2.0.0', ..    
-00000c40: 2020 2020 2773 6572 7665 7227 3a20 2732      'server': '2
-00000c50: 2e31 2e32 272c 200d 0a20 2020 2020 2020  .1.2', ..       
-00000c60: 2027 6e6f 7a7a 6c65 5f64 6961 6d65 7465   'nozzle_diamete
-00000c70: 7227 3a20 302e 342c 200d 0a20 2020 2020  r': 0.4, ..     
-00000c80: 2020 2027 7465 7874 273a 2027 5072 7573     'text': 'Prus
-00000c90: 614c 696e 6b27 2c20 0d0a 2020 2020 2020  aLink', ..      
-00000ca0: 2020 2768 6f73 746e 616d 6527 3a20 2727    'hostname': ''
-00000cb0: 2c20 0d0a 2020 2020 2020 2020 2763 6170  , ..        'cap
-00000cc0: 6162 696c 6974 6965 7327 3a20 0d0a 2020  abilities': ..  
-00000cd0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00000ce0: 2020 2020 2027 7570 6c6f 6164 2d62 792d       'upload-by-
-00000cf0: 7075 7427 3a20 5472 7565 0d0a 2020 2020  put': True..    
-00000d00: 2020 2020 7d0d 0a20 2020 207d 0d0a 0d0a      }..    }....
-00000d10: 0d0a 2323 2050 7275 7361 4c69 6e6b 5079  ..## PrusaLinkPy
-00000d20: 2e67 6574 5f70 7269 6e74 6572 2829 0d0a  .get_printer()..
-00000d30: 0d0a 4765 7420 7072 696e 7465 7220 3a0d  ..Get printer :.
-00000d40: 0a0d 0a20 2020 2069 6d70 6f72 7420 5072  ...    import Pr
-00000d50: 7573 614c 696e 6b50 790d 0a20 2020 2070  usaLinkPy..    p
-00000d60: 7275 7361 4d69 6e69 203d 2050 7275 7361  rusaMini = Prusa
-00000d70: 4c69 6e6b 5079 2e50 7275 7361 4c69 6e6b  LinkPy.PrusaLink
-00000d80: 5079 2822 3139 322e 3136 382e 302e 3132  Py("192.168.0.12
-00000d90: 3322 2c20 2238 6f6a 484b 4847 4e75 4148  3", "8ojHKHGNuAH
-00000da0: 4132 624d 2229 0d0a 2020 2020 6f62 6a20  A2bM")..    obj 
-00000db0: 3d20 7072 7573 614d 696e 692e 6765 745f  = prusaMini.get_
-00000dc0: 7072 696e 7465 7228 290d 0a20 2020 206f  printer()..    o
-00000dd0: 626a 2e6a 736f 6e28 290d 0a20 2020 200d  bj.json()..    .
-00000de0: 0a57 6169 7469 6e67 2066 6f72 2043 6861  .Waiting for Cha
-00000df0: 6e67 696e 6720 4669 6c61 6d65 6e74 203a  nging Filament :
-00000e00: 0d0a 0d0a 2020 2020 276c 696e 6b5f 7374  ....    'link_st
-00000e10: 6174 6527 3a20 2741 5454 454e 5449 4f4e  ate': 'ATTENTION
-00000e20: 2720 0d0a 2020 2020 2765 7272 6f72 273a  ' ..    'error':
-00000e30: 2054 7275 650d 0a20 2020 200d 0a52 6574   True..    ..Ret
-00000e40: 7572 6e20 736f 6d65 7468 696e 6720 6c69  urn something li
-00000e50: 6b65 203a 0d0a 0d0a 2020 2020 7b0d 0a20  ke :....    {.. 
-00000e60: 2020 2020 2020 2027 7465 6c65 6d65 7472         'telemetr
-00000e70: 7927 3a20 0d0a 2020 2020 2020 2020 7b0d  y': ..        {.
-00000e80: 0a20 2020 2020 2020 2020 2020 2027 7465  .            'te
-00000e90: 6d70 2d62 6564 273a 2031 362e 332c 0d0a  mp-bed': 16.3,..
-00000ea0: 2020 2020 2020 2020 2020 2020 2774 656d              'tem
-00000eb0: 702d 6e6f 7a7a 6c65 273a 2031 362e 372c  p-nozzle': 16.7,
-00000ec0: 0d0a 2020 2020 2020 2020 2020 2020 2770  ..            'p
-00000ed0: 7269 6e74 2d73 7065 6564 273a 2031 3030  rint-speed': 100
-00000ee0: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00000ef0: 7a2d 6865 6967 6874 273a 2038 322e 302c  z-height': 82.0,
-00000f00: 0d0a 2020 2020 2020 2020 2020 2020 276d  ..            'm
-00000f10: 6174 6572 6961 6c27 3a20 2750 4c41 270d  aterial': 'PLA'.
-00000f20: 0a20 2020 2020 2020 207d 2c20 0d0a 2020  .        }, ..  
-00000f30: 2020 2020 2020 2774 656d 7065 7261 7475        'temperatu
-00000f40: 7265 273a 200d 0a20 2020 2020 2020 207b  re': ..        {
-00000f50: 0d0a 2020 2020 2020 2020 2020 2020 2774  ..            't
-00000f60: 6f6f 6c30 273a 200d 0a20 2020 2020 2020  ool0': ..       
-00000f70: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00000f80: 2020 2020 2020 2020 2761 6374 7561 6c27          'actual'
-00000f90: 3a20 3136 2e37 2c0d 0a20 2020 2020 2020  : 16.7,..       
-00000fa0: 2020 2020 2020 2020 2027 7461 7267 6574           'target
-00000fb0: 273a 2030 2e30 2c0d 0a20 2020 2020 2020  ': 0.0,..       
-00000fc0: 2020 2020 2020 2020 2027 6469 7370 6c61           'displa
-00000fd0: 7927 3a20 302e 302c 0d0a 2020 2020 2020  y': 0.0,..      
-00000fe0: 2020 2020 2020 2020 2020 276f 6666 7365            'offse
-00000ff0: 7427 3a20 300d 0a20 2020 2020 2020 2020  t': 0..         
-00001000: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
-00001010: 2020 2027 6265 6427 3a20 0d0a 2020 2020     'bed': ..    
-00001020: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00001030: 2020 2020 2020 2020 2020 2027 6163 7475             'actu
-00001040: 616c 273a 3136 2e33 2c0d 0a20 2020 2020  al':16.3,..     
-00001050: 2020 2020 2020 2020 2020 2027 7461 7267             'targ
-00001060: 6574 273a 2030 2e30 2c0d 0a20 2020 2020  et': 0.0,..     
-00001070: 2020 2020 2020 2020 2020 2027 6f66 6673             'offs
-00001080: 6574 273a 2030 0d0a 2020 2020 2020 2020  et': 0..        
-00001090: 2020 2020 7d0d 0a20 2020 2020 2020 207d      }..        }
-000010a0: 2c0d 0a20 2020 2020 2020 2027 7374 6174  ,..        'stat
-000010b0: 6527 3a20 0d0a 2020 2020 2020 2020 7b0d  e': ..        {.
-000010c0: 0a20 2020 2020 2020 2020 2020 2027 7465  .            'te
-000010d0: 7874 273a 2027 4f70 6572 6174 696f 6e61  xt': 'Operationa
-000010e0: 6c27 2c0d 0a20 2020 2020 2020 2020 2020  l',..           
-000010f0: 2027 666c 6167 7327 3a20 0d0a 2020 2020   'flags': ..    
-00001100: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00001110: 2020 2020 2020 2020 2020 2027 6f70 6572             'oper
-00001120: 6174 696f 6e61 6c27 3a20 5472 7565 2c0d  ational': True,.
-00001130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001140: 2027 7061 7573 6564 273a 2046 616c 7365   'paused': False
-00001150: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001160: 2020 2027 7072 696e 7469 6e67 273a 2046     'printing': F
-00001170: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-00001180: 2020 2020 2020 2027 6361 6e63 656c 6c69         'cancelli
-00001190: 6e67 273a 2046 616c 7365 2c0d 0a20 2020  ng': False,..   
-000011a0: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
-000011b0: 7573 696e 6727 3a20 4661 6c73 652c 0d0a  using': False,..
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 2765 7272 6f72 273a 2046 616c 7365 2c0d  'error': False,.
-000011e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011f0: 2027 7364 5265 6164 7927 3a20 4661 6c73   'sdReady': Fals
-00001200: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00001210: 2020 2020 2763 6c6f 7365 644f 6e45 7272      'closedOnErr
-00001220: 6f72 273a 2046 616c 7365 2c0d 0a20 2020  or': False,..   
-00001230: 2020 2020 2020 2020 2020 2020 2027 7265               're
-00001240: 6164 7927 3a20 5472 7565 2c0d 0a20 2020  ady': True,..   
-00001250: 2020 2020 2020 2020 2020 2020 2027 6275               'bu
-00001260: 7379 273a 2046 616c 7365 0d0a 2020 2020  sy': False..    
-00001270: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00001280: 2020 207d 0d0a 2020 2020 7d0d 0a0d 0a23     }..    }....#
-00001290: 2320 5072 7573 614c 696e 6b50 792e 6765  # PrusaLinkPy.ge
-000012a0: 745f 6a6f 6228 290d 0a0d 0a47 6574 206a  t_job()....Get j
-000012b0: 6f62 203a 0d0a 0d0a 2020 2020 696d 706f  ob :....    impo
-000012c0: 7274 2050 7275 7361 4c69 6e6b 5079 0d0a  rt PrusaLinkPy..
-000012d0: 2020 2020 7072 7573 614d 696e 6920 3d20      prusaMini = 
-000012e0: 5072 7573 614c 696e 6b50 792e 5072 7573  PrusaLinkPy.Prus
-000012f0: 614c 696e 6b50 7928 2231 3932 2e31 3638  aLinkPy("192.168
-00001300: 2e30 2e31 3233 222c 2022 386f 6a48 4b48  .0.123", "8ojHKH
-00001310: 474e 7541 4841 3262 4d22 290d 0a20 2020  GNuAHA2bM")..   
-00001320: 206f 626a 203d 2070 7275 7361 4d69 6e69   obj = prusaMini
-00001330: 2e67 6574 5f6a 6f62 2829 0d0a 2020 2020  .get_job()..    
-00001340: 6f62 6a2e 6a73 6f6e 2829 0d0a 2020 2020  obj.json()..    
-00001350: 0d0a 5265 7475 726e 2073 6f6d 6574 6869  ..Return somethi
-00001360: 6e67 206c 696b 6520 3a0d 0a0d 0a20 2020  ng like :....   
-00001370: 207b 0d0a 2020 2020 2020 2020 2273 7461   {..        "sta
-00001380: 7465 223a 224f 7065 7261 7469 6f6e 616c  te":"Operational
-00001390: 222c 0d0a 2020 2020 2020 2020 226a 6f62  ",..        "job
-000013a0: 223a 204e 6f6e 652c 0d0a 2020 2020 2020  ": None,..      
-000013b0: 2020 2270 726f 6772 6573 7322 3a20 4e6f    "progress": No
-000013c0: 6e65 0d0a 2020 2020 7d0d 0a20 2020 200d  ne..    }..    .
-000013d0: 0a23 2320 5072 7573 614c 696e 6b50 792e  .## PrusaLinkPy.
-000013e0: 6465 6c65 7465 5f6a 6f62 286a 6f62 290d  delete_job(job).
-000013f0: 0a0d 0a44 656c 6574 6520 6120 6a6f 622e  ...Delete a job.
-00001400: 204a 6f62 206e 756d 6265 7220 6973 2061   Job number is a
-00001410: 7661 696c 6162 6c65 2077 6974 6820 6765  vailable with ge
-00001420: 745f 6a6f 6228 2920 6f72 2067 6574 5f73  t_job() or get_s
-00001430: 7461 7475 7328 290d 0a0d 0a20 2020 2069  tatus()....    i
-00001440: 6d70 6f72 7420 5072 7573 614c 696e 6b50  mport PrusaLinkP
-00001450: 790d 0a20 2020 2070 7275 7361 4d69 6e69  y..    prusaMini
-00001460: 203d 2050 7275 7361 4c69 6e6b 5079 2e50   = PrusaLinkPy.P
-00001470: 7275 7361 4c69 6e6b 5079 2822 3139 322e  rusaLinkPy("192.
-00001480: 3136 382e 302e 3132 3322 2c20 2238 6f6a  168.0.123", "8oj
-00001490: 484b 4847 4e75 4148 4132 624d 2229 0d0a  HKHGNuAHA2bM")..
-000014a0: 2020 2020 6f62 6a20 3d20 7072 7573 614d      obj = prusaM
-000014b0: 696e 692e 6465 6c65 7465 5f6a 6f62 2822  ini.delete_job("
-000014c0: 3433 2229 0d0a 2020 2020 0d0a 0d0a 2323  43")..    ....##
-000014d0: 2050 7275 7361 4c69 6e6b 5079 2e67 6574   PrusaLinkPy.get
-000014e0: 5f73 7461 7475 7328 290d 0a0d 0a47 6574  _status()....Get
-000014f0: 206a 6f62 203a 0d0a 0d0a 2020 2020 696d   job :....    im
-00001500: 706f 7274 2050 7275 7361 4c69 6e6b 5079  port PrusaLinkPy
-00001510: 0d0a 2020 2020 7072 7573 614d 696e 6920  ..    prusaMini 
-00001520: 3d20 5072 7573 614c 696e 6b50 792e 5072  = PrusaLinkPy.Pr
-00001530: 7573 614c 696e 6b50 7928 2231 3932 2e31  usaLinkPy("192.1
-00001540: 3638 2e30 2e31 3233 222c 2022 386f 6a48  68.0.123", "8ojH
-00001550: 4b48 474e 7541 4841 3262 4d22 290d 0a20  KHGNuAHA2bM").. 
-00001560: 2020 206f 626a 203d 2070 7275 7361 4d69     obj = prusaMi
-00001570: 6e69 2e67 6574 5f73 7461 7475 7328 290d  ni.get_status().
-00001580: 0a20 2020 206f 626a 2e6a 736f 6e28 290d  .    obj.json().
-00001590: 0a20 2020 200d 0a56 616c 7565 206f 6620  .    ..Value of 
-000015a0: 7072 696e 7465 722d 3e73 7461 7465 203a  printer->state :
-000015b0: 0d0a 0d0a 2020 2020 4944 4c45 2028 4d61  ....    IDLE (Ma
-000015c0: 696e 2053 6372 6565 6e29 0d0a 2020 2020  in Screen)..    
-000015d0: 5052 494e 5449 4e47 0d0a 2020 2020 4649  PRINTING..    FI
-000015e0: 4e49 5348 4544 2028 5072 696e 7420 6669  NISHED (Print fi
-000015f0: 6e69 7368 2c20 7363 7265 656e 206e 6f74  nish, screen not
-00001600: 206f 6e20 6d61 696e 2073 6372 6565 6e29   on main screen)
-00001610: 0d0a 2020 2020 5041 5553 4544 2028 5061  ..    PAUSED (Pa
-00001620: 7573 6520 6279 2075 7365 722c 2050 7269  use by user, Pri
-00001630: 6e74 2066 616e 2065 7272 6f72 290d 0a20  nt fan error).. 
-00001640: 2020 2053 544f 5050 4544 2028 5072 696e     STOPPED (Prin
-00001650: 7420 6669 6e69 7368 2c20 7374 6f70 7065  t finish, stoppe
-00001660: 6420 6279 2075 7365 7229 0d0a 2020 2020  d by user)..    
-00001670: 4154 5445 4e54 494f 4e20 2846 696c 616d  ATTENTION (Filam
-00001680: 656e 7420 4368 616e 6765 290d 0a20 2020  ent Change)..   
-00001690: 200d 0a52 6574 7572 6e20 736f 6d65 7468   ..Return someth
-000016a0: 696e 6720 6c69 6b65 203a 0d0a 0d0a 2020  ing like :....  
-000016b0: 2020 7b0d 0a20 2020 2020 2020 2022 6a6f    {..        "jo
-000016c0: 6222 3a0d 0a20 2020 2020 2020 207b 0d0a  b":..        {..
-000016d0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
-000016e0: 3a34 332c 0d0a 2020 2020 2020 2020 2020  :43,..          
-000016f0: 2020 2270 726f 6772 6573 7322 3a30 2e30    "progress":0.0
-00001700: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00001710: 2274 696d 655f 7265 6d61 696e 696e 6722  "time_remaining"
-00001720: 3a31 3230 2c0d 0a20 2020 2020 2020 2020  :120,..         
-00001730: 2020 2022 7469 6d65 5f70 7269 6e74 696e     "time_printin
-00001740: 6722 3a31 3433 0d0a 2020 2020 2020 2020  g":143..        
-00001750: 7d2c 0d0a 2020 2020 2020 2020 2273 746f  },..        "sto
-00001760: 7261 6765 223a 0d0a 2020 2020 2020 2020  rage":..        
-00001770: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00001780: 7061 7468 223a 222f 7573 622f 222c 0d0a  path":"/usb/",..
-00001790: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-000017a0: 6522 3a22 7573 6222 2c0d 0a20 2020 2020  e":"usb",..     
-000017b0: 2020 2020 2020 2022 7265 6164 5f6f 6e6c         "read_onl
-000017c0: 7922 3a66 616c 7365 0d0a 2020 2020 2020  y":false..      
-000017d0: 2020 7d2c 0d0a 2020 2020 2020 2020 2270    },..        "p
-000017e0: 7269 6e74 6572 223a 0d0a 2020 2020 2020  rinter":..      
-000017f0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00001800: 2022 7374 6174 6522 3a22 5052 494e 5449   "state":"PRINTI
-00001810: 4e47 222c 0d0a 2020 2020 2020 2020 2020  NG",..          
-00001820: 2020 2274 656d 705f 6265 6422 3a35 372e    "temp_bed":57.
-00001830: 332c 0d0a 2020 2020 2020 2020 2020 2020  3,..            
-00001840: 2274 6172 6765 745f 6265 6422 3a30 2e30  "target_bed":0.0
-00001850: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00001860: 7465 6d70 5f6e 6f7a 7a6c 6522 3a32 342e  temp_nozzle":24.
-00001870: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
-00001880: 2274 6172 6765 745f 6e6f 7a7a 6c65 223a  "target_nozzle":
-00001890: 302e 302c 0d0a 2020 2020 2020 2020 2020  0.0,..          
-000018a0: 2020 2261 7869 735f 7a22 3a31 3632 2e32    "axis_z":162.2
-000018b0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000018c0: 666c 6f77 223a 3130 302c 0d0a 2020 2020  flow":100,..    
-000018d0: 2020 2020 2020 2020 2273 7065 6564 223a          "speed":
-000018e0: 3130 302c 0d0a 2020 2020 2020 2020 2020  100,..          
-000018f0: 2020 2266 616e 5f68 6f74 656e 6422 3a30    "fan_hotend":0
-00001900: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00001910: 6661 6e5f 7072 696e 7422 3a30 0d0a 2020  fan_print":0..  
-00001920: 2020 2020 2020 7d0d 0a20 2020 207d 0d0a        }..    }..
-00001930: 2020 2020 0d0a 2323 2050 7275 7361 4c69      ..## PrusaLi
-00001940: 6e6b 5079 2e67 6574 5f73 746f 7261 6765  nkPy.get_storage
-00001950: 2829 0d0a 0d0a 4765 7420 6a6f 6220 3a0d  ()....Get job :.
-00001960: 0a0d 0a20 2020 2069 6d70 6f72 7420 5072  ...    import Pr
-00001970: 7573 614c 696e 6b50 790d 0a20 2020 2070  usaLinkPy..    p
-00001980: 7275 7361 4d69 6e69 203d 2050 7275 7361  rusaMini = Prusa
-00001990: 4c69 6e6b 5079 2e50 7275 7361 4c69 6e6b  LinkPy.PrusaLink
-000019a0: 5079 2822 3139 322e 3136 382e 302e 3132  Py("192.168.0.12
-000019b0: 3322 2c20 2238 6f6a 484b 4847 4e75 4148  3", "8ojHKHGNuAH
-000019c0: 4132 624d 2229 0d0a 2020 2020 6f62 6a20  A2bM")..    obj 
-000019d0: 3d20 7072 7573 614d 696e 692e 6765 745f  = prusaMini.get_
-000019e0: 7374 6f72 6167 6528 290d 0a20 2020 206f  storage()..    o
-000019f0: 626a 2e6a 736f 6e28 290d 0a20 2020 200d  bj.json()..    .
-00001a00: 0a52 6574 7572 6e20 736f 6d65 7468 696e  .Return somethin
-00001a10: 6720 6c69 6b65 203a 0d0a 0d0a 2020 2020  g like :....    
-00001a20: 7b0d 0a20 2020 2020 2020 2027 7374 6f72  {..        'stor
-00001a30: 6167 655f 6c69 7374 273a 200d 0a20 2020  age_list': ..   
-00001a40: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
-00001a50: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00001a60: 2020 2020 2020 2027 7061 7468 273a 2027         'path': '
-00001a70: 2f75 7362 2f27 2c20 0d0a 2020 2020 2020  /usb/', ..      
-00001a80: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
-00001a90: 3a20 2775 7362 272c 0d0a 2020 2020 2020  : 'usb',..      
-00001aa0: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
-00001ab0: 3a20 2755 5342 272c 200d 0a20 2020 2020  : 'USB', ..     
-00001ac0: 2020 2020 2020 2020 2020 2027 7265 6164             'read
-00001ad0: 5f6f 6e6c 7927 3a20 4661 6c73 652c 200d  _only': False, .
-00001ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001af0: 2027 6176 6169 6c61 626c 6527 3a20 5472   'available': Tr
-00001b00: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00001b10: 7d0d 0a20 2020 2020 2020 205d 0d0a 2020  }..        ]..  
-00001b20: 2020 7d0d 0a20 2020 200d 0a23 2320 5072    }..    ..## Pr
-00001b30: 7573 614c 696e 6b50 792e 6765 745f 7472  usaLinkPy.get_tr
-00001b40: 616e 7366 6572 2829 0d0a 0d0a 4e6f 7420  ansfer()....Not 
-00001b50: 5465 7374 6564 0d0a 0d0a 4765 7420 6a6f  Tested....Get jo
-00001b60: 6220 3a0d 0a0d 0a20 2020 2069 6d70 6f72  b :....    impor
-00001b70: 7420 5072 7573 614c 696e 6b50 790d 0a20  t PrusaLinkPy.. 
-00001b80: 2020 2070 7275 7361 4d69 6e69 203d 2050     prusaMini = P
-00001b90: 7275 7361 4c69 6e6b 5079 2e50 7275 7361  rusaLinkPy.Prusa
-00001ba0: 4c69 6e6b 5079 2822 3139 322e 3136 382e  LinkPy("192.168.
-00001bb0: 302e 3132 3322 2c20 2238 6f6a 484b 4847  0.123", "8ojHKHG
-00001bc0: 4e75 4148 4132 624d 2229 0d0a 2020 2020  NuAHA2bM")..    
-00001bd0: 6f62 6a20 3d20 7072 7573 614d 696e 692e  obj = prusaMini.
-00001be0: 6765 745f 7472 616e 7366 6572 2829 0d0a  get_transfer()..
-00001bf0: 2020 2020 6f62 6a2e 7465 7874 0d0a 2020      obj.text..  
-00001c00: 2020 0d0a 5265 7475 726e 2073 6f6d 6574    ..Return somet
-00001c10: 6869 6e67 206c 696b 6520 3a0d 0a0d 0a20  hing like :.... 
-00001c20: 2020 2054 4f44 4f0d 0a20 2020 200d 0a23     TODO..    ..#
-00001c30: 2320 5072 7573 614c 696e 6b50 792e 6765  # PrusaLinkPy.ge
-00001c40: 745f 7365 7474 696e 6773 2829 0d0a 0d0a  t_settings()....
-00001c50: 436f 6d70 6c65 7465 6c79 2075 7365 6c65  Completely usele
-00001c60: 7373 0d0a 0d0a 5365 6520 6865 7265 203a  ss....See here :
-00001c70: 0d0a 0d0a 6874 7470 733a 2f2f 6769 7468  ....https://gith
-00001c80: 7562 2e63 6f6d 2f70 7275 7361 3364 2f50  ub.com/prusa3d/P
-00001c90: 7275 7361 2d46 6972 6d77 6172 652d 4275  rusa-Firmware-Bu
-00001ca0: 6464 792f 626c 6f62 2f34 6265 6139 3233  ddy/blob/4bea923
-00001cb0: 3831 3033 3032 6436 3534 6239 3332 3239  810302d654b93229
-00001cc0: 3162 6133 3234 6561 6564 6666 3037 3266  1ba324eaedff072f
-00001cd0: 632f 6c69 622f 5755 492f 6c69 6e6b 5f63  c/lib/WUI/link_c
-00001ce0: 6f6e 7465 6e74 2f70 7275 7361 5f6c 696e  ontent/prusa_lin
-00001cf0: 6b5f 6170 692e 6370 7023 4c31 3831 4331  k_api.cpp#L181C1
-00001d00: 362d 4c31 3831 4331 360d 0a0d 0a43 6f6d  6-L181C16....Com
-00001d10: 6d65 6e74 2066 726f 6d20 5072 7573 6120  ment from Prusa 
-00001d20: 4465 7665 6c6f 7070 6572 203a 0d0a 0d0a  Developper :....
-00001d30: 2020 2020 202f 2f20 536f 6d65 2073 7475       // Some stu
-00001d40: 6273 2066 6f72 206e 6f77 2c20 746f 206d  bs for now, to m
-00001d50: 616b 6520 6d6f 7265 2063 6c69 656e 7473  ake more clients
-00001d60: 2028 696e 636c 7564 696e 6720 7468 6520   (including the 
-00001d70: 7765 6220 7061 6765 2920 6861 7070 6965  web page) happie
-00001d80: 722e 0d0a 0d0a 4765 7420 6a6f 6220 3a0d  r.....Get job :.
-00001d90: 0a0d 0a20 2020 2069 6d70 6f72 7420 5072  ...    import Pr
-00001da0: 7573 614c 696e 6b50 790d 0a20 2020 2070  usaLinkPy..    p
-00001db0: 7275 7361 4d69 6e69 203d 2050 7275 7361  rusaMini = Prusa
-00001dc0: 4c69 6e6b 5079 2e50 7275 7361 4c69 6e6b  LinkPy.PrusaLink
-00001dd0: 5079 2822 3139 322e 3136 382e 302e 3132  Py("192.168.0.12
-00001de0: 3322 2c20 2238 6f6a 484b 4847 4e75 4148  3", "8ojHKHGNuAH
-00001df0: 4132 624d 2229 0d0a 2020 2020 6f62 6a20  A2bM")..    obj 
-00001e00: 3d20 7072 7573 614d 696e 692e 6765 745f  = prusaMini.get_
-00001e10: 7472 616e 7366 6572 2829 0d0a 2020 2020  transfer()..    
-00001e20: 6f62 6a2e 7465 7874 0d0a 2020 2020 0d0a  obj.text..    ..
-00001e30: 5265 7475 726e 2073 6f6d 6574 6869 6e67  Return something
-00001e40: 206c 696b 6520 3a0d 0a0d 0a20 2020 207b   like :....    {
-00001e50: 2270 7269 6e74 6572 223a 207b 7d7d 0d0a  "printer": {}}..
-00001e60: 2020 2020 0d0a 2323 2050 7275 7361 4c69      ..## PrusaLi
-00001e70: 6e6b 5079 2e67 6574 5f66 696c 6573 2820  nkPy.get_files( 
-00001e80: 7265 6d6f 7465 4469 7220 3d20 272f 2729  remoteDir = '/')
-00001e90: 0d0a 0d0a 4765 7420 4669 6c65 7320 6f6e  ....Get Files on
-00001ea0: 2055 5342 2044 7269 7665 203a 0d0a 0d0a   USB Drive :....
-00001eb0: 2020 2020 696d 706f 7274 2050 7275 7361      import Prusa
-00001ec0: 4c69 6e6b 5079 0d0a 2020 2020 7072 7573  LinkPy..    prus
-00001ed0: 614d 696e 6920 3d20 5072 7573 614c 696e  aMini = PrusaLin
-00001ee0: 6b50 792e 5072 7573 614c 696e 6b50 7928  kPy.PrusaLinkPy(
-00001ef0: 2231 3932 2e31 3638 2e30 2e31 3233 222c  "192.168.0.123",
-00001f00: 2022 386f 6a48 4b48 474e 7541 4841 3262   "8ojHKHGNuAHA2b
-00001f10: 4d22 290d 0a20 2020 206f 626a 203d 2070  M")..    obj = p
-00001f20: 7275 7361 4d69 6e69 2e67 6574 5f66 696c  rusaMini.get_fil
-00001f30: 6573 2829 0d0a 2020 2020 6669 6c65 7352  es()..    filesR
-00001f40: 6574 203d 206f 626a 2e6a 736f 6e28 290d  et = obj.json().
-00001f50: 0a20 2020 200d 0a52 6574 7572 6e20 736f  .    ..Return so
-00001f60: 6d65 7468 696e 6720 6c69 6b65 203a 0d0a  mething like :..
-00001f70: 0d0a 2020 2020 7b0d 0a20 2020 2020 2020  ..    {..       
-00001f80: 2027 7479 7065 273a 2027 464f 4c44 4552   'type': 'FOLDER
-00001f90: 272c 200d 0a20 2020 2020 2020 2027 726f  ', ..        'ro
-00001fa0: 273a 2046 616c 7365 2c20 0d0a 2020 2020  ': False, ..    
-00001fb0: 2020 2020 276e 616d 6527 3a20 2775 7362      'name': 'usb
-00001fc0: 272c 200d 0a20 2020 2020 2020 2027 6368  ', ..        'ch
-00001fd0: 696c 6472 656e 273a 200d 0a20 2020 2020  ildren': ..     
-00001fe0: 2020 205b 0d0a 2020 2020 2020 2020 7b0d     [..        {.
-00001ff0: 0a20 2020 2020 2020 2020 2020 2027 6e61  .            'na
-00002000: 6d65 273a 2027 4d54 4e27 2c20 0d0a 2020  me': 'MTN', ..  
-00002010: 2020 2020 2020 2020 2020 2772 6f27 3a20            'ro': 
-00002020: 4661 6c73 652c 200d 0a20 2020 2020 2020  False, ..       
-00002030: 2020 2020 2027 7479 7065 273a 2027 464f       'type': 'FO
-00002040: 4c44 4552 272c 200d 0a20 2020 2020 2020  LDER', ..       
-00002050: 2020 2020 2027 6d5f 7469 6d65 7374 616d       'm_timestam
-00002060: 7027 3a20 3137 3032 3632 3839 3435 2c20  p': 1702628945, 
-00002070: 0d0a 2020 2020 2020 2020 2020 2020 2764  ..            'd
-00002080: 6973 706c 6179 5f6e 616d 6527 3a20 274d  isplay_name': 'M
-00002090: 544e 270d 0a20 2020 2020 2020 207d 2c0d  TN'..        },.
-000020a0: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-000020b0: 2020 2020 2020 2020 276e 616d 6527 3a20          'name': 
-000020c0: 2753 325f 5632 4953 272c 200d 0a20 2020  'S2_V2IS', ..   
-000020d0: 2020 2020 2020 2020 2027 726f 273a 2046           'ro': F
-000020e0: 616c 7365 2c20 0d0a 2020 2020 2020 2020  alse, ..        
-000020f0: 2020 2020 2774 7970 6527 3a20 2746 4f4c      'type': 'FOL
-00002100: 4445 5227 2c20 0d0a 2020 2020 2020 2020  DER', ..        
-00002110: 2020 2020 276d 5f74 696d 6573 7461 6d70      'm_timestamp
-00002120: 273a 2031 3730 3235 3635 3138 322c 200d  ': 1702565182, .
-00002130: 0a20 2020 2020 2020 2020 2020 2027 6469  .            'di
-00002140: 7370 6c61 795f 6e61 6d65 273a 2027 5332  splay_name': 'S2
-00002150: 5f56 3249 5327 0d0a 2020 2020 2020 2020  _V2IS'..        
-00002160: 7d0d 0a20 2020 2020 2020 205d 0d0a 2020  }..        ]..  
-00002170: 2020 7d0d 0a20 2020 200d 0a57 6f72 6b61    }..    ..Worka
-00002180: 6c73 6f20 7769 7468 2073 7562 666f 6c64  lso with subfold
-00002190: 6572 0d0a 0d0a 2020 2020 6f62 6a20 3d20  er....    obj = 
-000021a0: 7072 7573 614d 696e 692e 6765 745f 6669  prusaMini.get_fi
-000021b0: 6c65 7328 7265 6d6f 7465 4469 7220 3d20  les(remoteDir = 
-000021c0: 272f 5355 4246 4f4c 4445 5227 290d 0a0d  '/SUBFOLDER')...
-000021d0: 0a23 2320 5072 7573 614c 696e 6b50 792e  .## PrusaLinkPy.
-000021e0: 6765 745f 7265 6375 7273 6976 655f 6669  get_recursive_fi
-000021f0: 6c65 7328 2072 656d 6f74 6544 6972 203d  les( remoteDir =
-00002200: 2027 2f27 290d 0a0d 0a47 6574 2061 6c6c   '/')....Get all
-00002210: 2066 696c 6573 2028 6f6e 6c79 2067 636f   files (only gco
-00002220: 6465 2061 6e64 2062 6763 6f64 6529 2069  de and bgcode) i
-00002230: 6e20 6120 666f 6c64 6572 2061 6e64 2073  n a folder and s
-00002240: 7562 666f 6c64 6572 2e0d 0a0d 0a57 6172  ubfolder.....War
-00002250: 6e69 6e67 203a 2072 6574 7572 6e20 6e65  ning : return ne
-00002260: 7374 6564 2064 6963 742e 0d0a 0d0a 0d0a  sted dict.......
-00002270: 2020 2020 696d 706f 7274 2050 7275 7361      import Prusa
-00002280: 4c69 6e6b 5079 0d0a 2020 2020 7072 7573  LinkPy..    prus
-00002290: 614d 696e 6920 3d20 5072 7573 614c 696e  aMini = PrusaLin
-000022a0: 6b50 792e 5072 7573 614c 696e 6b50 7928  kPy.PrusaLinkPy(
-000022b0: 2231 3932 2e31 3638 2e30 2e31 3233 222c  "192.168.0.123",
-000022c0: 2022 386f 6a48 4b48 474e 7541 4841 3262   "8ojHKHGNuAHA2b
-000022d0: 4d22 290d 0a20 2020 2064 6963 7474 203d  M")..    dictt =
-000022e0: 2070 7275 7361 4d69 6e69 2e67 6574 5f72   prusaMini.get_r
-000022f0: 6563 7572 7369 7665 5f66 696c 6573 2829  ecursive_files()
-00002300: 0d0a 2020 2020 0d0a 2020 2020 7b0d 0a20  ..    ..    {.. 
-00002310: 2020 2020 2020 2027 4d54 4e27 3a20 0d0a         'MTN': ..
-00002320: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00002330: 2020 2020 2020 2027 4348 4754 5f42 5553         'CHGT_BUS
-00002340: 452e 6763 6f64 6527 3a20 272f 4d54 4e2f  E.gcode': '/MTN/
-00002350: 4348 4754 5f42 7e31 2e47 434f 272c 200d  CHGT_B~1.GCO', .
-00002360: 0a20 2020 2020 2020 2020 2020 2027 4445  .            'DE
-00002370: 424f 5543 4841 4745 2e67 636f 6465 273a  BOUCHAGE.gcode':
-00002380: 2027 2f4d 544e 2f44 4542 4f55 437e 312e   '/MTN/DEBOUC~1.
-00002390: 4743 4f27 2c20 0d0a 2020 2020 2020 2020  GCO', ..        
-000023a0: 2020 2020 2750 5245 4348 4155 4646 452e      'PRECHAUFFE.
-000023b0: 6763 6f64 6527 3a20 272f 4d54 4e2f 5052  gcode': '/MTN/PR
-000023c0: 4543 4841 7e31 2e47 434f 270d 0a20 2020  ECHA~1.GCO'..   
-000023d0: 2020 2020 207d 2c20 0d0a 2020 2020 2020       }, ..      
-000023e0: 2020 2753 325f 5632 4953 273a 200d 0a20    'S2_V2IS': .. 
-000023f0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00002400: 2020 2020 2020 2732 6833 336d 2e62 6763        '2h33m.bgc
-00002410: 6f64 6527 3a20 272f 5332 5f56 3249 532f  ode': '/S2_V2IS/
-00002420: 3248 3333 4d7e 312e 4247 4327 2c0d 0a20  2H33M~1.BGC',.. 
-00002430: 2020 2020 2020 2020 2020 2027 3568 356d             '5h5m
-00002440: 2e62 6763 6f64 6527 3a20 272f 5332 5f56  .bgcode': '/S2_V
-00002450: 3249 532f 3548 354d 7e31 2e42 4743 270d  2IS/5H5M~1.BGC'.
-00002460: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
-00002470: 7d0d 0a0d 0a23 2320 5072 7573 614c 696e  }....## PrusaLin
-00002480: 6b50 792e 6465 6c65 7465 2872 656d 6f74  kPy.delete(remot
-00002490: 6550 6174 6829 200d 0a0d 0a44 656c 6574  ePath) ....Delet
-000024a0: 6520 6120 6669 6c65 206f 7220 6120 666f  e a file or a fo
-000024b0: 6c64 6572 206f 6e20 5553 4220 6472 6976  lder on USB driv
-000024c0: 650d 0a0d 0a20 2020 2069 6d70 6f72 7420  e....    import 
-000024d0: 5072 7573 614c 696e 6b50 790d 0a20 2020  PrusaLinkPy..   
-000024e0: 2070 7275 7361 4d69 6e69 203d 2050 7275   prusaMini = Pru
-000024f0: 7361 4c69 6e6b 5079 2e50 7275 7361 4c69  saLinkPy.PrusaLi
-00002500: 6e6b 5079 2822 3139 322e 3136 382e 302e  nkPy("192.168.0.
-00002510: 3132 3322 2c20 2238 6f6a 484b 4847 4e75  123", "8ojHKHGNu
-00002520: 4148 4132 624d 2229 0d0a 2020 2020 6f62  AHA2bM")..    ob
-00002530: 6a20 3d20 7072 7573 614d 696e 692e 6465  j = prusaMini.de
-00002540: 6c65 7465 2827 2f44 4542 4f55 437e 312e  lete('/DEBOUC~1.
-00002550: 4743 4f27 290d 0a0d 0a0d 0a23 2320 5072  GCO')......## Pr
-00002560: 7573 614c 696e 6b50 792e 706f 7374 5f67  usaLinkPy.post_g
-00002570: 636f 6465 2872 656d 6f74 6550 6174 6829  code(remotePath)
-00002580: 200d 0a0d 0a50 7269 6e74 2061 2066 696c   ....Print a fil
-00002590: 6520 616c 7265 6164 7920 706f 7265 7365  e already porese
-000025a0: 6e74 206f 6e20 5553 4220 6b65 7920 0d0a  nt on USB key ..
-000025b0: 0d0a 2020 2020 696d 706f 7274 2050 7275  ..    import Pru
-000025c0: 7361 4c69 6e6b 5079 0d0a 2020 2020 7072  saLinkPy..    pr
-000025d0: 7573 614d 696e 6920 3d20 5072 7573 614c  usaMini = PrusaL
-000025e0: 696e 6b50 792e 5072 7573 614c 696e 6b50  inkPy.PrusaLinkP
-000025f0: 7928 2231 3932 2e31 3638 2e30 2e31 3233  y("192.168.0.123
-00002600: 222c 2022 386f 6a48 4b48 474e 7541 4841  ", "8ojHKHGNuAHA
-00002610: 3262 4d22 290d 0a20 2020 206f 626a 203d  2bM")..    obj =
-00002620: 2070 7275 7361 4d69 6e69 2e70 6f73 745f   prusaMini.post_
-00002630: 6763 6f64 6528 272f 4445 424f 5543 7e31  gcode('/DEBOUC~1
-00002640: 2e47 434f 2729 0d0a 0d0a 2323 2050 7275  .GCO')....## Pru
-00002650: 7361 4c69 6e6b 5079 2e70 7574 5f67 636f  saLinkPy.put_gco
-00002660: 6465 2872 656d 6f74 6550 6174 682c 2070  de(remotePath, p
-00002670: 7269 6e74 4166 7465 7255 706c 6f61 6420  rintAfterUpload 
-00002680: 3d20 4661 6c73 652c 206f 7665 7277 7269  = False, overwri
-00002690: 7465 203d 2046 616c 7365 2920 0d0a 0d0a  te = False) ....
-000026a0: 5365 6e64 2061 2066 696c 6520 6f6e 2055  Send a file on U
-000026b0: 5342 2044 7269 7665 2e0d 0a0d 0a43 616e  SB Drive.....Can
-000026c0: 2063 7265 6174 6520 6120 666f 6c64 6572   create a folder
-000026d0: 2021 0d0a 0d0a 6966 2072 6574 2e73 7461   !....if ret.sta
-000026e0: 7475 735f 636f 6465 203d 2034 3039 202d  tus_code = 409 -
-000026f0: 3e20 436f 6e66 6c69 6374 203a 2046 696c  > Conflict : Fil
-00002700: 6520 616c 7265 6164 7920 6578 6973 7473  e already exists
-00002710: 0d0a 6966 2072 6574 2e73 7461 7475 735f  ..if ret.status_
-00002720: 636f 6465 203d 2034 3135 202d 3e20 7b22  code = 415 -> {"
-00002730: 7469 746c 6522 3a20 2234 3135 3a20 556e  title": "415: Un
-00002740: 7375 7070 6f72 7465 6420 4d65 6469 6120  supported Media 
-00002750: 5479 7065 222c 226d 6573 7361 6765 223a  Type","message":
-00002760: 224e 6f74 2061 2047 434f 4445 227d 0d0a  "Not a GCODE"}..
-00002770: 0d0a 7072 696e 7441 6674 6572 5570 6c6f  ..printAfterUplo
-00002780: 6164 203a 2053 6574 2061 7420 5472 7565  ad : Set at True
-00002790: 2074 6f20 7072 696e 7420 6166 7465 7220   to print after 
-000027a0: 7570 6c6f 6164 2e20 0d0a 0d0a 6f76 6572  upload. ....over
-000027b0: 7772 6974 6520 3a20 416c 6c6f 7720 6669  write : Allow fi
-000027c0: 6c65 204f 7665 7277 7269 7465 0d0a 0d0a  le Overwrite....
-000027d0: 4657 2035 2e31 2e30 203a 0d0a 0d0a 202a  FW 5.1.0 :.... *
-000027e0: 2057 6172 6e69 6e67 3a20 7072 696e 7469   Warning: printi
-000027f0: 6e67 2073 7461 7274 7320 6576 656e 2069  ng starts even i
-00002800: 6620 7468 6520 6265 6420 6973 206e 6f74  f the bed is not
-00002810: 2065 6d70 7479 0d0a 202a 2043 616e 206f   empty.. * Can o
-00002820: 6e6c 7920 7365 6e64 2062 6763 6f64 6520  nly send bgcode 
-00002830: 616e 6420 6763 6f64 650d 0a20 2020 200d  and gcode..    .
-00002840: 0a0d 0a20 2020 2069 6d70 6f72 7420 5072  ...    import Pr
-00002850: 7573 614c 696e 6b50 790d 0a20 2020 2070  usaLinkPy..    p
-00002860: 7275 7361 4d69 6e69 203d 2050 7275 7361  rusaMini = Prusa
-00002870: 4c69 6e6b 5079 2e50 7275 7361 4c69 6e6b  LinkPy.PrusaLink
-00002880: 5079 2822 3139 322e 3136 382e 302e 3132  Py("192.168.0.12
-00002890: 3322 2c20 2238 6f6a 484b 4847 4e75 4148  3", "8ojHKHGNuAH
-000028a0: 4132 624d 2229 0d0a 2020 2020 7374 6174  A2bM")..    stat
-000028b0: 7573 203d 2070 7275 7361 4d69 6e69 2e70  us = prusaMini.p
-000028c0: 7574 2827 433a 2f4d 544e 2f44 4542 4f55  ut('C:/MTN/DEBOU
-000028d0: 4348 4147 452e 6763 6f64 6527 202c 2027  CHAGE.gcode' , '
-000028e0: 4d54 4e2f 4445 424f 5543 4841 4745 2e67  MTN/DEBOUCHAGE.g
-000028f0: 636f 6465 2729 0d0a 2020 2020 2320 4f76  code')..    # Ov
-00002900: 6572 7772 6974 650d 0a20 2020 2073 7461  erwrite..    sta
-00002910: 7475 7320 3d20 7072 7573 614d 696e 692e  tus = prusaMini.
-00002920: 7075 7428 2743 3a2f 4d54 4e2f 4445 424f  put('C:/MTN/DEBO
-00002930: 5543 4841 4745 2e67 636f 6465 2720 2c20  UCHAGE.gcode' , 
-00002940: 274d 544e 2f44 4542 4f55 4348 4147 452e  'MTN/DEBOUCHAGE.
-00002950: 6763 6f64 6527 2c20 4661 6c73 652c 2054  gcode', False, T
-00002960: 7275 6529 0d0a 2020 2020 2320 4f76 6572  rue)..    # Over
-00002970: 7772 6974 6520 616e 6420 5072 696e 740d  write and Print.
-00002980: 0a20 2020 2073 7461 7475 7320 3d20 7072  .    status = pr
-00002990: 7573 614d 696e 692e 7075 7428 2743 3a2f  usaMini.put('C:/
-000029a0: 4d54 4e2f 4445 424f 5543 4841 4745 2e67  MTN/DEBOUCHAGE.g
-000029b0: 636f 6465 2720 2c20 274d 544e 2f44 4542  code' , 'MTN/DEB
-000029c0: 4f55 4348 4147 452e 6763 6f64 6527 2c20  OUCHAGE.gcode', 
-000029d0: 5472 7565 2c20 5472 7565 290d 0a20 2020  True, True)..   
-000029e0: 200d 0a23 2320 5072 7573 614c 696e 6b50   ..## PrusaLinkP
-000029f0: 792e 6578 6973 7473 5f67 636f 6465 2872  y.exists_gcode(r
-00002a00: 656d 6f74 6550 6174 6829 200d 0a0d 0a43  emotePath) ....C
-00002a10: 6865 636b 2069 6620 6120 6669 6c65 2065  heck if a file e
-00002a20: 7869 7374 7320 6f6e 2055 5342 2064 7269  xists on USB dri
-00002a30: 7665 2e20 0d0a 0d0a 5265 7475 726e 2054  ve. ....Return T
-00002a40: 7275 6520 6f72 2046 616c 7365 0d0a 0d0a  rue or False....
-00002a50: 2020 2020 696d 706f 7274 2050 7275 7361      import Prusa
-00002a60: 4c69 6e6b 5079 0d0a 2020 2020 7072 7573  LinkPy..    prus
-00002a70: 614d 696e 6920 3d20 5072 7573 614c 696e  aMini = PrusaLin
-00002a80: 6b50 792e 5072 7573 614c 696e 6b50 7928  kPy.PrusaLinkPy(
-00002a90: 2231 3932 2e31 3638 2e30 2e31 3233 222c  "192.168.0.123",
-00002aa0: 2022 386f 6a48 4b48 474e 7541 4841 3262   "8ojHKHGNuAHA2b
-00002ab0: 4d22 290d 0a20 2020 2073 7461 7475 7320  M")..    status 
-00002ac0: 3d20 7072 7573 614d 696e 692e 6578 6973  = prusaMini.exis
-00002ad0: 7473 5f67 636f 6465 2827 2f44 4542 4f55  ts_gcode('/DEBOU
-00002ae0: 437e 312e 4743 4f27 290d 0a0d 0a23 2320  C~1.GCO')....## 
-00002af0: 5072 7573 614c 696e 6b50 792e 7061 7573  PrusaLinkPy.paus
-00002b00: 655f 7072 696e 7428 2920 0d0a 0d0a 5061  e_print() ....Pa
-00002b10: 7573 6520 6163 7475 616c 2070 7269 6e74  use actual print
-00002b20: 2e0d 0a0d 0a41 6464 6564 2069 6e20 322e  .....Added in 2.
-00002b30: 322e 3020 2e0d 0a0d 0a23 2320 5072 7573  2.0 .....## Prus
-00002b40: 614c 696e 6b50 792e 7265 7375 6d65 5f70  aLinkPy.resume_p
-00002b50: 7269 6e74 2829 200d 0a0d 0a52 6573 756d  rint() ....Resum
-00002b60: 6520 7061 7573 6564 2070 7269 6e74 2e0d  e paused print..
-00002b70: 0a0d 0a41 6464 6564 2069 6e20 322e 322e  ...Added in 2.2.
-00002b80: 3020 2e0d 0a0d 0a23 2320 5072 7573 614c  0 .....## PrusaL
-00002b90: 696e 6b50 792e 7374 6f70 5f70 7269 6e74  inkPy.stop_print
-00002ba0: 2829 200d 0a0d 0a53 746f 7020 6163 7475  () ....Stop actu
-00002bb0: 616c 2070 7269 6e74 2e0d 0a0d 0a41 6464  al print.....Add
-00002bc0: 6564 2069 6e20 322e 322e 3020 2e0d 0a0d  ed in 2.2.0 ....
-00002bd0: 0a23 2041 5049 0d0a 0d0a 4150 4920 6e6f  .# API....API no
-00002be0: 7420 696d 706c 656d 656e 7465 6420 696e  t implemented in
-00002bf0: 206d 7920 6c69 6220 203a 200d 0a0d 0a20   my lib  : .... 
-00002c00: 2a20 7265 7472 6965 7665 2074 6875 6d62  * retrieve thumb
-00002c10: 6e61 696c 203a 0d0a 0d0a 2020 2020 7220  nail :....    r 
-00002c20: 3d20 7265 7175 6573 7473 2e67 6574 2827  = requests.get('
-00002c30: 6874 7470 3a2f 2f31 3932 2e31 3638 2e30  http://192.168.0
-00002c40: 2e31 3233 3a38 3031 372f 7468 756d 622f  .123:8017/thumb/
-00002c50: 6c2f 7573 622f 5441 5645 524e 7e31 2e47  l/usb/TAVERN~1.G
-00002c60: 434f 272c 2068 6561 6465 7273 3d68 6561  CO', headers=hea
-00002c70: 6465 7273 290d 0a0d 0a2f 6170 692f 7365  ders)..../api/se
-00002c80: 7474 696e 6773 0d0a 0d0a 0d0a 504f 5354  ttings......POST
-00002c90: 202f 6170 692f 6a6f 620d 0a2a 2a5b 4c69   /api/job..**[Li
-00002ca0: 6e6b 2074 6f20 4275 6464 7920 636f 6465  nk to Buddy code
-00002cb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002cc0: 2e63 6f6d 2f70 7275 7361 3364 2f50 7275  .com/prusa3d/Pru
-00002cd0: 7361 2d46 6972 6d77 6172 652d 4275 6464  sa-Firmware-Budd
-00002ce0: 792f 626c 6f62 2f6d 6173 7465 722f 6c69  y/blob/master/li
-00002cf0: 622f 5755 492f 6c69 6e6b 5f63 6f6e 7465  b/WUI/link_conte
-00002d00: 6e74 2f70 7275 7361 5f6c 696e 6b5f 6170  nt/prusa_link_ap
-00002d10: 692e 6370 7023 4c32 3736 292a 2a0d 0a0d  i.cpp#L276)**...
-00002d20: 0a47 4554 2f50 4f53 5420 2f61 7069 2f64  .GET/POST /api/d
-00002d30: 6f77 6e6c 6f61 6420 0d0a 2a2a 5b4c 696e  ownload ..**[Lin
-00002d40: 6b20 746f 2042 7564 6479 2063 6f64 655d  k to Buddy code]
-00002d50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002d60: 636f 6d2f 7072 7573 6133 642f 5072 7573  com/prusa3d/Prus
-00002d70: 612d 4669 726d 7761 7265 2d42 7564 6479  a-Firmware-Buddy
-00002d80: 2f62 6c6f 622f 6d61 7374 6572 2f6c 6962  /blob/master/lib
-00002d90: 2f57 5549 2f6c 696e 6b5f 636f 6e74 656e  /WUI/link_conten
-00002da0: 742f 7072 7573 615f 6c69 6e6b 5f61 7069  t/prusa_link_api
-00002db0: 2e63 7070 234c 3238 3929 2a2a 0d0a 0d0a  .cpp#L289)**....
-00002dc0: 0d0a 2320 2042 7567 7320 7072 6573 656e  ..#  Bugs presen
-00002dd0: 7420 696e 2050 7275 7361 204d 494e 4920  t in Prusa MINI 
-00002de0: 7072 696e 7465 7220 6669 726d 7761 7265  printer firmware
-00002df0: 2034 2e34 2e31 3a0d 0a0d 0a20 2a20 5468   4.4.1:.... * Th
-00002e00: 6572 6520 6973 206e 6f20 706f 7373 6962  ere is no possib
-00002e10: 696c 6974 7920 746f 2068 6176 6520 7468  ility to have th
-00002e20: 6520 6c69 7374 206f 6620 666f 6c64 6572  e list of folder
-00002e30: 7320 7072 6573 656e 7420 696e 2061 2064  s present in a d
-00002e40: 6972 6563 746f 7279 0d0a 2020 2020 2a20  irectory..    * 
-00002e50: 536f 6c76 6564 2069 6e20 6669 726d 7761  Solved in firmwa
-00002e60: 7265 2035 0d0a 202a 2059 6f75 2063 616e  re 5.. * You can
-00002e70: 6e6f 7420 7570 6c6f 6164 2061 2067 636f  not upload a gco
-00002e80: 6465 2069 6e20 6120 7375 6266 6f6c 6465  de in a subfolde
-00002e90: 7220 6f66 2074 6865 2055 5342 206b 6579  r of the USB key
-00002ea0: 0d0a 2020 2020 2a20 536f 6c76 6564 2069  ..    * Solved i
-00002eb0: 6e20 6669 726d 7761 7265 2035 0d0a 202a  n firmware 5.. *
-00002ec0: 2057 6865 6e20 7468 6520 7072 696e 7465   When the printe
-00002ed0: 7220 6465 7465 6374 7320 7468 6520 656e  r detects the en
-00002ee0: 6420 6f66 2074 6865 2066 696c 616d 656e  d of the filamen
-00002ef0: 7420 616e 6420 6974 2064 6973 706c 6179  t and it display
-00002f00: 7320 2243 6861 6e67 6520 4669 6c61 6d65  s "Change Filame
-00002f10: 6e74 2220 7468 6520 7465 6c65 6d65 7472  nt" the telemetr
-00002f20: 7920 696e 666f 726d 6174 696f 6e20 6973  y information is
-00002f30: 206e 6f20 6c6f 6e67 6572 2067 6f6f 642e   no longer good.
-00002f40: 2048 6572 6520 6973 2074 6865 2069 6e66   Here is the inf
-00002f50: 6f72 6d61 7469 6f6e 2072 6574 7572 6e65  ormation returne
-00002f60: 6420 6279 2074 6865 2070 7269 6e74 6572  d by the printer
-00002f70: 2069 6e20 7468 6973 2063 6173 653a 0d0a   in this case:..
-00002f80: 200d 0a20 2020 2027 7465 6c65 6d65 7472   ..    'telemetr
-00002f90: 7927 3a20 7b27 7465 6d70 2d62 6564 273a  y': {'temp-bed':
-00002fa0: 2030 2e30 2c20 2774 656d 702d 6e6f 7a7a   0.0, 'temp-nozz
-00002fb0: 6c65 273a 2030 2e30 2c20 2770 7269 6e74  le': 0.0, 'print
-00002fc0: 2d73 7065 6564 273a 2031 3030 2c20 277a  -speed': 100, 'z
-00002fd0: 2d68 6569 6768 7427 3a20 302e 302c 2027  -height': 0.0, '
-00002fe0: 6d61 7465 7269 616c 273a 2027 2d2d 2d27  material': '---'
-00002ff0: 7d0d 0a20 2020 200d 0a20 2a20 5374 696c  }..    .. * Stil
-00003000: 6c20 696e 2074 6865 2063 6173 6520 6f66  l in the case of
-00003010: 2061 2066 696c 616d 656e 7420 6368 616e   a filament chan
-00003020: 6765 2c20 7468 6520 7374 6174 7573 2069  ge, the status i
-00003030: 6e66 6f72 6d61 7469 6f6e 2069 7320 696e  nformation is in
-00003040: 636f 7272 6563 743a 0d0a 0d0a 2020 2020  correct:....    
-00003050: 2773 7461 7465 273a 207b 2774 6578 7427  'state': {'text'
-00003060: 3a20 274f 7065 7261 7469 6f6e 616c 272c  : 'Operational',
-00003070: 2027 666c 6167 7327 3a20 7b27 6f70 6572   'flags': {'oper
-00003080: 6174 696f 6e61 6c27 3a20 5472 7565 2c20  ational': True, 
-00003090: 2770 6175 7365 6427 3a20 4661 6c73 652c  'paused': False,
-000030a0: 2027 7072 696e 7469 6e67 273a 2046 616c   'printing': Fal
-000030b0: 7365 2c20 2763 616e 6365 6c6c 696e 6727  se, 'cancelling'
-000030c0: 3a20 4661 6c73 652c 2027 7061 7573 696e  : False, 'pausin
-000030d0: 6727 3a20 4661 6c73 652c 2027 7364 5265  g': False, 'sdRe
-000030e0: 6164 7927 3a20 4661 6c73 652c 2027 6572  ady': False, 'er
-000030f0: 726f 7227 3a20 4661 6c73 652c 2027 636c  ror': False, 'cl
-00003100: 6f73 6564 4f6e 4572 726f 7227 3a20 4661  osedOnError': Fa
-00003110: 6c73 652c 2027 7265 6164 7927 3a20 5472  lse, 'ready': Tr
-00003120: 7565 2c20 2762 7573 7927 3a20 4661 6c73  ue, 'busy': Fals
-00003130: 657d 0d0a 0d0a 0d0a 2320 496e 7370 6972  e}......# Inspir
-00003140: 6174 696f 6e0d 0a0d 0a41 6e20 6f74 6865  ation....An othe
-00003150: 7220 6c69 6220 3a20 0d0a 0d0a 6874 7470  r lib : ....http
-00003160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-00003170: 6f6d 652d 6173 7369 7374 616e 742d 6c69  ome-assistant-li
-00003180: 6273 2f50 7275 7361 4c69 6e6b 5079 2f62  bs/PrusaLinkPy/b
-00003190: 6c6f 622f 6d61 696e 2f50 7275 7361 4c69  lob/main/PrusaLi
-000031a0: 6e6b 5079 2f0d 0a0d 0a0d 0a4c 6573 2063  nkPy/......Les c
-000031b0: 6f6d 6d61 6e64 6573 2064 616e 7320 6c61  ommandes dans la
-000031c0: 206d 696e 6920 3a0d 0a68 7474 7073 3a2f   mini :..https:/
-000031d0: 2f67 6974 6875 622e 636f 6d2f 7072 7573  /github.com/prus
-000031e0: 6133 642f 5072 7573 612d 4669 726d 7761  a3d/Prusa-Firmwa
-000031f0: 7265 2d42 7564 6479 2f62 6c6f 622f 6d61  re-Buddy/blob/ma
-00003200: 7374 6572 2f6c 6962 2f57 5549 2f6c 696e  ster/lib/WUI/lin
-00003210: 6b5f 636f 6e74 656e 742f 6261 7369 635f  k_content/basic_
-00003220: 6765 7473 2e63 7070 0d0a 0d0a 0d0a 0d0a  gets.cpp........
-00003230: 2320 436f 6e73 7472 7569 7265 206c 6120  # Construire la 
-00003240: 6c69 620d 0a0d 0a20 2020 2070 7920 2d6d  lib....    py -m
-00003250: 2062 7569 6c64 0d0a 0d0a 546f 2075 706c   build....To upl
-00003260: 6f61 6420 746f 2074 6573 7470 6920 7265  oad to testpi re
-00003270: 706f 203a 0d0a 0d0a 2020 2020 7079 202d  po :....    py -
-00003280: 6d20 7477 696e 6520 7570 6c6f 6164 202d  m twine upload -
-00003290: 2d72 6570 6f73 6974 6f72 7920 7465 7374  -repository test
-000032a0: 7069 2064 6973 742f 2a0d 0a0d 0a54 6f20  pi dist/*....To 
-000032b0: 7570 6c6f 6164 2074 6f20 7079 7069 2072  upload to pypi r
-000032c0: 6570 6f20 3a0d 0a0d 0a20 2020 2070 7920  epo :....    py 
-000032d0: 2d6d 2074 7769 6e65 2075 706c 6f61 6420  -m twine upload 
-000032e0: 6469 7374 2f2a 0d0a 0d0a 0d0a 6874 7470  dist/*......http
-000032f0: 733a 2f2f 6d65 6469 756d 2e63 6f6d 2f61  s://medium.com/a
-00003300: 6e61 6c79 7469 6373 2d76 6964 6879 612f  nalytics-vidhya/
-00003310: 686f 772d 746f 2d63 7265 6174 652d 612d  how-to-create-a-
-00003320: 7079 7468 6f6e 2d6c 6962 7261 7279 2d37  python-library-7
-00003330: 6435 6165 6138 3063 6333 660d 0a0d 0a    d5aea80cc3f....
+00000090: 7374 2e0d 0a0d 0a49 6e73 7461 6c6c 6174  st.....Installat
+000000a0: 696f 6e20 3a0d 0a0d 0a20 2020 2070 6970  ion :....    pip
+000000b0: 2069 6e73 7461 6c6c 2050 7950 7275 7361   install PyPrusa
+000000c0: 4c69 6e6b 0d0a 2020 2020 0d0a 5570 6461  Link..    ..Upda
+000000d0: 7465 203a 0d0a 0d0a 2020 2020 7069 7020  te :....    pip 
+000000e0: 696e 7374 616c 6c20 5079 5072 7573 614c  install PyPrusaL
+000000f0: 696e 6b20 2d55 0d0a 0d0a 4578 616d 706c  ink -U....Exampl
+00000100: 6520 6f66 2075 7365 203a 0d0a 0d0a 2020  e of use :....  
+00000110: 2020 2320 4c69 6272 6172 7920 696d 706f    # Library impo
+00000120: 7274 0d0a 2020 2020 696d 706f 7274 2050  rt..    import P
+00000130: 7275 7361 4c69 6e6b 5079 0d0a 2020 2020  rusaLinkPy..    
+00000140: 0d0a 2020 2020 2320 5072 696e 7465 7220  ..    # Printer 
+00000150: 696e 7374 616e 7469 6174 696f 6e0d 0a20  instantiation.. 
+00000160: 2020 2023 2049 5020 3a20 3139 322e 3136     # IP : 192.16
+00000170: 382e 302e 3132 330d 0a20 2020 2023 2041  8.0.123..    # A
+00000180: 5049 204b 4559 203a 2038 6f6a 484b 4847  PI KEY : 8ojHKHG
+00000190: 4e75 4148 4132 624d 0d0a 2020 2020 7072  NuAHA2bM..    pr
+000001a0: 7573 614d 696e 6920 3d20 5072 7573 614c  usaMini = PrusaL
+000001b0: 696e 6b50 792e 5072 7573 614c 696e 6b50  inkPy.PrusaLinkP
+000001c0: 7928 2231 3932 2e31 3638 2e30 2e31 3233  y("192.168.0.123
+000001d0: 222c 2022 386f 6a48 4b48 474e 7541 4841  ", "8ojHKHGNuAHA
+000001e0: 3262 4d22 290d 0a20 2020 200d 0a20 2020  2bM")..    ..   
+000001f0: 2023 2047 6574 2062 6564 2074 656d 7065   # Get bed tempe
+00000200: 7261 7475 7265 0d0a 2020 2020 6765 7450  rature..    getP
+00000210: 7269 6e74 203d 2070 7275 7361 4d69 6e69  rint = prusaMini
+00000220: 2e67 6574 5f70 7269 6e74 6572 2829 0d0a  .get_printer()..
+00000230: 2020 2020 0d0a 2020 2020 2320 4469 7370      ..    # Disp
+00000240: 6c61 7920 6265 6420 7465 6d70 6572 6174  lay bed temperat
+00000250: 7572 650d 0a20 2020 2070 7269 6e74 2867  ure..    print(g
+00000260: 6574 5072 696e 742e 6a73 6f6e 2829 5b22  etPrint.json()["
+00000270: 7465 6c65 6d65 7472 7922 5d5b 2274 656d  telemetry"]["tem
+00000280: 702d 6265 6422 5d29 0d0a 2020 2020 0d0a  p-bed"])..    ..
+00000290: 2020 2020 2320 4465 6c65 7465 2061 2066      # Delete a f
+000002a0: 696c 6573 206f 6e20 5553 4220 6472 6976  iles on USB driv
+000002b0: 6520 3a0d 0a20 2020 2070 7275 7361 4d69  e :..    prusaMi
+000002c0: 6e69 2e64 656c 6574 6528 222f 3548 3330  ni.delete("/5H30
+000002d0: 4d5f 7e31 2e47 434f 2229 0d0a 2020 2020  M_~1.GCO")..    
+000002e0: 0d0a 2020 2020 2320 5472 616e 7366 6572  ..    # Transfer
+000002f0: 7269 6e67 2061 2066 696c 6520 746f 2074  ring a file to t
+00000300: 6865 2070 7269 6e74 6572 0d0a 2020 2020  he printer..    
+00000310: 6966 206e 6f74 2070 7275 7361 4d69 6e69  if not prusaMini
+00000320: 2e65 7869 7374 735f 6763 6f64 6528 2746  .exists_gcode('F
+00000330: 4f4c 4445 522f 7465 7374 2e67 636f 6465  OLDER/test.gcode
+00000340: 2729 203a 0d0a 2020 2020 2020 2020 7072  ') :..        pr
+00000350: 7573 614d 696e 692e 7075 745f 6763 6f64  usaMini.put_gcod
+00000360: 6528 2743 3a2f 414d 2f74 6573 742e 6763  e('C:/AM/test.gc
+00000370: 6f64 6527 2c20 2746 4f4c 4445 522f 7465  ode', 'FOLDER/te
+00000380: 7374 2e67 636f 6465 2729 0d0a 2020 2020  st.gcode')..    
+00000390: 0d0a 2020 2020 2320 4c69 7374 2066 696c  ..    # List fil
+000003a0: 6573 206f 6e20 5553 4220 4472 6976 6520  es on USB Drive 
+000003b0: 3a0d 0a20 2020 2070 7275 7361 4d69 6e69  :..    prusaMini
+000003c0: 2e67 6574 5f66 696c 6573 2829 2e6a 736f  .get_files().jso
+000003d0: 6e28 295b 2263 6869 6c64 7265 6e22 5d0d  n()["children"].
+000003e0: 0a20 2020 200d 0a20 2020 2023 2050 7269  .    ..    # Pri
+000003f0: 6e74 2074 6869 7320 6669 6c65 200d 0a20  nt this file .. 
+00000400: 2020 2070 7275 7361 4d69 6e69 2e70 6f73     prusaMini.pos
+00000410: 745f 7072 696e 745f 6763 6f64 6528 272f  t_print_gcode('/
+00000420: 7573 622f 7465 7374 2e67 636f 6465 2729  usb/test.gcode')
+00000430: 0d0a 2020 2020 0d0a 0d0a 5468 6520 6c69  ..    ....The li
+00000440: 6272 6172 7920 6368 616e 6765 6420 6974  brary changed it
+00000450: 7320 6e61 6d65 2069 6e20 4d61 7920 3230  s name in May 20
+00000460: 3234 2e20 4265 666f 7265 2069 7420 7761  24. Before it wa
+00000470: 7320 6361 6c6c 6564 2070 7275 7361 4c69  s called prusaLi
+00000480: 6e6b 2e0d 0a50 7275 7361 2073 7461 6666  nk...Prusa staff
+00000490: 2061 736b 6564 206d 6520 746f 206c 6561   asked me to lea
+000004a0: 7665 2074 6865 6d20 7468 6520 6e61 6d65  ve them the name
+000004b0: 2e0d 0a0d 0a23 2043 6861 6e67 6520 4c6f  .....# Change Lo
+000004c0: 6720 0d0a 0d0a 2323 2032 2e32 2e31 203a  g ....## 2.2.1 :
+000004d0: 0d0a 0d0a 5461 6220 636f 7272 6563 7469  ....Tab correcti
+000004e0: 6f6e 0d0a 0d0a 2323 2032 2e32 203a 0d0a  on....## 2.2 :..
+000004f0: 0d0a 2020 5665 7273 696f 6e20 6d61 6465  ..  Version made
+00000500: 2062 7920 5b65 6e72 6761 7263 695d 2868   by [enrgarci](h
+00000510: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000520: 6d2f 656e 7267 6172 6369 290d 0a20 2d20  m/enrgarci).. - 
+00000530: 5570 6461 7465 2052 4541 444d 452e 6d64  Update README.md
+00000540: 0d0a 202d 204d 6f64 6966 6965 6420 5b64  .. - Modified [d
+00000550: 656c 6574 655f 6a6f 6228 295d 2823 7072  elete_job()](#pr
+00000560: 7573 616c 696e 6b70 7964 656c 6574 655f  usalinkpydelete_
+00000570: 6a6f 6229 2074 6f20 6669 7820 7265 7175  job) to fix requ
+00000580: 6573 7420 6672 6f6d 2067 6574 2074 6f20  est from get to 
+00000590: 6465 6c65 7465 0d0a 202d 2061 6464 6564  delete.. - added
+000005a0: 203a 0d0a 2020 202d 205b 7061 7573 655f   :..   - [pause_
+000005b0: 7072 696e 7428 295d 2823 7072 7573 616c  print()](#prusal
+000005c0: 696e 6b70 7970 6175 7365 5f70 7269 6e74  inkpypause_print
+000005d0: 290d 0a20 2020 2d20 5b72 6573 756d 655f  )..   - [resume_
+000005e0: 7072 696e 7428 295d 2823 7072 7573 616c  print()](#prusal
+000005f0: 696e 6b70 7972 6573 756d 655f 7072 696e  inkpyresume_prin
+00000600: 7429 0d0a 2020 202d 205b 7374 6f70 5f70  t)..   - [stop_p
+00000610: 7269 6e74 2829 5d28 2370 7275 7361 6c69  rint()](#prusali
+00000620: 6e6b 7079 7374 6f70 5f70 7269 6e74 290d  nkpystop_print).
+00000630: 0a0d 0a23 2320 322e 312e 3120 3a0d 0a0d  ...## 2.1.1 :...
+00000640: 0a20 2d20 5570 6461 7465 2052 4541 444d  . - Update READM
+00000650: 452e 6d64 0d0a 202d 2061 6464 6564 203a  E.md.. - added :
+00000660: 0d0a 2020 202d 2067 6574 5f74 7261 6e73  ..   - get_trans
+00000670: 6665 720d 0a20 2020 2d20 6765 745f 7365  fer..   - get_se
+00000680: 7474 696e 6773 0d0a 200d 0a23 2320 322e  ttings.. ..## 2.
+00000690: 312e 3020 3a0d 0a0d 0a20 2d20 5570 6461  1.0 :.... - Upda
+000006a0: 7465 2052 4541 444d 452e 6d64 0d0a 202d  te README.md.. -
+000006b0: 2061 6464 6564 203a 0d0a 2020 202d 2064   added :..   - d
+000006c0: 656c 6574 650d 0a20 2020 2d20 5b67 6574  elete..   - [get
+000006d0: 5f73 7461 7475 7328 295d 2823 7072 7573  _status()](#prus
+000006e0: 616c 696e 6b70 7967 6574 5f73 7461 7475  alinkpyget_statu
+000006f0: 7329 0d0a 2020 202d 205b 6765 745f 7374  s)..   - [get_st
+00000700: 6f72 6167 6528 295d 2823 7072 7573 616c  orage()](#prusal
+00000710: 696e 6b70 7967 6574 5f73 746f 7261 6765  inkpyget_storage
+00000720: 290d 0a20 2020 2d20 5b64 656c 6574 655f  )..   - [delete_
+00000730: 6a6f 6228 295d 2823 7072 7573 616c 696e  job()](#prusalin
+00000740: 6b70 7964 656c 6574 655f 6a6f 6229 0d0a  kpydelete_job)..
+00000750: 200d 0a23 2320 322e 302e 3120 3a0d 0a0d   ..## 2.0.1 :...
+00000760: 0a20 2d20 4275 6720 636f 7272 6563 7469  . - Bug correcti
+00000770: 6f6e 206f 6e20 5b70 7574 5f67 636f 6465  on on [put_gcode
+00000780: 2866 696c 6550 6174 684c 6f63 616c 2c20  (filePathLocal, 
+00000790: 7265 6d6f 7465 4469 722c 2070 7269 6e74  remoteDir, print
+000007a0: 4166 7465 7255 706c 6f61 6420 3d20 4661  AfterUpload = Fa
+000007b0: 6c73 652c 206f 7665 7277 7269 7465 203d  lse, overwrite =
+000007c0: 2046 616c 7365 295d 2823 7072 7573 616c   False)](#prusal
+000007d0: 696e 6b70 7970 7574 5f67 636f 6465 7265  inkpyput_gcodere
+000007e0: 6d6f 7465 7061 7468 2d70 7269 6e74 6166  motepath-printaf
+000007f0: 7465 7275 706c 6f61 642d 2d66 616c 7365  terupload--false
+00000800: 2d6f 7665 7277 7269 7465 2d2d 6661 6c73  -overwrite--fals
+00000810: 6529 0d0a 200d 0a23 2320 322e 302e 3020  e).. ..## 2.0.0 
+00000820: 3a0d 0a0d 0a20 2d20 5375 7070 6f72 7420  :.... - Support 
+00000830: 6669 726d 7761 7265 2035 2e31 2e30 0d0a  firmware 5.1.0..
+00000840: 202d 2041 6464 6564 203a 200d 0a20 2020   - Added : ..   
+00000850: 2d20 5b67 6574 5f66 696c 6573 2872 656d  - [get_files(rem
+00000860: 6f74 6544 6972 295d 2823 7072 7573 616c  oteDir)](#prusal
+00000870: 696e 6b70 7967 6574 5f66 696c 6573 2d72  inkpyget_files-r
+00000880: 656d 6f74 6564 6972 2d2d 290d 0a20 2020  emotedir--)..   
+00000890: 2d20 5b70 7574 5f67 636f 6465 2866 696c  - [put_gcode(fil
+000008a0: 6550 6174 684c 6f63 616c 2c20 7265 6d6f  ePathLocal, remo
+000008b0: 7465 4469 722c 2070 7269 6e74 4166 7465  teDir, printAfte
+000008c0: 7255 706c 6f61 6420 3d20 4661 6c73 652c  rUpload = False,
+000008d0: 206f 7665 7277 7269 7465 203d 2046 616c   overwrite = Fal
+000008e0: 7365 295d 2823 7072 7573 616c 696e 6b70  se)](#prusalinkp
+000008f0: 7970 7574 5f67 636f 6465 7265 6d6f 7465  yput_gcoderemote
+00000900: 7061 7468 2d70 7269 6e74 6166 7465 7275  path-printafteru
+00000910: 706c 6f61 642d 2d66 616c 7365 2d6f 7665  pload--false-ove
+00000920: 7277 7269 7465 2d2d 6661 6c73 6529 0d0a  rwrite--false)..
+00000930: 2020 202d 205b 6578 6973 7473 5f67 636f     - [exists_gco
+00000940: 6465 2872 656d 6f74 6550 6174 6829 5d28  de(remotePath)](
+00000950: 2370 7275 7361 6c69 6e6b 7079 6578 6973  #prusalinkpyexis
+00000960: 7473 5f67 636f 6465 7265 6d6f 7465 7061  ts_gcoderemotepa
+00000970: 7468 290d 0a20 0d0a 2323 2031 2e30 2e30  th).. ..## 1.0.0
+00000980: 203a 0d0a 0d0a 202d 2046 6972 7374 2052   :.... - First R
+00000990: 656c 6561 7365 0d0a 0d0a 2320 496e 7374  elease....# Inst
+000009a0: 616c 6c69 6e67 2050 7275 7361 4c69 6e6b  alling PrusaLink
+000009b0: 5079 2061 6e64 2053 7570 706f 7274 6564  Py and Supported
+000009c0: 2056 6572 7369 6f6e 730d 0a0d 0a50 7275   Versions....Pru
+000009d0: 7361 4c69 6e6b 5079 2069 7320 6176 6169  saLinkPy is avai
+000009e0: 6c61 626c 6520 6f6e 2070 6970 203a 0d0a  lable on pip :..
+000009f0: 0d0a 2020 2020 7079 7468 6f6e 202d 6d20  ..    python -m 
+00000a00: 7069 7020 696e 7374 616c 6c20 5072 7573  pip install Prus
+00000a10: 614c 696e 6b50 790d 0a0d 0a50 7275 7361  aLinkPy....Prusa
+00000a20: 4c69 6e6b 5079 206f 6666 6963 6961 6c6c  LinkPy officiall
+00000a30: 7920 7375 7070 6f72 7473 2050 7974 686f  y supports Pytho
+00000a40: 6e20 332e 392b 2077 6974 6820 5072 7573  n 3.9+ with Prus
+00000a50: 6120 7072 696e 7465 7273 2028 4d49 4e49  a printers (MINI
+00000a60: 2c20 4d4b 3420 6f72 2058 4c29 2066 6972  , MK4 or XL) fir
+00000a70: 6d77 6172 6520 352e 312e 302e 0d0a 0d0a  mware 5.1.0.....
+00000a80: 0d0a 2320 4150 4920 5265 6665 7265 6e63  ..# API Referenc
+00000a90: 650d 0a0d 0a23 2320 4c6f 7720 4c65 7665  e....## Low Leve
+00000aa0: 6c20 4675 6e63 7469 6f6e 730d 0a0d 0a5b  l Functions....[
+00000ab0: 6765 745f 7665 7273 696f 6e28 295d 2823  get_version()](#
+00000ac0: 7072 7573 616c 696e 6b70 7967 6574 5f76  prusalinkpyget_v
+00000ad0: 6572 7369 6f6e 290d 0a0d 0a5b 6765 745f  ersion)....[get_
+00000ae0: 7072 696e 7465 7228 295d 2823 7072 7573  printer()](#prus
+00000af0: 616c 696e 6b70 7967 6574 5f70 7269 6e74  alinkpyget_print
+00000b00: 6572 290d 0a0d 0a5b 6765 745f 6a6f 6228  er)....[get_job(
+00000b10: 295d 2823 7072 7573 616c 696e 6b70 7967  )](#prusalinkpyg
+00000b20: 6574 5f6a 6f62 290d 0a0d 0a5b 6765 745f  et_job)....[get_
+00000b30: 7374 6174 7573 2829 5d28 2370 7275 7361  status()](#prusa
+00000b40: 6c69 6e6b 7079 6765 745f 7374 6174 7573  linkpyget_status
+00000b50: 290d 0a0d 0a5b 6765 745f 7374 6f72 6167  )....[get_storag
+00000b60: 6528 295d 2823 7072 7573 616c 696e 6b70  e()](#prusalinkp
+00000b70: 7967 6574 5f73 746f 7261 6765 290d 0a0d  yget_storage)...
+00000b80: 0a5b 6765 745f 6669 6c65 7328 7265 6d6f  .[get_files(remo
+00000b90: 7465 4469 7229 5d28 2370 7275 7361 6c69  teDir)](#prusali
+00000ba0: 6e6b 7079 6765 745f 6669 6c65 732d 7265  nkpyget_files-re
+00000bb0: 6d6f 7465 6469 722d 2d29 0d0a 0d0a 5b64  motedir--)....[d
+00000bc0: 656c 6574 6528 7265 6d6f 7465 5061 7468  elete(remotePath
+00000bd0: 295d 2823 7072 7573 616c 696e 6b70 7964  )](#prusalinkpyd
+00000be0: 656c 6574 6572 656d 6f74 6570 6174 6829  eleteremotepath)
+00000bf0: 0d0a 0d0a 5b70 6f73 745f 6763 6f64 6528  ....[post_gcode(
+00000c00: 7265 6d6f 7465 5061 7468 295d 2823 7072  remotePath)](#pr
+00000c10: 7573 616c 696e 6b70 7970 7574 5f70 6f73  usalinkpyput_pos
+00000c20: 745f 6763 6f64 6529 0d0a 0d0a 5b70 7574  t_gcode)....[put
+00000c30: 5f67 636f 6465 2866 696c 6550 6174 684c  _gcode(filePathL
+00000c40: 6f63 616c 2c20 7265 6d6f 7465 4469 722c  ocal, remoteDir,
+00000c50: 2070 7269 6e74 4166 7465 7255 706c 6f61   printAfterUploa
+00000c60: 6420 3d20 4661 6c73 652c 206f 7665 7277  d = False, overw
+00000c70: 7269 7465 203d 2046 616c 7365 295d 2823  rite = False)](#
+00000c80: 7072 7573 616c 696e 6b70 7970 7574 5f67  prusalinkpyput_g
+00000c90: 636f 6465 7265 6d6f 7465 7061 7468 2d70  coderemotepath-p
+00000ca0: 7269 6e74 6166 7465 7275 706c 6f61 642d  rintafterupload-
+00000cb0: 2d66 616c 7365 2d6f 7665 7277 7269 7465  -false-overwrite
+00000cc0: 2d2d 6661 6c73 6529 0d0a 0d0a 5b65 7869  --false)....[exi
+00000cd0: 7374 735f 6763 6f64 6528 7265 6d6f 7465  sts_gcode(remote
+00000ce0: 5061 7468 295d 2823 7072 7573 616c 696e  Path)](#prusalin
+00000cf0: 6b70 7965 7869 7374 735f 6763 6f64 6572  kpyexists_gcoder
+00000d00: 656d 6f74 6570 6174 6829 0d0a 0d0a 5b70  emotepath)....[p
+00000d10: 6175 7365 5f70 7269 6e74 2829 5d28 2370  ause_print()](#p
+00000d20: 7275 7361 6c69 6e6b 7079 7061 7573 655f  rusalinkpypause_
+00000d30: 7072 696e 7429 0d0a 0d0a 5b72 6573 756d  print)....[resum
+00000d40: 655f 7072 696e 7428 295d 2823 7072 7573  e_print()](#prus
+00000d50: 616c 696e 6b70 7972 6573 756d 655f 7072  alinkpyresume_pr
+00000d60: 696e 7429 0d0a 0d0a 5b73 746f 705f 7072  int)....[stop_pr
+00000d70: 696e 7428 295d 2823 7072 7573 616c 696e  int()](#prusalin
+00000d80: 6b70 7973 746f 705f 7072 696e 7429 0d0a  kpystop_print)..
+00000d90: 0d0a 4e6f 7420 646f 6375 6d65 6e74 6564  ..Not documented
+00000da0: 203a 0d0a 202a 2067 6574 5f74 7261 6e73   :.. * get_trans
+00000db0: 6665 720d 0a20 2a20 6765 745f 7365 7474  fer.. * get_sett
+00000dc0: 696e 6773 0d0a 0d0a 466f 7220 636f 6d70  ings....For comp
+00000dd0: 6174 6962 696c 6974 7920 7769 7468 206f  atibility with o
+00000de0: 6c64 2076 6572 7369 6f6e 7320 3a0d 0a0d  ld versions :...
+00000df0: 0a5b 6465 6c65 7465 5f6a 6f62 2829 5d28  .[delete_job()](
+00000e00: 2370 7275 7361 6c69 6e6b 7079 6465 6c65  #prusalinkpydele
+00000e10: 7465 5f6a 6f62 290d 0a0d 0a23 2320 4869  te_job)....## Hi
+00000e20: 6768 204c 6576 656c 2046 756e 6374 696f  gh Level Functio
+00000e30: 6e73 200d 0a0d 0a5b 6765 745f 7265 6375  ns ....[get_recu
+00000e40: 7273 6976 655f 6669 6c65 7328 7265 6d6f  rsive_files(remo
+00000e50: 7465 4469 7229 5d28 2370 7275 7361 6c69  teDir)](#prusali
+00000e60: 6e6b 7079 6765 745f 7265 6375 7273 6976  nkpyget_recursiv
+00000e70: 655f 6669 6c65 732d 7265 6d6f 7465 6469  e_files-remotedi
+00000e80: 722d 2d29 0d0a 0d0a 0d0a 2320 5573 6572  r--)......# User
+00000e90: 2047 7569 6465 0d0a 0d0a 2323 2050 7275   Guide....## Pru
+00000ea0: 7361 4c69 6e6b 5079 2e67 6574 5f76 6572  saLinkPy.get_ver
+00000eb0: 7369 6f6e 2829 0d0a 0d0a 5265 6164 2076  sion()....Read v
+00000ec0: 6572 7369 6f6e 203a 0d0a 0d0a 0d0a 2020  ersion :......  
+00000ed0: 2020 696d 706f 7274 2050 7275 7361 4c69    import PrusaLi
+00000ee0: 6e6b 5079 0d0a 2020 2020 7072 7573 614d  nkPy..    prusaM
+00000ef0: 696e 6920 3d20 5072 7573 614c 696e 6b50  ini = PrusaLinkP
+00000f00: 792e 5072 7573 614c 696e 6b50 7928 2231  y.PrusaLinkPy("1
+00000f10: 3932 2e31 3638 2e30 2e31 3233 222c 2022  92.168.0.123", "
+00000f20: 386f 6a48 4b48 474e 7541 4841 3262 4d22  8ojHKHGNuAHA2bM"
+00000f30: 2c20 706f 7274 3d38 3031 3729 0d0a 2020  , port=8017)..  
+00000f40: 2020 6f62 6a20 3d20 7072 7573 614d 696e    obj = prusaMin
+00000f50: 692e 6765 745f 7665 7273 696f 6e28 290d  i.get_version().
+00000f60: 0a20 2020 206f 626a 2e6a 736f 6e28 290d  .    obj.json().
+00000f70: 0a20 2020 200d 0a52 6574 7572 6e20 736f  .    ..Return so
+00000f80: 6d65 7468 696e 6720 6c69 6b65 203a 0d0a  mething like :..
+00000f90: 0d0a 2020 2020 7b0d 0a20 2020 2020 2020  ..    {..       
+00000fa0: 2027 6170 6927 3a20 2732 2e30 2e30 272c   'api': '2.0.0',
+00000fb0: 200d 0a20 2020 2020 2020 2027 7365 7276   ..        'serv
+00000fc0: 6572 273a 2027 322e 312e 3227 2c20 0d0a  er': '2.1.2', ..
+00000fd0: 2020 2020 2020 2020 276e 6f7a 7a6c 655f          'nozzle_
+00000fe0: 6469 616d 6574 6572 273a 2030 2e34 2c20  diameter': 0.4, 
+00000ff0: 0d0a 2020 2020 2020 2020 2774 6578 7427  ..        'text'
+00001000: 3a20 2750 7275 7361 4c69 6e6b 272c 200d  : 'PrusaLink', .
+00001010: 0a20 2020 2020 2020 2027 686f 7374 6e61  .        'hostna
+00001020: 6d65 273a 2027 272c 200d 0a20 2020 2020  me': '', ..     
+00001030: 2020 2027 6361 7061 6269 6c69 7469 6573     'capabilities
+00001040: 273a 200d 0a20 2020 2020 2020 207b 0d0a  ': ..        {..
+00001050: 2020 2020 2020 2020 2020 2020 2775 706c              'upl
+00001060: 6f61 642d 6279 2d70 7574 273a 2054 7275  oad-by-put': Tru
+00001070: 650d 0a20 2020 2020 2020 207d 0d0a 2020  e..        }..  
+00001080: 2020 7d0d 0a0d 0a0d 0a23 2320 5072 7573    }......## Prus
+00001090: 614c 696e 6b50 792e 6765 745f 7072 696e  aLinkPy.get_prin
+000010a0: 7465 7228 290d 0a0d 0a47 6574 2070 7269  ter()....Get pri
+000010b0: 6e74 6572 203a 0d0a 0d0a 2020 2020 696d  nter :....    im
+000010c0: 706f 7274 2050 7275 7361 4c69 6e6b 5079  port PrusaLinkPy
+000010d0: 0d0a 2020 2020 7072 7573 614d 696e 6920  ..    prusaMini 
+000010e0: 3d20 5072 7573 614c 696e 6b50 792e 5072  = PrusaLinkPy.Pr
+000010f0: 7573 614c 696e 6b50 7928 2231 3932 2e31  usaLinkPy("192.1
+00001100: 3638 2e30 2e31 3233 222c 2022 386f 6a48  68.0.123", "8ojH
+00001110: 4b48 474e 7541 4841 3262 4d22 290d 0a20  KHGNuAHA2bM").. 
+00001120: 2020 206f 626a 203d 2070 7275 7361 4d69     obj = prusaMi
+00001130: 6e69 2e67 6574 5f70 7269 6e74 6572 2829  ni.get_printer()
+00001140: 0d0a 2020 2020 6f62 6a2e 6a73 6f6e 2829  ..    obj.json()
+00001150: 0d0a 2020 2020 0d0a 5761 6974 696e 6720  ..    ..Waiting 
+00001160: 666f 7220 4368 616e 6769 6e67 2046 696c  for Changing Fil
+00001170: 616d 656e 7420 3a0d 0a0d 0a20 2020 2027  ament :....    '
+00001180: 6c69 6e6b 5f73 7461 7465 273a 2027 4154  link_state': 'AT
+00001190: 5445 4e54 494f 4e27 200d 0a20 2020 2027  TENTION' ..    '
+000011a0: 6572 726f 7227 3a20 5472 7565 0d0a 2020  error': True..  
+000011b0: 2020 0d0a 5265 7475 726e 2073 6f6d 6574    ..Return somet
+000011c0: 6869 6e67 206c 696b 6520 3a0d 0a0d 0a20  hing like :.... 
+000011d0: 2020 207b 0d0a 2020 2020 2020 2020 2774     {..        't
+000011e0: 656c 656d 6574 7279 273a 200d 0a20 2020  elemetry': ..   
+000011f0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00001200: 2020 2020 2774 656d 702d 6265 6427 3a20      'temp-bed': 
+00001210: 3136 2e33 2c0d 0a20 2020 2020 2020 2020  16.3,..         
+00001220: 2020 2027 7465 6d70 2d6e 6f7a 7a6c 6527     'temp-nozzle'
+00001230: 3a20 3136 2e37 2c0d 0a20 2020 2020 2020  : 16.7,..       
+00001240: 2020 2020 2027 7072 696e 742d 7370 6565       'print-spee
+00001250: 6427 3a20 3130 302c 0d0a 2020 2020 2020  d': 100,..      
+00001260: 2020 2020 2020 277a 2d68 6569 6768 7427        'z-height'
+00001270: 3a20 3832 2e30 2c0d 0a20 2020 2020 2020  : 82.0,..       
+00001280: 2020 2020 2027 6d61 7465 7269 616c 273a       'material':
+00001290: 2027 504c 4127 0d0a 2020 2020 2020 2020   'PLA'..        
+000012a0: 7d2c 200d 0a20 2020 2020 2020 2027 7465  }, ..        'te
+000012b0: 6d70 6572 6174 7572 6527 3a20 0d0a 2020  mperature': ..  
+000012c0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+000012d0: 2020 2020 2027 746f 6f6c 3027 3a20 0d0a       'tool0': ..
+000012e0: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
+000012f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001300: 6163 7475 616c 273a 2031 362e 372c 0d0a  actual': 16.7,..
+00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001320: 2774 6172 6765 7427 3a20 302e 302c 0d0a  'target': 0.0,..
+00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001340: 2764 6973 706c 6179 273a 2030 2e30 2c0d  'display': 0.0,.
+00001350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001360: 2027 6f66 6673 6574 273a 2030 0d0a 2020   'offset': 0..  
+00001370: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
+00001380: 2020 2020 2020 2020 2020 2762 6564 273a            'bed':
+00001390: 200d 0a20 2020 2020 2020 2020 2020 207b   ..            {
+000013a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000013b0: 2020 2761 6374 7561 6c27 3a31 362e 332c    'actual':16.3,
+000013c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000013d0: 2020 2774 6172 6765 7427 3a20 302e 302c    'target': 0.0,
+000013e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000013f0: 2020 276f 6666 7365 7427 3a20 300d 0a20    'offset': 0.. 
+00001400: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00001410: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00001420: 2020 2773 7461 7465 273a 200d 0a20 2020    'state': ..   
+00001430: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00001440: 2020 2020 2774 6578 7427 3a20 274f 7065      'text': 'Ope
+00001450: 7261 7469 6f6e 616c 272c 0d0a 2020 2020  rational',..    
+00001460: 2020 2020 2020 2020 2766 6c61 6773 273a          'flags':
+00001470: 200d 0a20 2020 2020 2020 2020 2020 207b   ..            {
+00001480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001490: 2020 276f 7065 7261 7469 6f6e 616c 273a    'operational':
+000014a0: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
+000014b0: 2020 2020 2020 2020 2770 6175 7365 6427          'paused'
+000014c0: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
+000014d0: 2020 2020 2020 2020 2020 2770 7269 6e74            'print
+000014e0: 696e 6727 3a20 4661 6c73 652c 0d0a 2020  ing': False,..  
+000014f0: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+00001500: 616e 6365 6c6c 696e 6727 3a20 4661 6c73  ancelling': Fals
+00001510: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00001520: 2020 2020 2770 6175 7369 6e67 273a 2046      'pausing': F
+00001530: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00001540: 2020 2020 2020 2027 6572 726f 7227 3a20         'error': 
+00001550: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00001560: 2020 2020 2020 2020 2773 6452 6561 6479          'sdReady
+00001570: 273a 2046 616c 7365 2c0d 0a20 2020 2020  ': False,..     
+00001580: 2020 2020 2020 2020 2020 2027 636c 6f73             'clos
+00001590: 6564 4f6e 4572 726f 7227 3a20 4661 6c73  edOnError': Fals
+000015a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000015b0: 2020 2020 2772 6561 6479 273a 2054 7275      'ready': Tru
+000015c0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000015d0: 2020 2020 2762 7573 7927 3a20 4661 6c73      'busy': Fals
+000015e0: 650d 0a20 2020 2020 2020 2020 2020 207d  e..            }
+000015f0: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
+00001600: 207d 0d0a 0d0a 2323 2050 7275 7361 4c69   }....## PrusaLi
+00001610: 6e6b 5079 2e67 6574 5f6a 6f62 2829 0d0a  nkPy.get_job()..
+00001620: 0d0a 4765 7420 6a6f 6220 3a0d 0a0d 0a20  ..Get job :.... 
+00001630: 2020 2069 6d70 6f72 7420 5072 7573 614c     import PrusaL
+00001640: 696e 6b50 790d 0a20 2020 2070 7275 7361  inkPy..    prusa
+00001650: 4d69 6e69 203d 2050 7275 7361 4c69 6e6b  Mini = PrusaLink
+00001660: 5079 2e50 7275 7361 4c69 6e6b 5079 2822  Py.PrusaLinkPy("
+00001670: 3139 322e 3136 382e 302e 3132 3322 2c20  192.168.0.123", 
+00001680: 2238 6f6a 484b 4847 4e75 4148 4132 624d  "8ojHKHGNuAHA2bM
+00001690: 2229 0d0a 2020 2020 6f62 6a20 3d20 7072  ")..    obj = pr
+000016a0: 7573 614d 696e 692e 6765 745f 6a6f 6228  usaMini.get_job(
+000016b0: 290d 0a20 2020 206f 626a 2e6a 736f 6e28  )..    obj.json(
+000016c0: 290d 0a20 2020 200d 0a52 6574 7572 6e20  )..    ..Return 
+000016d0: 736f 6d65 7468 696e 6720 6c69 6b65 203a  something like :
+000016e0: 0d0a 0d0a 2020 2020 7b0d 0a20 2020 2020  ....    {..     
+000016f0: 2020 2022 7374 6174 6522 3a22 4f70 6572     "state":"Oper
+00001700: 6174 696f 6e61 6c22 2c0d 0a20 2020 2020  ational",..     
+00001710: 2020 2022 6a6f 6222 3a20 4e6f 6e65 2c0d     "job": None,.
+00001720: 0a20 2020 2020 2020 2022 7072 6f67 7265  .        "progre
+00001730: 7373 223a 204e 6f6e 650d 0a20 2020 207d  ss": None..    }
+00001740: 0d0a 2020 2020 0d0a 2323 2050 7275 7361  ..    ..## Prusa
+00001750: 4c69 6e6b 5079 2e64 656c 6574 655f 6a6f  LinkPy.delete_jo
+00001760: 6228 6a6f 6229 0d0a 0d0a 4465 6c65 7465  b(job)....Delete
+00001770: 2061 206a 6f62 2e20 4a6f 6220 6e75 6d62   a job. Job numb
+00001780: 6572 2069 7320 6176 6169 6c61 626c 6520  er is available 
+00001790: 7769 7468 2067 6574 5f6a 6f62 2829 206f  with get_job() o
+000017a0: 7220 6765 745f 7374 6174 7573 2829 0d0a  r get_status()..
+000017b0: 0d0a 2020 2020 696d 706f 7274 2050 7275  ..    import Pru
+000017c0: 7361 4c69 6e6b 5079 0d0a 2020 2020 7072  saLinkPy..    pr
+000017d0: 7573 614d 696e 6920 3d20 5072 7573 614c  usaMini = PrusaL
+000017e0: 696e 6b50 792e 5072 7573 614c 696e 6b50  inkPy.PrusaLinkP
+000017f0: 7928 2231 3932 2e31 3638 2e30 2e31 3233  y("192.168.0.123
+00001800: 222c 2022 386f 6a48 4b48 474e 7541 4841  ", "8ojHKHGNuAHA
+00001810: 3262 4d22 290d 0a20 2020 206f 626a 203d  2bM")..    obj =
+00001820: 2070 7275 7361 4d69 6e69 2e64 656c 6574   prusaMini.delet
+00001830: 655f 6a6f 6228 2234 3322 290d 0a20 2020  e_job("43")..   
+00001840: 200d 0a0d 0a23 2320 5072 7573 614c 696e   ....## PrusaLin
+00001850: 6b50 792e 6765 745f 7374 6174 7573 2829  kPy.get_status()
+00001860: 0d0a 0d0a 4765 7420 6a6f 6220 3a0d 0a0d  ....Get job :...
+00001870: 0a20 2020 2069 6d70 6f72 7420 5072 7573  .    import Prus
+00001880: 614c 696e 6b50 790d 0a20 2020 2070 7275  aLinkPy..    pru
+00001890: 7361 4d69 6e69 203d 2050 7275 7361 4c69  saMini = PrusaLi
+000018a0: 6e6b 5079 2e50 7275 7361 4c69 6e6b 5079  nkPy.PrusaLinkPy
+000018b0: 2822 3139 322e 3136 382e 302e 3132 3322  ("192.168.0.123"
+000018c0: 2c20 2238 6f6a 484b 4847 4e75 4148 4132  , "8ojHKHGNuAHA2
+000018d0: 624d 2229 0d0a 2020 2020 6f62 6a20 3d20  bM")..    obj = 
+000018e0: 7072 7573 614d 696e 692e 6765 745f 7374  prusaMini.get_st
+000018f0: 6174 7573 2829 0d0a 2020 2020 6f62 6a2e  atus()..    obj.
+00001900: 6a73 6f6e 2829 0d0a 2020 2020 0d0a 5661  json()..    ..Va
+00001910: 6c75 6520 6f66 2070 7269 6e74 6572 2d3e  lue of printer->
+00001920: 7374 6174 6520 3a0d 0a0d 0a20 2020 2049  state :....    I
+00001930: 444c 4520 284d 6169 6e20 5363 7265 656e  DLE (Main Screen
+00001940: 290d 0a20 2020 2050 5249 4e54 494e 470d  )..    PRINTING.
+00001950: 0a20 2020 2046 494e 4953 4845 4420 2850  .    FINISHED (P
+00001960: 7269 6e74 2066 696e 6973 682c 2073 6372  rint finish, scr
+00001970: 6565 6e20 6e6f 7420 6f6e 206d 6169 6e20  een not on main 
+00001980: 7363 7265 656e 290d 0a20 2020 2050 4155  screen)..    PAU
+00001990: 5345 4420 2850 6175 7365 2062 7920 7573  SED (Pause by us
+000019a0: 6572 2c20 5072 696e 7420 6661 6e20 6572  er, Print fan er
+000019b0: 726f 7229 0d0a 2020 2020 5354 4f50 5045  ror)..    STOPPE
+000019c0: 4420 2850 7269 6e74 2066 696e 6973 682c  D (Print finish,
+000019d0: 2073 746f 7070 6564 2062 7920 7573 6572   stopped by user
+000019e0: 290d 0a20 2020 2041 5454 454e 5449 4f4e  )..    ATTENTION
+000019f0: 2028 4669 6c61 6d65 6e74 2043 6861 6e67   (Filament Chang
+00001a00: 6529 0d0a 2020 2020 0d0a 5265 7475 726e  e)..    ..Return
+00001a10: 2073 6f6d 6574 6869 6e67 206c 696b 6520   something like 
+00001a20: 3a0d 0a0d 0a20 2020 207b 0d0a 2020 2020  :....    {..    
+00001a30: 2020 2020 226a 6f62 223a 0d0a 2020 2020      "job":..    
+00001a40: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+00001a50: 2020 2022 6964 223a 3433 2c0d 0a20 2020     "id":43,..   
+00001a60: 2020 2020 2020 2020 2022 7072 6f67 7265           "progre
+00001a70: 7373 223a 302e 3030 2c0d 0a20 2020 2020  ss":0.00,..     
+00001a80: 2020 2020 2020 2022 7469 6d65 5f72 656d         "time_rem
+00001a90: 6169 6e69 6e67 223a 3132 302c 0d0a 2020  aining":120,..  
+00001aa0: 2020 2020 2020 2020 2020 2274 696d 655f            "time_
+00001ab0: 7072 696e 7469 6e67 223a 3134 330d 0a20  printing":143.. 
+00001ac0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
+00001ad0: 2020 2022 7374 6f72 6167 6522 3a0d 0a20     "storage":.. 
+00001ae0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00001af0: 2020 2020 2020 2270 6174 6822 3a22 2f75        "path":"/u
+00001b00: 7362 2f22 2c0d 0a20 2020 2020 2020 2020  sb/",..         
+00001b10: 2020 2022 6e61 6d65 223a 2275 7362 222c     "name":"usb",
+00001b20: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
+00001b30: 6561 645f 6f6e 6c79 223a 6661 6c73 650d  ead_only":false.
+00001b40: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
+00001b50: 2020 2020 2022 7072 696e 7465 7222 3a0d       "printer":.
+00001b60: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
+00001b70: 2020 2020 2020 2020 2273 7461 7465 223a          "state":
+00001b80: 2250 5249 4e54 494e 4722 2c0d 0a20 2020  "PRINTING",..   
+00001b90: 2020 2020 2020 2020 2022 7465 6d70 5f62           "temp_b
+00001ba0: 6564 223a 3537 2e33 2c0d 0a20 2020 2020  ed":57.3,..     
+00001bb0: 2020 2020 2020 2022 7461 7267 6574 5f62         "target_b
+00001bc0: 6564 223a 302e 302c 0d0a 2020 2020 2020  ed":0.0,..      
+00001bd0: 2020 2020 2020 2274 656d 705f 6e6f 7a7a        "temp_nozz
+00001be0: 6c65 223a 3234 2e31 2c0d 0a20 2020 2020  le":24.1,..     
+00001bf0: 2020 2020 2020 2022 7461 7267 6574 5f6e         "target_n
+00001c00: 6f7a 7a6c 6522 3a30 2e30 2c0d 0a20 2020  ozzle":0.0,..   
+00001c10: 2020 2020 2020 2020 2022 6178 6973 5f7a           "axis_z
+00001c20: 223a 3136 322e 322c 0d0a 2020 2020 2020  ":162.2,..      
+00001c30: 2020 2020 2020 2266 6c6f 7722 3a31 3030        "flow":100
+00001c40: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00001c50: 7370 6565 6422 3a31 3030 2c0d 0a20 2020  speed":100,..   
+00001c60: 2020 2020 2020 2020 2022 6661 6e5f 686f           "fan_ho
+00001c70: 7465 6e64 223a 302c 0d0a 2020 2020 2020  tend":0,..      
+00001c80: 2020 2020 2020 2266 616e 5f70 7269 6e74        "fan_print
+00001c90: 223a 300d 0a20 2020 2020 2020 207d 0d0a  ":0..        }..
+00001ca0: 2020 2020 7d0d 0a20 2020 200d 0a23 2320      }..    ..## 
+00001cb0: 5072 7573 614c 696e 6b50 792e 6765 745f  PrusaLinkPy.get_
+00001cc0: 7374 6f72 6167 6528 290d 0a0d 0a47 6574  storage()....Get
+00001cd0: 206a 6f62 203a 0d0a 0d0a 2020 2020 696d   job :....    im
+00001ce0: 706f 7274 2050 7275 7361 4c69 6e6b 5079  port PrusaLinkPy
+00001cf0: 0d0a 2020 2020 7072 7573 614d 696e 6920  ..    prusaMini 
+00001d00: 3d20 5072 7573 614c 696e 6b50 792e 5072  = PrusaLinkPy.Pr
+00001d10: 7573 614c 696e 6b50 7928 2231 3932 2e31  usaLinkPy("192.1
+00001d20: 3638 2e30 2e31 3233 222c 2022 386f 6a48  68.0.123", "8ojH
+00001d30: 4b48 474e 7541 4841 3262 4d22 290d 0a20  KHGNuAHA2bM").. 
+00001d40: 2020 206f 626a 203d 2070 7275 7361 4d69     obj = prusaMi
+00001d50: 6e69 2e67 6574 5f73 746f 7261 6765 2829  ni.get_storage()
+00001d60: 0d0a 2020 2020 6f62 6a2e 6a73 6f6e 2829  ..    obj.json()
+00001d70: 0d0a 2020 2020 0d0a 5265 7475 726e 2073  ..    ..Return s
+00001d80: 6f6d 6574 6869 6e67 206c 696b 6520 3a0d  omething like :.
+00001d90: 0a0d 0a20 2020 207b 0d0a 2020 2020 2020  ...    {..      
+00001da0: 2020 2773 746f 7261 6765 5f6c 6973 7427    'storage_list'
+00001db0: 3a20 0d0a 2020 2020 2020 2020 5b0d 0a20  : ..        [.. 
+00001dc0: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+00001de0: 6174 6827 3a20 272f 7573 622f 272c 200d  ath': '/usb/', .
+00001df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e00: 2027 6e61 6d65 273a 2027 7573 6227 2c0d   'name': 'usb',.
+00001e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e20: 2027 7479 7065 273a 2027 5553 4227 2c20   'type': 'USB', 
+00001e30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001e40: 2020 2772 6561 645f 6f6e 6c79 273a 2046    'read_only': F
+00001e50: 616c 7365 2c20 0d0a 2020 2020 2020 2020  alse, ..        
+00001e60: 2020 2020 2020 2020 2761 7661 696c 6162          'availab
+00001e70: 6c65 273a 2054 7275 650d 0a20 2020 2020  le': True..     
+00001e80: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00001e90: 2020 5d0d 0a20 2020 207d 0d0a 2020 2020    ]..    }..    
+00001ea0: 0d0a 2323 2050 7275 7361 4c69 6e6b 5079  ..## PrusaLinkPy
+00001eb0: 2e67 6574 5f74 7261 6e73 6665 7228 290d  .get_transfer().
+00001ec0: 0a0d 0a4e 6f74 2054 6573 7465 640d 0a0d  ...Not Tested...
+00001ed0: 0a47 6574 206a 6f62 203a 0d0a 0d0a 2020  .Get job :....  
+00001ee0: 2020 696d 706f 7274 2050 7275 7361 4c69    import PrusaLi
+00001ef0: 6e6b 5079 0d0a 2020 2020 7072 7573 614d  nkPy..    prusaM
+00001f00: 696e 6920 3d20 5072 7573 614c 696e 6b50  ini = PrusaLinkP
+00001f10: 792e 5072 7573 614c 696e 6b50 7928 2231  y.PrusaLinkPy("1
+00001f20: 3932 2e31 3638 2e30 2e31 3233 222c 2022  92.168.0.123", "
+00001f30: 386f 6a48 4b48 474e 7541 4841 3262 4d22  8ojHKHGNuAHA2bM"
+00001f40: 290d 0a20 2020 206f 626a 203d 2070 7275  )..    obj = pru
+00001f50: 7361 4d69 6e69 2e67 6574 5f74 7261 6e73  saMini.get_trans
+00001f60: 6665 7228 290d 0a20 2020 206f 626a 2e74  fer()..    obj.t
+00001f70: 6578 740d 0a20 2020 200d 0a52 6574 7572  ext..    ..Retur
+00001f80: 6e20 736f 6d65 7468 696e 6720 6c69 6b65  n something like
+00001f90: 203a 0d0a 0d0a 2020 2020 544f 444f 0d0a   :....    TODO..
+00001fa0: 2020 2020 0d0a 2323 2050 7275 7361 4c69      ..## PrusaLi
+00001fb0: 6e6b 5079 2e67 6574 5f73 6574 7469 6e67  nkPy.get_setting
+00001fc0: 7328 290d 0a0d 0a43 6f6d 706c 6574 656c  s()....Completel
+00001fd0: 7920 7573 656c 6573 730d 0a0d 0a53 6565  y useless....See
+00001fe0: 2068 6572 6520 3a0d 0a0d 0a68 7474 7073   here :....https
+00001ff0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7072  ://github.com/pr
+00002000: 7573 6133 642f 5072 7573 612d 4669 726d  usa3d/Prusa-Firm
+00002010: 7761 7265 2d42 7564 6479 2f62 6c6f 622f  ware-Buddy/blob/
+00002020: 3462 6561 3932 3338 3130 3330 3264 3635  4bea923810302d65
+00002030: 3462 3933 3232 3931 6261 3332 3465 6165  4b932291ba324eae
+00002040: 6466 6630 3732 6663 2f6c 6962 2f57 5549  dff072fc/lib/WUI
+00002050: 2f6c 696e 6b5f 636f 6e74 656e 742f 7072  /link_content/pr
+00002060: 7573 615f 6c69 6e6b 5f61 7069 2e63 7070  usa_link_api.cpp
+00002070: 234c 3138 3143 3136 2d4c 3138 3143 3136  #L181C16-L181C16
+00002080: 0d0a 0d0a 436f 6d6d 656e 7420 6672 6f6d  ....Comment from
+00002090: 2050 7275 7361 2044 6576 656c 6f70 7065   Prusa Developpe
+000020a0: 7220 3a0d 0a0d 0a20 2020 2020 2f2f 2053  r :....     // S
+000020b0: 6f6d 6520 7374 7562 7320 666f 7220 6e6f  ome stubs for no
+000020c0: 772c 2074 6f20 6d61 6b65 206d 6f72 6520  w, to make more 
+000020d0: 636c 6965 6e74 7320 2869 6e63 6c75 6469  clients (includi
+000020e0: 6e67 2074 6865 2077 6562 2070 6167 6529  ng the web page)
+000020f0: 2068 6170 7069 6572 2e0d 0a0d 0a47 6574   happier.....Get
+00002100: 206a 6f62 203a 0d0a 0d0a 2020 2020 696d   job :....    im
+00002110: 706f 7274 2050 7275 7361 4c69 6e6b 5079  port PrusaLinkPy
+00002120: 0d0a 2020 2020 7072 7573 614d 696e 6920  ..    prusaMini 
+00002130: 3d20 5072 7573 614c 696e 6b50 792e 5072  = PrusaLinkPy.Pr
+00002140: 7573 614c 696e 6b50 7928 2231 3932 2e31  usaLinkPy("192.1
+00002150: 3638 2e30 2e31 3233 222c 2022 386f 6a48  68.0.123", "8ojH
+00002160: 4b48 474e 7541 4841 3262 4d22 290d 0a20  KHGNuAHA2bM").. 
+00002170: 2020 206f 626a 203d 2070 7275 7361 4d69     obj = prusaMi
+00002180: 6e69 2e67 6574 5f74 7261 6e73 6665 7228  ni.get_transfer(
+00002190: 290d 0a20 2020 206f 626a 2e74 6578 740d  )..    obj.text.
+000021a0: 0a20 2020 200d 0a52 6574 7572 6e20 736f  .    ..Return so
+000021b0: 6d65 7468 696e 6720 6c69 6b65 203a 0d0a  mething like :..
+000021c0: 0d0a 2020 2020 7b22 7072 696e 7465 7222  ..    {"printer"
+000021d0: 3a20 7b7d 7d0d 0a20 2020 200d 0a23 2320  : {}}..    ..## 
+000021e0: 5072 7573 614c 696e 6b50 792e 6765 745f  PrusaLinkPy.get_
+000021f0: 6669 6c65 7328 2072 656d 6f74 6544 6972  files( remoteDir
+00002200: 203d 2027 2f27 290d 0a0d 0a47 6574 2046   = '/')....Get F
+00002210: 696c 6573 206f 6e20 5553 4220 4472 6976  iles on USB Driv
+00002220: 6520 3a0d 0a0d 0a20 2020 2069 6d70 6f72  e :....    impor
+00002230: 7420 5072 7573 614c 696e 6b50 790d 0a20  t PrusaLinkPy.. 
+00002240: 2020 2070 7275 7361 4d69 6e69 203d 2050     prusaMini = P
+00002250: 7275 7361 4c69 6e6b 5079 2e50 7275 7361  rusaLinkPy.Prusa
+00002260: 4c69 6e6b 5079 2822 3139 322e 3136 382e  LinkPy("192.168.
+00002270: 302e 3132 3322 2c20 2238 6f6a 484b 4847  0.123", "8ojHKHG
+00002280: 4e75 4148 4132 624d 2229 0d0a 2020 2020  NuAHA2bM")..    
+00002290: 6f62 6a20 3d20 7072 7573 614d 696e 692e  obj = prusaMini.
+000022a0: 6765 745f 6669 6c65 7328 290d 0a20 2020  get_files()..   
+000022b0: 2066 696c 6573 5265 7420 3d20 6f62 6a2e   filesRet = obj.
+000022c0: 6a73 6f6e 2829 0d0a 2020 2020 0d0a 5265  json()..    ..Re
+000022d0: 7475 726e 2073 6f6d 6574 6869 6e67 206c  turn something l
+000022e0: 696b 6520 3a0d 0a0d 0a20 2020 207b 0d0a  ike :....    {..
+000022f0: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
+00002300: 2746 4f4c 4445 5227 2c20 0d0a 2020 2020  'FOLDER', ..    
+00002310: 2020 2020 2772 6f27 3a20 4661 6c73 652c      'ro': False,
+00002320: 200d 0a20 2020 2020 2020 2027 6e61 6d65   ..        'name
+00002330: 273a 2027 7573 6227 2c20 0d0a 2020 2020  ': 'usb', ..    
+00002340: 2020 2020 2763 6869 6c64 7265 6e27 3a20      'children': 
+00002350: 0d0a 2020 2020 2020 2020 5b0d 0a20 2020  ..        [..   
+00002360: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00002370: 2020 2020 276e 616d 6527 3a20 274d 544e      'name': 'MTN
+00002380: 272c 200d 0a20 2020 2020 2020 2020 2020  ', ..           
+00002390: 2027 726f 273a 2046 616c 7365 2c20 0d0a   'ro': False, ..
+000023a0: 2020 2020 2020 2020 2020 2020 2774 7970              'typ
+000023b0: 6527 3a20 2746 4f4c 4445 5227 2c20 0d0a  e': 'FOLDER', ..
+000023c0: 2020 2020 2020 2020 2020 2020 276d 5f74              'm_t
+000023d0: 696d 6573 7461 6d70 273a 2031 3730 3236  imestamp': 17026
+000023e0: 3238 3934 352c 200d 0a20 2020 2020 2020  28945, ..       
+000023f0: 2020 2020 2027 6469 7370 6c61 795f 6e61       'display_na
+00002400: 6d65 273a 2027 4d54 4e27 0d0a 2020 2020  me': 'MTN'..    
+00002410: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
+00002420: 7b0d 0a20 2020 2020 2020 2020 2020 2027  {..            '
+00002430: 6e61 6d65 273a 2027 5332 5f56 3249 5327  name': 'S2_V2IS'
+00002440: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00002450: 2772 6f27 3a20 4661 6c73 652c 200d 0a20  'ro': False, .. 
+00002460: 2020 2020 2020 2020 2020 2027 7479 7065             'type
+00002470: 273a 2027 464f 4c44 4552 272c 200d 0a20  ': 'FOLDER', .. 
+00002480: 2020 2020 2020 2020 2020 2027 6d5f 7469             'm_ti
+00002490: 6d65 7374 616d 7027 3a20 3137 3032 3536  mestamp': 170256
+000024a0: 3531 3832 2c20 0d0a 2020 2020 2020 2020  5182, ..        
+000024b0: 2020 2020 2764 6973 706c 6179 5f6e 616d      'display_nam
+000024c0: 6527 3a20 2753 325f 5632 4953 270d 0a20  e': 'S2_V2IS'.. 
+000024d0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+000024e0: 2020 5d0d 0a20 2020 207d 0d0a 2020 2020    ]..    }..    
+000024f0: 0d0a 576f 726b 616c 736f 2077 6974 6820  ..Workalso with 
+00002500: 7375 6266 6f6c 6465 720d 0a0d 0a20 2020  subfolder....   
+00002510: 206f 626a 203d 2070 7275 7361 4d69 6e69   obj = prusaMini
+00002520: 2e67 6574 5f66 696c 6573 2872 656d 6f74  .get_files(remot
+00002530: 6544 6972 203d 2027 2f53 5542 464f 4c44  eDir = '/SUBFOLD
+00002540: 4552 2729 0d0a 0d0a 2323 2050 7275 7361  ER')....## Prusa
+00002550: 4c69 6e6b 5079 2e67 6574 5f72 6563 7572  LinkPy.get_recur
+00002560: 7369 7665 5f66 696c 6573 2820 7265 6d6f  sive_files( remo
+00002570: 7465 4469 7220 3d20 272f 2729 0d0a 0d0a  teDir = '/')....
+00002580: 4765 7420 616c 6c20 6669 6c65 7320 286f  Get all files (o
+00002590: 6e6c 7920 6763 6f64 6520 616e 6420 6267  nly gcode and bg
+000025a0: 636f 6465 2920 696e 2061 2066 6f6c 6465  code) in a folde
+000025b0: 7220 616e 6420 7375 6266 6f6c 6465 722e  r and subfolder.
+000025c0: 0d0a 0d0a 5761 726e 696e 6720 3a20 7265  ....Warning : re
+000025d0: 7475 726e 206e 6573 7465 6420 6469 6374  turn nested dict
+000025e0: 2e0d 0a0d 0a0d 0a20 2020 2069 6d70 6f72  .......    impor
+000025f0: 7420 5072 7573 614c 696e 6b50 790d 0a20  t PrusaLinkPy.. 
+00002600: 2020 2070 7275 7361 4d69 6e69 203d 2050     prusaMini = P
+00002610: 7275 7361 4c69 6e6b 5079 2e50 7275 7361  rusaLinkPy.Prusa
+00002620: 4c69 6e6b 5079 2822 3139 322e 3136 382e  LinkPy("192.168.
+00002630: 302e 3132 3322 2c20 2238 6f6a 484b 4847  0.123", "8ojHKHG
+00002640: 4e75 4148 4132 624d 2229 0d0a 2020 2020  NuAHA2bM")..    
+00002650: 6469 6374 7420 3d20 7072 7573 614d 696e  dictt = prusaMin
+00002660: 692e 6765 745f 7265 6375 7273 6976 655f  i.get_recursive_
+00002670: 6669 6c65 7328 290d 0a20 2020 200d 0a20  files()..    .. 
+00002680: 2020 207b 0d0a 2020 2020 2020 2020 274d     {..        'M
+00002690: 544e 273a 200d 0a20 2020 2020 2020 207b  TN': ..        {
+000026a0: 0d0a 2020 2020 2020 2020 2020 2020 2743  ..            'C
+000026b0: 4847 545f 4255 5345 2e67 636f 6465 273a  HGT_BUSE.gcode':
+000026c0: 2027 2f4d 544e 2f43 4847 545f 427e 312e   '/MTN/CHGT_B~1.
+000026d0: 4743 4f27 2c20 0d0a 2020 2020 2020 2020  GCO', ..        
+000026e0: 2020 2020 2744 4542 4f55 4348 4147 452e      'DEBOUCHAGE.
+000026f0: 6763 6f64 6527 3a20 272f 4d54 4e2f 4445  gcode': '/MTN/DE
+00002700: 424f 5543 7e31 2e47 434f 272c 200d 0a20  BOUC~1.GCO', .. 
+00002710: 2020 2020 2020 2020 2020 2027 5052 4543             'PREC
+00002720: 4841 5546 4645 2e67 636f 6465 273a 2027  HAUFFE.gcode': '
+00002730: 2f4d 544e 2f50 5245 4348 417e 312e 4743  /MTN/PRECHA~1.GC
+00002740: 4f27 0d0a 2020 2020 2020 2020 7d2c 200d  O'..        }, .
+00002750: 0a20 2020 2020 2020 2027 5332 5f56 3249  .        'S2_V2I
+00002760: 5327 3a20 0d0a 2020 2020 2020 2020 7b0d  S': ..        {.
+00002770: 0a20 2020 2020 2020 2020 2020 2027 3268  .            '2h
+00002780: 3333 6d2e 6267 636f 6465 273a 2027 2f53  33m.bgcode': '/S
+00002790: 325f 5632 4953 2f32 4833 334d 7e31 2e42  2_V2IS/2H33M~1.B
+000027a0: 4743 272c 0d0a 2020 2020 2020 2020 2020  GC',..          
+000027b0: 2020 2735 6835 6d2e 6267 636f 6465 273a    '5h5m.bgcode':
+000027c0: 2027 2f53 325f 5632 4953 2f35 4835 4d7e   '/S2_V2IS/5H5M~
+000027d0: 312e 4247 4327 0d0a 2020 2020 2020 2020  1.BGC'..        
+000027e0: 7d0d 0a20 2020 207d 0d0a 0d0a 2323 2050  }..    }....## P
+000027f0: 7275 7361 4c69 6e6b 5079 2e64 656c 6574  rusaLinkPy.delet
+00002800: 6528 7265 6d6f 7465 5061 7468 2920 0d0a  e(remotePath) ..
+00002810: 0d0a 4465 6c65 7465 2061 2066 696c 6520  ..Delete a file 
+00002820: 6f72 2061 2066 6f6c 6465 7220 6f6e 2055  or a folder on U
+00002830: 5342 2064 7269 7665 0d0a 0d0a 2020 2020  SB drive....    
+00002840: 696d 706f 7274 2050 7275 7361 4c69 6e6b  import PrusaLink
+00002850: 5079 0d0a 2020 2020 7072 7573 614d 696e  Py..    prusaMin
+00002860: 6920 3d20 5072 7573 614c 696e 6b50 792e  i = PrusaLinkPy.
+00002870: 5072 7573 614c 696e 6b50 7928 2231 3932  PrusaLinkPy("192
+00002880: 2e31 3638 2e30 2e31 3233 222c 2022 386f  .168.0.123", "8o
+00002890: 6a48 4b48 474e 7541 4841 3262 4d22 290d  jHKHGNuAHA2bM").
+000028a0: 0a20 2020 206f 626a 203d 2070 7275 7361  .    obj = prusa
+000028b0: 4d69 6e69 2e64 656c 6574 6528 272f 4445  Mini.delete('/DE
+000028c0: 424f 5543 7e31 2e47 434f 2729 0d0a 0d0a  BOUC~1.GCO')....
+000028d0: 0d0a 2323 2050 7275 7361 4c69 6e6b 5079  ..## PrusaLinkPy
+000028e0: 2e70 6f73 745f 6763 6f64 6528 7265 6d6f  .post_gcode(remo
+000028f0: 7465 5061 7468 2920 0d0a 0d0a 5072 696e  tePath) ....Prin
+00002900: 7420 6120 6669 6c65 2061 6c72 6561 6479  t a file already
+00002910: 2070 6f72 6573 656e 7420 6f6e 2055 5342   poresent on USB
+00002920: 206b 6579 200d 0a0d 0a20 2020 2069 6d70   key ....    imp
+00002930: 6f72 7420 5072 7573 614c 696e 6b50 790d  ort PrusaLinkPy.
+00002940: 0a20 2020 2070 7275 7361 4d69 6e69 203d  .    prusaMini =
+00002950: 2050 7275 7361 4c69 6e6b 5079 2e50 7275   PrusaLinkPy.Pru
+00002960: 7361 4c69 6e6b 5079 2822 3139 322e 3136  saLinkPy("192.16
+00002970: 382e 302e 3132 3322 2c20 2238 6f6a 484b  8.0.123", "8ojHK
+00002980: 4847 4e75 4148 4132 624d 2229 0d0a 2020  HGNuAHA2bM")..  
+00002990: 2020 6f62 6a20 3d20 7072 7573 614d 696e    obj = prusaMin
+000029a0: 692e 706f 7374 5f67 636f 6465 2827 2f44  i.post_gcode('/D
+000029b0: 4542 4f55 437e 312e 4743 4f27 290d 0a0d  EBOUC~1.GCO')...
+000029c0: 0a23 2320 5072 7573 614c 696e 6b50 792e  .## PrusaLinkPy.
+000029d0: 7075 745f 6763 6f64 6528 7265 6d6f 7465  put_gcode(remote
+000029e0: 5061 7468 2c20 7072 696e 7441 6674 6572  Path, printAfter
+000029f0: 5570 6c6f 6164 203d 2046 616c 7365 2c20  Upload = False, 
+00002a00: 6f76 6572 7772 6974 6520 3d20 4661 6c73  overwrite = Fals
+00002a10: 6529 200d 0a0d 0a53 656e 6420 6120 6669  e) ....Send a fi
+00002a20: 6c65 206f 6e20 5553 4220 4472 6976 652e  le on USB Drive.
+00002a30: 0d0a 0d0a 4361 6e20 6372 6561 7465 2061  ....Can create a
+00002a40: 2066 6f6c 6465 7220 210d 0a0d 0a69 6620   folder !....if 
+00002a50: 7265 742e 7374 6174 7573 5f63 6f64 6520  ret.status_code 
+00002a60: 3d20 3430 3920 2d3e 2043 6f6e 666c 6963  = 409 -> Conflic
+00002a70: 7420 3a20 4669 6c65 2061 6c72 6561 6479  t : File already
+00002a80: 2065 7869 7374 730d 0a69 6620 7265 742e   exists..if ret.
+00002a90: 7374 6174 7573 5f63 6f64 6520 3d20 3431  status_code = 41
+00002aa0: 3520 2d3e 207b 2274 6974 6c65 223a 2022  5 -> {"title": "
+00002ab0: 3431 353a 2055 6e73 7570 706f 7274 6564  415: Unsupported
+00002ac0: 204d 6564 6961 2054 7970 6522 2c22 6d65   Media Type","me
+00002ad0: 7373 6167 6522 3a22 4e6f 7420 6120 4743  ssage":"Not a GC
+00002ae0: 4f44 4522 7d0d 0a0d 0a70 7269 6e74 4166  ODE"}....printAf
+00002af0: 7465 7255 706c 6f61 6420 3a20 5365 7420  terUpload : Set 
+00002b00: 6174 2054 7275 6520 746f 2070 7269 6e74  at True to print
+00002b10: 2061 6674 6572 2075 706c 6f61 642e 200d   after upload. .
+00002b20: 0a0d 0a6f 7665 7277 7269 7465 203a 2041  ...overwrite : A
+00002b30: 6c6c 6f77 2066 696c 6520 4f76 6572 7772  llow file Overwr
+00002b40: 6974 650d 0a0d 0a46 5720 352e 312e 3020  ite....FW 5.1.0 
+00002b50: 3a0d 0a0d 0a20 2a20 5761 726e 696e 673a  :.... * Warning:
+00002b60: 2070 7269 6e74 696e 6720 7374 6172 7473   printing starts
+00002b70: 2065 7665 6e20 6966 2074 6865 2062 6564   even if the bed
+00002b80: 2069 7320 6e6f 7420 656d 7074 790d 0a20   is not empty.. 
+00002b90: 2a20 4361 6e20 6f6e 6c79 2073 656e 6420  * Can only send 
+00002ba0: 6267 636f 6465 2061 6e64 2067 636f 6465  bgcode and gcode
+00002bb0: 0d0a 2020 2020 0d0a 0d0a 2020 2020 696d  ..    ....    im
+00002bc0: 706f 7274 2050 7275 7361 4c69 6e6b 5079  port PrusaLinkPy
+00002bd0: 0d0a 2020 2020 7072 7573 614d 696e 6920  ..    prusaMini 
+00002be0: 3d20 5072 7573 614c 696e 6b50 792e 5072  = PrusaLinkPy.Pr
+00002bf0: 7573 614c 696e 6b50 7928 2231 3932 2e31  usaLinkPy("192.1
+00002c00: 3638 2e30 2e31 3233 222c 2022 386f 6a48  68.0.123", "8ojH
+00002c10: 4b48 474e 7541 4841 3262 4d22 290d 0a20  KHGNuAHA2bM").. 
+00002c20: 2020 2073 7461 7475 7320 3d20 7072 7573     status = prus
+00002c30: 614d 696e 692e 7075 7428 2743 3a2f 4d54  aMini.put('C:/MT
+00002c40: 4e2f 4445 424f 5543 4841 4745 2e67 636f  N/DEBOUCHAGE.gco
+00002c50: 6465 2720 2c20 274d 544e 2f44 4542 4f55  de' , 'MTN/DEBOU
+00002c60: 4348 4147 452e 6763 6f64 6527 290d 0a20  CHAGE.gcode').. 
+00002c70: 2020 2023 204f 7665 7277 7269 7465 0d0a     # Overwrite..
+00002c80: 2020 2020 7374 6174 7573 203d 2070 7275      status = pru
+00002c90: 7361 4d69 6e69 2e70 7574 2827 433a 2f4d  saMini.put('C:/M
+00002ca0: 544e 2f44 4542 4f55 4348 4147 452e 6763  TN/DEBOUCHAGE.gc
+00002cb0: 6f64 6527 202c 2027 4d54 4e2f 4445 424f  ode' , 'MTN/DEBO
+00002cc0: 5543 4841 4745 2e67 636f 6465 272c 2046  UCHAGE.gcode', F
+00002cd0: 616c 7365 2c20 5472 7565 290d 0a20 2020  alse, True)..   
+00002ce0: 2023 204f 7665 7277 7269 7465 2061 6e64   # Overwrite and
+00002cf0: 2050 7269 6e74 0d0a 2020 2020 7374 6174   Print..    stat
+00002d00: 7573 203d 2070 7275 7361 4d69 6e69 2e70  us = prusaMini.p
+00002d10: 7574 2827 433a 2f4d 544e 2f44 4542 4f55  ut('C:/MTN/DEBOU
+00002d20: 4348 4147 452e 6763 6f64 6527 202c 2027  CHAGE.gcode' , '
+00002d30: 4d54 4e2f 4445 424f 5543 4841 4745 2e67  MTN/DEBOUCHAGE.g
+00002d40: 636f 6465 272c 2054 7275 652c 2054 7275  code', True, Tru
+00002d50: 6529 0d0a 2020 2020 0d0a 2323 2050 7275  e)..    ..## Pru
+00002d60: 7361 4c69 6e6b 5079 2e65 7869 7374 735f  saLinkPy.exists_
+00002d70: 6763 6f64 6528 7265 6d6f 7465 5061 7468  gcode(remotePath
+00002d80: 2920 0d0a 0d0a 4368 6563 6b20 6966 2061  ) ....Check if a
+00002d90: 2066 696c 6520 6578 6973 7473 206f 6e20   file exists on 
+00002da0: 5553 4220 6472 6976 652e 200d 0a0d 0a52  USB drive. ....R
+00002db0: 6574 7572 6e20 5472 7565 206f 7220 4661  eturn True or Fa
+00002dc0: 6c73 650d 0a0d 0a20 2020 2069 6d70 6f72  lse....    impor
+00002dd0: 7420 5072 7573 614c 696e 6b50 790d 0a20  t PrusaLinkPy.. 
+00002de0: 2020 2070 7275 7361 4d69 6e69 203d 2050     prusaMini = P
+00002df0: 7275 7361 4c69 6e6b 5079 2e50 7275 7361  rusaLinkPy.Prusa
+00002e00: 4c69 6e6b 5079 2822 3139 322e 3136 382e  LinkPy("192.168.
+00002e10: 302e 3132 3322 2c20 2238 6f6a 484b 4847  0.123", "8ojHKHG
+00002e20: 4e75 4148 4132 624d 2229 0d0a 2020 2020  NuAHA2bM")..    
+00002e30: 7374 6174 7573 203d 2070 7275 7361 4d69  status = prusaMi
+00002e40: 6e69 2e65 7869 7374 735f 6763 6f64 6528  ni.exists_gcode(
+00002e50: 272f 4445 424f 5543 7e31 2e47 434f 2729  '/DEBOUC~1.GCO')
+00002e60: 0d0a 0d0a 2323 2050 7275 7361 4c69 6e6b  ....## PrusaLink
+00002e70: 5079 2e70 6175 7365 5f70 7269 6e74 2829  Py.pause_print()
+00002e80: 200d 0a0d 0a50 6175 7365 2061 6374 7561   ....Pause actua
+00002e90: 6c20 7072 696e 742e 0d0a 0d0a 4164 6465  l print.....Adde
+00002ea0: 6420 696e 2032 2e32 2e30 202e 0d0a 0d0a  d in 2.2.0 .....
+00002eb0: 2323 2050 7275 7361 4c69 6e6b 5079 2e72  ## PrusaLinkPy.r
+00002ec0: 6573 756d 655f 7072 696e 7428 2920 0d0a  esume_print() ..
+00002ed0: 0d0a 5265 7375 6d65 2070 6175 7365 6420  ..Resume paused 
+00002ee0: 7072 696e 742e 0d0a 0d0a 4164 6465 6420  print.....Added 
+00002ef0: 696e 2032 2e32 2e30 202e 0d0a 0d0a 2323  in 2.2.0 .....##
+00002f00: 2050 7275 7361 4c69 6e6b 5079 2e73 746f   PrusaLinkPy.sto
+00002f10: 705f 7072 696e 7428 2920 0d0a 0d0a 5374  p_print() ....St
+00002f20: 6f70 2061 6374 7561 6c20 7072 696e 742e  op actual print.
+00002f30: 0d0a 0d0a 4164 6465 6420 696e 2032 2e32  ....Added in 2.2
+00002f40: 2e30 202e 0d0a 0d0a 2320 4150 490d 0a0d  .0 .....# API...
+00002f50: 0a41 5049 206e 6f74 2069 6d70 6c65 6d65  .API not impleme
+00002f60: 6e74 6564 2069 6e20 6d79 206c 6962 2020  nted in my lib  
+00002f70: 3a20 0d0a 0d0a 202a 2072 6574 7269 6576  : .... * retriev
+00002f80: 6520 7468 756d 626e 6169 6c20 3a0d 0a0d  e thumbnail :...
+00002f90: 0a20 2020 2072 203d 2072 6571 7565 7374  .    r = request
+00002fa0: 732e 6765 7428 2768 7474 703a 2f2f 3139  s.get('http://19
+00002fb0: 322e 3136 382e 302e 3132 333a 3830 3137  2.168.0.123:8017
+00002fc0: 2f74 6875 6d62 2f6c 2f75 7362 2f54 4156  /thumb/l/usb/TAV
+00002fd0: 4552 4e7e 312e 4743 4f27 2c20 6865 6164  ERN~1.GCO', head
+00002fe0: 6572 733d 6865 6164 6572 7329 0d0a 0d0a  ers=headers)....
+00002ff0: 2f61 7069 2f73 6574 7469 6e67 730d 0a0d  /api/settings...
+00003000: 0a0d 0a50 4f53 5420 2f61 7069 2f6a 6f62  ...POST /api/job
+00003010: 0d0a 2a2a 5b4c 696e 6b20 746f 2042 7564  ..**[Link to Bud
+00003020: 6479 2063 6f64 655d 2868 7474 7073 3a2f  dy code](https:/
+00003030: 2f67 6974 6875 622e 636f 6d2f 7072 7573  /github.com/prus
+00003040: 6133 642f 5072 7573 612d 4669 726d 7761  a3d/Prusa-Firmwa
+00003050: 7265 2d42 7564 6479 2f62 6c6f 622f 6d61  re-Buddy/blob/ma
+00003060: 7374 6572 2f6c 6962 2f57 5549 2f6c 696e  ster/lib/WUI/lin
+00003070: 6b5f 636f 6e74 656e 742f 7072 7573 615f  k_content/prusa_
+00003080: 6c69 6e6b 5f61 7069 2e63 7070 234c 3237  link_api.cpp#L27
+00003090: 3629 2a2a 0d0a 0d0a 4745 542f 504f 5354  6)**....GET/POST
+000030a0: 202f 6170 692f 646f 776e 6c6f 6164 200d   /api/download .
+000030b0: 0a2a 2a5b 4c69 6e6b 2074 6f20 4275 6464  .**[Link to Budd
+000030c0: 7920 636f 6465 5d28 6874 7470 733a 2f2f  y code](https://
+000030d0: 6769 7468 7562 2e63 6f6d 2f70 7275 7361  github.com/prusa
+000030e0: 3364 2f50 7275 7361 2d46 6972 6d77 6172  3d/Prusa-Firmwar
+000030f0: 652d 4275 6464 792f 626c 6f62 2f6d 6173  e-Buddy/blob/mas
+00003100: 7465 722f 6c69 622f 5755 492f 6c69 6e6b  ter/lib/WUI/link
+00003110: 5f63 6f6e 7465 6e74 2f70 7275 7361 5f6c  _content/prusa_l
+00003120: 696e 6b5f 6170 692e 6370 7023 4c32 3839  ink_api.cpp#L289
+00003130: 292a 2a0d 0a0d 0a0d 0a23 2020 4275 6773  )**......#  Bugs
+00003140: 2070 7265 7365 6e74 2069 6e20 5072 7573   present in Prus
+00003150: 6120 4d49 4e49 2070 7269 6e74 6572 2066  a MINI printer f
+00003160: 6972 6d77 6172 6520 342e 342e 313a 0d0a  irmware 4.4.1:..
+00003170: 0d0a 202a 2054 6865 7265 2069 7320 6e6f  .. * There is no
+00003180: 2070 6f73 7369 6269 6c69 7479 2074 6f20   possibility to 
+00003190: 6861 7665 2074 6865 206c 6973 7420 6f66  have the list of
+000031a0: 2066 6f6c 6465 7273 2070 7265 7365 6e74   folders present
+000031b0: 2069 6e20 6120 6469 7265 6374 6f72 790d   in a directory.
+000031c0: 0a20 2020 202a 2053 6f6c 7665 6420 696e  .    * Solved in
+000031d0: 2066 6972 6d77 6172 6520 350d 0a20 2a20   firmware 5.. * 
+000031e0: 596f 7520 6361 6e6e 6f74 2075 706c 6f61  You cannot uploa
+000031f0: 6420 6120 6763 6f64 6520 696e 2061 2073  d a gcode in a s
+00003200: 7562 666f 6c64 6572 206f 6620 7468 6520  ubfolder of the 
+00003210: 5553 4220 6b65 790d 0a20 2020 202a 2053  USB key..    * S
+00003220: 6f6c 7665 6420 696e 2066 6972 6d77 6172  olved in firmwar
+00003230: 6520 350d 0a20 2a20 5768 656e 2074 6865  e 5.. * When the
+00003240: 2070 7269 6e74 6572 2064 6574 6563 7473   printer detects
+00003250: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
+00003260: 6669 6c61 6d65 6e74 2061 6e64 2069 7420  filament and it 
+00003270: 6469 7370 6c61 7973 2022 4368 616e 6765  displays "Change
+00003280: 2046 696c 616d 656e 7422 2074 6865 2074   Filament" the t
+00003290: 656c 656d 6574 7279 2069 6e66 6f72 6d61  elemetry informa
+000032a0: 7469 6f6e 2069 7320 6e6f 206c 6f6e 6765  tion is no longe
+000032b0: 7220 676f 6f64 2e20 4865 7265 2069 7320  r good. Here is 
+000032c0: 7468 6520 696e 666f 726d 6174 696f 6e20  the information 
+000032d0: 7265 7475 726e 6564 2062 7920 7468 6520  returned by the 
+000032e0: 7072 696e 7465 7220 696e 2074 6869 7320  printer in this 
+000032f0: 6361 7365 3a0d 0a20 0d0a 2020 2020 2774  case:.. ..    't
+00003300: 656c 656d 6574 7279 273a 207b 2774 656d  elemetry': {'tem
+00003310: 702d 6265 6427 3a20 302e 302c 2027 7465  p-bed': 0.0, 'te
+00003320: 6d70 2d6e 6f7a 7a6c 6527 3a20 302e 302c  mp-nozzle': 0.0,
+00003330: 2027 7072 696e 742d 7370 6565 6427 3a20   'print-speed': 
+00003340: 3130 302c 2027 7a2d 6865 6967 6874 273a  100, 'z-height':
+00003350: 2030 2e30 2c20 276d 6174 6572 6961 6c27   0.0, 'material'
+00003360: 3a20 272d 2d2d 277d 0d0a 2020 2020 0d0a  : '---'}..    ..
+00003370: 202a 2053 7469 6c6c 2069 6e20 7468 6520   * Still in the 
+00003380: 6361 7365 206f 6620 6120 6669 6c61 6d65  case of a filame
+00003390: 6e74 2063 6861 6e67 652c 2074 6865 2073  nt change, the s
+000033a0: 7461 7475 7320 696e 666f 726d 6174 696f  tatus informatio
+000033b0: 6e20 6973 2069 6e63 6f72 7265 6374 3a0d  n is incorrect:.
+000033c0: 0a0d 0a20 2020 2027 7374 6174 6527 3a20  ...    'state': 
+000033d0: 7b27 7465 7874 273a 2027 4f70 6572 6174  {'text': 'Operat
+000033e0: 696f 6e61 6c27 2c20 2766 6c61 6773 273a  ional', 'flags':
+000033f0: 207b 276f 7065 7261 7469 6f6e 616c 273a   {'operational':
+00003400: 2054 7275 652c 2027 7061 7573 6564 273a   True, 'paused':
+00003410: 2046 616c 7365 2c20 2770 7269 6e74 696e   False, 'printin
+00003420: 6727 3a20 4661 6c73 652c 2027 6361 6e63  g': False, 'canc
+00003430: 656c 6c69 6e67 273a 2046 616c 7365 2c20  elling': False, 
+00003440: 2770 6175 7369 6e67 273a 2046 616c 7365  'pausing': False
+00003450: 2c20 2773 6452 6561 6479 273a 2046 616c  , 'sdReady': Fal
+00003460: 7365 2c20 2765 7272 6f72 273a 2046 616c  se, 'error': Fal
+00003470: 7365 2c20 2763 6c6f 7365 644f 6e45 7272  se, 'closedOnErr
+00003480: 6f72 273a 2046 616c 7365 2c20 2772 6561  or': False, 'rea
+00003490: 6479 273a 2054 7275 652c 2027 6275 7379  dy': True, 'busy
+000034a0: 273a 2046 616c 7365 7d0d 0a0d 0a0d 0a23  ': False}......#
+000034b0: 2049 6e73 7069 7261 7469 6f6e 0d0a 0d0a   Inspiration....
+000034c0: 416e 206f 7468 6572 206c 6962 203a 200d  An other lib : .
+000034d0: 0a0d 0a68 7474 7073 3a2f 2f67 6974 6875  ...https://githu
+000034e0: 622e 636f 6d2f 686f 6d65 2d61 7373 6973  b.com/home-assis
+000034f0: 7461 6e74 2d6c 6962 732f 5072 7573 614c  tant-libs/PrusaL
+00003500: 696e 6b50 792f 626c 6f62 2f6d 6169 6e2f  inkPy/blob/main/
+00003510: 5072 7573 614c 696e 6b50 792f 0d0a 0d0a  PrusaLinkPy/....
+00003520: 0d0a 4c65 7320 636f 6d6d 616e 6465 7320  ..Les commandes 
+00003530: 6461 6e73 206c 6120 6d69 6e69 203a 0d0a  dans la mini :..
+00003540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003550: 6f6d 2f70 7275 7361 3364 2f50 7275 7361  om/prusa3d/Prusa
+00003560: 2d46 6972 6d77 6172 652d 4275 6464 792f  -Firmware-Buddy/
+00003570: 626c 6f62 2f6d 6173 7465 722f 6c69 622f  blob/master/lib/
+00003580: 5755 492f 6c69 6e6b 5f63 6f6e 7465 6e74  WUI/link_content
+00003590: 2f62 6173 6963 5f67 6574 732e 6370 700d  /basic_gets.cpp.
+000035a0: 0a0d 0a0d 0a0d 0a23 2043 6f6e 7374 7275  .......# Constru
+000035b0: 6972 6520 6c61 206c 6962 0d0a 0d0a 2020  ire la lib....  
+000035c0: 2020 7079 202d 6d20 6275 696c 640d 0a0d    py -m build...
+000035d0: 0a54 6f20 7570 6c6f 6164 2074 6f20 7465  .To upload to te
+000035e0: 7374 7069 2072 6570 6f20 3a0d 0a0d 0a20  stpi repo :.... 
+000035f0: 2020 2070 7920 2d6d 2074 7769 6e65 2075     py -m twine u
+00003600: 706c 6f61 6420 2d2d 7265 706f 7369 746f  pload --reposito
+00003610: 7279 2074 6573 7470 6920 6469 7374 2f2a  ry testpi dist/*
+00003620: 0d0a 0d0a 546f 2075 706c 6f61 6420 746f  ....To upload to
+00003630: 2070 7970 6920 7265 706f 203a 0d0a 0d0a   pypi repo :....
+00003640: 2020 2020 7079 202d 6d20 7477 696e 6520      py -m twine 
+00003650: 7570 6c6f 6164 2064 6973 742f 2a0d 0a0d  upload dist/*...
+00003660: 0a0d 0a68 7474 7073 3a2f 2f6d 6564 6975  ...https://mediu
+00003670: 6d2e 636f 6d2f 616e 616c 7974 6963 732d  m.com/analytics-
+00003680: 7669 6468 7961 2f68 6f77 2d74 6f2d 6372  vidhya/how-to-cr
+00003690: 6561 7465 2d61 2d70 7974 686f 6e2d 6c69  eate-a-python-li
+000036a0: 6272 6172 792d 3764 3561 6561 3830 6363  brary-7d5aea80cc
+000036b0: 3366 0d0a 0d0a                           3f....
```

### Comparing `prusalinkpy-2.2.0/pyproject.toml` & `prusalinkpy-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PrusaLinkPy"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
   { name="Guillaume RICO", email="guillaume.rico@alpesmesures.fr" },
 ]
 description = "A library to interface with the PrusaLink API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

