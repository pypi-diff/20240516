# Comparing `tmp/semantic-field-definition-generator-1.4.0.tar.gz` & `tmp/semantic-field-definition-generator-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic-field-definition-generator-1.4.0.tar", last modified: Thu Nov 30 16:07:13 2023, max compression
+gzip compressed data, was "semantic-field-definition-generator-1.4.1.tar", last modified: Fri Dec  1 15:39:49 2023, max compression
```

## Comparing `semantic-field-definition-generator-1.4.0.tar` & `semantic-field-definition-generator-1.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-11-30 16:07:13.331930 semantic-field-definition-generator-1.4.0/
--rw-r--r--   0 casties    (501) staff       (20)     1073 2023-02-20 08:35:34.000000 semantic-field-definition-generator-1.4.0/LICENSE
--rw-r--r--   0 casties    (501) staff       (20)     7804 2023-11-30 16:07:13.331743 semantic-field-definition-generator-1.4.0/PKG-INFO
--rw-r--r--   0 casties    (501) staff       (20)     5934 2023-11-30 16:02:17.000000 semantic-field-definition-generator-1.4.0/README.md
--rw-r--r--   0 casties    (501) staff       (20)     1024 2023-11-30 15:56:55.000000 semantic-field-definition-generator-1.4.0/pyproject.toml
--rw-r--r--   0 casties    (501) staff       (20)       38 2023-11-30 16:07:13.331973 semantic-field-definition-generator-1.4.0/setup.cfg
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-11-30 16:07:13.327704 semantic-field-definition-generator-1.4.0/src/
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-11-30 16:07:13.329072 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/
--rw-r--r--   0 casties    (501) staff       (20)        0 2023-02-25 16:29:53.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/__init__.py
--rw-r--r--   0 casties    (501) staff       (20)     4093 2023-11-30 15:43:28.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/generator.py
--rw-r--r--   0 casties    (501) staff       (20)    11026 2023-11-30 14:00:03.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/parser.py
--rwxr-xr-x   0 casties    (501) staff       (20)     5976 2023-11-30 14:11:44.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/semantic_field_util.py
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-11-30 16:07:13.330406 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/
--rw-r--r--   0 casties    (501) staff       (20)     2799 2023-03-02 18:26:32.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     2853 2023-03-02 18:26:16.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/json.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     5181 2023-11-30 15:43:52.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     4030 2023-11-30 15:39:56.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     5451 2023-11-30 15:43:45.000000 semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-11-30 16:07:13.331503 semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/
--rw-r--r--   0 casties    (501) staff       (20)     7804 2023-11-30 16:07:13.000000 semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/PKG-INFO
--rw-r--r--   0 casties    (501) staff       (20)      955 2023-11-30 16:07:13.000000 semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/SOURCES.txt
--rw-r--r--   0 casties    (501) staff       (20)        1 2023-11-30 16:07:13.000000 semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/dependency_links.txt
--rw-r--r--   0 casties    (501) staff       (20)       98 2023-11-30 16:07:13.000000 semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/entry_points.txt
--rw-r--r--   0 casties    (501) staff       (20)       22 2023-11-30 16:07:13.000000 semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/requires.txt
--rw-r--r--   0 casties    (501) staff       (20)       33 2023-11-30 16:07:13.000000 semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/top_level.txt
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-12-01 15:39:49.323357 semantic-field-definition-generator-1.4.1/
+-rw-r--r--   0 casties    (501) staff       (20)     1073 2023-02-20 08:35:34.000000 semantic-field-definition-generator-1.4.1/LICENSE
+-rw-r--r--   0 casties    (501) staff       (20)     7804 2023-12-01 15:39:49.323153 semantic-field-definition-generator-1.4.1/PKG-INFO
+-rw-r--r--   0 casties    (501) staff       (20)     5934 2023-11-30 16:02:17.000000 semantic-field-definition-generator-1.4.1/README.md
+-rw-r--r--   0 casties    (501) staff       (20)     1024 2023-12-01 15:39:32.000000 semantic-field-definition-generator-1.4.1/pyproject.toml
+-rw-r--r--   0 casties    (501) staff       (20)       38 2023-12-01 15:39:49.323402 semantic-field-definition-generator-1.4.1/setup.cfg
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-12-01 15:39:49.319108 semantic-field-definition-generator-1.4.1/src/
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-12-01 15:39:49.320505 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/
+-rw-r--r--   0 casties    (501) staff       (20)        0 2023-02-25 16:29:53.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/__init__.py
+-rw-r--r--   0 casties    (501) staff       (20)     4093 2023-11-30 15:43:28.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/generator.py
+-rw-r--r--   0 casties    (501) staff       (20)    10802 2023-12-01 15:33:44.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/parser.py
+-rwxr-xr-x   0 casties    (501) staff       (20)     6507 2023-12-01 15:39:03.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/semantic_field_util.py
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-12-01 15:39:49.321834 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/
+-rw-r--r--   0 casties    (501) staff       (20)     2799 2023-03-02 18:26:32.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     2853 2023-03-02 18:26:16.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/json.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     5181 2023-11-30 15:43:52.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     4030 2023-11-30 15:39:56.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     5451 2023-11-30 15:43:45.000000 semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-12-01 15:39:49.322911 semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/
+-rw-r--r--   0 casties    (501) staff       (20)     7804 2023-12-01 15:39:49.000000 semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/PKG-INFO
+-rw-r--r--   0 casties    (501) staff       (20)      955 2023-12-01 15:39:49.000000 semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 casties    (501) staff       (20)        1 2023-12-01 15:39:49.000000 semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 casties    (501) staff       (20)       98 2023-12-01 15:39:49.000000 semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/entry_points.txt
+-rw-r--r--   0 casties    (501) staff       (20)       22 2023-12-01 15:39:49.000000 semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/requires.txt
+-rw-r--r--   0 casties    (501) staff       (20)       33 2023-12-01 15:39:49.000000 semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/top_level.txt
```

### Comparing `semantic-field-definition-generator-1.4.0/LICENSE` & `semantic-field-definition-generator-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.4.0/PKG-INFO` & `semantic-field-definition-generator-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-field-definition-generator
-Version: 1.4.0
+Version: 1.4.1
 Summary: A generator for Field Definitions for ResearchSpace and Metaphacts
 Author-email: Robert Casties <casties@mpiwg-berlin.mpg.de>, Florian Kräutli <florian.kraeutli@uzh.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `semantic-field-definition-generator-1.4.0/README.md` & `semantic-field-definition-generator-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.4.0/pyproject.toml` & `semantic-field-definition-generator-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantic-field-definition-generator"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Robert Casties", email="casties@mpiwg-berlin.mpg.de" },
   { name="Florian Kräutli", email="florian.kraeutli@uzh.ch" },
 ]
 description = "A generator for Field Definitions for ResearchSpace and Metaphacts"
 readme = "README.md"
 license = {file = "LICENSE"}
```

