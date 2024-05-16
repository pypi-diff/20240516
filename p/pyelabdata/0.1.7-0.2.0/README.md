# Comparing `tmp/pyelabdata-0.1.7.tar.gz` & `tmp/pyelabdata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelabdata-0.1.7.tar", last modified: Fri Feb 23 11:19:06 2024, max compression
+gzip compressed data, was "pyelabdata-0.2.0.tar", last modified: Thu May 16 10:43:33 2024, max compression
```

## Comparing `pyelabdata-0.1.7.tar` & `pyelabdata-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 11:19:06.339139 pyelabdata-0.1.7/
--rw-rw-rw-   0        0        0     1097 2024-01-25 17:49:20.000000 pyelabdata-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     7088 2024-02-23 11:19:06.338139 pyelabdata-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6185 2024-02-23 11:18:30.000000 pyelabdata-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 11:19:06.315139 pyelabdata-0.1.7/pyelabdata/
--rw-rw-rw-   0        0        0       27 2024-02-23 10:39:15.000000 pyelabdata-0.1.7/pyelabdata/__init__.py
--rw-rw-rw-   0        0        0    16095 2024-02-23 11:16:27.000000 pyelabdata-0.1.7/pyelabdata/pyelabdata.py
-drwxrwxrwx   0        0        0        0 2024-02-23 11:19:06.338139 pyelabdata-0.1.7/pyelabdata.egg-info/
--rw-rw-rw-   0        0        0     7088 2024-02-23 11:19:06.000000 pyelabdata-0.1.7/pyelabdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-02-23 11:19:06.000000 pyelabdata-0.1.7/pyelabdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 11:19:06.000000 pyelabdata-0.1.7/pyelabdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-02-23 11:19:06.000000 pyelabdata-0.1.7/pyelabdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-23 11:19:06.000000 pyelabdata-0.1.7/pyelabdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      967 2024-02-23 11:18:41.000000 pyelabdata-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-23 11:19:06.339139 pyelabdata-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 10:43:33.732818 pyelabdata-0.2.0/
+-rw-rw-rw-   0        0        0     1097 2024-01-25 17:49:20.000000 pyelabdata-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10904 2024-05-16 10:43:33.730818 pyelabdata-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9934 2024-05-16 10:06:32.000000 pyelabdata-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 10:43:33.704819 pyelabdata-0.2.0/pyelabdata/
+-rw-rw-rw-   0        0        0       27 2024-02-23 10:39:15.000000 pyelabdata-0.2.0/pyelabdata/__init__.py
+-rw-rw-rw-   0        0        0    27062 2024-05-16 10:03:05.000000 pyelabdata-0.2.0/pyelabdata/pyelabdata.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:43:33.729820 pyelabdata-0.2.0/pyelabdata.egg-info/
+-rw-rw-rw-   0        0        0    10904 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1167 2024-05-10 15:45:32.000000 pyelabdata-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 10:43:33.732818 pyelabdata-0.2.0/setup.cfg
```

### Comparing `pyelabdata-0.1.7/LICENSE` & `pyelabdata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyelabdata-0.1.7/PKG-INFO` & `pyelabdata-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: pyelabdata
-Version: 0.1.7
+Version: 0.2.0
 Summary: pyelabdata provides functions for simple one-line access to data in eLabFTW
 Author-email: "Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg" <physik-ep@fau.de>, "Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg" <michael.krieger@fau.de>
 Project-URL: Repository, https://github.com/FAU-PHYSIK-EP/pyelabdata
 Project-URL: Issues, https://github.com/FAU-PHYSIK-EP/pyelabdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: elabapi_python
 Requires-Dist: pandas
+Requires-Dist: json
+Requires-Dist: h5py
 Requires-Dist: ipyparams
 Requires-Dist: matplotlib
 Requires-Dist: pathlib
+Requires-Dist: datetime
 Requires-Dist: IPython
 
 # pyelabdata
 pyelabdata provides functions for simple one-line access to data stored
 in eLabFTW via Python or Jupyter.
 
 ## Examples
 Examples for the use of pyelabdata can be found in the examples folder.
 
 ## Functions
 
