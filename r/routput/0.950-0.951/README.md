# Comparing `tmp/routput-0.950.tar.gz` & `tmp/routput-0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.950.tar", last modified: Thu May 16 11:52:49 2024, max compression
+gzip compressed data, was "routput-0.951.tar", last modified: Thu May 16 12:05:45 2024, max compression
```

## Comparing `routput-0.950.tar` & `routput-0.951.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:52:49.887101 routput-0.950/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.950/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 11:52:49.886056 routput-0.950/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.950/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 11:52:49.885039 routput-0.950/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 11:52:49.000000 routput-0.950/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-05-16 11:52:49.000000 routput-0.950/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:52:49.000000 routput-0.950/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 11:52:49.000000 routput-0.950/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 11:52:49.887101 routput-0.950/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 11:38:04.000000 routput-0.950/setup.py
--rw-rw-rw-   0        0        0    19907 2024-05-16 11:52:49.000000 routput-0.950/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:05:45.876639 routput-0.951/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.951/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:05:45.876639 routput-0.951/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.951/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:05:45.000000 routput-0.951/README.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:05:45.875612 routput-0.951/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:05:45.000000 routput-0.951/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-16 12:05:45.000000 routput-0.951/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:05:45.000000 routput-0.951/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 12:05:45.000000 routput-0.951/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:05:45.876639 routput-0.951/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:05:29.000000 routput-0.951/setup.py
+-rw-rw-rw-   0        0        0    19875 2024-05-16 12:05:45.000000 routput-0.951/templated_setup.py
```

### Comparing `routput-0.950/LICENCE` & `routput-0.951/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.950/PKG-INFO` & `routput-0.951/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.950
+Version: 0.951
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
@@ -86,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.950 released on 16th/5/2024
+## V0.951 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.950/README.md` & `routput-0.951/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.950/routput.egg-info/PKG-INFO` & `routput-0.951/routput.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.950
+Version: 0.951
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
@@ -86,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.950 released on 16th/5/2024
+## V0.951 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.950/templated_setup.py` & `routput-0.951/templated_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,20 @@
 
 
 	@staticmethod
 	def __init_description(readme_file_path_) -> "str":
 
 		description = None
 
+		try:
+			import README #type:ignore
+			return base64_x_b64decode(README.__README__.encode()).decode()
+		except:
+			pass
+
 		if not os.path.exists(readme_file_path_):
 			raise FileNotFoundError(f"No such file or directory: [{readme_file_path_}].")
 		
 		if not os.path.isabs(readme_file_path_):
 			readme_file_path_ = os.path.abspath(readme_file_path_)
 
 		if not os.path.isfile(readme_file_path_):
@@ -628,14 +634,15 @@
 			time_x_sleep(0.5)
 			print(".", end="", flush=True)
 			time_x_sleep(0.8)
 
 		cls._name = name
 		cls._author = author
 		cls._description = description
+		cls._kwargs_for_setup_tools = kwargs_for_setup_tools
 
 		_Setup_Helper.__load_parameters()
 
 		assert isinstance(cls._date_of_last_modified, str)
 		cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._date_of_last_modified)
 
 		assert isinstance(cls._date_of_last_modified, datetime_x_date)
@@ -663,29 +670,22 @@
 	#################
 
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
-		# NOTE: If we do not hardcode the version, then pip will throw a fit when trying to install the 
-		# NOTE:   `templated-setup` package.
-		from . import _hardcoded #type:ignore
-		kwargs_for_setup_tools = base64_x_b64decode(_hardcoded.__kwargs_for_setup_tools__.encode("utf-8")) #type:ignore
-		kwargs_for_setup_tools = pickle_x_loads(kwargs_for_setup_tools)
-		long_description = base64_x_b64decode(_hardcoded.__long_description__.encode("utf-8")) #type:ignore
-		long_description = pickle_x_loads(long_description)
 		setup(
 			name=name,
-			version=_hardcoded.__version__, #type:ignore
-			author=_hardcoded.__author__, #type:ignore
-			description=_hardcoded.__description__, #type:ignore
+			version=cls._version.version_number,
+			author=cls._author,
+			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
-			long_description=long_description, #type:ignore
-			**kwargs_for_setup_tools
+			long_description=cls.long_description, #type:ignore
+			**cls._kwargs_for_setup_tools
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
 
 
@@ -698,14 +698,16 @@
 		assert isinstance(cls._notes, str)
 		assert isinstance(cls._readme_file_path, str)
 
 		long_description = _Setup_Helper.__init_description(cls._readme_file_path)
 		long_description += f"\n## V{cls._version.version_number} released on {cls._version.repr_date()}\n"
 		long_description += cls._notes
 
+		cls._long_description = long_description
+
 		_Setup_Helper.__clear_screen()
 		print(f"Current Directory: [{os.path.abspath(os.getcwd())}].\n\n")
 		is_root_of_project = _Setup_Helper.__get_y_n("Is this the root of the project?")
 		_Setup_Helper.__clear_screen()
 
 		if not is_root_of_project:
 			raise Exception("This script must be run from the root of the project directory.")
@@ -743,30 +745,38 @@
 		_Setup_Helper.__clear_screen()
 
 		meta = None
 		with open(__file__, "r") as f:
 			meta = f.read()
 		with open("templated_setup.py", "w") as f:
 			f.write(meta)
+		with open(cls._readme_file_path, "r") as f:
+			readme = f.read()
+		with open("README.py", "w") as f:
+			f.write("__README__ = \"\"\"")
+			f.write(base64_x_b64encode(readme.encode()).decode())
+			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
+		kwargs_for_setup_tools["py_modules"].append("README")
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
 		os.remove("templated_setup.py")
+		os.remove("README.py")
 
 		print("\n] Setup complete.\n\n")
 
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
```

