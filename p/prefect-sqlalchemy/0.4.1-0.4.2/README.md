# Comparing `tmp/prefect_sqlalchemy-0.4.1.tar.gz` & `tmp/prefect_sqlalchemy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_sqlalchemy-0.4.1.tar", last modified: Thu Apr 25 16:19:29 2024, max compression
+gzip compressed data, was "prefect_sqlalchemy-0.4.2.tar", last modified: Fri Apr 26 15:04:37 2024, max compression
```

## Comparing `prefect_sqlalchemy-0.4.1.tar` & `prefect_sqlalchemy-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:19:29.052434 prefect_sqlalchemy-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-25 16:19:29.052434 prefect_sqlalchemy-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:19:29.044434 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    35914 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:19:29.048434 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-25 16:19:29.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 16:19:28.000000 prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:19:29.052434 prefect_sqlalchemy-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:19:29.048434 prefect_sqlalchemy-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    23372 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 16:19:16.000000 prefect_sqlalchemy-0.4.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:37.173594 prefect_sqlalchemy-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-26 15:04:37.173594 prefect_sqlalchemy-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:37.169594 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:36.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35914 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:37.169594 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-26 15:04:36.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-26 15:04:37.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:36.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 15:04:36.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-26 15:04:36.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:04:36.000000 prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:37.173594 prefect_sqlalchemy-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:37.169594 prefect_sqlalchemy-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23372 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-26 15:04:22.000000 prefect_sqlalchemy-0.4.2/tests/test_version.py
```

### Comparing `prefect_sqlalchemy-0.4.1/PKG-INFO` & `prefect_sqlalchemy-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-sqlalchemy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Prefect integrations for working with databases
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: sqlalchemy<3,>=1.4.31
 Requires-Dist: prefect>=2.13.5
 Provides-Extra: dev
 Requires-Dist: aiosqlite; extra == "dev"
 Requires-Dist: asyncpg; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.1 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.2 Summary: Prefect
 integrations for working with databases Author-email: "Prefect Technologies,
 Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Requires-Dist: sqlalchemy<3,>=1.4.31 Requires-Dist:
-prefect>=2.13.5 Provides-Extra: dev Requires-Dist: aiosqlite; extra == "dev"
-Requires-Dist: asyncpg; extra == "dev" Requires-Dist: coverage; extra == "dev"
-Requires-Dist: interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files;
-extra == "dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist:
-mkdocs; extra == "dev" Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev" Requires-Dist:
-mypy; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-
-commit; extra == "dev" Requires-Dist: psycopg2; extra == "dev" Requires-Dist:
-pytest-asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: pytest; extra == "dev" # prefect-sqlalchemy
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+sqlalchemy<3,>=1.4.31 Requires-Dist: prefect>=2.13.5 Provides-Extra: dev
+Requires-Dist: aiosqlite; extra == "dev" Requires-Dist: asyncpg; extra == "dev"
+Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
+"dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
+material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
+mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
+"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
+pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
+psycopg2; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist: pytest; extra ==
+"dev" # prefect-sqlalchemy
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                   _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to
 see additional examples and the API reference. The prefect-sqlalchemy
 collection makes it easy to connect to a database in your Prefect flows. Check
 out the examples below to get started! ## Getting started ### Integrate with
 Prefect flows Prefect and SQLAlchemy are a data powerhouse duo. With Prefect,
```

### Comparing `prefect_sqlalchemy-0.4.1/README.md` & `prefect_sqlalchemy-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/credentials.py` & `prefect_sqlalchemy-0.4.2/prefect_sqlalchemy/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.1/prefect_sqlalchemy/database.py` & `prefect_sqlalchemy-0.4.2/prefect_sqlalchemy/database.py`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/PKG-INFO` & `prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-sqlalchemy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Prefect integrations for working with databases
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: sqlalchemy<3,>=1.4.31
 Requires-Dist: prefect>=2.13.5
 Provides-Extra: dev
 Requires-Dist: aiosqlite; extra == "dev"
 Requires-Dist: asyncpg; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.1 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.2 Summary: Prefect
 integrations for working with databases Author-email: "Prefect Technologies,
 Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Requires-Dist: sqlalchemy<3,>=1.4.31 Requires-Dist:
-prefect>=2.13.5 Provides-Extra: dev Requires-Dist: aiosqlite; extra == "dev"
-Requires-Dist: asyncpg; extra == "dev" Requires-Dist: coverage; extra == "dev"
-Requires-Dist: interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files;
-extra == "dev" Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist:
-mkdocs; extra == "dev" Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev" Requires-Dist:
-mypy; extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-
-commit; extra == "dev" Requires-Dist: psycopg2; extra == "dev" Requires-Dist:
-pytest-asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: pytest; extra == "dev" # prefect-sqlalchemy
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+sqlalchemy<3,>=1.4.31 Requires-Dist: prefect>=2.13.5 Provides-Extra: dev
+Requires-Dist: aiosqlite; extra == "dev" Requires-Dist: asyncpg; extra == "dev"
+Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
+"dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
+material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
+mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
+"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
+pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
+psycopg2; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist: pytest; extra ==
+"dev" # prefect-sqlalchemy
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                   _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to
 see additional examples and the API reference. The prefect-sqlalchemy
 collection makes it easy to connect to a database in your Prefect flows. Check
 out the examples below to get started! ## Getting started ### Integrate with
 Prefect flows Prefect and SQLAlchemy are a data powerhouse duo. With Prefect,
```

### Comparing `prefect_sqlalchemy-0.4.1/prefect_sqlalchemy.egg-info/SOURCES.txt` & `prefect_sqlalchemy-0.4.2/prefect_sqlalchemy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 prefect_sqlalchemy/__init__.py
 prefect_sqlalchemy/_version.py
 prefect_sqlalchemy/credentials.py
 prefect_sqlalchemy/database.py
 prefect_sqlalchemy.egg-info/PKG-INFO
```

### Comparing `prefect_sqlalchemy-0.4.1/pyproject.toml` & `prefect_sqlalchemy-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.1/tests/conftest.py` & `prefect_sqlalchemy-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.1/tests/test_block_standards.py` & `prefect_sqlalchemy-0.4.2/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.1/tests/test_credentials.py` & `prefect_sqlalchemy-0.4.2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.1/tests/test_database.py` & `prefect_sqlalchemy-0.4.2/tests/test_database.py`

 * *Files identical despite different names*

