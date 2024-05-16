# Comparing `tmp/ontobio-2.8.8.tar.gz` & `tmp/ontobio-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontobio-2.8.8.tar", last modified: Fri May 19 18:08:01 2023, max compression
+gzip compressed data, was "ontobio-2.8.9.tar", last modified: Thu Aug 24 00:31:46 2023, max compression
```

## Comparing `ontobio-2.8.8.tar` & `ontobio-2.8.9.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.421720 ontobio-2.8.8/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1547 2023-02-15 19:42:46.000000 ontobio-2.8.8/LICENSE
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)       28 2023-02-15 19:42:46.000000 ontobio-2.8.8/MANIFEST.in
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1691 2023-05-19 18:08:01.421720 ontobio-2.8.8/PKG-INFO
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      970 2023-02-15 19:42:46.000000 ontobio-2.8.8/README.rst
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.381720 ontobio-2.8.8/bin/
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)      171 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/clear-cache.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6455 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/materialize.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     7499 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/ogr.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)    20798 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/ontobio-assoc.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     7331 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/ontobio-lexmap.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     9695 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/ontobio-parse-assocs.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1778 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/rdfgen.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)    31600 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/validate.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.381720 ontobio-2.8.8/ontobio/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1697 2023-05-19 18:06:42.000000 ontobio-2.8.8/ontobio/__init__.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.381720 ontobio-2.8.8/ontobio/analysis/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/analysis/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      457 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/analysis/semsim.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6821 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/assoc_factory.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3665 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/assoc_schema.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    17363 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/assocmodel.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2114 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/cgraph.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7379 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/config.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1084 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/config.yaml
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3867 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/ecomap.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/golr/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3013 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/beacon_query.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10470 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_associations.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        1 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_entities.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2174 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_matrix.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    68763 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_query.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1450 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_sim.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4799 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_stats.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/io/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      228 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    40092 2023-05-12 00:17:37.000000 ontobio-2.8.8/ontobio/io/assocparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6271 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/assocwriter.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    18018 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/differ.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    13053 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/entityparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2902 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/entitywriter.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6868 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/gaference.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1544 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/gafgpibridge.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    24503 2023-04-25 22:08:05.000000 ontobio-2.8.8/ontobio/io/gafparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    23204 2023-04-25 22:08:05.000000 ontobio-2.8.8/ontobio/io/gpadparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6903 2023-04-19 18:09:14.000000 ontobio-2.8.8/ontobio/io/hpoaparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12899 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/ontol_renderers.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1633 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/parsereport.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    43181 2023-05-19 18:03:52.000000 ontobio-2.8.8/ontobio/io/qc.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    35539 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/lexmap.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/model/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1527 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/GolrResults.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      972 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/OBOGraph.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    27873 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/association.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3211 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/bbop_graph.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3589 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/biomodel.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5399 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/collections.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/model/mme/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/mme/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1928 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/mme/request.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      607 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/mme/response.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1227 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/nlp.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2252 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/similarity.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/neo/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/neo/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8261 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/neo/scigraph_ontology.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12801 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/obograph_util.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    37123 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/ontol.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6351 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/ontol_factory.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/rdfgen/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12608 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/assoc_rdfgen.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/rdfgen/gocamgen/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     9655 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/collapsed_assoc.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      489 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/errors.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3330 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/filter_rule.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    13135 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/gocam_builder.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    56549 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/gocamgen.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4947 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8070 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/subgraphs.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7567 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/triple_pattern_finder.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6653 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/utils.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8382 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/relations.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/sim/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6273 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/annotation_scorer.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/sim/api/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2397 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/interfaces.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    17404 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/owlsim2.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2163 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/owlsim3.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7262 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/semsearch.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2918 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/mme.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7583 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/phenosim_engine.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1290 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/sim_engine.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2961 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/slimmer.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/sparql/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2261 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/rdf2nx.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1531 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/rdflib_bridge.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4073 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/skos.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12491 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/sparql_go.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    11088 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/sparql_ontol_utils.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8756 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/sparql_ontology.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4673 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/wikidata.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5814 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/wikidata_ontology.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1642 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/tsv_expander.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/util/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      516 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/curie_map.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2826 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/go_utils.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)      736 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/obog2cg.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    18224 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/scigraph_util.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      903 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/user_agent.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/validation/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/validation/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5693 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/validation/metadata.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10167 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/validation/rules.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1322 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/validation/tools.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/vocabulary/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      239 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/categories.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1226 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/relations.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      955 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/similarity.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      823 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/upper.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      310 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/xref_util.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.381720 ontobio-2.8.8/ontobio.egg-info/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1691 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/PKG-INFO
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4357 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/SOURCES.txt
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        1 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/dependency_links.txt
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      471 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/requires.txt
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)       14 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/top_level.txt
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)       80 2023-05-19 18:08:01.421720 ontobio-2.8.8/setup.cfg
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2370 2023-02-15 19:42:46.000000 ontobio-2.8.8/setup.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.421720 ontobio-2.8.8/tests/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      510 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_alt_id.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12770 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_assoc_writer.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3528 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_assocfactory.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3636 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_assocmodel.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      775 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_bgiparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5151 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_collections.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      915 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_config.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      736 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_ecomap.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1478 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_enrich.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1756 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_evidence_table.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      719 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_expand_tsv.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5319 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gaference.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    26453 2023-05-12 00:17:37.000000 ontobio-2.8.8/tests/test_gafparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4929 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_goassociation_model.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5645 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gocamgen.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5578 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_golr_associations.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1536 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_golr_map2slim.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      983 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_golr_query.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2234 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_golr_search.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10349 2023-04-25 22:08:05.000000 ontobio-2.8.8/tests/test_gpad_parser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      761 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gpad_writer.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gpaddiffer.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1043 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gpiparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      963 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gpiwriter.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2199 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_hpoaparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1043 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_lexmap.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    11952 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_lexmap_local.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8184 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_local_json.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1159 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_local_ttl.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1912 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_map2slim.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      695 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_mutable.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1706 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_ontol.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3967 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_owlsim2_int.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4535 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_parse_ids.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      664 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_parse_taxon.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5390 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_phenosim_engine.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    33092 2023-05-19 18:03:52.000000 ontobio-2.8.8/tests/test_qc.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4310 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_rdfgen.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      450 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_relations.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3363 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_remote_scigraph.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5059 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_remote_sparql.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1846 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_semsearch.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      550 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_skos_local.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1281 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_sparql_connection.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3463 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_validation_rules.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1301 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_wd.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1610 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_wd_ontol.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      351 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_write_obo.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.562887 ontobio-2.8.9/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1547 2023-02-15 19:42:46.000000 ontobio-2.8.9/LICENSE
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)       28 2023-02-15 19:42:46.000000 ontobio-2.8.9/MANIFEST.in
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1691 2023-08-24 00:31:46.562887 ontobio-2.8.9/PKG-INFO
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      970 2023-02-15 19:42:46.000000 ontobio-2.8.9/README.rst
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.522887 ontobio-2.8.9/bin/
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)      171 2023-02-15 19:42:46.000000 ontobio-2.8.9/bin/clear-cache.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6455 2023-02-15 19:42:46.000000 ontobio-2.8.9/bin/materialize.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     7499 2023-02-15 19:42:46.000000 ontobio-2.8.9/bin/ogr.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)    20798 2023-02-15 19:42:46.000000 ontobio-2.8.9/bin/ontobio-assoc.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     7331 2023-02-15 19:42:46.000000 ontobio-2.8.9/bin/ontobio-lexmap.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     9695 2023-02-15 19:42:46.000000 ontobio-2.8.9/bin/ontobio-parse-assocs.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1778 2023-02-15 19:42:46.000000 ontobio-2.8.9/bin/rdfgen.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)    31600 2023-02-15 19:42:46.000000 ontobio-2.8.9/bin/validate.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.532887 ontobio-2.8.9/ontobio/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1697 2023-08-23 23:58:01.000000 ontobio-2.8.9/ontobio/__init__.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.532887 ontobio-2.8.9/ontobio/analysis/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/analysis/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      457 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/analysis/semsim.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6821 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/assoc_factory.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3665 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/assoc_schema.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    17363 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/assocmodel.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2114 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/cgraph.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7379 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/config.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1084 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/config.yaml
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3867 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/ecomap.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.532887 ontobio-2.8.9/ontobio/golr/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/golr/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3013 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/golr/beacon_query.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10470 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/golr/golr_associations.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        1 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/golr/golr_entities.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2174 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/golr/golr_matrix.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    68763 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/golr/golr_query.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1450 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/golr/golr_sim.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4799 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/golr/golr_stats.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.532887 ontobio-2.8.9/ontobio/io/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      228 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    40090 2023-08-23 23:58:01.000000 ontobio-2.8.9/ontobio/io/assocparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6271 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/assocwriter.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    18018 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/differ.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    13053 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/entityparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2902 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/entitywriter.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6868 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/gaference.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1544 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/gafgpibridge.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    24503 2023-08-23 00:21:06.000000 ontobio-2.8.9/ontobio/io/gafparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    23204 2023-04-25 22:08:05.000000 ontobio-2.8.9/ontobio/io/gpadparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6903 2023-04-19 18:09:14.000000 ontobio-2.8.9/ontobio/io/hpoaparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12899 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/ontol_renderers.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1633 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/io/parsereport.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    43520 2023-08-23 23:58:01.000000 ontobio-2.8.9/ontobio/io/qc.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    35539 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/lexmap.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.532887 ontobio-2.8.9/ontobio/model/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1527 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/GolrResults.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      972 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/OBOGraph.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    27873 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/association.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3211 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/bbop_graph.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3589 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/biomodel.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5399 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/collections.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/model/mme/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/mme/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1928 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/mme/request.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      607 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/mme/response.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1227 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/nlp.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2252 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/model/similarity.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/neo/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/neo/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8261 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/neo/scigraph_ontology.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12801 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/obograph_util.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    37123 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/ontol.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6351 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/ontol_factory.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/rdfgen/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12608 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/assoc_rdfgen.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/rdfgen/gocamgen/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     9655 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/collapsed_assoc.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      489 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/errors.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3330 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/filter_rule.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    13133 2023-08-23 21:11:10.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/gocam_builder.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    56549 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/gocamgen.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4947 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8070 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/subgraphs.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7567 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/triple_pattern_finder.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6653 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/gocamgen/utils.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8382 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/rdfgen/relations.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/sim/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6273 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/annotation_scorer.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/sim/api/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/api/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2397 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/api/interfaces.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    17404 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/api/owlsim2.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2163 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/api/owlsim3.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7262 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/api/semsearch.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2918 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/mme.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7583 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/phenosim_engine.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1290 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sim/sim_engine.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2961 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/slimmer.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/sparql/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sparql/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2261 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sparql/rdf2nx.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1531 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sparql/rdflib_bridge.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4565 2023-08-23 21:11:10.000000 ontobio-2.8.9/ontobio/sparql/skos.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12491 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sparql/sparql_go.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    11088 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sparql/sparql_ontol_utils.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8756 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sparql/sparql_ontology.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4673 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sparql/wikidata.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5814 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/sparql/wikidata_ontology.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1642 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/tsv_expander.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/util/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/util/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      516 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/util/curie_map.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2826 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/util/go_utils.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)      736 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/util/obog2cg.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    18224 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/util/scigraph_util.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      903 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/util/user_agent.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/validation/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/validation/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5693 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/validation/metadata.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10167 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/validation/rules.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1322 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/validation/tools.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.542887 ontobio-2.8.9/ontobio/vocabulary/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/vocabulary/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      239 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/vocabulary/categories.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1226 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/vocabulary/relations.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      955 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/vocabulary/similarity.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      823 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/vocabulary/upper.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      310 2023-02-15 19:42:46.000000 ontobio-2.8.9/ontobio/xref_util.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.532887 ontobio-2.8.9/ontobio.egg-info/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1691 2023-08-24 00:31:46.000000 ontobio-2.8.9/ontobio.egg-info/PKG-INFO
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4357 2023-08-24 00:31:46.000000 ontobio-2.8.9/ontobio.egg-info/SOURCES.txt
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        1 2023-08-24 00:31:46.000000 ontobio-2.8.9/ontobio.egg-info/dependency_links.txt
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      466 2023-08-24 00:31:46.000000 ontobio-2.8.9/ontobio.egg-info/requires.txt
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)       14 2023-08-24 00:31:46.000000 ontobio-2.8.9/ontobio.egg-info/top_level.txt
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)       80 2023-08-24 00:31:46.562887 ontobio-2.8.9/setup.cfg
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2386 2023-08-23 21:11:10.000000 ontobio-2.8.9/setup.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-08-24 00:31:46.562887 ontobio-2.8.9/tests/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      510 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_alt_id.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12770 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_assoc_writer.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3528 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_assocfactory.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3636 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_assocmodel.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      775 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_bgiparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5151 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_collections.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      915 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_config.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      736 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_ecomap.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1478 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_enrich.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1756 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_evidence_table.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      719 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_expand_tsv.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5319 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_gaference.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    26453 2023-08-23 21:25:52.000000 ontobio-2.8.9/tests/test_gafparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4929 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_goassociation_model.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5645 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_gocamgen.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5578 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_golr_associations.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1536 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_golr_map2slim.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      983 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_golr_query.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2234 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_golr_search.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10349 2023-04-25 22:08:05.000000 ontobio-2.8.9/tests/test_gpad_parser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      761 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_gpad_writer.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_gpaddiffer.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1043 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_gpiparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      963 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_gpiwriter.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2199 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_hpoaparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1043 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_lexmap.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    11952 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_lexmap_local.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8184 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_local_json.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1159 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_local_ttl.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1912 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_map2slim.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      695 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_mutable.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1706 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_ontol.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3967 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_owlsim2_int.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4535 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_parse_ids.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      664 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_parse_taxon.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5390 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_phenosim_engine.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    33397 2023-08-23 23:58:01.000000 ontobio-2.8.9/tests/test_qc.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4310 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_rdfgen.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      450 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_relations.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3363 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_remote_scigraph.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5059 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_remote_sparql.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1846 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_semsearch.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      546 2023-08-23 21:11:10.000000 ontobio-2.8.9/tests/test_skos_local.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1281 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_sparql_connection.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3463 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_validation_rules.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1301 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_wd.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1610 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_wd_ontol.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      351 2023-02-15 19:42:46.000000 ontobio-2.8.9/tests/test_write_obo.py
```

### Comparing `ontobio-2.8.8/LICENSE` & `ontobio-2.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/PKG-INFO` & `ontobio-2.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontobio
-Version: 2.8.8
+Version: 2.8.9
 Summary: Library for working with OBO Library Ontologies and associations
 Home-page: https://github.com/biolink/ontobio
 Author: Chris Mungall
 Author-email: cmungall@gmail.com
 License: BSD
 Keywords: ontology graph obo owl sparql networkx network
 Platform: UNKNOWN
