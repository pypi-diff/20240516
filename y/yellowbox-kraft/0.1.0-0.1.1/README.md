# Comparing `tmp/yellowbox_kraft-0.1.0.tar.gz` & `tmp/yellowbox_kraft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox_kraft-0.1.0.tar", max compression
+gzip compressed data, was "yellowbox_kraft-0.1.1.tar", max compression
```

## Comparing `yellowbox_kraft-0.1.0.tar` & `yellowbox_kraft-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-06-11 14:15:49.532845 yellowbox_kraft-0.1.0/LICENSE
--rw-r--r--   0        0        0     1645 2023-06-11 14:15:49.532845 yellowbox_kraft-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-06-11 14:15:49.536845 yellowbox_kraft-0.1.0/yellowbox_kraft/__init__.py
--rw-r--r--   0        0        0       22 2023-06-11 14:15:49.536845 yellowbox_kraft-0.1.0/yellowbox_kraft/_version.py
--rw-r--r--   0        0        0     3116 2023-06-11 14:15:49.536845 yellowbox_kraft-0.1.0/yellowbox_kraft/kraft.py
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 yellowbox_kraft-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-16 07:15:04.269822 yellowbox_kraft-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1857 2024-05-16 07:15:04.269822 yellowbox_kraft-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      139 2024-05-16 07:15:04.273822 yellowbox_kraft-0.1.1/yellowbox_kraft/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-16 07:15:16.721740 yellowbox_kraft-0.1.1/yellowbox_kraft/_version.py
+-rw-r--r--   0        0        0     4560 2024-05-16 07:15:04.273822 yellowbox_kraft-0.1.1/yellowbox_kraft/kraft.py
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 yellowbox_kraft-0.1.1/PKG-INFO
```

### Comparing `yellowbox_kraft-0.1.0/LICENSE` & `yellowbox_kraft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox_kraft-0.1.0/pyproject.toml` & `yellowbox_kraft-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 [tool.poetry]
 name = "yellowbox-kraft"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Biocatch LTD <serverteam@biocatch.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 yellowbox = { version = ">=0.8.0" }
-kafka-python = ">=2.0.2"
+# python 3.11 and lower use kafka-python, 3.12 and higher use confluent-kafka
+kafka-python = { version = "*", python="<3.12" }
+confluent-kafka = { version = "*", python=">=3.12" }
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.267"
+ruff = ">=0.0.267"
 pytest = "*"
 pytest-cov = "*"
 mypy = ">=1"
-black = "^23.3.0"
 pytest-asyncio = "^0.21.0"
+confluent-kafka = "^2.4.0"
 
 [tool.ruff]
+line-length = 120
+output-format = "full"
+[tool.ruff.lint]
 # https://beta.ruff.rs/docs/rules/
 select = ["I", "E", "W", "F", "N", "S", "BLE", "COM", "C4", "ISC", "ICN", "G", "PIE", "T20", "PYI", "Q", "SLF", "SIM",
     "ERA", "PGH", "PLC", "PLE", "PLR", "PLW", "RUF", "PT", "UP", "B"]
 ignore = [
+    "ISC001",  # handled by formatter
     "COM812", # trailing comma, handled by black
     "UP035", # deprecated imports
     "PLR0912", # Too many branches
     "S104", # Possible binding to all interfaces
 ]
-line-length = 120
-show-source = true
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 raises-require-match-for = []
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**" = [
     "PT013", # Found incorrect import of pytest, use simple `import pytest` instead
     "PT004", # Fixture does not return anything, add leading underscore
     "S101", # asserts
     "PLR2004", # PLR2004 Magic value used in comparison
     "PLR0913", # PLR0913 Too many arguments to function call
     "B011", # assert false
 ]
 
-[tool.ruff.pyupgrade]
+[tool.ruff.lint.pyupgrade]
 # Preserve types, even if a file imports `from __future__ import annotations`.
 keep-runtime-typing = true
 
-[tool.black]
-line-length = 120
-
 [tool.coverage.report]
 precision = 2
 exclude_lines = ["pragma: no cover", "raise NotImplementedError", "raise NotImplemented", "if TYPE_CHECKING:", "@overload"]
```

### Comparing `yellowbox_kraft-0.1.0/PKG-INFO` & `yellowbox_kraft-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: yellowbox-kraft
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Biocatch LTD
 Author-email: serverteam@biocatch.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kafka-python (>=2.0.2)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: confluent-kafka ; python_version >= "3.12"
+Requires-Dist: kafka-python ; python_version < "3.12"
 Requires-Dist: yellowbox (>=0.8.0)
```

