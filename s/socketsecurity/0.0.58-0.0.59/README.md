# Comparing `tmp/socketsecurity-0.0.58.tar.gz` & `tmp/socketsecurity-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.58.tar", last modified: Thu May 16 09:30:19 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.59.tar", last modified: Thu May 16 10:05:13 2024, max compression
```

## Comparing `socketsecurity-0.0.58.tar` & `socketsecurity-0.0.59.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:30:19.266027 socketsecurity-0.0.58/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:30:19.265853 socketsecurity-0.0.58/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.58/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 09:30:10.000000 socketsecurity-0.0.58/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:30:19.266067 socketsecurity-0.0.58/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:30:19.250979 socketsecurity-0.0.58/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       49 2024-05-16 09:30:07.000000 socketsecurity-0.0.58/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:30:19.260981 socketsecurity-0.0.58/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 09:30:05.000000 socketsecurity-0.0.58/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.58/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.58/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.58/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    10963 2024-05-16 09:28:06.000000 socketsecurity-0.0.58/socketsecurity/core/glitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.58/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.58/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.58/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5641 2024-05-16 09:29:23.000000 socketsecurity-0.0.58/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:30:19.263893 socketsecurity-0.0.58/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      561 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 09:30:19.000000 socketsecurity-0.0.58/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:05:13.629278 socketsecurity-0.0.59/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:05:13.629091 socketsecurity-0.0.59/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.59/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 10:03:45.000000 socketsecurity-0.0.59/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:05:13.629317 socketsecurity-0.0.59/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:05:13.618192 socketsecurity-0.0.59/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.59/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:05:13.628281 socketsecurity-0.0.59/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 10:03:39.000000 socketsecurity-0.0.59/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.59/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.59/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.59/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11019 2024-05-16 09:57:17.000000 socketsecurity-0.0.59/socketsecurity/core/glitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.59/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.59/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.59/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5641 2024-05-16 09:29:23.000000 socketsecurity-0.0.59/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:05:13.628873 socketsecurity-0.0.59/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      561 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 10:05:13.000000 socketsecurity-0.0.59/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.58/PKG-INFO` & `socketsecurity-0.0.59/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.58
+Version: 0.0.59
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.58/pyproject.toml` & `socketsecurity-0.0.59/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.58"
+version = "0.0.59"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.58/socketsecurity/core/__init__.py` & `socketsecurity-0.0.59/socketsecurity/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.58'
+__version__ = '0.0.59'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
```

### Comparing `socketsecurity-0.0.58/socketsecurity/core/classes.py` & `socketsecurity-0.0.59/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.58/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.59/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.58/socketsecurity/core/github.py` & `socketsecurity-0.0.59/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.58/socketsecurity/core/glitlab.py` & `socketsecurity-0.0.59/socketsecurity/core/glitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     project_id: int
 
     def __init__(self):
         self.commit_sha = ci_commit_sha
         self.api_url = ci_api_v4_url
         self.ref_type = ""
         self.event_name = ci_pipeline_source
-        self.workspace = project_dir
+        self.workspace = ci_project_dir
         self.repository = ci_project_name
         if "/" in self.repository:
             self.repository = self.repository.rsplit("/")[1]
         self.branch = ci_merge_request_source_branch_name
         self.default_branch = ci_default_branch
         if self.branch == self.default_branch:
             self.is_default_branch = True
@@ -142,15 +142,15 @@
         self.project_id = ci_merge_request_project_id
         if self.api_token is None:
             print("Unable to get gitlab API Token from GH_API_TOKEN")
             sys.exit(2)
 
     @staticmethod
     def check_event_type() -> str:
-        if ci_pipeline_source.lower() == "push":
+        if ci_pipeline_source.lower() == "push" or ci_pipeline_source.lower == 'merge_request_event':
             if ci_merge_request_iid is None or ci_merge_request_iid == "":
                 event_type = "main"
             else:
                 event_type = "diff"
         elif ci_pipeline_source.lower() == "issue_comment":
             event_type = "comment"
         else:
```

### Comparing `socketsecurity-0.0.58/socketsecurity/core/issues.py` & `socketsecurity-0.0.59/socketsecurity/core/issues.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 	"mediumCVE",
 	"mildCVE",
 	"minifiedFile",
 	"missingAuthor",
 	"missingDependency",
 	"missingLicense",
 	"mixedLicense",
+	"ambiguousClassifier",
 	"modifiedException",
 	"modifiedLicense",
 	"networkAccess",
 	"newAuthor",
 	"noAuthorData",
 	"noBugTracker",
 	"noREADME",
@@ -378,15 +379,15 @@
 	suggestion: str
 	title: str
 	emoji: str
 	nextStepTitle: str
 
 	def __init__(self):
 		self.description = "(Experimental) Copyleft license information was found"