+### General functions
+
 ```python
 def connect(host: str, apikey: str):
 ```
 Connects to the API interface of the eLabFTW server specified by the
 parameter `host` (e.g. `https://yourserver.org/api/v2`) using the given
 `apikey`.
 
@@ -58,14 +63,27 @@
 
 ```python
 def close_experiment():
 ```
 Close the current experiment.
 Subsequent commands will not further operate on the experiment.
 
+### Read experiment data
+
+```python
+def get_experimentdata(expid: int=None):
+```
+Retrieve the complete data of the experiment.
+
+All parameters are optional.
+`expid` is an integer number which identifies the eLabFTW experiment; 
+if set to None, the currently opened experiment is used.
+
+The function returns a dictionary with the structured data.
+
 ```python
 def get_maintext(format: str='html', expid: int=None):
 ```
 Retrieve the body text of the experiment.
 
 All parameters are optional. If `format` is `'html'`, the content of
 body_html is returned, i.e. the body text in html format. Otherwise
@@ -88,28 +106,109 @@
 `datatype` may be either `'df'` or `'np'` (default). For `'df'`, a pandas dataframe
 representing the table data is returned, whereas for `'np'` a dictionary
 of numpy arrays for each column is returned, in which the keys correspond
 to the column heading (in case of `header = True`).
 `expid` is an integer number which identifies the eLabFTW experiment; 
 if set to None, the currently opened experiment is used.
 
+```python
+def get_extrafields(fieldname: str=None, expid: int=None):
+```
+In eLabFTW, so-called extra fields can be defined. These are
+key-value pairs, which are additionally described with units,
+value type, description and which may be grouped.
+
+All parameters are optional. If `fieldname` is None,
+all extra fields are returned as a dictionary.
+If `fieldname` is specified, the value of the entry
+is returned. If the field type is numeric or date/time,
+the return value is of the respective type.
+
+### Read files
+
+```python
+def get_file_data(filename: str, filename_is_long_name: bool=False, expid: int=None):
+```
+Get the (binary) data from a file attached to eLabFTW experiments.
+`filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
+
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`. The binary data is returned as a byte string.
 
 ```python
-def get_file_csv_data(filename: str, 
+def get_file_csv_data(filename: str, filename_is_long_name: bool=False,
                       header: bool=True, sep: str=',', 
                       datatype: str='np', expid: int=None):
 ```
 Get the data from csv files attached to eLabFTW experiments.
 `filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
 
 All other parameters are optional. `sep` is the column separator,
 by default a comma. The parameters `header`, `datatype` and `expid` have the same
 meaning as in `get_table_data()`.
 
 ```python
+def get_file_hdf5_data(filename: str, filename_is_long_name: bool=False, expid: int=None):
+```
+Get the data from a hdf5 file attached to eLabFTW experiments.
+`filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
+
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`. The function returns a hdf5 file object as 
+created by `h5py.File()`.
+
+### Update experiment data
+
+```python
+def create_extrafield(fieldname: str, value, fieldtype:str='text',
+                      unit: str=None, units=None, description: str=None,
+                      groupname: str=None,
+                      readonly: bool=False, required: bool=False,
+                      expid: int=None):
+```
+Create a new extra field with the name `fieldname` of type `fieldtype`
+(possible values: text, number, date, time, datetime; the default
+type is `text`) containing the value of `value`. 
+You can define a list of possible units in the
+parameter `units` and specify the default unit in `unit`.
+The extra field may be assigned to an extra field group with name
+`groupname`; if the group doesn't exist, it will be created.
+`readonly` and `required` control the respective property of the
+extra field. 
+Depending on `fieldtype`, `value` will automatically be converted
+to string using appropriate functions (e.g. datetime.isoformat).
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+```python
+def update_extrafield(fieldname: str, value, expid: int=None):
+```
+Update the value of the extra field with the name `fieldname`.
+Depending on the type of the extra field, 
+`value` will automatically be converted
+to string using appropriate functions (e.g. datetime.isoformat).
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+```python
+def delete_extrafield(fieldname: str, expid: int=None):
+```
+Delete the extra field with name `fieldname`.
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+### Upload files
+
+```python
 def upload_file(file: str, comment: str,
                 replacefile: bool=True, expid: int=None):
 ```
 Upload a file from local drives to an eLabFTW experiment.
 `file` is the filepath of the file to be uploaded, 
 `comment` is a description of the file.
```