```

### Comparing `ontobio-2.8.8/README.rst` & `ontobio-2.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/bin/materialize.py` & `ontobio-2.8.9/bin/materialize.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/bin/ogr.py` & `ontobio-2.8.9/bin/ogr.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/bin/ontobio-assoc.py` & `ontobio-2.8.9/bin/ontobio-assoc.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/bin/ontobio-lexmap.py` & `ontobio-2.8.9/bin/ontobio-lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/bin/ontobio-parse-assocs.py` & `ontobio-2.8.9/bin/ontobio-parse-assocs.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/bin/rdfgen.py` & `ontobio-2.8.9/bin/rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/bin/validate.py` & `ontobio-2.8.9/bin/validate.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/__init__.py` & `ontobio-2.8.9/ontobio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import absolute_import
 
-__version__ = '2.8.8'
+__version__ = '2.8.9'
 
 
 from .ontol_factory import OntologyFactory
 from .ontol import Ontology, Synonym, TextDefinition
 from .assoc_factory import AssociationSetFactory
 from .io.ontol_renderers import GraphRenderer
```

### Comparing `ontobio-2.8.8/ontobio/assoc_factory.py` & `ontobio-2.8.9/ontobio/assoc_factory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/assoc_schema.py` & `ontobio-2.8.9/ontobio/assoc_schema.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/assocmodel.py` & `ontobio-2.8.9/ontobio/assocmodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/cgraph.py` & `ontobio-2.8.9/ontobio/cgraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/config.py` & `ontobio-2.8.9/ontobio/config.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/config.yaml` & `ontobio-2.8.9/ontobio/config.yaml`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/ecomap.py` & `ontobio-2.8.9/ontobio/ecomap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/golr/beacon_query.py` & `ontobio-2.8.9/ontobio/golr/beacon_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/golr/golr_associations.py` & `ontobio-2.8.9/ontobio/golr/golr_associations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/golr/golr_matrix.py` & `ontobio-2.8.9/ontobio/golr/golr_matrix.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/golr/golr_query.py` & `ontobio-2.8.9/ontobio/golr/golr_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/golr/golr_sim.py` & `ontobio-2.8.9/ontobio/golr/golr_sim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/golr/golr_stats.py` & `ontobio-2.8.9/ontobio/golr/golr_stats.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/assocparser.py` & `ontobio-2.8.9/ontobio/io/assocparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,15 +733,15 @@
                         taxon=line.taxon, rule=20)
                     id = rb[0]
                 else:
                     self.report.error(line.line, Report.OBSOLETE_CLASS_NO_REPLACEMENT, id, msg="Violates GORULE:0000020",
                         taxon=line.taxon, rule=20)
                     id = None
             else:
-                self.report.warning(line.line, Report.OBSOLETE_CLASS, id, msg="Violates GORULE:0000020",
+                self.report.error(line.line, Report.OBSOLETE_CLASS, id, msg="Violates GORULE:0000020",
                     taxon=line.taxon, rule=20)
                 id = None
 
         return id
     
             
     # repair extensions
```

