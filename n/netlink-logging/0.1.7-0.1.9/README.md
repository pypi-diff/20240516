# Comparing `tmp/netlink-logging-0.1.7.tar.gz` & `tmp/netlink-logging-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-logging-0.1.7.tar", max compression
+gzip compressed data, was "netlink-logging-0.1.9.tar", max compression
```

## Comparing `netlink-logging-0.1.7.tar` & `netlink-logging-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1083 2022-03-08 08:32:23.896608 netlink-logging-0.1.7/LICENSE.md
--rw-r--r--   0        0        0      218 2022-03-08 08:56:56.980895 netlink-logging-0.1.7/netlink/logging/__init__.py
--rw-r--r--   0        0        0     1380 2022-06-14 09:54:19.619381 netlink-logging-0.1.7/netlink/logging/__init__.pyi
--rw-r--r--   0        0        0     3922 2022-08-19 13:25:39.607903 netlink-logging-0.1.7/netlink/logging/_logging.py
--rw-r--r--   0        0        0      824 2022-08-19 13:26:07.205480 netlink-logging-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4252 2022-06-29 08:01:43.991553 netlink-logging-0.1.7/README.md
--rw-r--r--   0        0        0     5159 2022-08-19 13:27:54.861919 netlink-logging-0.1.7/setup.py
--rw-r--r--   0        0        0     5117 2022-08-19 13:27:54.861919 netlink-logging-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-03-08 08:32:23.896608 netlink-logging-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0      218 2022-03-08 08:56:56.980895 netlink-logging-0.1.9/netlink/logging/__init__.py
+-rw-r--r--   0        0        0     1427 2022-08-22 11:30:52.366086 netlink-logging-0.1.9/netlink/logging/__init__.pyi
+-rw-r--r--   0        0        0     3992 2022-09-26 11:19:55.097947 netlink-logging-0.1.9/netlink/logging/_logging.py
+-rw-r--r--   0        0        0      824 2022-10-21 07:30:26.004055 netlink-logging-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4252 2022-06-29 08:01:43.991553 netlink-logging-0.1.9/README.md
+-rw-r--r--   0        0        0     5159 2022-10-21 14:39:31.072346 netlink-logging-0.1.9/setup.py
+-rw-r--r--   0        0        0     5117 2022-10-21 14:39:31.072346 netlink-logging-0.1.9/PKG-INFO
```

### Comparing `netlink-logging-0.1.7/LICENSE.md` & `netlink-logging-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netlink-logging-0.1.7/netlink/logging/__init__.pyi` & `netlink-logging-0.1.9/netlink/logging/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -39,7 +39,9 @@
         mode: str = "a",
         max_bytes: int = 100 * 1024 * 1024,
         backup_count: int = 5,
         encoding: str = "utf-8",
         log_level: Optional[int] = None,
         disable_stderr_logger: bool = False,
     ): ...
+    @staticmethod
+    def hide_location(): ...
```

### Comparing `netlink-logging-0.1.7/netlink/logging/_logging.py` & `netlink-logging-0.1.9/netlink/logging/_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,18 @@
 
 add_logging_level("success", SUCCESS)
 add_logging_level("verbose", VERBOSE)
 add_logging_level("trace", TRACE)
 
 logzero.loglevel(DEFAULT_LEVEL)
 logzero.formatter(logzero.LogFormatter(fmt=DEFAULT_MESSAGE_FORMAT, datefmt=DEFAULT_DATE_FORMAT, colors=DEFAULT_COLORS))
