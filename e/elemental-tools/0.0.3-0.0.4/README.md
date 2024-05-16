# Comparing `tmp/elemental_tools-0.0.3-py3-none-any.whl.zip` & `tmp/elemental_tools-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 3819 bytes, number of entries: 11
+Zip file size: 4134 bytes, number of entries: 11
 -rwx------  2.0 unx       15 b- defN 23-Oct-23 00:27 elemental_tools/__init__.py
 -rwx------  2.0 unx      267 b- defN 23-Oct-23 00:24 elemental_tools/design/__init__.py
 -rwx------  2.0 unx      532 b- defN 23-Oct-23 00:24 elemental_tools/file_manager/__init__.py
--rwx------  2.0 unx     1919 b- defN 23-Oct-23 01:41 elemental_tools/logger/__init__.py
--rwx------  2.0 unx      125 b- defN 23-Oct-23 01:42 elemental_tools/logger/test.py
+-rwx------  2.0 unx     1662 b- defN 23-Oct-23 15:29 elemental_tools/logger/__init__.py
+-rwx------  2.0 unx      146 b- defN 23-Oct-23 15:02 elemental_tools/logger/test.py
 -rwx------  2.0 unx      135 b- defN 23-Oct-23 00:35 elemental_tools/path/__init__.py
--rwx------  2.0 unx      158 b- defN 23-Oct-23 00:24 elemental_tools/storage/__init__.py
--rwx------  2.0 unx      235 b- defN 23-Oct-23 01:42 elemental_tools-0.0.3.dist-info/METADATA
--rwx------  2.0 unx       92 b- defN 23-Oct-23 01:42 elemental_tools-0.0.3.dist-info/WHEEL
--rwx------  2.0 unx       16 b- defN 23-Oct-23 01:42 elemental_tools-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      953 b- defN 23-Oct-23 01:42 elemental_tools-0.0.3.dist-info/RECORD
-11 files, 4447 bytes uncompressed, 2177 bytes compressed:  51.0%
+-rwx------  2.0 unx      936 b- defN 23-Oct-23 05:28 elemental_tools/storage/__init__.py
+-rwx------  2.0 unx      235 b- defN 23-Oct-23 15:39 elemental_tools-0.0.4.dist-info/METADATA
+-rwx------  2.0 unx       92 b- defN 23-Oct-23 15:39 elemental_tools-0.0.4.dist-info/WHEEL
+-rwx------  2.0 unx       16 b- defN 23-Oct-23 15:39 elemental_tools-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      953 b- defN 23-Oct-23 15:39 elemental_tools-0.0.4.dist-info/RECORD
+11 files, 4989 bytes uncompressed, 2492 bytes compressed:  50.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: elemental_tools/path/__init__.py
 Comment: 
 
 Filename: elemental_tools/storage/__init__.py
 Comment: 
 
-Filename: elemental_tools-0.0.3.dist-info/METADATA
+Filename: elemental_tools-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: elemental_tools-0.0.3.dist-info/WHEEL
+Filename: elemental_tools-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: elemental_tools-0.0.3.dist-info/top_level.txt
+Filename: elemental_tools-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: elemental_tools-0.0.3.dist-info/RECORD
+Filename: elemental_tools-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elemental_tools/logger/__init__.py

```diff
@@ -1,57 +1,58 @@
 import os
 
 from datetime import datetime
 
 from elemental_tools.design import unicode_colors
 
+
 def relative(path):
-    return os.path.join(os.path.dirname(__file__), path)
+	return os.path.join(os.path.dirname(__file__), path)
 
 
 class Logger:
-    
-    def __init__(self, app_name: str, owner: str, log_path: str, environment: str = ''):
-        if app_name is None:
-            self.app_name_upper = 'LOGGER'
-        else:
-            self.app_name_upper = str(app_name).upper()
-
-        self.log_path = log_path
-        self.environment = environment
-        self.owner = owner
-                
-    def log(self, level: str, message):
-        timestamp = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
-        level = level.upper()
-        owner = self.owner.upper()
-        correspondent_clr = unicode_colors.reset
-
-        def log_path():
-            if self.environment:
-                self.log_path = str(self.log_path + f"_{self.environment}")
-
-            os.makedirs(self.log_path, exist_ok=True)
-            filename = datetime.now().strftime('%d-%m-%Y') + ".log"
-            self.log_path = os.path.join(self.log_path, filename)
-            return self.log_path
-
-        content = f"{timestamp} [{self.app_name_upper}] [{owner}] [{level}]: {str(message)}"
-
-        with open(log_path(), 'a') as f:
-            f.write(str(content))
-
-        if level == 'INFO' or level == 'START':
-            correspondent_clr = unicode_colors.success_cyan
-        elif level == 'WARNING' or level == 'ALERT':
-            correspondent_clr = unicode_colors.alert
-        elif level == 'SUCCESS' or level == 'OK':
-            correspondent_clr = unicode_colors.success
-        elif level in ['CRITICAL', 'ERROR', 'FAULT', 'FAIL', 'FATAL']:
-            correspondent_clr = unicode_colors.fail
 
-        content = f"{timestamp} [{self.app_name_upper}] [{owner}] [{level}]: {str(message)}"
-        print(correspondent_clr, content, unicode_colors.reset)
+	def __init__(self, app_name: str, owner: str, log_path: str, environment: str = ''):
+		if app_name is None:
+			self.app_name_upper = 'LOGGER'
+		else:
+			self.app_name_upper = str(app_name).upper()
+
+		self.path = log_path
+		self.environment = environment
+		self.owner = owner
+
+	def log(self, level: str, message):
+		timestamp = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+		level = level.upper()
+		owner = self.owner.upper()
+		correspondent_clr = unicode_colors.reset
+
+		def log_path():
+			if self.environment:
+				self.path = str(self.log_path + f"_{self.environment}")
+			try:
+				os.makedirs(self.path, exist_ok=True)
+			except:
+				pass
+			filename = datetime.now().strftime('%d-%m-%Y') + ".log"
+			self.log_path = os.path.join(self.path, filename)
+			return self.log_path
+
+		content = f"\n{timestamp} [{self.app_name_upper}] [{owner}] [{level}]: {str(message)}"
+
+		with open(log_path(), 'a+') as f:
+			f.write(str(content))
+
+		if level == 'INFO' or level == 'START':
+			correspondent_clr = unicode_colors.success_cyan
+		elif level == 'WARNING' or level == 'ALERT':
+			correspondent_clr = unicode_colors.alert
+		elif level == 'SUCCESS' or level == 'OK':
+			correspondent_clr = unicode_colors.success
+		elif level in ['CRITICAL', 'ERROR', 'FAULT', 'FAIL', 'FATAL']:
+			correspondent_clr = unicode_colors.fail
 
-        return content
-        
+		content = f"{timestamp} [{self.app_name_upper}] [{owner}] [{level}]: {str(message)}"
+		print(correspondent_clr, content, unicode_colors.reset)
 
+		return content
```