### Comparing `ontobio-2.8.8/ontobio/io/assocwriter.py` & `ontobio-2.8.9/ontobio/io/assocwriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/differ.py` & `ontobio-2.8.9/ontobio/io/differ.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/entityparser.py` & `ontobio-2.8.9/ontobio/io/entityparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/entitywriter.py` & `ontobio-2.8.9/ontobio/io/entitywriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/gaference.py` & `ontobio-2.8.9/ontobio/io/gaference.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/gafgpibridge.py` & `ontobio-2.8.9/ontobio/io/gafgpibridge.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/gafparser.py` & `ontobio-2.8.9/ontobio/io/gafparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/gpadparser.py` & `ontobio-2.8.9/ontobio/io/gpadparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/hpoaparser.py` & `ontobio-2.8.9/ontobio/io/hpoaparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/ontol_renderers.py` & `ontobio-2.8.9/ontobio/io/ontol_renderers.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/parsereport.py` & `ontobio-2.8.9/ontobio/io/parsereport.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/io/qc.py` & `ontobio-2.8.9/ontobio/io/qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,19 +331,24 @@
         elif config.ontology is None:
             return self._result(True)
 
         passes = False
         if self.allowed_dual_species_terms is not None:
             dual = annotation.interacting_taxon is not None
             goterm = str(annotation.object.id)
