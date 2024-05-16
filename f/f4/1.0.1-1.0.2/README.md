# Comparing `tmp/f4-1.0.1.tar.gz` & `tmp/f4-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-1.0.1.tar", last modified: Mon May  6 13:05:07 2024, max compression
+gzip compressed data, was "f4-1.0.2.tar", last modified: Wed May 15 18:18:19 2024, max compression
```

## Comparing `f4-1.0.1.tar` & `f4-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.624354 f4-1.0.1/
--rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-1.0.1/LICENSE
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-05-06 13:05:07.624294 f4-1.0.1/PKG-INFO
--rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-1.0.1/README.md
--rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-1.0.1/pyproject.toml
--rw-r--r--   0 srp33      (503) staff       (20)      733 2024-05-06 13:05:07.624643 f4-1.0.1/setup.cfg
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.619825 f4-1.0.1/src/
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.622579 f4-1.0.1/src/f4/
--rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-1.0.1/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (503) staff       (20)    64912 2024-04-25 15:35:56.000000 f4-1.0.1/src/f4/Parser.py
--rw-r--r--   0 srp33      (503) staff       (20)    18358 2024-05-06 12:34:35.000000 f4-1.0.1/src/f4/Transformer.py
--rwxr-xr-x   0 srp33      (503) staff       (20)     8669 2024-05-06 12:56:18.000000 f4-1.0.1/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-1.0.1/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.624092 f4-1.0.1/src/f4.egg-info/
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (503) staff       (20)      300 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (503) staff       (20)        1 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (503) staff       (20)       67 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (503) staff       (20)        3 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.623459 f4-1.0.1/test/
--rwxr-xr-x   0 srp33      (503) staff       (20)    61473 2024-04-26 13:15:06.000000 f4-1.0.1/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-15 18:18:19.544397 f4-1.0.2/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-1.0.2/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-05-15 18:18:19.544304 f4-1.0.2/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-1.0.2/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-1.0.2/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-05-15 18:18:19.544795 f4-1.0.2/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-15 18:18:19.538397 f4-1.0.2/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-15 18:18:19.541990 f4-1.0.2/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    47478 2024-05-15 18:16:16.000000 f4-1.0.2/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    64921 2024-05-15 17:56:46.000000 f4-1.0.2/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    18444 2024-05-15 18:13:12.000000 f4-1.0.2/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     9765 2024-05-15 18:17:27.000000 f4-1.0.2/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-1.0.2/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-15 18:18:19.544021 f4-1.0.2/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-05-15 18:18:19.000000 f4-1.0.2/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-05-15 18:18:19.000000 f4-1.0.2/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-05-15 18:18:19.000000 f4-1.0.2/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-05-15 18:18:19.000000 f4-1.0.2/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-05-15 18:18:19.000000 f4-1.0.2/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-15 18:18:19.543135 f4-1.0.2/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    61571 2024-05-15 18:17:17.000000 f4-1.0.2/test/test.py
```

### Comparing `f4-1.0.1/LICENSE` & `f4-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-1.0.1/PKG-INFO` & `f4-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-1.0.1/setup.cfg` & `f4-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 1.0.1
+version = 1.0.2
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-1.0.1/src/f4/Builder.py` & `f4-1.0.2/src/f4/Builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,63 +35,90 @@
     # Determine the number of columns per chunk.
     num_cols_per_chunk = ceil(num_cols / num_parallel)
 
     # Separate the column indices into chunks.
     column_chunk_indices = generate_column_chunk_ranges(num_cols, num_cols_per_chunk, num_parallel)
 
     # Create temp directory.
-    tmp_dir_path2 = prepare_tmp_dir(tmp_dir_path)
+    tmp_dir_path2, use_checkpoints = prepare_tmp_dir(tmp_dir_path)
+
+    # Compare the arguments passed to this function against any that
+    # were saved. This code gives me a dictionary with the parameter
+    # names and values.
+    if use_checkpoints:
+        checkpoint_info = locals().copy()
+        checkpoint_file_path = f"{tmp_dir_path2}checkpoint__info"
+        if path.exists(checkpoint_file_path):
+            prior_checkpoint_info = deserialize(read_str_from_file(checkpoint_file_path))
+
+            if prior_checkpoint_info != checkpoint_info:
+                print_message(f"Checkpoint information was found at {checkpoint_file_path}, but it cannot be used because it does not match the arguments specified here.", verbose)
+                for file_path in glob(f"{tmp_dir_path2}checkpoint__*"):
+                    remove_tmp_file(file_path)
+
+                print_message(f"Saving checkpoint information to {checkpoint_file_path}.")
+                write_str_to_file(checkpoint_file_path, serialize(checkpoint_info), False)
 
     # Parse column info into a database for each chunk.
-    joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(parse_column_info)(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, chunk_indices[0], chunk_indices[1], tmp_dir_path2, out_items_chunk_size, verbose) for chunk_number, chunk_indices in enumerate(column_chunk_indices))
+    joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(parse_column_info)(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, chunk_indices[0], chunk_indices[1], tmp_dir_path2, out_items_chunk_size, use_checkpoints, verbose) for chunk_number, chunk_indices in enumerate(column_chunk_indices))
 
     # Save and format data to a temp file for each column chunk.
-    joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(save_formatted_data)(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, chunk_indices[0], chunk_indices[1], tmp_dir_path2, out_items_chunk_size, verbose) for chunk_number, chunk_indices in enumerate(column_chunk_indices))
+    joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(save_formatted_data)(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, chunk_indices[0], chunk_indices[1], tmp_dir_path2, out_items_chunk_size, use_checkpoints, verbose) for chunk_number, chunk_indices in enumerate(column_chunk_indices))
 
     # Combine column databases across the chunks.
-    combine_column_databases(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path2, verbose)
+    combine_column_databases(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path2, use_checkpoints, verbose)
 
     # Create meta files for all columns.
