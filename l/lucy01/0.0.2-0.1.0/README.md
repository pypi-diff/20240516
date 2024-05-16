# Comparing `tmp/lucy01-0.0.2.tar.gz` & `tmp/lucy01-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucy01-0.0.2.tar", last modified: Tue May 14 12:36:19 2024, max compression
+gzip compressed data, was "lucy01-0.1.0.tar", last modified: Wed May 15 14:22:24 2024, max compression
```

## Comparing `lucy01-0.0.2.tar` & `lucy01-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:36:19.452476 lucy01-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-14 12:36:19.452476 lucy01-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-14 12:36:15.000000 lucy01-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:36:19.448476 lucy01-0.0.2/lucy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:36:19.448476 lucy01-0.0.2/lucy/parser_/
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/parser_/atcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/parser_/contest.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/parser_/parser_.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/update_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-14 12:36:15.000000 lucy01-0.0.2/lucy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:36:19.452476 lucy01-0.0.2/lucy01.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-14 12:36:19.000000 lucy01-0.0.2/lucy01.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 12:36:19.000000 lucy01-0.0.2/lucy01.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:36:19.000000 lucy01-0.0.2/lucy01.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 12:36:19.000000 lucy01-0.0.2/lucy01.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 12:36:19.000000 lucy01-0.0.2/lucy01.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 12:36:19.000000 lucy01-0.0.2/lucy01.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 12:36:15.000000 lucy01-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:36:19.452476 lucy01-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:22:24.307439 lucy01-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-15 14:22:24.307439 lucy01-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-15 14:22:20.000000 lucy01-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:22:24.307439 lucy01-0.1.0/lucy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/dbx_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:22:24.307439 lucy01-0.1.0/lucy/parser_/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/parser_/atcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/parser_/contest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/parser_/parser_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/update_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-15 14:22:20.000000 lucy01-0.1.0/lucy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:22:24.307439 lucy01-0.1.0/lucy01.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-15 14:22:24.000000 lucy01-0.1.0/lucy01.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-15 14:22:24.000000 lucy01-0.1.0/lucy01.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:22:24.000000 lucy01-0.1.0/lucy01.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 14:22:24.000000 lucy01-0.1.0/lucy01.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 14:22:24.000000 lucy01-0.1.0/lucy01.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 14:22:24.000000 lucy01-0.1.0/lucy01.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-15 14:22:20.000000 lucy01-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:22:24.307439 lucy01-0.1.0/setup.cfg
```

### Comparing `lucy01-0.0.2/PKG-INFO` & `lucy01-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: lucy01
-Version: 0.0.2
+Version: 0.1.0
 Summary: CLI companion for CP.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: click
+Requires-Dist: dropbox
 Requires-Dist: lxml
+Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: selenium
 Provides-Extra: lint
 Requires-Dist: mypy; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: pylint[spelling]; extra == "lint"
 Requires-Dist: yapf; extra == "lint"
@@ -28,14 +30,15 @@
 
 ## Supported Platforms
 - [x] AtCoder
 - [ ] Codeforces
 
 ## Featues
 - [x] Fetch Sample Test Cases
+- [x] Fetch Hidden Test Cases (after the contest 🤪)
 - [x] Test Solution
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
```

### Comparing `lucy01-0.0.2/README.md` & `lucy01-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 ## Supported Platforms
 - [x] AtCoder
 - [ ] Codeforces
 
 ## Featues
 - [x] Fetch Sample Test Cases
+- [x] Fetch Hidden Test Cases (after the contest 🤪)
 - [x] Test Solution
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
```

### Comparing `lucy01-0.0.2/lucy/config.py` & `lucy01-0.1.0/lucy/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from enum import Enum
 import os
 
 import click
+import dotenv
+
+dotenv.load_dotenv()
 
 
 class Website(Enum):
     ATCODER = 1
 
     @staticmethod
     def from_string(website: str) -> Website:
@@ -29,27 +32,29 @@
 
 @dataclass
 class Config:
     WEBSITE_HOST = {Website.ATCODER: 'https://atcoder.jp'}
 
     LUCY_HOME = os.getenv('LUCY_HOME') or f'{os.getenv("HOME")}/.lucy'
     LUCY_HOME = os.path.abspath(LUCY_HOME)
-    os.makedirs(LUCY_HOME, exist_ok=True)
 
     SNIPPETS_DIR = f'{LUCY_HOME}/.vscode'
-    os.makedirs(SNIPPETS_DIR, exist_ok=True)
-    SNIPPETS_PATH = os.path.abspath(f'{SNIPPETS_DIR}/cp.code-snippets')
+    SNIPPETS_PATH = f'{SNIPPETS_DIR}/cp.code-snippets'
 
-    COMMONS_PATH = os.path.abspath(f'{LUCY_HOME}/common')
-    os.makedirs(COMMONS_PATH, exist_ok=True)
+    COMMONS_DIR = os.path.abspath(f'{LUCY_HOME}/common')
 
-    TEMPLATE_PATH = f'{COMMONS_PATH}/base.cpp'
-    if not os.path.exists(TEMPLATE_PATH):
-        with open(TEMPLATE_PATH, 'w+', encoding='utf-8'):
-            pass
+    TEMPLATE_PATH = f'{COMMONS_DIR}/base.cpp'
 
     CLI_WEBSITE_CHOICE = click.Choice(['atcoder'])
 
     IMPL_MAIN = 'main.cpp'
     IMPL_BIN = 'main'
 
     SAMPLES_DIR = 'tests'
+
+    # pylint: disable=line-too-long
+    DROPBOX_TOKEN = os.getenv(
+        'DROPBOX_TOKEN'
+    ) or 'sl.B1Rp-zCsGfT8Pd3K_LSV-CduAGyJrBbltWKlly2JvHDzRf3u9AG68md6obRbVyoygMgytF_2L5SYoLijtyQ99qsHH9d9r1SdomNlWZk7uyPTpN4TxhtvnRlbuEfXfpGPF285E61xlXNz'
+
+    ATCODER_TESTCASES_DROPBOX_LINK = 'https://www.dropbox.com/sh/nx3tnilzqz7df8a/AAAYlTq2tiEHl5hsESw6-yfLa?dl=0'
+    # pylint: enable=line-too-long
```

### Comparing `lucy01-0.0.2/lucy/scraper.py` & `lucy01-0.1.0/lucy/scraper.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.0.2/lucy/tester.py` & `lucy01-0.1.0/lucy/tester.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 from __future__ import annotations
-import os
 import subprocess
-from typing import Generator, Tuple
+from typing import Optional, Tuple
 
 import click
 
-from lucy import utils
-from lucy.config import SampleType, Website
+from lucy.config import Website
+from lucy.filesystem import LocalFS
 
 
 # pylint: disable=too-few-public-methods
 class Tester:
 
-    def __init__(self, website: Website, contest_id: str, task_id: str) -> None:
+    def __init__(self, website: Website, contest_id: str, task_id: str,
+                 test_id: Optional[int]) -> None:
         self.website = website
         self.contest_id = contest_id
         self.task_id = task_id
 
-        self.num_tests = len(
-            os.listdir(utils.get_sample_path(website, contest_id, task_id, SampleType.IN)))
+        self.num_tests = LocalFS.num_samples(website, contest_id, task_id)
 
-        self.impl_path = utils.get_impl_path(website, contest_id, task_id)
-        self.bin_path = utils.get_impl_path(website, contest_id, task_id, bin_=True)
+        self.test_ids: list[int] = list(range(self.num_tests))
+        if test_id is not None:
+            if test_id < 0 or test_id >= self.num_tests:
+                raise ValueError("Invalid `test_id`")
+            self.test_ids = [test_id]
+
+        self.impl_path = LocalFS.get_impl_path(website, contest_id, task_id)
+        self.bin_path = LocalFS.get_impl_path(website, contest_id, task_id, bin_=True)
 
     def __compile(self) -> None:
         subprocess.check_call(['g++', self.impl_path, '-o', self.bin_path])
 
