# Comparing `tmp/rdfvr-0.2.0.tar.gz` & `tmp/rdfvr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfvr-0.2.0.tar", last modified: Fri Sep 15 03:34:37 2023, max compression
+gzip compressed data, was "rdfvr-0.3.0.tar", last modified: Wed Dec  6 03:16:02 2023, max compression
```

## Comparing `rdfvr-0.2.0.tar` & `rdfvr-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mengli     (501) staff       (20)        0 2023-09-15 03:34:37.849283 rdfvr-0.2.0/
--rw-r--r--   0 mengli     (501) staff       (20)     4507 2023-09-15 03:34:37.849128 rdfvr-0.2.0/PKG-INFO
--rw-r--r--   0 mengli     (501) staff       (20)     4179 2023-09-12 15:28:57.000000 rdfvr-0.2.0/README.md
-drwxr-xr-x   0 mengli     (501) staff       (20)        0 2023-09-15 03:34:37.848920 rdfvr-0.2.0/rdfvr.egg-info/
--rw-r--r--   0 mengli     (501) staff       (20)     4507 2023-09-15 03:34:37.000000 rdfvr-0.2.0/rdfvr.egg-info/PKG-INFO
--rw-r--r--   0 mengli     (501) staff       (20)      203 2023-09-15 03:34:37.000000 rdfvr-0.2.0/rdfvr.egg-info/SOURCES.txt
--rw-r--r--   0 mengli     (501) staff       (20)        1 2023-09-15 03:34:37.000000 rdfvr-0.2.0/rdfvr.egg-info/dependency_links.txt
--rw-r--r--   0 mengli     (501) staff       (20)       37 2023-09-15 03:34:37.000000 rdfvr-0.2.0/rdfvr.egg-info/entry_points.txt
--rw-r--r--   0 mengli     (501) staff       (20)       93 2023-09-15 03:34:37.000000 rdfvr-0.2.0/rdfvr.egg-info/requires.txt
--rw-r--r--   0 mengli     (501) staff       (20)        6 2023-09-15 03:34:37.000000 rdfvr-0.2.0/rdfvr.egg-info/top_level.txt
--rw-r--r--   0 mengli     (501) staff       (20)    10813 2023-09-12 15:48:53.000000 rdfvr-0.2.0/rdfvr.py
--rw-r--r--   0 mengli     (501) staff       (20)       38 2023-09-15 03:34:37.849341 rdfvr-0.2.0/setup.cfg
--rw-r--r--   0 mengli     (501) staff       (20)      767 2023-09-15 03:34:28.000000 rdfvr-0.2.0/setup.py
+drwxr-xr-x   0 mengli     (501) staff       (20)        0 2023-12-06 03:16:02.741912 rdfvr-0.3.0/
+-rw-r--r--   0 mengli     (501) staff       (20)     4537 2023-12-06 03:16:02.741772 rdfvr-0.3.0/PKG-INFO
+-rw-r--r--   0 mengli     (501) staff       (20)     4209 2023-12-06 03:15:12.000000 rdfvr-0.3.0/README.md
+drwxr-xr-x   0 mengli     (501) staff       (20)        0 2023-12-06 03:16:02.741565 rdfvr-0.3.0/rdfvr.egg-info/
+-rw-r--r--   0 mengli     (501) staff       (20)     4537 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/PKG-INFO
+-rw-r--r--   0 mengli     (501) staff       (20)      203 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/SOURCES.txt
+-rw-r--r--   0 mengli     (501) staff       (20)        1 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/dependency_links.txt
+-rw-r--r--   0 mengli     (501) staff       (20)       37 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/entry_points.txt
+-rw-r--r--   0 mengli     (501) staff       (20)       93 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/requires.txt
+-rw-r--r--   0 mengli     (501) staff       (20)        6 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/top_level.txt
+-rw-r--r--   0 mengli     (501) staff       (20)    10873 2023-12-06 03:15:12.000000 rdfvr-0.3.0/rdfvr.py
+-rw-r--r--   0 mengli     (501) staff       (20)       38 2023-12-06 03:16:02.741960 rdfvr-0.3.0/setup.cfg
+-rw-r--r--   0 mengli     (501) staff       (20)      767 2023-12-06 03:15:55.000000 rdfvr-0.3.0/setup.py
```

### Comparing `rdfvr-0.2.0/PKG-INFO` & `rdfvr-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfvr
-Version: 0.2.0
+Version: 0.3.0
 Summary: RDFVR: RDF Validation Report
 Home-page: https://github.com/meng6/rdfvr
 Author: Meng Li
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -54,15 +54,15 @@
   --mappings MAPPINGS, -m MAPPINGS
                         File of the mappings to shorten the report (str): path of the JSON file, where the key is the original text and the value is the shorter text.
   --output OUTPUT, -o OUTPUT
                         Path(s) of the validation report without extension (list[str] | str ). If no value, then output will be a string. Please use comma (no space) to split
                         multiple file paths (e.g. file1,file2,file3).
   --outputformat OUTPUTFORMAT, -of OUTPUTFORMAT
                         File format(s) of the output, validation report (list[str] | str ). Orders should be consistent with the input of --output. Default format is