### Comparing `semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/generator.py` & `semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/generator.py`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/parser.py` & `semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,14 @@
             ?field a fielddef:Field .
         }
     }
     ORDER BY ?field'''
     logging.debug(f"fields query='{query}'")
     res = store.query(query, initNs=prefixes)
     
-    logging.info(f"found {len(res)} fields (flavor={flavor})")
     for r in res:
         logging.debug(f"field uri={r.field} in graph={r.graph}")
         field_id = str(r.field)
         if field_id_prefix and field_id.startswith(field_id_prefix):
             field_id = field_id[len(field_id_prefix):]
             
         field = read_field(store, r.field, r.graph, field_id, prefixes)
@@ -263,25 +262,23 @@
             field['queries'] = [{k: v} for k, v in queries.items()]
     
     return field
 
 def write_fields_yaml(fields, filename, field_id_prefix=None, splitFields=False):
     """write all fields to YAML file filename."""
     if splitFields:
-        logging.info(f"writing {len(fields)} fields to YAML directory {filename}")
         for field in fields:
             fn = quote_plus(field['id']) + '.yml'
             with open(Path(filename, fn), 'w') as f:
                 data = {'fields': [field]}
                 if field_id_prefix:
                     data['prefix'] = field_id_prefix
                 
                 yaml.dump(data, stream=f)
             
     else:
-        logging.info(f"writing {len(fields)} fields to YAML file {filename}")
         with open(filename, 'w') as f:
             data = {'fields': fields}
             if field_id_prefix:
                 data['prefix'] = field_id_prefix
             
             yaml.dump(data, stream=f)
```

### Comparing `semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/semantic_field_util.py` & `semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/semantic_field_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,28 +66,33 @@
         if args.add_ns_prefix:
             add_ns_prefix = { key: val for key, val in [prefs.split('=') for prefs in args.add_ns_prefix.split(',')]}
         else:
             add_ns_prefix = None
     
         logging.info(f"reading field definitions from YAML file {args.yaml_file}")
         model = generator.loadSourceFromFile(args.yaml_file)
+        logging.info(f"  read {len(model['fields'])} field definitions")
         if args.split_fields:
             # generate split field list of ids and outputs
             outputs = generator.generate(model, flavor, splitFields=True, add_ns_prefix=add_ns_prefix)
             p = Path(args.trig_file)
             if not p.is_dir():
                 sys.exit(f"ERROR: TRIG_FILE {p} must be directory for option split_fields!")
                 
             logging.info(f"writing field definitions to RDF trig files in directory {args.trig_file} in flavor {args.flavor}")
+            cnt = 0
             for field_id, output in outputs:
                 filename = urllib.parse.quote_plus(field_id) + '.trig'
                 with open(p / filename, 'w') as f:
                     logging.debug(f"writing trig file {filename}")
                     f.write(output)
+                    cnt += 1
                 
+            logging.info(f"  wrote {cnt} trig files")
+
         else:
             output = generator.generate(model, flavor, splitFields=False, add_ns_prefix=add_ns_prefix)
             with open(args.trig_file, 'w') as f:
                 logging.info(f"writing field definitions to RDF trig file {args.trig_file} in flavor {args.flavor}")
                 f.write(output)
 
     ##
@@ -98,21 +103,27 @@
             flavor = parser.RESEARCHSPACE
         elif args.flavor == 'MP':
             flavor = parser.METAPHACTS
         else:
             sys.exit(f"ERROR: action 'read' does not support flavor {args.flavor}!")
             
         if args.add_ns_prefix:
+            # create dict from add_ns_prefix string
             add_ns_prefix = { key: val for key, val in [prefs.split('=') for prefs in args.add_ns_prefix.split(',')]}
         else:
             add_ns_prefix = None
     
         if args.sparql_uri:
             store = parser.open_sparql_store(args.sparql_uri, repository=args.sparql_repository, 
                                       auth_user=args.sparql_user, auth_pass=args.sparql_pass)
         elif args.trig_file:
             store = parser.read_trig_store(args.trig_file)
         else:
             sys.exit(f"ERROR: action 'read' requires SPARQL_URI or TRIG_FILE!")
     
         fields = parser.read_fields(store, flavor, field_id_prefix=args.field_prefix, add_ns_prefix=add_ns_prefix)
+        logging.info(f"  found {len(fields)} fields (flavor={args.flavor})")
         parser.write_fields_yaml(fields, args.yaml_file, field_id_prefix=args.field_prefix, splitFields=args.split_fields)
+        if args.split_fields:
+            logging.info(f"  wrote {len(fields)} fields to YAML directory {args.yaml_file}")
+        else:
+            logging.info(f"  wrote {len(fields)} fields to YAML file {args.yaml_file}")
```

### Comparing `semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars` & `semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/json.handlebars` & `semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/json.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars` & `semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars` & `semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.4.0/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars` & `semantic-field-definition-generator-1.4.1/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/PKG-INFO` & `semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-field-definition-generator
-Version: 1.4.0
+Version: 1.4.1
 Summary: A generator for Field Definitions for ResearchSpace and Metaphacts
 Author-email: Robert Casties <casties@mpiwg-berlin.mpg.de>, Florian Kräutli <florian.kraeutli@uzh.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `semantic-field-definition-generator-1.4.0/src/semantic_field_definition_generator.egg-info/SOURCES.txt` & `semantic-field-definition-generator-1.4.1/src/semantic_field_definition_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