-    save_column_name_info(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, verbose)
-    save_column_types(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, verbose)
-    save_column_coordinates(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, verbose)
+    save_column_name_info(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, use_checkpoints, verbose)
+    save_column_types(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, use_checkpoints, verbose)
+    save_column_coordinates(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path2, use_checkpoints, verbose)
 
     # Merge the saved/formatted data across the column chunks.
-    # Get number of rows.
-    num_rows, line_length = combine_data_for_column_chunks(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path2, verbose)
+    combine_data_for_column_chunks(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path2, use_checkpoints, verbose)
+
+    num_rows = int(read_str_from_file(f"{tmp_dir_path2}num_rows"))
+    line_length_total = int(read_str_from_file(f"{tmp_dir_path2}line_length_total"))
 
     if num_rows == 0:
         raise Exception(f"A header row but no data rows were detected in {delimited_file_path}.")
 
     if index_columns:
-        build_indexes(f4_file_path, tmp_dir_path2, index_columns, num_rows, line_length, num_parallel, get_columns_database_file_path(tmp_dir_path2), verbose)
-
-    remove(get_columns_database_file_path(tmp_dir_path2))
+        build_indexes(f4_file_path, tmp_dir_path2, index_columns, num_rows, line_length_total, num_parallel, get_columns_database_file_path(tmp_dir_path2), use_checkpoints, verbose)
 
     #TODO: Parallelize this by row chunks.
     if compression_type:
-        compress_data(tmp_dir_path2, compression_type, num_rows, line_length)
+        compress_data(delimited_file_path, f4_file_path, tmp_dir_path2, compression_type, num_rows, line_length_total, use_checkpoints, verbose)
     # else:
     #     # The combined file will be compressed, so we need to decompress it.
     #     rename(get_data_path(tmp_dir_path2, "data"), get_data_path(tmp_dir_path2, "datacmpr"))
     #
     #     with open_temp_file(get_data_path(tmp_dir_path2, "datacmpr"), "rb") as cmpr_file:
     #         with open(get_data_path(tmp_dir_path2, "data"), "wb") as data_file:
     #             chunk_size = 1000000
     #             while True:
     #                 content = cmpr_file.read(chunk_size)
     #                 # If the content is empty, end of file has been reached
     #                 if not content:
     #                     break
     #
     #                 data_file.write(content)
-
     combine_into_single_file(delimited_file_path, f4_file_path, tmp_dir_path2, file_read_chunk_size, verbose)
 
-    rmtree(tmp_dir_path2)
+    remove_tmp_file(get_columns_database_file_path(tmp_dir_path2))
+
+    # Remove checkpoint files because we successfully built the file.
+    for file_path in glob(f"{tmp_dir_path2}checkpoint__*"):
+        remove_tmp_file(file_path)
+
+    remove_tmp_file(f"{tmp_dir_path2}num_rows")
+    remove_tmp_file(f"{tmp_dir_path2}line_length_total")
+
+    # Only remove the temp directory if we created it.
+    if not tmp_dir_path:
+        rmtree(tmp_dir_path2)
 
     print_message(f"Done converting {delimited_file_path} to {f4_file_path}.", verbose)
 
 #####################################################
 # Non-public function(s)
 #####################################################
 
@@ -199,15 +226,18 @@
 
         # in_file.seek(current_index + newline_index + 1)
 
     if len(save_tuples) > 0:
         cursor.executemany(sql, save_tuples)
 
 # This function is executed in parallel.
-def parse_column_info(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, start_column_index, end_column_index, tmp_dir_path, out_items_chunk_size, verbose):
+def parse_column_info(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, start_column_index, end_column_index, tmp_dir_path, out_items_chunk_size, use_checkpoints, verbose):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, chunk_number, verbose):
+        return
+
     print_message(f"Parsing column names, sizes, and types when converting {delimited_file_path} to {f4_file_path} for columns {start_column_index} - {end_column_index - 1}.", verbose)
 
     columns_file_path = get_columns_database_file_path(tmp_dir_path, chunk_number)
     conn = connect_sql(columns_file_path)
     cursor = conn.cursor()
     cursor.execute('BEGIN TRANSACTION')
 
@@ -224,14 +254,16 @@
     with get_delimited_file_handle(delimited_file_path) as in_file:
         skip_comments(in_file, comment_prefix)
         skip_line(in_file) # Header line
 
         # Loop through the file for the specified columns and update the dictionaries.
         save_tuples = []
         for column_index, value in iterate_delimited_file_column_indices(in_file, delimiter, file_read_chunk_size, start_column_index, end_column_index):
+            print_message(f"Parsing column names, sizes, and types for column_index {column_index} when converting {delimited_file_path} to {f4_file_path} for columns {start_column_index} - {end_column_index - 1}.", verbose, column_index)
+
             if column_index == start_column_index:
                 num_rows += 1
 
             if start_column_index <= column_index < end_column_index:
                 this_size = len(value)
                 i, f, s = infer_type(value)
 
@@ -255,30 +287,35 @@
 
     cursor.executemany(sql_infer_type, ((column_index,) for column_index in range(start_column_index, end_column_index)))
 
     conn.commit()
     cursor.close()
     conn.close()
 
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, chunk_number)
+
     print_message(f"Done parsing column names, sizes, and types when converting {delimited_file_path} to {f4_file_path} for columns {start_column_index} - {end_column_index - 1}.", verbose)
 
 # This function is executed in parallel.
-def save_formatted_data(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, start_column_index, end_column_index, tmp_dir_path, out_items_chunk_size, verbose):
+def save_formatted_data(delimited_file_path, f4_file_path, comment_prefix, delimiter, file_read_chunk_size, chunk_number, start_column_index, end_column_index, tmp_dir_path, out_items_chunk_size, use_checkpoints, verbose):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, chunk_number, verbose):
+        return
+
     print_message(f"Saving formatted data when converting {delimited_file_path} to {f4_file_path} for columns {start_column_index} - {end_column_index - 1}.", verbose)
 
     columns_file_path = get_columns_database_file_path(tmp_dir_path, chunk_number)
     conn = connect_sql(columns_file_path)
     cursor = conn.cursor()
 
     cursor.execute('''SELECT SUM(size) AS size
                       FROM columns
                       WHERE column_index BETWEEN ? AND ?''', (start_column_index, end_column_index,))
     line_length = cursor.fetchone()["size"]
 
