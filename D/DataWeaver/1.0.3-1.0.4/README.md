# Comparing `tmp/dataweaver-1.0.3.tar.gz` & `tmp/dataweaver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataweaver-1.0.3.tar", last modified: Thu Apr 18 09:00:38 2024, max compression
+gzip compressed data, was "dataweaver-1.0.4.tar", last modified: Thu May 16 09:04:40 2024, max compression
```

## Comparing `dataweaver-1.0.3.tar` & `dataweaver-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:00:38.865356 dataweaver-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 09:00:34.000000 dataweaver-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17490 2024-04-18 09:00:38.865356 dataweaver-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16777 2024-04-18 09:00:34.000000 dataweaver-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-18 09:00:34.000000 dataweaver-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:00:38.865356 dataweaver-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:00:38.865356 dataweaver-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:00:38.865356 dataweaver-1.0.3/src/DataWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17490 2024-04-18 09:00:38.000000 dataweaver-1.0.3/src/DataWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 09:00:38.000000 dataweaver-1.0.3/src/DataWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:00:38.000000 dataweaver-1.0.3/src/DataWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 09:00:38.000000 dataweaver-1.0.3/src/DataWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 09:00:38.000000 dataweaver-1.0.3/src/DataWeaver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:00:38.865356 dataweaver-1.0.3/src/data_weaver/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 09:00:34.000000 dataweaver-1.0.3/src/data_weaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-18 09:00:34.000000 dataweaver-1.0.3/src/data_weaver/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-18 09:00:34.000000 dataweaver-1.0.3/src/data_weaver/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-18 09:00:34.000000 dataweaver-1.0.3/src/data_weaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:40.532630 dataweaver-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 09:04:36.000000 dataweaver-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23720 2024-05-16 09:04:40.532630 dataweaver-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23007 2024-05-16 09:04:36.000000 dataweaver-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 09:04:36.000000 dataweaver-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:04:40.532630 dataweaver-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:40.528630 dataweaver-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:40.532630 dataweaver-1.0.4/src/DataWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23720 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:40.532630 dataweaver-1.0.4/src/data_weaver/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 09:04:36.000000 dataweaver-1.0.4/src/data_weaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-16 09:04:36.000000 dataweaver-1.0.4/src/data_weaver/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-16 09:04:36.000000 dataweaver-1.0.4/src/data_weaver/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 09:04:36.000000 dataweaver-1.0.4/src/data_weaver/utils.py
```

### Comparing `dataweaver-1.0.3/LICENSE` & `dataweaver-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dataweaver-1.0.3/PKG-INFO` & `dataweaver-1.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: DataWeaver
-Version: 1.0.3
-Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
-Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
-License: MIT License
-Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiofiles>=0.7.0
-Requires-Dist: PyYAML>=5.4
-
 # DataWeaver
 
 A brief description of what this project does and who it's for. This project is an asynchronous data processing library designed to transform and process data entries efficiently, with a special focus on handling complex data structures.
 
 ## Features
 
 - Asynchronous data processing for improved performance.
@@ -151,18 +136,25 @@
 Define mappings and additional fields required for processing your data in a Dict.
 
 There are three main sections in the configuration file:
 
 - `mapping`: Specifies how keys in the input data should be mapped to keys in the output data. The logical here is the following: `target_key: source_key`.
 - `additionalFields`: Specifies additional fields that should be added to the output data. The logical here is the following: `target_key: value`.
 - `transforms`: Specifies how different fields in the data are transformed using various functions. Each key represents a field or type of fields, and the associated value describes the transformation to be applied to that field.
+- `default`: Specifies default values for fields that may not exist in the input data. This is useful for ensuring that the output data contains all expected fields, even if they are not present in the input data.
+
+In the `default` section there is some sub sections.
+
+- `static`: Specifies default values that are static and do not depend on the input data.
+- `dynamic`: Specifies default values that are dynamic and depend on the input data.
+- `transforms`: Specifies transformations that should be applied to default values.
 
  Here's an example that demonstrates handling complex keys:
 
- ### Configuration File: Mapping
+### Configuration File: Mapping
 
 This section of the configuration file specifies how keys in the input data should be mapped to keys in the output data. Each key represents a target key in the output data, and the associated value represents the source key in the input data.
 
 The target key can be a simple key or a complex key with nested objects and arrays. The source key can also be a simple key or a complex key with nested objects and arrays. A dot (`.`) is used to represent nested objects, and a digit is used to represent array indices.
 
 ```python
     config = {
@@ -305,20 +297,36 @@
 }
 ```
 
 ### Configuration File: Transforms
 
 This section of the configuration file specifies how different fields in the data are transformed using various functions. Each key represents a field or type of fields, and the associated value describes the transformation to be applied to that field. These transformations can include formatting, concatenation, type conversion, and more.
 