### Comparing `pyelabdata-0.1.7/README.md` & `pyelabdata-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 in eLabFTW via Python or Jupyter.
 
 ## Examples
 Examples for the use of pyelabdata can be found in the examples folder.
 
 ## Functions
 
+### General functions
+
 ```python
 def connect(host: str, apikey: str):
 ```
 Connects to the API interface of the eLabFTW server specified by the
 parameter `host` (e.g. `https://yourserver.org/api/v2`) using the given
 `apikey`.
 
@@ -37,14 +39,27 @@
 
 ```python
 def close_experiment():
 ```
 Close the current experiment.
 Subsequent commands will not further operate on the experiment.
 
+### Read experiment data
+
+```python
+def get_experimentdata(expid: int=None):
+```
+Retrieve the complete data of the experiment.
+
+All parameters are optional.
+`expid` is an integer number which identifies the eLabFTW experiment; 
+if set to None, the currently opened experiment is used.
+
+The function returns a dictionary with the structured data.
+
 ```python
 def get_maintext(format: str='html', expid: int=None):
 ```
 Retrieve the body text of the experiment.
 
 All parameters are optional. If `format` is `'html'`, the content of
 body_html is returned, i.e. the body text in html format. Otherwise
@@ -67,28 +82,109 @@
 `datatype` may be either `'df'` or `'np'` (default). For `'df'`, a pandas dataframe
 representing the table data is returned, whereas for `'np'` a dictionary
 of numpy arrays for each column is returned, in which the keys correspond
 to the column heading (in case of `header = True`).
 `expid` is an integer number which identifies the eLabFTW experiment; 
 if set to None, the currently opened experiment is used.
 
+```python
+def get_extrafields(fieldname: str=None, expid: int=None):
+```
+In eLabFTW, so-called extra fields can be defined. These are
+key-value pairs, which are additionally described with units,
+value type, description and which may be grouped.
+
+All parameters are optional. If `fieldname` is None,
+all extra fields are returned as a dictionary.
+If `fieldname` is specified, the value of the entry
+is returned. If the field type is numeric or date/time,
+the return value is of the respective type.
+
+### Read files
+
+```python
+def get_file_data(filename: str, filename_is_long_name: bool=False, expid: int=None):
+```
+Get the (binary) data from a file attached to eLabFTW experiments.
+`filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
+
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`. The binary data is returned as a byte string.
 
 ```python
-def get_file_csv_data(filename: str, 
+def get_file_csv_data(filename: str, filename_is_long_name: bool=False,
                       header: bool=True, sep: str=',', 
                       datatype: str='np', expid: int=None):
 ```
 Get the data from csv files attached to eLabFTW experiments.
 `filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
 
 All other parameters are optional. `sep` is the column separator,
 by default a comma. The parameters `header`, `datatype` and `expid` have the same
 meaning as in `get_table_data()`.
 
 ```python