-path = pathlib.Path(__main__.__file__)
+try:
+    path = pathlib.Path(__main__.__file__)
+except AttributeError:
+    path = pathlib.Path('<input>')
 if path.stem == '__main__':
     path = path.parent
 
 
 def _default_file():
     logzero.logfile(
         filename="_input_.log" if path.stem == "<input>" else path.with_suffix(".log"),
```

### Comparing `netlink-logging-0.1.7/pyproject.toml` & `netlink-logging-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "netlink-logging"
-version = "0.1.7"
+version = "0.1.9"
 description = "A wrapper around logging and logzero"
 license = "MIT"
 authors = ["Bernhard Radermacher <bernhard.radermacher@netlink-consulting.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/netlink-consulting/netlink-logging"
 keywords = ["logging"]
 classifiers = ["Topic :: Software Development"]
 packages = [ { include = "netlink/logging" } ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 logzero = "^1.7.0"
-netlink-core = "^0.0.3"
+netlink-core = "^0.0.4"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pytest = "^7.0.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `netlink-logging-0.1.7/README.md` & `netlink-logging-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `netlink-logging-0.1.7/setup.py` & `netlink-logging-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['logging']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['logzero>=1.7.0,<2.0.0', 'netlink-core>=0.0.3,<0.0.4']
+['logzero>=1.7.0,<2.0.0', 'netlink-core>=0.0.4,<0.0.5']
 
 setup_kwargs = {
     'name': 'netlink-logging',
-    'version': '0.1.7',
+    'version': '0.1.9',
     'description': 'A wrapper around logging and logzero',
     'long_description': '# netlink-logging\n\n_Part of the NetLink Python Tools_\n\nA small wrapper around python logging and [logzero](https://logzero.readthedocs.io/en/latest/).\n\n## Features\n\n- Log to a logfile automatically (same name as the top-level script, `_input_` for console)\n- Additional levels:\n  - `TRACE` (`5`)\n  - `VERBOSE` (`15`)\n  - `SUCCESS` (`25`)\n- Timestamps are in UTC and use format `%Y-%m-%d %H:%M:%S`\n- Uncaught Exceptions are logged as `CRITICAL`\n\n## Installation\n\n```bash\npip install netlink-logging\n```\n\n## Usage\n\n```python\nfrom netlink.logging import logger \n\nlogger.trace(\'A TRACE entry.\')\nlogger.debug(\'A DEBUG entry.\')\nlogger.verbose(\'A VERBOSE entry.\')\nlogger.info(\'An INFO entry.\')\nlogger.success(\'A SUCCESS entry.\')\nlogger.warning(\'A WARNING entry.\')\nlogger.error(\'An ERROR entry.\')\nlogger.critical(\'A CRITICAL entry.\')\n```\n\nresults in\n\n``` \n[D 2022-02-32 26:27:28 <input>:…] A DEBUG entry.\n[V 2022-02-32 26:27:28 <input>:…] A VERBOSE entry.\n[I 2022-02-32 26:27:28 <input>:…] An INFO entry.\n[S 2022-02-32 26:27:28 <input>:…] A SUCCESS entry.\n[W 2022-02-32 26:27:28 <input>:…] A WARNING entry.\n[E 2022-02-32 26:27:28 <input>:…] An ERROR entry.\n[C 2022-02-32 26:27:28 <input>:…] A CRITICAL entry.\n```\n\n## Additional Methods\n\n### `set_file`\n\nUse `set_file` to change the file that is logged to:\n\n```\nlogger.set_file([filename, \n                [formatter,] \n                [mode,] \n                [max_bytes,] \n                [backup_count,] \n                [encoding,] \n                [log_level,] \n                [disable_stderr_logger]])\n```\n\n#### Parameters\n\n- **filename** (optional, `str`)\n\n  Must be provided, if any other parameter is provided. If not provided, or set to `None` logging to file is disabled.\n\n- **formatter** (optional, `logging.Formatter`)\n  \n  Formatter to use for logging to file. Defaults to `[K time module:line number] (message`, where \n  - **K** is the first letter of the logging level\n  - **time** is `%Y-%m-%d %H:%M:%S` in UTC\n  - **module** and **line number show the location in code\n  - **message** as provided in call\n\n- **mode** (optional, `str`)\n\n  Mode to open the file with. Defaults to `a`.\n\n- **max_bytes** (optional, `int`)\n  \n   Size of the logfile when rollover should occur. If set to `0`, rollover never occurs. Defaults to `100 MB`. \n\n- **backup_count** (optional, `int`)\n\n  Number of backups to keep. If set to 0, rollover never occurs. Defaults to `5`.\n\n- **encoding** (optional, `str`)\n \n  Used to open the file with that encoding. Defaults to `utf-8`.\n\n- **log_level** (optional, `int`)\n\n  Set a custom logging level for the file logger. Defaults to the current logging level.\n\n- **disable_stderr_logger** (optional, `bool`)\n\n  Should the default stderr logger be disabled. Defaults to `False`.\n\n\n### `set_level`\n\nThe current logging level can be set without additional imports:\n\n```python\nfrom netlink.logging import logger\n\nlogger.set_level(logger.ERROR)\n```\n\n### `enable_file`\n\nEnable logging to file, if it was disabled. Takes _boolean_.\n\n### `disable_file`\n\nDisable logging to file.\n\n\n## Roadmap\n\nAn additional feature that is considered would log **every** Exception raised.\n\n## License\n\n### MIT License\n\nCopyright (c) 2022 Bernhard Radermacher\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n',
     'author': 'Bernhard Radermacher',
     'author_email': 'bernhard.radermacher@netlink-consulting.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/netlink-consulting/netlink-logging',
```

### Comparing `netlink-logging-0.1.7/PKG-INFO` & `netlink-logging-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlink-logging
-Version: 0.1.7
+Version: 0.1.9
 Summary: A wrapper around logging and logzero
 Home-page: https://gitlab.com/netlink-consulting/netlink-logging
 License: MIT
 Keywords: logging
 Author: Bernhard Radermacher
 Author-email: bernhard.radermacher@netlink-consulting.com
 Requires-Python: >=3.7,<3.11
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Dist: logzero (>=1.7.0,<2.0.0)
-Requires-Dist: netlink-core (>=0.0.3,<0.0.4)
+Requires-Dist: netlink-core (>=0.0.4,<0.0.5)
 Project-URL: Repository, https://gitlab.com/netlink-consulting/netlink-logging
 Description-Content-Type: text/markdown
 
 # netlink-logging
 
 _Part of the NetLink Python Tools_
```