+| Function Name | Description |
+| --- | --- |
+| `capitalize` | Converts the first character of the string to uppercase and the rest to lowercase. |
+| `lower` | Converts all characters in the string to lowercase. |
+| `upper` | Converts all characters in the string to uppercase. |
+| `title` | Converts the first character of each word to uppercase and the remaining characters of each word to lowercase. |
+| `concat(delimiter=' ')` | Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space. /!\ All elements must be strings |
+| `join(delimiter=' ')` | Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space. |
+| `prefix(string='prefix-')` | Prepends the specified string to the beginning of the target string. Default prefix is "prefix-". |
+| `suffix(string='-suffix')` | Appends the specified string to the end of the target string. Default suffix is "-suffix". |
+| `split(delimiter=' ')` | Splits the string into a list of substrings around the specified delimiter. Default is a space. |
+| `replace(old, new)` | Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new. |
+| `regex(pattern, replace)` | Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace. |
+| `parse_type(typename)` | Converts the string to the specified type (typename). Valid types include str, bool, int, and float. |
+
 ## Function Descriptions
 
-### 1. Text Case Functions:
+### 1. Text Case Functions
 
 - `capitalize`: Converts the first character of the string to uppercase and the rest to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "capitalize",
@@ -340,284 +348,335 @@
   {
     "fullName": "John doe",
   }
   ```
 
 - `lower`: Converts all characters in the string to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "lower",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "JOHN DOE",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
 - `upper`: Converts all characters in the string to uppercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "upper",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "JOHN DOE",
   }
   ```
+
 - `title`: Converts the first character of each word to uppercase and the remaining characters of each word to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "title",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "John Doe",
   }
   ```
 
-### 2. String Manipulation Functions:
+### 2. String Manipulation Functions
 
 - `concat(delimiter=' ')`: Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space.
+
     ```json
   {
     "mapping": {
       "person.fullName": ["firstName", "lastName"],
     },
     "transforms": {
       "person.fullName": "concat(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "firstName": "John",
     "lastName": "Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": "John Doe",
     }
   }
   ```
+
 - `prefix(string='prefix-')`: Prepends the specified string to the beginning of the target string. Default prefix is "prefix-".
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "prefix(string='hello-')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
 
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello-world",
     }
   }
   ```
 
 - `suffix(string='-suffix')`: Appends the specified string to the end of the target string. Default suffix is "-suffix".
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "suffix(string='-world')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "hello",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello-world",
     }
   }
   ```
 
 - `split(delimiter=' ')`: Splits the string into a list of substrings around the specified delimiter. Default is a space.
   Example:
+
   ```json
   {
     "mapping": {
       "person.fullName": "fullName",
     },
     "transforms": {
       "person.fullName": "split(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "John Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": ["John", "Doe"],
     }
   }
   ```
 
-
 - `join(delimiter=' ')`: Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space.
+
     ```json
   {
     "mapping": {
       "person.fullName": ["firstName", "lastName"],
     },
     "transforms": {
       "person.fullName": "join(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "firstName": "John",
     "lastName": "Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": "John Doe",
     }
   }
   ```
 
-### 3. Replacement and Pattern Matching Functions:
+### 3. Replacement and Pattern Matching Functions
 
 - `replace(old, new)`: Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new.
   Example:
-  ```json 
+
+  ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "replace(old='world', new='hello')",
     }
   }
   ```
 
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
 
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello",
     }
   }
   ```
