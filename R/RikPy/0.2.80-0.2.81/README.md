# Comparing `tmp/RikPy-0.2.80.tar.gz` & `tmp/RikPy-0.2.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.80.tar", last modified: Thu May 16 17:37:32 2024, max compression
+gzip compressed data, was "RikPy-0.2.81.tar", last modified: Thu May 16 17:45:06 2024, max compression
```

## Comparing `RikPy-0.2.80.tar` & `RikPy-0.2.81.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 17:37:32.006959 RikPy-0.2.80/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.80/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-16 17:37:32.003968 RikPy-0.2.80/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 17:37:31.983029 RikPy-0.2.80/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.80/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.80/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.80/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.80/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.80/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.80/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     4062 2024-05-16 17:32:02.000000 RikPy-0.2.80/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     7919 2024-02-07 12:06:25.000000 RikPy-0.2.80/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.80/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.80/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:37:32.001972 RikPy-0.2.80/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-16 17:37:31.000000 RikPy-0.2.80/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-16 17:37:31.000000 RikPy-0.2.80/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 17:37:31.000000 RikPy-0.2.80/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 17:37:31.000000 RikPy-0.2.80/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.80/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.80/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-16 17:37:32.016931 RikPy-0.2.80/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.80/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:45:05.998157 RikPy-0.2.81/
+-rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.81/MANIFEST.in
+-rw-rw-rw-   0        0        0      176 2024-05-16 17:45:05.995164 RikPy-0.2.81/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 17:45:05.974221 RikPy-0.2.81/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.81/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.81/RikPy/commonfunctions.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.81/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.81/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.81/RikPy/commonleonardo.py
+-rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.81/RikPy/commonlogging.py
+-rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.81/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     7919 2024-02-07 12:06:25.000000 RikPy-0.2.81/RikPy/commons3.py
+-rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.81/RikPy/commonshopify.py
+-rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.81/RikPy/customresponse.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:45:05.991174 RikPy-0.2.81/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-16 17:45:05.000000 RikPy-0.2.81/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-16 17:45:05.000000 RikPy-0.2.81/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:45:05.000000 RikPy-0.2.81/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 17:45:05.000000 RikPy-0.2.81/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.81/logfile.txt
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.81/readme.md
+-rw-rw-rw-   0        0        0      295 2024-05-16 17:45:06.004140 RikPy-0.2.81/setup.cfg
+-rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.81/setup.py
```

### Comparing `RikPy-0.2.80/RikPy/commonfunctions.py` & `RikPy-0.2.81/RikPy/commonfunctions.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.80/RikPy/commongoogle.py` & `RikPy-0.2.81/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.80/RikPy/commonheroku.py` & `RikPy-0.2.81/RikPy/commonheroku.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.80/RikPy/commonleonardo.py` & `RikPy-0.2.81/RikPy/commonleonardo.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.80/RikPy/commonopenai.py` & `RikPy-0.2.81/RikPy/commonopenai.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,17 @@
 
         print("Summoning Pixels from the Digital Depths!")
         print(image_prompt)
 
         response = requests.post(url, headers=headers, data=json.dumps(payload))
         response_json = response.json()
 
+        # Print all headers for debugging
+        print("Response Headers:", response.headers)
+
         if response.status_code != 200: return CustomResponse(data={"error": response_json.get("error", "Unknown error")}, status_code=response.status_code)
         # Extract token usage information from headers
         token_usage = response.headers.get('X-OpenAI-Usage')
         return CustomResponse(data={"response": response_json, "usage": token_usage}, status_code=200)
 
     except requests.exceptions.RequestException as e:
         return CustomResponse(data={"error": str(e)}, status_code=500)
```

### Comparing `RikPy-0.2.80/RikPy/commons3.py` & `RikPy-0.2.81/RikPy/commons3.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.80/RikPy/commonshopify.py` & `RikPy-0.2.81/RikPy/commonshopify.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.80/logfile.txt` & `RikPy-0.2.81/logfile.txt`

 * *Files identical despite different names*