-    write_str_to_file(get_data_path(tmp_dir_path, "ll", chunk_number), str(line_length).encode())
+    write_str_to_file(get_data_path(tmp_dir_path, "ll", chunk_number), str(line_length).encode(), False)
 
     with get_delimited_file_handle(delimited_file_path) as in_file:
         skip_comments(in_file, comment_prefix)
         skip_line(in_file)  # Header line
 
         # Save data.
         with open_temp_file_to_compress(get_data_path(tmp_dir_path, "data", chunk_number)) as data_file:
@@ -292,14 +329,16 @@
                 cursor.execute('''SELECT size
                                   FROM columns''')
 
                 for column_index in range(start_column_index, end_column_index):
                     column_size_cache[column_index] = cursor.fetchone()["size"]
 
             for column_index, value in iterate_delimited_file_column_indices(in_file, delimiter, file_read_chunk_size, start_column_index, end_column_index):
+                print_message(f"Saving formatted data for column index {column_index} when converting {delimited_file_path} to {f4_file_path} for columns {start_column_index} - {end_column_index - 1}.", verbose, column_index)
+
                 if len(column_size_cache) == 0:
                     if column_index == start_column_index:
                         cursor.close()
                         cursor = conn.cursor()
                         cursor.execute('''SELECT size
                                           FROM columns''')
 
@@ -315,44 +354,56 @@
 
             if len(out_list) > 0:
                 data_file.write(b"".join(out_list))
 
     cursor.close()
     conn.close()
 
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, chunk_number)
+
     print_message(f"Done saving formatted data when converting {delimited_file_path} to {f4_file_path} for columns {start_column_index} - {end_column_index - 1}.", verbose)
 
-def combine_column_databases(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path, verbose):
+def combine_column_databases(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path, use_checkpoints, verbose):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, 0, verbose):
+        return
+
     # Combine the column sizes and types across the chunks.
     # We won't add the num_* columns to the combined file because they are no longer necessary.
     print_message(f"Combining column databases when converting {delimited_file_path} to {f4_file_path}.", verbose)
 
     conn_0 = connect_sql(get_columns_database_file_path(tmp_dir_path, 0))
     cursor_0 = conn_0.cursor()
 
     for chunk_number in range(1, len(column_chunk_indices)):
         chunk_file_path = get_columns_database_file_path(tmp_dir_path, chunk_number)
         cursor_0.execute(f"ATTACH DATABASE '{chunk_file_path}' AS db_chunk")
         cursor_0.execute(f"INSERT INTO columns (column_index, column_name, size, inferred_type) SELECT column_index, column_name, size, inferred_type FROM db_chunk.columns")
         cursor_0.execute("DETACH DATABASE db_chunk")
-        remove(chunk_file_path)
 
     cursor_0.close()
     conn_0.close()
 
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, 0)
+
     rename(get_columns_database_file_path(tmp_dir_path, 0), get_columns_database_file_path(tmp_dir_path))
 
+    for chunk_number in range(1, len(column_chunk_indices)):
+        remove_tmp_file(get_columns_database_file_path(tmp_dir_path, chunk_number))
+
 def get_max_column_length(cursor, column_name):
     sql = f'''SELECT MAX(LENGTH(CAST({column_name} AS TEXT))) AS max_length
               FROM columns'''
 
     cursor.execute(sql)
     return cursor.fetchone()["max_length"]
 
-def save_column_name_info(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path, verbose):
+def save_column_name_info(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path, use_checkpoints, verbose):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, 0, verbose):
+        return
+
     print_message(f"Saving column name info when converting {delimited_file_path} to {f4_file_path}.", verbose)
 
     conn = connect_sql(get_columns_database_file_path(tmp_dir_path))
     cursor = conn.cursor()
 
     max_column_name_length = get_max_column_length(cursor, "column_name")
     max_column_index_length = get_max_column_length(cursor, "column_index")
@@ -416,15 +467,20 @@
             cn_file_original_size += data_file.write(b"\n".join(out_list))
 
     cursor.close()
     conn.close()
 
     write_temp_file_original_size(get_data_path(tmp_dir_path, "cn"), cn_file_original_size)
 
-def save_column_types(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path, verbose):
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, 0)
+
+def save_column_types(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path, use_checkpoints, verbose):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, 0, verbose):
+        return
+
     print_message(f"Saving column type and size info when converting {delimited_file_path} to {f4_file_path}.", verbose)
 
     conn = connect_sql(get_columns_database_file_path(tmp_dir_path))
     cursor = conn.cursor()
 
     max_type_length = 1 # This should always be 1 unless we add a bunch of types.
 
@@ -448,15 +504,20 @@
             ct_file_original_size += data_file.write(b"".join(out_list))
 
     cursor.close()
     conn.close()
 
     write_temp_file_original_size(get_data_path(tmp_dir_path, "ct"), ct_file_original_size)
 
-def save_column_coordinates(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path, verbose):
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, 0)
+
+def save_column_coordinates(delimited_file_path, f4_file_path, out_items_chunk_size, tmp_dir_path, use_checkpoints, verbose):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, 0, verbose):
+        return
+
     print_message(f"Saving column coordinates when converting {delimited_file_path} to {f4_file_path}.", verbose)
 
     conn = connect_sql(get_columns_database_file_path(tmp_dir_path))
     cursor = conn.cursor()
 
     sql = f'''SELECT SUM(size) AS size
               FROM columns'''
@@ -490,26 +551,30 @@
     cursor.close()
     conn.close()
 
     write_temp_file_original_size(get_data_path(tmp_dir_path, "cc"), cc_file_original_size)
 
     write_str_to_file(get_data_path(tmp_dir_path, "ccml"), str(max_coord_length).encode())
 
