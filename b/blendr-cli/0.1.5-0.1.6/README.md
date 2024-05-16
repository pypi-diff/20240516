# Comparing `tmp/blendr_cli-0.1.5.tar.gz` & `tmp/blendr_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendr_cli-0.1.5.tar", last modified: Wed May  1 12:57:29 2024, max compression
+gzip compressed data, was "blendr_cli-0.1.6.tar", last modified: Thu May 16 11:58:10 2024, max compression
```

## Comparing `blendr_cli-0.1.5.tar` & `blendr_cli-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,48 @@
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-01 12:57:29.277717 blendr_cli-0.1.5/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3239 2024-05-01 12:57:29.277467 blendr_cli-0.1.5/PKG-INFO
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2677 2024-04-29 20:20:22.000000 blendr_cli-0.1.5/README.md
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-01 12:57:29.274339 blendr_cli-0.1.5/blendr/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-20 16:49:51.000000 blendr_cli-0.1.5/blendr/__init__.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-01 12:57:29.274731 blendr_cli-0.1.5/blendr/auth/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:43.000000 blendr_cli-0.1.5/blendr/auth/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     1923 2024-04-30 07:06:02.000000 blendr_cli-0.1.5/blendr/auth/authenticate.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     1917 2024-04-30 07:02:44.000000 blendr_cli-0.1.5/blendr/cli.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-01 12:57:29.275362 blendr_cli-0.1.5/blendr/config/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:41.000000 blendr_cli-0.1.5/blendr/config/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      158 2024-04-30 13:58:05.000000 blendr_cli-0.1.5/blendr/config/settings.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     6119 2024-04-30 14:25:22.000000 blendr_cli-0.1.5/blendr/config/setup.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-01 12:57:29.275860 blendr_cli-0.1.5/blendr/gpu_manager/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:38.000000 blendr_cli-0.1.5/blendr/gpu_manager/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      190 2024-04-29 20:05:17.000000 blendr_cli-0.1.5/blendr/gpu_manager/detect.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-01 12:57:29.276225 blendr_cli-0.1.5/blendr/task_manager/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:33.000000 blendr_cli-0.1.5/blendr/task_manager/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2245 2024-04-29 20:05:25.000000 blendr_cli-0.1.5/blendr/task_manager/listen.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-01 12:57:29.277197 blendr_cli-0.1.5/blendr_cli.egg-info/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3239 2024-05-01 12:57:29.000000 blendr_cli-0.1.5/blendr_cli.egg-info/PKG-INFO
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      506 2024-05-01 12:57:29.000000 blendr_cli-0.1.5/blendr_cli.egg-info/SOURCES.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        1 2024-05-01 12:57:29.000000 blendr_cli-0.1.5/blendr_cli.egg-info/dependency_links.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       43 2024-05-01 12:57:29.000000 blendr_cli-0.1.5/blendr_cli.egg-info/entry_points.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      161 2024-05-01 12:57:29.000000 blendr_cli-0.1.5/blendr_cli.egg-info/requires.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        7 2024-05-01 12:57:29.000000 blendr_cli-0.1.5/blendr_cli.egg-info/top_level.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       38 2024-05-01 12:57:29.277765 blendr_cli-0.1.5/setup.cfg
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      913 2024-05-01 12:57:21.000000 blendr_cli-0.1.5/setup.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.958085 blendr_cli-0.1.6/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3271 2024-05-16 11:58:10.957862 blendr_cli-0.1.6/PKG-INFO
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     2677 2024-04-29 20:20:22.000000 blendr_cli-0.1.6/README.md
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.952923 blendr_cli-0.1.6/blendr/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-20 16:49:51.000000 blendr_cli-0.1.6/blendr/__init__.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.953066 blendr_cli-0.1.6/blendr/ai/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-07 17:29:37.000000 blendr_cli-0.1.6/blendr/ai/__init__.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.953460 blendr_cli-0.1.6/blendr/ai/data/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-07 17:29:37.000000 blendr_cli-0.1.6/blendr/ai/data/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      874 2024-05-11 22:52:26.000000 blendr_cli-0.1.6/blendr/ai/data/cache.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      854 2024-05-07 18:37:26.000000 blendr_cli-0.1.6/blendr/ai/data/data_loader.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.953732 blendr_cli-0.1.6/blendr/ai/models/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-07 17:29:37.000000 blendr_cli-0.1.6/blendr/ai/models/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-12 17:44:41.000000 blendr_cli-0.1.6/blendr/ai/models/base_model.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.954082 blendr_cli-0.1.6/blendr/ai/tasks/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-07 17:29:37.000000 blendr_cli-0.1.6/blendr/ai/tasks/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-07 17:30:16.000000 blendr_cli-0.1.6/blendr/ai/tasks/evaluate.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3600 2024-05-16 10:04:13.000000 blendr_cli-0.1.6/blendr/ai/tasks/fine_tune.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.954619 blendr_cli-0.1.6/blendr/ai/training/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-07 17:29:37.000000 blendr_cli-0.1.6/blendr/ai/training/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      932 2024-05-07 18:39:20.000000 blendr_cli-0.1.6/blendr/ai/training/trainer.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-07 17:29:59.000000 blendr_cli-0.1.6/blendr/ai/training/training_utils.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.954844 blendr_cli-0.1.6/blendr/auth/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:43.000000 blendr_cli-0.1.6/blendr/auth/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     1999 2024-05-13 10:43:06.000000 blendr_cli-0.1.6/blendr/auth/authenticate.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     1917 2024-05-13 10:43:32.000000 blendr_cli-0.1.6/blendr/cli.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.955513 blendr_cli-0.1.6/blendr/config/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:41.000000 blendr_cli-0.1.6/blendr/config/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      197 2024-05-13 13:36:01.000000 blendr_cli-0.1.6/blendr/config/settings.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     6119 2024-04-30 14:25:22.000000 blendr_cli-0.1.6/blendr/config/setup.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.955915 blendr_cli-0.1.6/blendr/gpu_manager/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:38.000000 blendr_cli-0.1.6/blendr/gpu_manager/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      190 2024-04-29 20:05:17.000000 blendr_cli-0.1.6/blendr/gpu_manager/detect.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.956167 blendr_cli-0.1.6/blendr/initiate_socket/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-05-12 18:29:28.000000 blendr_cli-0.1.6/blendr/initiate_socket/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      686 2024-05-16 09:27:17.000000 blendr_cli-0.1.6/blendr/initiate_socket/initiate.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.956535 blendr_cli-0.1.6/blendr/task_manager/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:33.000000 blendr_cli-0.1.6/blendr/task_manager/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     1731 2024-05-16 09:36:15.000000 blendr_cli-0.1.6/blendr/task_manager/listen.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-05-16 11:58:10.957632 blendr_cli-0.1.6/blendr_cli.egg-info/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3271 2024-05-16 11:58:10.000000 blendr_cli-0.1.6/blendr_cli.egg-info/PKG-INFO
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      922 2024-05-16 11:58:10.000000 blendr_cli-0.1.6/blendr_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        1 2024-05-16 11:58:10.000000 blendr_cli-0.1.6/blendr_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       43 2024-05-16 11:58:10.000000 blendr_cli-0.1.6/blendr_cli.egg-info/entry_points.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      178 2024-05-16 11:58:10.000000 blendr_cli-0.1.6/blendr_cli.egg-info/requires.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        7 2024-05-16 11:58:10.000000 blendr_cli-0.1.6/blendr_cli.egg-info/top_level.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       38 2024-05-16 11:58:10.958131 blendr_cli-0.1.6/setup.cfg
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      942 2024-05-16 11:58:08.000000 blendr_cli-0.1.6/setup.py
```

### Comparing `blendr_cli-0.1.5/PKG-INFO` & `blendr_cli-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendr-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: Blendr CLI tool for GPU Lending
 Home-page: https://www.blendr.network
 Author: Blendr Network
 Author-email: tech@blendr.network
 License: MIT
 Keywords: blendr cli
 Description-Content-Type: text/markdown
