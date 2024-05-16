# Comparing `tmp/ultyas-1.0.4.tar.gz` & `tmp/ultyas-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultyas-1.0.4.tar", last modified: Wed Jun  7 13:02:47 2023, max compression
+gzip compressed data, was "ultyas-1.0.5.tar", last modified: Fri Apr 12 01:21:23 2024, max compression
```

## Comparing `ultyas-1.0.4.tar` & `ultyas-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-06-07 13:02:47.006060 ultyas-1.0.4/
--rw-r--r--   0 work      (1000) work      (1000)       26 2023-04-18 14:41:15.000000 ultyas-1.0.4/.gitignore
--rw-r--r--   0 work      (1000) work      (1000)    35149 2023-04-04 03:13:38.000000 ultyas-1.0.4/LICENSE
--rw-r--r--   0 work      (1000) work      (1000)     1428 2023-06-07 13:02:47.006060 ultyas-1.0.4/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      713 2023-04-18 14:41:15.000000 ultyas-1.0.4/README.md
--rw-r--r--   0 work      (1000) work      (1000)       38 2023-06-07 13:02:47.006060 ultyas-1.0.4/setup.cfg
--rwxr-xr-x   0 work      (1000) work      (1000)     1256 2023-06-07 13:01:04.000000 ultyas-1.0.4/setup.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-06-07 13:02:47.006060 ultyas-1.0.4/ultyas/
--rw-r--r--   0 work      (1000) work      (1000)     4579 2023-06-07 12:45:28.000000 ultyas-1.0.4/ultyas/__init__.py
--rw-r--r--   0 work      (1000) work      (1000)     6908 2023-06-07 12:45:28.000000 ultyas-1.0.4/ultyas/ultisnips.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-06-07 13:02:47.006060 ultyas-1.0.4/ultyas.egg-info/
--rw-r--r--   0 work      (1000) work      (1000)     1428 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      229 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/SOURCES.txt
--rw-r--r--   0 work      (1000) work      (1000)        1 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/dependency_links.txt
--rw-r--r--   0 work      (1000) work      (1000)       66 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/entry_points.txt
--rw-r--r--   0 work      (1000) work      (1000)        7 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-04-12 01:21:23.397992 ultyas-1.0.5/
+-rw-r--r--   0 dev        (455) work      (1000)       26 2024-04-12 01:20:02.000000 ultyas-1.0.5/.gitignore
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-04-12 01:20:02.000000 ultyas-1.0.5/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     1527 2024-04-12 01:21:23.397992 ultyas-1.0.5/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      812 2024-04-12 01:20:02.000000 ultyas-1.0.5/README.md
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-04-12 01:21:23.397992 ultyas-1.0.5/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     1256 2024-04-12 01:20:02.000000 ultyas-1.0.5/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-04-12 01:21:23.397992 ultyas-1.0.5/ultyas/
+-rw-r--r--   0 dev        (455) work      (1000)     4620 2024-04-12 01:20:02.000000 ultyas-1.0.5/ultyas/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     8859 2024-04-12 01:20:02.000000 ultyas-1.0.5/ultyas/ultisnips.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-04-12 01:21:23.397992 ultyas-1.0.5/ultyas.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     1527 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      229 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       66 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)        7 2024-04-12 01:21:23.000000 ultyas-1.0.5/ultyas.egg-info/top_level.txt
```

### Comparing `ultyas-1.0.4/LICENSE` & `ultyas-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ultyas-1.0.4/PKG-INFO` & `ultyas-1.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultyas
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool for converting code snippets from Ultisnips to YASnippet format
 Home-page: https://github.com/jamescherti/ultyas
 Author: James Cherti
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
@@ -14,31 +14,36 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ultyas - Ultisnips to YASnippet Conversion Tool
 
