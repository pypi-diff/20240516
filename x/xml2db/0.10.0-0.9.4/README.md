# Comparing `tmp/xml2db-0.10.0.tar.gz` & `tmp/xml2db-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xml2db-0.10.0.tar", last modified: Thu May 16 16:28:10 2024, max compression
+gzip compressed data, was "xml2db-0.9.4.tar", last modified: Mon Apr 29 17:21:57 2024, max compression
```

## Comparing `xml2db-0.10.0.tar` & `xml2db-0.9.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:28:10.849695 xml2db-0.10.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 16:27:58.000000 xml2db-0.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-16 16:28:10.849695 xml2db-0.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-16 16:27:58.000000 xml2db-0.10.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-16 16:27:58.000000 xml2db-0.10.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:28:10.849695 xml2db-0.10.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:28:10.845695 xml2db-0.10.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:28:10.845695 xml2db-0.10.0/src/xml2db/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27840 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27773 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:28:10.849695 xml2db-0.10.0/src/xml2db/table/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/table/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/table/duplicated_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/table/relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/table/reused_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14388 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/table/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/table/transformed_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-05-16 16:27:58.000000 xml2db-0.10.0/src/xml2db/xml_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:28:10.849695 xml2db-0.10.0/src/xml2db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-16 16:28:10.000000 xml2db-0.10.0/src/xml2db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-16 16:28:10.000000 xml2db-0.10.0/src/xml2db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:28:10.000000 xml2db-0.10.0/src/xml2db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-16 16:28:10.000000 xml2db-0.10.0/src/xml2db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 16:28:10.000000 xml2db-0.10.0/src/xml2db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:28:10.849695 xml2db-0.10.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-16 16:27:58.000000 xml2db-0.10.0/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-16 16:27:58.000000 xml2db-0.10.0/tests/test_models_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-16 16:27:58.000000 xml2db-0.10.0/tests/test_roundtrip.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:21:57.543948 xml2db-0.9.4/
+-rw-rw-rw-   0        0        0     1100 2024-03-21 09:53:18.000000 xml2db-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0     3721 2024-04-29 17:21:57.390222 xml2db-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2024-03-21 08:22:04.000000 xml2db-0.9.4/README.md
+-rw-rw-rw-   0        0        0     1092 2024-03-21 08:52:06.000000 xml2db-0.9.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:21:57.544905 xml2db-0.9.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 17:21:54.919067 xml2db-0.9.4/src/
+-rw-rw-rw-   0        0        0      767 2023-10-24 14:26:10.000000 xml2db-0.9.4/src/debug.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:21:55.346423 xml2db-0.9.4/src/xml2db/
+-rw-rw-rw-   0        0        0      472 2023-09-05 08:57:47.000000 xml2db-0.9.4/src/xml2db/__init__.py
+-rw-rw-rw-   0        0        0    27793 2024-02-01 15:54:51.000000 xml2db-0.9.4/src/xml2db/document.py
+-rw-rw-rw-   0        0        0      137 2023-09-05 08:57:47.000000 xml2db-0.9.4/src/xml2db/exceptions.py
+-rw-rw-rw-   0        0        0    27733 2024-01-30 15:55:37.000000 xml2db-0.9.4/src/xml2db/model.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:21:56.578184 xml2db-0.9.4/src/xml2db/table/
+-rw-rw-rw-   0        0        0      239 2023-09-05 08:57:47.000000 xml2db-0.9.4/src/xml2db/table/__init__.py
+-rw-rw-rw-   0        0        0     7562 2024-02-01 15:54:51.000000 xml2db-0.9.4/src/xml2db/table/column.py
+-rw-rw-rw-   0        0        0     7386 2024-01-29 15:05:08.000000 xml2db-0.9.4/src/xml2db/table/duplicated_table.py
+-rw-rw-rw-   0        0        0     9538 2024-01-29 15:05:08.000000 xml2db-0.9.4/src/xml2db/table/relations.py
+-rw-rw-rw-   0        0        0     6661 2024-02-01 15:54:51.000000 xml2db-0.9.4/src/xml2db/table/reused_table.py
+-rw-rw-rw-   0        0        0    14744 2024-01-29 15:05:08.000000 xml2db-0.9.4/src/xml2db/table/table.py
+-rw-rw-rw-   0        0        0    13739 2023-10-25 15:34:10.000000 xml2db-0.9.4/src/xml2db/table/transformed_table.py
+-rw-rw-rw-   0        0        0    11670 2024-01-30 15:55:37.000000 xml2db-0.9.4/src/xml2db/xml_converter.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:21:57.226631 xml2db-0.9.4/src/xml2db.egg-info/
+-rw-rw-rw-   0        0        0     3721 2024-04-29 17:21:54.000000 xml2db-0.9.4/src/xml2db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2024-04-29 17:21:54.000000 xml2db-0.9.4/src/xml2db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:21:54.000000 xml2db-0.9.4/src/xml2db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2024-04-29 17:21:54.000000 xml2db-0.9.4/src/xml2db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 17:21:54.000000 xml2db-0.9.4/src/xml2db.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 17:21:56.951694 xml2db-0.9.4/tests/
+-rw-rw-rw-   0        0        0     2408 2023-10-04 13:19:21.000000 xml2db-0.9.4/tests/test_conversions.py
+-rw-rw-rw-   0        0        0     3275 2023-10-27 14:14:40.000000 xml2db-0.9.4/tests/test_roundtrip.py
```

### Comparing `xml2db-0.10.0/LICENSE` & `xml2db-0.9.4/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2024 Commission de régulation de l'énergie
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2024 Commission de régulation de l'énergie
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `xml2db-0.10.0/PKG-INFO` & `xml2db-0.9.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-Metadata-Version: 2.1
-Name: xml2db
-Version: 0.10.0
-Summary: Import complex XML files to a relational database
-Author-email: Commission de régulation de l'énergie <opensource@cre.fr>
-Project-URL: Documentation, https://cre-dev.github.io/xml2db
-Project-URL: Repository, https://github.com/cre-dev/xml2db
-Project-URL: Issues page, https://github.com/cre-dev/xml2db/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: sqlalchemy>1.4
-Requires-Dist: xmlschema==3.1.0
-Requires-Dist: lxml==5.1.0
-Provides-Extra: docs
-Requires-Dist: mkdocs-material==9.5.23; extra == "docs"
-Requires-Dist: mkdocstrings-python==1.10.2; extra == "docs"
-Provides-Extra: tests
-Requires-Dist: pytest>=7.0; extra == "tests"
-
-# Xml2db
-
-`xml2db` is a Python package which allows loading XML data into a relational database. It is designed to handle complex 
-schemas which cannot be easily denormalized to a flat table, without any custom code.
-
-It builds a data model (i.e. a set of database tables linked with foreign keys relationships) based on a XSD schema and
-allows parsing and loading XML files into the database, and get them back to XML, if needed.
-
-It is as simple as:
-
-```python
-from xml2db import DataModel
-
-# Create a data model of tables with relations based on the XSD file
-data_model = DataModel(
-    xsd_file="path/to/file.xsd", 
-    connection_string="postgresql+psycopg2://testuser:testuser@localhost:5432/testdb",
-)
-# Parse an XML file based on this XSD
-document = data_model.parse_xml(
-    xml_file="path/to/file.xml"
-)
-# Insert the document content into the database
-document.insert_into_target_tables()
-```
-
-The data model will adhere closely to the XSD schema, but `xml2db` will perform simplifications aimed at limiting the 
-complexity of the resulting data model and the storage footprint.
-
-The raw data loaded into the database can then be processed using [DBT](https://www.getdbt.com/), SQL views or 
-other tools aimed at extracting, correcting and formatting the data into more user-friendly tables.
-
-`xml2db` is developed and used at the [French energy regulation authority (CRE)](https://www.cre.fr/) to process XML 
-data.
-
-This package uses `sqlalchemy` to interact with the database, so it should work with different database backends. 
-Automated integration tests run against PostgreSQL, MySQL and MS SQL Server. `xml2db` does not work with SQLite. You may
-have to install additional packages to connect to your database (e.g. `psycopg2` for PostgreSQL, `pymysql` for MySQL or 
-`pyodbc` for MS SQL Server).
-
-**Please read the [package documentation website](https://cre-dev.github.io/xml2db) for all the details!**
-
-## Installation
-
-The package can be installed, preferably in a virtual environment, using `pip`:
-
-``` bash
-pip install xml2db
-```
-
-## Testing
-
-Running the tests requires installing additional development dependencies, after cloning the repo, with:
-
-```bash
-pip install -e .[tests,docs]
-```
-
-Run all tests with the following command:
-
-```bash
-python -m pytest
-```
-
-Integration tests require write access to a PostgreSQL or MS SQL Server database; the connection string is provided as an
-environment variable `DB_STRING`. If you want to run only conversion tests that do not require a database you can run:
-
-```bash
-pytest -m "not dbtest"
-`````
-
-## Contributing
-
-Contributions are more than welcome, as well as bug reports, starting with the project's 
-[issue page](https://github.com/cre-dev/xml2db/issues).
+Metadata-Version: 2.1
+Name: xml2db
+Version: 0.9.4
+Summary: Import complex XML files to a relational database
+Author-email: Commission de régulation de l'énergie <opensource@cre.fr>
+Project-URL: Documentation, https://cre-dev.github.io/xml2db
+Project-URL: Repository, https://github.com/cre-dev/xml2db
+Project-URL: Issues page, https://github.com/cre-dev/xml2db/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sqlalchemy>1.4
+Requires-Dist: xmlschema==3.1.0
+Requires-Dist: lxml==5.1.0
+Provides-Extra: docs
+Requires-Dist: mkdocs-material==9.5.14; extra == "docs"
+Requires-Dist: mkdocstrings[python]==0.24.1; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: pytest>=7.0; extra == "tests"
+
+# Xml2db
+
+`xml2db` is a Python package which allows loading XML data into a relational database. It is designed to handle complex 
+schemas which cannot be easily denormalized to a flat table, without any custom code.
+
+It builds a data model (i.e. a set of database tables linked with foreign keys relationships) based on a XSD schema and
+allows parsing and loading XML files into the database, and get them back to XML, if needed.
+
+It is as simple as:
+
+```python
+from xml2db import DataModel
+
+# Create a data model of tables with relations based on the XSD file
+data_model = DataModel(
+    xsd_file="path/to/file.xsd", 
+    connection_string="postgresql+psycopg2://testuser:testuser@localhost:5432/testdb",
+)
+# Parse an XML file based on this XSD
+document = data_model.parse_xml(
+    xml_file="path/to/file.xml"
+)
+# Insert the document content into the database
+document.insert_into_target_tables()
+```
+
+The data model will adhere closely to the XSD schema, but `xml2db` will perform simplifications aimed at limiting the 
+complexity of the resulting data model and the storage footprint.
+
+The raw data loaded into the database can then be processed using [DBT](https://www.getdbt.com/), SQL views or 
+other tools aimed at extracting, correcting and formatting the data into more user-friendly tables.
+
+`xml2db` is developed and used at the [French energy regulation authority (CRE)](https://www.cre.fr/) to process XML 
+data.
+
+This package uses `sqlalchemy` to interact with the database, so it should work with different database backends. It has
+been tested against PostgreSQL and MS SQL Server. It currently does not work with SQLite. You may have to install 
+additional packages to connect to your database (e.g. `pyodbc` which is the default connector for MS SQL Server, or 
+`psycopg2` for PostgreSQL).  
+
+**Please read the [package documentation website](https://cre-dev.github.io/xml2db) for all the details!**
+
+## Installation
+
+The package can be installed, preferably in a virtual environment, using `pip`:
+
+``` bash
+pip install xml2db
+```
+
+## Testing
+
+Running the tests requires installing additional development dependencies, after cloning the repo, with:
+
+```bash
+pip install -e .[tests,docs]
+```
+
+Run all tests with the following command:
+
+```bash
+python -m pytest
+```
+
+Integration tests require write access to a PostgreSQL or MS SQL Server database; the connection string is provided as an
+environment variable `DB_STRING`. If you want to run only conversion tests that do not require a database you can run:
+
+```bash
+pytest -m "not dbtest"
+`````
+
+## Contributing
+
+Contributions are more than welcome, as well as bug reports, starting with the project's 
+[issue page](https://github.com/cre-dev/xml2db/issues).
```

