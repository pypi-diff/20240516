# Comparing `tmp/neon_connector-0.0.1.tar.gz` & `tmp/neon_connector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_connector-0.0.1.tar", last modified: Thu Mar 21 08:22:44 2024, max compression
+gzip compressed data, was "neon_connector-0.0.2.tar", last modified: Wed Mar 27 10:35:20 2024, max compression
```

## Comparing `neon_connector-0.0.1.tar` & `neon_connector-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 08:22:44.307657 neon_connector-0.0.1/
--rw-rw-rw-   0        0        0     1564 2024-03-21 08:22:44.302589 neon_connector-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       93 2024-03-21 07:58:54.000000 neon_connector-0.0.1/README.md
--rw-rw-rw-   0        0        0     1076 2024-03-21 07:57:09.000000 neon_connector-0.0.1/license.txt
--rw-rw-rw-   0        0        0       90 2024-03-21 08:19:33.000000 neon_connector-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      533 2024-03-21 08:22:44.310589 neon_connector-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-21 08:22:44.197572 neon_connector-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 08:22:44.253963 neon_connector-0.0.1/src/neon_connector/
--rw-rw-rw-   0        0        0        0 2024-03-21 07:46:04.000000 neon_connector-0.0.1/src/neon_connector/__init__.py
--rw-rw-rw-   0        0        0     7715 2024-03-14 09:57:39.000000 neon_connector-0.0.1/src/neon_connector/neon_connector.py
-drwxrwxrwx   0        0        0        0 2024-03-21 08:22:44.297268 neon_connector-0.0.1/src/neon_connector.egg-info/
--rw-rw-rw-   0        0        0     1564 2024-03-21 08:22:44.000000 neon_connector-0.0.1/src/neon_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-03-21 08:22:44.000000 neon_connector-0.0.1/src/neon_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 08:22:44.000000 neon_connector-0.0.1/src/neon_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-03-21 08:22:44.000000 neon_connector-0.0.1/src/neon_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-21 08:22:44.000000 neon_connector-0.0.1/src/neon_connector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 10:35:20.754568 neon_connector-0.0.2/
+-rw-rw-rw-   0        0        0     1564 2024-03-27 10:35:20.753629 neon_connector-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2024-03-21 07:58:54.000000 neon_connector-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1076 2024-03-21 07:57:09.000000 neon_connector-0.0.2/license.txt
+-rw-rw-rw-   0        0        0       90 2024-03-21 08:19:33.000000 neon_connector-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      533 2024-03-27 10:35:20.759834 neon_connector-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-27 10:35:20.627910 neon_connector-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-03-27 10:35:20.699832 neon_connector-0.0.2/src/neon_connector/
+-rw-rw-rw-   0        0        0        0 2024-03-21 07:46:04.000000 neon_connector-0.0.2/src/neon_connector/__init__.py
+-rw-rw-rw-   0        0        0     7926 2024-03-27 10:32:33.000000 neon_connector-0.0.2/src/neon_connector/neon_connector.py
+drwxrwxrwx   0        0        0        0 2024-03-27 10:35:20.743373 neon_connector-0.0.2/src/neon_connector.egg-info/
+-rw-rw-rw-   0        0        0     1564 2024-03-27 10:35:20.000000 neon_connector-0.0.2/src/neon_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-03-27 10:35:20.000000 neon_connector-0.0.2/src/neon_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 10:35:20.000000 neon_connector-0.0.2/src/neon_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-03-27 10:35:20.000000 neon_connector-0.0.2/src/neon_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-03-27 10:35:20.000000 neon_connector-0.0.2/src/neon_connector.egg-info/top_level.txt
```

### Comparing `neon_connector-0.0.1/PKG-INFO` & `neon_connector-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_connector
-Version: 0.0.1
+Version: 0.0.2
 Summary: package to connect to the Neon database through Python and perform operations on it
 Author: Timotius Marselo
 Author-email: timotiusmarselo@gmail.com
 Description-Content-Type: text/markdown
 License-File: license.txt
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: psycopg2==2.9.9
```

### Comparing `neon_connector-0.0.1/license.txt` & `neon_connector-0.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `neon_connector-0.0.1/setup.cfg` & `neon_connector-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 656f 6e5f 636f 6e6e 6563 746f   = neon_connecto
 00000020: 720d 0a61 7574 686f 7220 3d20 5469 6d6f  r..author = Timo
 00000030: 7469 7573 204d 6172 7365 6c6f 0d0a 6175  tius Marselo..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 2074 696d  thor_email = tim
 00000050: 6f74 6975 736d 6172 7365 6c6f 4067 6d61  otiusmarselo@gma
 00000060: 696c 2e63 6f6d 0d0a 7665 7273 696f 6e20  il.com..version 
-00000070: 3d20 302e 302e 310d 0a64 6573 6372 6970  = 0.0.1..descrip
+00000070: 3d20 302e 302e 320d 0a64 6573 6372 6970  = 0.0.2..descrip
 00000080: 7469 6f6e 203d 2070 6163 6b61 6765 2074  tion = package t
 00000090: 6f20 636f 6e6e 6563 7420 746f 2074 6865  o connect to the
 000000a0: 204e 656f 6e20 6461 7461 6261 7365 2074   Neon database t
 000000b0: 6872 6f75 6768 2050 7974 686f 6e20 616e  hrough Python an
 000000c0: 6420 7065 7266 6f72 6d20 6f70 6572 6174  d perform operat
 000000d0: 696f 6e73 206f 6e20 6974 0d0a 6c6f 6e67  ions on it..long
 000000e0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `neon_connector-0.0.1/src/neon_connector/neon_connector.py` & `neon_connector-0.0.2/src/neon_connector/neon_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,22 @@
     def _cast_int(self, num):
         if pd.notna(num):
             return round(num)
         else:
             return None
 
     def convert_df_to_records(self, df, int_cols=[], json_cols=[]):
