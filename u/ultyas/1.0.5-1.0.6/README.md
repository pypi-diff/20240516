# Comparing `tmp/ultyas-1.0.5.tar.gz` & `tmp/ultyas-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultyas-1.0.5.tar", last modified: Fri Apr 12 01:21:23 2024, max compression
+gzip compressed data, was "ultyas-1.0.6.tar", last modified: Thu May 16 02:32:10 2024, max compression
```

## Comparing `ultyas-1.0.5.tar` & `ultyas-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-04-12 01:21:23.397992 ultyas-1.0.5/
--rw-r--r--   0 dev        (455) work      (1000)       26 2024-04-12 01:20:02.000000 ultyas-1.0.5/.gitignore
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-04-12 01:20:02.000000 ultyas-1.0.5/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     1527 2024-04-12 01:21:23.397992 ultyas-1.0.5/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      812 2024-04-12 01:20:02.000000 ultyas-1.0.5/README.md
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-04-12 01:21:23.397992 ultyas-1.0.5/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     1256 2024-04-12 01:20:02.000000 ultyas-1.0.5/setup.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-04-12 01:21:23.397992 ultyas-1.0.5/ultyas/
--rw-r--r--   0 dev        (455) work      (1000)     4620 2024-04-12 01:20:02.000000 ultyas-1.0.5/ultyas/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     8859 2024-04-12 01:20:02.000000 ultyas-1.0.5/ultyas/ultisnips.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-04-12 01:21:23.397992 ultyas-1.0.5/ultyas.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     1527 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      229 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       66 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)        7 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-16 02:32:10.208367 ultyas-1.0.6/
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-16 02:32:02.000000 ultyas-1.0.6/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     2850 2024-05-16 02:32:10.208367 ultyas-1.0.6/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     2135 2024-05-16 02:32:02.000000 ultyas-1.0.6/README.md
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-16 02:32:10.208367 ultyas-1.0.6/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     1256 2024-05-16 02:32:02.000000 ultyas-1.0.6/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-16 02:32:10.204367 ultyas-1.0.6/ultyas/
+-rw-r--r--   0 dev        (455) work      (1000)     4620 2024-05-16 02:32:02.000000 ultyas-1.0.6/ultyas/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     8882 2024-05-16 02:32:02.000000 ultyas-1.0.6/ultyas/ultisnips.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-16 02:32:10.208367 ultyas-1.0.6/ultyas.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     2850 2024-05-16 02:32:09.000000 ultyas-1.0.6/ultyas.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      218 2024-05-16 02:32:10.000000 ultyas-1.0.6/ultyas.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-16 02:32:09.000000 ultyas-1.0.6/ultyas.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       66 2024-05-16 02:32:09.000000 ultyas-1.0.6/ultyas.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)        7 2024-05-16 02:32:09.000000 ultyas-1.0.6/ultyas.egg-info/top_level.txt
```

### Comparing `ultyas-1.0.5/LICENSE` & `ultyas-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ultyas-1.0.5/setup.py` & `ultyas-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 CURRENT_DIRECTORY = Path(__file__).parent.resolve()
 LONG_DESCRIPTION = \
     (CURRENT_DIRECTORY / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ultyas",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(),
     description=("A tool for converting code snippets from "
                  "Ultisnips to YASnippet format"),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/ultyas",
     author="James Cherti",
```

### Comparing `ultyas-1.0.5/ultyas/__init__.py` & `ultyas-1.0.6/ultyas/__init__.py`

 * *Files identical despite different names*

### Comparing `ultyas-1.0.5/ultyas/ultisnips.py` & `ultyas-1.0.6/ultyas/ultisnips.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """Ultisnips to YASnippet Conversion Tool."""
 
-import platform
 import hashlib
 import os
+import platform
 import re
 from pathlib import Path
 from typing import List
 
 
 def md5sum_file(filename):
     md5 = hashlib.md5()
@@ -76,15 +76,15 @@
                         # Ignore other blocks (e.g., global)
                         continue
                     else:
                         block_content += line
                         continue
 
                 new_block_found = False
-                for block_name in ["snippet", "global"]:
+                for block_name in ("snippet", "global"):
                     if re.search(r"^" + re.escape(block_name) + r"\s",
                                  line_strip):
                         current_block = block_name
                         block_content = ""
                         new_block_found = True
 
                         if block_name == "snippet":
@@ -99,15 +99,15 @@
 
                         break
 
                 if new_block_found:
                     continue
 
                 one_liner_found = False
-                for one_liner in ["priority", "post_jump"]:
+                for one_liner in ("priority", "post_jump", "context"):
                     if re.search(r"^\s*" + re.escape(one_liner) + r"\s",
                                  line_strip):
                         one_liner_found = True
                         break
 
                 if one_liner_found:
                     continue
@@ -219,19 +219,20 @@
             index += 1
 
         return result
 
     @staticmethod
     def _sanitize_filename(filename: str) -> str:
         """
-        Remove invalid characters from a filename to ensure it is valid for most
-        file systems.
+        Remove invalid characters from a filename to ensure it is valid for
+        most file systems.
 
         Parameters:
-            filename: The original filename that may contain invalid characters.
+            filename: The original filename that may contain invalid
+            characters.
 
         Returns:
             A sanitized version of the filename without invalid characters.
         """
         invalid_chars = {'/', '\0'}
 
         if platform.system() == "Windows":
```