+
 - `regex(pattern, replace)`: Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "regex(pattern='[a-z]+', replace='X')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "X",
     }
   }
   ```
 
-### 4. Type Parsing Functions:
+### 4. Type Parsing Functions
 
 - `parse_type(typename)`: Converts the string to the specified type (typename). Valid types include str, bool, int, and float.
   Example:
+
   ```json
   {
     "mapping": {
       "age_mapped": "age",
       "is_student_mapped": "is_student", 
       "is_teacher_mapped": "is_teacher", 
       "salary_mapped": "salary",
@@ -628,25 +687,29 @@
       "is_student_mapped": "parse_type(typename='bool')",
       "is_teacher_mapped": "parse_type(typename='bool')",
       "salary_mapped": "parse_type(typename='float')",
       "student_id_mapped": "parse_type(typename='int')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "age": "30",
     "is_student": "True",
     "is_teacher": "False",
     "salary": "3000.50",
     "student_id": 12345,
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "age_mapped": 30,
     "is_student_mapped": true,
     "is_teacher_mapped": false,
     "salary_mapped": 3000.50,
     "student_id_mapped": "12345",
@@ -654,10 +717,230 @@
   ```
 
 PS : bool type is case insensitive, so you can pass :
 
 - "true", "True", "TRUE", "yes",  "Yes", "YES", "y", "Y" it will be converted to True
 - "no", "No", "NO", "n", "N", "false", "False", "FALSE"  it will be converted to False
 
+### Chaining Transformations
+
+You can chain multiple transformations together by describe them in a list. This allows you to apply multiple transformations to a single field in a specific order.
+
+```json
+{
+  "mapping": {
+    "person.cn": ["firstName", "lastName"],
+  },
+  "transforms": {
+    "person.name": ["lower", "concat(delimiter='.')"],
+  }
+}
+```
+
+The object below:
+
+```json
+{
+  "firstName": "John",
+  "lastName": "Doe",
+}
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "john.doe",
+  }
+}
+```
+
+### Default Values
+
+You can also specify default values for fields that may not exist in the input data. This is useful for ensuring that the output data contains all expected fields, even if they are not present in the input data.
+
+```json
+{
+  "mapping": {
+    "person.name": "fullName",
+    "person.age": "age",
+  },
+  "default": {
+    "static": {
+      "person.age": 0,
+    },
+    "dynamic": {
+      "person.name": ["firstName", "lastName"],
+    }
+  }
+}
+
+```
+
+The object below:
+
+```json
+{
+  "fullName": "John Doe",
+  "firstName": "John",
+  "lastName": "Doe",
+  "age": 30,
+}
+
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "John Doe",
+    "age": 30,
+  }
+}
+
+```
+
+But if there is no age in the input data, and no fullname the output will be:
+
+```json
+{
+  "person": {
+    "name": ["John", "Doe"],
+    "age": 0,
+  }
+}
+
+```
+
+You can also add transformations to default values:
+
+```json
+{
+  "mapping": {
+    "person.name": "fullName",
+    "person.age": "age",
+  },
+  "default": {
+    "static": {
+      "person.age": 0,
+    },
+    "dynamic": {
+      "person.name": ["firstName", "lastName"],
+    },
+    "transforms": {
+      "person.name": ["lower", "concat(delimiter='.')"],
+    }
+  }
+}
+
+```
+
+The object below:
+
+```json
+{
+  "fullName": "John Doe",
+  "firstName": "John",
+  "lastName": "Doe",
+}
+
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "john.doe",
+    "age": 0,
+  }
+}
+
+```
+
+### Advanced Configuration
+
+Here's an example of a more complex configuration file that demonstrates the use of multiple mapping, additional fields, and transformation functions:
+
+```json
+config = {
+  "mapping": {
+    "uid": "login",
+    "uid2": "login2",
+    "fullname": ["nom", "prenom"],
+  },
+  "transforms": {
+    "fullname": ["join(delimiter=' ')"],
+    "uid": ["replace(old='.', new='')"],
+  },
+  "default": {
+    "dynamic": {
+      "uid": ["nom", "prenom"]
+    },
+    "static": {
+      "uid2": "test"
+    },
+    "transforms": {
+      "uid": ["join(delimiter='.')","lower", "regex(pattern='(?<=\\b\\w)\\w+(?=\\.)', replace='')"],
+    },
+  }
+}
+```
+
+This configuration file specifies the following:
+
+- The `uid` field in the output data should be mapped to the `login` field in the input data.
+- The `uid2` field in the output data should be mapped to the `login2` field in the input data.
+- The `fullname` field in the output data should be mapped to the `nom` and `prenom` fields in the input data. The transformations applied to this field are:
+  - Convert the field to lowercase.
+  - Join the elements of the list with a period (`.`) delimiter.
+  - Apply a regular expression to remove all characters after the first period (`.`) in the string.
+- The `uid` field should be created by joining the `nom` and `prenom` fields in the input data, converting the result to lowercase, and removing all characters after the first period (`.`) in the string.
+- The `uid2` field should have a default value of `test`.
+- The `uid` field should have a default value of `nom` and `prenom` in the input data, converted to lowercase, and with all characters after the first period (`.`) removed.
+
+The following input data:
+
+```json
+{
+  "login": "John.Doe",
+  "login2": "Jane.Doe",
+  "nom": "John",
+  "prenom": "Doe"
+}
+```
+
+Will be transformed to:
+
+```json
+{
+    "uid": "JohnDoe",
+    "uid2": "Jane.Doe",
+    "fullname": "John Doe"
+}
+```
+
+And this one :
+
+```json
+{
+  "login2": "Jane.Doe",
+  "nom": "John",
+  "prenom": "Doe"
+}
+```
+
+Will be transformed to:
+
+```json
+{
+    "uid": "j.doe",
+    "uid2": "Jane.Doe",
+    "fullname": "John Doe"
+}
+```
+
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `dataweaver-1.0.3/README.md` & `dataweaver-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: DataWeaver
+Version: 1.0.4
+Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
+Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
+License: MIT License
+Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiofiles>=0.7.0
+Requires-Dist: PyYAML>=5.4
+
 # DataWeaver
 
 A brief description of what this project does and who it's for. This project is an asynchronous data processing library designed to transform and process data entries efficiently, with a special focus on handling complex data structures.
 
 ## Features
 
 - Asynchronous data processing for improved performance.
@@ -136,18 +151,25 @@
 Define mappings and additional fields required for processing your data in a Dict.
 
 There are three main sections in the configuration file:
 
 - `mapping`: Specifies how keys in the input data should be mapped to keys in the output data. The logical here is the following: `target_key: source_key`.
 - `additionalFields`: Specifies additional fields that should be added to the output data. The logical here is the following: `target_key: value`.
 - `transforms`: Specifies how different fields in the data are transformed using various functions. Each key represents a field or type of fields, and the associated value describes the transformation to be applied to that field.
+- `default`: Specifies default values for fields that may not exist in the input data. This is useful for ensuring that the output data contains all expected fields, even if they are not present in the input data.
+
+In the `default` section there is some sub sections.
+
+- `static`: Specifies default values that are static and do not depend on the input data.
+- `dynamic`: Specifies default values that are dynamic and depend on the input data.
+- `transforms`: Specifies transformations that should be applied to default values.
 
  Here's an example that demonstrates handling complex keys:
 