-                        txt. Each item can only be one of {txt,png}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
+                        txt. Each item can only be one of {txt,png,svg,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
                         output files have the same format, only need to write once.
 
 ```
 
 ## Python Module Use
 You can call the `validation_report` function of the `rdfvr` module as follows:
 
@@ -73,14 +73,14 @@
 
 Where
 - `file_path` is the file path (string) of a RDF graph
 - `file_format` is the format (string) of the RDF graph file
 - `schema` is the file path (string) of the RDF graph's schema
 - `schema_format` is the format (string) of the schema file
 - `output_path` is the file path (string) of the validation report without extension
-- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `gv`
+- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `svg` or `gv`
 - `mappings` is the mappings (dictionary) to shorten the report
 
 The return value is `None`.
 
-The output will be either a `txt` file, a `png` file, a `gv` file, or a `string` print in Bash.
+The output will be either a `txt` file, a `png` file, a `svg` file, a `gv` file, or a `string` print in Bash.
```

### Comparing `rdfvr-0.2.0/README.md` & `rdfvr-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   --mappings MAPPINGS, -m MAPPINGS
                         File of the mappings to shorten the report (str): path of the JSON file, where the key is the original text and the value is the shorter text.
   --output OUTPUT, -o OUTPUT
                         Path(s) of the validation report without extension (list[str] | str ). If no value, then output will be a string. Please use comma (no space) to split
                         multiple file paths (e.g. file1,file2,file3).
   --outputformat OUTPUTFORMAT, -of OUTPUTFORMAT
                         File format(s) of the output, validation report (list[str] | str ). Orders should be consistent with the input of --output. Default format is
-                        txt. Each item can only be one of {txt,png}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
+                        txt. Each item can only be one of {txt,png,svg,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
                         output files have the same format, only need to write once.
 
 ```
 
 ## Python Module Use
 You can call the `validation_report` function of the `rdfvr` module as follows:
 
@@ -61,14 +61,14 @@
 
 Where
 - `file_path` is the file path (string) of a RDF graph
 - `file_format` is the format (string) of the RDF graph file
 - `schema` is the file path (string) of the RDF graph's schema
 - `schema_format` is the format (string) of the schema file
 - `output_path` is the file path (string) of the validation report without extension
-- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `gv`
+- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `svg` or `gv`
 - `mappings` is the mappings (dictionary) to shorten the report
 
 The return value is `None`.
 
-The output will be either a `txt` file, a `png` file, a `gv` file, or a `string` print in Bash.
+The output will be either a `txt` file, a `png` file, a `svg` file, a `gv` file, or a `string` print in Bash.
```

### Comparing `rdfvr-0.2.0/rdfvr.egg-info/PKG-INFO` & `rdfvr-0.3.0/rdfvr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfvr
-Version: 0.2.0
+Version: 0.3.0
 Summary: RDFVR: RDF Validation Report
 Home-page: https://github.com/meng6/rdfvr
 Author: Meng Li
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -54,15 +54,15 @@
   --mappings MAPPINGS, -m MAPPINGS
                         File of the mappings to shorten the report (str): path of the JSON file, where the key is the original text and the value is the shorter text.
   --output OUTPUT, -o OUTPUT
                         Path(s) of the validation report without extension (list[str] | str ). If no value, then output will be a string. Please use comma (no space) to split
                         multiple file paths (e.g. file1,file2,file3).
   --outputformat OUTPUTFORMAT, -of OUTPUTFORMAT
                         File format(s) of the output, validation report (list[str] | str ). Orders should be consistent with the input of --output. Default format is
-                        txt. Each item can only be one of {txt,png}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
+                        txt. Each item can only be one of {txt,png,svg,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all
                         output files have the same format, only need to write once.
 
 ```
 
 ## Python Module Use
 You can call the `validation_report` function of the `rdfvr` module as follows:
 
@@ -73,14 +73,14 @@
 
 Where
 - `file_path` is the file path (string) of a RDF graph
 - `file_format` is the format (string) of the RDF graph file
 - `schema` is the file path (string) of the RDF graph's schema
 - `schema_format` is the format (string) of the schema file
 - `output_path` is the file path (string) of the validation report without extension
-- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `gv`
+- `output_format` is the format (string) of the validation report, i.e., `txt` or `png` or `svg` or `gv`
 - `mappings` is the mappings (dictionary) to shorten the report
 
 The return value is `None`.
 
-The output will be either a `txt` file, a `png` file, a `gv` file, or a `string` print in Bash.
+The output will be either a `txt` file, a `png` file, a `svg` file, a `gv` file, or a `string` print in Bash.
```

### Comparing `rdfvr-0.2.0/rdfvr.py` & `rdfvr-0.3.0/rdfvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     q = """
         PREFIX : <http://www.w3.org/ns/shacl#>
 
         SELECT ?focus ?msg ?path
         WHERE {
             ?curr_node :focusNode ?focus .
             ?curr_node :resultMessage ?msg .
-            ?curr_node :resultPath ?path.
+            OPTIONAL { ?curr_node :resultPath ?path. }
             OPTIONAL { ?curr_node :detail ?child_node. }
             FILTER (!bound(?child_node))
         }
     """
     rows = []
     for r in results_graph.query(q):
         rows.append(r)
@@ -131,25 +131,24 @@
     # Validate the RDF graph
     results_graph = validate_rdf(rdf_graph, schema_file, data_graph_format=file_format, shacl_graph_format=schema_format)
     # Find the most important errors
     errors = extract_errors(results_graph, mappings)
     # Find the suggested error nodes
     (rdf_graph_processed, errors_with_suggested_nodes) = process_graph(rdf_graph, mappings, errors)
     # Output
-    if output_format not in ["txt", "png", "gv"]:
-        raise ValueError("The output file format can only be one of {txt, png, gv}, but " + str(output_format) + " was given. Please check --outputformat.")
+    if output_format not in ["txt", "png", "svg", "gv"]:
+        raise ValueError("The output file format can only be one of {txt, png, svg, gv}, but " + str(output_format) + " was given. Please check --outputformat.")
 
     if output_path:
         output_path = output_path + "." + output_format
         ensure_dir_exists(output_path)
-    if output_format == "png" or output_format == "gv":
+    if output_format == "png" or output_format == "svg" or output_format == "gv":
         G = visualize_graph_as_dot(rdf_graph_processed, errors_with_suggested_nodes)
-        if output_format == "png":
-            G.layout(prog="dot")
-            G.draw(output_path)
+        if output_format == "png" or output_format == "svg":
+            G.draw(output_path, prog="dot")
         else: # gv
             G.write(output_path)
     else: # txt
         report_text = report_graph_as_txt(errors_with_suggested_nodes)
         if not output_path:
             # If NO --output, print a string
             print(report_text)
@@ -163,15 +162,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("--file", "-f", help="File(s) of the RDF graph(s) to be validated (list[str] | str ): please use comma (no space) to split multiple file paths (e.g. file1,file2,file3).")
     parser.add_argument("--schema", "-s", help="Schema of the RDF graph, i.e., Shapes Constraint Language (SHACL) graph (str): path of the file.")
     parser.add_argument("--fileformat", "-ff", help="File format(s) of the RDF graph(s) to be validated (list[str] | str ). Orders should be consistent with the input of --file. Default format is json-ld. If all input files have the same format, only need to write once.")
     parser.add_argument("--schemaformat", "-sf", default="ttl", choices=["xml", "n3", "turtle", "nt", "pretty-xml", "trix", "trig", "nquads", "json-ld", "hext"], help="File format of the schema (str). Default format is ttl.")
     parser.add_argument("--mappings", "-m", help="File of the mappings to shorten the report (str): path of the JSON file, where the key is the original text and the value is the shorter text.")
     parser.add_argument("--output", "-o", help="Path(s) of the validation report without extension (list[str] | str ). If no value, then output will be a string. Please use comma (no space) to split multiple file paths (e.g. file1,file2,file3).")
-    parser.add_argument("--outputformat", "-of", help="File format(s) of the output, validation report (list[str] | str ).  Orders should be consistent with the input of --output. Default format is txt. Each item can only be one of {txt,png,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all output files have the same format, only need to write once.")
+    parser.add_argument("--outputformat", "-of", help="File format(s) of the output, validation report (list[str] | str ).  Orders should be consistent with the input of --output. Default format is txt. Each item can only be one of {txt,png,svg,gv}. Please use comma (no space) to split multiple formats (e.g. format1,format2,format3). If all output files have the same format, only need to write once.")
     arg_file, arg_schema, arg_fileformat, arg_schemaformat, arg_mappings, arg_outputformat, arg_output = parser.parse_args().file, parser.parse_args().schema, parser.parse_args().fileformat, parser.parse_args().schemaformat, parser.parse_args().mappings, parser.parse_args().outputformat, parser.parse_args().output
 
     if not arg_file:
         parser.error("File(s) of the RDF graph(s) to be validated are missing. Please add: --file.")
     if not arg_schema:
         parser.error("Schema file is missing. Please add: --schema.")
     if arg_mappings:
```

### Comparing `rdfvr-0.2.0/setup.py` & `rdfvr-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="rdfvr",
-    version="0.2.0",
+    version="0.3.0",
     description="RDFVR: RDF Validation Report",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meng6/rdfvr",
     author="Meng Li",
     classifiers=[
         "Programming Language :: Python :: 3.10",
```

