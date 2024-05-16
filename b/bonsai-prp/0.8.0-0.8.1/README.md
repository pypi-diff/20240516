# Comparing `tmp/bonsai_prp-0.8.0.tar.gz` & `tmp/bonsai_prp-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonsai_prp-0.8.0.tar", last modified: Wed May 15 14:08:34 2024, max compression
+gzip compressed data, was "bonsai_prp-0.8.1.tar", last modified: Thu May 16 14:43:54 2024, max compression
```

## Comparing `bonsai_prp-0.8.0.tar` & `bonsai_prp-0.8.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:34.000383 bonsai_prp-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-15 14:08:34.000383 bonsai_prp-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/bonsai_prp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 14:08:33.000000 bonsai_prp-0.8.0/bonsai_prp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.992382 bonsai_prp-0.8.0/prp/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/prp/models/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/phenotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/species.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/models/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/prp/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/prp/parse/phenotype/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/amrfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/mykrobe.py
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/resfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/serotypefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/tbprofiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/phenotype/virulencefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/species.py
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/prp/parse/variant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:08:34.000383 bonsai_prp-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:08:33.996382 bonsai_prp-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-15 14:08:20.000000 bonsai_prp-0.8.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.521755 bonsai_prp-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-16 14:43:54.521755 bonsai_prp-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/bonsai_prp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.513755 bonsai_prp-0.8.1/prp/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/prp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/phenotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/prp/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/prp/parse/phenotype/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/amrfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/mykrobe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/resfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/serotypefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/tbprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/virulencefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:43:54.521755 bonsai_prp-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/tests/test_cli.py
```

### Comparing `bonsai_prp-0.8.0/LICENSE` & `bonsai_prp-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/PKG-INFO` & `bonsai_prp-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.8.0
+Version: 0.8.1
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `bonsai_prp-0.8.0/README.md` & `bonsai_prp-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/bonsai_prp.egg-info/PKG-INFO` & `bonsai_prp-0.8.1/bonsai_prp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.8.0
+Version: 0.8.1
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `bonsai_prp-0.8.0/bonsai_prp.egg-info/SOURCES.txt` & `bonsai_prp-0.8.1/bonsai_prp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/cli.py` & `bonsai_prp-0.8.1/prp/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     parse_resfinder_amr_pred,
     parse_serotypefinder_oh_typing,
     parse_tbprofiler_amr_pred,
     parse_tbprofiler_lineage_results,
     parse_virulencefinder_stx_typing,
     parse_virulencefinder_vir_pred,
 )
+from .parse.species import get_mykrobe_spp_prediction
 from .parse.metadata import get_database_info, get_gb_genome_version, parse_run_info
 from .parse.utils import _get_path, get_db_version, parse_input_dir
 from .parse.variant import annotate_delly_variants
 
 logging.basicConfig(
     level=logging.INFO, format="[%(asctime)s] %(levelname)s in %(module)s: %(message)s"
 )
@@ -225,19 +226,18 @@
         LOG.info("Parse serotypefinder results")
         # OH typing
         res: MethodIndex | None = parse_serotypefinder_oh_typing(serotypefinder)
         if res is not None:
             results["typing_result"].extend(res)
 
     # species id
+    results["species_prediction"] = []
     if kraken:
         LOG.info("Parse kraken results")
-        results["species_prediction"] = parse_kraken_result(kraken)
-    else:
-        results["species_prediction"] = []
+        results["species_prediction"].append(parse_kraken_result(kraken))
 
     # mycobacterium tuberculosis
     # mykrobe
     if mykrobe:
         LOG.info("Parse mykrobe results")
         pred_res = pd.read_csv(mykrobe, quotechar='"')
         pred_res.columns.values[3] = "variants"
@@ -268,14 +268,17 @@
 
         lin_res: MethodIndex | None = parse_mykrobe_lineage_results(
             pred_res, TypingMethod.LINEAGE
         )
         if lin_res is not None:
             results["typing_result"].append(lin_res)
 
+        # parse mykrobe species prediction result
+        results["species_prediction"].append(get_mykrobe_spp_prediction(pred_res))
+
     # tbprofiler
     if tbprofiler:
         LOG.info("Parse tbprofiler results")
         with open(tbprofiler, "r", encoding="utf-8") as tbprofiler_json:
             pred_res = json.load(tbprofiler_json)
             db_info: List[SoupVersion] = []
             db_info = [
```

### Comparing `bonsai_prp-0.8.0/prp/models/metadata.py` & `bonsai_prp-0.8.1/prp/models/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/models/phenotype.py` & `bonsai_prp-0.8.1/prp/models/phenotype.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/models/qc.py` & `bonsai_prp-0.8.1/prp/models/qc.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/models/sample.py` & `bonsai_prp-0.8.1/prp/models/sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pydantic import Field
 
 from .base import RWModel
 from .metadata import RunMetadata
 from .phenotype import ElementType, ElementTypeResult, PredictionSoftware, VariantBase
 from .qc import QcMethodIndex
-from .species import SpeciesPredictionResult
+from .species import SppMethodIndex
 from .typing import (
     TypingMethod,
     TypingResultCgMlst,
     TypingResultGeneAllele,
     TypingResultLineage,
     TypingResultMlst,
     TypingSoftware,
@@ -33,15 +33,15 @@
 
 
 class SampleBase(RWModel):
     """Base datamodel for sample data structure"""
 
     run_metadata: RunMetadata = Field(..., alias="runMetadata")
     qc: List[QcMethodIndex] = Field(...)
-    species_prediction: SpeciesPredictionResult = Field(..., alias="speciesPrediction")
+    species_prediction: List[SppMethodIndex] = Field(..., alias="speciesPrediction")
 
 
 class ReferenceGenome(RWModel):
     """Reference genome."""
 
     name: str
     accession: str
```

### Comparing `bonsai_prp-0.8.0/prp/models/tags.py` & `bonsai_prp-0.8.1/prp/models/tags.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/models/typing.py` & `bonsai_prp-0.8.1/prp/models/typing.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/__init__.py` & `bonsai_prp-0.8.1/prp/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/metadata.py` & `bonsai_prp-0.8.1/prp/parse/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/phenotype/amrfinder.py` & `bonsai_prp-0.8.1/prp/parse/phenotype/amrfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/phenotype/mykrobe.py` & `bonsai_prp-0.8.1/prp/parse/phenotype/mykrobe.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/phenotype/resfinder.py` & `bonsai_prp-0.8.1/prp/parse/phenotype/resfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/phenotype/serotypefinder.py` & `bonsai_prp-0.8.1/prp/parse/phenotype/serotypefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/phenotype/tbprofiler.py` & `bonsai_prp-0.8.1/prp/parse/phenotype/tbprofiler.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/phenotype/virulencefinder.py` & `bonsai_prp-0.8.1/prp/parse/phenotype/virulencefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/qc.py` & `bonsai_prp-0.8.1/prp/parse/qc.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/typing.py` & `bonsai_prp-0.8.1/prp/parse/typing.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/utils.py` & `bonsai_prp-0.8.1/prp/parse/utils.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/prp/parse/variant.py` & `bonsai_prp-0.8.1/prp/parse/variant.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/pyproject.toml` & `bonsai_prp-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.0/tests/test_cli.py` & `bonsai_prp-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