-def combine_data_for_column_chunks(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path, verbose):
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, 0)
+
+def combine_data_for_column_chunks(delimited_file_path, f4_file_path, column_chunk_indices, tmp_dir_path, use_checkpoints, verbose):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, 0, verbose):
+        return
+
     print_message(f"Combining data for column chunks when converting {delimited_file_path} to {f4_file_path}.", verbose)
 
     file_handles = {}
     for chunk_number in range(len(column_chunk_indices)):
         file_handles[chunk_number] = open_temp_file_compressed(get_data_path(tmp_dir_path, "data", chunk_number))
 
     line_lengths = {}
     for chunk_number in range(len(column_chunk_indices)):
         line_length_file_path = get_data_path(tmp_dir_path, "ll", chunk_number)
         line_lengths[chunk_number] = int(read_str_from_file(line_length_file_path))
-        remove(line_length_file_path)
 
     line_length_total = sum(line_lengths.values())
 
     out_file_original_size = 0
     with open_temp_file_to_compress(get_data_path(tmp_dir_path, "data")) as out_file:
         num_rows = 0
         while line_0 := file_handles[0].read(line_lengths[0]):
@@ -517,88 +582,28 @@
             out_file_original_size += out_file.write(line_0)
 
             for chunk_number in range(1, len(column_chunk_indices)):
                 out_file_original_size += out_file.write(file_handles[chunk_number].read(line_lengths[chunk_number]))
 
     write_temp_file_original_size(get_data_path(tmp_dir_path, "data"), out_file_original_size)
 
-    for chunk_number in range(len(column_chunk_indices)):
-        file_handles[chunk_number].close()
-        remove(get_data_path(tmp_dir_path, "data", chunk_number))
-
-    return num_rows, line_length_total
-
-def compress_data(tmp_dir_path, compression_type, num_rows, line_length):
-    # For now, we assume z-standard compression.
-    compressor = ZstdCompressor(level=1)
-
-    # Compress the data.
-    # TODO: If necessary, chunk the compression so we can handle extremely wide files.
-    compressed_row_ends = []
-    current_compressed_row_end = 0
-    compressed_lines_to_save = []
-    compressed_chars_not_saved = 0
-
-    with open_temp_file_compressed(get_data_path(tmp_dir_path, "data")) as file_handle:
-        cmpr_file_original_size = 0
-
-        with open_temp_file_to_compress(get_data_path(tmp_dir_path, "cmpr")) as cmpr_file:
-            with open_temp_file_to_compress(get_data_path(tmp_dir_path, "re_tmp")) as re_tmp_file:
-                for row_i in range(num_rows):
-                    row_start = row_i * line_length
-                    row_end = (row_i + 1) * line_length
-
-                    file_handle.seek(row_start)
-                    row = file_handle.read(row_end - row_start)
-                    compressed_line = compressor.compress(row)
-                    compressed_row_length = len(compressed_line)
-
-                    current_compressed_row_end += compressed_row_length
-                    compressed_row_ends.append(current_compressed_row_end)
-                    compressed_lines_to_save.append(compressed_line)
-                    compressed_chars_not_saved += compressed_row_length
-
-                    if compressed_chars_not_saved >= 1000000:
-                        cmpr_file_original_size += cmpr_file.write(b"".join(compressed_lines_to_save))
-
-                        re_tmp_file.write(b"\n".join([str(rl).encode() for rl in compressed_row_ends]))
-                        if row_i != (num_rows - 1):
-                            re_tmp_file.write(b"\n")
-
-                        mrel = len(str(compressed_row_ends[-1]))
-                        compressed_row_ends = []
-                        compressed_lines_to_save = []
-                        compressed_chars_not_saved = 0
-
-                if compressed_chars_not_saved > 0:
-                    cmpr_file_original_size += cmpr_file.write(b"".join(compressed_lines_to_save))
-                    re_tmp_file.write(b"\n".join([str(rl).encode() for rl in compressed_row_ends]))
-
-    rename(get_data_path(tmp_dir_path, "cmpr"), get_data_path(tmp_dir_path, "data"))
-    write_temp_file_original_size(get_data_path(tmp_dir_path, "data"), cmpr_file_original_size)
-
-    if len(compressed_row_ends) > 0:
-        mrel = len(str(compressed_row_ends[-1]))
-
-    write_str_to_file(get_data_path(tmp_dir_path, "mrel"), str(mrel).encode())
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, 0)
 
-    re_file_original_size = 0
-    with open_temp_file_to_compress(get_data_path(tmp_dir_path, "re")) as re_file:
-        for line in read_compressed_file_line_by_line(get_data_path(tmp_dir_path, "re_tmp")):
-            row_end = line.rstrip(b"\n")
-            re_file_original_size += re_file.write(format_string_as_fixed_width(row_end, mrel))
+    for chunk_number in range(len(column_chunk_indices)):
+        remove_tmp_file(get_data_path(tmp_dir_path, "ll", chunk_number))
+        remove_tmp_file(get_data_path(tmp_dir_path, "data", chunk_number))
 
-    write_temp_file_original_size(get_data_path(tmp_dir_path, "re"), re_file_original_size)
-    remove(get_data_path(tmp_dir_path, "re_tmp"))
+    # We save these numbers to files so we can retrieve them when checkpoints are used.
+    write_str_to_file(f"{tmp_dir_path}num_rows", str(num_rows).encode(), False)
+    write_str_to_file(f"{tmp_dir_path}line_length_total", str(line_length_total).encode(), False)
 
-    write_str_to_file(get_data_path(tmp_dir_path, "ll"), str(line_length).encode())
-    write_str_to_file(get_data_path(tmp_dir_path, "nrow"), str(num_rows).encode())
-    write_str_to_file(get_data_path(tmp_dir_path, "cmpr"), b"z")
+def build_indexes(f4_file_path, tmp_dir_path, index_columns, num_rows, line_length, num_parallel, columns_database_file_path, use_checkpoints, verbose=False):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, 0, verbose):
+        return
 