- ### Configuration File: Mapping
+### Configuration File: Mapping
 
 This section of the configuration file specifies how keys in the input data should be mapped to keys in the output data. Each key represents a target key in the output data, and the associated value represents the source key in the input data.
 
 The target key can be a simple key or a complex key with nested objects and arrays. The source key can also be a simple key or a complex key with nested objects and arrays. A dot (`.`) is used to represent nested objects, and a digit is used to represent array indices.
 
 ```python
     config = {
@@ -290,20 +312,36 @@
 }
 ```
 
 ### Configuration File: Transforms
 
 This section of the configuration file specifies how different fields in the data are transformed using various functions. Each key represents a field or type of fields, and the associated value describes the transformation to be applied to that field. These transformations can include formatting, concatenation, type conversion, and more.
 
+| Function Name | Description |
+| --- | --- |
+| `capitalize` | Converts the first character of the string to uppercase and the rest to lowercase. |
+| `lower` | Converts all characters in the string to lowercase. |
+| `upper` | Converts all characters in the string to uppercase. |
+| `title` | Converts the first character of each word to uppercase and the remaining characters of each word to lowercase. |
+| `concat(delimiter=' ')` | Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space. /!\ All elements must be strings |
+| `join(delimiter=' ')` | Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space. |
+| `prefix(string='prefix-')` | Prepends the specified string to the beginning of the target string. Default prefix is "prefix-". |
+| `suffix(string='-suffix')` | Appends the specified string to the end of the target string. Default suffix is "-suffix". |
+| `split(delimiter=' ')` | Splits the string into a list of substrings around the specified delimiter. Default is a space. |
+| `replace(old, new)` | Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new. |
+| `regex(pattern, replace)` | Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace. |
+| `parse_type(typename)` | Converts the string to the specified type (typename). Valid types include str, bool, int, and float. |
+
 ## Function Descriptions
 
-### 1. Text Case Functions:
+### 1. Text Case Functions
 
 - `capitalize`: Converts the first character of the string to uppercase and the rest to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "capitalize",
@@ -325,284 +363,335 @@
   {
     "fullName": "John doe",
   }
   ```
 
 - `lower`: Converts all characters in the string to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "lower",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "JOHN DOE",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
 - `upper`: Converts all characters in the string to uppercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "upper",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "JOHN DOE",
   }
   ```
+
 - `title`: Converts the first character of each word to uppercase and the remaining characters of each word to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "title",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "John Doe",
   }
   ```
 
-### 2. String Manipulation Functions:
+### 2. String Manipulation Functions
 
 - `concat(delimiter=' ')`: Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space.
+
     ```json
   {
     "mapping": {
       "person.fullName": ["firstName", "lastName"],
     },
     "transforms": {
       "person.fullName": "concat(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "firstName": "John",
     "lastName": "Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": "John Doe",
     }
   }
   ```
+
 - `prefix(string='prefix-')`: Prepends the specified string to the beginning of the target string. Default prefix is "prefix-".
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "prefix(string='hello-')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
 
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello-world",
     }
   }
   ```
 
 - `suffix(string='-suffix')`: Appends the specified string to the end of the target string. Default suffix is "-suffix".
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "suffix(string='-world')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "hello",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello-world",
     }
   }
   ```
 
 - `split(delimiter=' ')`: Splits the string into a list of substrings around the specified delimiter. Default is a space.
   Example:
+
   ```json
   {
     "mapping": {
       "person.fullName": "fullName",
     },
     "transforms": {
       "person.fullName": "split(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "John Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": ["John", "Doe"],
     }
   }
   ```
 
-
 - `join(delimiter=' ')`: Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space.
+
     ```json
   {
     "mapping": {
       "person.fullName": ["firstName", "lastName"],
     },
     "transforms": {
       "person.fullName": "join(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "firstName": "John",
     "lastName": "Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": "John Doe",
     }
   }
   ```
 
-### 3. Replacement and Pattern Matching Functions:
+### 3. Replacement and Pattern Matching Functions
 
 - `replace(old, new)`: Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new.
   Example:
-  ```json 
+
+  ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "replace(old='world', new='hello')",
     }
   }
   ```
 
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
 
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello",
     }
   }
   ```
