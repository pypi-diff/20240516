# Comparing `tmp/lollms_client-0.5.5.tar.gz` & `tmp/lollms_client-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.5.5.tar", last modified: Mon Apr 29 23:43:26 2024, max compression
+gzip compressed data, was "lollms_client-0.5.6.tar", last modified: Wed May 15 22:33:18 2024, max compression
```

## Comparing `lollms_client-0.5.5.tar` & `lollms_client-0.5.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 23:43:26.251910 lollms_client-0.5.5/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.5.5/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-04-29 23:43:26.250609 lollms_client-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 23:43:26.229139 lollms_client-0.5.5/lollms_client/
--rw-rw-rw-   0        0        0      341 2024-04-27 17:10:22.000000 lollms_client-0.5.5/lollms_client/__init__.py
--rw-rw-rw-   0        0        0    21876 2024-03-20 22:06:25.000000 lollms_client-0.5.5/lollms_client/lollms_config.py
--rw-rw-rw-   0        0        0    19899 2024-04-29 15:50:14.000000 lollms_client-0.5.5/lollms_client/lollms_core.py
--rw-rw-rw-   0        0        0     2073 2024-04-27 17:07:34.000000 lollms_client-0.5.5/lollms_client/lollms_discussion.py
--rw-rw-rw-   0        0        0    20548 2024-04-27 23:24:03.000000 lollms_client-0.5.5/lollms_client/lollms_personality.py
--rw-rw-rw-   0        0        0    65331 2024-04-27 15:52:23.000000 lollms_client-0.5.5/lollms_client/lollms_personality_worker.py
--rw-rw-rw-   0        0        0    18863 2024-04-29 23:43:11.000000 lollms_client-0.5.5/lollms_client/lollms_tasks.py
--rw-rw-rw-   0        0        0     2170 2024-04-29 23:40:27.000000 lollms_client-0.5.5/lollms_client/lollms_types.py
--rw-rw-rw-   0        0        0     2087 2024-04-27 16:48:27.000000 lollms_client-0.5.5/lollms_client/lollms_utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-29 23:43:26.249885 lollms_client-0.5.5/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-04-29 23:43:25.000000 lollms_client-0.5.5/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-04-29 23:43:26.000000 lollms_client-0.5.5/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 23:43:26.000000 lollms_client-0.5.5/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 23:43:26.000000 lollms_client-0.5.5/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 23:43:26.000000 lollms_client-0.5.5/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 23:43:26.251910 lollms_client-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      814 2024-04-29 23:43:16.000000 lollms_client-0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:33:18.692263 lollms_client-0.5.6/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.5.6/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-05-15 22:33:18.691263 lollms_client-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 22:33:18.667729 lollms_client-0.5.6/lollms_client/
+-rw-rw-rw-   0        0        0      341 2024-04-27 17:10:22.000000 lollms_client-0.5.6/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0    21876 2024-03-20 22:06:25.000000 lollms_client-0.5.6/lollms_client/lollms_config.py
+-rw-rw-rw-   0        0        0    20023 2024-05-07 23:05:45.000000 lollms_client-0.5.6/lollms_client/lollms_core.py
+-rw-rw-rw-   0        0        0     2073 2024-04-27 17:07:34.000000 lollms_client-0.5.6/lollms_client/lollms_discussion.py
+-rw-rw-rw-   0        0        0    20548 2024-04-27 23:24:03.000000 lollms_client-0.5.6/lollms_client/lollms_personality.py
+-rw-rw-rw-   0        0        0    65331 2024-04-27 15:52:23.000000 lollms_client-0.5.6/lollms_client/lollms_personality_worker.py
+-rw-rw-rw-   0        0        0    18863 2024-04-29 23:43:11.000000 lollms_client-0.5.6/lollms_client/lollms_tasks.py
+-rw-rw-rw-   0        0        0     2170 2024-04-29 23:40:27.000000 lollms_client-0.5.6/lollms_client/lollms_types.py
+-rw-rw-rw-   0        0        0     2087 2024-04-27 16:48:27.000000 lollms_client-0.5.6/lollms_client/lollms_utilities.py
+-rw-rw-rw-   0        0        0      900 2024-05-15 22:32:42.000000 lollms_client-0.5.6/lollms_client/lollms_xtts.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:33:18.690261 lollms_client-0.5.6/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:33:18.692263 lollms_client-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-05-15 22:33:06.000000 lollms_client-0.5.6/setup.py
```

### Comparing `lollms_client-0.5.5/LICENSE` & `lollms_client-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/PKG-INFO` & `lollms_client-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.5.5
+Version: 0.5.6
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.5.5/README.md` & `lollms_client-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/lollms_client/lollms_config.py` & `lollms_client-0.5.6/lollms_client/lollms_config.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/lollms_client/lollms_core.py` & `lollms_client-0.5.6/lollms_client/lollms_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,39 +302,41 @@
             headers = {
                 'Content-Type': 'application/json',
             }
 
         data = {
             'model':model_name,
             'prompt': prompt,
-            "stream":True,
+            "stream":stream,
             "temperature": float(temperature),
             "max_tokens": n_predict
         }
         completion_format_path = "/api/generate"
         if host_address.endswith("/"):
             host_address = host_address[:-1]
         url = f'{host_address}{completion_format_path}'
 
         response = requests.post(url, json=data, headers=headers)
 
         if response.status_code==404:
             ASCIIColors.error(response.content.decode("utf-8", errors='ignore'))
         text = ""
-        for line in response.iter_lines():
-            decoded = line.decode("utf-8")
-            json_data = json.loads(decoded)
-            chunk = json_data["response"]
-            ## Process the JSON data here
-            text +=chunk
-            if streaming_callback:
-                if not streaming_callback(chunk, MSG_TYPE.MSG_TYPE_CHUNK):
-                    break            
-            return text
-
+        if stream:
+            for line in response.iter_lines():
+                decoded = line.decode("utf-8")
+                json_data = json.loads(decoded)
+                chunk = json_data["response"]
+                ## Process the JSON data here
+                text +=chunk
+                if streaming_callback:
+                    if not streaming_callback(chunk, MSG_TYPE.MSG_TYPE_CHUNK):
+                        break            
+                return text
+        else:
+            return response.content["response"]
     def litellm_generate(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format:ELF_COMPLETION_FORMAT=ELF_COMPLETION_FORMAT.Instruct, service_key:str="", streaming_callback=None):
         # Set default values to instance variables if optional arguments are None
         host_address = host_address if host_address else self.host_address
         model_name = model_name if model_name else self.model_name
         n_predict = n_predict if n_predict else self.n_predict
         personality = personality if personality is not None else self.personality
         # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
```

### Comparing `lollms_client-0.5.5/lollms_client/lollms_discussion.py` & `lollms_client-0.5.6/lollms_client/lollms_discussion.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/lollms_client/lollms_personality.py` & `lollms_client-0.5.6/lollms_client/lollms_personality.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/lollms_client/lollms_personality_worker.py` & `lollms_client-0.5.6/lollms_client/lollms_personality_worker.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/lollms_client/lollms_tasks.py` & `lollms_client-0.5.6/lollms_client/lollms_tasks.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/lollms_client/lollms_types.py` & `lollms_client-0.5.6/lollms_client/lollms_types.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/lollms_client/lollms_utilities.py` & `lollms_client-0.5.6/lollms_client/lollms_utilities.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.5/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.5.6/lollms_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.5.5
+Version: 0.5.6
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.5.5/setup.py` & `lollms_client-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().splitlines()
     
 setuptools.setup(
     name="lollms_client",
-    version="0.5.5",
+    version="0.5.6",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