+            term_in_allowed_dual_species_terms = goterm in self.allowed_dual_species_terms
+            
+            # dual species have to be unique for multi-organism interactions
+            if dual and term_in_allowed_dual_species_terms and annotation.interacting_taxon == annotation.subject.taxon:
+               return self._result(False) 
 
             # We fail if we are a dual taxon and then the term is not in this list
             # This is the same as dual -> goterm in list
             # Implication rewritten is Not P OR Q
-            passes = not dual or (goterm in self.allowed_dual_species_terms)
+            passes = not dual or (term_in_allowed_dual_species_terms) 
 
         return self._result(passes)
 
 
 class GoRule16(GoRule):
 
     def __init__(self):
```

### Comparing `ontobio-2.8.8/ontobio/lexmap.py` & `ontobio-2.8.9/ontobio/lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/GolrResults.py` & `ontobio-2.8.9/ontobio/model/GolrResults.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/OBOGraph.py` & `ontobio-2.8.9/ontobio/model/OBOGraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/association.py` & `ontobio-2.8.9/ontobio/model/association.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/bbop_graph.py` & `ontobio-2.8.9/ontobio/model/bbop_graph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/biomodel.py` & `ontobio-2.8.9/ontobio/model/biomodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/collections.py` & `ontobio-2.8.9/ontobio/model/collections.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/mme/request.py` & `ontobio-2.8.9/ontobio/model/mme/request.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/mme/response.py` & `ontobio-2.8.9/ontobio/model/mme/response.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/nlp.py` & `ontobio-2.8.9/ontobio/model/nlp.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/model/similarity.py` & `ontobio-2.8.9/ontobio/model/similarity.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/neo/scigraph_ontology.py` & `ontobio-2.8.9/ontobio/neo/scigraph_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/obograph_util.py` & `ontobio-2.8.9/ontobio/obograph_util.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/ontol.py` & `ontobio-2.8.9/ontobio/ontol.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/ontol_factory.py` & `ontobio-2.8.9/ontobio/ontol_factory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/assoc_rdfgen.py` & `ontobio-2.8.9/ontobio/rdfgen/assoc_rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/gocamgen/collapsed_assoc.py` & `ontobio-2.8.9/ontobio/rdfgen/gocamgen/collapsed_assoc.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/gocamgen/filter_rule.py` & `ontobio-2.8.9/ontobio/rdfgen/gocamgen/filter_rule.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/gocamgen/gocam_builder.py` & `ontobio-2.8.9/ontobio/rdfgen/gocamgen/gocam_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 # GoCamInputHandler
 
 
 class GoCamBuilder:
     def __init__(self, parser_config: AssocParserConfig, modelstate=None):
         self.config = parser_config
         self.aspector = GoAspector(self.config.ontology)