+def get_file_hdf5_data(filename: str, filename_is_long_name: bool=False, expid: int=None):
+```
+Get the data from a hdf5 file attached to eLabFTW experiments.
+`filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
+
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`. The function returns a hdf5 file object as 
+created by `h5py.File()`.
+
+### Update experiment data
+
+```python
+def create_extrafield(fieldname: str, value, fieldtype:str='text',
+                      unit: str=None, units=None, description: str=None,
+                      groupname: str=None,
+                      readonly: bool=False, required: bool=False,
+                      expid: int=None):
+```
+Create a new extra field with the name `fieldname` of type `fieldtype`
+(possible values: text, number, date, time, datetime; the default
+type is `text`) containing the value of `value`. 
+You can define a list of possible units in the
+parameter `units` and specify the default unit in `unit`.
+The extra field may be assigned to an extra field group with name
+`groupname`; if the group doesn't exist, it will be created.
+`readonly` and `required` control the respective property of the
+extra field. 
+Depending on `fieldtype`, `value` will automatically be converted
+to string using appropriate functions (e.g. datetime.isoformat).
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+```python
+def update_extrafield(fieldname: str, value, expid: int=None):
+```
+Update the value of the extra field with the name `fieldname`.
+Depending on the type of the extra field, 
+`value` will automatically be converted
+to string using appropriate functions (e.g. datetime.isoformat).
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+```python
+def delete_extrafield(fieldname: str, expid: int=None):
+```
+Delete the extra field with name `fieldname`.
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+### Upload files
+
+```python
 def upload_file(file: str, comment: str,
                 replacefile: bool=True, expid: int=None):
 ```
 Upload a file from local drives to an eLabFTW experiment.
 `file` is the filepath of the file to be uploaded, 
 `comment` is a description of the file.
```

### Comparing `pyelabdata-0.1.7/pyelabdata.egg-info/PKG-INFO` & `pyelabdata-0.2.0/pyelabdata.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: pyelabdata
-Version: 0.1.7
+Version: 0.2.0
 Summary: pyelabdata provides functions for simple one-line access to data in eLabFTW
 Author-email: "Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg" <physik-ep@fau.de>, "Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg" <michael.krieger@fau.de>
 Project-URL: Repository, https://github.com/FAU-PHYSIK-EP/pyelabdata
 Project-URL: Issues, https://github.com/FAU-PHYSIK-EP/pyelabdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: elabapi_python
 Requires-Dist: pandas
+Requires-Dist: json
+Requires-Dist: h5py
 Requires-Dist: ipyparams
 Requires-Dist: matplotlib
 Requires-Dist: pathlib
+Requires-Dist: datetime
 Requires-Dist: IPython
 
 # pyelabdata
 pyelabdata provides functions for simple one-line access to data stored
 in eLabFTW via Python or Jupyter.
 
 ## Examples
 Examples for the use of pyelabdata can be found in the examples folder.
 
 ## Functions
 
+### General functions
+
 ```python
 def connect(host: str, apikey: str):
 ```
 Connects to the API interface of the eLabFTW server specified by the
 parameter `host` (e.g. `https://yourserver.org/api/v2`) using the given
 `apikey`.
 
@@ -58,14 +63,27 @@
 
 ```python
 def close_experiment():
 ```
 Close the current experiment.
 Subsequent commands will not further operate on the experiment.
 
+### Read experiment data
+
+```python
+def get_experimentdata(expid: int=None):
+```
+Retrieve the complete data of the experiment.
+
+All parameters are optional.
+`expid` is an integer number which identifies the eLabFTW experiment; 
+if set to None, the currently opened experiment is used.
+
+The function returns a dictionary with the structured data.
+
 ```python
 def get_maintext(format: str='html', expid: int=None):
 ```
 Retrieve the body text of the experiment.
 
 All parameters are optional. If `format` is `'html'`, the content of
 body_html is returned, i.e. the body text in html format. Otherwise
@@ -88,28 +106,109 @@
 `datatype` may be either `'df'` or `'np'` (default). For `'df'`, a pandas dataframe
 representing the table data is returned, whereas for `'np'` a dictionary
 of numpy arrays for each column is returned, in which the keys correspond
 to the column heading (in case of `header = True`).
 `expid` is an integer number which identifies the eLabFTW experiment; 
 if set to None, the currently opened experiment is used.
 