+        def convert_json(x):
+            if type(x) == list:
+                return json.dumps(x) if pd.notna(x).any() else None
+            else:
+                return json.dumps(x) if pd.notna(x) else None
+        
         temp_df = df.copy()
-        temp_df[json_cols] = temp_df[json_cols].map(lambda x: json.dumps(x) if pd.notna(x) else None)
+        temp_df[json_cols] = temp_df[json_cols].map(convert_json)
         
         for col in temp_df.columns:
             if temp_df[col].dtype == "datetime64[ns]":
                 temp_df[col] = temp_df[col].astype(str)
         
         temp_df["updated_on"] = pd.Timestamp.now(tz="GMT").strftime("%Y-%m-%d %H:%M:%S")
         temp_df = temp_df.replace({np.nan: None, 'NaT': None})
@@ -165,15 +171,15 @@
             print("Error:", e)
             self.connection.rollback()
 
         finally:
             self._exit()
             
     def execute_function(self, function_name, args=[]):
-        """Execute a stored function with the given name and arguments. Only use this function for DML functions (INSERT, UPDATE, DELETE).
+        """Execute a stored function with the given name and arguments. If the function is a select query, it's suggested to use the select_query method instead.
 
         Args:
             function_name (str): The name of the function to execute.
             args (list, optional): A list of arguments to pass to the function. Defaults to [].
 
         Returns:
             Any: The result returned by the function.
```

### Comparing `neon_connector-0.0.1/src/neon_connector.egg-info/PKG-INFO` & `neon_connector-0.0.2/src/neon_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_connector
-Version: 0.0.1
+Version: 0.0.2
 Summary: package to connect to the Neon database through Python and perform operations on it
 Author: Timotius Marselo
 Author-email: timotiusmarselo@gmail.com
 Description-Content-Type: text/markdown
 License-File: license.txt
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: psycopg2==2.9.9
```

