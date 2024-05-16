# Comparing `tmp/rdfvr-0.3.0.tar.gz` & `tmp/rdfvr-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfvr-0.3.0.tar", last modified: Wed Dec  6 03:16:02 2023, max compression
+gzip compressed data, was "rdfvr-0.3.1.tar", last modified: Thu May 16 19:50:05 2024, max compression
```

## Comparing `rdfvr-0.3.0.tar` & `rdfvr-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mengli     (501) staff       (20)        0 2023-12-06 03:16:02.741912 rdfvr-0.3.0/
--rw-r--r--   0 mengli     (501) staff       (20)     4537 2023-12-06 03:16:02.741772 rdfvr-0.3.0/PKG-INFO
--rw-r--r--   0 mengli     (501) staff       (20)     4209 2023-12-06 03:15:12.000000 rdfvr-0.3.0/README.md
-drwxr-xr-x   0 mengli     (501) staff       (20)        0 2023-12-06 03:16:02.741565 rdfvr-0.3.0/rdfvr.egg-info/
--rw-r--r--   0 mengli     (501) staff       (20)     4537 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/PKG-INFO
--rw-r--r--   0 mengli     (501) staff       (20)      203 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/SOURCES.txt
--rw-r--r--   0 mengli     (501) staff       (20)        1 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/dependency_links.txt
--rw-r--r--   0 mengli     (501) staff       (20)       37 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/entry_points.txt
--rw-r--r--   0 mengli     (501) staff       (20)       93 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/requires.txt
--rw-r--r--   0 mengli     (501) staff       (20)        6 2023-12-06 03:16:02.000000 rdfvr-0.3.0/rdfvr.egg-info/top_level.txt
--rw-r--r--   0 mengli     (501) staff       (20)    10873 2023-12-06 03:15:12.000000 rdfvr-0.3.0/rdfvr.py
--rw-r--r--   0 mengli     (501) staff       (20)       38 2023-12-06 03:16:02.741960 rdfvr-0.3.0/setup.cfg
--rw-r--r--   0 mengli     (501) staff       (20)      767 2023-12-06 03:15:55.000000 rdfvr-0.3.0/setup.py
+drwxr-xr-x   0 mengli     (501) staff       (20)        0 2024-05-16 19:50:05.824919 rdfvr-0.3.1/
+-rw-r--r--   0 mengli     (501) staff       (20)     4537 2024-05-16 19:50:05.824795 rdfvr-0.3.1/PKG-INFO
+-rw-r--r--   0 mengli     (501) staff       (20)     4209 2023-12-06 03:15:12.000000 rdfvr-0.3.1/README.md
+drwxr-xr-x   0 mengli     (501) staff       (20)        0 2024-05-16 19:50:05.824622 rdfvr-0.3.1/rdfvr.egg-info/
+-rw-r--r--   0 mengli     (501) staff       (20)     4537 2024-05-16 19:50:05.000000 rdfvr-0.3.1/rdfvr.egg-info/PKG-INFO
+-rw-r--r--   0 mengli     (501) staff       (20)      203 2024-05-16 19:50:05.000000 rdfvr-0.3.1/rdfvr.egg-info/SOURCES.txt
+-rw-r--r--   0 mengli     (501) staff       (20)        1 2024-05-16 19:50:05.000000 rdfvr-0.3.1/rdfvr.egg-info/dependency_links.txt
+-rw-r--r--   0 mengli     (501) staff       (20)       37 2024-05-16 19:50:05.000000 rdfvr-0.3.1/rdfvr.egg-info/entry_points.txt
+-rw-r--r--   0 mengli     (501) staff       (20)       93 2024-05-16 19:50:05.000000 rdfvr-0.3.1/rdfvr.egg-info/requires.txt
+-rw-r--r--   0 mengli     (501) staff       (20)        6 2024-05-16 19:50:05.000000 rdfvr-0.3.1/rdfvr.egg-info/top_level.txt
+-rw-r--r--   0 mengli     (501) staff       (20)    10575 2024-05-16 19:46:28.000000 rdfvr-0.3.1/rdfvr.py
+-rw-r--r--   0 mengli     (501) staff       (20)       38 2024-05-16 19:50:05.824957 rdfvr-0.3.1/setup.cfg
+-rw-r--r--   0 mengli     (501) staff       (20)      767 2024-05-16 19:45:40.000000 rdfvr-0.3.1/setup.py
```

### Comparing `rdfvr-0.3.0/PKG-INFO` & `rdfvr-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfvr
-Version: 0.3.0
+Version: 0.3.1
 Summary: RDFVR: RDF Validation Report
 Home-page: https://github.com/meng6/rdfvr
 Author: Meng Li
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rdfvr-0.3.0/README.md` & `rdfvr-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rdfvr-0.3.0/rdfvr.egg-info/PKG-INFO` & `rdfvr-0.3.1/rdfvr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfvr
-Version: 0.3.0
+Version: 0.3.1
 Summary: RDFVR: RDF Validation Report
 Home-page: https://github.com/meng6/rdfvr
 Author: Meng Li
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rdfvr-0.3.0/rdfvr.py` & `rdfvr-0.3.1/rdfvr.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,103 +56,104 @@
     :param results_graph: a RDF Graph object showing all errors
     :return errors: a Pandas data frame with node, msg, and path columns
     """
 
     q = """
         PREFIX : <http://www.w3.org/ns/shacl#>
 
