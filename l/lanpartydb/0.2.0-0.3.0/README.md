# Comparing `tmp/lanpartydb-0.2.0.tar.gz` & `tmp/lanpartydb-0.3.0.tar.gz`

## Comparing `lanpartydb-0.2.0.tar` & `lanpartydb-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/.editorconfig
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/src/lanpartydb/__init__.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/src/lanpartydb/models.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/src/lanpartydb/reading.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/LICENSE
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/README.md
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 lanpartydb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/src/lanpartydb/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/src/lanpartydb/models.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/src/lanpartydb/reading.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/LICENSE
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/README.md
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 lanpartydb-0.3.0/PKG-INFO
```

### Comparing `lanpartydb-0.2.0/src/lanpartydb/models.py` & `lanpartydb-0.3.0/src/lanpartydb/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     slug: str
     title: str
     series_slug: str | None = field(kw_only=True, default=None)
     organizer_entity: str | None = field(kw_only=True, default=None)
     start_on: date
     end_on: date
     seats: int | None = None
+    attendees: int | None = None
     online: bool | None = False
     location: Location | None = None
     links: Links | None = None
 
 
 @dataclass(frozen=True)
 class Location:
```

### Comparing `lanpartydb-0.2.0/src/lanpartydb/reading.py` & `lanpartydb-0.3.0/src/lanpartydb/reading.py`

 * *Files identical despite different names*

### Comparing `lanpartydb-0.2.0/LICENSE` & `lanpartydb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lanpartydb-0.2.0/pyproject.toml` & `lanpartydb-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 [project]
 name = "lanpartydb"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python library for the OrgaTalk LAN Party Database"
 authors = [
     { name = "Jochen Kupperschmidt", email = "homework@nwsnet.de" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.11"
 license = { text = "MIT" }
+keywords = [ "lanparty" ]
+classifiers = [
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+]
+
+[project.urls]
+Repository = "https://github.com/orgatalk/lanpartydb-lib-python"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
```