-def build_indexes(f4_file_path, tmp_dir_path, index_columns, num_rows, line_length, num_parallel, columns_database_file_path, verbose=False):
     index_info_dict = {}
 
     if isinstance(index_columns, str):
         index_columns, reverse_status_dict = check_index_column_reverse_status([index_columns])
 
         build_index(f4_file_path, tmp_dir_path, 0, index_columns, reverse_status_dict, num_rows, line_length, columns_database_file_path, verbose)
         index_info_dict[(index_columns, reverse_status_dict[index_columns])] = 0
@@ -620,14 +625,16 @@
         for i, key in enumerate(keys):
             index_info_dict[key] = i
     else:
         raise Exception("When specifying index columns, they must either be a string or a list.")
 
     write_str_to_file(f"{tmp_dir_path}i", serialize(index_info_dict))
 
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, 0)
+
 def build_index(f4_file_path, tmp_dir_path, index_number, index_columns, reverse_status_dict, num_rows, line_length, columns_database_file_path, verbose):
     out_index_file_path_prefix = f"{tmp_dir_path}i{index_number}"
     ccml = fast_int(read_str_from_file(get_data_path(tmp_dir_path, "ccml")))
 
     print_message(f"Saving index information for {', '.join(index_columns)} column(s) in {f4_file_path}.", verbose)
 
     # Collect other information about each column.
@@ -774,15 +781,15 @@
     write_str_to_file(f"{out_index_file_path_prefix}ccml", str(ccml).encode())
 
     cc = b""
     for x in coords:
         cc += format_string_as_fixed_width(x, ccml)
     write_str_to_file(f"{out_index_file_path_prefix}cc", cc)
 
-    remove(index_database_file_path)
+    remove_tmp_file(index_database_file_path)
 
     print_message(f"Done building index for {', '.join(index_columns)} column(s) in {f4_file_path}.", verbose)
 
 def build_index_parallel(f4_file_path, tmp_dir_path, num_rows, line_length, index_number, index_column, columns_database_file_path, verbose):
     index_column_list = [index_column] if isinstance(index_column, str) else index_column
     index_column_list, reverse_status_dict = check_index_column_reverse_status(index_column_list)
 
@@ -802,39 +809,14 @@
             index_columns[i] = index_column.rstrip("_endswith")
             reverse_status_dict[index_columns[i]] = True
         else:
             reverse_status_dict[index_column] = False
 
     return index_columns, reverse_status_dict
 
-# def get_column_index_and_type(tmp_dir_path, index_column_name):
-#     columns_file_path = get_columns_database_file_path(tmp_dir_path)
-#
-#     conn = connect_sql(columns_file_path)
-#     cursor = conn.cursor()
-#
-#     cursor.execute('''SELECT column_index, inferred_type
-#                       FROM columns
-#                       WHERE TRIM(column_name) = ?''', (index_column_name, ))
-#
-#     row = cursor.fetchone()
-#
-#     if not row:
-#         raise Exception(f"No column exists with the name '{index_column_name}.'")
-#         cursor.close()
-#         conn.close()
-#
-#     index_column_index = row["column_index"]
-#     index_column_type = row["inferred_type"]
-#
-#     cursor.close()
-#     conn.close()
-#
-#     return index_column_index, index_column_type
-
 def get_column_index_coords(tmp_dir_path, index_column_index, ccml):
     with open_temp_file_compressed(get_data_path(tmp_dir_path, "cc")) as file_handle:
         # with mmap(file_handle.fileno(), 0, prot=PROT_READ) as mmap_handle:
         pos_a = index_column_index * ccml
         pos_b = pos_a + ccml
         pos_c = pos_b + ccml
 
@@ -842,14 +824,89 @@
         file_handle.seek(pos_a)
         coord1 = file_handle.read(pos_b - pos_a)
         file_handle.seek(pos_b)
         coord2 = file_handle.read(pos_c - pos_b)
 
         return fast_int(coord1), fast_int(coord2)
 
+def compress_data(delimited_file_path, f4_file_path, tmp_dir_path, compression_type, num_rows, line_length, use_checkpoints, verbose):
+    if has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, 0, verbose):
+        return
+
+    print_message(f"Compressing data for {delimited_file_path} to {f4_file_path}.", verbose)
+
+    # For now, we assume z-standard compression.
+    compressor = ZstdCompressor(level=1)
+
+    # Compress the data.
+    # TODO: If necessary, chunk the compression so we can handle extremely wide files.
+    compressed_row_ends = []
+    current_compressed_row_end = 0
+    compressed_lines_to_save = []
+    compressed_chars_not_saved = 0
+
+    with open_temp_file_compressed(get_data_path(tmp_dir_path, "data")) as file_handle:
+        cmpr_file_original_size = 0
+
+        with open_temp_file_to_compress(get_data_path(tmp_dir_path, "cmpr")) as cmpr_file:
+            with open_temp_file_to_compress(get_data_path(tmp_dir_path, "re_tmp")) as re_tmp_file:
+                for row_i in range(num_rows):
+                    row_start = row_i * line_length
+                    row_end = (row_i + 1) * line_length
+
+                    file_handle.seek(row_start)
+                    row = file_handle.read(row_end - row_start)
+                    compressed_line = compressor.compress(row)
+                    compressed_row_length = len(compressed_line)
+
+                    current_compressed_row_end += compressed_row_length
+                    compressed_row_ends.append(current_compressed_row_end)
+                    compressed_lines_to_save.append(compressed_line)
+                    compressed_chars_not_saved += compressed_row_length
+
+                    if compressed_chars_not_saved >= 1000000:
+                        cmpr_file_original_size += cmpr_file.write(b"".join(compressed_lines_to_save))
+
+                        re_tmp_file.write(b"\n".join([str(rl).encode() for rl in compressed_row_ends]))
+                        if row_i != (num_rows - 1):
+                            re_tmp_file.write(b"\n")
+
+                        mrel = len(str(compressed_row_ends[-1]))
+                        compressed_row_ends = []
+                        compressed_lines_to_save = []
+                        compressed_chars_not_saved = 0
+
+                if compressed_chars_not_saved > 0:
+                    cmpr_file_original_size += cmpr_file.write(b"".join(compressed_lines_to_save))
+                    re_tmp_file.write(b"\n".join([str(rl).encode() for rl in compressed_row_ends]))
+
+    if len(compressed_row_ends) > 0:
+        mrel = len(str(compressed_row_ends[-1]))
+
+    write_str_to_file(get_data_path(tmp_dir_path, "mrel"), str(mrel).encode())
+
+    re_file_original_size = 0
+    with open_temp_file_to_compress(get_data_path(tmp_dir_path, "re")) as re_file:
+        for line in read_compressed_file_line_by_line(get_data_path(tmp_dir_path, "re_tmp")):
+            row_end = line.rstrip(b"\n")
+            re_file_original_size += re_file.write(format_string_as_fixed_width(row_end, mrel))
+
+    write_temp_file_original_size(get_data_path(tmp_dir_path, "re"), re_file_original_size)
+
+    record_checkpoint_reached(use_checkpoints, tmp_dir_path, 0)
+
+    rename(get_data_path(tmp_dir_path, "cmpr"), get_data_path(tmp_dir_path, "data"))
+    write_temp_file_original_size(get_data_path(tmp_dir_path, "data"), cmpr_file_original_size)
+
+    write_str_to_file(get_data_path(tmp_dir_path, "ll"), str(line_length).encode())
+    write_str_to_file(get_data_path(tmp_dir_path, "nrow"), str(num_rows).encode())
+    write_str_to_file(get_data_path(tmp_dir_path, "cmpr"), b"z")
+
+    remove_tmp_file(get_data_path(tmp_dir_path, "re_tmp"))
+
 def combine_into_single_file(delimited_file_path, f4_file_path, tmp_dir_path, read_chunk_size, verbose):
     def _create_file_map(start_end_positions):
         start_end_dict = {}
 
         for x in start_end_positions:
             file_extension = x[0]
             positions = x[1:]
