# Comparing `tmp/routput-0.9985.tar.gz` & `tmp/routput-0.9986.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.9985.tar", last modified: Thu May 16 13:23:15 2024, max compression
+gzip compressed data, was "routput-0.9986.tar", last modified: Thu May 16 13:31:25 2024, max compression
```

## Comparing `routput-0.9985.tar` & `routput-0.9986.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:23:15.694417 routput-0.9985/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9985/LICENCE
--rw-rw-rw-   0        0        0     6443 2024-05-16 13:23:15.694417 routput-0.9985/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9985/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 13:23:15.000000 routput-0.9985/_README.py
--rw-rw-rw-   0        0        0     8505 2024-05-16 13:23:15.000000 routput-0.9985/_pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:23:15.693400 routput-0.9985/routput.egg-info/
--rw-rw-rw-   0        0        0     6443 2024-05-16 13:23:15.000000 routput-0.9985/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-16 13:23:15.000000 routput-0.9985/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:23:15.000000 routput-0.9985/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-16 13:23:15.000000 routput-0.9985/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 13:23:15.694417 routput-0.9985/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:45:46.000000 routput-0.9985/setup.py
--rw-rw-rw-   0        0        0    21175 2024-05-16 13:23:15.000000 routput-0.9985/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:31:25.078730 routput-0.9986/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9986/LICENCE
+-rw-rw-rw-   0        0        0     2597 2024-05-16 13:31:25.077716 routput-0.9986/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9986/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 13:31:24.000000 routput-0.9986/_README.py
+-rw-rw-rw-   0        0        0     3509 2024-05-16 13:31:24.000000 routput-0.9986/_pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:31:25.076680 routput-0.9986/routput.egg-info/
+-rw-rw-rw-   0        0        0     2597 2024-05-16 13:31:25.000000 routput-0.9986/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-16 13:31:25.000000 routput-0.9986/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:31:25.000000 routput-0.9986/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-16 13:31:25.000000 routput-0.9986/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:31:25.078730 routput-0.9986/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 13:30:51.000000 routput-0.9986/setup.py
+-rw-rw-rw-   0        0        0    21254 2024-05-16 13:31:24.000000 routput-0.9986/templated_setup.py
```

### Comparing `routput-0.9985/LICENCE` & `routput-0.9986/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.9985/README.md` & `routput-0.9986/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.9985/_README.py` & `routput-0.9986/_README.py`

 * *Files identical despite different names*

### Comparing `routput-0.9985/templated_setup.py` & `routput-0.9986/templated_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,27 +679,29 @@
 		version = c["version"]
 		author = c["author"]
 		description = c["description"]
 		long_description = c["long_description"]
 		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
 		if not kwargs_for_setup_tools.get("py_modules"):
 			kwargs_for_setup_tools["py_modules"] = []
+		if not kwargs_for_setup_tools.get("packages"):
+			kwargs_for_setup_tools["packages"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 		kwargs_for_setup_tools["py_modules"].append("pickled")
 		kwargs_for_setup_tools["py_modules"].append("README")
-		kwargs_for_setup_tools["py_modules"].append(name)
+		kwargs_for_setup_tools["packages"].append(name)
 
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
 			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
-			long_description=long_description, #type:ignore
+			long_description=long_description,
 			**kwargs_for_setup_tools
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
```