-    @staticmethod
-    def __read(path: str) -> str:
-        with open(path) as f:  # pylint: disable=unspecified-encoding
-            return f.read()
-
-    def __tests(self) -> Generator[Tuple[str, str], None, None]:
-        for idx in range(self.num_tests):
-            in_path = utils.get_sample_path(self.website, self.contest_id, self.task_id,
-                                            SampleType.IN, idx)
-            out_path = utils.get_sample_path(self.website, self.contest_id, self.task_id,
-                                             SampleType.OUT, idx)
-            yield (Tester.__read(in_path), Tester.__read(out_path))
-
-    def __exec(self, in_txt: str, truth_txt: str) -> bool:
+    def __exec(self, in_txt: str, truth_txt: str) -> Tuple[bool, str]:
         with subprocess.Popen([self.bin_path], stdin=subprocess.PIPE,
                               stdout=subprocess.PIPE) as process:
             assert process.stdin
             process.stdin.write(in_txt.encode())
             process.stdin.close()
             assert process.stdout
             out_txt = process.stdout.read().decode()
             process.wait()
-        return out_txt.strip() == truth_txt.strip()
+        return out_txt.strip() == truth_txt.strip(), out_txt
 
-    def run(self) -> None:
+    def run(self, verbose: bool = False) -> None:
         self.__compile()
 
-        for i, (in_txt, out_txt) in enumerate(self.__tests()):
+        for i, (in_txt, truth_txt) in zip(
+                self.test_ids,
+                LocalFS.tests(self.website, self.contest_id, self.task_id, self.test_ids)):
             click.echo(f'Test#{i:02d}', nl=False)
             click.echo(f'{"." * 50}', nl=False)
-            passes = self.__exec(in_txt, out_txt)
+            passes, out_txt = self.__exec(in_txt, truth_txt)
             if passes:
                 click.secho('AC', bg='green')
             else:
                 click.secho('WA', bg='red')
+                if verbose:
+                    click.secho("Input:", bg='white', bold=True)
+                    print(in_txt.strip())
+                    click.secho("Output:", bg='red', bold=True)
+                    print(out_txt.strip())
+                    click.secho("Expected:", bg='green', bold=True)
+                    print(truth_txt.strip())
```

### Comparing `lucy01-0.0.2/lucy/update_snippets.py` & `lucy01-0.1.0/lucy/update_snippets.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.0.2/lucy01.egg-info/PKG-INFO` & `lucy01-0.1.0/lucy01.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: lucy01
-Version: 0.0.2
+Version: 0.1.0
 Summary: CLI companion for CP.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: click
+Requires-Dist: dropbox
 Requires-Dist: lxml
+Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: selenium
 Provides-Extra: lint
 Requires-Dist: mypy; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: pylint[spelling]; extra == "lint"
 Requires-Dist: yapf; extra == "lint"
@@ -28,14 +30,15 @@
 
 ## Supported Platforms
 - [x] AtCoder
 - [ ] Codeforces
 
 ## Featues
 - [x] Fetch Sample Test Cases
+- [x] Fetch Hidden Test Cases (after the contest 🤪)
 - [x] Test Solution
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
```

### Comparing `lucy01-0.0.2/pyproject.toml` & `lucy01-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [project]
 name = "lucy01"
-version = "0.0.2"
+version = "0.1.0"
 description = "CLI companion for CP."
 readme = "README.md"
 dependencies = [
     "bs4",
     "click",
+    "dropbox",
     "lxml",
+    "python-dotenv",
     "requests",
     "selenium",
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 lint = ["mypy", "pylint", "pylint[spelling]", "yapf"]
```