+
 - `regex(pattern, replace)`: Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "regex(pattern='[a-z]+', replace='X')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "X",
     }
   }
   ```
 
-### 4. Type Parsing Functions:
+### 4. Type Parsing Functions
 
 - `parse_type(typename)`: Converts the string to the specified type (typename). Valid types include str, bool, int, and float.
   Example:
+
   ```json
   {
     "mapping": {
       "age_mapped": "age",
       "is_student_mapped": "is_student", 
       "is_teacher_mapped": "is_teacher", 
       "salary_mapped": "salary",
@@ -613,25 +702,29 @@
       "is_student_mapped": "parse_type(typename='bool')",
       "is_teacher_mapped": "parse_type(typename='bool')",
       "salary_mapped": "parse_type(typename='float')",
       "student_id_mapped": "parse_type(typename='int')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "age": "30",
     "is_student": "True",
     "is_teacher": "False",
     "salary": "3000.50",
     "student_id": 12345,
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "age_mapped": 30,
     "is_student_mapped": true,
     "is_teacher_mapped": false,
     "salary_mapped": 3000.50,
     "student_id_mapped": "12345",
@@ -639,10 +732,230 @@
   ```
 
 PS : bool type is case insensitive, so you can pass :
 
 - "true", "True", "TRUE", "yes",  "Yes", "YES", "y", "Y" it will be converted to True
 - "no", "No", "NO", "n", "N", "false", "False", "FALSE"  it will be converted to False
 
+### Chaining Transformations
+
+You can chain multiple transformations together by describe them in a list. This allows you to apply multiple transformations to a single field in a specific order.
+
+```json
+{
+  "mapping": {
+    "person.cn": ["firstName", "lastName"],
+  },
+  "transforms": {
+    "person.name": ["lower", "concat(delimiter='.')"],
+  }
+}
+```
+
+The object below:
+
+```json
+{
+  "firstName": "John",
+  "lastName": "Doe",
+}
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "john.doe",
+  }
+}
+```
+
+### Default Values
+
+You can also specify default values for fields that may not exist in the input data. This is useful for ensuring that the output data contains all expected fields, even if they are not present in the input data.
+
+```json
+{
+  "mapping": {
+    "person.name": "fullName",
+    "person.age": "age",
+  },
+  "default": {
+    "static": {
+      "person.age": 0,
+    },
+    "dynamic": {
+      "person.name": ["firstName", "lastName"],
+    }
+  }
+}
+
+```
+
+The object below:
+
+```json
+{
+  "fullName": "John Doe",
+  "firstName": "John",
+  "lastName": "Doe",
+  "age": 30,
+}
+
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "John Doe",
+    "age": 30,
+  }
+}
+
+```
+
+But if there is no age in the input data, and no fullname the output will be:
+
+```json
+{
+  "person": {
+    "name": ["John", "Doe"],
+    "age": 0,
+  }
+}
+
+```
+
+You can also add transformations to default values:
+
+```json
+{
+  "mapping": {
+    "person.name": "fullName",
+    "person.age": "age",
+  },
+  "default": {
+    "static": {
+      "person.age": 0,
+    },
+    "dynamic": {
+      "person.name": ["firstName", "lastName"],
+    },
+    "transforms": {
+      "person.name": ["lower", "concat(delimiter='.')"],
+    }
+  }
+}
+
+```
+
+The object below:
+
+```json
+{
+  "fullName": "John Doe",
+  "firstName": "John",
+  "lastName": "Doe",
+}
+
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "john.doe",
+    "age": 0,
+  }
+}
+
+```
+
+### Advanced Configuration
+
+Here's an example of a more complex configuration file that demonstrates the use of multiple mapping, additional fields, and transformation functions:
+
+```json
+config = {
+  "mapping": {
+    "uid": "login",
+    "uid2": "login2",
+    "fullname": ["nom", "prenom"],
+  },
+  "transforms": {
+    "fullname": ["join(delimiter=' ')"],
+    "uid": ["replace(old='.', new='')"],
+  },
+  "default": {
+    "dynamic": {
+      "uid": ["nom", "prenom"]
+    },
+    "static": {
+      "uid2": "test"
+    },
+    "transforms": {
+      "uid": ["join(delimiter='.')","lower", "regex(pattern='(?<=\\b\\w)\\w+(?=\\.)', replace='')"],
+    },
+  }
+}
+```
+
+This configuration file specifies the following:
+
+- The `uid` field in the output data should be mapped to the `login` field in the input data.
+- The `uid2` field in the output data should be mapped to the `login2` field in the input data.
+- The `fullname` field in the output data should be mapped to the `nom` and `prenom` fields in the input data. The transformations applied to this field are:
+  - Convert the field to lowercase.
+  - Join the elements of the list with a period (`.`) delimiter.
+  - Apply a regular expression to remove all characters after the first period (`.`) in the string.
+- The `uid` field should be created by joining the `nom` and `prenom` fields in the input data, converting the result to lowercase, and removing all characters after the first period (`.`) in the string.
+- The `uid2` field should have a default value of `test`.
+- The `uid` field should have a default value of `nom` and `prenom` in the input data, converted to lowercase, and with all characters after the first period (`.`) removed.
+
+The following input data:
+
+```json
+{
+  "login": "John.Doe",
+  "login2": "Jane.Doe",
+  "nom": "John",
+  "prenom": "Doe"
+}
+```
+
+Will be transformed to:
+
+```json
+{
+    "uid": "JohnDoe",
+    "uid2": "Jane.Doe",
+    "fullname": "John Doe"
+}
+```
+
+And this one :
+
+```json
+{
+  "login2": "Jane.Doe",
+  "nom": "John",
+  "prenom": "Doe"
+}
+```
+
+Will be transformed to:
+
+```json
+{
+    "uid": "j.doe",
+    "uid2": "Jane.Doe",
+    "fullname": "John Doe"
+}
+```
+
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `dataweaver-1.0.3/pyproject.toml` & `dataweaver-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DataWeaver"
-version = "1.0.3"
+version = "1.0.4"
 authors = [{name = "RICHARD Quentin", email = "richard.quentin88@gmail.com"}]
 description = "DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing."
 readme = "README.md"
 license = {text = "MIT License"}  # Update the license as appropriate
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dataweaver-1.0.3/src/DataWeaver.egg-info/PKG-INFO` & `dataweaver-1.0.4/src/DataWeaver.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 1.0.3
+Version: 1.0.4
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -151,18 +151,25 @@
 Define mappings and additional fields required for processing your data in a Dict.
 
 There are three main sections in the configuration file:
 
 - `mapping`: Specifies how keys in the input data should be mapped to keys in the output data. The logical here is the following: `target_key: source_key`.
 - `additionalFields`: Specifies additional fields that should be added to the output data. The logical here is the following: `target_key: value`.
 - `transforms`: Specifies how different fields in the data are transformed using various functions. Each key represents a field or type of fields, and the associated value describes the transformation to be applied to that field.