-        SELECT ?focus ?msg ?path
+        SELECT ?focus ?msg ?target
         WHERE {
             ?curr_node :focusNode ?focus .
             ?curr_node :resultMessage ?msg .
-            OPTIONAL { ?curr_node :resultPath ?path. }
+            OPTIONAL { ?curr_node :value ?target}
             OPTIONAL { ?curr_node :detail ?child_node. }
             FILTER (!bound(?child_node))
         }
     """
     rows = []
     for r in results_graph.query(q):
         rows.append(r)
-    errors = pd.DataFrame(rows, columns=["node", "msg", "path"]).replace(mappings, regex=True).drop_duplicates()
+    errors = pd.DataFrame(rows, columns=["node", "msg", "target"]).replace(mappings, regex=True).drop_duplicates()
+    errors["target"] = errors["target"].fillna(errors["node"])
     return errors
 
-def process_graph(rdf_graph, mappings, errors):
+def graph(rdf_graph, mappings):
     """
-    This function is to process a RDF Graph object:
+    This function is to convert a RDF Graph object to a Pandas data frame:
         (1) make the node name shorter
-        (2) export as a Pandas data frame
-        (3) add suggested nodes to be updated to the errors data frame
+        (2) export as a Pandas data frame with source, label, and target columns
     :param rdf_graph: a RDF Graph object
     :param mappings: a dictionary used to make the node name shorter
-    :param errors: a Pandas data frame with node, msg, and path columns
     :return rdf_graph_processed: a Pandas data frame