@@ -860,15 +917,16 @@
 
     print_message(f"Combining data into a single file for {delimited_file_path} to {f4_file_path}.", verbose)
 
     write_str_to_file(f"{tmp_dir_path}ver", get_current_version_major().encode())
 
     start_end_positions = []
     for file_path in sorted(glob(f"{tmp_dir_path}*")):
-        if file_path.endswith("__original_size"):
+        file_name = path.basename(file_path)
+        if file_path.endswith("__original_size") or file_name.startswith("checkpoint__") or file_name == "columns.db" or file_name == "num_rows" or file_name == "line_length_total":
             continue
 
         extension = path.basename(file_path)
         extension = "" if extension == "data" else extension
         # file_size = path.getsize(file_path)
         file_size = get_temp_file_original_size(file_path)
 
@@ -899,22 +957,24 @@
 
     # Write the output file
     with open(f4_file_path, "wb") as f4_file:
         f4_file.write(file_map_serialized)
 
         for file_start_end in start_end_positions:
             file_path = f"{tmp_dir_path}{file_start_end[0]}"
+
             if file_start_end[0] == "":
                 file_path += "data"
 
             with open_temp_file_compressed(file_path) as component_file:
                 while chunk := component_file.read(read_chunk_size):
                     f4_file.write(chunk)
 
-            remove(file_path)
+            remove_tmp_file(file_path)
+            remove_tmp_file(f"{file_path}__original_size")
 
 def skip_comments(in_file, comment_prefix):
     if comment_prefix is None:
         return
 
     next_text = in_file.read(len(comment_prefix))
```

### Comparing `f4-1.0.1/src/f4/Parser.py` & `f4-1.0.2/src/f4/Parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,15 +582,15 @@
                                 write_obj.write(chunk_file.readline().rstrip(b"\n") + b"\t")
 
                     for chunk_file in chunk_file_dict.values():
                         chunk_file.close()
 
             for row_chunk_number in range(num_row_index_chunks):
                 for column_chunk_number in range(num_select_column_chunks):
-                    remove(f"{tmp_dir_path}{row_chunk_number}_{column_chunk_number}")
+                    remove_tmp_file(f"{tmp_dir_path}{row_chunk_number}_{column_chunk_number}")
 
     # TODO: Use the RangeSet or intervaltree packages to store discrete
     #         indices more compactly (and quickly)?
 
 def head(data_file_path, n=10, select_columns=None, out_file_path=None, out_file_type="tsv"):
     if not select_columns:
         select_columns = []
```

### Comparing `f4-1.0.1/src/f4/Transformer.py` & `f4-1.0.2/src/f4/Transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
     print_message(f"Finding max column width when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
 
     with initialize(f4_src_file_path, use_memory_mapping) as src_file_data:
         num_cols = src_file_data.cache_dict["num_cols"]
         max_column_width = get_max_column_width(src_file_data)
 
-    tmp_dir_path2 = prepare_tmp_dir(tmp_dir_path)
+    # TODO: Support checkpoints.
+    tmp_dir_path2, use_checkpoints = prepare_tmp_dir(tmp_dir_path)
     tmp_tsv_file_path = f"{tmp_dir_path2}transposed.tsv.zstd"
 
     if num_parallel == 1:
         transpose_column_chunk(f4_src_file_path, use_memory_mapping, src_column_for_names, 0, range(num_cols), max_column_width, tmp_tsv_file_path, verbose)
     else:
         max_cols_per_chunk = 10001
 
@@ -42,20 +43,20 @@
         with open_temp_file_to_compress(tmp_tsv_file_path, "wb") as tmp_tsv_file:
             for chunk_number, _ignore in enumerate(generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel)):
                 chunk_file_path = f"{tmp_dir_path2}transposed_chunk_{chunk_number}.tsv.zstd"
 
                 for line in read_compressed_file_line_by_line(chunk_file_path):
                     tmp_tsv_file.write(line + b"\n")
 