-        self.store = plugin.get('IOMemory', Store)()
+        self.store = plugin.get('Memory', Store)()
         self.errors = GeneErrorSet()  # Errors by gene ID
         self.gpi_entities = self.parse_gpi(parser_config.gpi_authority_path)
         self.modelstate = modelstate
 
     def translate_to_model(self, gene, assocs: List[GoAssociation]):
         if gene not in self.gpi_entities:
             error_msg = "Gene ID '{}' missing from provided GPI. Skipping model translation.".format(gene)
```

### Comparing `ontobio-2.8.8/ontobio/rdfgen/gocamgen/gocamgen.py` & `ontobio-2.8.9/ontobio/rdfgen/gocamgen/gocamgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py` & `ontobio-2.8.9/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/gocamgen/subgraphs.py` & `ontobio-2.8.9/ontobio/rdfgen/gocamgen/subgraphs.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/gocamgen/triple_pattern_finder.py` & `ontobio-2.8.9/ontobio/rdfgen/gocamgen/triple_pattern_finder.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/gocamgen/utils.py` & `ontobio-2.8.9/ontobio/rdfgen/gocamgen/utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/rdfgen/relations.py` & `ontobio-2.8.9/ontobio/rdfgen/relations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sim/annotation_scorer.py` & `ontobio-2.8.9/ontobio/sim/annotation_scorer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sim/api/interfaces.py` & `ontobio-2.8.9/ontobio/sim/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sim/api/owlsim2.py` & `ontobio-2.8.9/ontobio/sim/api/owlsim2.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sim/api/owlsim3.py` & `ontobio-2.8.9/ontobio/sim/api/owlsim3.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sim/api/semsearch.py` & `ontobio-2.8.9/ontobio/sim/api/semsearch.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sim/mme.py` & `ontobio-2.8.9/ontobio/sim/mme.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sim/phenosim_engine.py` & `ontobio-2.8.9/ontobio/sim/phenosim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sim/sim_engine.py` & `ontobio-2.8.9/ontobio/sim/sim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/slimmer.py` & `ontobio-2.8.9/ontobio/slimmer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sparql/rdf2nx.py` & `ontobio-2.8.9/ontobio/sparql/rdf2nx.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sparql/rdflib_bridge.py` & `ontobio-2.8.9/ontobio/sparql/rdflib_bridge.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sparql/skos.py` & `ontobio-2.8.9/ontobio/sparql/skos.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,39 +3,57 @@
 
 import rdflib
 from rdflib import Namespace
 from rdflib.namespace import RDF
 from rdflib.namespace import SKOS
 from prefixcommons.curie_util import contract_uri
 