-		self.props = {"comments": "Comments", "exceptionId": "Exception id", "licenseId": "License Identifier"}
+		self.props = {"comments": "Comments", "licenseId": "License Identifiers"}
 		self.suggestion = "Determine whether use of copyleft material works for you"
 		self.title = "Copyleft License"
 		self.emoji = "\u26a0\ufe0f"
 		self.nextStepTitle = "What do I need to know about license files?"
 
 	def __str__(self):
 		return json.dumps(self.__dict__)
@@ -398,15 +399,15 @@
 	suggestion: str
 	title: str
 	emoji: str
 	nextStepTitle: str
 
 	def __init__(self):
 		self.description = "(Experimental) A license not known to be considered permissive was found"
-		self.props = {"comments": "Comments", "exceptionId": "Exception id", "licenseId": "License Identifier"}
+		self.props = {"comments": "Comments", "licenseId": "License Identifier"}
 		self.suggestion = "Determine whether use of material not offered under a known permissive license works for you"
 		self.title = "Non-permissive License"
 		self.emoji = "\u26a0\ufe0f"
 		self.nextStepTitle = "What do I need to know about license files?"
 
 	def __str__(self):
 		return json.dumps(self.__dict__)
@@ -1102,24 +1103,44 @@
 	suggestion: str
 	title: str
 	emoji: str
 	nextStepTitle: str
 
 	def __init__(self):
 		self.description = "(Experimental) Package contains multiple licenses."
-		self.props = {"licenseId": "License Id"}
+		self.props = {"licenseId": "License Ids"}
 		self.suggestion = "A new version of the package should be published that includes a single license. Consumers may seek clarification from the package author. Ensure that the license details are consistent across the LICENSE file, package.json license field and license details mentioned in the README."
 		self.title = "Mixed license"
 		self.emoji = "\u26a0\ufe0f"
 		self.nextStepTitle = "What is a mixed license?"
 
 	def __str__(self):
 		return json.dumps(self.__dict__)
 
 
+class ambiguousClassifier:
+	props: dict
+	description: str
+	suggestion: str
+	title: str
+	emoji: str
+	nextStepTitle: str
+
+	def __init__(self):
+		self.props = {"classifier": "The classifier"}
+		self.description = "(Experimental) An ambiguous license classifier was found."
+		self.suggestion = "A specific license or licenses should be identified"
+		self.title = "Ambiguous License Classifier"
+		self.emoji = "\u26a0\ufe0f"
+		self.nextStepTitle = "What is an ambiguous license classifier?"
+
+	def __str__(self):
+		return json.dumps(self.__dict__)
+
+
 class modifiedException:
 	description: str
 	props: dict
 	suggestion: str
 	title: str
 	emoji: str
 	nextStepTitle: str
@@ -1939,14 +1960,15 @@
 	mediumCVE: mediumCVE
 	mildCVE: mildCVE
 	minifiedFile: minifiedFile
 	missingAuthor: missingAuthor
 	missingDependency: missingDependency
 	missingLicense: missingLicense
 	mixedLicense: mixedLicense
+	ambiguousClassifier: ambiguousClassifier
 	modifiedException: modifiedException
 	modifiedLicense: modifiedLicense
 	networkAccess: networkAccess
 	newAuthor: newAuthor
 	noAuthorData: noAuthorData
 	noBugTracker: noBugTracker
 	noREADME: noREADME
@@ -1979,15 +2001,14 @@
 	unstableOwnership: unstableOwnership
 	unusedDependency: unusedDependency
 	urlStrings: urlStrings
 	usesEval: usesEval
 	zeroWidth: zeroWidth
 	floatingDependency: floatingDependency
 	unpopularPackage: unpopularPackage
-
 	def __init__(self):
 		self.badEncoding = badEncoding()
 		self.badSemver = badSemver()
 		self.badSemverDependency = badSemverDependency()
 		self.bidi = bidi()
 		self.binScriptConfusion = binScriptConfusion()
 		self.chronoAnomaly = chronoAnomaly()
@@ -2033,14 +2054,15 @@
 		self.mediumCVE = mediumCVE()
 		self.mildCVE = mildCVE()
 		self.minifiedFile = minifiedFile()
 		self.missingAuthor = missingAuthor()
 		self.missingDependency = missingDependency()
 		self.missingLicense = missingLicense()
 		self.mixedLicense = mixedLicense()
+		self.ambiguousClassifier = ambiguousClassifier()
 		self.modifiedException = modifiedException()
 		self.modifiedLicense = modifiedLicense()
 		self.networkAccess = networkAccess()
 		self.newAuthor = newAuthor()
 		self.noAuthorData = noAuthorData()
 		self.noBugTracker = noBugTracker()
 		self.noREADME = noREADME()
```

### Comparing `socketsecurity-0.0.58/socketsecurity/core/licenses.py` & `socketsecurity-0.0.59/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.58/socketsecurity/core/messages.py` & `socketsecurity-0.0.59/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.58/socketsecurity/socketcli.py` & `socketsecurity-0.0.59/socketsecurity/socketcli.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.58/socketsecurity.egg-info/PKG-INFO` & `socketsecurity-0.0.59/socketsecurity.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.58
+Version: 0.0.59
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.58/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.59/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