-    :return errors_with_suggested_nodes: a Pandas data frame with node, msg, and target columns, where target column denotes suggested nodes to be updated
     """
     # Query the imported triples in rdf_graph
     q = """
             SELECT ?s ?p ?o
             WHERE {
                 ?s ?p ?o
             }
             ORDER BY ?s ?p ?o
         """
     rows = []
     for r in rdf_graph.query(q):
         rows.append(r)
     rdf_graph_processed = pd.DataFrame(rows, columns=["source", "label", "target"]).replace(mappings, regex=True)
-    errors_with_suggested_nodes = errors.merge(rdf_graph_processed, how="left", left_on=["node", "path"], right_on=["source", "label"])[["node", "msg", "target"]]
-    return rdf_graph_processed, errors_with_suggested_nodes
+    return rdf_graph_processed
 
-def visualize_graph_as_dot(rdf_graph_processed, errors_with_suggested_nodes):
+def visualize_graph_as_dot(rdf_graph_processed, errors):
     # Create a directed graph
     G = pgv.AGraph(directed=True)
     # Add nodes and edges
     for _, row in rdf_graph_processed.iterrows():
         G.add_node(row["source"], shape="box", style="filled, rounded", fillcolor="#b3e2cd")
         G.add_node(row["target"], shape="box", style="filled, rounded", fillcolor="#b3e2cd")
         G.add_edge(row["source"], row["target"], label=row["label"])
-    for _, row in errors_with_suggested_nodes[["node", "msg"]].drop_duplicates().iterrows():
+    for _, row in errors[["node", "msg"]].drop_duplicates().iterrows():
         G.add_node(row["node"], shape="box", style="filled, rounded", fillcolor="#fdccac")
         G.add_node(row["msg"], shape="box", style="filled, rounded, dashed", fillcolor="#fdccac")
         G.add_edge(row["node"], row["msg"], label="ErrorMsg", style="dashed")
     # Suggested nodes to be updated
-    for suggested_node in errors_with_suggested_nodes["target"].dropna().unique():
+    for suggested_node in errors["target"].dropna().unique():
         G.add_node(suggested_node, shape="box", style="filled, rounded", fillcolor="#cbd5e8")
     return G
 
-def report_graph_as_txt(errors_with_suggested_nodes):
+def report_graph_as_txt(errors):
     report_text = ""
-    for _, row in errors_with_suggested_nodes.groupby(["node", "msg"])["target"].agg(list).reset_index().iterrows():
-        report_text = report_text + "Node: {node} \nError Message: {msg}\nSuggested Node(s) to be Updated: {suggested_node}\n\n".format(node=row["node"], msg=row["msg"], suggested_node=str(row["target"]))
+    errors = errors.groupby(["node", "msg"])["target"].agg(list).reset_index()
+    errors["target"] = errors["target"].apply(lambda x: ", ".join(x))
+    for target, group in errors.groupby("target"):
+        report_text = report_text + "**************************************************\nSuggested Node(s) to be Updated: {target}\n**************************************************\n".format(target=target)
+        for _, row in group.iterrows():
+            report_text = report_text + "Node: {node} \nError Message: {msg}\n\n".format(node=row["node"], msg=row["msg"])
     return report_text
 
 def validation_report(file_path, file_format, schema_file, schema_format, output_path, output_format, mappings):
     # Load a file with a given format as a RDF Graph object supported by RDFLib
     rdf_graph = load_file(file_path, graph_format=file_format)
     # Validate the RDF graph
     results_graph = validate_rdf(rdf_graph, schema_file, data_graph_format=file_format, shacl_graph_format=schema_format)
     # Find the most important errors
     errors = extract_errors(results_graph, mappings)
-    # Find the suggested error nodes
-    (rdf_graph_processed, errors_with_suggested_nodes) = process_graph(rdf_graph, mappings, errors)
     # Output
     if output_format not in ["txt", "png", "svg", "gv"]:
         raise ValueError("The output file format can only be one of {txt, png, svg, gv}, but " + str(output_format) + " was given. Please check --outputformat.")
 
     if output_path:
         output_path = output_path + "." + output_format
         ensure_dir_exists(output_path)
     if output_format == "png" or output_format == "svg" or output_format == "gv":
-        G = visualize_graph_as_dot(rdf_graph_processed, errors_with_suggested_nodes)
+        # Find the suggested error nodes
+        rdf_graph_processed = graph(rdf_graph, mappings)
+        G = visualize_graph_as_dot(rdf_graph_processed, errors)
         if output_format == "png" or output_format == "svg":
             G.draw(output_path, prog="dot")
         else: # gv
             G.write(output_path)
     else: # txt
-        report_text = report_graph_as_txt(errors_with_suggested_nodes)
+        report_text = report_graph_as_txt(errors)
         if not output_path:
             # If NO --output, print a string
             print(report_text)
         else:
             with open(output_path, mode="w", encoding="utf-8") as fout:
                 fout.write(report_text)
     return
```

### Comparing `rdfvr-0.3.0/setup.py` & `rdfvr-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="rdfvr",
-    version="0.3.0",
+    version="0.3.1",
     description="RDFVR: RDF Validation Report",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meng6/rdfvr",
     author="Meng Li",
     classifiers=[
         "Programming Language :: Python :: 3.10",
```