### Comparing `xml2db-0.10.0/README.md` & `xml2db-0.9.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-# Xml2db
-
-`xml2db` is a Python package which allows loading XML data into a relational database. It is designed to handle complex 
-schemas which cannot be easily denormalized to a flat table, without any custom code.
-
-It builds a data model (i.e. a set of database tables linked with foreign keys relationships) based on a XSD schema and
-allows parsing and loading XML files into the database, and get them back to XML, if needed.
-
-It is as simple as:
-
-```python
-from xml2db import DataModel
-
-# Create a data model of tables with relations based on the XSD file
-data_model = DataModel(
-    xsd_file="path/to/file.xsd", 
-    connection_string="postgresql+psycopg2://testuser:testuser@localhost:5432/testdb",
-)
-# Parse an XML file based on this XSD
-document = data_model.parse_xml(
-    xml_file="path/to/file.xml"
-)
-# Insert the document content into the database
-document.insert_into_target_tables()
-```
-
-The data model will adhere closely to the XSD schema, but `xml2db` will perform simplifications aimed at limiting the 
-complexity of the resulting data model and the storage footprint.
-
-The raw data loaded into the database can then be processed using [DBT](https://www.getdbt.com/), SQL views or 
-other tools aimed at extracting, correcting and formatting the data into more user-friendly tables.
-
-`xml2db` is developed and used at the [French energy regulation authority (CRE)](https://www.cre.fr/) to process XML 
-data.
-
-This package uses `sqlalchemy` to interact with the database, so it should work with different database backends. 
-Automated integration tests run against PostgreSQL, MySQL and MS SQL Server. `xml2db` does not work with SQLite. You may
-have to install additional packages to connect to your database (e.g. `psycopg2` for PostgreSQL, `pymysql` for MySQL or 
-`pyodbc` for MS SQL Server).
-
-**Please read the [package documentation website](https://cre-dev.github.io/xml2db) for all the details!**
-
-## Installation
-
-The package can be installed, preferably in a virtual environment, using `pip`:
-
-``` bash
-pip install xml2db
-```
-
-## Testing
-
-Running the tests requires installing additional development dependencies, after cloning the repo, with:
-
-```bash
-pip install -e .[tests,docs]
-```
-
-Run all tests with the following command:
-
-```bash
-python -m pytest
-```
-
-Integration tests require write access to a PostgreSQL or MS SQL Server database; the connection string is provided as an
-environment variable `DB_STRING`. If you want to run only conversion tests that do not require a database you can run:
-
-```bash
-pytest -m "not dbtest"
-`````
-
-## Contributing
-
-Contributions are more than welcome, as well as bug reports, starting with the project's 
-[issue page](https://github.com/cre-dev/xml2db/issues).
+# Xml2db
+
+`xml2db` is a Python package which allows loading XML data into a relational database. It is designed to handle complex 
+schemas which cannot be easily denormalized to a flat table, without any custom code.
+
+It builds a data model (i.e. a set of database tables linked with foreign keys relationships) based on a XSD schema and
+allows parsing and loading XML files into the database, and get them back to XML, if needed.
+
+It is as simple as:
+
+```python
+from xml2db import DataModel
+
+# Create a data model of tables with relations based on the XSD file
+data_model = DataModel(
+    xsd_file="path/to/file.xsd", 
+    connection_string="postgresql+psycopg2://testuser:testuser@localhost:5432/testdb",
+)
+# Parse an XML file based on this XSD
+document = data_model.parse_xml(
+    xml_file="path/to/file.xml"
+)
+# Insert the document content into the database
+document.insert_into_target_tables()
+```
+
+The data model will adhere closely to the XSD schema, but `xml2db` will perform simplifications aimed at limiting the 
+complexity of the resulting data model and the storage footprint.
+
+The raw data loaded into the database can then be processed using [DBT](https://www.getdbt.com/), SQL views or 
+other tools aimed at extracting, correcting and formatting the data into more user-friendly tables.
+
+`xml2db` is developed and used at the [French energy regulation authority (CRE)](https://www.cre.fr/) to process XML 
+data.
+
+This package uses `sqlalchemy` to interact with the database, so it should work with different database backends. It has
+been tested against PostgreSQL and MS SQL Server. It currently does not work with SQLite. You may have to install 
+additional packages to connect to your database (e.g. `pyodbc` which is the default connector for MS SQL Server, or 
+`psycopg2` for PostgreSQL).  
+
+**Please read the [package documentation website](https://cre-dev.github.io/xml2db) for all the details!**
+
+## Installation
+
+The package can be installed, preferably in a virtual environment, using `pip`:
+
+``` bash
+pip install xml2db
+```
+
+## Testing
+
+Running the tests requires installing additional development dependencies, after cloning the repo, with:
+
+```bash
+pip install -e .[tests,docs]
+```
+
+Run all tests with the following command:
+
+```bash
+python -m pytest
+```
+
+Integration tests require write access to a PostgreSQL or MS SQL Server database; the connection string is provided as an
+environment variable `DB_STRING`. If you want to run only conversion tests that do not require a database you can run:
+
+```bash
+pytest -m "not dbtest"
+`````
+
+## Contributing
+
+Contributions are more than welcome, as well as bug reports, starting with the project's 
+[issue page](https://github.com/cre-dev/xml2db/issues).
```

### Comparing `xml2db-0.10.0/pyproject.toml` & `xml2db-0.9.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "xml2db"
-version = "0.10.0"
-authors = [
-  { name="Commission de régulation de l'énergie", email="opensource@cre.fr" },
-]
-description = "Import complex XML files to a relational database"
-readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "sqlalchemy>1.4",
-    "xmlschema==3.1.0",
-    "lxml==5.1.0",
-]
-
-[project.optional-dependencies]
-docs = ["mkdocs-material==9.5.23", "mkdocstrings-python==1.10.2"]
-tests = ["pytest>=7.0"]
-
-[project.urls]
-"Documentation" = "https://cre-dev.github.io/xml2db"
-"Repository" = "https://github.com/cre-dev/xml2db"
-"Issues page" = "https://github.com/cre-dev/xml2db/issues"
-
-[tool.pytest.ini_options]
-markers = [
-    "dbtest: marks tests as integration tests requiring a database backend (deselect with '-m \"not dbtest\"')",
-]
-junit_family = "xunit2"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "xml2db"
+version = "0.9.4"
+authors = [
+  { name="Commission de régulation de l'énergie", email="opensource@cre.fr" },
+]
+description = "Import complex XML files to a relational database"
+readme = "README.md"
+requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "sqlalchemy>1.4",
+    "xmlschema==3.1.0",
+    "lxml==5.1.0",
+]
+
+[project.optional-dependencies]
+docs = ["mkdocs-material==9.5.14", "mkdocstrings[python]==0.24.1"]
+tests = ["pytest>=7.0"]
+
+[project.urls]
+"Documentation" = "https://cre-dev.github.io/xml2db"
+"Repository" = "https://github.com/cre-dev/xml2db"
+"Issues page" = "https://github.com/cre-dev/xml2db/issues"
+
+[tool.pytest.ini_options]
+markers = [
+    "dbtest: marks tests as integration tests requiring a database backend (deselect with '-m \"not dbtest\"')",
+]
+junit_family = "xunit2"
```

### Comparing `xml2db-0.10.0/src/xml2db/document.py` & `xml2db-0.9.4/src/xml2db/document.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,671 +1,653 @@
-import csv
-import datetime
-import logging
-import multiprocessing
-from hashlib import sha1
-from io import BytesIO
-from typing import Union, TYPE_CHECKING, Dict
-from zoneinfo import ZoneInfo
-from sqlalchemy import Column, Table, text, select
-from sqlalchemy.engine import Connection
-from sqlalchemy.sql.expression import TextClause
-from lxml import etree
-
-if TYPE_CHECKING:
-    from .model import DataModel
-
-from xml2db.exceptions import DataModelConfigError
-from xml2db.xml_converter import XMLConverter
-
-logger = logging.getLogger(__name__)
-
-
-class Document:
-    """A class to represent a single XML file with its data, based on a given XSD.
-
-    Based on a given DataModel object which represents the data model defined in the XSD, this class deals with \
-    the data itself. It allows parsing an XML file to extract the data into the data model format \
-     (performing the transforms defined in the DataModel object) and inserting the data into the database.
-
-    :param model: A `DataModel` object for this document
-    """
-
-    def __init__(self, model: "DataModel"):
-        self.model = model
-        self.data = {}
-        self.xml_file_path = None
-
-    def parse_xml(
-        self,
-        xml_file: Union[str, BytesIO],
-        xml_file_path: str = None,
-        skip_validation: bool = True,
-    ) -> None:
-        """Parse an XML document and apply transformation corresponding to the target data model
-
-        This method will first parse the XML file into a dict (document tree) using lxml
-        and then compute hash for all nodes based on their content, and finally convert
-        the document tree to tables data, creating primary keys and relations, ready to
-        be inserted in the database.
-
-        :param xml_file: the path or the file object of an XML file to parse
-        :param xml_file_path: path of the XML file, must be provided if 'xml_file' is provided as a file object \
-        (type 'BytesIO'), in order to fill the 'xml2db_input_file_path' column of the root table.
-        :param skip_validation: should we validate the document against the schema first? default to skip for \
-        backward compatibility
-        """
-        if type(xml_file) == BytesIO:
-            if xml_file_path is None:
-                error_message = (
-                    "If 'xml_file' is provided as a file object (type 'BytesIO') then 'xml_file_path' must be provided "
-                    "too in order to fill the 'xml2db_input_file_path' column of the root table."
-                )
-                logger.error(error_message)
-                raise ValueError(error_message)
-        self.xml_file_path = xml_file_path if xml_file_path is not None else xml_file
-
-        document_tree = self.model.xml_converter.parse_xml(
-            xml_file, self.xml_file_path, skip_validation
-        )
-
-        logger.info(f"Computing records hashes for {self.xml_file_path}")
-        self._compute_records_hashes(document_tree)
-
-        if "document_tree_hook" in self.model.model_config:
-            if not callable(self.model.model_config["document_tree_hook"]):
-                raise DataModelConfigError(
-                    "document_tree_hook provided in config must be callable"
-                )
-            logger.info(f"Running document_tree_hook function for {self.xml_file_path}")
-            document_tree = self.model.model_config["document_tree_hook"](document_tree)
-
-        logger.info(f"Adding records to data model for {self.xml_file_path}")
-        self.data = self.doc_tree_to_flat_data(document_tree)
-
-        logger.debug(self.__repr__())
-
-    def to_xml(
-        self, out_file: str = None, nsmap: dict = None, indent: str = "  "
-    ) -> etree.Element:
-        """Convert a document tree (nested dict) into an XML file
-
-        :param out_file: If provided, write output to a file.
-        :param nsmap: An optional namespace mapping.
-        :param indent: A string used as indentin XML output.
-        :return: The etree object corresponding to the root XML node.
-        """
-        converter = XMLConverter(self.model)
-        converter.document_tree = self.flat_data_to_doc_tree()
-        return converter.to_xml(out_file=out_file, nsmap=nsmap, indent=indent)
-
-    def _compute_records_hashes(self, node: Dict) -> bytes:
-        """Compute the hash of records recursively, taking into account children, for deduplication purpose.
-
-        :param node: a node of the parsed document tree
-        :return: the hash string representation of the node
-        """
-        if node is None:
-            return b""
-        h = sha1()
-        table = self.model.tables[node["type"]]
-        for field_type, name, _ in table.fields:
-            if field_type == "col":
-                h.update(str(node["content"].get(name, None)).encode("utf-8"))
-            elif field_type == "rel1":
-                h.update(
-                    self._compute_records_hashes(node["content"].get(name, [None])[0])
-                )
-            elif field_type == "reln":
-                h_children = [
-                    self._compute_records_hashes(v)
-                    for v in node["content"].get(name, [])
-                ]
-                for h_child in sorted(h_children):
-                    h.update(h_child)
-        node["record_hash"] = h.digest()
-        return node["record_hash"]
-
-    def doc_tree_to_flat_data(self, document_tree: dict) -> dict:
-        """Convert document tree (nested dict) to flat tables data model to prepare database import
-
-        :param document_tree: A nested dict which represents an XML document
-        :returns: A dict containing flat tables
-        """
-
-        def _extract_node(
-            node: Dict, pk_parent_node: int, row_number: int, data_model: dict
-        ) -> int:
-            """Extract nodes recursively
-
-            :param node: a dict containing a node of the document tree
-            :param pk_parent_node: the primary key of its parent node
-            :param data_model: the dict to write output to
-            :return: the primary key given to this node
-            """
-
-            # get the corresponding table model
-            model_table = self.model.tables[node["type"]]
-
-            # initialize data structure
-            if node["type"] not in data_model:
-                data_model[node["type"]] = {"next_pk": 1, "records": []}
-                if model_table.is_reused:
-                    data_model[node["type"]]["hashmap"] = {}
-                if any(
-                    [
-                        rel.other_table.is_reused
-                        for rel in model_table.relations_n.values()
-                    ]
-                ):
-                    data_model[node["type"]]["relations_n"] = {
-                        rel.rel_table_name: {"next_pk": 1, "records": []}
-                        for rel in model_table.relations_n.values()
-                        if rel.other_table.is_reused
-                    }
-            data = data_model[node["type"]]
-
-            hex_hash = str(node["record_hash"])
-
-            # if node is reused and a record with identical hash is already inserted, return its pk
-            if model_table.is_reused:
-                if hex_hash in data["hashmap"]:
-                    return data["hashmap"][hex_hash]
-
-            record = {}
-
-            # add pk
-            record_pk = data["next_pk"]
-            record[f"temp_pk_{model_table.name}"] = record_pk
-            data["next_pk"] += 1
-
-            # add parent pk if node is not reused
-            if not model_table.is_reused:
-                record[f"temp_fk_parent_{model_table.parent.name}"] = pk_parent_node
-                if self.model.model_config["row_numbers"]:
-                    record["xml2db_row_number"] = row_number
-
-            # build record from fields for columns and n-1 relations
-            for field_type, key, _ in model_table.fields:
-                if field_type == "col":
-                    if key in node["content"]:
-                        if model_table.columns[key].data_type in ["decimal", "float"]:
-                            val = [float(v) for v in node["content"][key]]
-                        elif model_table.columns[key].data_type == "integer":
-                            val = [int(v) for v in node["content"][key]]
-                        elif model_table.columns[key].data_type == "boolean":
-                            val = [
-                                v == "true" or v == "1" for v in node["content"][key]
-                            ]
-                        else:
-                            val = node["content"][key]
-
-                        if len(val) == 1:
-                            record[key] = val[0]
-                        else:
-                            esc_val = [str(v).replace('"', '\\"') for v in val]
-                            esc_val = [
-                                (
-                                    f'"{v}"'
-                                    if "," in v or "\n" in v or "\r" in v or '"' in v
-                                    else v
-                                )
-                                for v in esc_val
-                            ]
-                            record[key] = ",".join(esc_val)
-                    else:
-                        record[key] = None
-
-                elif field_type == "rel1":
-                    rel = model_table.relations_1[key]
-                    if key in node["content"]:
-                        record[f"temp_{rel.field_name}"] = _extract_node(
-                            node["content"][key][0],
-                            record_pk,
-                            0,
-                            data_model,
-                        )
-                    else:
-                        record[f"temp_{rel.field_name}"] = None
-
-            record["record_hash"] = bytes(node["record_hash"])
-
-            # add integration meta data if root table
-            if model_table.type_name == self.model.root_table:
-                record["xml2db_input_file_path"] = self.xml_file_path
-                record["xml2db_processed_at"] = self.model.processed_at
-
-            # add n-n relationship data for reused children nodes
-            for rel in model_table.relations_n.values():
-                if rel.name in node["content"]:
-                    if rel.other_table.is_reused:
-                        rel_data = data["relations_n"][rel.rel_table_name]
-                        i = 1
-                        for rel_child in node["content"][rel.name]:
-                            rel_row = {
-                                f"temp_fk_{model_table.name}": record_pk,
-                                f"temp_fk_{rel.other_table.name}": _extract_node(
-                                    rel_child,
-                                    record_pk,
-                                    i,
-                                    data_model,
-                                ),
-                            }
-                            if self.model.model_config["row_numbers"]:
-                                rel_row["xml2db_row_number"] = i
-                            rel_data["records"].append(rel_row)
-                            i += 1
-                    else:
-                        i = 1
-                        for rel_child in node["content"][rel.name]:
-                            _extract_node(rel_child, record_pk, i, data_model)
-                            i += 1
-
-            data["records"].append(record)
-
-            if model_table.is_reused:
-                data["hashmap"][hex_hash] = record_pk
-
-            return record_pk
-
-        flat_tables = {}
-        _extract_node(document_tree, 0, 0, flat_tables)
-
-        return flat_tables
-
-    def flat_data_to_doc_tree(self) -> dict:
-        """Convert the data stored in flat tables into a document tree (nested dict)
-
-        :return: The document tree (nested dict)
-        """
-        data_index = {}
-
-        # convert data to keyed dict for easier access
-        temp = (
-            ""
-            if f"pk_{self.model.tables[self.model.root_table].name}"
-            in self.data[self.model.root_table]["records"][0]
-            else "temp_"
-        )
-        for tb in self.model.tables.values():
-            data_index[tb.type_name] = {
-                "records": {},
-                "relations_n": {},
-            }
-            if tb.type_name in self.data:
-                data_index[tb.type_name]["records"] = {
-                    row[f"{temp}pk_{tb.name}"]: row
-                    for row in self.data[tb.type_name]["records"]
-                }
-            for rel in tb.relations_n.values():
-                index = {}
-                if rel.other_table.is_reused:
-                    if tb.type_name in self.data:
-                        for row in self.data[tb.type_name]["relations_n"][
-                            rel.rel_table_name
-                        ]["records"]:
-                            if row[f"{temp}fk_{tb.name}"] not in index:
-                                index[row[f"{temp}fk_{tb.name}"]] = []
-                            index[row[f"{temp}fk_{tb.name}"]].append(
-                                row[f"{temp}fk_{rel.other_table.name}"]
-                            )
-                else:
-                    if rel.other_table.type_name in self.data:
-                        for row in self.data[rel.other_table.type_name]["records"]:
-                            if row[f"{temp}fk_parent_{tb.name}"] not in index:
-                                index[row[f"{temp}fk_parent_{tb.name}"]] = []
-                            index[row[f"{temp}fk_parent_{tb.name}"]].append(
-                                row[f"{temp}pk_{rel.other_table.name}"]
-                            )
-                data_index[tb.type_name]["relations_n"][rel.rel_table_name] = index
-
-        def _build_node(node_type: str, node_pk: int) -> dict:
-            """Build a dict node recursively
-
-            :param node_type: The node type
-            :param node_pk: The node primary key
-            :return: A node as a dict
-            """
-            tb = self.model.tables[node_type]
-            node = {
-                "type": node_type,
-                "content": {},
-            }
-            record = data_index[node_type]["records"][node_pk]
-            for field_type, rel_name, rel in tb.fields:
-                if field_type == "col" and record[rel_name] is not None:
-                    if rel.data_type in [
-                        "decimal",
-                        "float",
-                    ]:  # remove trailing ".0" for decimal and float
-                        node["content"][rel_name] = [
-                            value.rstrip("0").rstrip(".") if "." in value else value
-                            for value in str(record[rel_name]).split(",")
-                        ]
-                    elif isinstance(record[rel_name], datetime.datetime):
-                        node["content"][rel_name] = [
-                            record[rel_name].isoformat(timespec="milliseconds")
-                        ]
-                    else:
-                        node["content"][rel_name] = (
-                            list(csv.reader([str(record[rel_name])], escapechar="\\"))[
-                                0
-                            ]
-                            if "," in str(record[rel_name])
-                            else [str(record[rel_name])]
-                        )
-                elif (
-                    field_type == "rel1"
-                    and record[f"{temp}{rel.field_name}"] is not None
-                ):
-                    node["content"][rel_name] = [
-                        _build_node(
-                            rel.other_table.type_name, record[f"{temp}{rel.field_name}"]
-                        )
-                    ]
-                elif (
-                    field_type == "reln"
-                    and node_pk
-                    in data_index[tb.type_name]["relations_n"][rel.rel_table_name]
-                ):
-                    node["content"][rel_name] = [
-                        _build_node(rel.other_table.type_name, pk)
-                        for pk in data_index[tb.type_name]["relations_n"][
-                            rel.rel_table_name
-                        ][node_pk]
-                    ]
-            return node
-
-        return _build_node(
-            self.model.root_table,
-            int(list(data_index[self.model.root_table]["records"].keys())[0]),
-        )
-
-    def insert_into_temp_tables(self) -> None:
-        """Insert data into temporary tables
-
-        (Re)creates temp tables before inserting data.
-        """
-        logger.info(f"Dropping temp tables if exist for {self.xml_file_path}")
-        self.model.drop_all_temp_tables()
-
-        logger.info(f"Creating temp tables for {self.xml_file_path}")
-        self.model.create_all_tables(temp=True)
-
-        logger.info(f"Inserting data into temporary tables from {self.xml_file_path}")
-        for tb in self.model.fk_ordered_tables:
-            for query, data in tb.get_insert_temp_records_statements(
-                self.data.get(tb.type_name, None)
-            ):
-                with self.model.engine.begin() as conn:
-                    conn.execute(query, data)
-
-    def merge_into_target_tables(self) -> int:
-        """Merge data into target data model
-
-        Execute all update and insert statements needed to merge temporary tables content \
-        into target tables, within a transaction.
-
-        :return: The number of inserted rows
-        """
-        inserted_rows_count = 0
-        with self.model.engine.begin() as conn:
-            for tb in self.model.fk_ordered_tables:
-                for query in tb.get_merge_temp_records_statements():
-                    result = conn.execute(query)
-                    if query.is_insert:
-                        inserted_rows_count += result.rowcount
-        if inserted_rows_count == 0:
-            logger.warning("No rows were inserted!")
-        else:
-            logger.info(f"Inserted rows: {inserted_rows_count}")
-
-        return inserted_rows_count
-
-    def insert_into_target_tables(
-        self,
-        db_semaphore: multiprocessing.Semaphore = None,
-    ) -> int:
-        """Insert and merge data into the database
-
-        Insert data into temporary tables and then merge temporary tables into target tables.
-
-        :param db_semaphore: An optional semaphore to avoid concurrent access to the database. When provided, it will \
-            ensure that only one merging operation at a time is performed.
-        :return: The number of inserted rows
-        """
-        try:
-            self.model.create_db_schema()
-            self.insert_into_temp_tables()
-        except Exception as e:
-            logger.error(
-                f"Error while importing into temporary tables from {self.xml_file_path}"
-            )
-            logger.error(e)
-            raise
-        else:
-            logger.info(
-                f"Merging temporary tables into target tables for {self.xml_file_path}"
-            )
-            if db_semaphore is not None:
-                db_semaphore.acquire()
-            try:
-                self.model.create_all_tables()  # Create target tables if not exist
-                inserted_rows = self.merge_into_target_tables()
-            except Exception as e:
-                logger.error(
-                    f"Error while merging temporary tables into target tables for {self.xml_file_path}"
-                )
-                logger.error(e)
-                raise
-            finally:
-                if db_semaphore is not None:
-                    db_semaphore.release()
-        finally:
-            logger.info(f"Dropping temporary tables for {self.xml_file_path}")
-            self.model.drop_all_temp_tables()
-
-        return inserted_rows
-
-    def extract_from_database(
-        self,
-        root_table_name: str,
-        root_select_where: str,
-        force_tz: Union[str, None] = None,
-    ) -> dict:
-        """Extract a subtree from the database and store it in a flat format
-
-        :param root_table_name: The root table name to start from
-        :param root_select_where: A where clause to apply to this root table
-        :param force_tz: Apply this timezone if database returns timezone-naïve datetime
-        :return: A shallow dict of flat data tables
-        """
-
-        if force_tz:
-            force_tz = ZoneInfo(force_tz)
-
-        def _fetch_data(
-            sqla_table: Table,
-            key_column: Column,
-            join_sequence: list[tuple[Column, Table, Column]],
-            top_where_clause: TextClause,
-            order_by: Union[None, tuple[Column]],
-            append_to: list,
-            conn: Connection,
-        ):
-            """Fetch data from a specific table and write fetched rows in a dict keyed by the first row column"""
-            quer = select(*(sqla_table.columns.values()))
-
-            join_sequence = join_sequence.copy()
-            if len(join_sequence) > 0:
-                left_col, join_tb, right_col = join_sequence.pop()
-                sub_quer = select(right_col)
-                prev_join_col = left_col
-                for left_col, join_tb, right_col in reversed(join_sequence):
-                    sub_quer = sub_quer.join(join_tb, right_col == prev_join_col)
-                    prev_join_col = left_col
-                sub_quer = sub_quer.where(top_where_clause)
-                quer = quer.where(key_column.in_(sub_quer))
-            else:
-                quer = quer.where(top_where_clause)
-
-            if order_by:
-                quer = quer.order_by(*order_by)
-
-            def add_tz(x):
-                if (
-                    force_tz
-                    and isinstance(x, datetime.datetime)
-                    and (x.tzinfo is None or x.tzinfo.utcoffset(x) is None)
-                ):
-                    x = x.replace(tzinfo=force_tz)
-                return x
-
-            col_names = sqla_table.columns.keys()
-            for row in conn.execute(quer):
-                append_to.append({key: add_tz(val) for key, val in zip(col_names, row)})
-
-        def _do_extract_table(
-            tb,
-            top_where_clause,
-            parent_table,
-            join_sequence,
-            res_dict,
-            conn,
-        ):
-            """Fetch tables and relationship tables recursively"""
-            if tb.type_name not in res_dict:
-                res_dict[tb.type_name] = {"records": []}
-            _fetch_data(
-                tb.table,
-                (
-                    getattr(tb.table.c, f"pk_{tb.name}")
-                    if tb.is_reused
-                    else getattr(tb.table.c, f"fk_parent_{parent_table.name}")
-                ),
-                join_sequence,
-                top_where_clause,
-                (
-                    None
-                    if tb.is_reused or not tb.data_model.model_config["row_numbers"]
-                    else (
-                        getattr(tb.table.c, f"fk_parent_{parent_table.name}"),
-                        tb.table.c.xml2db_row_number,
-                    )
-                ),
-                res_dict[tb.type_name]["records"],
-                conn,
-            )
-            join_root = (
-                [(None, tb.table, getattr(tb.table.c, f"pk_{tb.name}"))]
-                if parent_table is None
-                else []
-            )
-            if len(tb.relations_n) > 0:
-                if "relations_n" not in res_dict[tb.type_name]:
-                    res_dict[tb.type_name]["relations_n"] = {}
-                for rel in tb.relations_n.values():
-                    if rel.rel_table_name not in res_dict[tb.type_name]["relations_n"]:
-                        res_dict[tb.type_name]["relations_n"][rel.rel_table_name] = {
-                            "records": []
-                        }
-                    new_join = []
-                    if not tb.is_reused:
-                        new_join = [
-                            (
-                                getattr(tb.table.c, f"fk_parent_{parent_table.name}"),
-                                tb.table,
-                                getattr(tb.table.c, f"pk_{tb.table.name}"),
-                            )
-                        ]
-                    if rel.other_table.is_reused:
-                        _fetch_data(
-                            rel.rel_table,
-                            getattr(rel.rel_table.c, f"fk_{tb.name}"),
-                            join_sequence + join_root + new_join,
-                            top_where_clause,
-                            (
-                                (
-                                    getattr(rel.rel_table.c, f"fk_{tb.name}"),
-                                    rel.rel_table.c.xml2db_row_number,
-                                )
-                                if tb.data_model.model_config["row_numbers"]
-                                else None
-                            ),
-                            res_dict[tb.type_name]["relations_n"][rel.rel_table_name][
-                                "records"
-                            ],
-                            conn,
-                        )
-                        new_join = new_join + [
-                            (
-                                getattr(rel.rel_table.c, f"fk_{tb.name}"),
-                                rel.rel_table,
-                                getattr(rel.rel_table.c, f"fk_{rel.other_table.name}"),
-                            )
-                        ]
-                    _do_extract_table(
-                        rel.other_table,
-                        top_where_clause,
-                        tb,
-                        join_sequence + join_root + new_join,
-                        res_dict,
-                        conn,
-                    )
-            for rel in tb.relations_1.values():
-                _do_extract_table(
-                    rel.other_table,
-                    top_where_clause,
-                    tb,
-                    join_sequence
-                    + [
-                        (
-                            getattr(
-                                tb.table.c,
-                                (
-                                    f"pk_{tb.name}"
-                                    if tb.is_reused
-                                    else f"fk_parent_{parent_table.name}"
-                                ),
-                            ),
-                            tb.table,
-                            getattr(tb.table.c, f"{rel.field_name}"),
-                        )
-                    ],
-                    res_dict,
-                    conn,
-                )
-
-        flat_tables = {}
-
-        with self.model.engine.connect() as conn:
-            _do_extract_table(
-                self.model.tables[root_table_name],
-                text(root_select_where),
-                None,
-                [],
-                flat_tables,
-                conn,
-            )
-
-        self.data = flat_tables
-        return flat_tables
-
-    def __repr__(self) -> str:
-        """Output a repr string for the current document with records count"""
-        settings = (
-            f"temp_prefix: {self.model.temp_prefix}, db_schema: {self.model.db_schema}"
-        )
-        if not self.data:
-            return f"Empty {self.model.data_flow_name} document ({settings})"
-        else:
-            n = sum([len(v["records"]) for v in self.data.values()])
-            return "\n".join(
-                [
-                    f"Parsed {self.xml_file_path} into a {self.model.data_flow_name} document: {n} records",
-                    f"({settings})",
-                ]
-                + [
-                    f"   {self.model.tables[k].name}: {len(v['records'])}"
-                    for k, v in self.data.items()
-                ]
-            )
+import csv
+import datetime
+import logging
+import multiprocessing
+from hashlib import sha1
+from io import BytesIO
+from typing import Union, TYPE_CHECKING, Dict
+
+from sqlalchemy import Column, Table, text, select
+from sqlalchemy.engine import Connection
+from sqlalchemy.sql.expression import TextClause
+from lxml import etree
+
+if TYPE_CHECKING:
+    from .model import DataModel
+
+from xml2db.exceptions import DataModelConfigError
+from xml2db.xml_converter import XMLConverter
+
+logger = logging.getLogger(__name__)
+
+
+class Document:
+    """A class to represent a single XML file with its data, based on a given XSD.
+
+    Based on a given DataModel object which represents the data model defined in the XSD, this class deals with \
+    the data itself. It allows parsing an XML file to extract the data into the data model format \
+     (performing the transforms defined in the DataModel object) and inserting the data into the database.
+
+    :param model: A `DataModel` object for this document
+    """
+
+    def __init__(self, model: "DataModel"):
+        self.model = model
+        self.data = {}
+        self.xml_file_path = None
+
+    def parse_xml(
+        self,
+        xml_file: Union[str, BytesIO],
+        xml_file_path: str = None,
+        skip_validation: bool = True,
+    ) -> None:
+        """Parse an XML document and apply transformation corresponding to the target data model
+
+        This method will first parse the XML file into a dict (document tree) using lxml
+        and then compute hash for all nodes based on their content, and finally convert
+        the document tree to tables data, creating primary keys and relations, ready to
+        be inserted in the database.
+
+        :param xml_file: the path or the file object of an XML file to parse
+        :param xml_file_path: path of the XML file, must be provided if 'xml_file' is provided as a file object \
+        (type 'BytesIO'), in order to fill the 'xml2db_input_file_path' column of the root table.
+        :param skip_validation: should we validate the document against the schema first? default to skip for \
+        backward compatibility
+        """
+        if type(xml_file) == BytesIO:
+            if xml_file_path is None:
+                error_message = (
+                    "If 'xml_file' is provided as a file object (type 'BytesIO') then 'xml_file_path' must be provided "
+                    "too in order to fill the 'xml2db_input_file_path' column of the root table."
+                )
+                logger.error(error_message)
+                raise ValueError(error_message)
+        self.xml_file_path = xml_file_path if xml_file_path is not None else xml_file
+
+        document_tree = self.model.xml_converter.parse_xml(
+            xml_file, self.xml_file_path, skip_validation
+        )
+
+        logger.info(f"Computing records hashes for {self.xml_file_path}")
+        self._compute_records_hashes(document_tree)
+
+        if "document_tree_hook" in self.model.model_config:
+            if not callable(self.model.model_config["document_tree_hook"]):
+                raise DataModelConfigError(
+                    "document_tree_hook provided in config must be callable"
+                )
+            logger.info(f"Running document_tree_hook function for {self.xml_file_path}")
+            document_tree = self.model.model_config["document_tree_hook"](document_tree)
+
+        logger.info(f"Adding records to data model for {self.xml_file_path}")
+        self.data = self.doc_tree_to_flat_data(document_tree)
+
+        logger.debug(self.__repr__())
+
+    def to_xml(
+        self, out_file: str = None, nsmap: dict = None, indent: str = "  "
+    ) -> etree.Element:
+        """Convert a document tree (nested dict) into an XML file
+
+        :param out_file: If provided, write output to a file.
+        :param nsmap: An optional namespace mapping.
+        :param indent: A string used as indentin XML output.
+        :return: The etree object corresponding to the root XML node.
+        """
+        converter = XMLConverter(self.model)
+        converter.document_tree = self.flat_data_to_doc_tree()
+        return converter.to_xml(out_file=out_file, nsmap=nsmap, indent=indent)
+
+    def _compute_records_hashes(self, node: Dict) -> bytes:
+        """Compute the hash of records recursively, taking into account children, for deduplication purpose.
+
+        :param node: a node of the parsed document tree
+        :return: the hash string representation of the node
+        """
+        if node is None:
+            return b""
+        h = sha1()
+        table = self.model.tables[node["type"]]
+        for field_type, name, _ in table.fields:
+            if field_type == "col":
+                h.update(str(node["content"].get(name, None)).encode("utf-8"))
+            elif field_type == "rel1":
+                h.update(
+                    self._compute_records_hashes(node["content"].get(name, [None])[0])
+                )
+            elif field_type == "reln":
+                h_children = [
+                    self._compute_records_hashes(v)
+                    for v in node["content"].get(name, [])
+                ]
+                for h_child in sorted(h_children):
+                    h.update(h_child)
+        node["record_hash"] = h.digest()
+        return node["record_hash"]
+
+    def doc_tree_to_flat_data(self, document_tree: dict) -> dict:
+        """Convert document tree (nested dict) to flat tables data model to prepare database import
+
+        :param document_tree: A nested dict which represents an XML document
+        :returns: A dict containing flat tables
+        """
+
+        def _extract_node(
+            node: Dict, pk_parent_node: int, row_number: int, data_model: dict
+        ) -> int:
+            """Extract nodes recursively
+
+            :param node: a dict containing a node of the document tree
+            :param pk_parent_node: the primary key of its parent node
+            :param data_model: the dict to write output to
+            :return: the primary key given to this node
+            """
+
+            # get the corresponding table model
+            model_table = self.model.tables[node["type"]]
+
+            # initialize data structure
+            if node["type"] not in data_model:
+                data_model[node["type"]] = {"next_pk": 1, "records": []}
+                if model_table.is_reused:
+                    data_model[node["type"]]["hashmap"] = {}
+                if any(
+                    [
+                        rel.other_table.is_reused
+                        for rel in model_table.relations_n.values()
+                    ]
+                ):
+                    data_model[node["type"]]["relations_n"] = {
+                        rel.rel_table_name: {"next_pk": 1, "records": []}
+                        for rel in model_table.relations_n.values()
+                        if rel.other_table.is_reused
+                    }
+            data = data_model[node["type"]]
+
+            hex_hash = str(node["record_hash"])
+
+            # if node is reused and a record with identical hash is already inserted, return its pk
+            if model_table.is_reused:
+                if hex_hash in data["hashmap"]:
+                    return data["hashmap"][hex_hash]
+
+            record = {}
+
+            # add pk
+            record_pk = data["next_pk"]
+            record[f"temp_pk_{model_table.name}"] = record_pk
+            data["next_pk"] += 1
+
+            # add parent pk if node is not reused
+            if not model_table.is_reused:
+                record[f"temp_fk_parent_{model_table.parent.name}"] = pk_parent_node
+                if self.model.model_config["row_numbers"]:
+                    record["xml2db_row_number"] = row_number
+
+            # build record from fields for columns and n-1 relations
+            for field_type, key, _ in model_table.fields:
+                if field_type == "col":
+                    if key in node["content"]:
+                        if model_table.columns[key].data_type in ["decimal", "float"]:
+                            val = [float(v) for v in node["content"][key]]
+                        elif model_table.columns[key].data_type == "integer":
+                            val = [int(v) for v in node["content"][key]]
+                        elif model_table.columns[key].data_type == "boolean":
+                            val = [
+                                v == "true" or v == "1" for v in node["content"][key]
+                            ]
+                        else:
+                            val = node["content"][key]
+
+                        if len(val) == 1:
+                            record[key] = val[0]
+                        else:
+                            esc_val = [str(v).replace('"', '\\"') for v in val]
+                            esc_val = [
+                                f'"{v}"'
+                                if "," in v or "\n" in v or "\r" in v or '"' in v
+                                else v
+                                for v in esc_val
+                            ]
+                            record[key] = ",".join(esc_val)
+                    else:
+                        record[key] = None
+
+                elif field_type == "rel1":
+                    rel = model_table.relations_1[key]
+                    if key in node["content"]:
+                        record[f"temp_{rel.field_name}"] = _extract_node(
+                            node["content"][key][0],
+                            record_pk,
+                            0,
+                            data_model,
+                        )
+                    else:
+                        record[f"temp_{rel.field_name}"] = None
+
+            record["record_hash"] = bytes(node["record_hash"])
+
+            # add integration meta data if root table
+            if model_table.type_name == self.model.root_table:
+                record["xml2db_input_file_path"] = self.xml_file_path
+                record["xml2db_processed_at"] = self.model.processed_at
+
+            # add n-n relationship data for reused children nodes
+            for rel in model_table.relations_n.values():
+                if rel.name in node["content"]:
+                    if rel.other_table.is_reused:
+                        rel_data = data["relations_n"][rel.rel_table_name]
+                        i = 1
+                        for rel_child in node["content"][rel.name]:
+                            rel_row = {
+                                f"temp_fk_{model_table.name}": record_pk,
+                                f"temp_fk_{rel.other_table.name}": _extract_node(
+                                    rel_child,
+                                    record_pk,
+                                    i,
+                                    data_model,
+                                ),
+                            }
+                            if self.model.model_config["row_numbers"]:
+                                rel_row["xml2db_row_number"] = i
+                            rel_data["records"].append(rel_row)
+                            i += 1
+                    else:
+                        i = 1
+                        for rel_child in node["content"][rel.name]:
+                            _extract_node(rel_child, record_pk, i, data_model)
+                            i += 1
+
+            data["records"].append(record)
+
+            if model_table.is_reused:
+                data["hashmap"][hex_hash] = record_pk
+
+            return record_pk
+
+        flat_tables = {}
+        _extract_node(document_tree, 0, 0, flat_tables)
+
+        return flat_tables
+
+    def flat_data_to_doc_tree(self) -> dict:
+        """Convert the data stored in flat tables into a document tree (nested dict)
+
+        :return: The document tree (nested dict)
+        """
+        data_index = {}
+
+        # convert data to keyed dict for easier access
+        temp = (
+            ""
+            if f"pk_{self.model.tables[self.model.root_table].name}"
+            in self.data[self.model.root_table]["records"][0]
+            else "temp_"
+        )
+        for tb in self.model.tables.values():
+            data_index[tb.type_name] = {
+                "records": {},
+                "relations_n": {},
+            }
+            if tb.type_name in self.data:
+                data_index[tb.type_name]["records"] = {
+                    row[f"{temp}pk_{tb.name}"]: row
+                    for row in self.data[tb.type_name]["records"]
+                }
+            for rel in tb.relations_n.values():
+                index = {}
+                if rel.other_table.is_reused:
+                    if tb.type_name in self.data:
+                        for row in self.data[tb.type_name]["relations_n"][
+                            rel.rel_table_name
+                        ]["records"]:
+                            if row[f"{temp}fk_{tb.name}"] not in index:
+                                index[row[f"{temp}fk_{tb.name}"]] = []
+                            index[row[f"{temp}fk_{tb.name}"]].append(
+                                row[f"{temp}fk_{rel.other_table.name}"]
+                            )
+                else:
+                    if rel.other_table.type_name in self.data:
+                        for row in self.data[rel.other_table.type_name]["records"]:
+                            if row[f"{temp}fk_parent_{tb.name}"] not in index:
+                                index[row[f"{temp}fk_parent_{tb.name}"]] = []
+                            index[row[f"{temp}fk_parent_{tb.name}"]].append(
+                                row[f"{temp}pk_{rel.other_table.name}"]
+                            )
+                data_index[tb.type_name]["relations_n"][rel.rel_table_name] = index
+
+        def _build_node(node_type: str, node_pk: int) -> dict:
+            """Build a dict node recursively
+
+            :param node_type: The node type
+            :param node_pk: The node primary key
+            :return: A node as a dict
+            """
+            tb = self.model.tables[node_type]
+            node = {
+                "type": node_type,
+                "content": {},
+            }
+            record = data_index[node_type]["records"][node_pk]
+            for field_type, rel_name, rel in tb.fields:
+                if field_type == "col" and record[rel_name] is not None:
+                    if rel.data_type in [
+                        "decimal",
+                        "float",
+                    ]:  # remove trailing ".0" for decimal and float
+                        node["content"][rel_name] = [
+                            value.rstrip("0").rstrip(".") if "." in value else value
+                            for value in str(record[rel_name]).split(",")
+                        ]
+                    elif isinstance(record[rel_name], datetime.datetime):
+                        node["content"][rel_name] = [
+                            record[rel_name].isoformat(timespec="milliseconds")
+                        ]
+                    else:
+                        node["content"][rel_name] = (
+                            list(csv.reader([str(record[rel_name])], escapechar="\\"))[
+                                0
+                            ]
+                            if "," in str(record[rel_name])
+                            else [str(record[rel_name])]
+                        )
+                elif (
+                    field_type == "rel1"
+                    and record[f"{temp}{rel.field_name}"] is not None
+                ):
+                    node["content"][rel_name] = [
+                        _build_node(
+                            rel.other_table.type_name, record[f"{temp}{rel.field_name}"]
+                        )
+                    ]
+                elif (
+                    field_type == "reln"
+                    and node_pk
+                    in data_index[tb.type_name]["relations_n"][rel.rel_table_name]
+                ):
+                    node["content"][rel_name] = [
+                        _build_node(rel.other_table.type_name, pk)
+                        for pk in data_index[tb.type_name]["relations_n"][
+                            rel.rel_table_name
+                        ][node_pk]
+                    ]
+            return node
+
+        return _build_node(
+            self.model.root_table,
+            int(list(data_index[self.model.root_table]["records"].keys())[0]),
+        )
+
+    def insert_into_temp_tables(self) -> None:
+        """Insert data into temporary tables
+
+        (Re)creates temp tables before inserting data.
+        """
+        logger.info(f"Dropping temp tables if exist for {self.xml_file_path}")
+        self.model.drop_all_temp_tables()
+
+        logger.info(f"Creating temp tables for {self.xml_file_path}")
+        self.model.create_all_tables(temp=True)
+
+        logger.info(f"Inserting data into temporary tables from {self.xml_file_path}")
+        for tb in self.model.fk_ordered_tables:
+            for query, data in tb.get_insert_temp_records_statements(
+                self.data.get(tb.type_name, None)
+            ):
+                with self.model.engine.begin() as conn:
+                    conn.execute(query, data)
+
+    def merge_into_target_tables(self) -> int:
+        """Merge data into target data model
+
+        Execute all update and insert statements needed to merge temporary tables content \
+        into target tables, within a transaction.
+
+        :return: The number of inserted rows
+        """
+        inserted_rows_count = 0
+        with self.model.engine.begin() as conn:
+            for tb in self.model.fk_ordered_tables:
+                for query in tb.get_merge_temp_records_statements():
+                    result = conn.execute(query)
+                    if query.is_insert:
+                        inserted_rows_count += result.rowcount
+        if inserted_rows_count == 0:
+            logger.warning("No rows were inserted!")
+        else:
+            logger.info(f"Inserted rows: {inserted_rows_count}")
+
+        return inserted_rows_count
+
+    def insert_into_target_tables(
+        self,
+        db_semaphore: multiprocessing.Semaphore = None,
+    ) -> int:
+        """Insert and merge data into the database
+
+        Insert data into temporary tables and then merge temporary tables into target tables.
+
+        :param db_semaphore: An optional semaphore to avoid concurrent access to the database. When provided, it will \
+            ensure that only one merging operation at a time is performed.
+        :return: The number of inserted rows
+        """
+        try:
+            self.model.create_db_schema()
+            self.insert_into_temp_tables()
+        except Exception as e:
+            logger.error(
+                f"Error while importing into temporary tables from {self.xml_file_path}"
+            )
+            logger.error(e)
+            raise
+        else:
+            logger.info(
+                f"Merging temporary tables into target tables for {self.xml_file_path}"
+            )
+            if db_semaphore is not None:
+                db_semaphore.acquire()
+            try:
+                self.model.create_all_tables()  # Create target tables if not exist
+                inserted_rows = self.merge_into_target_tables()
+            except Exception as e:
+                logger.error(
+                    f"Error while merging temporary tables into target tables for {self.xml_file_path}"
+                )
+                logger.error(e)
+                raise
+            finally:
+                if db_semaphore is not None:
+                    db_semaphore.release()
+        finally:
+            logger.info(f"Dropping temporary tables for {self.xml_file_path}")
+            self.model.drop_all_temp_tables()
+
+        return inserted_rows
+
+    def extract_from_database(
+        self,
+        root_table_name: str,
+        root_select_where: str,
+    ) -> dict:
+        """Extract a subtree from the database and store it in a flat format
+
+        :param root_table_name: The root table name to start from
+        :param root_select_where: A where clause to apply to this root table
+        :return: A shallow dict of flat data tables
+        """
+
+        def _fetch_data(
+            sqla_table: Table,
+            key_column: Column,
+            join_sequence: list[tuple[Column, Table, Column]],
+            top_where_clause: TextClause,
+            order_by: Union[None, tuple[Column]],
+            append_to: list,
+            conn: Connection,
+        ):
+            """Fetch data from a specific table and write fetched rows in a dict keyed by the first row column"""
+            quer = select(*(sqla_table.columns.values()))
+
+            join_sequence = join_sequence.copy()
+            if len(join_sequence) > 0:
+                left_col, join_tb, right_col = join_sequence.pop()
+                sub_quer = select(right_col)
+                prev_join_col = left_col
+                for left_col, join_tb, right_col in reversed(join_sequence):
+                    sub_quer = sub_quer.join(join_tb, right_col == prev_join_col)
+                    prev_join_col = left_col
+                sub_quer = sub_quer.where(top_where_clause)
+                quer = quer.where(key_column.in_(sub_quer))
+            else:
+                quer = quer.where(top_where_clause)
+
+            if order_by:
+                quer = quer.order_by(*order_by)
+
+            col_names = sqla_table.columns.keys()
+            for row in conn.execute(quer):
+                append_to.append({key: val for key, val in zip(col_names, row)})
+
+        def _do_extract_table(
+            tb,
+            top_where_clause,
+            parent_table,
+            join_sequence,
+            res_dict,
+            conn,
+        ):
+            """Fetch tables and relationship tables recursively"""
+            if tb.type_name not in res_dict:
+                res_dict[tb.type_name] = {"records": []}
+            _fetch_data(
+                tb.table,
+                (
+                    getattr(tb.table.c, f"pk_{tb.name}")
+                    if tb.is_reused
+                    else getattr(tb.table.c, f"fk_parent_{parent_table.name}")
+                ),
+                join_sequence,
+                top_where_clause,
+                (
+                    None
+                    if tb.is_reused or not tb.data_model.model_config["row_numbers"]
+                    else (
+                        getattr(tb.table.c, f"fk_parent_{parent_table.name}"),
+                        tb.table.c.xml2db_row_number,
+                    )
+                ),
+                res_dict[tb.type_name]["records"],
+                conn,
+            )
+            join_root = (
+                [(None, tb.table, getattr(tb.table.c, f"pk_{tb.name}"))]
+                if parent_table is None
+                else []
+            )
+            if len(tb.relations_n) > 0:
+                if "relations_n" not in res_dict[tb.type_name]:
+                    res_dict[tb.type_name]["relations_n"] = {}
+                for rel in tb.relations_n.values():
+                    if rel.rel_table_name not in res_dict[tb.type_name]["relations_n"]:
+                        res_dict[tb.type_name]["relations_n"][rel.rel_table_name] = {
+                            "records": []
+                        }
+                    new_join = []
+                    if not tb.is_reused:
+                        new_join = [
+                            (
+                                getattr(tb.table.c, f"fk_parent_{parent_table.name}"),
+                                tb.table,
+                                getattr(tb.table.c, f"pk_{tb.table.name}"),
+                            )
+                        ]
+                    if rel.other_table.is_reused:
+                        _fetch_data(
+                            rel.rel_table,
+                            getattr(rel.rel_table.c, f"fk_{tb.name}"),
+                            join_sequence + join_root + new_join,
+                            top_where_clause,
+                            (
+                                (
+                                    getattr(rel.rel_table.c, f"fk_{tb.name}"),
+                                    rel.rel_table.c.xml2db_row_number,
+                                )
+                                if tb.data_model.model_config["row_numbers"]
+                                else None
+                            ),
+                            res_dict[tb.type_name]["relations_n"][rel.rel_table_name][
+                                "records"
+                            ],
+                            conn,
+                        )
+                        new_join = new_join + [
+                            (
+                                getattr(rel.rel_table.c, f"fk_{tb.name}"),
+                                rel.rel_table,
+                                getattr(rel.rel_table.c, f"fk_{rel.other_table.name}"),
+                            )
+                        ]
+                    _do_extract_table(
+                        rel.other_table,
+                        top_where_clause,
+                        tb,
+                        join_sequence + join_root + new_join,
+                        res_dict,
+                        conn,
+                    )
+            for rel in tb.relations_1.values():
+                _do_extract_table(
+                    rel.other_table,
+                    top_where_clause,
+                    tb,
+                    join_sequence
+                    + [
+                        (
+                            getattr(
+                                tb.table.c,
+                                f"pk_{tb.name}"
+                                if tb.is_reused
+                                else f"fk_parent_{parent_table.name}",
+                            ),
+                            tb.table,
+                            getattr(tb.table.c, f"{rel.field_name}"),
+                        )
+                    ],
+                    res_dict,
+                    conn,
+                )
+
+        flat_tables = {}
+
+        with self.model.engine.connect() as conn:
+            _do_extract_table(
+                self.model.tables[root_table_name],
+                text(root_select_where),
+                None,
+                [],
+                flat_tables,
+                conn,
+            )
+
+        self.data = flat_tables
+        return flat_tables
+
+    def __repr__(self) -> str:
+        """Output a repr string for the current document with records count"""
+        settings = (
+            f"temp_prefix: {self.model.temp_prefix}, db_schema: {self.model.db_schema}"
+        )
+        if not self.data:
+            return f"Empty {self.model.data_flow_name} document ({settings})"
+        else:
+            n = sum([len(v["records"]) for v in self.data.values()])
+            return "\n".join(
+                [
+                    f"Parsed {self.xml_file_path} into a {self.model.data_flow_name} document: {n} records",
+                    f"({settings})",
+                ]
+                + [
+                    f"   {self.model.tables[k].name}: {len(v['records'])}"
+                    for k, v in self.data.items()
+                ]
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xml2db-0.10.0/src/xml2db/model.py` & `xml2db-0.9.4/src/xml2db/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,658 +1,643 @@
-import logging
-import os
-from datetime import datetime
-from io import BytesIO
-from typing import Iterable, Union
-from uuid import uuid4
-
-import xmlschema
-import sqlalchemy
-from sqlalchemy import MetaData, create_engine, inspect
-from sqlalchemy.sql.ddl import CreateIndex, CreateTable
-from graphlib import TopologicalSorter
-
-from xml2db import document
-from xml2db.exceptions import DataModelConfigError
-from xml2db.table import (
-    DataModelTableReused,
-    DataModelTableDuplicated,
-)
-from xml2db.xml_converter import XMLConverter
-
-logger = logging.getLogger(__name__)
-
-
-class DataModel:
-    """A class to manage a data model based on an XML schema and its database equivalent.
-
-    This class allows parsing a set of XSD files to build  a representation of
-    the XML schema, simplify it and convert it into a set of database tables.
-    It also allows parsing XML documents that fit this XML schema in order to import
-    the data into the database.
-
-    :param xsd_file: A path to a XSD file
-    :param short_name: A short name for the schema
-    :param long_name: A longer name for the schema
-    :param base_url: The root folder to find other dependant XSD files (by default, the location of the \
-    provided XSD file)
-    :param model_config: A config dict to provide options for building the model
-    :param connection_string: A database connection string (optional if you will not be loading data)
-    :param db_type: The targeted database backend (postgresql, mssql, mysql...). It is ignored and inferred from \
-    `connection_string`, if provided
-    :param db_schema: A schema name to use in the database
-    :param temp_prefix: A prefix to use for temporary tables (if `None`, will be generated randomly)
-
-    :ivar xml_schema: The `xmlschema.XMLSchema` object associated with this data model
-    :ivar data_flow_name: A short identifier used for the data model (`short_name` argument value)
-    :ivar data_flow_long_name: A longer for the data model (`long_name` argument value)
-    :ivar db_schema: A database schema name to store the database tables
-    :ivar source_tree: A text representation of the source data model tree
-    :ivar target_tree: A text representation of the simplified data model tree \
-    which will be used to create target tables
-    """
-
-    def __init__(
-        self,
-        xsd_file: str,
-        short_name: str = None,
-        long_name: str = None,
-        base_url: str = None,
-        model_config: dict = None,
-        connection_string: str = None,
-        db_type: str = None,
-        db_schema: str = None,
-        temp_prefix: str = None,
-    ):
-        self.xml_schema = xmlschema.XMLSchema(
-            os.path.basename(xsd_file) if base_url is None else xsd_file,
-            base_url=(
-                base_url
-                if base_url is not None
-                else os.path.normpath(os.path.dirname(xsd_file))
-            ),
-        )
-        self.xml_converter = XMLConverter(data_model=self)
-        self.data_flow_name = short_name
-        self.data_flow_long_name = long_name
-
-        if connection_string is None:
-            logger.warning(
-                "DataModel created without connection string cannot do actual imports"
-            )
-            self.engine = None
-            self.db_type = db_type
-        else:
-            engine_options = {}
-            if "mssql" in connection_string:
-                engine_options = {
-                    "fast_executemany": True,
-                }
-            self.engine = create_engine(
-                connection_string,
-                isolation_level="SERIALIZABLE",
-                **engine_options,
-            )
-            self.db_type = self.engine.dialect.name
-
-        self.model_config = {} if model_config is None else model_config
-
-        # validate row_numbers global option value
-        if "row_numbers" in self.model_config:
-            if not isinstance(self.model_config["row_numbers"], bool):
-                raise DataModelConfigError("row_numbers must be a bool")
-        else:
-            self.model_config["row_numbers"] = False
-
-        # as_columnstore global option available only for MSSQL database
-        if "as_columnstore" in self.model_config:
-            if not isinstance(self.model_config["as_columnstore"], bool):
-                raise DataModelConfigError("as_columnstore must be a bool")
-            if (
-                self.model_config["as_columnstore"]
-                and self.engine
-                and not self.engine.dialect.name == "mssql"
-            ):
-                self.model_config["as_columnstore"] = False
-                logger.info(
-                    "Clustered columnstore indexes are only supported with MS SQL Server database, noop"
-                )
-        else:
-            self.model_config["as_columnstore"] = False
-
-        self.db_schema = db_schema
-        self.temp_prefix = str(uuid4())[:8] if temp_prefix is None else temp_prefix
-
-        self.tables = {}
-        self.names_types_map = {}
-        self.root_table = None
-        self.types_transforms = {}
-        self.fields_transforms = {}
-        self.ordered_tables_keys = []
-        self.source_tree = ""
-        self.target_tree = ""
-        self.metadata = MetaData()
-        self.processed_at = datetime.now()
-
-        self._build_model()
-
-    @property
-    def fk_ordered_tables(
-        self,
-    ) -> Iterable[Union[DataModelTableDuplicated, DataModelTableReused]]:
-        """Yields tables in create/insert order (tables referenced in foreign keys first)"""
-        for key in self.ordered_tables_keys:
-            yield self.tables[key]
-
-    @property
-    def fk_ordered_tables_reversed(
-        self,
-    ) -> Iterable[Union[DataModelTableDuplicated, DataModelTableReused]]:
-        """Yields tables in drop/delete order (tables referencing foreign keys first)"""
-        for key in reversed(self.ordered_tables_keys):
-            yield self.tables[key]
-
-    def _create_table_model(
-        self,
-        table_name: str,
-        type_name: str,
-        is_root_table: bool = False,
-        is_virtual_node: bool = False,
-    ) -> Union[DataModelTableReused, DataModelTableDuplicated]:
-        """Helper to create a data table model
-
-        :param table_name: name of the table
-        :param type_name: type of the table
-        :param is_root_table: is this table the root table?
-        :param is_virtual_node: was this table created to store multiple root elements?
-        :return: a data table model
-        """
-        table_config = self.model_config.get("tables", {}).get(table_name, {})
-        if table_config.get("reuse", True):
-            return DataModelTableReused(
-                table_name,
-                type_name,
-                is_root_table,
-                is_virtual_node,
-                self.metadata,
-                table_config,
-                self.db_schema,
-                self.temp_prefix,
-                self,
-            )
-        else:
-            return DataModelTableDuplicated(
-                table_name,
-                type_name,
-                is_root_table,
-                is_virtual_node,
-                self.metadata,
-                table_config,
-                self.db_schema,
-                self.temp_prefix,
-                self,
-            )
-
-    def _build_model(self):
-        """Build model from the provided XSD schema and config.
-
-        It will parse the XML schema, then simplify it, then create all sqlalchemy objects.
-        """
-        # parse the XML schema recursively and hold a reference to the head table
-        root_table = self._parse_tree(
-            self.xml_schema[0] if len(self.xml_schema) == 1 else self.xml_schema,
-            is_root_table=True,
-        )
-        self.root_table = root_table.type_name
-        # compute a text representation of the original data model and store it
-        self.source_tree = "\n".join(self._repr_tree(root_table))
-        # check user-provided configuration for tables
-        for tb_config in self.model_config.get("tables", {}):
-            if tb_config not in self.names_types_map:
-                raise DataModelConfigError(
-                    f"Table '{tb_config}' provided in config does not exist"
-                )
-        # simplify the data model recursively starting from the root table
-        self.types_transforms, self.fields_transforms = root_table.simplify_table()
-        # remove tables that have been flagged for deletion during the simplification process
-        root_table.keep_table = True
-        self.tables = {
-            key: tb for key, tb in self.tables.items() if hasattr(tb, "keep_table")
-        }
-        # compute a text representation of the simplified data model and store it
-        self.target_tree = "\n".join(self._repr_tree(root_table))
-        # add parent table information on each table when it is not reused
-        # raises an error if a table is not configured as "reused" and have more than 1 parent table
-        for tb in self.tables.values():
-            tb.compute_dependencies()
-        # build a list of tables in insert/create order
-        ts = TopologicalSorter(
-            {key: sorted(tb.dependencies) for key, tb in self.tables.items()}
-        )
-        self.ordered_tables_keys = list(ts.static_order())
-        # build the ordered table in the sqlalchemy Metadata object (cannot be done before simplification because
-        # it will fail if we attempt to recreate tables that already exist in the sqlalchemy metadata
-        for tb in self.fk_ordered_tables:
-            tb.build_sqlalchemy_tables()
-
-    def _parse_tree(
-        self, parent_node: xmlschema.XsdElement, is_root_table: bool = False
-    ):
-        """Parse a node of an XML schema recursively and create a target data model without any simplification
-
-        We parse the XSD tree recursively to create for each node (basically a complex type in the XSD) an equivalent \
-        DataModelTable (which represents a table in the target data model). By default, tables are named after the \
-        first field name of this type. This is because we hope that fields names will be 'better' than actual \
-        type names. To be on the safe side, we need to make our new table names unique in the event where different \
-        XSD types are used with the same field names somewhere in the data model. Actual XSD types names and our \
-        table names are bijective.
-        This step is fairly straightforward, as we create DataModelTable objects recursively along the XSD tree, and \
-        populate them with appropriate columns and relations.
-
-        :param parent_node: the current XSD node being parsed
-        :param is_root_table: True if this is the root table
-        """
-
-        # find current node type and name and returns corresponding table if it already exists
-        parent_type = (
-            parent_node.type.local_name
-            if hasattr(parent_node, "type")
-            else self.data_flow_name
-        )
-        if parent_type is None:
-            parent_type = parent_node.local_name
-
-        # if this type has already been encountered, stop here and return existing table
-        if parent_type in self.tables:
-            parent_table = self.tables[parent_type]
-            return parent_table
-
-        # elements names and types should be bijective. If an element name is used for different types,
-        # we add a suffix to the name to make it unique again (using a dict to keep the name/type association)
-        parent_name = (
-            parent_node.local_name
-            if hasattr(parent_node, "local_name")
-            else self.data_flow_name
-        )
-        if parent_name in self.names_types_map:
-            i = 1
-            while "_".join([parent_name, str(i)]) in self.names_types_map:
-                i += 1
-            parent_name = "_".join([parent_name, str(i)])
-        self.names_types_map[parent_name] = parent_type
-
-        # create a new table object associated with the element
-        parent_table = self._create_table_model(
-            parent_name,
-            parent_type,
-            is_root_table,
-            isinstance(parent_node, xmlschema.XMLSchema),
-        )
-        self.tables[parent_type] = parent_table
-
-        def recurse_parse_simple_type(elem_type):
-            """Parse simple types to extract properties in case of restrictions, unions, and nested forms"""
-            if len(elem_type) > 1:
-                data_types = []
-                min_lengths = []
-                max_lengths = []
-                allow_empties = []
-                for el_type in elem_type:
-                    dt, mil, mal, ae = recurse_parse_simple_type([el_type])
-                    data_types.append(dt)
-                    min_lengths.append(mil)
-                    max_lengths.append(mal)
-                    allow_empties.append(ae)
-                return (
-                    data_types[0] if len(set(data_types)) == 1 else "string",
-                    (
-                        min(min_lengths)
-                        if all(e is not None for e in min_lengths)
-                        else None
-                    ),
-                    (
-                        max(max_lengths)
-                        if all(e is not None for e in max_lengths)
-                        else None
-                    ),
-                    any(allow_empties),
-                )
-            elem_type = elem_type[0]
-            if elem_type.is_union():
-                return (
-                    recurse_parse_simple_type(elem_type.base_type.member_types)
-                    if elem_type.base_type
-                    else recurse_parse_simple_type(elem_type.member_types)
-                )
-            if elem_type.is_restriction():
-                dt = elem_type.base_type.local_name
-                mil = elem_type.min_length
-                mal = elem_type.max_length
-                ae = elem_type.allow_empty
-                if elem_type.base_type.is_restriction():
-                    bt_dt, bt_mil, bt_mal, bt_ae = recurse_parse_simple_type(
-                        [elem_type.base_type]
-                    )
-                    dt = bt_dt
-                    mil = (
-                        min(mil, bt_mil)
-                        if mil is not None and bt_mil is not None
-                        else None
-                    )
-                    mal = (
-                        max(mal, bt_mal)
-                        if mal is not None and bt_mal is not None
-                        else None
-                    )
-                    ae = ae and bt_ae if ae is not None and bt_ae is not None else None
-                if elem_type.enumeration is not None:
-                    mil = min([len(val) for val in elem_type.enumeration])
-                    mal = max([len(val) for val in elem_type.enumeration])
-                return dt, mil, mal, ae
-            return (
-                elem_type.local_name,
-                elem_type.min_length,
-                elem_type.max_length,
-                elem_type.allow_empty,
-            )
-
-        def get_occurs(particle):
-            parent_occurs = [1, 1]
-            if particle.parent and hasattr(particle.parent, "model"):
-                parent_occurs = get_occurs(particle.parent)
-                if particle.parent.model == "choice":
-                    parent_occurs[0] = 0
-            return [
-                min(parent_occurs[0], particle.min_occurs),
-                (
-                    max(parent_occurs[1], particle.max_occurs)
-                    if parent_occurs[1] is not None and particle.max_occurs is not None
-                    else None
-                ),
-            ]
-
-        # go through item attributes and add them as columns
-        for attrib_name, attrib in parent_node.attributes.items():
-            (
-                data_type,
-                min_length,
-                max_length,
-                allow_empty,
-            ) = recurse_parse_simple_type([attrib.type])
-            parent_table.add_column(
-                f"{attrib_name}",
-                data_type,
-                [0, 1],
-                min_length,
-                max_length,
-                True,
-                False,
-                allow_empty,
-                None,
-            )
-        nested_containers = []
-        # go through the children to add either arguments either relations to the current element
-        for child in parent_node:
-            if type(child) is xmlschema.XsdElement:
-                # "nested_containers" is used to allow ordering nodes in mostly correct order in case of nested sequence
-                # with multiple occurrence when generating XML. For instance, if we have a sequence A, B with
-                # max occur > 1, we want to generate A, B, A, B and not A, A, B, B, thus we mark A and B as member of
-                # the same "ngroup", which will be used when generating XML
-                if (
-                    len(nested_containers) > 1
-                    and child.parent == nested_containers[-2][0]
-                ):
-                    nested_containers.pop()
-                elif (
-                    len(nested_containers) == 0
-                    or child.parent != nested_containers[-1][0]
-                ):
-                    nested_containers.append(
-                        (
-                            child.parent,
-                            (
-                                str(hash(child.parent))
-                                if child.parent
-                                and child.parent.max_occurs != 1
-                                and child.parent.model != "choice"
-                                else None
-                            ),
-                        )
-                    )
-                ct = child.type
-                if (
-                    ct.is_complex()
-                    and len(child) == 0
-                    and len(child.attributes) == 0
-                    and ct.base_type is not None
-                ):
-                    ct = ct.base_type
-                if ct.is_simple():
-                    (
-                        data_type,
-                        min_length,
-                        max_length,
-                        allow_empty,
-                    ) = recurse_parse_simple_type([ct])
-                    occurs = get_occurs(child)
-                    parent_table.add_column(
-                        child.local_name,
-                        data_type,
-                        occurs,
-                        min_length,
-                        max_length,
-                        False,
-                        False,
-                        allow_empty,
-                        nested_containers[-1][1],
-                    )
-
-                elif ct.is_complex():
-                    child_table = self._parse_tree(child)
-                    child_table.model_group = (
-                        "choice"
-                        if ct.model_group and ct.model_group.model == "choice"
-                        else "sequence"
-                    )
-                    occurs = get_occurs(child)
-                    if child.is_single():
-                        parent_table.add_relation_1(
-                            child.local_name,
-                            child_table,
-                            occurs,
-                            nested_containers[-1][1],
-                        )
-                    else:
-                        parent_table.add_relation_n(
-                            child.local_name,
-                            child_table,
-                            occurs,
-                            nested_containers[-1][1],
-                        )
-                else:
-                    raise ValueError("unknown case; please check")
-            else:
-                raise ValueError("unknown case; please check (child not an XsdElement)")
-
-        if hasattr(parent_node, "type") and (
-            parent_node.type.has_mixed_content()
-            or parent_node.type.has_simple_content()
-        ):
-            if parent_node.type.base_type is not None:
-                (
-                    data_type,
-                    min_length,
-                    max_length,
-                    allow_empty,
-                ) = recurse_parse_simple_type([parent_node.type.base_type])
-            else:
-                data_type, min_length, max_length, allow_empty = "string", 0, None, True
-
-            parent_table.add_column(
-                "value",
-                data_type,
-                [0, 1],
-                min_length,
-                max_length,
-                False,
-                True,
-                allow_empty,
-                None,
-            )
-
-        return parent_table
-
-    def _repr_tree(
-        self,
-        parent_table: Union[DataModelTableReused, DataModelTableDuplicated],
-        visited_nodes=None,
-    ):
-        """Build a text representation of the data model tree
-
-        :param parent_table: the current data model table object
-        """
-        if visited_nodes is None:
-            visited_nodes = set()
-        else:
-            visited_nodes = {item for item in visited_nodes}
-        visited_nodes.add(parent_table.name)
-        for field_type, name, field in parent_table.fields:
-            if field_type == "col":
-                yield f"{field.name}{field.occurs}: {field.data_type}"
-            elif field_type == "rel1":
-                mg = " (choice)" if field.other_table.model_group == "choice" else ""
-                yield f"{field.name}{field.occurs}{mg}:{' ...' if field_type in visited_nodes else ''}"
-                if field.other_table.name not in visited_nodes:
-                    for line in self._repr_tree(field.other_table, visited_nodes):
-                        yield f"    {line}"
-            elif field_type == "reln":
-                mg = " (choice)" if field.other_table.model_group == "choice" else ""
-                yield f"{field.name}{field.occurs}{mg}:{' ...' if field_type in visited_nodes else ''}"
-                for line in self._repr_tree(field.other_table, visited_nodes):
-                    yield f"    {line}"
-
-    def get_entity_rel_diagram(self, text_context=True) -> str:
-        """Build an entity relationship diagram for the data model
-
-        The ERD syntax is used by mermaid.js to create a visual representation of the diagram, which is supported
-        by Pycharm IDE or GitHub in markdown files, among others
-
-        :param text_context: Should we add a title, a text explanation, etc. or just the ERD?
-        :return: A string representation of the ERD
-        """
-        out = ["erDiagram"]
-        for tb in self.fk_ordered_tables_reversed:
-            out += tb.get_entity_rel_diagram()
-
-        if text_context:
-            out = (
-                [
-                    f"# {self.data_flow_long_name}\n",
-                    f"### Data model name: `{self.data_flow_name}`\n",
-                    (
-                        "The following *Entity Relationships Diagram* represents the target data model, after the "
-                        "simplification of the source data model, but before the transformations performed to optimize "
-                        "data storage (transformation of `1-1` and `1-n` relationships into `n-1` and `n-n` "
-                        "relationships, respectively, as described [here](../../docs/recycling_nodes.md)).\n"
-                    ),
-                    (
-                        "As a consequence, not all tables of the actual data model used in the database are shown. "
-                        "Specifically, `1-n` relationships presented may be stored in the database using an additional "
-                        "relationship table (noted with an asterisk in the relationship name).\n"
-                    ),
-                    "```mermaid",
-                ]
-                + out
-                + [
-                    "```",
-                    (
-                        "`-N` suffix in field type indicates that the field can have multiple values, which will be "
-                        "stored as comma separated values."
-                    ),
-                ]
-            )
-        return "\n".join(out)
-
-    def get_all_create_table_statements(self, temp=False) -> Iterable[CreateTable]:
-        """Yield create table statements for all tables
-
-        :param temp: If True, yield create table statements for temporary tables (prefixed)
-        """
-        for tb in self.fk_ordered_tables:
-            yield from tb.get_create_table_statements(temp)
-
-    def get_all_create_index_statements(self) -> Iterable[CreateIndex]:
-        """Yield create index statements for all tables"""
-        for tb in self.fk_ordered_tables:
-            yield from tb.get_create_index_statements()
-
-    def create_all_tables(self, temp: bool = False) -> None:
-        """Create tables for the data model, either target tables or temp tables used to import data
-
-        :param temp: If True, create temporary (prefixed) tables
-        """
-        for tb in self.fk_ordered_tables:
-            tb.create_tables(self.engine, temp)
-
-    def create_db_schema(self) -> None:
-        """Create database schema if it does not already exist."""
-        if self.db_schema is not None:
-            inspector = inspect(self.engine)
-            if self.db_schema not in inspector.get_schema_names():
-                with self.engine.connect() as conn:
-                    conn.execute(sqlalchemy.schema.CreateSchema(self.db_schema))
-                    conn.commit()
-                logger.info(f"Created schema: {self.db_schema}")
-
-    def drop_all_tables(self):
-        """Drop the data model target (unprefixed) tables.
-
-        BE CAUTIOUS, THIS METHOD DROPS TABLES WITHOUT FURTHER NOTICE!
-
-        """
-        for tb in self.fk_ordered_tables_reversed:
-            tb.drop_tables(self.engine)
-
-    def drop_all_temp_tables(self):
-        """Drop the data model temporary (prefixed) tables.
-
-        BE CAUTIOUS, THIS METHOD DROPS TABLES WITHOUT FURTHER NOTICE!
-
-        """
-        for tb in self.fk_ordered_tables_reversed:
-            tb.drop_temp_tables(self.engine)
-
-    def parse_xml(
-        self,
-        xml_file: Union[str, BytesIO],
-        xml_file_path: str = None,
-        skip_validation: bool = True,
-    ) -> document.Document:
-        """Parse an XML document based on this data model
-
-        This method is just a wrapper around the parse_xml method of the Document class.
-
-        :param xml_file: The path or the file object of an XML file to parse
-        :param xml_file_path: The path of the XML file, mandatory if xml_file is file object in order to fill the \
-        'xml2db_input_file_path' column of the root table.
-        :param skip_validation: Should we validate the documents against the schema first?
-        :return: A parsed `Document` object
-        """
-        doc = document.Document(self)
-        doc.parse_xml(xml_file, xml_file_path, skip_validation)
-        return doc
-
-    def extract_from_database(
-        self,
-        root_select_where: str,
-        force_tz: Union[str, None] = None,
-    ) -> document.Document:
-        """Extract a document from the database, based on a where clause applied to the root table. For instance, you
-        can use the column `xml2db_input_file_path` to filter the data loaded from a specific file.
-
-        :param root_select_where: A where clause to apply to this root table, as a string
-        :param force_tz: Apply this timezone if database returns timezone-naïve datetime
-        :return: A `Document` object containing extracted data
-        """
-        doc = document.Document(self)
-        doc.extract_from_database(self.root_table, root_select_where, force_tz=force_tz)
-        return doc
+import logging
+import os
+from datetime import datetime
+from io import BytesIO
+from typing import Iterable, Union
+from uuid import uuid4
+
+import xmlschema
+import sqlalchemy
+from sqlalchemy import MetaData, create_engine, inspect
+from sqlalchemy.sql.ddl import CreateIndex, CreateTable
+from graphlib import TopologicalSorter
+
+from xml2db import document
+from xml2db.exceptions import DataModelConfigError
+from xml2db.table import (
+    DataModelTableReused,
+    DataModelTableDuplicated,
+)
+from xml2db.xml_converter import XMLConverter
+
+logger = logging.getLogger(__name__)
+
+
+class DataModel:
+    """A class to manage a data model based on an XML schema and its database equivalent.
+
+    This class allows parsing a set of XSD files to build  a representation of
+    the XML schema, simplify it and convert it into a set of database tables.
+    It also allows parsing XML documents that fit this XML schema in order to import
+    the data into the database.
+
+    :param xsd_file: A path to a XSD file
+    :param short_name: A short name for the schema
+    :param long_name: A longer name for the schema
+    :param base_url: The root folder to find other dependant XSD files (by default, the location of the \
+    provided XSD file)
+    :param model_config: A config dict to provide options for building the model
+    :param connection_string: A database connection string (optional if you will not be loading data)
+    :param db_schema: A schema name to use in the database
+    :param temp_prefix: A prefix to use for temporary tables (if `None`, will be generated randomly)
+
+    :ivar xml_schema: The `xmlschema.XMLSchema` object associated with this data model
+    :ivar data_flow_name: A short identifier used for the data model (`short_name` argument value)
+    :ivar data_flow_long_name: A longer for the data model (`long_name` argument value)
+    :ivar db_schema: A database schema name to store the database tables
+    :ivar source_tree: A text representation of the source data model tree
+    :ivar target_tree: A text representation of the simplified data model tree \
+    which will be used to create target tables
+    """
+
+    def __init__(
+        self,
+        xsd_file: str,
+        short_name: str = None,
+        long_name: str = None,
+        base_url: str = None,
+        model_config: dict = None,
+        connection_string: str = None,
+        db_schema: str = None,
+        temp_prefix: str = None,
+    ):
+        self.xml_schema = xmlschema.XMLSchema(
+            os.path.basename(xsd_file) if base_url is None else xsd_file,
+            base_url=base_url
+            if base_url is not None
+            else os.path.normpath(os.path.dirname(xsd_file)),
+        )
+        self.xml_converter = XMLConverter(data_model=self)
+        self.data_flow_name = short_name
+        self.data_flow_long_name = long_name
+
+        if connection_string is None:
+            logger.warning(
+                "DataModel created without connection string cannot do actual imports"
+            )
+            self.engine = None
+        else:
+            engine_options = {}
+            if "mssql" in connection_string:
+                engine_options = {
+                    "fast_executemany": True,
+                }
+            self.engine = create_engine(
+                connection_string,
+                isolation_level="SERIALIZABLE",
+                **engine_options,
+            )
+
+        self.model_config = {} if model_config is None else model_config
+
+        # validate row_numbers global option value
+        if "row_numbers" in self.model_config:
+            if not isinstance(self.model_config["row_numbers"], bool):
+                raise DataModelConfigError("row_numbers must be a bool")
+        else:
+            self.model_config["row_numbers"] = False
+
+        # as_columnstore global option available only for MSSQL database
+        if "as_columnstore" in self.model_config:
+            if not isinstance(self.model_config["as_columnstore"], bool):
+                raise DataModelConfigError("as_columnstore must be a bool")
+            if (
+                self.model_config["as_columnstore"]
+                and self.engine
+                and not self.engine.dialect.name == "mssql"
+            ):
+                self.model_config["as_columnstore"] = False
+                logger.info(
+                    "Clustered columnstore indexes are only supported with MS SQL Server database, noop"
+                )
+        else:
+            self.model_config["as_columnstore"] = False
+
+        self.db_schema = db_schema
+        self.temp_prefix = str(uuid4())[:8] if temp_prefix is None else temp_prefix
+
+        self.tables = {}
+        self.names_types_map = {}
+        self.root_table = None
+        self.types_transforms = {}
+        self.fields_transforms = {}
+        self.ordered_tables_keys = []
+        self.source_tree = ""
+        self.target_tree = ""
+        self.metadata = MetaData()
+        self.processed_at = datetime.now()
+
+        self._build_model()
+
+    @property
+    def fk_ordered_tables(
+        self,
+    ) -> Iterable[Union[DataModelTableDuplicated, DataModelTableReused]]:
+        """Yields tables in create/insert order (tables referenced in foreign keys first)"""
+        for key in self.ordered_tables_keys:
+            yield self.tables[key]
+
+    @property
+    def fk_ordered_tables_reversed(
+        self,
+    ) -> Iterable[Union[DataModelTableDuplicated, DataModelTableReused]]:
+        """Yields tables in drop/delete order (tables referencing foreign keys first)"""
+        for key in reversed(self.ordered_tables_keys):
+            yield self.tables[key]
+
+    def _create_table_model(
+        self,
+        table_name: str,
+        type_name: str,
+        is_root_table: bool = False,
+        is_virtual_node: bool = False,
+    ) -> Union[DataModelTableReused, DataModelTableDuplicated]:
+        """Helper to create a data table model
+
+        :param table_name: name of the table
+        :param type_name: type of the table
+        :param is_root_table: is this table the root table?
+        :param is_virtual_node: was this table created to store multiple root elements?
+        :return: a data table model
+        """
+        table_config = self.model_config.get("tables", {}).get(table_name, {})
+        if table_config.get("reuse", True):
+            return DataModelTableReused(
+                table_name,
+                type_name,
+                is_root_table,
+                is_virtual_node,
+                self.metadata,
+                table_config,
+                self.db_schema,
+                self.temp_prefix,
+                self,
+            )
+        else:
+            return DataModelTableDuplicated(
+                table_name,
+                type_name,
+                is_root_table,
+                is_virtual_node,
+                self.metadata,
+                table_config,
+                self.db_schema,
+                self.temp_prefix,
+                self,
+            )
+
+    def _build_model(self):
+        """Build model from the provided XSD schema and config.
+
+        It will parse the XML schema, then simplify it, then create all sqlalchemy objects.
+        """
+        # parse the XML schema recursively and hold a reference to the head table
+        root_table = self._parse_tree(
+            self.xml_schema[0] if len(self.xml_schema) == 1 else self.xml_schema,
+            is_root_table=True,
+        )
+        self.root_table = root_table.type_name
+        # compute a text representation of the original data model and store it
+        self.source_tree = "\n".join(self._repr_tree(root_table))
+        # check user-provided configuration for tables
+        for tb_config in self.model_config.get("tables", {}):
+            if tb_config not in self.names_types_map:
+                raise DataModelConfigError(
+                    f"Table '{tb_config}' provided in config does not exist"
+                )
+        # simplify the data model recursively starting from the root table
+        self.types_transforms, self.fields_transforms = root_table.simplify_table()
+        # remove tables that have been flagged for deletion during the simplification process
+        root_table.keep_table = True
+        self.tables = {
+            key: tb for key, tb in self.tables.items() if hasattr(tb, "keep_table")
+        }
+        # compute a text representation of the simplified data model and store it
+        self.target_tree = "\n".join(self._repr_tree(root_table))
+        # add parent table information on each table when it is not reused
+        # raises an error if a table is not configured as "reused" and have more than 1 parent table
+        for tb in self.tables.values():
+            tb.compute_dependencies()
+        # build a list of tables in insert/create order
+        ts = TopologicalSorter(
+            {key: sorted(tb.dependencies) for key, tb in self.tables.items()}
+        )
+        self.ordered_tables_keys = list(ts.static_order())
+        # build the ordered table in the sqlalchemy Metadata object (cannot be done before simplification because
+        # it will fail if we attempt to recreate tables that already exist in the sqlalchemy metadata
+        for tb in self.fk_ordered_tables:
+            tb.build_sqlalchemy_tables()
+
+    def _parse_tree(
+        self, parent_node: xmlschema.XsdElement, is_root_table: bool = False
+    ):
+        """Parse a node of an XML schema recursively and create a target data model without any simplification
+
+        We parse the XSD tree recursively to create for each node (basically a complex type in the XSD) an equivalent \
+        DataModelTable (which represents a table in the target data model). By default, tables are named after the \
+        first field name of this type. This is because we hope that fields names will be 'better' than actual \
+        type names. To be on the safe side, we need to make our new table names unique in the event where different \
+        XSD types are used with the same field names somewhere in the data model. Actual XSD types names and our \
+        table names are bijective.
+        This step is fairly straightforward, as we create DataModelTable objects recursively along the XSD tree, and \
+        populate them with appropriate columns and relations.
+
+        :param parent_node: the current XSD node being parsed
+        :param is_root_table: True if this is the root table
+        """
+
+        # find current node type and name and returns corresponding table if it already exists
+        parent_type = (
+            parent_node.type.local_name
+            if hasattr(parent_node, "type")
+            else self.data_flow_name
+        )
+        if parent_type is None:
+            parent_type = parent_node.local_name
+
+        # if this type has already been encountered, stop here and return existing table
+        if parent_type in self.tables:
+            parent_table = self.tables[parent_type]
+            return parent_table
+
+        # elements names and types should be bijective. If an element name is used for different types,
+        # we add a suffix to the name to make it unique again (using a dict to keep the name/type association)
+        parent_name = (
+            parent_node.local_name
+            if hasattr(parent_node, "local_name")
+            else self.data_flow_name
+        )
+        if parent_name in self.names_types_map:
+            i = 1
+            while "_".join([parent_name, str(i)]) in self.names_types_map:
+                i += 1
+            parent_name = "_".join([parent_name, str(i)])
+        self.names_types_map[parent_name] = parent_type
+
+        # create a new table object associated with the element
+        parent_table = self._create_table_model(
+            parent_name,
+            parent_type,
+            is_root_table,
+            isinstance(parent_node, xmlschema.XMLSchema),
+        )
+        self.tables[parent_type] = parent_table
+
+        def recurse_parse_simple_type(elem_type):
+            """Parse simple types to extract properties in case of restrictions, unions, and nested forms"""
+            if len(elem_type) > 1:
+                data_types = []
+                min_lengths = []
+                max_lengths = []
+                allow_empties = []
+                for el_type in elem_type:
+                    dt, mil, mal, ae = recurse_parse_simple_type([el_type])
+                    data_types.append(dt)
+                    min_lengths.append(mil)
+                    max_lengths.append(mal)
+                    allow_empties.append(ae)
+                return (
+                    data_types[0] if len(set(data_types)) == 1 else "string",
+                    (
+                        min(min_lengths)
+                        if all(e is not None for e in min_lengths)
+                        else None
+                    ),
+                    (
+                        max(max_lengths)
+                        if all(e is not None for e in max_lengths)
+                        else None
+                    ),
+                    any(allow_empties),
+                )
+            elem_type = elem_type[0]
+            if elem_type.is_union():
+                return (
+                    recurse_parse_simple_type(elem_type.base_type.member_types)
+                    if elem_type.base_type
+                    else recurse_parse_simple_type(elem_type.member_types)
+                )
+            if elem_type.is_restriction():
+                dt = elem_type.base_type.local_name
+                mil = elem_type.min_length
+                mal = elem_type.max_length
+                ae = elem_type.allow_empty
+                if elem_type.base_type.is_restriction():
+                    bt_dt, bt_mil, bt_mal, bt_ae = recurse_parse_simple_type(
+                        [elem_type.base_type]
+                    )
+                    dt = bt_dt
+                    mil = (
+                        min(mil, bt_mil)
+                        if mil is not None and bt_mil is not None
+                        else None
+                    )
+                    mal = (
+                        max(mal, bt_mal)
+                        if mal is not None and bt_mal is not None
+                        else None
+                    )
+                    ae = ae and bt_ae if ae is not None and bt_ae is not None else None
+                if elem_type.enumeration is not None:
+                    mil = min([len(val) for val in elem_type.enumeration])
+                    mal = max([len(val) for val in elem_type.enumeration])
+                return dt, mil, mal, ae
+            return (
+                elem_type.local_name,
+                elem_type.min_length,
+                elem_type.max_length,
+                elem_type.allow_empty,
+            )
+
+        def get_occurs(particle):
+            parent_occurs = [1, 1]
+            if particle.parent and hasattr(particle.parent, "model"):
+                parent_occurs = get_occurs(particle.parent)
+            return [
+                min(parent_occurs[0], particle.min_occurs),
+                max(parent_occurs[1], particle.max_occurs)
+                if parent_occurs[1] is not None and particle.max_occurs is not None
+                else None,
+            ]
+
+        # go through item attributes and add them as columns
+        for attrib_name, attrib in parent_node.attributes.items():
+            (
+                data_type,
+                min_length,
+                max_length,
+                allow_empty,
+            ) = recurse_parse_simple_type([attrib.type])
+            parent_table.add_column(
+                f"{attrib_name}",
+                data_type,
+                [0, 1],
+                min_length,
+                max_length,
+                True,
+                False,
+                allow_empty,
+                None,
+            )
+        nested_containers = []
+        # go through the children to add either arguments either relations to the current element
+        for child in parent_node:
+            if type(child) is xmlschema.XsdElement:
+                # "nested_containers" is used to allow ordering nodes in mostly correct order in case of nested sequence
+                # with multiple occurrence when generating XML. For instance, if we have a sequence A, B with
+                # max occur > 1, we want to generate A, B, A, B and not A, A, B, B, thus we mark A and B as member of
+                # the same "ngroup", which will be used when generating XML
+                if (
+                    len(nested_containers) > 1
+                    and child.parent == nested_containers[-2][0]
+                ):
+                    nested_containers.pop()
+                elif (
+                    len(nested_containers) == 0
+                    or child.parent != nested_containers[-1][0]
+                ):
+                    nested_containers.append(
+                        (
+                            child.parent,
+                            str(hash(child.parent))
+                            if child.parent
+                            and child.parent.max_occurs != 1
+                            and child.parent.model != "choice"
+                            else None,
+                        )
+                    )
+                ct = child.type
+                if (
+                    ct.is_complex()
+                    and len(child) == 0
+                    and len(child.attributes) == 0
+                    and ct.base_type is not None
+                ):
+                    ct = ct.base_type
+                if ct.is_simple():
+                    (
+                        data_type,
+                        min_length,
+                        max_length,
+                        allow_empty,
+                    ) = recurse_parse_simple_type([ct])
+                    occurs = get_occurs(child)
+                    parent_table.add_column(
+                        child.local_name,
+                        data_type,
+                        occurs,
+                        min_length,
+                        max_length,
+                        False,
+                        False,
+                        allow_empty,
+                        nested_containers[-1][1],
+                    )
+
+                elif ct.is_complex():
+                    child_table = self._parse_tree(child)
+                    child_table.model_group = (
+                        "choice"
+                        if ct.model_group and ct.model_group.model == "choice"
+                        else "sequence"
+                    )
+                    occurs = get_occurs(child)
+                    if child.is_single():
+                        parent_table.add_relation_1(
+                            child.local_name,
+                            child_table,
+                            occurs,
+                            nested_containers[-1][1],
+                        )
+                    else:
+                        parent_table.add_relation_n(
+                            child.local_name,
+                            child_table,
+                            occurs,
+                            nested_containers[-1][1],
+                        )
+                else:
+                    raise ValueError("unknown case; please check")
+            else:
+                raise ValueError("unknown case; please check (child not an XsdElement)")
+
+        if hasattr(parent_node, "type") and (
+            parent_node.type.has_mixed_content()
+            or parent_node.type.has_simple_content()
+        ):
+            if parent_node.type.base_type is not None:
+                (
+                    data_type,
+                    min_length,
+                    max_length,
+                    allow_empty,
+                ) = recurse_parse_simple_type([parent_node.type.base_type])
+            else:
+                data_type, min_length, max_length, allow_empty = "string", 0, None, True
+
+            parent_table.add_column(
+                "value",
+                data_type,
+                [0, 1],
+                min_length,
+                max_length,
+                False,
+                True,
+                allow_empty,
+                None,
+            )
+
+        return parent_table
+
+    def _repr_tree(
+        self,
+        parent_table: Union[DataModelTableReused, DataModelTableDuplicated],
+        visited_nodes=None,
+    ):
+        """Build a text representation of the data model tree
+
+        :param parent_table: the current data model table object
+        """
+        if visited_nodes is None:
+            visited_nodes = set()
+        else:
+            visited_nodes = {item for item in visited_nodes}
+        visited_nodes.add(parent_table.name)
+        for field_type, name, field in parent_table.fields:
+            if field_type == "col":
+                yield f"{field.name}{field.occurs}: {field.data_type}"
+            elif field_type == "rel1":
+                mg = " (choice)" if field.other_table.model_group == "choice" else ""
+                yield f"{field.name}{field.occurs}{mg}:{' ...' if field_type in visited_nodes else ''}"
+                if field.other_table.name not in visited_nodes:
+                    for line in self._repr_tree(field.other_table, visited_nodes):
+                        yield f"    {line}"
+            elif field_type == "reln":
+                mg = " (choice)" if field.other_table.model_group == "choice" else ""
+                yield f"{field.name}{field.occurs}{mg}:{' ...' if field_type in visited_nodes else ''}"
+                for line in self._repr_tree(field.other_table, visited_nodes):
+                    yield f"    {line}"
+
+    def get_entity_rel_diagram(self, text_context=True) -> str:
+        """Build an entity relationship diagram for the data model
+
+        The ERD syntax is used by mermaid.js to create a visual representation of the diagram, which is supported
+        by Pycharm IDE or GitHub in markdown files, among others
+
+        :param text_context: Should we add a title, a text explanation, etc. or just the ERD?
+        :return: A string representation of the ERD
+        """
+        out = ["erDiagram"]
+        for tb in self.fk_ordered_tables_reversed:
+            out += tb.get_entity_rel_diagram()
+
+        if text_context:
+            out = (
+                [
+                    f"# {self.data_flow_long_name}\n",
+                    f"### Data model name: `{self.data_flow_name}`\n",
+                    (
+                        "The following *Entity Relationships Diagram* represents the target data model, after the "
+                        "simplification of the source data model, but before the transformations performed to optimize "
+                        "data storage (transformation of `1-1` and `1-n` relationships into `n-1` and `n-n` "
+                        "relationships, respectively, as described [here](../../docs/recycling_nodes.md)).\n"
+                    ),
+                    (
+                        "As a consequence, not all tables of the actual data model used in the database are shown. "
+                        "Specifically, `1-n` relationships presented may be stored in the database using an additional "
+                        "relationship table (noted with an asterisk in the relationship name).\n"
+                    ),
+                    "```mermaid",
+                ]
+                + out
+                + [
+                    "```",
+                    (
+                        "`-N` suffix in field type indicates that the field can have multiple values, which will be "
+                        "stored as comma separated values."
+                    ),
+                ]
+            )
+        return "\n".join(out)
+
+    def get_all_create_table_statements(self, temp=False) -> Iterable[CreateTable]:
+        """Yield create table statements for all tables
+
+        :param temp: If True, yield create table statements for temporary tables (prefixed)
+        """
+        for tb in self.fk_ordered_tables:
+            yield from tb.get_create_table_statements(temp)
+
+    def get_all_create_index_statements(self) -> Iterable[CreateIndex]:
+        """Yield create index statements for all tables"""
+        for tb in self.fk_ordered_tables:
+            yield from tb.get_create_index_statements()
+
+    def create_all_tables(self, temp: bool = False) -> None:
+        """Create tables for the data model, either target tables or temp tables used to import data
+
+        :param temp: If True, create temporary (prefixed) tables
+        """
+        for tb in self.fk_ordered_tables:
+            tb.create_tables(self.engine, temp)
+
+    def create_db_schema(self) -> None:
+        """Create database schema if it does not already exist."""
+        if self.db_schema is not None:
+            inspector = inspect(self.engine)
+            if self.db_schema not in inspector.get_schema_names():
+                with self.engine.connect() as conn:
+                    conn.execute(sqlalchemy.schema.CreateSchema(self.db_schema))
+                    conn.commit()
+                logger.info(f"Created schema: {self.db_schema}")
+
+    def drop_all_tables(self):
+        """Drop the data model target (unprefixed) tables.
+
+        BE CAUTIOUS, THIS METHOD DROPS TABLES WITHOUT FURTHER NOTICE!
+
+        """
+        for tb in self.fk_ordered_tables_reversed:
+            tb.drop_tables(self.engine)
+
+    def drop_all_temp_tables(self):
+        """Drop the data model temporary (prefixed) tables.
+
+        BE CAUTIOUS, THIS METHOD DROPS TABLES WITHOUT FURTHER NOTICE!
+
+        """
+        for tb in self.fk_ordered_tables_reversed:
+            tb.drop_temp_tables(self.engine)
+
+    def parse_xml(
+        self,
+        xml_file: Union[str, BytesIO],
+        xml_file_path: str = None,
+        skip_validation: bool = True,
+    ) -> document.Document:
+        """Parse an XML document based on this data model
+
+        This method is just a wrapper around the parse_xml method of the Document class.
+
+        :param xml_file: The path or the file object of an XML file to parse
+        :param xml_file_path: The path of the XML file, mandatory if xml_file is file object in order to fill the \
+        'xml2db_input_file_path' column of the root table.
+        :param skip_validation: Should we validate the documents against the schema first?
+        :return: A parsed `Document` object
+        """
+        doc = document.Document(self)
+        doc.parse_xml(xml_file, xml_file_path, skip_validation)
+        return doc
+
+    def extract_from_database(
+        self,
+        root_select_where: str,
+    ) -> document.Document:
+        """Extract a document from the database, based on a where clause applied to the root table. For instance, you
+        can use the column `xml2db_input_file_path` to filter the data loaded from a specific file.
+
+        :param root_select_where: A where clause to apply to this root table, as a string
+        :return: A `Document` object containing extracted data
+        """
+        doc = document.Document(self)
+        doc.extract_from_database(self.root_table, root_select_where)
+        return doc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xml2db-0.10.0/src/xml2db/table/column.py` & `xml2db-0.9.4/src/xml2db/table/column.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,222 +1,199 @@
-import logging
-from typing import List, Iterable, Any, Union, TYPE_CHECKING
-
-from sqlalchemy import (
-    Integer,
-    Double,
-    Boolean,
-    BigInteger,
-    SmallInteger,
-    Column,
-    DateTime,
-    String,
-    LargeBinary,
-)
-from sqlalchemy.dialects import mssql, mysql
-
-if TYPE_CHECKING:
-    from xml2db.model import DataModel
-
-logger = logging.getLogger(__name__)
-
-
-def types_mapping_default(temp: bool, col: "DataModelColumn") -> Any:
-    """Defines the sqlalchemy type to use for given column properties in target tables
-
-    :param temp: are we targeting the temporary tables schema or the final tables?
-    :param col: an object representing a column of a table for which we are determining the SQL type to define
-    :return: a sqlalchemy class representing the data type to be used
-    """
-    if col.occurs[1] != 1:
-        return String(8000)
-    if col.data_type in ["decimal", "float"]:
-        return Double
-    if col.data_type == "dateTime":
-        return DateTime(timezone=True)
-    if col.data_type == "integer" or col.data_type == "int":
-        return Integer
-    if col.data_type == "boolean":
-        return Boolean
-    if col.data_type == "byte":
-        return SmallInteger
-    if col.data_type == "long":
-        return BigInteger
-    if col.data_type == "date":
-        return String(16)
-    if col.data_type == "time":
-        return String(18)
-    if col.data_type in ["string", "NMTOKEN", "duration", "token"]:
-        if col.max_length is None:
-            return String(1000)
-        min_length = 0 if col.min_length is None else col.min_length
-        if min_length >= col.max_length - 1 and not col.allow_empty:
-            return String(col.max_length)
-        return String(col.max_length)
-    if col.data_type == "binary":
-        return LargeBinary(col.max_length)
-    else:
-        logger.warning(
-            f"unknown type '{col.data_type}' for column '{col.name}', defaulting to VARCHAR(1000) "
-            f"(this can be overridden by providing a field type in the configuration)"
-        )
-        return String(1000)
-
-
-def types_mapping_mssql(temp: bool, col: "DataModelColumn") -> Any:
-    """Defines the MSSQL type to use for given column properties in target tables
-
-    :param temp: are we targeting the temporary tables schema or the final tables?
-    :param col: an object representing a column of a table for which we are determining the SQL type to define
-    :return: a sqlalchemy class representing the data type to be used
-    """
-    if col.occurs[1] != 1:
-        return mssql.VARCHAR(8000)
-    if col.data_type in ["decimal", "float"]:
-        return Double
-    if col.data_type == "dateTime":
-        # using the DATETIMEOFFSET directly in the temporary table caused issues when inserting data in the target
-        # table with INSERT INTO SELECT converts datetime VARCHAR to DATETIMEOFFSET without errors
-        return mssql.VARCHAR(100) if temp else mssql.DATETIMEOFFSET
-    if col.data_type == "integer" or col.data_type == "int":
-        return Integer
-    if col.data_type == "boolean":
-        return Boolean
-    if col.data_type == "byte":
-        return SmallInteger
-    if col.data_type == "long":
-        return BigInteger
-    if col.data_type == "date":
-        return mssql.VARCHAR(16)
-    if col.data_type == "time":
-        return mssql.VARCHAR(18)
-    if col.data_type in ["string", "NMTOKEN", "duration", "token"]:
-        if col.max_length is None:
-            return mssql.VARCHAR(1000)
-        min_length = 0 if col.min_length is None else col.min_length
-        if min_length >= col.max_length - 1 and not col.allow_empty:
-            return mssql.CHAR(col.max_length)
-        return mssql.VARCHAR(col.max_length)
-    if col.data_type == "binary":
-        if col.max_length == col.min_length:
-            return mssql.BINARY(col.max_length)
-        return mssql.VARBINARY(col.max_length)
-    else:
-        logger.warning(
-            f"unknown type '{col.data_type}' for column '{col.name}', defaulting to VARCHAR(1000) "
-            f"(this can be overridden by providing a field type in the configuration)"
-        )
-        return mssql.VARCHAR(1000)
-
-
-def types_mapping_mysql(temp: bool, col: "DataModelColumn") -> Any:
-    """Defines the MySQL/sqlalchemy type to use for given column properties in target tables
-
-    :param temp: are we targeting the temporary tables schema or the final tables?
-    :param col: an object representing a column of a table for which we are determining the SQL type to define
-    :return: a sqlalchemy class representing the data type to be used
-    """
-    if col.occurs[1] != 1:
-        return String(4000)
-    if col.data_type in ["string", "NMTOKEN", "duration", "token"]:
-        if col.max_length is None:
-            return String(255)
-    if col.data_type == "binary":
-        if col.max_length == col.min_length:
-            return mysql.BINARY(col.max_length)
-        return mysql.VARBINARY(col.max_length)
-    return types_mapping_default(temp, col)
-
-
-class DataModelColumn:
-    """A class representing a column of a table
-
-    :param name: column name
-    :param data_type: column data type
-    :param occurs: min and max occurrences of the field
-    :param min_length: min length
-    :param max_length: max length
-    :param is_attr: does the column value come from an xml attribute?
-    :param is_content: is the column used to store the content value of a mixed complex type?
-    :param allow_empty: is nullable ?
-    :param ngroup: a key used to handle nested sequences
-    :param model_config: data model config, may contain column type information
-    :param data_model: the DataModel object it belongs to
-    :ivar name: the name of the field (i.e. column name)
-    :ivar data_type: the data type, extracted from XSD data type
-    :ivar occurs: list of int with two elements: min occurrences and max occurrences. \
-    Max occurrences is None if unbounded
-    """
-
-    def __init__(
-        self,
-        name: str,
-        name_chain: list,
-        data_type: str,
-        occurs: List[int],
-        min_length: int,
-        max_length: Union[int, None],
-        is_attr: bool,
-        is_content: bool,
-        allow_empty: bool,
-        ngroup: Union[int, None],
-        model_config: dict[str, Any],
-        data_model: "DataModel",
-    ):
-        """Constructor method"""
-        self.name = name
-        self.name_chain = name_chain
-        self.data_type = data_type
-        self.occurs = occurs
-        self.min_length = min_length
-        self.max_length = max_length
-        self.is_attr = is_attr
-        self.is_content = is_content
-        self.allow_empty = allow_empty
-        self.ngroup = ngroup
-        self.model_config = model_config
-        self.data_model = data_model
-        self.other_table = None  # just to avoid a linting warning
-        self.types_mapping = (
-            types_mapping_mssql
-            if data_model.db_type == "mssql"
-            else (
-                types_mapping_mysql
-                if data_model.db_type == "mysql"
-                else types_mapping_default
-            )
-        )
-
-    @property
-    def can_join_values_as_string(self):
-        """Decide whether multiple values can be stored as comma separated values in this column
-
-        :return: True if data type is compatible with comma separated values
-        :raises ValueError: if data type does not allow storage as comma separated values
-        """
-        if self.occurs[1] == 1:
-            return True
-        if self.occurs[1] is None or self.occurs[1] > 1:
-            if self.data_type in (
-                "string",
-                "date",
-                "dateTime",
-                "NMTOKEN",
-                "time",
-            ):
-                return True
-            raise ValueError(
-                f"Col type '{self.data_type}' with maxOccur > 1 is not supported."
-            )
-        return False
-
-    def get_sqlalchemy_column(self, temp: bool = False) -> Iterable[Column]:
-        """Create sqlalchemy Column object
-
-        :param temp: temp table or target table ?
-        """
-        # use type specified in config if exists
-        column_type = self.model_config.get("fields", {}).get(self.name, {}).get(
-            "type"
-        ) or self.types_mapping(temp, self)
-
-        yield Column(self.name, column_type)
+import logging
+from typing import List, Iterable, Any, Union, TYPE_CHECKING
+
+from sqlalchemy import (
+    Integer,
+    Float,
+    Boolean,
+    BigInteger,
+    SmallInteger,
+    Column,
+    DateTime,
+    String,
+    LargeBinary,
+)
+from sqlalchemy.dialects import mssql
+
+if TYPE_CHECKING:
+    from xml2db.model import DataModel
+
+logger = logging.getLogger(__name__)
+
+
+def types_mapping_default(temp: bool, col: "DataModelColumn") -> Any:
+    """Defines the sqlalchemy type to use for given column properties in target tables
+
+    :param temp: are we targeting the temporary tables schema or the final tables?
+    :param col: an object representing a column of a table for which we are determining the SQL type to define
+    :return: a sqlalchemy class representing the data type to be used
+    """
+    if col.occurs[1] != 1:
+        return String(8000)
+    if col.data_type in ["decimal", "float"]:
+        return Float
+    if col.data_type == "dateTime":
+        return DateTime(timezone=True)
+    if col.data_type == "integer" or col.data_type == "int":
+        return Integer
+    if col.data_type == "boolean":
+        return Boolean
+    if col.data_type == "byte":
+        return SmallInteger
+    if col.data_type == "long":
+        return BigInteger
+    if col.data_type == "date":
+        return String(16)
+    if col.data_type == "time":
+        return String(18)
+    if col.data_type in ["string", "NMTOKEN", "duration", "token"]:
+        if col.max_length is None:
+            return String(1000)
+        min_length = 0 if col.min_length is None else col.min_length
+        if min_length >= col.max_length - 1 and not col.allow_empty:
+            return String(col.max_length)
+        return String(col.max_length)
+    if col.data_type == "binary":
+        return LargeBinary(col.max_length)
+    else:
+        logger.warning(
+            f"unknown type '{col.data_type}' for column '{col.name}', defaulting to VARCHAR(1000) "
+            f"(this can be overridden by providing a field type in the configuration)"
+        )
+        return String(1000)
+
+
+def types_mapping_mssql(temp: bool, col: "DataModelColumn") -> Any:
+    """Defines the MSSQL type to use for given column properties in target tables
+
+    :param temp: are we targeting the temporary tables schema or the final tables?
+    :param col: an object representing a column of a table for which we are determining the SQL type to define
+    :return: a sqlalchemy class representing the data type to be used
+    """
+    if col.occurs[1] != 1:
+        return mssql.VARCHAR(8000)
+    if col.data_type in ["decimal", "float"]:
+        return Float
+    if col.data_type == "dateTime":
+        # using the DATETIMEOFFSET directly in the temporary table caused issues when inserting data in the target
+        # table with INSERT INTO SELECT converts datetime VARCHAR to DATETIMEOFFSET without errors
+        return mssql.VARCHAR(100) if temp else mssql.DATETIMEOFFSET
+    if col.data_type == "integer" or col.data_type == "int":
+        return Integer
+    if col.data_type == "boolean":
+        return Boolean
+    if col.data_type == "byte":
+        return SmallInteger
+    if col.data_type == "long":
+        return BigInteger
+    if col.data_type == "date":
+        return mssql.VARCHAR(16)
+    if col.data_type == "time":
+        return mssql.VARCHAR(18)
+    if col.data_type in ["string", "NMTOKEN", "duration", "token"]:
+        if col.max_length is None:
+            return mssql.VARCHAR(1000)
+        min_length = 0 if col.min_length is None else col.min_length
+        if min_length >= col.max_length - 1 and not col.allow_empty:
+            return mssql.CHAR(col.max_length)
+        return mssql.VARCHAR(col.max_length)
+    if col.data_type == "binary":
+        if col.max_length == col.min_length:
+            return mssql.BINARY(col.max_length)
+        return mssql.VARBINARY(col.max_length)
+    else:
+        logger.warning(
+            f"unknown type '{col.data_type}' for column '{col.name}', defaulting to VARCHAR(1000) "
+            f"(this can be overridden by providing a field type in the configuration)"
+        )
+        return mssql.VARCHAR(1000)
+
+
+class DataModelColumn:
+    """A class representing a column of a table
+
+    :param name: column name
+    :param data_type: column data type
+    :param occurs: min and max occurrences of the field
+    :param min_length: min length
+    :param max_length: max length
+    :param is_attr: does the column value come from an xml attribute?
+    :param is_content: is the column used to store the content value of a mixed complex type?
+    :param allow_empty: is nullable ?
+    :param ngroup: a key used to handle nested sequences
+    :param model_config: data model config, may contain column type information
+    :param data_model: the DataModel object it belongs to
+    :ivar name: the name of the field (i.e. column name)
+    :ivar data_type: the data type, extracted from XSD data type
+    :ivar occurs: list of int with two elements: min occurrences and max occurrences. \
+    Max occurrences is None if unbounded
+    """
+
+    def __init__(
+        self,
+        name: str,
+        name_chain: list,
+        data_type: str,
+        occurs: List[int],
+        min_length: int,
+        max_length: Union[int, None],
+        is_attr: bool,
+        is_content: bool,
+        allow_empty: bool,
+        ngroup: Union[int, None],
+        model_config: dict[str, Any],
+        data_model: "DataModel",
+    ):
+        """Constructor method"""
+        self.name = name
+        self.name_chain = name_chain
+        self.data_type = data_type
+        self.occurs = occurs
+        self.min_length = min_length
+        self.max_length = max_length
+        self.is_attr = is_attr
+        self.is_content = is_content
+        self.allow_empty = allow_empty
+        self.ngroup = ngroup
+        self.model_config = model_config
+        self.data_model = data_model
+        self.other_table = None  # just to avoid a linting warning
+        self.types_mapping = (
+            types_mapping_mssql
+            if data_model.engine and data_model.engine.dialect.name == "mssql"
+            else types_mapping_default
+        )
+
+    @property
+    def can_join_values_as_string(self):
+        """Decide whether multiple values can be stored as comma separated values in this column
+
+        :return: True if data type is compatible with comma separated values
+        :raises ValueError: if data type does not allow storage as comma separated values
+        """
+        if self.occurs[1] == 1:
+            return True
+        if self.occurs[1] is None or self.occurs[1] > 1:
+            if self.data_type in (
+                "string",
+                "date",
+                "dateTime",
+                "NMTOKEN",
+                "time",
+            ):
+                return True
+            raise ValueError(
+                f"Col type '{self.data_type}' with maxOccur > 1 is not supported."
+            )
+        return False
+
+    def get_sqlalchemy_column(self, temp: bool = False) -> Iterable[Column]:
+        """Create sqlalchemy Column object
+
+        :param temp: temp table or target table ?
+        """
+        # use type specified in config if exists
+        column_type = self.model_config.get("fields", {}).get(self.name, {}).get(
+            "type"
+        ) or self.types_mapping(temp, self)
+
+        yield Column(self.name, column_type)
```

### Comparing `xml2db-0.10.0/src/xml2db/table/relations.py` & `xml2db-0.9.4/src/xml2db/table/relations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-import sqlalchemy.engine
-from sqlalchemy import Table, Column, ForeignKey, Integer, Index, select
-from typing import TYPE_CHECKING, List, Iterable, Any, Union
-
-if TYPE_CHECKING:
-    from xml2db.table.table import DataModelTable
-    from xml2db.model import DataModel
-
-
-class DataModelRelation:
-    """A class representing a relation with another table
-
-    :param name: the name of the field holding the relation in the parent table
-    :param table: the parent table model in the relation
-    :param other_table: the other table model in the relation
-    :param occurs: list of int with two elements: min occurrences and max occurrences. \
-    Max occurrences is None if unbounded
-    :param ngroup: a key used to handle nested sequences
-    :param data_model: the DataModel object it belongs to
-    """
-
-    def __init__(
-        self,
-        name: str,
-        name_chain: list,
-        table: "DataModelTable",
-        other_table: "DataModelTable",
-        occurs: List[int],
-        ngroup: Union[str, None],
-        data_model: "DataModel",
-    ):
-        """Constructor method"""
-        self.name = name
-        self.name_chain = name_chain
-        self.table = table
-        self.other_table = other_table
-        self.occurs = occurs
-        self.ngroup = ngroup
-        self.rel_table_name = None
-        self.field_name = None
-        self.rel_table = None
-        self.temp_rel_table = None
-        self.data_model = data_model
-
-
-class DataModelRelation1(DataModelRelation):
-    """A class representing a 1-1 relation with another table"""
-
-    def get_sqlalchemy_column(self, temp: bool = False):
-        """Yields SQLAlchemy object representing the foreign key relation
-
-        :param temp: are we targeting temp or target table?
-        """
-        self.field_name = (
-            f"{self.name}_fk_{self.other_table.name}"
-            if not self.name.endswith(self.other_table.name)
-            else f"fk_{self.name}"
-        )
-        if temp:
-            yield Column(f"temp_{self.field_name}", Integer)
-            yield Column(self.field_name, Integer)
-        else:
-            yield Column(
-                self.field_name,
-                Integer,
-                ForeignKey(f"{self.other_table.name}.pk_{self.other_table.name}"),
-                index=True,
-            )
-
-    def get_merge_temp_records_statements(self) -> Iterable[Any]:
-        """A SQL statement to update foreign keys values from target table back to temp table after insert
-
-        :return: iterable of SQL statements
-        """
-        yield self.table.temp_table.update().values(
-            **{
-                self.field_name: getattr(
-                    self.other_table.temp_table.c, f"pk_{self.other_table.name}"
-                )
-            }
-        ).where(
-            getattr(self.table.temp_table.c, f"temp_{self.field_name}")
-            == getattr(
-                self.other_table.temp_table.c, f"temp_pk_{self.other_table.name}"
-            )
-        )
-
-
-class DataModelRelationN(DataModelRelation):
-    """A class representing a 1-N relation with another table"""
-
-    def build_relation_tables(self) -> None:
-        """Builds sqlalchemy objects for intermediate relationship tables"""
-        self.rel_table_name = (
-            f"{self.table.name}_{self.name}_{self.other_table.name}"
-            if not self.name.endswith(self.other_table.name)
-            else f"{self.table.name}_{self.name}"
-        )
-        prefix = f"temp_{self.table.temp_prefix}_"
-        if self.other_table.is_reused:
-            self.temp_rel_table = Table(
-                f"{prefix}{self.rel_table_name}",
-                self.table.metadata,
-                Column(f"temp_fk_{self.table.name}", Integer, nullable=False),
-                Column(f"fk_{self.table.name}", Integer),
-                Column(f"temp_fk_{self.other_table.name}", Integer, nullable=False),
-                Column(f"fk_{self.other_table.name}", Integer),
-                *(
-                    (
-                        Column(
-                            "xml2db_row_number",
-                            Integer,
-                            nullable=False,
-                        ),
-                    )
-                    if self.data_model.model_config["row_numbers"]
-                    else ()
-                ),
-            )
-            cl_index = ()
-            if (
-                self.data_model.engine
-                and self.data_model.engine.dialect.name == "mssql"
-                and not self.data_model.model_config["as_columnstore"]
-            ):
-                # n-n relation tables don't have a primary key, so we define a clustered index on the first FK
-                cl_index = (
-                    Index(
-                        f"ix_fk_{self.rel_table_name}",
-                        f"fk_{self.table.name}",
-                        mssql_clustered=True,
-                    ),
-                )
-
-            self.rel_table = Table(
-                self.rel_table_name,
-                self.table.metadata,
-                Column(
-                    f"fk_{self.table.name}",
-                    Integer,
-                    ForeignKey(f"{self.table.name}.pk_{self.table.name}"),
-                    nullable=False,
-                ),
-                Column(
-                    f"fk_{self.other_table.name}",
-                    Integer,
-                    ForeignKey(f"{self.other_table.name}.pk_{self.other_table.name}"),
-                    nullable=False,
-                    index=True,
-                ),
-                *(
-                    (
-                        Column(
-                            "xml2db_row_number",
-                            Integer,
-                            nullable=False,
-                        ),
-                    )
-                    if self.data_model.model_config["row_numbers"]
-                    else ()
-                ),
-                *cl_index,
-            )
-
-            # set columnstore index
-            if self.data_model.model_config["as_columnstore"]:
-                self.rel_table.append_constraint(
-                    Index(
-                        f"idx_{self.rel_table.name}_columnstore",
-                        mssql_clustered=True,
-                        mssql_columnstore=True,
-                    )
-                )
-
-            if self.table.db_schema is not None:
-                self.rel_table.schema = self.table.db_schema
-                self.temp_rel_table.schema = self.table.db_schema
-
-    def create_table(
-        self, engine: sqlalchemy.engine.Engine, temp: bool = False
-    ) -> None:
-        """Create intermediate relationship table
-
-        :param engine: sqlalchemy engine to use
-        :param temp: are we creating temp or target table?
-        """
-        if temp:
-            if self.temp_rel_table is not None:
-                self.temp_rel_table.create(engine, checkfirst=True)
-        else:
-            if self.rel_table is not None:
-                self.rel_table.create(engine, checkfirst=True)
-
-    def get_merge_temp_records_statements(self) -> Iterable[Any]:
-        """Issue SQL statements to insert new records in the intermediate relationship table
-
-        First, it will update foreign keys in the relationship table to use target tables foreign keys.
-        Then, it will insert new relationship records into the target relationship table
-
-        :return: sqlalchemy query statements
-        """
-        if self.other_table.is_reused:
-            rel_tb = self.temp_rel_table
-            # update foreign key with self
-            yield rel_tb.update().values(
-                **{
-                    f"fk_{self.table.name}": getattr(
-                        self.table.temp_table.c, f"pk_{self.table.name}"
-                    )
-                }
-            ).where(
-                getattr(  # noqa: Linter puzzled by ==
-                    rel_tb.c, f"temp_fk_{self.table.name}"
-                )
-                == getattr(self.table.temp_table.c, f"temp_pk_{self.table.name}")
-            ).where(
-                self.table.temp_table.c.temp_exists
-                == False  # noqa: SQLAlchemy not supporting "is False"
-            )
-            # update foreign key with other table
-            yield rel_tb.update().values(
-                **{
-                    f"fk_{self.other_table.name}": getattr(
-                        self.other_table.temp_table.c, f"pk_{self.other_table.name}"
-                    )
-                }
-            ).where(
-                getattr(  # noqa: Linter puzzled by ==
-                    rel_tb.c, f"temp_fk_{self.other_table.name}"
-                )
-                == getattr(
-                    self.other_table.temp_table.c, f"temp_pk_{self.other_table.name}"
-                )
-            )
-            # insert new records
-            cols = [f"fk_{self.table.name}", f"fk_{self.other_table.name}"]
-            if self.data_model.model_config["row_numbers"]:
-                cols = cols + ["xml2db_row_number"]
-            sel = select(*[getattr(rel_tb.c, col) for col in cols]).where(
-                getattr(rel_tb.c, f"fk_{self.table.name}")  # noqa
-                != None  # SQLAlchemy not supporting "is not None"
-            )
-            yield self.rel_table.insert().from_select(cols, sel)
+import sqlalchemy.engine
+from sqlalchemy import Table, Column, ForeignKey, Integer, Index, select
+from typing import TYPE_CHECKING, List, Iterable, Any, Union
+
+if TYPE_CHECKING:
+    from xml2db.table.table import DataModelTable
+    from xml2db.model import DataModel
+
+
+class DataModelRelation:
+    """A class representing a relation with another table
+
+    :param name: the name of the field holding the relation in the parent table
+    :param table: the parent table model in the relation
+    :param other_table: the other table model in the relation
+    :param occurs: list of int with two elements: min occurrences and max occurrences. \
+    Max occurrences is None if unbounded
+    :param ngroup: a key used to handle nested sequences
+    :param data_model: the DataModel object it belongs to
+    """
+
+    def __init__(
+        self,
+        name: str,
+        name_chain: list,
+        table: "DataModelTable",
+        other_table: "DataModelTable",
+        occurs: List[int],
+        ngroup: Union[str, None],
+        data_model: "DataModel",
+    ):
+        """Constructor method"""
+        self.name = name
+        self.name_chain = name_chain
+        self.table = table
+        self.other_table = other_table
+        self.occurs = occurs
+        self.ngroup = ngroup
+        self.rel_table_name = None
+        self.field_name = None
+        self.rel_table = None
+        self.temp_rel_table = None
+        self.data_model = data_model
+
+
+class DataModelRelation1(DataModelRelation):
+    """A class representing a 1-1 relation with another table"""
+
+    def get_sqlalchemy_column(self, temp: bool = False):
+        """Yields SQLAlchemy object representing the foreign key relation
+
+        :param temp: are we targeting temp or target table?
+        """
+        self.field_name = (
+            f"{self.name}_fk_{self.other_table.name}"
+            if not self.name.endswith(self.other_table.name)
+            else f"fk_{self.name}"
+        )
+        if temp:
+            yield Column(f"temp_{self.field_name}", Integer)
+            yield Column(self.field_name, Integer)
+        else:
+            yield Column(
+                self.field_name,
+                Integer,
+                ForeignKey(f"{self.other_table.name}.pk_{self.other_table.name}"),
+                index=True,
+            )
+
+    def get_merge_temp_records_statements(self) -> Iterable[Any]:
+        """A SQL statement to update foreign keys values from target table back to temp table after insert
+
+        :return: iterable of SQL statements
+        """
+        yield self.table.temp_table.update().values(
+            **{
+                self.field_name: getattr(
+                    self.other_table.temp_table.c, f"pk_{self.other_table.name}"
+                )
+            }
+        ).where(
+            getattr(self.table.temp_table.c, f"temp_{self.field_name}")
+            == getattr(
+                self.other_table.temp_table.c, f"temp_pk_{self.other_table.name}"
+            )
+        )
+
+
+class DataModelRelationN(DataModelRelation):
+    """A class representing a 1-N relation with another table"""
+
+    def build_relation_tables(self) -> None:
+        """Builds sqlalchemy objects for intermediate relationship tables"""
+        self.rel_table_name = (
+            f"{self.table.name}_{self.name}_{self.other_table.name}"
+            if not self.name.endswith(self.other_table.name)
+            else f"{self.table.name}_{self.other_table.name}"
+        )
+        prefix = f"temp_{self.table.temp_prefix}_"
+        if self.other_table.is_reused:
+            self.temp_rel_table = Table(
+                f"{prefix}{self.rel_table_name}",
+                self.table.metadata,
+                Column(f"temp_fk_{self.table.name}", Integer, nullable=False),
+                Column(f"fk_{self.table.name}", Integer),
+                Column(f"temp_fk_{self.other_table.name}", Integer, nullable=False),
+                Column(f"fk_{self.other_table.name}", Integer),
+                *(
+                    (
+                        Column(
+                            "xml2db_row_number",
+                            Integer,
+                            nullable=False,
+                        ),
+                    )
+                    if self.data_model.model_config["row_numbers"]
+                    else ()
+                ),
+            )
+            cl_index = ()
+            if (
+                self.data_model.engine
+                and self.data_model.engine.dialect.name == "mssql"
+                and not self.data_model.model_config["as_columnstore"]
+            ):
+                # n-n relation tables don't have a primary key, so we define a clustered index on the first FK
+                cl_index = (
+                    Index(
+                        f"ix_fk_{self.rel_table_name}",
+                        f"fk_{self.table.name}",
+                        mssql_clustered=True,
+                    ),
+                )
+
+            self.rel_table = Table(
+                self.rel_table_name,
+                self.table.metadata,
+                Column(
+                    f"fk_{self.table.name}",
+                    Integer,
+                    ForeignKey(f"{self.table.name}.pk_{self.table.name}"),
+                    nullable=False,
+                ),
+                Column(
+                    f"fk_{self.other_table.name}",
+                    Integer,
+                    ForeignKey(f"{self.other_table.name}.pk_{self.other_table.name}"),
+                    nullable=False,
+                    index=True,
+                ),
+                *(
+                    (
+                        Column(
+                            "xml2db_row_number",
+                            Integer,
+                            nullable=False,
+                        ),
+                    )
+                    if self.data_model.model_config["row_numbers"]
+                    else ()
+                ),
+                *cl_index,
+            )
+
+            # set columnstore index
+            if self.data_model.model_config["as_columnstore"]:
+                self.rel_table.append_constraint(
+                    Index(
+                        f"idx_{self.rel_table.name}_columnstore",
+                        mssql_clustered=True,
+                        mssql_columnstore=True,
+                    )
+                )
+
+            if self.table.db_schema is not None:
+                self.rel_table.schema = self.table.db_schema
+                self.temp_rel_table.schema = self.table.db_schema
+
+    def create_table(
+        self, engine: sqlalchemy.engine.Engine, temp: bool = False
+    ) -> None:
+        """Create intermediate relationship table
+
+        :param engine: sqlalchemy engine to use
+        :param temp: are we creating temp or target table?
+        """
+        if temp:
+            if self.temp_rel_table is not None:
+                self.temp_rel_table.create(engine, checkfirst=True)
+        else:
+            if self.rel_table is not None:
+                self.rel_table.create(engine, checkfirst=True)
+
+    def get_merge_temp_records_statements(self) -> Iterable[Any]:
+        """Issue SQL statements to insert new records in the intermediate relationship table
+
+        First, it will update foreign keys in the relationship table to use target tables foreign keys.
+        Then, it will insert new relationship records into the target relationship table
+
+        :return: sqlalchemy query statements
+        """
+        if self.other_table.is_reused:
+            rel_tb = self.temp_rel_table
+            # update foreign key with self
+            yield rel_tb.update().values(
+                **{
+                    f"fk_{self.table.name}": getattr(
+                        self.table.temp_table.c, f"pk_{self.table.name}"
+                    )
+                }
+            ).where(
+                getattr(  # noqa: Linter puzzled by ==
+                    rel_tb.c, f"temp_fk_{self.table.name}"
+                )
+                == getattr(self.table.temp_table.c, f"temp_pk_{self.table.name}")
+            ).where(
+                self.table.temp_table.c.temp_exists
+                == False  # noqa: SQLAlchemy not supporting "is False"
+            )
+            # update foreign key with other table
+            yield rel_tb.update().values(
+                **{
+                    f"fk_{self.other_table.name}": getattr(
+                        self.other_table.temp_table.c, f"pk_{self.other_table.name}"
+                    )
+                }
+            ).where(
+                getattr(  # noqa: Linter puzzled by ==
+                    rel_tb.c, f"temp_fk_{self.other_table.name}"
+                )
+                == getattr(
+                    self.other_table.temp_table.c, f"temp_pk_{self.other_table.name}"
+                )
+            )
+            # insert new records
+            cols = [f"fk_{self.table.name}", f"fk_{self.other_table.name}"]
+            if self.data_model.model_config["row_numbers"]:
+                cols = cols + ["xml2db_row_number"]
+            sel = select(*[getattr(rel_tb.c, col) for col in cols]).where(
+                getattr(rel_tb.c, f"fk_{self.table.name}")  # noqa
+                != None  # SQLAlchemy not supporting "is not None"
+            )
+            yield self.rel_table.insert().from_select(cols, sel)
```

### Comparing `xml2db-0.10.0/src/xml2db/table/reused_table.py` & `xml2db-0.9.4/src/xml2db/table/reused_table.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-from sqlalchemy import (
-    Table,
-    Column,
-    Integer,
-    Index,
-    PrimaryKeyConstraint,
-    UniqueConstraint,
-    Boolean,
-    DateTime,
-    String,
-    LargeBinary,
-    select,
-)
-
-from .transformed_table import DataModelTableTransformed
-from .column import DataModelColumn
-
-
-class DataModelTableReused(DataModelTableTransformed):
-    """A table data model which de-duplicates records in the database based on their hash value.
-
-    This table model is the default model to store XML nodes. n-n relationships with parent nodes \
-    are represented with an intermediate relationship table. Although more complicated than the \
-    duplicated version, this table model store less records in the database.
-    """
-
-    is_reused = True
-
-    def build_sqlalchemy_tables(self):
-        """Build sqlalchemy table objects.
-
-        Build the sqlalchemy table objet based on table attributes for the main table, \
-        and relation tables to store n-n relationships, for target and temp tables \
-        (so it builds at least 2 tables if there is no relations).
-        This method is intended to be called only once (if it called more than once it \
-        will return immediately) and further changes to the table will not be updated.
-
-        """
-
-        if self.table is not None:
-            return
-
-        prefix = f"temp_{self.temp_prefix}_"
-
-        # build target table and n-n relations tables
-        def get_col(temp=False):
-            for field_type, key, field in self.fields:
-                if field_type == "col" or field_type == "rel1":
-                    yield from field.get_sqlalchemy_column(temp)
-            # Root table is given additional integration metadata columns
-            if self.is_root_table:
-                yield Column("xml2db_input_file_path", String(256), nullable=False)
-                # Use DataModelColumn to create record hash column in order to get the right data type
-                processed_at_col = DataModelColumn(
-                    "xml2db_processed_at",
-                    [],
-                    "dateTime",
-                    [1, 1],
-                    0,
-                    None,
-                    False,
-                    False,
-                    False,
-                    None,
-                    self.config,
-                    self.data_model,
-                )
-                yield from processed_at_col.get_sqlalchemy_column(temp)
-            hash_col = DataModelColumn(
-                "record_hash",
-                [],
-                "binary",
-                [1, 1],
-                20,
-                20,
-                False,
-                False,
-                False,
-                None,
-                self.config,
-                self.data_model,
-            )
-            yield from hash_col.get_sqlalchemy_column(temp)
-            yield UniqueConstraint(
-                "record_hash",
-                name=f"{prefix if temp else ''}{self.name}_xml2db_record_hash",
-            )
-
-        # build target table
-        self.table = Table(
-            self.name,
-            self.metadata,
-            Column(f"pk_{self.name}", Integer, primary_key=True, autoincrement=True),
-            PrimaryKeyConstraint(
-                name=f"cx_pk_{self.name}",
-                mssql_clustered=not self.config["as_columnstore"],
-            ),
-            *get_col(),
-        )
-
-        # set columnstore index
-        if self.config["as_columnstore"]:
-            self.table.append_constraint(
-                Index(
-                    f"idx_{self.name}_columnstore",
-                    mssql_clustered=True,
-                    mssql_columnstore=True,
-                )
-            )
-
-        # build temporary table
-        self.temp_table = Table(
-            f"{prefix}{self.name}",
-            self.metadata,
-            Column(f"pk_{self.name}", Integer),
-            Column(
-                f"temp_pk_{self.name}", Integer, primary_key=True, autoincrement=False
-            ),
-            *get_col(temp=True),
-            Column("temp_exists", Boolean, default=False),
-        )
-
-        # build relation tables
-        for rel in self.relations_n.values():
-            rel.build_relation_tables()
-
-        self._set_db_schema()
-
-    def get_merge_temp_records_statements(self):
-        """Yield insert and update statements to merge temporary tables into target tables
-
-        This method yield SQL statements inserting the data of the temporary table (prefixed)
-        into the target tables (unprefixed). It deals with primary keys and foreign keys by
-        looking up first existing records with the same hash in order to reuse already existing
-        records when the new record is identical.
-
-        This method should not be called directly but through the save_db method in the Document
-        class, which will ensure that merge queries are issued in the correct order for all the
-        data flow, and which will encapsulated all queries in a transaction in order to rollback
-        changes on failure.
-        """
-
-        # find matching records hash in target table
-        yield self.temp_table.update().values(temp_exists=True).where(
-            getattr(self.temp_table.c, "record_hash")  # noqa: Linter puzzled by ==
-            == getattr(self.table.c, "record_hash")
-        )
-
-        # update foreign keys for n-1 relations tables
-        for rel in self.relations_1.values():
-            yield from rel.get_merge_temp_records_statements()
-
-        # insert missing records from temp table to target
-        cols = [
-            col_name
-            for col_name in self.temp_table.columns.keys()
-            if not col_name.startswith("temp_") and col_name != f"pk_{self.name}"
-        ]
-        sel = select(*[getattr(self.temp_table.c, col) for col in cols]).where(
-            self.temp_table.c.temp_exists
-            == False  # noqa: SQLAlchemy not supporting "is False"
-        )
-        yield self.table.insert().from_select(cols, sel)
-
-        # update primary keys back in temp table
-        yield self.temp_table.update().values(
-            **{f"pk_{self.name}": getattr(self.table.c, f"pk_{self.name}")}
-        ).where(
-            getattr(self.temp_table.c, "record_hash")  # noqa: Linter puzzled by ==
-            == getattr(self.table.c, "record_hash")
-        )
-
-        # update primary keys for n-n relations tables
-        for rel in self.relations_n.values():
-            yield from rel.get_merge_temp_records_statements()
+from sqlalchemy import (
+    Table,
+    Column,
+    Integer,
+    Index,
+    PrimaryKeyConstraint,
+    UniqueConstraint,
+    Boolean,
+    DateTime,
+    String,
+    LargeBinary,
+    select,
+)
+
+from .transformed_table import DataModelTableTransformed
+from .column import DataModelColumn
+
+
+class DataModelTableReused(DataModelTableTransformed):
+    """A table data model which de-duplicates records in the database based on their hash value.
+
+    This table model is the default model to store XML nodes. n-n relationships with parent nodes \
+    are represented with an intermediate relationship table. Although more complicated than the \
+    duplicated version, this table model store less records in the database.
+    """
+
+    is_reused = True
+
+    def build_sqlalchemy_tables(self):
+        """Build sqlalchemy table objects.
+
+        Build the sqlalchemy table objet based on table attributes for the main table, \
+        and relation tables to store n-n relationships, for target and temp tables \
+        (so it builds at least 2 tables if there is no relations).
+        This method is intended to be called only once (if it called more than once it \
+        will return immediately) and further changes to the table will not be updated.
+
+        """
+
+        if self.table is not None:
+            return
+
+        prefix = f"temp_{self.temp_prefix}_"
+
+        # build target table and n-n relations tables
+        def get_col(temp=False):
+            for field_type, key, field in self.fields:
+                if field_type == "col" or field_type == "rel1":
+                    yield from field.get_sqlalchemy_column(temp)
+            # Root table is given additional integration metadata columns
+            if self.is_root_table:
+                yield Column("xml2db_input_file_path", String(256), nullable=False)
+                # Use DataModelColumn to create record hash column in order to get the right data type
+                processed_at_col = DataModelColumn(
+                    "xml2db_processed_at",
+                    [],
+                    "dateTime",
+                    [1, 1],
+                    0,
+                    None,
+                    False,
+                    False,
+                    False,
+                    None,
+                    self.config,
+                    self.data_model,
+                )
+                yield from processed_at_col.get_sqlalchemy_column(temp)
+            hash_col = DataModelColumn(
+                "record_hash",
+                [],
+                "binary",
+                [1, 1],
+                20,
+                20,
+                False,
+                False,
+                False,
+                None,
+                self.config,
+                self.data_model,
+            )
+            yield from hash_col.get_sqlalchemy_column(temp)
+            yield UniqueConstraint(
+                "record_hash",
+                name=f"{prefix if temp else ''}{self.name}_xml2db_record_hash",
+            )
+
+        # build target table
+        self.table = Table(
+            self.name,
+            self.metadata,
+            Column(f"pk_{self.name}", Integer, primary_key=True, autoincrement=True),
+            PrimaryKeyConstraint(
+                name=f"cx_pk_{self.name}",
+                mssql_clustered=not self.config["as_columnstore"],
+            ),
+            *get_col(),
+        )
+
+        # set columnstore index
+        if self.config["as_columnstore"]:
+            self.table.append_constraint(
+                Index(
+                    f"idx_{self.name}_columnstore",
+                    mssql_clustered=True,
+                    mssql_columnstore=True,
+                )
+            )
+
+        # build temporary table
+        self.temp_table = Table(
+            f"{prefix}{self.name}",
+            self.metadata,
+            Column(f"pk_{self.name}", Integer),
+            Column(
+                f"temp_pk_{self.name}", Integer, primary_key=True, autoincrement=False
+            ),
+            *get_col(temp=True),
+            Column("temp_exists", Boolean, default=False),
+        )
+
+        # build relation tables
+        for rel in self.relations_n.values():
+            rel.build_relation_tables()
+
+        self._set_db_schema()
+
+    def get_merge_temp_records_statements(self):
+        """Yield insert and update statements to merge temporary tables into target tables
+
+        This method yield SQL statements inserting the data of the temporary table (prefixed)
+        into the target tables (unprefixed). It deals with primary keys and foreign keys by
+        looking up first existing records with the same hash in order to reuse already existing
+        records when the new record is identical.
+
+        This method should not be called directly but through the save_db method in the Document
+        class, which will ensure that merge queries are issued in the correct order for all the
+        data flow, and which will encapsulated all queries in a transaction in order to rollback
+        changes on failure.
+        """
+
+        # find matching records hash in target table
+        yield self.temp_table.update().values(temp_exists=True).where(
+            getattr(self.temp_table.c, "record_hash")  # noqa: Linter puzzled by ==
+            == getattr(self.table.c, "record_hash")
+        )
+
+        # update foreign keys for n-1 relations tables
+        for rel in self.relations_1.values():
+            yield from rel.get_merge_temp_records_statements()
+
+        # insert missing records from temp table to target
+        cols = [
+            col_name
+            for col_name in self.temp_table.columns.keys()
+            if not col_name.startswith("temp_") and col_name != f"pk_{self.name}"
+        ]
+        sel = select(*[getattr(self.temp_table.c, col) for col in cols]).where(
+            self.temp_table.c.temp_exists
+            == False  # noqa: SQLAlchemy not supporting "is False"
+        )
+        yield self.table.insert().from_select(cols, sel)
+
+        # update primary keys back in temp table
+        yield self.temp_table.update().values(
+            **{f"pk_{self.name}": getattr(self.table.c, f"pk_{self.name}")}
+        ).where(
+            getattr(self.temp_table.c, "record_hash")  # noqa: Linter puzzled by ==
+            == getattr(self.table.c, "record_hash")
+        )
+
+        # update primary keys for n-n relations tables
+        for rel in self.relations_n.values():
+            yield from rel.get_merge_temp_records_statements()
```

### Comparing `xml2db-0.10.0/src/xml2db/table/table.py` & `xml2db-0.9.4/src/xml2db/table/table.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,356 +1,356 @@
-from typing import Iterable, List, Any, Union, TYPE_CHECKING
-import logging
-import sqlalchemy
-from sqlalchemy import Table
-from sqlalchemy.schema import CreateTable, CreateIndex
-
-from xml2db.table.column import DataModelColumn
-from xml2db.table.relations import DataModelRelation1, DataModelRelationN
-from xml2db.exceptions import DataModelConfigError
-
-if TYPE_CHECKING:
-    from xml2db.model import DataModel
-
-logger = logging.getLogger(__name__)
-
-
-class DataModelTable:
-    """A class representing a database table translated from an XML schema complex type
-
-    :param table_name: the table's name
-    :param type_name: the XSD complex type name
-    :param is_root_table: is this table the root table?
-    :param is_virtual_node: was this table created to store multiple root elements?
-    :param metadata: :class:`sqlalchemy.Metadata` object to build sqlalchemy models into
-    :param config: model's configuration
-    :param db_schema: database schema to use
-    :param temp_prefix: temp prefix to use for naming temp tables
-    :param data_model: the `DataModel` instance
-    :ivar model_group: 'choice' or 'sequence', extracted from the XSD. 'choice' means that only one field \
-    can have a value at the same time
-    :ivar is_root_table: is this table the root table?
-    :ivar fields: a list of tuples describing all table fields, ordered, in the form (type, name, object) where \
-    type can be "col", "rel1" or "reln", name is the name of the column or relation, and object is the column \
-    or relationship object
-    :ivar columns: a dict of all columns (fields with simple values), keyed by field name
-    :ivar relations_1: a dict of 0-1 or 1-1 relations, keyed by field name
-    :ivar relations_n: a dict of 0-n or 1-n relations, keyed by field name
-    """
-
-    is_reused = None
-
-    def __init__(
-        self,
-        table_name: str,
-        type_name: str,
-        is_root_table: bool,
-        is_virtual_node: bool,
-        metadata: sqlalchemy.MetaData,
-        config: dict,
-        db_schema: str,
-        temp_prefix: str,
-        data_model: "DataModel",
-    ):
-        """Constructor method"""
-        # config attributes
-        self.name = table_name
-        self.type_name = type_name
-        self.is_root_table = is_root_table
-        self.is_virtual_node = is_virtual_node
-        self.model_group = "sequence"
-        self.config = {} if config is None else config
-        if "as_columnstore" in self.config:
-            if not isinstance(self.config["as_columnstore"], bool):
-                raise DataModelConfigError("as_columnstore must be a bool")
-            if (
-                self.config["as_columnstore"]
-                and data_model.engine
-                and not data_model.engine.dialect.name == "mssql"
-            ):
-                self.config["as_columnstore"] = False
-                logger.warning(
-                    "Clustered columnstore indexes are only supported with MS SQL Server database"
-                )
-        else:
-            self.config["as_columnstore"] = data_model.model_config["as_columnstore"]
-        self.db_schema = db_schema
-        self.temp_prefix = temp_prefix
-        # fields (columns and relations)
-        self.fields = []
-        self.columns = {}
-        self.relations_1 = {}
-        self.relations_n = {}
-        # dependencies logic
-        self.is_simplified = False  # is the table already simplified ? (used in the simplification process)
-        self.parents_1 = (
-            set()
-        )  # a set of 1-1 relations the table is involved in as a child
-        self.parents_n = (
-            set()
-        )  # a set of 1-n relations the table is involved in as a child
-        self.parent = None
-        self.dependencies = (
-            set()
-        )  # a set of tables this table depends on (can be children or parents)
-        self.referenced_as_fk = False
-        # sqlalchemy objects
-        self.metadata = metadata
-        self.table = None
-        self.temp_table = None
-        self.data_model = data_model
-
-    def add_column(
-        self,
-        name: str,
-        data_type: str,
-        occurs: List[int],
-        min_length: int,
-        max_length: Union[int, None],
-        is_attr: bool,
-        is_content: bool,
-        allow_empty: bool,
-        ngroup: Union[str, None],
-    ) -> None:
-        """Helper to add a new column to the model
-
-        :param name: name of the column
-        :param data_type: data type
-        :param occurs: min and max occurrences
-        :param min_length: minimum length
-        :param max_length: maximum length
-        :param is_attr: is XML attribute or element?
-        :param is_content: is content of a mixed type element?
-        :param allow_empty: is nullable?
-        :param ngroup: a string id signaling that the column belongs to a nested sequence
-        """
-        self.columns[name] = DataModelColumn(
-            name,
-            [(name, None)],
-            data_type,
-            occurs,
-            min_length,
-            max_length,
-            is_attr,
-            is_content,
-            allow_empty,
-            ngroup,
-            self.config,
-            self.data_model,
-        )
-        self.fields.append(("col", name, self.columns[name]))
-
-    def add_relation_1(
-        self,
-        name: str,
-        other_table: "DataModelTable",
-        occurs: List[int],
-        ngroup: Union[str, None],
-    ) -> None:
-        """Helper to add a 1-to-1 relationship
-
-        :param name: name of the 1-1 relationship
-        :param other_table: the child table of the relationship
-        :param occurs: min and max occurs for this relationship
-        :param ngroup: a string id signaling that the relation belongs to a nested sequence
-        """
-        if occurs[1] != 1:
-            raise ValueError(
-                "attempting to add a 1-1 relationship with max occurrences different from 1"
-            )
-        rel = DataModelRelation1(
-            name,
-            [(name, other_table.type_name)],
-            self,
-            other_table,
-            occurs,
-            ngroup,
-            self.data_model,
-        )
-        self.relations_1[name] = rel
-        self.fields.append(("rel1", name, rel))
-        other_table.parents_1.add(rel)
-
-    def add_relation_n(self, name, other_table, occurs, ngroup):
-        """Helper to add a 1-to-many relationship
-
-        :param name: name of the 1-1 relationship
-        :param other_table: the child table of the relationship
-        :param occurs: min and max occurs for this relationship
-        :param ngroup: a string id signaling that the relation belongs to a nested sequence
-        """
-        if occurs[1] == 1:
-            raise ValueError(
-                "attempting to add a 1-n relationship with max occurrences equal to 1"
-            )
-        rel = DataModelRelationN(
-            name,
-            [(name, other_table.type_name)],
-            self,
-            other_table,
-            occurs,
-            ngroup,
-            self.data_model,
-        )
-        self.relations_n[name] = rel
-        self.fields.append(("reln", name, rel))
-        other_table.parents_n.add(rel)
-
-    def compute_dependencies(self) -> None:
-        """Compute the table's dependencies according to foreign keys relationships.
-
-        Dependencies are tables that the current table holds foreign keys relationships to (i.e. the one which need
-        to exist before this one can be created, for instance). To compute `dependencies` list, it ignores fk referenced
-        in relationship tables for n-n relationships. For `referenced_as_fk` it is more litteral and include those.
-
-        This function should be called after schema simplification because dependencies will not \
-        be properly updated during the simplification process.
-        """
-        # we drop parents information which is no longer accurate after schema simplification
-        self.parents_1 = None
-        self.parents_n = None
-        for field_type, rel_name, relation in self.fields:
-            if field_type == "rel1" or field_type == "reln":
-                if (
-                    relation.other_table.parent is not None
-                    and not relation.other_table.is_reused
-                ):
-                    raise ValueError(
-                        f"unsupported: table {relation.other_table.name} is not reused and has more than 1 parent"
-                    )
-                relation.other_table.parent = self
-                if relation.other_table.is_reused:
-                    self.dependencies.add(relation.other_table.type_name)
-                    relation.other_table.referenced_as_fk = True
-                    if (
-                        field_type == "reln"
-                    ):  # the relationship table will create a fk constraint to self
-                        self.referenced_as_fk = True
-                else:
-                    relation.other_table.dependencies.add(self.type_name)
-                    self.referenced_as_fk = True
-
-    def _set_db_schema(self) -> None:
-        """Set db schema value for sqlalchemy tables objects"""
-        if (
-            self.db_schema is not None
-            and self.table is not None
-            and self.temp_table is not None
-        ):
-            # sqlalchemy.Table.schema is the db_schema
-            self.table.schema = self.db_schema
-            self.temp_table.schema = self.db_schema
-
-    def get_create_table_statements(self, temp=False) -> Iterable[CreateTable]:
-        """Yield create table statements for the table and the rel tables
-
-        :param temp: if True, yield create table statements for temporary tables (prefixed)
-        """
-        if temp:
-            yield CreateTable(self.temp_table)
-            for relation in self.relations_n.values():
-                if relation.temp_rel_table is not None:
-                    yield CreateTable(relation.temp_rel_table)
-        else:
-            yield CreateTable(self.table)
-            for relation in self.relations_n.values():
-                if relation.rel_table is not None:
-                    yield CreateTable(relation.rel_table)
-
-    def get_create_index_statements(self) -> Iterable[CreateIndex]:
-        """Yield create index statements for the indexes of the table and its relation tables"""
-
-        def yield_indexes(table: Table) -> Iterable[CreateIndex]:
-            indexes = [index for index in table.indexes]
-            # Sort to guarantee indexes statements of a same table are printed in the same order everytime, otherwise
-            # the order is random, and it may create useless git changes in the output folder
-            indexes.sort(key=lambda index: index.name)
-            for index in indexes:
-                yield CreateIndex(index)
-
-        yield from yield_indexes(self.table)
-
-        for relation in self.relations_n.values():
-            if relation.rel_table is not None:
-                yield from yield_indexes(relation.rel_table)
-
-    def create_tables(self, engine: sqlalchemy.engine.base.Engine, temp: bool = False):
-        """Create tables, either target tables or temp tables used to import data
-
-        :param engine: a sqlalchemy engine to use
-        :param temp: if True, create temporary (prefixed) tables
-        """
-        if temp:
-            self.temp_table.create(engine, checkfirst=True)
-        else:
-            self.table.create(engine, checkfirst=True)
-        for relation in self.relations_n.values():
-            relation.create_table(engine, temp)
-
-    def get_insert_temp_records_statements(self, data: dict) -> Iterable[Any]:
-        """Yield drop table if exists, create table and insert statement for temporary tables"""
-        if data is not None and len(data["records"]) > 0:
-            yield self.temp_table.insert(), data["records"]
-            data_rel = data.get("relations_n", {})
-            for relation in self.relations_n.values():
-                if (
-                    relation.rel_table_name in data_rel
-                    and len(data_rel[relation.rel_table_name]["records"]) > 0
-                ):
-                    yield relation.temp_rel_table.insert(), data_rel[
-                        relation.rel_table_name
-                    ]["records"]
-
-    def drop_tables(self, engine: sqlalchemy.engine.base.Engine) -> None:
-        """Drop target (unprefixed) tables (main table and relations)
-
-        BE CAUTIOUS, THIS METHOD DROPS TABLES WITHOUT FURTHER NOTICE!
-
-        :param engine: a sqlalchemy engine to use
-        """
-        for rel in self.relations_n.values():
-            if rel.rel_table is not None:
-                rel.rel_table.drop(engine, checkfirst=True)
-        self.table.drop(engine, checkfirst=True)
-
-    def drop_temp_tables(self, engine: sqlalchemy.engine.base.Engine) -> None:
-        """Drop temporary (prefixed) tables (main table and relations)
-
-        BE CAUTIOUS, THIS METHOD DROPS TABLES WITHOUT FURTHER NOTICE!
-
-        :param engine: a sqlalchemy engine to use
-        """
-        for rel in self.relations_n.values():
-            if rel.temp_rel_table is not None:
-                rel.temp_rel_table.drop(engine, checkfirst=True)
-        self.temp_table.drop(engine, checkfirst=True)
-
-    def get_entity_rel_diagram(self) -> List:
-        """Build ERD representation for a single table and its relationships
-
-        The string representation is used by mermaid.js to create a visual diagram.
-
-        :return: a list of strings (lines)
-        """
-        out = (
-            [
-                f"{self.name} ||--{'o' if rel.occurs[0] == 0 else '|'}| {rel.other_table.name} : "
-                f'"{rel.name}"'
-                for rel in self.relations_1.values()
-            ]
-            + [
-                f"{self.name} ||--{'o' if rel.occurs[0] == 0 else '|'}{{ {rel.other_table.name} : "
-                f"\"{rel.name}{'*' if rel.other_table.is_reused else ''}\""
-                for rel in self.relations_n.values()
-            ]
-            + [f"{self.name} {{"]
-            + [
-                (
-                    f"    {self.columns[field[1]].data_type}{'-N' if self.columns[field[1]].occurs[1] is None else ''} "
-                    f"{field[1].replace('.', '_')}"
-                )
-                for field in self.fields
-                if field[0] == "col"
-            ]
-            + ["}"]
-        )
-        return [f"    {line}" for line in out]
+from typing import Iterable, List, Any, Union, TYPE_CHECKING
+import logging
+import sqlalchemy
+from sqlalchemy import Table
+from sqlalchemy.schema import CreateTable, CreateIndex
+
+from xml2db.table.column import DataModelColumn
+from xml2db.table.relations import DataModelRelation1, DataModelRelationN
+from xml2db.exceptions import DataModelConfigError
+
+if TYPE_CHECKING:
+    from xml2db.model import DataModel
+
+logger = logging.getLogger(__name__)
+
+
+class DataModelTable:
+    """A class representing a database table translated from an XML schema complex type
+
+    :param table_name: the table's name
+    :param type_name: the XSD complex type name
+    :param is_root_table: is this table the root table?
+    :param is_virtual_node: was this table created to store multiple root elements?
+    :param metadata: :class:`sqlalchemy.Metadata` object to build sqlalchemy models into
+    :param config: model's configuration
+    :param db_schema: database schema to use
+    :param temp_prefix: temp prefix to use for naming temp tables
+    :param data_model: the `DataModel` instance
+    :ivar model_group: 'choice' or 'sequence', extracted from the XSD. 'choice' means that only one field \
+    can have a value at the same time
+    :ivar is_root_table: is this table the root table?
+    :ivar fields: a list of tuples describing all table fields, ordered, in the form (type, name, object) where \
+    type can be "col", "rel1" or "reln", name is the name of the column or relation, and object is the column \
+    or relationship object
+    :ivar columns: a dict of all columns (fields with simple values), keyed by field name
+    :ivar relations_1: a dict of 0-1 or 1-1 relations, keyed by field name
+    :ivar relations_n: a dict of 0-n or 1-n relations, keyed by field name
+    """
+
+    is_reused = None
+
+    def __init__(
+        self,
+        table_name: str,
+        type_name: str,
+        is_root_table: bool,
+        is_virtual_node: bool,
+        metadata: sqlalchemy.MetaData,
+        config: dict,
+        db_schema: str,
+        temp_prefix: str,
+        data_model: "DataModel",
+    ):
+        """Constructor method"""
+        # config attributes
+        self.name = table_name
+        self.type_name = type_name
+        self.is_root_table = is_root_table
+        self.is_virtual_node = is_virtual_node
+        self.model_group = "sequence"
+        self.config = {} if config is None else config
+        if "as_columnstore" in self.config:
+            if not isinstance(self.config["as_columnstore"], bool):
+                raise DataModelConfigError("as_columnstore must be a bool")
+            if (
+                self.config["as_columnstore"]
+                and data_model.engine
+                and not data_model.engine.dialect.name == "mssql"
+            ):
+                self.config["as_columnstore"] = False
+                logger.warning(
+                    "Clustered columnstore indexes are only supported with MS SQL Server database"
+                )
+        else:
+            self.config["as_columnstore"] = data_model.model_config["as_columnstore"]
+        self.db_schema = db_schema
+        self.temp_prefix = temp_prefix
+        # fields (columns and relations)
+        self.fields = []
+        self.columns = {}
+        self.relations_1 = {}
+        self.relations_n = {}
+        # dependencies logic
+        self.is_simplified = False  # is the table already simplified ? (used in the simplification process)
+        self.parents_1 = (
+            set()
+        )  # a set of 1-1 relations the table is involved in as a child
+        self.parents_n = (
+            set()
+        )  # a set of 1-n relations the table is involved in as a child
+        self.parent = None
+        self.dependencies = (
+            set()
+        )  # a set of tables this table depends on (can be children or parents)
+        self.referenced_as_fk = False
+        # sqlalchemy objects
+        self.metadata = metadata
+        self.table = None
+        self.temp_table = None
+        self.data_model = data_model
+
+    def add_column(
+        self,
+        name: str,
+        data_type: str,
+        occurs: List[int],
+        min_length: int,
+        max_length: Union[int, None],
+        is_attr: bool,
+        is_content: bool,
+        allow_empty: bool,
+        ngroup: Union[str, None],
+    ) -> None:
+        """Helper to add a new column to the model
+
+        :param name: name of the column
+        :param data_type: data type
+        :param occurs: min and max occurrences
+        :param min_length: minimum length
+        :param max_length: maximum length
+        :param is_attr: is XML attribute or element?
+        :param is_content: is content of a mixed type element?
+        :param allow_empty: is nullable?
+        :param ngroup: a string id signaling that the column belongs to a nested sequence
+        """
+        self.columns[name] = DataModelColumn(
+            name,
+            [(name, None)],
+            data_type,
+            occurs,
+            min_length,
+            max_length,
+            is_attr,
+            is_content,
+            allow_empty,
+            ngroup,
+            self.config,
+            self.data_model,
+        )
+        self.fields.append(("col", name, self.columns[name]))
+
+    def add_relation_1(
+        self,
+        name: str,
+        other_table: "DataModelTable",
+        occurs: List[int],
+        ngroup: Union[str, None],
+    ) -> None:
+        """Helper to add a 1-to-1 relationship
+
+        :param name: name of the 1-1 relationship
+        :param other_table: the child table of the relationship
+        :param occurs: min and max occurs for this relationship
+        :param ngroup: a string id signaling that the relation belongs to a nested sequence
+        """
+        if occurs[1] != 1:
+            raise ValueError(
+                "attempting to add a 1-1 relationship with max occurrences different from 1"
+            )
+        rel = DataModelRelation1(
+            name,
+            [(name, other_table.type_name)],
+            self,
+            other_table,
+            occurs,
+            ngroup,
+            self.data_model,
+        )
+        self.relations_1[name] = rel
+        self.fields.append(("rel1", name, rel))
+        other_table.parents_1.add(rel)
+
+    def add_relation_n(self, name, other_table, occurs, ngroup):
+        """Helper to add a 1-to-many relationship
+
+        :param name: name of the 1-1 relationship
+        :param other_table: the child table of the relationship
+        :param occurs: min and max occurs for this relationship
+        :param ngroup: a string id signaling that the relation belongs to a nested sequence
+        """
+        if occurs[1] == 1:
+            raise ValueError(
+                "attempting to add a 1-n relationship with max occurrences equal to 1"
+            )
+        rel = DataModelRelationN(
+            name,
+            [(name, other_table.type_name)],
+            self,
+            other_table,
+            occurs,
+            ngroup,
+            self.data_model,
+        )
+        self.relations_n[name] = rel
+        self.fields.append(("reln", name, rel))
+        other_table.parents_n.add(rel)
+
+    def compute_dependencies(self) -> None:
+        """Compute the table's dependencies according to foreign keys relationships.
+
+        Dependencies are tables that the current table holds foreign keys relationships to (i.e. the one which need
+        to exist before this one can be created, for instance). To compute `dependencies` list, it ignores fk referenced
+        in relationship tables for n-n relationships. For `referenced_as_fk` it is more litteral and include those.
+
+        This function should be called after schema simplification because dependencies will not \
+        be properly updated during the simplification process.
+        """
+        # we drop parents information which is no longer accurate after schema simplification
+        self.parents_1 = None
+        self.parents_n = None
+        for field_type, rel_name, relation in self.fields:
+            if field_type == "rel1" or field_type == "reln":
+                if (
+                    relation.other_table.parent is not None
+                    and not relation.other_table.is_reused
+                ):
+                    raise ValueError(
+                        f"unsupported: table {relation.other_table.name} is not reused and has more than 1 parent"
+                    )
+                relation.other_table.parent = self
+                if relation.other_table.is_reused:
+                    self.dependencies.add(relation.other_table.type_name)
+                    relation.other_table.referenced_as_fk = True
+                    if (
+                        field_type == "reln"
+                    ):  # the relationship table will create a fk constraint to self
+                        self.referenced_as_fk = True
+                else:
+                    relation.other_table.dependencies.add(self.type_name)
+                    self.referenced_as_fk = True
+
+    def _set_db_schema(self) -> None:
+        """Set db schema value for sqlalchemy tables objects"""
+        if (
+            self.db_schema is not None
+            and self.table is not None
+            and self.temp_table is not None
+        ):
+            # sqlalchemy.Table.schema is the db_schema
+            self.table.schema = self.db_schema
+            self.temp_table.schema = self.db_schema
+
+    def get_create_table_statements(self, temp=False) -> Iterable[CreateTable]:
+        """Yield create table statements for the table and the rel tables
+
+        :param temp: if True, yield create table statements for temporary tables (prefixed)
+        """
+        if temp:
+            yield CreateTable(self.temp_table)
+            for relation in self.relations_n.values():
+                if relation.temp_rel_table is not None:
+                    yield CreateTable(relation.temp_rel_table)
+        else:
+            yield CreateTable(self.table)
+            for relation in self.relations_n.values():
+                if relation.rel_table is not None:
+                    yield CreateTable(relation.rel_table)
+
+    def get_create_index_statements(self) -> Iterable[CreateIndex]:
+        """Yield create index statements for the indexes of the table and its relation tables"""
+
+        def yield_indexes(table: Table) -> Iterable[CreateIndex]:
+            indexes = [index for index in table.indexes]
+            # Sort to guarantee indexes statements of a same table are printed in the same order everytime, otherwise
+            # the order is random, and it may create useless git changes in the output folder
+            indexes.sort(key=lambda index: index.name)
+            for index in indexes:
+                yield CreateIndex(index)
+
+        yield from yield_indexes(self.table)
+
+        for relation in self.relations_n.values():
+            if relation.rel_table is not None:
+                yield from yield_indexes(relation.rel_table)
+
+    def create_tables(self, engine: sqlalchemy.engine.base.Engine, temp: bool = False):
+        """Create tables, either target tables or temp tables used to import data
+
+        :param engine: a sqlalchemy engine to use
+        :param temp: if True, create temporary (prefixed) tables
+        """
+        if temp:
+            self.temp_table.create(engine, checkfirst=True)
+        else:
+            self.table.create(engine, checkfirst=True)
+        for relation in self.relations_n.values():
+            relation.create_table(engine, temp)
+
+    def get_insert_temp_records_statements(self, data: dict) -> Iterable[Any]:
+        """Yield drop table if exists, create table and insert statement for temporary tables"""
+        if data is not None and len(data["records"]) > 0:
+            yield self.temp_table.insert(), data["records"]
+            data_rel = data.get("relations_n", {})
+            for relation in self.relations_n.values():
+                if (
+                    relation.rel_table_name in data_rel
+                    and len(data_rel[relation.rel_table_name]["records"]) > 0
+                ):
+                    yield relation.temp_rel_table.insert(), data_rel[
+                        relation.rel_table_name
+                    ]["records"]
+
+    def drop_tables(self, engine: sqlalchemy.engine.base.Engine) -> None:
+        """Drop target (unprefixed) tables (main table and relations)
+
+        BE CAUTIOUS, THIS METHOD DROPS TABLES WITHOUT FURTHER NOTICE!
+
+        :param engine: a sqlalchemy engine to use
+        """
+        for rel in self.relations_n.values():
+            if rel.rel_table is not None:
+                rel.rel_table.drop(engine, checkfirst=True)
+        self.table.drop(engine, checkfirst=True)
+
+    def drop_temp_tables(self, engine: sqlalchemy.engine.base.Engine) -> None:
+        """Drop temporary (prefixed) tables (main table and relations)
+
+        BE CAUTIOUS, THIS METHOD DROPS TABLES WITHOUT FURTHER NOTICE!
+
+        :param engine: a sqlalchemy engine to use
+        """
+        for rel in self.relations_n.values():
+            if rel.temp_rel_table is not None:
+                rel.temp_rel_table.drop(engine, checkfirst=True)
+        self.temp_table.drop(engine, checkfirst=True)
+
+    def get_entity_rel_diagram(self) -> List:
+        """Build ERD representation for a single table and its relationships
+
+        The string representation is used by mermaid.js to create a visual diagram.
+
+        :return: a list of strings (lines)
+        """
+        out = (
+            [
+                f"{self.name} ||--{'o' if rel.occurs[0] == 0 else '|'}| {rel.other_table.name} : "
+                f'"{rel.name}"'
+                for rel in self.relations_1.values()
+            ]
+            + [
+                f"{self.name} ||--{'o' if rel.occurs[0] == 0 else '|'}{{ {rel.other_table.name} : "
+                f"\"{rel.name}{'*' if rel.other_table.is_reused else ''}\""
+                for rel in self.relations_n.values()
+            ]
+            + [f"{self.name} {{"]
+            + [
+                (
+                    f"    {self.columns[field[1]].data_type}{'-N' if self.columns[field[1]].occurs[1] is None else ''} "
+                    f"{field[1].replace('.', '_')}"
+                )
+                for field in self.fields
+                if field[0] == "col"
+            ]
+            + ["}"]
+        )
+        return [f"    {line}" for line in out]
```

### Comparing `xml2db-0.10.0/src/xml2db/table/transformed_table.py` & `xml2db-0.9.4/src/xml2db/table/transformed_table.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,312 +1,314 @@
-from typing import Union, List, Tuple
-
-from xml2db.exceptions import DataModelConfigError
-from .column import DataModelColumn
-from .relations import DataModelRelation1, DataModelRelationN
-from .table import DataModelTable
-
-
-class DataModelTableTransformed(DataModelTable):
-    """A class extending DataModelTable with transformations
-
-    This class allows simplifying a DataModelTable object with default or configured transformations in \
-    order to reduce final schema complexity.
-    """
-
-    def _can_choice_transform_table(self) -> bool:
-        """Check if the table is of type "choice" and can be transformed to type/value fields.
-
-        :return: True if the table model be converted to type/value choice model, False otherwise
-        """
-        if self.model_group == "choice":
-            col_types = list(set([col.data_type for col in self.columns.values()]))
-            return (
-                len(self.relations_1) == 0
-                and len(self.relations_n) == 0
-                and len(col_types) == 1
-            )
-        return False
-
-    def _is_table_choice_transform_applicable(self) -> bool:
-        """Determine if choice transform should be applied to the whole table.
-
-        We try the choice_transform value provided in config, if any, and otherwise fall back to default value.
-
-        :return: True if choice transform is to be applied, False otherwise.
-        """
-        if "choice_transform" in self.config:
-            if isinstance(self.config["choice_transform"], bool):
-                if self.config["choice_transform"]:
-                    if self._can_choice_transform_table():
-                        return True
-                    else:
-                        raise DataModelConfigError(
-                            f"Choice-transform cannot be applied to table '{self.name}', see conditions in "
-                            f"DataModelTableTransformed._can_choice_transform_table."
-                        )
-                else:
-                    return False
-            else:
-                raise DataModelConfigError(
-                    f"Unrecognized choice_transform value '{self.config['choice_transform']}'"
-                    f" for table '{self.name}'. Only boolean values True or False are allowed."
-                )
-        elif self._can_choice_transform_table() and len(self.columns) > 2:
-            # column number isn't reduced if the number of columns = 2, as it would be elevated to 2 columns then
-            return True
-        return False
-
-    def _transform_to_choice(self) -> None:
-        """Transform the current table to a choice model representation with only type and value fields"""
-        col_types = list(set([col.data_type for col in self.columns.values()]))
-        col_names = [col.name for col in self.columns.values()]
-        min_lengths = [col.min_length for col in self.columns.values()]
-        max_lengths = [col.max_length for col in self.columns.values()]
-        allow_empty = [col.allow_empty for col in self.columns.values()]
-        self.columns = {
-            "type": DataModelColumn(
-                "type",
-                [("type", None)],
-                "string",
-                [1, 1],
-                min(len(name) for name in col_names),
-                max(len(name) for name in col_names),
-                False,
-                False,
-                False,
-                None,
-                self.config,
-                self.data_model,
-            ),
-            "value": DataModelColumn(
-                "value",
-                [("value", None)],
-                col_types[0],
-                [1, 1],
-                min(min_lengths) if all(e is not None for e in min_lengths) else None,
-                max(max_lengths) if all(e is not None for e in max_lengths) else None,
-                False,
-                False,
-                any(allow_empty),
-                None,
-                self.config,
-                self.data_model,
-            ),
-        }
-        self.fields = [
-            ("col", "type", self.columns["type"]),
-            ("col", "value", self.columns["value"]),
-        ]
-
-    def _can_transform_field(
-        self, field_type: str, field_name: str, transform: str = "join"
-    ) -> bool:
-        """Check if a given transformation can be applied to a given field
-
-        :param field_type: the field type ("col", "rel1" or "reln")
-        :param field_name: the field name
-        :param transform: the transform to be tested
-        :return: True is the field can be transformed
-        """
-        if field_type == "col" and transform == "join":
-            # check if simple columns with max occurrences > 1 can be joined as string
-            if self.columns[field_name].can_join_values_as_string:
-                return True
-        elif field_type == "rel1":
-            return transform in ["elevate", "elevate_wo_prefix"]
-        # "reln" can never be transformed
-        return False
-
-    def _get_field_transform(
-        self, field_type: str, field_name: str
-    ) -> Union[str, None]:
-        """Get the transformation that should be applied to this field, taking into account user-provided config
-
-        :param field_type: the field type ("col", "rel1", "reln")
-        :param field_name: the field name
-        :return: the default transformation that should be applied
-        """
-        field_config = self.config.get("fields", {}).get(field_name, {})
-        if "transform" in field_config:
-            if field_config["transform"] is False:
-                return None
-            if self._can_transform_field(
-                field_type, field_name, field_config["transform"]
-            ):
-                return field_config["transform"]
-            else:
-                raise DataModelConfigError(
-                    f"Transform value '{field_config['transform']}' cannot be applied"
-                    f" to field '{field_name}' of table '{self.name}'."
-                )
-        else:
-            if field_type == "col":
-                if self._can_transform_field("col", field_name, "join"):
-                    return "join"
-            elif field_type == "rel1":
-                if (
-                    self.relations_1[field_name].occurs[0] == 1
-                    or len(self.relations_1[field_name].other_table.columns) <= 4
-                ) and len(self.relations_1[field_name].other_table.parents_n) == 0:
-                    return (
-                        "elevate_wo_prefix"
-                        if len(self.columns) == 0 and len(self.relations_1) == 1
-                        else "elevate"
-                    )
-
-    def _elevate_relation_1(
-        self, rel_name, transform
-    ) -> List[
-        Tuple[str, str, Union[DataModelColumn, DataModelRelation1, DataModelRelationN]]
-    ]:
-        """Elevate a child table to the upper level"""
-        rel = self.relations_1[rel_name]
-        if transform == "elevate_wo_prefix":
-            prefix = ""
-        else:
-            prefix = f"{rel.name}_"
-
-        del self.relations_1[rel_name]
-
-        # insert the children fields into the current table
-        elevated_fields = []
-        for child_field_type, key, child_field in rel.other_table.fields:
-            prefixed_key = f"{prefix}{key}"
-            if child_field_type == "col":
-                self.columns[prefixed_key] = DataModelColumn(
-                    prefixed_key,
-                    [(rel.name, rel.other_table.type_name)] + child_field.name_chain,
-                    child_field.data_type,
-                    [0, child_field.occurs[1]]
-                    if rel.occurs[0] == 0
-                    else child_field.occurs,
-                    child_field.min_length,
-                    child_field.max_length,
-                    child_field.is_attr,
-                    child_field.is_content,
-                    child_field.allow_empty,
-                    child_field.ngroup,
-                    self.config,
-                    self.data_model,
-                )
-                elevated_fields.append(
-                    (
-                        "col",
-                        prefixed_key,
-                        self.columns[prefixed_key],
-                    )
-                )
-            elif child_field_type == "rel1":
-                self.relations_1[prefixed_key] = DataModelRelation1(
-                    prefixed_key,
-                    [(rel.name, rel.other_table.type_name)] + child_field.name_chain,
-                    self,
-                    child_field.other_table,
-                    [0, child_field.occurs[1]]
-                    if rel.occurs[0] == 0
-                    else child_field.occurs,
-                    child_field.ngroup,
-                    self.data_model,
-                )
-                elevated_fields.append(
-                    (
-                        "rel1",
-                        prefixed_key,
-                        self.relations_1[prefixed_key],
-                    )
-                )
-            elif child_field_type == "reln":
-                self.relations_n[prefixed_key] = DataModelRelationN(
-                    prefixed_key,
-                    [(rel.name, rel.other_table.type_name)] + child_field.name_chain,
-                    self,
-                    child_field.other_table,
-                    [0, child_field.occurs[1]]
-                    if rel.occurs[0] == 0
-                    else child_field.occurs,
-                    child_field.ngroup,
-                    self.data_model,
-                )
-                elevated_fields.append(
-                    (
-                        "reln",
-                        prefixed_key,
-                        self.relations_n[prefixed_key],
-                    )
-                )
-        return elevated_fields
-
-    def simplify_table(self) -> Tuple[dict, dict]:
-        """Simplify table recursively and return a dict of simplifications applied
-
-        Return values are dict which associate xml types and xml field with transform operations. These dicts are used \
-        at parsing stage and should contain all xml types and field names, even if there is no transformation to apply.\
-        Transformations are described by keywords:
-           For tables (aka XML complex types):
-              - "choice_transform": transform a choice between 2+ different fields to type / value fields in order to \
-              reduce the number of columns.
-           For fields:
-              - "join": applies to fields with multiple values allowed: append all values in a comma separated string
-              - "elevate": pull up child type to parent level, appending field name to child field names
-              - "elevate_wo_prefix": same as "elevate" but keeping only child's fields names (without prefixing)
-              - False: prevents any transformation on this field
-
-
-        :return: a tuple of 2 dicts: the first one for type transforms, the second one for fields transforms
-        """
-
-        # if the table is already simplified, stop here
-        if self.is_simplified:
-            return {}, {}
-        self.is_simplified = True
-
-        # if the table can be transformed, stop here
-        if self._is_table_choice_transform_applicable():
-            self._transform_to_choice()
-            self.is_simplified = True
-            return {self.type_name: "choice"}, {}
-
-        # loop through field to transform them if need be
-        out_fields = []
-        types_transforms = {}
-        fields_transforms = {}
-        for field_type, field_name, field in self.fields:
-            if field_type == "col":
-                if self._get_field_transform("col", field_name) == "join":
-                    fields_transforms[(self.type_name, field_name)] = (
-                        None,
-                        "join",
-                    )
-                out_fields.append(("col", field_name, field))
-
-            else:
-                # simplify child table
-                (
-                    types_transforms_child,
-                    fields_transforms_child,
-                ) = field.other_table.simplify_table()
-                types_transforms.update(types_transforms_child)
-                fields_transforms.update(fields_transforms_child)
-
-                # check if children can be "elevated" to the upper level
-                transform = self._get_field_transform(field_type, field_name)
-                if transform is not None:
-                    if field_type == "rel1":
-                        elevated_fields = self._elevate_relation_1(
-                            field_name, transform
-                        )
-                        out_fields.extend(elevated_fields)
-                        fields_transforms[(self.type_name, field_name)] = (
-                            field.other_table.type_name,
-                            transform,
-                        )
-                else:
-                    out_fields.append((field_type, field_name, field))
-                    fields_transforms[(self.type_name, field_name)] = (
-                        field.other_table.type_name,
-                        None,
-                    )
-                    field.other_table.keep_table = True
-
-        self.fields = out_fields
-        return types_transforms, fields_transforms
+from typing import Union, List, Tuple
+
+from xml2db.exceptions import DataModelConfigError
+from .column import DataModelColumn
+from .relations import DataModelRelation1, DataModelRelationN
+from .table import DataModelTable
+
+
+class DataModelTableTransformed(DataModelTable):
+    """A class extending DataModelTable with transformations
+
+    This class allows simplifying a DataModelTable object with default or configured transformations in \
+    order to reduce final schema complexity.
+    """
+
+    def _can_choice_transform_table(self) -> bool:
+        """Check if the table is of type "choice" and can be transformed to type/value fields.
+
+        :return: True if the table model be converted to type/value choice model, False otherwise
+        """
+        if self.model_group == "choice":
+            col_types = list(set([col.data_type for col in self.columns.values()]))
+            return (
+                len(self.relations_1) == 0
+                and len(self.relations_n) == 0
+                and len(col_types) == 1
+            )
+        return False
+
+    def _is_table_choice_transform_applicable(self) -> bool:
+        """Determine if choice transform should be applied to the whole table.
+
+        We try the choice_transform value provided in config, if any, and otherwise fall back to default value.
+
+        :return: True if choice transform is to be applied, False otherwise.
+        """
+        if "choice_transform" in self.config:
+            if isinstance(self.config["choice_transform"], bool):
+                if self.config["choice_transform"]:
+                    if self._can_choice_transform_table():
+                        return True
+                    else:
+                        raise DataModelConfigError(
+                            f"Choice-transform cannot be applied to table '{self.name}', see conditions in "
+                            f"DataModelTableTransformed._can_choice_transform_table."
+                        )
+                else:
+                    return False
+            else:
+                raise DataModelConfigError(
+                    f"Unrecognized choice_transform value '{self.config['choice_transform']}'"
+                    f" for table '{self.name}'. Only boolean values True or False are allowed."
+                )
+        elif self._can_choice_transform_table() and len(self.columns) > 2:
+            # column number isn't reduced if the number of columns = 2, as it would be elevated to 2 columns then
+            return True
+        return False
+
+    def _transform_to_choice(self) -> None:
+        """Transform the current table to a choice model representation with only type and value fields"""
+        col_types = list(set([col.data_type for col in self.columns.values()]))
+        col_names = [col.name for col in self.columns.values()]
+        min_lengths = [col.min_length for col in self.columns.values()]
+        max_lengths = [col.max_length for col in self.columns.values()]
+        allow_empty = [col.allow_empty for col in self.columns.values()]
+        self.columns = {
+            "type": DataModelColumn(
+                "type",
+                [("type", None)],
+                "string",
+                [1, 1],
+                min(len(name) for name in col_names),
+                max(len(name) for name in col_names),
+                False,
+                False,
+                False,
+                None,
+                self.config,
+                self.data_model,
+            ),
+            "value": DataModelColumn(
+                "value",
+                [("value", None)],
+                col_types[0],
+                [1, 1],
+                min(min_lengths) if all(e is not None for e in min_lengths) else None,
+                max(max_lengths) if all(e is not None for e in max_lengths) else None,
+                False,
+                False,
+                any(allow_empty),
+                None,
+                self.config,
+                self.data_model,
+            ),
+        }
+        self.fields = [
+            ("col", "type", self.columns["type"]),
+            ("col", "value", self.columns["value"]),
+        ]
+
+    def _can_transform_field(
+        self, field_type: str, field_name: str, transform: str = "join"
+    ) -> bool:
+        """Check if a given transformation can be applied to a given field
+
+        :param field_type: the field type ("col", "rel1" or "reln")
+        :param field_name: the field name
+        :param transform: the transform to be tested
+        :return: True is the field can be transformed
+        """
+        if field_type == "col" and transform == "join":
+            # check if simple columns with max occurrences > 1 can be joined as string
+            if self.columns[field_name].can_join_values_as_string:
+                return True
+        elif field_type == "rel1":
+            return transform in ["elevate", "elevate_wo_prefix"]
+        # "reln" can never be transformed
+        return False
+
+    def _get_field_transform(
+        self, field_type: str, field_name: str
+    ) -> Union[str, None]:
+        """Get the transformation that should be applied to this field, taking into account user-provided config
+
+        :param field_type: the field type ("col", "rel1", "reln")
+        :param field_name: the field name
+        :return: the default transformation that should be applied
+        """
+        field_config = self.config.get("fields", {}).get(field_name, {})
+        if "transform" in field_config:
+            if field_config["transform"] is False:
+                return None
+            if self._can_transform_field(
+                field_type, field_name, field_config["transform"]
+            ):
+                return field_config["transform"]
+            else:
+                raise DataModelConfigError(
+                    f"Transform value '{field_config['transform']}' cannot be applied"
+                    f" to field {field_name} of table '{self.name}'."
+                )
+        else:
+            if field_type == "col":
+                if self._can_transform_field("col", field_name, "join"):
+                    return "join"
+            elif field_type == "rel1":
+                if (
+                    self.relations_1[field_name].occurs[0] == 1
+                    or len(self.relations_1[field_name].other_table.columns) <= 4
+                ) and len(self.relations_1[field_name].other_table.parents_n) == 0:
+                    transform = (
+                        "elevate_wo_prefix"
+                        if len(self.columns) == 0 and len(self.relations_1) == 1
+                        else "elevate"
+                    )
+                    if self._can_transform_field("rel1", field_name, transform):
+                        return transform
+
+    def _elevate_relation_1(
+        self, rel_name, transform
+    ) -> List[
+        Tuple[str, str, Union[DataModelColumn, DataModelRelation1, DataModelRelationN]]
+    ]:
+        """Elevate a child table to the upper level"""
+        rel = self.relations_1[rel_name]
+        if transform == "elevate_wo_prefix":
+            prefix = ""
+        else:
+            prefix = f"{rel.name}_"
+
+        del self.relations_1[rel_name]
+
+        # insert the children fields into the current table
+        elevated_fields = []
+        for child_field_type, key, child_field in rel.other_table.fields:
+            prefixed_key = f"{prefix}{key}"
+            if child_field_type == "col":
+                self.columns[prefixed_key] = DataModelColumn(
+                    prefixed_key,
+                    [(rel.name, rel.other_table.type_name)] + child_field.name_chain,
+                    child_field.data_type,
+                    [0, child_field.occurs[1]]
+                    if rel.occurs[0] == 0
+                    else child_field.occurs,
+                    child_field.min_length,
+                    child_field.max_length,
+                    child_field.is_attr,
+                    child_field.is_content,
+                    child_field.allow_empty,
+                    child_field.ngroup,
+                    self.config,
+                    self.data_model,
+                )
+                elevated_fields.append(
+                    (
+                        "col",
+                        prefixed_key,
+                        self.columns[prefixed_key],
+                    )
+                )
+            elif child_field_type == "rel1":
+                self.relations_1[prefixed_key] = DataModelRelation1(
+                    prefixed_key,
+                    [(rel.name, rel.other_table.type_name)] + child_field.name_chain,
+                    self,
+                    child_field.other_table,
+                    [0, child_field.occurs[1]]
+                    if rel.occurs[0] == 0
+                    else child_field.occurs,
+                    child_field.ngroup,
+                    self.data_model,
+                )
+                elevated_fields.append(
+                    (
+                        "rel1",
+                        prefixed_key,
+                        self.relations_1[prefixed_key],
+                    )
+                )
+            elif child_field_type == "reln":
+                self.relations_n[prefixed_key] = DataModelRelationN(
+                    prefixed_key,
+                    [(rel.name, rel.other_table.type_name)] + child_field.name_chain,
+                    self,
+                    child_field.other_table,
+                    [0, child_field.occurs[1]]
+                    if rel.occurs[0] == 0
+                    else child_field.occurs,
+                    child_field.ngroup,
+                    self.data_model,
+                )
+                elevated_fields.append(
+                    (
+                        "reln",
+                        prefixed_key,
+                        self.relations_n[prefixed_key],
+                    )
+                )
+        return elevated_fields
+
+    def simplify_table(self) -> Tuple[dict, dict]:
+        """Simplify table recursively and return a dict of simplifications applied
+
+        Return values are dict which associate xml types and xml field with transform operations. These dicts are used \
+        at parsing stage and should contain all xml types and field names, even if there is no transformation to apply.\
+        Transformations are described by keywords:
+           For tables (aka XML complex types):
+              - "choice_transform": transform a choice between 2+ different fields to type / value fields in order to \
+              reduce the number of columns.
+           For fields:
+              - "join": applies to fields with multiple values allowed: append all values in a comma separated string
+              - "elevate": pull up child type to parent level, appending field name to child field names
+              - "elevate_wo_prefix": same as "elevate" but keeping only child's fields names (without prefixing)
+              - False: prevents any transformation on this field
+
+
+        :return: a tuple of 2 dicts: the first one for type transforms, the second one for fields transforms
+        """
+
+        # if the table is already simplified, stop here
+        if self.is_simplified:
+            return {}, {}
+        self.is_simplified = True
+
+        # if the table can be transformed, stop here
+        if self._is_table_choice_transform_applicable():
+            self._transform_to_choice()
+            self.is_simplified = True
+            return {self.type_name: "choice"}, {}
+
+        # loop through field to transform them if need be
+        out_fields = []
+        types_transforms = {}
+        fields_transforms = {}
+        for field_type, field_name, field in self.fields:
+            if field_type == "col":
+                if self._get_field_transform("col", field_name) == "join":
+                    fields_transforms[(self.type_name, field_name)] = (
+                        None,
+                        "join",
+                    )
+                out_fields.append(("col", field_name, field))
+
+            else:
+                # simplify child table
+                (
+                    types_transforms_child,
+                    fields_transforms_child,
+                ) = field.other_table.simplify_table()
+                types_transforms.update(types_transforms_child)
+                fields_transforms.update(fields_transforms_child)
+
+                # check if children can be "elevated" to the upper level
+                transform = self._get_field_transform(field_type, field_name)
+                if transform is not None:
+                    if field_type == "rel1":
+                        elevated_fields = self._elevate_relation_1(
+                            field_name, transform
+                        )
+                        out_fields.extend(elevated_fields)
+                        fields_transforms[(self.type_name, field_name)] = (
+                            field.other_table.type_name,
+                            transform,
+                        )
+                else:
+                    out_fields.append((field_type, field_name, field))
+                    fields_transforms[(self.type_name, field_name)] = (
+                        field.other_table.type_name,
+                        None,
+                    )
+                    field.other_table.keep_table = True
+
+        self.fields = out_fields
+        return types_transforms, fields_transforms
```

### Comparing `xml2db-0.10.0/src/xml2db.egg-info/PKG-INFO` & `xml2db-0.9.4/src/xml2db.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-Metadata-Version: 2.1
-Name: xml2db
-Version: 0.10.0
-Summary: Import complex XML files to a relational database
-Author-email: Commission de régulation de l'énergie <opensource@cre.fr>
-Project-URL: Documentation, https://cre-dev.github.io/xml2db
-Project-URL: Repository, https://github.com/cre-dev/xml2db
-Project-URL: Issues page, https://github.com/cre-dev/xml2db/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: sqlalchemy>1.4
-Requires-Dist: xmlschema==3.1.0
-Requires-Dist: lxml==5.1.0
-Provides-Extra: docs
-Requires-Dist: mkdocs-material==9.5.23; extra == "docs"
-Requires-Dist: mkdocstrings-python==1.10.2; extra == "docs"
-Provides-Extra: tests
-Requires-Dist: pytest>=7.0; extra == "tests"
-
-# Xml2db
-
-`xml2db` is a Python package which allows loading XML data into a relational database. It is designed to handle complex 
-schemas which cannot be easily denormalized to a flat table, without any custom code.
-
-It builds a data model (i.e. a set of database tables linked with foreign keys relationships) based on a XSD schema and
-allows parsing and loading XML files into the database, and get them back to XML, if needed.
-
-It is as simple as:
-
-```python
-from xml2db import DataModel
-
-# Create a data model of tables with relations based on the XSD file
-data_model = DataModel(
-    xsd_file="path/to/file.xsd", 
-    connection_string="postgresql+psycopg2://testuser:testuser@localhost:5432/testdb",
-)
-# Parse an XML file based on this XSD
-document = data_model.parse_xml(
-    xml_file="path/to/file.xml"
-)
-# Insert the document content into the database
-document.insert_into_target_tables()
-```
-
-The data model will adhere closely to the XSD schema, but `xml2db` will perform simplifications aimed at limiting the 
-complexity of the resulting data model and the storage footprint.
-
-The raw data loaded into the database can then be processed using [DBT](https://www.getdbt.com/), SQL views or 
-other tools aimed at extracting, correcting and formatting the data into more user-friendly tables.
-
-`xml2db` is developed and used at the [French energy regulation authority (CRE)](https://www.cre.fr/) to process XML 
-data.
-
-This package uses `sqlalchemy` to interact with the database, so it should work with different database backends. 
-Automated integration tests run against PostgreSQL, MySQL and MS SQL Server. `xml2db` does not work with SQLite. You may
-have to install additional packages to connect to your database (e.g. `psycopg2` for PostgreSQL, `pymysql` for MySQL or 
-`pyodbc` for MS SQL Server).
-
-**Please read the [package documentation website](https://cre-dev.github.io/xml2db) for all the details!**
-
-## Installation
-
-The package can be installed, preferably in a virtual environment, using `pip`:
-
-``` bash
-pip install xml2db
-```
-
-## Testing
-
-Running the tests requires installing additional development dependencies, after cloning the repo, with:
-
-```bash
-pip install -e .[tests,docs]
-```
-
-Run all tests with the following command:
-
-```bash
-python -m pytest
-```
-
-Integration tests require write access to a PostgreSQL or MS SQL Server database; the connection string is provided as an
-environment variable `DB_STRING`. If you want to run only conversion tests that do not require a database you can run:
-
-```bash
-pytest -m "not dbtest"
-`````
-
-## Contributing
-
-Contributions are more than welcome, as well as bug reports, starting with the project's 
-[issue page](https://github.com/cre-dev/xml2db/issues).
+Metadata-Version: 2.1
+Name: xml2db
+Version: 0.9.4
+Summary: Import complex XML files to a relational database
+Author-email: Commission de régulation de l'énergie <opensource@cre.fr>
+Project-URL: Documentation, https://cre-dev.github.io/xml2db
+Project-URL: Repository, https://github.com/cre-dev/xml2db
+Project-URL: Issues page, https://github.com/cre-dev/xml2db/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sqlalchemy>1.4
+Requires-Dist: xmlschema==3.1.0
+Requires-Dist: lxml==5.1.0
+Provides-Extra: docs
+Requires-Dist: mkdocs-material==9.5.14; extra == "docs"
+Requires-Dist: mkdocstrings[python]==0.24.1; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: pytest>=7.0; extra == "tests"
+
+# Xml2db
+
+`xml2db` is a Python package which allows loading XML data into a relational database. It is designed to handle complex 
+schemas which cannot be easily denormalized to a flat table, without any custom code.
+
+It builds a data model (i.e. a set of database tables linked with foreign keys relationships) based on a XSD schema and
+allows parsing and loading XML files into the database, and get them back to XML, if needed.
+
+It is as simple as:
+
+```python
+from xml2db import DataModel
+
+# Create a data model of tables with relations based on the XSD file
+data_model = DataModel(
+    xsd_file="path/to/file.xsd", 
+    connection_string="postgresql+psycopg2://testuser:testuser@localhost:5432/testdb",
+)
+# Parse an XML file based on this XSD
+document = data_model.parse_xml(
+    xml_file="path/to/file.xml"
+)
+# Insert the document content into the database
+document.insert_into_target_tables()
+```
+
+The data model will adhere closely to the XSD schema, but `xml2db` will perform simplifications aimed at limiting the 
+complexity of the resulting data model and the storage footprint.
+
+The raw data loaded into the database can then be processed using [DBT](https://www.getdbt.com/), SQL views or 
+other tools aimed at extracting, correcting and formatting the data into more user-friendly tables.
+
+`xml2db` is developed and used at the [French energy regulation authority (CRE)](https://www.cre.fr/) to process XML 
+data.
+
+This package uses `sqlalchemy` to interact with the database, so it should work with different database backends. It has
+been tested against PostgreSQL and MS SQL Server. It currently does not work with SQLite. You may have to install 
+additional packages to connect to your database (e.g. `pyodbc` which is the default connector for MS SQL Server, or 
+`psycopg2` for PostgreSQL).  
+
+**Please read the [package documentation website](https://cre-dev.github.io/xml2db) for all the details!**
+
+## Installation
+
+The package can be installed, preferably in a virtual environment, using `pip`:
+
+``` bash
+pip install xml2db
+```
+
+## Testing
+
+Running the tests requires installing additional development dependencies, after cloning the repo, with:
+
+```bash
+pip install -e .[tests,docs]
+```
+
+Run all tests with the following command:
+
+```bash
+python -m pytest
+```
+
+Integration tests require write access to a PostgreSQL or MS SQL Server database; the connection string is provided as an
+environment variable `DB_STRING`. If you want to run only conversion tests that do not require a database you can run:
+
+```bash
+pytest -m "not dbtest"
+`````
+
+## Contributing
+
+Contributions are more than welcome, as well as bug reports, starting with the project's 
+[issue page](https://github.com/cre-dev/xml2db/issues).
```

### Comparing `xml2db-0.10.0/src/xml2db.egg-info/SOURCES.txt` & `xml2db-0.9.4/src/xml2db.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+src/debug.py
 src/xml2db/__init__.py
 src/xml2db/document.py
 src/xml2db/exceptions.py
 src/xml2db/model.py
 src/xml2db/xml_converter.py
 src/xml2db.egg-info/PKG-INFO
 src/xml2db.egg-info/SOURCES.txt
@@ -15,9 +16,8 @@
 src/xml2db/table/column.py
 src/xml2db/table/duplicated_table.py
 src/xml2db/table/relations.py
 src/xml2db/table/reused_table.py
 src/xml2db/table/table.py
 src/xml2db/table/transformed_table.py
 tests/test_conversions.py
-tests/test_models_output.py
 tests/test_roundtrip.py
```

### Comparing `xml2db-0.10.0/tests/test_roundtrip.py` & `xml2db-0.9.4/tests/test_roundtrip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,105 @@
-import os
-import pytest
-from lxml import etree
-from xml2db.xml_converter import XMLConverter
-
-from .fixtures import setup_db_model, conn_string
-from .sample_models import models
-
-
-@pytest.mark.dbtest
-@pytest.mark.parametrize(
-    "model_config",
-    [{**model, **version} for model in models for version in model["versions"]],
-)
-def test_database_xml_roundtrip(setup_db_model, model_config):
-    """A test for roundtrip insert to the database from and to XML"""
-
-    model = setup_db_model
-    xml_files = [
-        os.path.join(model_config["xml_path"], file)
-        for file in os.listdir(model_config["xml_path"])
-    ]
-
-    for file in xml_files:
-        # do parse and insert into the database
-        doc = model.parse_xml(file)
-        doc.insert_into_target_tables()
-
-    for file in xml_files:
-        doc = model.extract_from_database(
-            f"xml2db_input_file_path='{file}'", force_tz="Europe/Paris"
-        )
-
-        with open(file, "rt") as f:
-            ref_xml = f.read()
-        src = etree.parse(file).getroot()
-
-        el = doc.to_xml(nsmap=src.nsmap)
-        for key, val in src.attrib.items():
-            el.set(key, val)
-
-        xml = etree.tostring(
-            el,
-            pretty_print=True,
-            encoding="utf-8",
-            xml_declaration=True,
-        ).decode("utf-8")
-
-        assert xml == ref_xml
-
-
-@pytest.mark.dbtest
-@pytest.mark.parametrize(
-    "model_config",
-    [{**model, **version} for model in models for version in model["versions"]],
-)
-def test_database_document_tree_roundtrip(setup_db_model, model_config):
-    """A test for roundtrip insert to the database from and to document tree"""
-
-    model = setup_db_model
-    xml_files = [
-        os.path.join(model_config["xml_path"], file)
-        for file in os.listdir(model_config["xml_path"])
-    ]
-
-    for file in xml_files:
-        # do parse and insert into the database
-        doc = model.parse_xml(file)
-        doc.insert_into_target_tables()
-
-    for file in xml_files:
-        doc = model.extract_from_database(
-            f"xml2db_input_file_path='{file}'", force_tz="Europe/Paris"
-        )
-
-        # parse file to doctree for reference
-        converter = XMLConverter(model)
-        converter.parse_xml(file, file)
-
-        assert doc.flat_data_to_doc_tree() == converter.document_tree
-
-
-@pytest.mark.skip
-@pytest.mark.parametrize(
-    "model_config",
-    [
-        {**model, **version, "xml_file": xml_file}
-        for model in models
-        for xml_file in os.listdir(model["xml_path"])
-        for version in model["versions"]
-    ],
-)
-def test_database_single_document_tree_roundtrip(setup_db_model, model_config):
-    """A test for roundtrip insert to the database for a single file, useful for debugging but very slow"""
-
-    model = setup_db_model
-    file_path = os.path.join(model_config["xml_path"], model_config["xml_file"])
-
-    # do parse and insert into the database
-    doc = model.parse_xml(file_path)
-    doc.insert_into_target_tables()
-
-    doc = model.extract_from_database(
-        f"xml2db_input_file_path='{file_path}'", force_tz="Europe/Paris"
-    )
-
-    # parse file to doctree for reference
-    converter = XMLConverter(model)
-    converter.parse_xml(file_path, file_path)
-
-    assert doc.flat_data_to_doc_tree() == converter.document_tree
+import os
+import pytest
+from lxml import etree
+from xml2db.xml_converter import XMLConverter
+
+from .fixtures import setup_db_model, conn_string
+from .sample_models import models
+
+
+@pytest.mark.dbtest
+@pytest.mark.parametrize(
+    "model_config",
+    [{**model, **version} for model in models for version in model["versions"]],
+)
+def test_database_xml_roundtrip(setup_db_model, model_config):
+    """A test for roundtrip insert to the database from and to XML"""
+
+    model = setup_db_model
+    xml_files = [
+        os.path.join(model_config["xml_path"], file)
+        for file in os.listdir(model_config["xml_path"])
+    ]
+
+    for file in xml_files:
+        # do parse and insert into the database
+        doc = model.parse_xml(file)
+        doc.insert_into_target_tables()
+
+    for file in xml_files:
+        doc = model.extract_from_database(f"xml2db_input_file_path='{file}'")
+
+        with open(file, "rt") as f:
+            ref_xml = f.read()
+        src = etree.parse(file).getroot()
+
+        el = doc.to_xml(nsmap=src.nsmap)
+        for key, val in src.attrib.items():
+            el.set(key, val)
+
+        xml = etree.tostring(
+            el,
+            pretty_print=True,
+            encoding="utf-8",
+            xml_declaration=True,
+        ).decode("utf-8")
+
+        assert xml == ref_xml
+
+
+@pytest.mark.dbtest
+@pytest.mark.parametrize(
+    "model_config",
+    [{**model, **version} for model in models for version in model["versions"]],
+)
+def test_database_document_tree_roundtrip(setup_db_model, model_config):
+    """A test for roundtrip insert to the database from and to document tree"""
+
+    model = setup_db_model
+    xml_files = [
+        os.path.join(model_config["xml_path"], file)
+        for file in os.listdir(model_config["xml_path"])
+    ]
+
+    for file in xml_files:
+        # do parse and insert into the database
+        doc = model.parse_xml(file)
+        doc.insert_into_target_tables()
+
+    for file in xml_files:
+        doc = model.extract_from_database(f"xml2db_input_file_path='{file}'")
+
+        # parse file to doctree for reference
+        converter = XMLConverter(model)
+        converter.parse_xml(file, file)
+
+        assert doc.flat_data_to_doc_tree() == converter.document_tree
+
+
+@pytest.mark.skip
+@pytest.mark.parametrize(
+    "model_config",
+    [
+        {**model, **version, "xml_file": xml_file}
+        for model in models
+        for xml_file in os.listdir(model["xml_path"])
+        for version in model["versions"]
+    ],
+)
+def test_database_single_document_tree_roundtrip(setup_db_model, model_config):
+    """A test for roundtrip insert to the database for a single file, useful for debugging but very slow"""
+
+    model = setup_db_model
+    file_path = os.path.join(model_config["xml_path"], model_config["xml_file"])
+
+    # do parse and insert into the database
+    doc = model.parse_xml(file_path)
+    doc.insert_into_target_tables()
+
+    doc = model.extract_from_database(f"xml2db_input_file_path='{file_path}'")
+
+    # parse file to doctree for reference
+    converter = XMLConverter(model)
+    converter.parse_xml(file_path, file_path)
+
+    assert doc.flat_data_to_doc_tree() == converter.document_tree
```