+- `default`: Specifies default values for fields that may not exist in the input data. This is useful for ensuring that the output data contains all expected fields, even if they are not present in the input data.
+
+In the `default` section there is some sub sections.
+
+- `static`: Specifies default values that are static and do not depend on the input data.
+- `dynamic`: Specifies default values that are dynamic and depend on the input data.
+- `transforms`: Specifies transformations that should be applied to default values.
 
  Here's an example that demonstrates handling complex keys:
 
- ### Configuration File: Mapping
+### Configuration File: Mapping
 
 This section of the configuration file specifies how keys in the input data should be mapped to keys in the output data. Each key represents a target key in the output data, and the associated value represents the source key in the input data.
 
 The target key can be a simple key or a complex key with nested objects and arrays. The source key can also be a simple key or a complex key with nested objects and arrays. A dot (`.`) is used to represent nested objects, and a digit is used to represent array indices.
 
 ```python
     config = {
@@ -305,20 +312,36 @@
 }
 ```
 
 ### Configuration File: Transforms
 
 This section of the configuration file specifies how different fields in the data are transformed using various functions. Each key represents a field or type of fields, and the associated value describes the transformation to be applied to that field. These transformations can include formatting, concatenation, type conversion, and more.
 
+| Function Name | Description |
+| --- | --- |
+| `capitalize` | Converts the first character of the string to uppercase and the rest to lowercase. |
+| `lower` | Converts all characters in the string to lowercase. |
+| `upper` | Converts all characters in the string to uppercase. |
+| `title` | Converts the first character of each word to uppercase and the remaining characters of each word to lowercase. |
+| `concat(delimiter=' ')` | Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space. /!\ All elements must be strings |
+| `join(delimiter=' ')` | Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space. |
+| `prefix(string='prefix-')` | Prepends the specified string to the beginning of the target string. Default prefix is "prefix-". |
+| `suffix(string='-suffix')` | Appends the specified string to the end of the target string. Default suffix is "-suffix". |
+| `split(delimiter=' ')` | Splits the string into a list of substrings around the specified delimiter. Default is a space. |
+| `replace(old, new)` | Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new. |
+| `regex(pattern, replace)` | Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace. |
+| `parse_type(typename)` | Converts the string to the specified type (typename). Valid types include str, bool, int, and float. |
+
 ## Function Descriptions
 
-### 1. Text Case Functions:
+### 1. Text Case Functions
 
 - `capitalize`: Converts the first character of the string to uppercase and the rest to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "capitalize",
@@ -340,284 +363,335 @@
   {
     "fullName": "John doe",
   }
   ```
 
 - `lower`: Converts all characters in the string to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "lower",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "JOHN DOE",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
 - `upper`: Converts all characters in the string to uppercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "upper",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "JOHN DOE",
   }
   ```
+
 - `title`: Converts the first character of each word to uppercase and the remaining characters of each word to lowercase.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "title",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "john doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "fullName": "John Doe",
   }
   ```
 
-### 2. String Manipulation Functions:
+### 2. String Manipulation Functions
 
 - `concat(delimiter=' ')`: Concatenates list elements into a single string with elements separated by the specified delimiter. Default is a space.
+
     ```json
   {
     "mapping": {
       "person.fullName": ["firstName", "lastName"],
     },
     "transforms": {
       "person.fullName": "concat(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "firstName": "John",
     "lastName": "Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": "John Doe",
     }
   }
   ```
+
 - `prefix(string='prefix-')`: Prepends the specified string to the beginning of the target string. Default prefix is "prefix-".
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "prefix(string='hello-')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
 
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello-world",
     }
   }
   ```
 
 - `suffix(string='-suffix')`: Appends the specified string to the end of the target string. Default suffix is "-suffix".
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "suffix(string='-world')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "hello",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello-world",
     }
   }
   ```
 
 - `split(delimiter=' ')`: Splits the string into a list of substrings around the specified delimiter. Default is a space.
   Example:
+
   ```json
   {
     "mapping": {
       "person.fullName": "fullName",
     },
     "transforms": {
       "person.fullName": "split(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "John Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": ["John", "Doe"],
     }
   }
   ```
 
-
 - `join(delimiter=' ')`: Joins elements of a list into a single string with elements separated by the specified delimiter. Default is a space.
+
     ```json
   {
     "mapping": {
       "person.fullName": ["firstName", "lastName"],
     },
     "transforms": {
       "person.fullName": "join(delimiter=' ')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "firstName": "John",
     "lastName": "Doe",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "fullName": "John Doe",
     }
   }
   ```
 
-### 3. Replacement and Pattern Matching Functions:
+### 3. Replacement and Pattern Matching Functions
 
 - `replace(old, new)`: Replaces occurrences of a substring (old) within the string with another substring (new). Options must specify old and new.
   Example:
-  ```json 
+
+  ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "replace(old='world', new='hello')",
     }
   }
   ```
 
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
 
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "hello",
     }
   }
   ```