+```python
+def get_extrafields(fieldname: str=None, expid: int=None):
+```
+In eLabFTW, so-called extra fields can be defined. These are
+key-value pairs, which are additionally described with units,
+value type, description and which may be grouped.
+
+All parameters are optional. If `fieldname` is None,
+all extra fields are returned as a dictionary.
+If `fieldname` is specified, the value of the entry
+is returned. If the field type is numeric or date/time,
+the return value is of the respective type.
+
+### Read files
+
+```python
+def get_file_data(filename: str, filename_is_long_name: bool=False, expid: int=None):
+```
+Get the (binary) data from a file attached to eLabFTW experiments.
+`filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
+
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`. The binary data is returned as a byte string.
 
 ```python
-def get_file_csv_data(filename: str, 
+def get_file_csv_data(filename: str, filename_is_long_name: bool=False,
                       header: bool=True, sep: str=',', 
                       datatype: str='np', expid: int=None):
 ```
 Get the data from csv files attached to eLabFTW experiments.
 `filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
 
 All other parameters are optional. `sep` is the column separator,
 by default a comma. The parameters `header`, `datatype` and `expid` have the same
 meaning as in `get_table_data()`.
 
 ```python
+def get_file_hdf5_data(filename: str, filename_is_long_name: bool=False, expid: int=None):
+```
+Get the data from a hdf5 file attached to eLabFTW experiments.
+`filename` is the name of the file stored in the experiment. 
+if `filename_is_long_name` is set to True, `filename` is 
+regarded as the long_name of the file stored in eLabFTW.
+
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`. The function returns a hdf5 file object as 
+created by `h5py.File()`.
+
+### Update experiment data
+
+```python
+def create_extrafield(fieldname: str, value, fieldtype:str='text',
+                      unit: str=None, units=None, description: str=None,
+                      groupname: str=None,
+                      readonly: bool=False, required: bool=False,
+                      expid: int=None):
+```
+Create a new extra field with the name `fieldname` of type `fieldtype`
+(possible values: text, number, date, time, datetime; the default
+type is `text`) containing the value of `value`. 
+You can define a list of possible units in the
+parameter `units` and specify the default unit in `unit`.
+The extra field may be assigned to an extra field group with name
+`groupname`; if the group doesn't exist, it will be created.
+`readonly` and `required` control the respective property of the
+extra field. 
+Depending on `fieldtype`, `value` will automatically be converted
+to string using appropriate functions (e.g. datetime.isoformat).
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+```python
+def update_extrafield(fieldname: str, value, expid: int=None):
+```
+Update the value of the extra field with the name `fieldname`.
+Depending on the type of the extra field, 
+`value` will automatically be converted
+to string using appropriate functions (e.g. datetime.isoformat).
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+```python
+def delete_extrafield(fieldname: str, expid: int=None):
+```
+Delete the extra field with name `fieldname`.
+The parameter `expid` is optional and has the same meaning as in
+`get_table_data()`.
+
+### Upload files
+
+```python
 def upload_file(file: str, comment: str,
                 replacefile: bool=True, expid: int=None):
 ```
 Upload a file from local drives to an eLabFTW experiment.
 `file` is the filepath of the file to be uploaded, 
 `comment` is a description of the file.
```

### Comparing `pyelabdata-0.1.7/pyproject.toml` & `pyelabdata-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+# Build package as follows:
+# - delete all files in the directory dist
+# - run the following commands
+#     python -m build
+#     twine upload dist/*
+
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyelabdata"
-version = "0.1.7"
+version = "0.2.0"
 authors = [
     { name="Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg", email="physik-ep@fau.de" },
     { name="Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg", email="michael.krieger@fau.de"}
 ]
 description = "pyelabdata provides functions for simple one-line access to data in eLabFTW"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -17,16 +23,19 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "numpy",
     "elabapi_python",
     "pandas",
+    "json",
+    "h5py",
     "ipyparams",
     "matplotlib",
     "pathlib",
+    "datetime",
     "IPython"
 ]
 
 [project.urls]
 "Repository" = "https://github.com/FAU-PHYSIK-EP/pyelabdata"
 "Issues" = "https://github.com/FAU-PHYSIK-EP/pyelabdata/issues"
```