-                remove(chunk_file_path)
+                remove_tmp_file(chunk_file_path)
 
     print_message(f"Converting temp file at {tmp_tsv_file_path} when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
     convert_delimited_file(tmp_tsv_file_path, f4_dest_file_path, comment_prefix=None, compression_type=src_file_data.decompression_type, index_columns=index_columns, num_parallel=num_parallel, verbose=verbose)
 
-    remove(tmp_tsv_file_path)
+    remove_tmp_file(tmp_tsv_file_path)
     rmtree(tmp_dir_path2)
 
 def generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel):
     if num_cols > max_cols_per_chunk:
         column_ranges = generate_range_chunks(num_cols, max_cols_per_chunk)
     else:
         column_ranges = generate_range_chunks(num_cols, ceil(num_cols / num_parallel))
@@ -165,15 +166,15 @@
         with open(tmp_fw_file_path, "rb") as fw_file:
             with open_temp_file_to_compress(tmp_tsv_file_path) as tsv_file:
                 for line in fw_file:
                     line_items = line.rstrip(b"\n").split(b"\t")
                     line_items = [x.rstrip(b" ") for x in line_items]
                     tsv_file.write(b"\t".join(line_items) + b"\n")
 
-        remove(tmp_fw_file_path)
+        remove_tmp_file(tmp_fw_file_path)
 
 def advance_to_column_names(src_file_data, first_col_index):
     cn_current = src_file_data.file_map_dict["cn"][0]
     cn_end = src_file_data.file_map_dict["cn"][1]
 
     # Advance to the first column name for this chunk range.
     for column_index in range(first_col_index):
@@ -297,9 +298,9 @@
             compression_type = None
             if left_file_data.decompression_type == "zstd" or right_file_data.decompression_type == "zstd":
                 compression_type = "zstd"
 
             print_message(f"Converting temp file at {tmp_tsv_file_path} to {f4_dest_file_path}.", verbose)
             convert_delimited_file(tmp_tsv_file_path, f4_dest_file_path, compression_type=compression_type, index_columns=index_columns, num_parallel=num_parallel, comment_prefix=None, verbose=verbose)
 
-    remove(tmp_tsv_file_path)
+    remove_tmp_file(tmp_tsv_file_path)
     rmtree(tmp_dir_path)
```

### Comparing `f4-1.0.1/src/f4/Utilities.py` & `f4-1.0.2/src/f4/Utilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from contextlib import contextmanager
 from copy import deepcopy
 import csv
 from datetime import datetime
 from glob import glob
 import gzip
 from fastnumbers import isint, isfloat, fast_int, fast_float
+from inspect import stack
 from itertools import chain
 from math import ceil, log
 from mmap import mmap, PROT_READ, PROT_WRITE
 from msgspec import msgpack
 from operator import eq, ge, gt, le, lt, ne, itemgetter
 from os import makedirs, path, remove, rename
 from re import compile
@@ -17,15 +18,15 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "1.0.1"
+    return "1.0.2"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
@@ -37,19 +38,20 @@
         file_handle.seek(start_position)
         return file_handle.read(end_position - start_position)
 
 def read_str_from_file(file_path, file_extension=""):
     with open_temp_file_compressed(file_path + file_extension) as the_file:
         return the_file.read()
 
-def write_str_to_file(file_path, the_string):
+def write_str_to_file(file_path, the_string, save_original_size=True):
     with open_temp_file_to_compress(file_path) as the_file:
         the_file.write(the_string)
 
-    write_temp_file_original_size(file_path, len(the_string))
+    if save_original_size:
+        write_temp_file_original_size(file_path, len(the_string))
 
 def print_message(message, verbose=False, count=None):
     if verbose:
         if count:
             for y in range(20, 0, -1):
                 if count <= 10**y and count % 10**(y - 1) == 0:
                     sys.stderr.write(f"{message} - count = {count} - {datetime.now().strftime('%d/%m/%Y %H:%M:%S.%f')}\n")
@@ -61,14 +63,33 @@
 
 def do_nothing(x):
      return(x)
 
 def reverse_string(s):
     return s[::-1]
 
+def has_checkpoint_been_reached_previously(use_checkpoints, tmp_dir_path, chunk_number, verbose):
+    # This gets the name of the function that called this function.
+    checkpoint_name = stack()[1].function
+    checkpoint_file_path = f"{tmp_dir_path}checkpoint__{checkpoint_name}__{chunk_number}"
+
+    if use_checkpoints and path.exists(checkpoint_file_path):
+        print_message(f"Using previously saved data for checkpoint {checkpoint_name} from {checkpoint_file_path}.", verbose)
+        return True
+
+    return False
+
+def record_checkpoint_reached(use_checkpoints, tmp_dir_path, chunk_number):
+    # This gets the name of the function that called this function.
+    checkpoint_name = stack()[1].function
+    checkpoint_file_path = f"{tmp_dir_path}checkpoint__{checkpoint_name}__{chunk_number}"
+
+    if use_checkpoints:
+        write_str_to_file(checkpoint_file_path, b"", False)
+
 def get_delimited_file_handle(file_path):
     if file_path.endswith(".gz"):
         return gzip.open(file_path)
     elif file_path.endswith(".zstd"):
         # FYI: This compression format is a hidden feature for input files.
         # Skipping comments is not supported.
         return open_temp_file_compressed(file_path)
@@ -179,34 +200,37 @@
 def fix_dir_path_ending(dir_path):
     return dir_path if dir_path.endswith("/") else dir_path + "/"
 
 def prepare_tmp_dir(tmp_dir_path):
     # Figure out where temp files will be stored and create directory, if needed.
     if tmp_dir_path:
         makedirs(tmp_dir_path, exist_ok=True)
-        tmp_dir_path = tmp_dir_path
+        tmp_dir_path = fix_dir_path_ending(tmp_dir_path)
+        use_checkpoints = True
     else:
         tmp_dir_path = mkdtemp()
+        tmp_dir_path = fix_dir_path_ending(tmp_dir_path)# + f"f4_{uuid4()}/"
+        use_checkpoints = False
 