-from ontobio.ontol import Ontology, Synonym
+from ontobio.ontol import Ontology, Synonym, TextDefinition
 
 # TODO: make configurable
 GEMET = Namespace('http://www.eionet.europa.eu/gemet/2004/06/gemet-schema.rdf#')
 
 logger = logging.getLogger(__name__)
 
 
+def _preferred_label(rg, concept):
+    """
+    Return a list of (label_prop, label) pairs, where label_prop is either skos:prefLabel or rdfs:label.
+
+    :param: rg: rdflib.Graph object
+    :param: concept: rdflib.URIRef object
+    :param: lang: language code
+
+    """
+
+    labels = list(rg.objects(concept, SKOS.prefLabel))
+    if len(labels) == 0:
+        print("No labels for {}".format(concept))
+
+    else:
+        return [(SKOS.prefLabel, l_) for l_ in labels]
+
+
 class Skos(object):
     """
     SKOS is an RDF data model for representing thesauri and terminologies.
 
     See https://www.w3.org/TR/skos-primer/ for more details
     """
 
     def __init__(self, prefixmap=None, lang='en'):
         self.prefixmap = prefixmap if prefixmap is not None else {}
         self.lang = lang
         self.context = None
 
     def _uri2id(self, uri):
         s = "{:s}".format(str(uri))
-        for prefix,uribase in self.prefixmap.items():
-            if (s.startswith(uribase)):
-                s = s.replace(uribase,prefix+":")
+        for prefix, uribase in self.prefixmap.items():
+            if s.startswith(uribase):
+                s = s.replace(uribase, prefix+":")
                 return s
         curies = contract_uri(uri)
         if len(curies) > 0:
             return curies[0]
         return s
 
     def process_file(self,filename=None, format=None):
@@ -53,16 +71,16 @@
         
     def process_rdfgraph(self, rg, ont=None):
         """
         Transform a skos terminology expressed in an rdf graph into an Ontology object
 
         Arguments
         ---------
-        rg: rdflib.Graph
-            graph object
+        :param: rg: rdflib.Graph object
+        :param: ont: ontobio.ontol.Ontology object
 
         Returns
         -------
         Ontology
         """
         # TODO: ontology metadata
         if ont is None:
@@ -75,22 +93,21 @@
             
         subset_map = {}
         for concept in rg.subjects(RDF.type, SKOS.Concept):
             for s in self._get_schemes(rg, concept):
                 subset_map[self._uri2id(s)] = s
                 
         for concept in sorted(list(rg.subjects(RDF.type, SKOS.Concept))):
-            concept_uri = str(concept)
             id=self._uri2id(concept)
             logger.info("ADDING: {}".format(id))
-            ont.add_node(id, self._get_label(rg,concept))
+            ont.add_node(id, self._get_label(rg, concept))
                     
             for defn in rg.objects(concept, SKOS.definition):
-                if (defn.language == self.lang):
-                    td = TextDefinition(id, escape_value(defn.value))
+                if defn.language == self.lang:
+                    td = TextDefinition(id, defn.value)
                     ont.add_text_definition(td)
                     
             for s in rg.objects(concept, SKOS.broader):
                 ont.add_parent(id, self._uri2id(s))
                 
             for s in rg.objects(concept, SKOS.related):
                 ont.add_parent(id, self._uri2id(s), self._uri2id(SKOS.related))
