# Comparing `tmp/plsp-0.21.tar.gz` & `tmp/plsp-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plsp-0.21.tar", last modified: Thu May 16 13:01:51 2024, max compression
+gzip compressed data, was "plsp-0.22.tar", last modified: Thu May 16 13:16:33 2024, max compression
```

## Comparing `plsp-0.21.tar` & `plsp-0.22.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:01:51.715724 plsp-0.21/
--rw-rw-rw-   0        0        0     2442 2024-05-16 13:01:51.714653 plsp-0.21/PKG-INFO
--rw-rw-rw-   0        0        0     5929 2024-05-16 09:31:25.000000 plsp-0.21/README.md
--rw-rw-rw-   0        0        0     7683 2024-05-16 13:01:51.000000 plsp-0.21/README.py
--rw-rw-rw-   0        0        0     3401 2024-05-16 13:01:51.000000 plsp-0.21/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:01:51.714144 plsp-0.21/plsp.egg-info/
--rw-rw-rw-   0        0        0     2442 2024-05-16 13:01:51.000000 plsp-0.21/plsp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2024-05-16 13:01:51.000000 plsp-0.21/plsp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:01:51.000000 plsp-0.21/plsp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 13:01:51.000000 plsp-0.21/plsp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 13:01:51.715724 plsp-0.21/setup.cfg
--rw-rw-rw-   0        0        0      287 2024-05-16 13:01:06.000000 plsp-0.21/setup.py
--rw-rw-rw-   0        0        0    21056 2024-05-16 13:01:51.000000 plsp-0.21/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:16:33.254373 plsp-0.22/
+-rw-rw-rw-   0        0        0     6288 2024-05-16 13:16:33.254373 plsp-0.22/PKG-INFO
+-rw-rw-rw-   0        0        0     5929 2024-05-16 09:31:25.000000 plsp-0.22/README.md
+-rw-rw-rw-   0        0        0     7683 2024-05-16 13:16:33.000000 plsp-0.22/_README.py
+-rw-rw-rw-   0        0        0     8401 2024-05-16 13:16:33.000000 plsp-0.22/_pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:16:33.253301 plsp-0.22/plsp.egg-info/
+-rw-rw-rw-   0        0        0     6288 2024-05-16 13:16:33.000000 plsp-0.22/plsp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-05-16 13:16:33.000000 plsp-0.22/plsp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:16:33.000000 plsp-0.22/plsp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-16 13:16:33.000000 plsp-0.22/plsp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:16:33.255394 plsp-0.22/setup.cfg
+-rw-rw-rw-   0        0        0      287 2024-05-16 13:01:06.000000 plsp-0.22/setup.py
+-rw-rw-rw-   0        0        0    21122 2024-05-16 13:16:33.000000 plsp-0.22/templated_setup.py
```

### Comparing `plsp-0.21/README.md` & `plsp-0.22/README.md`

 * *Files identical despite different names*

### Comparing `plsp-0.21/README.py` & `plsp-0.22/_README.py`

 * *Files identical despite different names*

### Comparing `plsp-0.21/templated_setup.py` & `plsp-0.22/templated_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -670,16 +670,16 @@
 	#################
 
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
-		import pickled
-		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
+		import _pickled
+		c = pickle_x_loads(base64_x_b64decode(_pickled.__INST__.encode()))
 		version = c["version"]
 		author = c["author"]
 		description = c["description"]
 		long_description = c["long_description"]
 		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
 		if not kwargs_for_setup_tools.get("py_modules"):
 			kwargs_for_setup_tools["py_modules"] = []
@@ -761,54 +761,55 @@
 		meta = None
 		with open(__file__, "r") as f:
 			meta = f.read()
 		with open("templated_setup.py", "w") as f:
 			f.write(meta)
 		with open(cls._readme_file_path, "r") as f:
 			readme = f.read()
-		with open("README.py", "w") as f:
+		with open("_README.py", "w") as f:
 			f.write("__README__ = \"\"\"")
 			f.write(base64_x_b64encode(readme.encode()).decode())
 			f.write("\"\"\"")
 		assert cls._version is not None
 		assert cls._author is not None
 		assert cls._description is not None
 		assert cls._name is not None
 		assert cls._long_description is not None
-		with open("pickled.py", "w") as f:
+		with open("_pickled.py", "w") as f:
 			f.write("__INST__ = \"\"\"")
 			f.write(base64_x_b64encode(pickle_x_dumps({
 				"version": cls._version,
 				"author": cls._author,
 				"description": cls._description,
 				"name": cls._name,
 				"long_description": cls._long_description,
 				"kwargs_for_setup_tools": kwargs_for_setup_tools,
 			})).decode())
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
-		kwargs_for_setup_tools["py_modules"].append("README")
-		kwargs_for_setup_tools["py_modules"].append("pickled")
+		kwargs_for_setup_tools["py_modules"].append("_README")
+		kwargs_for_setup_tools["py_modules"].append("_pickled")
+		kwargs_for_setup_tools["py_modules"].append(cls._name)
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
-		os.remove("pickled.py")
+		os.remove("_pickled.py")
 		os.remove("templated_setup.py")
-		os.remove("README.py")
+		os.remove("_README.py")
 
 		print("\n] Setup complete.\n\n")
 
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
```

