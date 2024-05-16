# Comparing `tmp/parameterframe-0.1.3.tar.gz` & `tmp/parameterframe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameterframe-0.1.3.tar", last modified: Wed May 15 00:09:33 2024, max compression
+gzip compressed data, was "parameterframe-0.1.4.tar", last modified: Thu May 16 01:51:27 2024, max compression
```

## Comparing `parameterframe-0.1.3.tar` & `parameterframe-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:33.055855 parameterframe-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 00:06:06.000000 parameterframe-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42951 2024-05-15 00:09:33.055855 parameterframe-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-15 00:06:06.000000 parameterframe-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:33.055855 parameterframe-0.1.3/parameterframe/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 00:09:06.000000 parameterframe-0.1.3/parameterframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    98684 2024-05-15 00:09:06.000000 parameterframe-0.1.3/parameterframe/parameterframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:33.055855 parameterframe-0.1.3/parameterframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42951 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 00:09:33.000000 parameterframe-0.1.3/parameterframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:09:33.055855 parameterframe-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:51:27.315345 parameterframe-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-16 01:46:42.000000 parameterframe-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43745 2024-05-16 01:51:27.315345 parameterframe-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-16 01:46:42.000000 parameterframe-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:51:27.315345 parameterframe-0.1.4/parameterframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 01:51:01.000000 parameterframe-0.1.4/parameterframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100447 2024-05-16 01:51:01.000000 parameterframe-0.1.4/parameterframe/parameterframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 01:51:26.000000 parameterframe-0.1.4/parameterframe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:51:27.315345 parameterframe-0.1.4/parameterframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43745 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:51:27.315345 parameterframe-0.1.4/setup.cfg
```

### Comparing `parameterframe-0.1.3/LICENSE` & `parameterframe-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `parameterframe-0.1.3/PKG-INFO` & `parameterframe-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,22 +25,18 @@
 
 
 ```python
 import sys
 import pandas as pd
 import os
 sys.path.append('../')
-from python_modules.parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
+from parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
 
 ```
 
-    /Users/insani_dei/miniconda3/envs/parameterframe/lib/python3.11/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html
-      from .autonotebook import tqdm as notebook_tqdm
-
-
 ## Content
 
 1. Adding new solution and uploading it
 2. Processing new files and creating parameter set
 3. Adding parameter set to solution and commiting
 4. Uploading parameter sets
 5. Getting latest parameter set id for solution
@@ -860,15 +856,18 @@
 
     True
 
 
 
 
 ```python
-pf2.pull_solution()
+pf2.pull_solution(
+    # optional parameter to skip pull of attributes if data pulled just for show_ methods
+    pull_attribute_values = False
+)
 ```
 
 
 
 
     True
 
@@ -914,15 +913,15 @@
       <th>0</th>
       <td>cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5</td>
       <td>new_example_solution</td>
       <td>Description of new example solution.</td>
       <td>2024-xx-xx</td>
       <td>None</td>
       <td>some text about maintainers credentials</td>
-      <td>2</td>
+      <td>6</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -959,29 +958,65 @@
       <th>insertion_datetime</th>
       <th>commited_parameters</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
+      <td>5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5</td>
+      <td>green_tiny_car_749</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-15 01:36:09</td>
+      <td>3</td>
+    </tr>
+    <tr>
+      <th>1</th>
       <td>3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf</td>
       <td>blue_tiny_television_381</td>
       <td></td>
       <td>STAGING</td>
       <td>2024-05-15 00:37:50</td>
       <td>2</td>
     </tr>
     <tr>
-      <th>1</th>
-      <td>5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5</td>
-      <td>yellow_shiny_microwave_931</td>
+      <th>2</th>
+      <td>2f3ee8e19d91a89298d40984df5e7bdd1f1a48008b2e61c88a7f6f81b4ab23f5</td>
+      <td>silver_happy_car_441</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-15 00:36:04</td>
-      <td>3</td>
+      <td>2024-05-16 00:03:25</td>
+      <td>1</td>
+    </tr>
+    <tr>
+      <th>3</th>
+      <td>82b8c5340454adf83667e59092fedbee28213475fd58ab6b3d95b4fc60f4d45f</td>
+      <td>purple_giant_television_135</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-16 00:05:43</td>
+      <td>1</td>
+    </tr>
+    <tr>
+      <th>4</th>
+      <td>dddc057bc151de9f8fb8caa834c8e13b789cf68cb53299b4c65c23f1e1310acd</td>
+      <td>red_sad_scooter_769</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-16 00:08:21</td>
+      <td>2</td>
+    </tr>
+    <tr>
+      <th>5</th>
+      <td>73ece98c90d4e0bcce8b523a8e8d2bd4290c68f2a783ea279b39fe4507e42de7</td>
+      <td>blue_fuzzy_refrigerator_297</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-15 23:57:17</td>
+      <td>1</td>
     </tr>
   </tbody>
 </table>
 </div>
```