@@ -13,14 +13,15 @@
 Requires-Dist: colorama==0.4.6
 Requires-Dist: GPUtil==1.4.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: keyring==25.2.0
 Requires-Dist: speedtest-cli==2.1.3
 Requires-Dist: py-cpuinfo==9.0.0
 Requires-Dist: python-socketio[client]==5.11.2
+Requires-Dist: datasets==2.19.1
 
 # Blendr CLI
 
 Blendr CLI is a command-line interface designed to help users lend their GPU resources for computational tasks on the Blendr platform. This tool allows for easy setup, management, and monitoring of GPU resources from your terminal.
 
 ## Features
```

### Comparing `blendr_cli-0.1.5/README.md` & `blendr_cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.5/blendr/auth/authenticate.py` & `blendr_cli-0.1.6/blendr/auth/authenticate.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import keyring
 
 
 def login():
     """Handles user login with server validation."""
     
       # Request session ID from server
+    print("Requesting session ID from the server...")
+    print(SERVER_URL)
     response = requests.post(f'{SERVER_URL}/api/generate/session-id', json={'deviceID': 'macOS'})
     session_id = response.json().get('sessionId')
 
     # Open browser for user login and confirmation
     print("Opening browser for user login and confirmation...")
     print(f'URL: {CLIENT_URL}/verify?sessionId={session_id}')
     webbrowser.open(f'{CLIENT_URL}/verify?sessionId={session_id}')
```

### Comparing `blendr_cli-0.1.5/blendr/cli.py` & `blendr_cli-0.1.6/blendr/cli.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.5/blendr/config/setup.py` & `blendr_cli-0.1.6/blendr/config/setup.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.5/blendr/task_manager/listen.py` & `blendr_cli-0.1.6/blendr/task_manager/listen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,66 @@
 from blendr.config.settings import SERVER_URL
 from blendr.config.setup import load_config
 import keyring