@@ -108,16 +125,16 @@
         return ont
     
     def _get_schemes(self, rg, concept):
         schemes = set(rg.objects(concept, SKOS.inScheme))
         schemes.update(rg.objects(concept, GEMET.group))
         return schemes
     
-    def _get_label(self, rg,concept):
-        labels = sorted(rg.preferredLabel(concept, lang=self.lang))
-        if len(labels) == 0:
+    def _get_label(self, rg, concept):
+        if _preferred_label(rg, concept) is not None:
+            labels = sorted(_preferred_label(rg, concept))
+        else:
             return None
         if len(labels) > 1:
             logger.warning(">1 label for {} : {}".format(concept, labels))
         return labels[0][1].value
-    
-    
+
```

### Comparing `ontobio-2.8.8/ontobio/sparql/sparql_go.py` & `ontobio-2.8.9/ontobio/sparql/sparql_go.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sparql/sparql_ontol_utils.py` & `ontobio-2.8.9/ontobio/sparql/sparql_ontol_utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sparql/sparql_ontology.py` & `ontobio-2.8.9/ontobio/sparql/sparql_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sparql/wikidata.py` & `ontobio-2.8.9/ontobio/sparql/wikidata.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/sparql/wikidata_ontology.py` & `ontobio-2.8.9/ontobio/sparql/wikidata_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/tsv_expander.py` & `ontobio-2.8.9/ontobio/tsv_expander.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/util/curie_map.py` & `ontobio-2.8.9/ontobio/util/curie_map.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/util/go_utils.py` & `ontobio-2.8.9/ontobio/util/go_utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/util/obog2cg.py` & `ontobio-2.8.9/ontobio/util/obog2cg.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/util/scigraph_util.py` & `ontobio-2.8.9/ontobio/util/scigraph_util.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/util/user_agent.py` & `ontobio-2.8.9/ontobio/util/user_agent.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/validation/metadata.py` & `ontobio-2.8.9/ontobio/validation/metadata.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/validation/rules.py` & `ontobio-2.8.9/ontobio/validation/rules.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/validation/tools.py` & `ontobio-2.8.9/ontobio/validation/tools.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/vocabulary/relations.py` & `ontobio-2.8.9/ontobio/vocabulary/relations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/vocabulary/similarity.py` & `ontobio-2.8.9/ontobio/vocabulary/similarity.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio/vocabulary/upper.py` & `ontobio-2.8.9/ontobio/vocabulary/upper.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/ontobio.egg-info/PKG-INFO` & `ontobio-2.8.9/ontobio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontobio
-Version: 2.8.8
+Version: 2.8.9
 Summary: Library for working with OBO Library Ontologies and associations
 Home-page: https://github.com/biolink/ontobio
 Author: Chris Mungall
 Author-email: cmungall@gmail.com
 License: BSD
 Keywords: ontology graph obo owl sparql networkx network
 Platform: UNKNOWN
```

### Comparing `ontobio-2.8.8/ontobio.egg-info/SOURCES.txt` & `ontobio-2.8.9/ontobio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/setup.py` & `ontobio-2.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import sys
 import re
 import subprocess
 
 import setuptools
 
-if sys.version_info.major < 3:
-    sys.exit("Error: Python 3 is required")
+if sys.version_info.major >= 3.10:
+    sys.exit("Error: Python 3.10 or later is required")
 
 directory = os.path.dirname(os.path.abspath(__file__))
 
 # version
 init_path = os.path.join(directory, 'ontobio', '__init__.py')
 with open(init_path) as read_file:
     text = read_file.read()