-Ultyas is a command-line tool, written by [James Cherti](https://www.jamescherti.com), designed to simplify the process of converting code snippets from Ultisnips to YASnippet format.
+Ultyas is a command-line tool designed to simplify the process of converting code snippets
+from Ultisnips (Vim) to YASnippet format (Emacs).
 
-With Ultyas, you can effortlessly migrate your code snippets to the YASnippet format, saving you valuable time and effort.
+With Ultyas, you can effortlessly migrate your code snippets to the YASnippet format,
+saving you valuable time and effort.
 
 ## Installation
 
+Here is how to install Ultyas locally to `~/.local/bin/ultyas` using pip:
 ```
-sudo pip install ultyas
+pip install --user ultyas
 ```
 
 ## Usage
 
-``` shell
-ultyas ~/.vim/UltiSnips/python.snippets -o ~/.emacs.d/snippets/python-mode/
+```
+~/.local/bin/ultyas ~/.vim/UltiSnips/python.snippets -o ~/.emacs.d/snippets/python-mode/
 ```
 
 ## License
 
+Copyright (c) [James Cherti](https://www.jamescherti.com)
+
 Distributed under terms of the GNU General Public License version 3.
 
 ## Links
 
 - [Ultyas @PyPI](https://pypi.org/project/ultyas/)
 - [Ultyas @GitHub](https://github.com/jamescherti/ultyas/)
```

### Comparing `ultyas-1.0.4/README.md` & `ultyas-1.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # Ultyas - Ultisnips to YASnippet Conversion Tool
 
-Ultyas is a command-line tool, written by [James Cherti](https://www.jamescherti.com), designed to simplify the process of converting code snippets from Ultisnips to YASnippet format.
+Ultyas is a command-line tool designed to simplify the process of converting code snippets
+from Ultisnips (Vim) to YASnippet format (Emacs).
 
-With Ultyas, you can effortlessly migrate your code snippets to the YASnippet format, saving you valuable time and effort.
+With Ultyas, you can effortlessly migrate your code snippets to the YASnippet format,
+saving you valuable time and effort.
 
 ## Installation
 
+Here is how to install Ultyas locally to `~/.local/bin/ultyas` using pip:
 ```
-sudo pip install ultyas
+pip install --user ultyas
 ```
 
 ## Usage
 
-``` shell
-ultyas ~/.vim/UltiSnips/python.snippets -o ~/.emacs.d/snippets/python-mode/
+```
+~/.local/bin/ultyas ~/.vim/UltiSnips/python.snippets -o ~/.emacs.d/snippets/python-mode/
 ```
 
 ## License
 
+Copyright (c) [James Cherti](https://www.jamescherti.com)
+
 Distributed under terms of the GNU General Public License version 3.
 
 ## Links
 
 - [Ultyas @PyPI](https://pypi.org/project/ultyas/)
 - [Ultyas @GitHub](https://github.com/jamescherti/ultyas/)
```

### Comparing `ultyas-1.0.4/setup.py` & `ultyas-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 CURRENT_DIRECTORY = Path(__file__).parent.resolve()
 LONG_DESCRIPTION = \
     (CURRENT_DIRECTORY / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ultyas",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     description=("A tool for converting code snippets from "
                  "Ultisnips to YASnippet format"),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/ultyas",
     author="James Cherti",
```

### Comparing `ultyas-1.0.4/ultyas/__init__.py` & `ultyas-1.0.5/ultyas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,13 +143,14 @@
 
             print(f"Successfully converted '{ultisnips_file}' to "
                   f"'{yasnippet_dir}'.")
     except UltisnipsParseError as err:
         print(f"Parse error: {err}", file=sys.stderr)
         sys.exit(1)
     except OSError as err:
-        print(f"Error: {err}", file=sys.stderr)
+        print(f"Error: {err.filename}: {err}", file=sys.stderr)
+        print(err.errno)
         sys.exit(1)
 
 
 if __name__ == '__main__':
     command_line_interface()
```

### Comparing `ultyas-1.0.4/ultyas/ultisnips.py` & `ultyas-1.0.5/ultyas/ultisnips.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """Ultisnips to YASnippet Conversion Tool."""
 
+import platform
 import hashlib
 import os
 import re
 from pathlib import Path
 from typing import List
 
 
@@ -48,73 +49,102 @@
 
 
 class UltisnipsSnippetsFile:
     def __init__(self):
         self.snippets = {}
 
     def load(self, snippet_file: os.PathLike):
-        inside_snippet = False
+        current_block = ""
         line_num = 0
         current_snippet_name = ""
-        current_snippet_content = ""
+        block_content = ""
+
         with open(snippet_file, "r", encoding="utf-8") as fhandler:
-            line_num += 1
             for line in fhandler.readlines():
-                line_strip = line.rstrip("\n").strip()
+                line_num += 1
+                line_strip = re.sub(r"#.*$", "", line.strip())
+
+                if current_block:
+                    if line_strip == f"end{current_block}":
+                        if current_block == "snippet":
+                            self.snippets[current_snippet_name] = \
+                                Snippet(name=current_snippet_name,
+                                        content=block_content)
+
+                        current_block = ""
+                        current_snippet_name = ""
 
-                if inside_snippet:
-                    if line_strip == "endsnippet":
-                        inside_snippet = False
-                        self.snippets[current_snippet_name] = \
-                            Snippet(name=current_snippet_name,
-                                    content=current_snippet_content)
+                        # Ignore other blocks (e.g., global)
+                        continue
                     else:
-                        current_snippet_content += line
+                        block_content += line
+                        continue
+
+                new_block_found = False
+                for block_name in ["snippet", "global"]:
+                    if re.search(r"^" + re.escape(block_name) + r"\s",
+                                 line_strip):
+                        current_block = block_name
+                        block_content = ""
+                        new_block_found = True
+
+                        if block_name == "snippet":
+                            try:
+                                current_snippet_name = \
+                                    re.split(r"\s+", line)[1]
+                            except IndexError:
+                                line = line.rstrip("\n")
+                                err = (f"Snippet name not specified: "
+                                       f"{snippet_file}: {line_num}: '{line}'")
+                                raise UltisnipsParseError(err) from IndexError
+
+                        break
 
-                    # Success
+                if new_block_found:
                     continue
 
-                if re.search(r"^snippet\s", line_strip):
-                    try:
-                        current_snippet_name = re.split(r"\s+", line)[1]
-                    except IndexError:
-                        line = line.rstrip("\n")
-                        err = (f"Snippet name not specified: "
-                               f"{snippet_file}: {line_num}: '{line}'")
-                        raise UltisnipsParseError(err) from IndexError
-
-                    current_snippet_content = ""
-                    inside_snippet = True
-                    continue  # Success
+                one_liner_found = False
+                for one_liner in ["priority", "post_jump"]:
+                    if re.search(r"^\s*" + re.escape(one_liner) + r"\s",
+                                 line_strip):
+                        one_liner_found = True
+                        break
 
-                if re.search(r"\s*priority\s", line):
-                    # Ignore priority
+                if one_liner_found:
                     continue
 
-                line_strip = re.sub(r"#.*$", "", line_strip)  # Comment
+                # Error
                 if line_strip != "":
                     line = line.rstrip("\n")
                     err = f"{snippet_file}: {line_num}: '{line}'"
                     raise UltisnipsParseError(err)
 
+        if current_block:
+            line = line.rstrip("\n")
+            err = \
+                f"{snippet_file}: {line_num}: Unable to find the " \
+                f"end of {current_block}"
+            raise UltisnipsParseError(err)
+
     def convert_to_yasnippet(self, directory: os.PathLike,
                              convert_tabs_to: str = "$>",
                              yas_indent_line: str = "") -> List[str]:
         if yas_indent_line and yas_indent_line not in ("auto", "fixed"):
             yas_indent_line = ""
 
         comment_yas_indent_line = (
             f"# expand-env: ((yas-indent-line '{yas_indent_line}))\n"
             if yas_indent_line
             else ""
         )
 
         result = []
         for snippet_name, snippet_data in self.snippets.items():
-            snippet_path = Path(directory).joinpath(snippet_name)
+            snippet_path = \
+                Path(directory).joinpath(self._sanitize_filename(snippet_name))
             result.append(str(snippet_path))
 
             header = ("# -*- mode: snippet -*-\n"
                       f"# name: {snippet_name}\n"
                       f"# key: {snippet_name}\n"  # Used to expand
                       f"{comment_yas_indent_line}"
                       "# --\n")
@@ -185,7 +215,35 @@
                     result += "\\"
 
             # Add the character
             result += string[index]
             index += 1
 
         return result
+
+    @staticmethod
+    def _sanitize_filename(filename: str) -> str:
+        """
+        Remove invalid characters from a filename to ensure it is valid for most
+        file systems.
+
+        Parameters:
+            filename: The original filename that may contain invalid characters.
+
+        Returns:
+            A sanitized version of the filename without invalid characters.
+        """
+        invalid_chars = {'/', '\0'}
+
+        if platform.system() == "Windows":
+            invalid_chars = {'/', '\\', ':', '*', '?', '"', '<', '>', '|'}
+            for index in range(0, 32):
+                invalid_chars.add(chr(index))
+
+        sanitized_filename = ""
+        for char in filename:
+            if char in invalid_chars:
+                sanitized_filename += hex(ord(char))
+            else:
+                sanitized_filename += char
+
+        return sanitized_filename
```

### Comparing `ultyas-1.0.4/ultyas.egg-info/PKG-INFO` & `ultyas-1.0.5/ultyas.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultyas
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool for converting code snippets from Ultisnips to YASnippet format
 Home-page: https://github.com/jamescherti/ultyas
 Author: James Cherti
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
@@ -14,31 +14,36 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ultyas - Ultisnips to YASnippet Conversion Tool
 
-Ultyas is a command-line tool, written by [James Cherti](https://www.jamescherti.com), designed to simplify the process of converting code snippets from Ultisnips to YASnippet format.
+Ultyas is a command-line tool designed to simplify the process of converting code snippets
+from Ultisnips (Vim) to YASnippet format (Emacs).
 
-With Ultyas, you can effortlessly migrate your code snippets to the YASnippet format, saving you valuable time and effort.
+With Ultyas, you can effortlessly migrate your code snippets to the YASnippet format,
+saving you valuable time and effort.
 
 ## Installation
 
+Here is how to install Ultyas locally to `~/.local/bin/ultyas` using pip:
 ```
-sudo pip install ultyas
+pip install --user ultyas
 ```
 
 ## Usage
 
-``` shell
-ultyas ~/.vim/UltiSnips/python.snippets -o ~/.emacs.d/snippets/python-mode/
+```
+~/.local/bin/ultyas ~/.vim/UltiSnips/python.snippets -o ~/.emacs.d/snippets/python-mode/
 ```
 
 ## License
 
+Copyright (c) [James Cherti](https://www.jamescherti.com)
+
 Distributed under terms of the GNU General Public License version 3.
 
 ## Links
 
 - [Ultyas @PyPI](https://pypi.org/project/ultyas/)
 - [Ultyas @GitHub](https://github.com/jamescherti/ultyas/)
```