## elemental_tools/logger/test.py

```diff
@@ -1,5 +1,6 @@
 from elemental_tools.logger import Logger
 
 logger = Logger('log', 'me', './path/to/log')
-logger.log('info', 'test message')
 
+for e in range(10):
+	logger.log('info', 'test message')
```

## elemental_tools/storage/__init__.py

```diff
@@ -1,9 +1,31 @@
-class cache:
-    mem = {}
+class Cache:
 
-    def store(self, owner, request):
-        self.mem[owner] = request
+	def __init__(self, file: str = cache_file):
+		self.cache_file = file
 
-    def read(self, owner):
-        return self.mem[owner]
+		if not os.path.isdir(os.path.dirname(os.path.abspath(cache_file))):
+			os.makedirs(os.path.dirname(os.path.abspath(cache_file)), exist_ok=True)
 
+		self.cache_file_content = open(cache_file, 'a+')
+		if self.cache_file_content.readlines():
+			self.cache_file_content = self.load()
+			try:
+				data = eval(self.cache_file_content.read())
+				for cache_item in data:
+					for title, value in cache_item.items():
+						setattr(self, title, value)
+
+			except SyntaxError:
+				raise Exception("Failed to parse the cache file!")
+
+	def save(self):
+		self.cache_file_content.write(
+			str([{title: value for title, value in self.__dict__.items() if not title.startswith('__')}]))
+		self.cache_file_content.close()
+		return open(cache_file, 'a+')
+
+	def load(self):
+		return open(self.cache_file, 'a+')
+
+	def get(self, prop):
+		return getattr(self, prop, None)
```

## Comparing `elemental_tools-0.0.3.dist-info/RECORD` & `elemental_tools-0.0.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 elemental_tools/__init__.py,sha256=ovguP4wzQEDNguczwiZnhMm4dRRVcvnzmHrfQtlRCNQ,15
 elemental_tools/design/__init__.py,sha256=Jrdq-3CBD7b3j-oQ7_8R8eSzxAWjZvmutq-_JEXQb5I,267
 elemental_tools/file_manager/__init__.py,sha256=R6xtViaKrIXyW64fyDdybDSVnEPUYh3jmYH0CGC041w,532
-elemental_tools/logger/__init__.py,sha256=8zbHt6dZmPOX8T37T5E6XZ4sAhyqXaSDfg9j8g0x8QA,1919
-elemental_tools/logger/test.py,sha256=YyZ6m7M6wLWfDjFGBayQ9sJD_pZDRM9bm8F3-rQMSjo,125
+elemental_tools/logger/__init__.py,sha256=rGwKe1a2lANeU22uv3qQL69RpFc3v_m3A_fMbaBBuOM,1662
+elemental_tools/logger/test.py,sha256=pvKYojX3sz4JqPhJXYuMrALUQGnvKY9fXy3soxEBq18,146
 elemental_tools/path/__init__.py,sha256=4xZzd6JwNVobHqRYi3IaW2Twh-b3sXPuvr5BPphImsc,135
-elemental_tools/storage/__init__.py,sha256=IhvZjkH0eB6mR6BN_1H5Llspif5CDhk0FGoUW4zUZMQ,158
-elemental_tools-0.0.3.dist-info/METADATA,sha256=sYKIdqrzVKZFz63dewgoIViDP0vfnfwT7_5HazqnNMQ,235
-elemental_tools-0.0.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-elemental_tools-0.0.3.dist-info/top_level.txt,sha256=pQ-DwAcAL19wFA8B6zXbM9opvSYDYVCfGcpZx00O-2U,16
-elemental_tools-0.0.3.dist-info/RECORD,,
+elemental_tools/storage/__init__.py,sha256=uzfoayXRPQ4XVgOMs3G4aX5Szj20FgfgYwERYijUZ40,936
+elemental_tools-0.0.4.dist-info/METADATA,sha256=hS-kLZwY28cU4j-uQUhTNdJvkT0MqyffFHgZXpd9dJk,235
+elemental_tools-0.0.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+elemental_tools-0.0.4.dist-info/top_level.txt,sha256=pQ-DwAcAL19wFA8B6zXbM9opvSYDYVCfGcpZx00O-2U,16
+elemental_tools-0.0.4.dist-info/RECORD,,
```