-    unique_id = uuid4()
-    tmp_dir_path = fix_dir_path_ending(tmp_dir_path) + f"f4_{unique_id}/"
-    makedirs(tmp_dir_path, exist_ok=True)
-
-    return tmp_dir_path
+    return tmp_dir_path, use_checkpoints
 
 def remove_tmp_dir(tmp_dir_path, verbose):
     # Remove the temp directory if it was generated by the code (not the user).
     if tmp_dir_path:
         try:
             rmtree(tmp_dir_path)
             print_message(f"Removed {tmp_dir_path} directory", verbose)
         except:
             print_message(f"Warning: {tmp_dir_path} directory could not be removed", verbose)
             pass
 
+def remove_tmp_file(file_path):
+    if path.exists(file_path):
+        remove(file_path)
+
 def split_list_into_chunks(my_list, max_items_per_chunk):
     cursor = 0
     total_elements = len(my_list)
 
     while cursor < total_elements:
         yield my_list[cursor:(cursor + max_items_per_chunk)]
         cursor += max_items_per_chunk
```

### Comparing `f4-1.0.1/src/f4.egg-info/PKG-INFO` & `f4-1.0.2/src/f4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-1.0.1/test/test.py` & `f4-1.0.2/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,22 +81,24 @@
     print(f"use_memory_mapping: {use_memory_mapping}")
     print("-------------------------------------------------------")
 
     # Clean up data files if they already exist
     for file_path in glob.glob(f"{f4_file_path}*"):
         os.unlink(file_path)
 
-    f4.convert_delimited_file(in_file_path, f4_file_path, compression_type=compression_type, num_parallel=num_parallel, index_columns=index_columns)
+    f4.convert_delimited_file(in_file_path, f4_file_path, compression_type=compression_type, num_parallel=num_parallel, index_columns=index_columns, tmp_dir_path="/tmp/f4_small_tests")
 
     try:
         f4.query("bogus_file_path")
         fail_test("Invalid file path.")
     except:
         pass_test("Invalid file path.")
 
+    print("version:")
+    print(f4.get_version(f4_file_path))
     check_result("Version", "Version number - major", f4.get_version(f4_file_path), "1")
     check_result("Dimensions", "Number of rows", f4.get_num_rows(f4_file_path, use_memory_mapping), 5)
     check_result("Dimensions", "Number of columns", f4.get_num_cols(f4_file_path, use_memory_mapping), 9)
     check_result("Indexes", "Index details", f4.get_indexes(f4_file_path, use_memory_mapping), index_columns)
 
     check_result("Column types", "ID column", f4.get_column_type_from_name(f4_file_path, "ID", use_memory_mapping), "s")
     check_result("Column types", "FloatA column", f4.get_column_type_from_name(f4_file_path, "FloatA", use_memory_mapping), "f")
@@ -869,31 +871,31 @@
             num_lines += 1
 
     print(f"  {elapsed_time:.2f} seconds, {num_lines} lines in output file")
 
 #run_all_small_tests()
 #sys.exit()
 
-for compression_type in [None]:
+#for compression_type in [None]:
 #for compression_type in ["zstd"]:
-#for compression_type in [None, "zstd"]:
+for compression_type in [None, "zstd"]:
 #    num_parallel = 1
-#    num_parallel = 4
-    num_parallel = 16
+    num_parallel = 4
+#    num_parallel = 16
     build_outputs = True
     #build_outputs = False
     verbose = True
     #verbose = False
     check_outputs = True
     #check_outputs = False
     #use_memory_mapping=True
     use_memory_mapping=False
 
     # Medium tests
-#    run_larger_tests(num_parallel=num_parallel, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=build_outputs, compression_type=compression_type, check_outputs=check_outputs, verbose=verbose, tmp_dir_path="/tmp/medium", use_memory_mapping=use_memory_mapping)
+    run_larger_tests(num_parallel=num_parallel, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=build_outputs, compression_type=compression_type, check_outputs=check_outputs, verbose=verbose, tmp_dir_path="/tmp/medium", use_memory_mapping=use_memory_mapping)
 
     # Large tests
 #    run_larger_tests(num_parallel=num_parallel, size="large_tall", extension="", discrete1_index=251, numeric1_index=501, build_outputs=build_outputs, compression_type=compression_type, check_outputs=check_outputs, verbose=verbose, tmp_dir_path="/tmp/large_tall", use_memory_mapping=use_memory_mapping)
 #    run_larger_tests(num_parallel=num_parallel, size="large_wide", extension="", discrete1_index=250001, numeric1_index=500001, build_outputs=build_outputs, compression_type=compression_type, check_outputs=check_outputs, verbose=verbose, tmp_dir_path="/tmp/large_wide", use_memory_mapping=use_memory_mapping)
 #
 #    run_super_tests(num_parallel=num_parallel, size="test_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/test_tall", use_memory_mapping=use_memory_mapping)
 #    run_super_tests(num_parallel=num_parallel, size="test_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/test_wide", use_memory_mapping=use_memory_mapping)
@@ -909,13 +911,13 @@
 
 #    run_super_tests(num_parallel=num_parallel, size="hyper_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/hyper_tall", use_memory_mapping=use_memory_mapping)
 #    run_super_tests(num_parallel=num_parallel, size="hyper_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/hyper_wide", use_memory_mapping=use_memory_mapping)
 
     #Attempt this? https://community.hpe.com/t5/servers-systems-the-right/cray-graph-engine-takes-on-a-trillion-triples/ba-p/7096770
 
 #    f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose, use_memory_mapping=use_memory_mapping)
-    f4.transpose("data/large_tall.f4", "/tmp/large_tall_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose, use_memory_mapping=use_memory_mapping)
+#    f4.transpose("data/large_tall.f4", "/tmp/large_tall_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose, use_memory_mapping=use_memory_mapping)
 
 #    f4.inner_join("data/medium.f4", "data/medium.f4", "ID", "/tmp/medium_joined.f4", num_parallel=num_parallel, verbose=verbose, use_memory_mapping=use_memory_mapping)
 #    f4.inner_join("data/large_tall.f4", "data/large_wide.f4", "ID", "/tmp/large_joined.f4", num_parallel=num_parallel, verbose=verbose, use_memory_mapping=use_memory_mapping)
 
 print("All tests passed!!")
```