+
 - `regex(pattern, replace)`: Applies a regular expression pattern to the string and replaces matches with the specified replacement string. Options must specify both pattern and replace.
   Example:
+
   ```json
   {
     "mapping": {
       "person.name": "fullName",
     },
     "transforms": {
       "person.name": "regex(pattern='[a-z]+', replace='X')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "fullName": "world",
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "person": {
       "name": "X",
     }
   }
   ```
 
-### 4. Type Parsing Functions:
+### 4. Type Parsing Functions
 
 - `parse_type(typename)`: Converts the string to the specified type (typename). Valid types include str, bool, int, and float.
   Example:
+
   ```json
   {
     "mapping": {
       "age_mapped": "age",
       "is_student_mapped": "is_student", 
       "is_teacher_mapped": "is_teacher", 
       "salary_mapped": "salary",
@@ -628,25 +702,29 @@
       "is_student_mapped": "parse_type(typename='bool')",
       "is_teacher_mapped": "parse_type(typename='bool')",
       "salary_mapped": "parse_type(typename='float')",
       "student_id_mapped": "parse_type(typename='int')",
     }
   }
   ```
+
   The object below:
+
   ```json
   {
     "age": "30",
     "is_student": "True",
     "is_teacher": "False",
     "salary": "3000.50",
     "student_id": 12345,
   }
   ```
+
   Will be transformed to:
+
   ```json
   {
     "age_mapped": 30,
     "is_student_mapped": true,
     "is_teacher_mapped": false,
     "salary_mapped": 3000.50,
     "student_id_mapped": "12345",
@@ -654,10 +732,230 @@
   ```
 
 PS : bool type is case insensitive, so you can pass :
 
 - "true", "True", "TRUE", "yes",  "Yes", "YES", "y", "Y" it will be converted to True
 - "no", "No", "NO", "n", "N", "false", "False", "FALSE"  it will be converted to False
 
