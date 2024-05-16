# Comparing `tmp/check_requirements_txt-1.2.0.tar.gz` & `tmp/check_requirements_txt-1.2.1.tar.gz`

## Comparing `check_requirements_txt-1.2.0.tar` & `check_requirements_txt-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.0/src/check_requirements_txt/__about__.py
--rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.0/src/check_requirements_txt/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.0/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.0/README.md
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.1/src/check_requirements_txt/__about__.py
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.1/src/check_requirements_txt/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.1/README.md
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 check_requirements_txt-1.2.1/PKG-INFO
```

### Comparing `check_requirements_txt-1.2.0/src/check_requirements_txt/__init__.py` & `check_requirements_txt-1.2.1/src/check_requirements_txt/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,15 @@
 import argparse
 import functools
 import os
 import re
 import sys
 from collections import defaultdict
 from pathlib import Path
-from typing import Dict
-from typing import Generator
-from typing import Iterable
-from typing import List
-from typing import Optional
-from typing import Sequence
-from typing import Set
-from typing import Union
+from typing import Dict, Generator, Iterable, List, Optional, Sequence, Set, Union
 
 import pkg_resources
 
 MODULE_IMPORT_P = re.compile(r"^\s*?import\s+(?P<module>[a-zA-Z0-9_]+)")
 MODULE_FROM_P = re.compile(r"^\s*?from\s+(?P<module>[a-zA-Z0-9_]+).*?\simport")
 DROP_LINE_P = re.compile(r"^\w+:/+", re.I)
 project_modules = set()
@@ -68,15 +61,15 @@
     record = egg_dir / "RECORD"
     if record.exists() and record.is_file():
         with open(record) as file_obj:
             for line in file_obj:
                 path = line.split(",", 1)[0].strip()
                 if egg_dir.name in path:
                     continue
-                if '__init__.' in path:
+                if "__init__." in path:
                     modules.add(Path(path).parent.name.lower())
 
     if not modules:
         modules.add(package_name)
     return list(modules)
 
 
@@ -107,30 +100,34 @@
         for pack in find_depends(package):
             for mod in find_real_modules(pack):
                 modules[mod].add(package)
     return modules
 
 
 def get_imports(
-    paths: Union[Generator[Path, None, None], List[Path]]
+        paths: Union[Generator[Path, None, None], List[Path]]
 ) -> Dict[str, Set[str]]:
     modules: Dict[str, Set[str]] = defaultdict(set)
-    for path in paths:
-        if path.is_file() and path.suffix.lower() == ".py":
-            with open(path) as file_obj:
+
+    def process_path(p: Path):
+        if p.is_file() and p.suffix.lower() == ".py":
+            with open(p) as file_obj:
                 for idx, line in enumerate(file_obj, 1):
                     match = MODULE_IMPORT_P.search(line) or MODULE_FROM_P.search(line)
                     if not match:
                         continue
                     module = match.group("module").lower()
                     if module not in project_modules:
-                        modules[module].add(f"{path}:{idx}")
-        elif path.is_dir():
-            for module, files in get_imports(path.glob("**/*.py")).items():
-                modules[module].update(files)
+                        modules[module].add(f"{p}:{idx}")
+        elif p.is_dir() and not p.name.startswith("."):
+            for item in p.iterdir():
+                process_path(item)
+
+    for path in paths:
+        process_path(path)
     return modules
 
 
 def param_as_set(value: str) -> Set[str]:
     return {v.strip() for v in value.split(",") if v}
 
 
@@ -193,17 +190,17 @@
     )
     project_modules.update(m for p in project_modules.copy() for m in p.split("."))
 
     if not args.req_paths:
         for project in project_dirs:
             for path in args.req_paths or project.glob("**/*requirement*.txt"):
                 args.req_paths.add(path)
-    assert (
-        args.req_paths
-    ), 'No files matched pattern "*requirement*.txt", you need to specify the requirement(s) path(s)'
+    if not args.req_paths:
+        msg = 'No files matched pattern "*requirement*.txt", you need to specify the requirement(s) path(s)'
+        raise ValueError(msg)
 
     for path in args.req_paths:
         for module, value in load_req_modules(path).items():
             builtin_modules[module].update(value)
 
     error_count = 0
     args.ignore.add("pip")
```

### Comparing `check_requirements_txt-1.2.0/LICENSE.txt` & `check_requirements_txt-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `check_requirements_txt-1.2.0/README.md` & `check_requirements_txt-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `check_requirements_txt-1.2.0/pyproject.toml` & `check_requirements_txt-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `check_requirements_txt-1.2.0/PKG-INFO` & `check_requirements_txt-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-requirements-txt
-Version: 1.2.0
+Version: 1.2.1
 Summary: Check the missing packages in requirements.txt
 Project-URL: Documentation, https://github.com/ferstar/check-requirements-txt#readme
 Project-URL: Issues, https://github.com/ferstar/check-requirements-txt/issues
 Project-URL: Source, https://github.com/ferstar/check-requirements-txt
 Author-email: ferstar <zhangjianfei3@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