```

### Comparing `ontobio-2.8.8/tests/test_assoc_writer.py` & `ontobio-2.8.9/tests/test_assoc_writer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_assocfactory.py` & `ontobio-2.8.9/tests/test_assocfactory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_assocmodel.py` & `ontobio-2.8.9/tests/test_assocmodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_bgiparser.py` & `ontobio-2.8.9/tests/test_bgiparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_collections.py` & `ontobio-2.8.9/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_config.py` & `ontobio-2.8.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_ecomap.py` & `ontobio-2.8.9/tests/test_ecomap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_enrich.py` & `ontobio-2.8.9/tests/test_enrich.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_evidence_table.py` & `ontobio-2.8.9/tests/test_evidence_table.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_expand_tsv.py` & `ontobio-2.8.9/tests/test_expand_tsv.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_gaference.py` & `ontobio-2.8.9/tests/test_gaference.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_gafparser.py` & `ontobio-2.8.9/tests/test_gafparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_goassociation_model.py` & `ontobio-2.8.9/tests/test_goassociation_model.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_gocamgen.py` & `ontobio-2.8.9/tests/test_gocamgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_golr_associations.py` & `ontobio-2.8.9/tests/test_golr_associations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_golr_map2slim.py` & `ontobio-2.8.9/tests/test_golr_map2slim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_golr_query.py` & `ontobio-2.8.9/tests/test_golr_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_golr_search.py` & `ontobio-2.8.9/tests/test_golr_search.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_gpad_parser.py` & `ontobio-2.8.9/tests/test_gpad_parser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_gpad_writer.py` & `ontobio-2.8.9/tests/test_gpad_writer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_gpiparser.py` & `ontobio-2.8.9/tests/test_gpiparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_gpiwriter.py` & `ontobio-2.8.9/tests/test_gpiwriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_hpoaparser.py` & `ontobio-2.8.9/tests/test_hpoaparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_lexmap.py` & `ontobio-2.8.9/tests/test_lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_lexmap_local.py` & `ontobio-2.8.9/tests/test_lexmap_local.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_local_json.py` & `ontobio-2.8.9/tests/test_local_json.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_local_ttl.py` & `ontobio-2.8.9/tests/test_local_ttl.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_map2slim.py` & `ontobio-2.8.9/tests/test_map2slim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_mutable.py` & `ontobio-2.8.9/tests/test_mutable.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_ontol.py` & `ontobio-2.8.9/tests/test_ontol.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_owlsim2_int.py` & `ontobio-2.8.9/tests/test_owlsim2_int.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_parse_ids.py` & `ontobio-2.8.9/tests/test_parse_ids.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_parse_taxon.py` & `ontobio-2.8.9/tests/test_parse_taxon.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_phenosim_engine.py` & `ontobio-2.8.9/tests/test_phenosim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_qc.py` & `ontobio-2.8.9/tests/test_qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,18 +220,23 @@
     assert test_result.result_type == qc.ResultType.WARNING
 
     assoc.object.id = Curie.from_str("GO:0002812")
     test_result = qc.GoRule15().test(assoc, all_rules_config(ontology=ontology))
     assert test_result.result_type == qc.ResultType.PASS
 
     assoc.object.id = Curie.from_str("GO:0044215")
-    assoc.object.id = Curie.from_str("NCBITaxon:123")
+    assoc.object.taxon = Curie.from_str("NCBITaxon:123")
     assoc.interacting_taxon = None # This is the important part, no interacting taxon
     test_result = qc.GoRule15().test(assoc, all_rules_config(ontology=ontology))
     assert test_result.result_type == qc.ResultType.PASS
+    
+    assoc.object.id = Curie.from_str("GO:0044419")
+    assoc.interacting_taxon = Curie.from_str("NCBITaxon:123") # Taxon and interacting taxon are same
+    test_result = qc.GoRule15().test(assoc, all_rules_config(ontology=ontology))
+    assert test_result.result_type == qc.ResultType.WARNING    
 
 def test_go_rule_16():
     # No GO term w/ID
     assoc = make_annotation(evidence="IC", withfrom="BLAH:12345").associations[0]
 
     test_result = qc.GoRule16().test(assoc, all_rules_config())
     assert test_result.result_type == qc.ResultType.WARNING
```

### Comparing `ontobio-2.8.8/tests/test_rdfgen.py` & `ontobio-2.8.9/tests/test_rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_remote_scigraph.py` & `ontobio-2.8.9/tests/test_remote_scigraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_remote_sparql.py` & `ontobio-2.8.9/tests/test_remote_sparql.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_semsearch.py` & `ontobio-2.8.9/tests/test_semsearch.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_skos_local.py` & `ontobio-2.8.9/tests/test_skos_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from ontobio.ontol_factory import OntologyFactory
 from ontobio.sparql.skos import Skos
 from ontobio import GraphRenderer
 import logging
 
+
 def test_skos():
     """
     Load ontology from SKOS
     """
     prefixmap = {'LTER': 'http://vocab.lternet.edu?tema=', 'SKOS': 'http://www.w3.org/2004/02/skos/core#'}
     skos = Skos(prefixmap=prefixmap)
 
-    
     fn = 'tests/resources/skos_example.rdf'
     ont = skos.process_file(fn, format='ttl')
 
     for n in ont.nodes():
         print('{}'.format(n))
 
     w = GraphRenderer.create('obo')
```

### Comparing `ontobio-2.8.8/tests/test_sparql_connection.py` & `ontobio-2.8.9/tests/test_sparql_connection.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_validation_rules.py` & `ontobio-2.8.9/tests/test_validation_rules.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_wd.py` & `ontobio-2.8.9/tests/test_wd.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.8/tests/test_wd_ontol.py` & `ontobio-2.8.9/tests/test_wd_ontol.py`

 * *Files identical despite different names*