+### Chaining Transformations
+
+You can chain multiple transformations together by describe them in a list. This allows you to apply multiple transformations to a single field in a specific order.
+
+```json
+{
+  "mapping": {
+    "person.cn": ["firstName", "lastName"],
+  },
+  "transforms": {
+    "person.name": ["lower", "concat(delimiter='.')"],
+  }
+}
+```
+
+The object below:
+
+```json
+{
+  "firstName": "John",
+  "lastName": "Doe",
+}
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "john.doe",
+  }
+}
+```
+
+### Default Values
+
+You can also specify default values for fields that may not exist in the input data. This is useful for ensuring that the output data contains all expected fields, even if they are not present in the input data.
+
+```json
+{
+  "mapping": {
+    "person.name": "fullName",
+    "person.age": "age",
+  },
+  "default": {
+    "static": {
+      "person.age": 0,
+    },
+    "dynamic": {
+      "person.name": ["firstName", "lastName"],
+    }
+  }
+}
+
+```
+
+The object below:
+
+```json
+{
+  "fullName": "John Doe",
+  "firstName": "John",
+  "lastName": "Doe",
+  "age": 30,
+}
+
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "John Doe",
+    "age": 30,
+  }
+}
+
+```
+
+But if there is no age in the input data, and no fullname the output will be:
+
+```json
+{
+  "person": {
+    "name": ["John", "Doe"],
+    "age": 0,
+  }
+}
+
+```
+
+You can also add transformations to default values:
+
+```json
+{
+  "mapping": {
+    "person.name": "fullName",
+    "person.age": "age",
+  },
+  "default": {
+    "static": {
+      "person.age": 0,
+    },
+    "dynamic": {
+      "person.name": ["firstName", "lastName"],
+    },
+    "transforms": {
+      "person.name": ["lower", "concat(delimiter='.')"],
+    }
+  }
+}
+
+```
+
+The object below:
+
+```json
+{
+  "fullName": "John Doe",
+  "firstName": "John",
+  "lastName": "Doe",
+}
+
+```
+
+Will be transformed to:
+
+```json
+{
+  "person": {
+    "name": "john.doe",
+    "age": 0,
+  }
+}
+
+```
+
+### Advanced Configuration
+
+Here's an example of a more complex configuration file that demonstrates the use of multiple mapping, additional fields, and transformation functions:
+
+```json
+config = {
+  "mapping": {
+    "uid": "login",
+    "uid2": "login2",
+    "fullname": ["nom", "prenom"],
+  },
+  "transforms": {
+    "fullname": ["join(delimiter=' ')"],
+    "uid": ["replace(old='.', new='')"],
+  },
+  "default": {
+    "dynamic": {
+      "uid": ["nom", "prenom"]
+    },
+    "static": {
+      "uid2": "test"
+    },
+    "transforms": {
+      "uid": ["join(delimiter='.')","lower", "regex(pattern='(?<=\\b\\w)\\w+(?=\\.)', replace='')"],
+    },
+  }
+}
+```
+
+This configuration file specifies the following:
+
+- The `uid` field in the output data should be mapped to the `login` field in the input data.
+- The `uid2` field in the output data should be mapped to the `login2` field in the input data.
+- The `fullname` field in the output data should be mapped to the `nom` and `prenom` fields in the input data. The transformations applied to this field are:
+  - Convert the field to lowercase.
+  - Join the elements of the list with a period (`.`) delimiter.
+  - Apply a regular expression to remove all characters after the first period (`.`) in the string.
+- The `uid` field should be created by joining the `nom` and `prenom` fields in the input data, converting the result to lowercase, and removing all characters after the first period (`.`) in the string.
+- The `uid2` field should have a default value of `test`.
+- The `uid` field should have a default value of `nom` and `prenom` in the input data, converted to lowercase, and with all characters after the first period (`.`) removed.
+
+The following input data:
+
+```json
+{
+  "login": "John.Doe",
+  "login2": "Jane.Doe",
+  "nom": "John",
+  "prenom": "Doe"
+}
+```
+
+Will be transformed to:
+
+```json
+{
+    "uid": "JohnDoe",
+    "uid2": "Jane.Doe",
+    "fullname": "John Doe"
+}
+```
+
+And this one :
+
+```json
+{
+  "login2": "Jane.Doe",
+  "nom": "John",
+  "prenom": "Doe"
+}
+```
+
+Will be transformed to:
+
+```json
+{
+    "uid": "j.doe",
+    "uid2": "Jane.Doe",
+    "fullname": "John Doe"
+}
+```
+
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `dataweaver-1.0.3/src/data_weaver/transforms.py` & `dataweaver-1.0.4/src/data_weaver/transforms.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         return f"{val}{suffix}"
     return apply_to_value(value, suffix_val)
 
 def split(value: str, delimiter: str = ' ') -> list:
     return value.split(delimiter)
 
 def join(values: list, delimiter: str = ' ') -> str:
-    return delimiter.join(values)
+    return delimiter.join(map(str, values))
 
 def lower(value: str | list | dict) -> str:
     def lower_val(val):
         return val.lower()
     return apply_to_value(value, lower_val)
 
 def title(value: str | list | dict) -> str:
@@ -88,29 +88,64 @@
     "suffix": lambda value, string: suffix(value, string),
     "split": lambda value, delimiter=None: split(value, delimiter),
     "join": lambda value, delimiter='': join(value, delimiter),
     "replace": lambda value, old, new: replace(value, old, new),
     "regex": lambda value, pattern, replace: regex(value, pattern, replace)
 }
 
-def parse_args(args: str) -> list:
+def parse_args(args: str) -> dict:
     kwargs = {}
-    for arg in args:
-        key_values = arg.split(", ")
-        for key_value in key_values:
-            key, value = key_value.split('=')
-            kwargs[key.strip()] = eval(value)  # Using eval to convert the string 'X' to X without quotes
+    
+    # Regex pattern to match key-value pairs considering nested structures and quoted strings
+    pattern = re.compile(r"(\w+)=('(?:\\.|[^'])*'|\"(?:\\.|[^\"])*\"|\([^)]*\)|\[[^\]]*\]|\{[^}]*\}|\S+)")
+    
+    for match in pattern.finditer(args):
+        key = match.group(1).strip()
+        value = match.group(2).strip()
+        
+        # Remove the outer quotes from strings, if they exist
+        if value.startswith(("'", '"')) and value.endswith(("'", '"')):
+            value = value[1:-1]
+        else:
+            # Try to parse the value using ast.literal_eval for safety
+            try:
+                value = ast.literal_eval(value)
+            except (ValueError, SyntaxError):
+                # If parsing fails, keep the value as a string
+                value = str(value)
+
+        kwargs[key] = value
+
     return kwargs
 
-async def parse_transform(transform: str, value: Any) -> Any:
-    func_name, *args = transform.replace(")", "").split("(")
+def parse_function_call(call_str):
+    # Define the regex pattern
+    pattern = re.compile(r"(\w+)(?:\((.*)\))?")
+    match = pattern.match(call_str)
+    
+    if not match:
+        print(f"Invalid function call: {call_str}")
+    
+    func_name = match.group(1)
+    args_str = match.group(2)
+    
+    if args_str is None:
+        # No arguments, return empty list for args
+        return func_name, {}
+    
+    kwargs = parse_args(args_str)
+    return func_name, kwargs
+
+def parse_transform(transform: str, value: Any) -> Any:
+    # func_name, *args = transform.replace(")", "").split("(")
+    func_name, kwargs = parse_function_call(transform)
     func = TRANSFORMATIONS.get(func_name)
     if not func:
         print(f"Invalid transform function: {func_name} for value: {value}")
         return value
     try :
-        kwargs = parse_args(args)
+        # kwargs = parse_args(args)
         return func(value, **kwargs)
     except Exception as e:
         print(e)
-        print(f"Error in transform function: {func_name} for value: {value} with args: {args}")
+        print(f"Error in transform function: {func_name} for value: {value} with args: {kwargs}")
         return value
```

### Comparing `dataweaver-1.0.3/src/data_weaver/utils.py` & `dataweaver-1.0.4/src/data_weaver/utils.py`

 * *Files identical despite different names*

