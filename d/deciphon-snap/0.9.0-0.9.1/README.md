# Comparing `tmp/deciphon_snap-0.9.0.tar.gz` & `tmp/deciphon_snap-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.9.0.tar", max compression
+gzip compressed data, was "deciphon_snap-0.9.1.tar", max compression
```

## Comparing `deciphon_snap-0.9.0.tar` & `deciphon_snap-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1063 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/LICENSE
--rw-r--r--   0        0        0     2453 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/README.md
--rw-r--r--   0        0        0      351 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/amino.py
--rw-r--r--   0        0        0     1025 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/fasta.py
--rw-r--r--   0        0        0     1351 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/gff.py
--rw-r--r--   0        0        0     2899 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/hit.py
--rw-r--r--   0        0        0     2294 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/hmmer.py
--rw-r--r--   0        0        0     4939 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/match.py
--rw-r--r--   0        0        0       72 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/path_like.py
--rw-r--r--   0        0        0     4072 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/prod.py
--rw-r--r--   0        0        0      705 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/query_interval.py
--rw-r--r--   0        0        0      418 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      570 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     3201 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      187 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/stringify.py
--rw-r--r--   0        0        0     6640 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/deciphon_snap/view.py
--rw-r--r--   0        0        0      604 2024-02-16 14:46:41.430211 deciphon_snap-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 deciphon_snap-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2453 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/README.md
+-rw-r--r--   0        0        0      351 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/amino.py
+-rw-r--r--   0        0        0     1025 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/fasta.py
+-rw-r--r--   0        0        0     1351 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/gff.py
+-rw-r--r--   0        0        0     2899 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/hit.py
+-rw-r--r--   0        0        0     2294 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/hmmer.py
+-rw-r--r--   0        0        0     4939 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/match.py
+-rw-r--r--   0        0        0       72 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0     4072 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      705 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/query_interval.py
+-rw-r--r--   0        0        0      418 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      570 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     3242 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      187 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0     6640 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/deciphon_snap/view.py
+-rw-r--r--   0        0        0      604 2024-02-19 12:22:27.210271 deciphon_snap-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 deciphon_snap-0.9.1/PKG-INFO
```

### Comparing `deciphon_snap-0.9.0/LICENSE` & `deciphon_snap-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/README.md` & `deciphon_snap-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/fasta.py` & `deciphon_snap-0.9.1/deciphon_snap/fasta.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/gff.py` & `deciphon_snap-0.9.1/deciphon_snap/gff.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/hit.py` & `deciphon_snap-0.9.1/deciphon_snap/hit.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/hmmer.py` & `deciphon_snap-0.9.1/deciphon_snap/hmmer.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/match.py` & `deciphon_snap-0.9.1/deciphon_snap/match.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/prod.py` & `deciphon_snap-0.9.1/deciphon_snap/prod.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/query_interval.py` & `deciphon_snap-0.9.1/deciphon_snap/query_interval.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/shorten.py` & `deciphon_snap-0.9.1/deciphon_snap/shorten.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/deciphon_snap/snap_file.py` & `deciphon_snap-0.9.1/deciphon_snap/snap_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,28 +31,29 @@
 
         with fs.open(prod_file, "rb") as file:
             prods: List[Prod] = []
             rows = [stringify(x) for x in file]
             fieldnames = csv_fieldnames(rows[0])
             for idx, row in enumerate((csv_parse(fieldnames, r) for r in rows[1:])):
                 seq_id = int(row["sequence"])
+                window = int(row["window"])
                 profile = str(row["profile"])
-                with fs.open(f"{hmmer_dir}/{seq_id}/{profile}.h3r", "rb") as f2:
+                with fs.open(f"{hmmer_dir}/{seq_id}/{window}/{profile}.h3r", "rb") as f2:
                     h3r = H3Result(raw=read_h3result(fileno=f2.fileno()))
                 window_start = int(row["window_start"])
                 window_stop = int(row["window_stop"])
                 hit_start = int(row["hit_start"])
                 hit_stop = int(row["hit_stop"])
                 window_interval = PyInterval(start=window_start, stop=window_stop)
                 hit_interval = PyInterval(start=hit_start, stop=hit_stop)
                 prods.append(
                     Prod(
                         id=idx,
                         seq_id=seq_id,
-                        window=int(row["window"]),
+                        window=window,
                         window_interval=window_interval,
                         hit_interval=hit_interval,
                         profile=profile,
                         abc=row["abc"],
                         lrt=float(row["lrt"]),
                         evalue=float(row["evalue"]),
                         match_list=LazyMatchList(raw=str(row["match"])),
```

### Comparing `deciphon_snap-0.9.0/deciphon_snap/view.py` & `deciphon_snap-0.9.1/deciphon_snap/view.py`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.9.0/pyproject.toml` & `deciphon_snap-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphon-snap"
-version = "0.9.0"
+version = "0.9.1"
 description = "Reader for Deciphon snap files."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphon_snap" }]
 
 [tool.poetry.dependencies]
```

### Comparing `deciphon_snap-0.9.0/PKG-INFO` & `deciphon_snap-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.9.0
+Version: 0.9.1
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