-import socketio
-import requests
-
-
+from blendr.ai.tasks.fine_tune import fine_tune
+from blendr.initiate_socket.initiate import sio, connect_to_server
 
+    
 def listen():
     """Listen to Server Tasks"""
     token = keyring.get_password("system", "blendr_jwt_token")
-    # print("Listening for task updates...")
+    connect_to_server(SERVER_URL, token)
 
-     # Create a Socket.IO client
-    http_session = requests.Session()
-    http_session.verify = False
-    sio = socketio.Client(http_session=http_session)
-    
     @sio.event
     def connect():
         print("Connected to the server. Listening to Task..")
-        initialConfig = load_config()
-        # print(initialConfig)
-        sio.emit('initialconfig', initialConfig)
+        # initialConfig = load_config()
+        # sio.emit('initialconfig', initialConfig)
 
     @sio.event
     def connect_error(data):
         print("The connection failed!")
     
     @sio.event()
     def error(data):
         print(f"Error: {data.get('message')}")
         
     @sio.event
     def disconnect():
         print("I'm disconnected!")
     
   
-# Process the task completion data
-    
+# Process the task completion dat
 #  mainEmitter.to(socketID).emit("MAIN: UserConnect", payload);
 
 
     # # Define event handlers
-    # @sio.on('task_update')
-    # def handle_task_update(data):
-    #     print(f"Received task update: {data}")
-    #     time.sleep(2)
-    #     print("emiting..")
-    #     sio.emit('test', {'foo': 'bar'})
+    @sio.on('BMAIN: NEW_TASK')
+    def handle_new_task(data):
+        print(f"New task received: {data}")
+        # Based on the task type, decide the function to call
+        if data['taskType'] == 'FINE_TUNE':
+            try:
+                fine_tune(data)
+            except Exception as e:
+                print(f"An error occurred during task execution: {str(e)}")
 
-    #     # Process the task update data
-
- 
-        # Process the task completion data
-        
-    # @sio.on('task_completed')
-    # def handle_task_completed(data):
-    #     print(f"Task completed: {data}")
-    #     # Process the task completion data
-
-    # # Listen for the 'error' event
-    # @sio.event
-    # def error_handler(data):
-    #     print(data)
-    #     print(f"Error: {data['message']}")
-    #     sio.disconnect()
-
-    # # Listen for the 'disconnect' event
-    # @sio.event
-    # def disconnect_handler():
-    #     print("Disconnected from server")
-
-    try:
-        sio.connect(SERVER_URL, headers={"Authorization": f"Bearer {token}"})
+    # try:
+    #     sio.connect(SERVER_URL, headers={"Authorization": f"Bearer {token}"})
         
-    except socketio.exceptions.ConnectionError as e:
-        print(f"ConnectionError: {str(e)}")
-    except Exception as e:
-        print(f"Unexpected error: {str(e)}")
-        return
+    # except socketio.exceptions.ConnectionError as e:
+    #     print(f"ConnectionError: {str(e)}")
+    # except Exception as e:
+    #     print(f"Unexpected error: {str(e)}")
+    #     return
     
 
- 
-
-
 
     # Start the event loop
     sio.wait()
 
     # Clean up and disconnect
-    # sio.disconnect()
+    sio.disconnect()
```

### Comparing `blendr_cli-0.1.5/blendr_cli.egg-info/PKG-INFO` & `blendr_cli-0.1.6/blendr_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendr-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: Blendr CLI tool for GPU Lending
 Home-page: https://www.blendr.network
 Author: Blendr Network
 Author-email: tech@blendr.network
 License: MIT
 Keywords: blendr cli
 Description-Content-Type: text/markdown
@@ -13,14 +13,15 @@
 Requires-Dist: colorama==0.4.6
 Requires-Dist: GPUtil==1.4.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: keyring==25.2.0
 Requires-Dist: speedtest-cli==2.1.3
 Requires-Dist: py-cpuinfo==9.0.0
 Requires-Dist: python-socketio[client]==5.11.2
+Requires-Dist: datasets==2.19.1
 
 # Blendr CLI
 
 Blendr CLI is a command-line interface designed to help users lend their GPU resources for computational tasks on the Blendr platform. This tool allows for easy setup, management, and monitoring of GPU resources from your terminal.
 
 ## Features
```

### Comparing `blendr_cli-0.1.5/setup.py` & `blendr_cli-0.1.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='blendr-cli',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'click==8.1.7',
         'requests==2.31.0',
         'colorama==0.4.6',
         'GPUtil==1.4.0',
         'psutil==5.9.8',
         'keyring==25.2.0',
         'speedtest-cli==2.1.3',
         'py-cpuinfo==9.0.0',
-        'python-socketio[client]==5.11.2'
+        'python-socketio[client]==5.11.2',
+        'datasets==2.19.1'
+
     ],
     entry_points={
         'console_scripts': [
             'blendr=blendr.cli:main'
         ]
     },
     author='Blendr Network',
```