### Comparing `parameterframe-0.1.3/README.md` & `parameterframe-0.1.4/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,62 +14,62 @@
 - contains __package_metadata__ (won't package without it)
 - falls under common license
 
 The ones that were not packages, could still be used as packages with [this instruction](https://github.com/Kiril-Mordan/reusables/blob/main/docs/module_from_raw_file.md).
 
 ## Content:
  
-[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
-
-This class uses the logging module to create and manage a logger for displaying formatted messages.
-It provides a method to output various types of lines and headers, with customizable message and line lengths.
-The purpose is to be integrated into other classes that also use logger.
-
-[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
+[module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
 
-A tool to run experiments based on defined grid and function with single iteration.
+This module provides a set of functions for interacting with the Google Drive API.
+It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
 
 [module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [release notes](release_notes/package_auto_assembler.md) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
 
 This tool is meant to streamline creation of single module packages.
 Its purpose is to automate as many aspects of python package creation as possible,
 to shorten a development cycle of reusable components, maintain certain standard of quality
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 
-[module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
-
-A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
-The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
-with a use of more expensive, slower or simply no-existant method.
-
-[module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
-
-This module provides a set of functions for interacting with the Google Drive API.
-It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
-
 [module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [release notes](release_notes/parameterframe.md) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameterframe
 
 The module provides an interface for managing solution parameters.
 It allows for the structured storage and retrieval of parameter sets from a database.
 
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
 Designed to automate and streamline the process of comparing textual data, particularly focusing on various metrics
 such as character and word count, punctuation usage, and semantic similarity.
 It's particularly useful for scenarios where consistent text analysis is required,
 such as evaluating the performance of natural language processing models, monitoring content quality,
 or tracking changes in textual data over time using manual evaluation.
 
+[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
+
+This class uses the logging module to create and manage a logger for displaying formatted messages.
+It provides a method to output various types of lines and headers, with customizable message and line lengths.
+The purpose is to be integrated into other classes that also use logger.
+
+[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
+
+A tool to run experiments based on defined grid and function with single iteration.
+
 [module](python_modules/mocker_db.py) | [usage](docs/mocker_db.md) | [drawio: -flow](docs/mocker_db-flow.png) | [release notes](release_notes/mocker_db.md) | [![PyPiVersion](https://img.shields.io/pypi/v/mocker-db)](https://pypi.org/project/mocker-db/) - MockerDB
 
 A python module that contains mock vector database like solution built around
 dictionary data type. It contains methods necessary to interact with this 'database',
 embed, search and persist.
 
 [module](python_modules/search_based_extractor.py) | [usage](docs/search_based_extractor.md) - Search Based Extractor
 
 Utility to simplify webscraping by taking advantave of search and assumptions about html structure.
 Extractor allows to find parent html element that contains searched term, record path to it in a file
 and reuse that to scrape data with same html structure.
 
+[module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
+
+A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
+The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
+with a use of more expensive, slower or simply no-existant method.
+
```

### Comparing `parameterframe-0.1.3/parameterframe/parameterframe.py` & `parameterframe-0.1.4/parameterframe/parameterframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,16 @@
 
         self.commit()
 
         return True
 
     def pull_tables(self,
                       solution_id : str = None,
-                      parameter_set_id : str = None):
+                      parameter_set_id : str = None,
+                      pull_attribute_values : bool = True):
 
         """
         Pulls commited tables from database for selected solutions
         """
 
         fetch_filters = {'table_name' : ['solution_description',
                                           'solution_parameter_set',
@@ -253,37 +254,41 @@
                           'parameter_id': param_ids})
 
         # get attribute_ids for fetching next tables
         dict_attribute_ids = self.get_entries(
             table_name = 'parameter_attribute',
             return_keys=['attribute_id'])
 
-        attribute_ids = [dict_attribute_id['attribute_id'] \
-            for dict_attribute_id in dict_attribute_ids]
-
-        # fetch final tables
-        self.fetch_entries(
-            filters={'table_name' : 'attribute_values',
-                          'attribute_id': attribute_ids})
+        if pull_attribute_values:
+            attribute_ids = [dict_attribute_id['attribute_id'] \
+                for dict_attribute_id in dict_attribute_ids]
+
+            # fetch final tables
+            self.fetch_entries(
+                filters={'table_name' : 'attribute_values',
+                            'attribute_id': attribute_ids})
 
         # get table lists from connector
         solution_description = self.get_entries(
     table_name = 'solution_description')
         solution_parameter_sets = self.get_entries(
     table_name = 'solution_parameter_set')
         parameter_sets = self.get_entries(
     table_name = 'parameter_set')
         parameter_set_descriptions = self.get_entries(
     table_name = 'parameter_set_description')
         parameter_descriptions = self.get_entries(
     table_name = 'parameter_description')
         parameter_attributes = self.get_entries(
     table_name = 'parameter_attribute')
-        attribute_values = self.get_entries(
-    table_name = 'attribute_values')
+        if pull_attribute_values:
+            attribute_values = self.get_entries(
+        table_name = 'attribute_values')
+        else:
+            attribute_values = None
 
         return (
             solution_description,
             solution_parameter_sets,
             parameter_sets,
             parameter_set_descriptions,
             parameter_descriptions,
@@ -551,15 +556,16 @@
             self._merge_entries(entries = inserts)
             return True
 
         return False
 
     def pull_tables(self,
                     solution_id : str = None,
-                    parameter_set_id : str = None):
+                    parameter_set_id : str = None,
+                    pull_attribute_values : bool = True):
 
         """
         Pulls commited tables from database for selected solutions
         """
 
         # if solution_id is None:
         #     raise ValueError("Provide solution_id!")
@@ -603,27 +609,46 @@
 
             # Continue to fetch related entries based on parameter_id
             parameter_descriptions = session.query(self.ParameterDescription).filter(
                 self.ParameterDescription.parameter_id.in_(param_ids)).all()
             parameter_attributes = session.query(self.ParameterAttribute).filter(
                 self.ParameterAttribute.parameter_id.in_(param_ids)).all()
 
-            # Get attribute_ids for fetching attribute values
-            attribute_ids = [attr.attribute_id for attr in parameter_attributes]
-            attribute_values = session.query(self.AttributeValues).filter(
-                self.AttributeValues.attribute_id.in_(attribute_ids)).all()
+            if pull_attribute_values:
+                # Get attribute_ids for fetching attribute values
+                attribute_ids = [attr.attribute_id for attr in parameter_attributes]
+                attribute_values = session.query(self.AttributeValues).filter(
+                    self.AttributeValues.attribute_id.in_(attribute_ids)).all()
+            else:
+                attribute_values = None
+
+            # transforming pulled data
+            if solution_descriptions:
+                solution_descriptions = [self._as_dict(data) for data in solution_descriptions]
+            if solution_parameter_sets:
+                solution_parameter_sets = [self._as_dict(data) for data in solution_parameter_sets]
+            if parameter_sets:
+                parameter_sets = [self._as_dict(data) for data in parameter_sets]
+            if parameter_set_descriptions:
+                parameter_set_descriptions = [self._as_dict(data) for data in parameter_set_descriptions]
+            if parameter_descriptions:
+                parameter_descriptions = [self._as_dict(data) for data in parameter_descriptions]
+            if parameter_attributes:
+                parameter_attributes = [self._as_dict(data) for data in parameter_attributes]
+            if attribute_values:
+                attribute_values = [self._as_dict(data) for data in attribute_values]
 
             return (
-                [self._as_dict(data) for data in solution_descriptions],
-                [self._as_dict(data) for data in solution_parameter_sets],
-                [self._as_dict(data) for data in parameter_sets],
-                [self._as_dict(data) for data in parameter_set_descriptions],
-                [self._as_dict(data) for data in parameter_descriptions],
-                [self._as_dict(data) for data in parameter_attributes],
-                [self._as_dict(data) for data in attribute_values]
+                solution_descriptions,
+                solution_parameter_sets,
+                parameter_sets,
+                parameter_set_descriptions,
+                parameter_descriptions,
+                parameter_attributes,
+                attribute_values
             )
 
         except Exception as e:
             session.rollback()
             print(f"An error occurred: {e}")
         finally:
             session.close()
@@ -2215,51 +2240,62 @@
                     self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id] = {}
 
                 if parameter_set_id not in self.commited_tables[solution_id]['attribute_values'].keys():
                     self.commited_tables[solution_id]['attribute_values'][parameter_set_id] = {}
 
                 for parameter_id in parameter_ids:
 
-                    # Distribute parameter_attributes
-                    self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id][parameter_id] = [
-                        parameter_attribute for parameter_attribute in parameter_attributes \
-                            if parameter_attribute['parameter_id'] == parameter_id]
+                    if parameter_attributes:
+                        # Distribute parameter_attributes
+                        self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id][parameter_id] = [
+                            parameter_attribute for parameter_attribute in parameter_attributes \
+                                if parameter_attribute['parameter_id'] == parameter_id]
+                    else:
+                        self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id][parameter_id] = []
+
+
+
+                    if attribute_values:
 
-                    attribute_ids = [parameter_attribute['attribute_id'] \
+                        attribute_ids = [parameter_attribute['attribute_id'] \
                         for parameter_attribute in parameter_attributes \
                             if parameter_attribute['parameter_id'] == parameter_id]
 
-                    # Distribute attribute_values
-                    self.commited_tables[solution_id]['attribute_values'][parameter_set_id][parameter_id] = [
-                        attribute_value for attribute_value in attribute_values \
-                            if attribute_value['attribute_id'] in attribute_ids]
+                        # Distribute attribute_values
+                        self.commited_tables[solution_id]['attribute_values'][parameter_set_id][parameter_id] = [
+                            attribute_value for attribute_value in attribute_values \
+                                if attribute_value['attribute_id'] in attribute_ids]
+                    else:
+                        self.commited_tables[solution_id]['attribute_values'][parameter_set_id][parameter_id] = []
 
         except Exception as e:
             self.logger.error("Problem during rebuilding of tables from pushed data!")
             raise e
 
 
 
     def pull_solution(self,
                       solution_id : str = None,
-                      parameter_set_id : str = None):
+                      parameter_set_id : str = None,
+                      pull_attribute_values : bool = True):
 
         """
         Pulls commited tables from database for selected solutions
         """
 
         (solution_descriptions,
          solution_parameter_sets,
          parameter_sets,
          parameter_set_descriptions,
          parameter_descriptions,
          parameter_attributes,
          attribute_values) = self.database_connector.pull_tables(
             solution_id = solution_id,
-            parameter_set_id = parameter_set_id
+            parameter_set_id = parameter_set_id,
+            pull_attribute_values = pull_attribute_values
         )
 
         if len(solution_descriptions) == 0:
             self.logger.warning(f"No solutions with {solution_id} could be pulled!")
 
         parameter_set_ids = [solution_parameter_set['parameter_set_id'] \
             for solution_parameter_set in solution_parameter_sets]
@@ -2287,16 +2323,19 @@
                         if sp['parameter_set_id'] == parameter_set_id]
 
                     parameter_set = [sp for sp in parameter_sets \
                         if sp['parameter_set_id'] == parameter_set_id]
 
                     parameter_ids = [sp['parameter_id'] for sp in parameter_set]
 
-                    parameter_description = [sp for sp in parameter_descriptions \
-                        if sp['parameter_id'] in parameter_ids]
+                    if parameter_descriptions:
+                        parameter_description = [sp for sp in parameter_descriptions \
+                            if sp['parameter_id'] in parameter_ids]
+                    else:
+                        parameter_description = None
 
                     # get table lists into commited
                     self._rebuild_tables_from_pulled_data(
                         solution_id = solution_id,
                         parameter_set_ids = [parameter_set_id],
                         solution_description = solution_description,
                         solution_parameter_sets = solution_parameter_set,
```

### Comparing `parameterframe-0.1.3/parameterframe/setup.py` & `parameterframe-0.1.4/parameterframe/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="parameterframe",
     packages=["parameterframe"],
-    install_requires=['### parameterframe.py', 'pyyaml', 'pandas', 'attrs', 'sqlalchemy', 'cryptography', 'mocker_db==0.1.1', 'dill'],
+    install_requires=['### parameterframe.py', 'pandas', 'pyyaml', 'sqlalchemy', 'attrs', 'dill', 'cryptography', 'mocker_db==0.1.1'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.3"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.4"
 )
```

### Comparing `parameterframe-0.1.3/parameterframe.egg-info/PKG-INFO` & `parameterframe-0.1.4/parameterframe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,22 +25,18 @@
 
 
 ```python
 import sys
 import pandas as pd
 import os
 sys.path.append('../')
-from python_modules.parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
+from parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
 
 ```
 
-    /Users/insani_dei/miniconda3/envs/parameterframe/lib/python3.11/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html
-      from .autonotebook import tqdm as notebook_tqdm
-
-
 ## Content
 
 1. Adding new solution and uploading it
 2. Processing new files and creating parameter set
 3. Adding parameter set to solution and commiting
 4. Uploading parameter sets
 5. Getting latest parameter set id for solution
@@ -860,15 +856,18 @@
 
     True
 
 
 
 
 ```python
-pf2.pull_solution()
+pf2.pull_solution(
+    # optional parameter to skip pull of attributes if data pulled just for show_ methods
+    pull_attribute_values = False
+)
 ```
 
 
 
 
     True
 
@@ -914,15 +913,15 @@
       <th>0</th>
       <td>cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5</td>
       <td>new_example_solution</td>
       <td>Description of new example solution.</td>
       <td>2024-xx-xx</td>
       <td>None</td>
       <td>some text about maintainers credentials</td>
-      <td>2</td>
+      <td>6</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -959,29 +958,65 @@
       <th>insertion_datetime</th>
       <th>commited_parameters</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
+      <td>5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5</td>
+      <td>green_tiny_car_749</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-15 01:36:09</td>
+      <td>3</td>
+    </tr>
+    <tr>
+      <th>1</th>
       <td>3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf</td>
       <td>blue_tiny_television_381</td>
       <td></td>
       <td>STAGING</td>
       <td>2024-05-15 00:37:50</td>
       <td>2</td>
     </tr>
     <tr>
-      <th>1</th>
-      <td>5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5</td>
-      <td>yellow_shiny_microwave_931</td>
+      <th>2</th>
+      <td>2f3ee8e19d91a89298d40984df5e7bdd1f1a48008b2e61c88a7f6f81b4ab23f5</td>
+      <td>silver_happy_car_441</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-15 00:36:04</td>
-      <td>3</td>
+      <td>2024-05-16 00:03:25</td>
+      <td>1</td>
+    </tr>
+    <tr>
+      <th>3</th>
+      <td>82b8c5340454adf83667e59092fedbee28213475fd58ab6b3d95b4fc60f4d45f</td>
+      <td>purple_giant_television_135</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-16 00:05:43</td>
+      <td>1</td>
+    </tr>
+    <tr>
+      <th>4</th>
+      <td>dddc057bc151de9f8fb8caa834c8e13b789cf68cb53299b4c65c23f1e1310acd</td>
+      <td>red_sad_scooter_769</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-16 00:08:21</td>
+      <td>2</td>
+    </tr>
+    <tr>
+      <th>5</th>
+      <td>73ece98c90d4e0bcce8b523a8e8d2bd4290c68f2a783ea279b39fe4507e42de7</td>
+      <td>blue_fuzzy_refrigerator_297</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-15 23:57:17</td>
+      <td>1</td>
     </tr>
   </tbody>
 </table>
 </div>
```

