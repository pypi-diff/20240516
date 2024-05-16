# Comparing `tmp/allelefinder-0.4.5.tar.gz` & `tmp/allelefinder-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allelefinder-0.4.5.tar", last modified: Wed May  8 13:38:41 2024, max compression
+gzip compressed data, was "allelefinder-0.4.6.tar", last modified: Wed May 15 16:10:42 2024, max compression
```

## Comparing `allelefinder-0.4.5.tar` & `allelefinder-0.4.6.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:38:41.990432 allelefinder-0.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:38:41.990432 allelefinder-0.4.5/AlleleFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-08 13:38:41.000000 allelefinder-0.4.5/AlleleFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-08 13:38:41.000000 allelefinder-0.4.5/AlleleFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:38:41.000000 allelefinder-0.4.5/AlleleFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 13:38:41.000000 allelefinder-0.4.5/AlleleFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 13:38:41.000000 allelefinder-0.4.5/AlleleFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 13:38:41.000000 allelefinder-0.4.5/AlleleFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-08 13:38:33.000000 allelefinder-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 13:38:33.000000 allelefinder-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-08 13:38:41.990432 allelefinder-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-08 13:38:33.000000 allelefinder-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:38:41.990432 allelefinder-0.4.5/allele_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:38:33.000000 allelefinder-0.4.5/allele_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26749 2024-05-08 13:38:33.000000 allelefinder-0.4.5/allele_tools/allele_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-05-08 13:38:33.000000 allelefinder-0.4.5/allele_tools/allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-05-08 13:38:33.000000 allelefinder-0.4.5/allele_tools/allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)   124250 2024-05-08 13:38:33.000000 allelefinder-0.4.5/allele_tools/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-08 13:38:33.000000 allelefinder-0.4.5/allele_tools/profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    52935 2024-05-08 13:38:33.000000 allelefinder-0.4.5/allele_tools/stec.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 13:38:33.000000 allelefinder-0.4.5/allele_tools/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 13:38:33.000000 allelefinder-0.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:38:41.990432 allelefinder-0.4.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-05-08 13:38:33.000000 allelefinder-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:38:41.990432 allelefinder-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_0_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_1_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_2_allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_3_stec_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_4_stec_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_5_stec_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_6_stec_aa_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_7_stec_allele_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_8_stec_allele_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-08 13:38:33.000000 allelefinder-0.4.5/tests/test_9_stec_allele_translate_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:42.548236 allelefinder-0.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:42.544236 allelefinder-0.4.6/AlleleFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-15 16:10:42.000000 allelefinder-0.4.6/AlleleFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 16:10:42.000000 allelefinder-0.4.6/AlleleFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:10:42.000000 allelefinder-0.4.6/AlleleFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 16:10:42.000000 allelefinder-0.4.6/AlleleFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 16:10:42.000000 allelefinder-0.4.6/AlleleFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 16:10:42.000000 allelefinder-0.4.6/AlleleFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 16:10:34.000000 allelefinder-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 16:10:34.000000 allelefinder-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-15 16:10:42.544236 allelefinder-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-15 16:10:34.000000 allelefinder-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:42.544236 allelefinder-0.4.6/allele_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26749 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/allele_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130687 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/split_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53274 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 16:10:34.000000 allelefinder-0.4.6/allele_tools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 16:10:34.000000 allelefinder-0.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:10:42.548236 allelefinder-0.4.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2402 2024-05-15 16:10:34.000000 allelefinder-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:42.544236 allelefinder-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_0_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_1_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_2_allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_3_stec_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_4_stec_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_5_stec_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_6_stec_aa_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_7_stec_allele_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_8_stec_allele_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_9_stec_allele_translate_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-15 16:10:34.000000 allelefinder-0.4.6/tests/test_split_db.py
```

### Comparing `allelefinder-0.4.5/AlleleFinder.egg-info/PKG-INFO` & `allelefinder-0.4.6/AlleleFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.4.5
+Version: 0.4.6
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.4.5/AlleleFinder.egg-info/SOURCES.txt` & `allelefinder-0.4.6/AlleleFinder.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 AlleleFinder.egg-info/top_level.txt
 allele_tools/__init__.py
 allele_tools/allele_profiler.py
 allele_tools/allele_translate_reduce.py
 allele_tools/allele_updater.py
 allele_tools/methods.py
 allele_tools/profile_reduce.py
+allele_tools/split_db.py
 allele_tools/stec.py
 allele_tools/version.py
 tests/__init__.py
 tests/test_0_profile_reduce.py
 tests/test_1_allele_translate_reduce.py
 tests/test_2_allele_updater.py
 tests/test_3_stec_profile_reduce.py
 tests/test_4_stec_allele_translate_reduce.py
 tests/test_5_stec_allele_find.py
 tests/test_6_stec_aa_allele_find.py
 tests/test_7_stec_allele_split.py
 tests/test_8_stec_allele_concatenate.py
-tests/test_9_stec_allele_translate_find.py
+tests/test_9_stec_allele_translate_find.py
+tests/test_split_db.py
```

### Comparing `allelefinder-0.4.5/LICENSE` & `allelefinder-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/PKG-INFO` & `allelefinder-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.4.5
+Version: 0.4.6
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.4.5/README.md` & `allelefinder-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/allele_tools/allele_profiler.py` & `allelefinder-0.4.6/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/allele_tools/allele_translate_reduce.py` & `allelefinder-0.4.6/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/allele_tools/allele_updater.py` & `allelefinder-0.4.6/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/allele_tools/methods.py` & `allelefinder-0.4.6/allele_tools/methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from argparse import ArgumentParser
 from csv import DictReader
 from glob import glob
 import json
 import logging
 import math
 import os
+from typing import (
+    Tuple,
+    Dict
+)
 
 # Third party inputs
 from olctools.accessoryFunctions.accessoryFunctions import (
     GenObject,
     make_path,
     MetadataObject,
     relative_symlink
@@ -384,15 +388,16 @@
         blast = NcbiblastxCommandline(
                 query=sample.general.bestassemblyfile,
                 db=os.path.splitext(combined_targets)[0],
                 evalue=0.001,
                 num_alignments=100000000,
                 num_threads=cpus,
                 outfmt=outfmt,
-                out=sample.alleles.blast_report
+                out=sample.alleles.blast_report,
+                seg='no'
             )
         blast()
 
 
 def create_gene_names(
         path=os.getcwd(),
         name='genes.txt'):
@@ -786,17 +791,17 @@
         'stx1b': 82,
         'stx1A': 313,
         'Stx1A': 313,
         'stx1a': 313,
         'stx2A': 313,
         'Stx2A': 313,
         'stx2a': 313,
-        'stx2B': 84,
-        'Stx2B': 84,
-        'stx2b': 84,
+        'stx2B': 82,
+        'Stx2B': 82,
+        'stx2b': 82,
     }
     filtered = False
     # Remove stop codons and all sequence following it
     aa_seq = aa_seq.split('*')[0]
     # Evaluate the translated length of the sequence
     filtered, notes = evaluate_translated_length(
         aa_seq=aa_seq,
@@ -1689,26 +1694,30 @@
     :param report_path: Name and absolute path to folder in which reports are
     to be created
     :param profile_file: Name and path of file containing reduced profiles
     :param genes: List of all genes in the analysis
     :param allele_comprehension: Dictionary of contig:full_range: {gene:allele}
     :param molecule: String of the current molecule being processed. Options
     are "aa" and "nt"
+    :param notes: Dictionary of contig: query_range: list of notes
     :return: profile_matches: Dictionary of contig:query_range:seq_type_match
     """
     # If the profile_data dictionary was not populated in the read_profiles
     # methods, there is nothing to match
     if not profile_data:
-        return
+        return None, None, None
     logging.info('Matching new %s profiles against profile file', molecule)
     profile_matches = {}
     # Extract all the profiles from the profile file (as a frozen string)
     frozen_profiles = freeze_profiles(
         profile_data=profile_data
     )
+    # Create a dictionary to store the contig: query range: novel status
+    novel = {}
+
     # Iterate over all the contigs with hits
     for contig, query_dict in frozen_allele_comprehension.items():
         # Iterate over the query ranges with hits on the current contig
         for query_range, frozen_allele_dict in query_dict.items():
             try:
                 # Extract the samples that match this profile
                 seq_type_match = frozen_profiles[frozen_allele_dict]
@@ -1716,14 +1725,15 @@
                 if contig not in profile_matches:
                     profile_matches[contig] = {}
                 if query_range not in profile_matches[contig]:
                     profile_matches[contig][query_range] = seq_type_match
             # The profile will not necessarily match any of the profiles
             # found in the analysis
             except KeyError:
+                # Initialise the dictionary
                 if contig not in profile_matches:
                     profile_matches[contig] = {}
                 # Update the profile file with this novel profile
                 profile_matches[contig][query_range] = update_profiles(
                     profile_file=profile_file,
                     report_path=report_path,
                     genes=genes,
@@ -1732,15 +1742,72 @@
                 )
                 # Update the profile_data dictionary with the new sequence type
                 profile_data[profile_matches[contig][query_range]] = \
                     allele_comprehension[contig][query_range]
                 frozen_profiles = freeze_profiles(
                     profile_data=profile_data
                 )
-    return profile_matches, frozen_profiles
+                # Create a dictionary to store the contig: query range: novel
+                if contig not in novel:
+                    novel[contig] = {}
+                if query_range not in novel[contig]:
+                    novel[contig][query_range] = True
+    return profile_matches, frozen_profiles, novel
+
+
+def update_notes(
+        aa_novel: Dict,
+        aa_profile_matches: Dict,
+        notes: Dict,
+        nt_novel: Dict,
+        nt_profile_matches: dict) -> Tuple[Dict, bool]:
+    """
+    Update the notes with the links between the nucleotide and amino acid
+    profiles
+    """
+    # If there are no nucleotide profile matches, return the notes as is
+    if nt_profile_matches is None:
+        return notes, True
+    # Iterate over the nucleotide profile matches
+    for contig, query_dict in nt_profile_matches.items():
+        # Iterate over the query dictionary
+        for query_range, nt_seq_match in query_dict.items():
+            # Get the corresponding amino acid sequence match
+            aa_seq_match = aa_profile_matches[contig][query_range]
+            # If the contig is not already in the notes, add it
+            if contig not in notes:
+                notes[contig] = {}
+            # If the query range is not already in the notes for this contig,
+            # add it
+            if query_range not in notes[contig]:
+                notes[contig][query_range] = []
+            # Initialize the note string
+            note_str = str()
+            # If there are novel nucleotide sequences, add a note about them
+            if nt_novel is not None:
+                try:
+                    if nt_novel[contig][query_range]:
+                        note_str += 'Novel '
+                except KeyError:
+                    pass
+            # Add a note about the nucleotide sequence type
+            note_str += f'nt seq_type {nt_seq_match} links to '
+            # If there are novel amino acid sequences, add a note about them
+            if aa_novel is not None:
+                try:
+                    if aa_novel[contig][query_range]:
+                        note_str += 'novel '
+                except KeyError:
+                    pass
+            # Add a note about the amino acid sequence type
+            note_str += f'aa seq_type {aa_seq_match}'
+            # Add the note to the notes for this contig and query range
+            notes[contig][query_range].append(note_str)
+    # Return the updated notes
+    return notes, False
 
 
 def freeze_profiles(profile_data: dict):
     """
     Freeze profiles, so that the frozen {gene:allele} dictionary can be used
     as the key and the corresponding sequence
     type as the value
@@ -1752,18 +1819,14 @@
     # Initialise a dictionary to store the frozen profiles information
     frozen_profiles = {}
     # Iterate over all the sequence type: {gene name: allele ID} pairs in
     # the dictionary
     for seq_type, allele_comprehension in profile_data.items():
         if allele_comprehension is None:
             continue
-        # # Convert the gene allele dictionary to lower case
-        # lower_comprehension = {}
-        # for gene, allele in allele_comprehension.items():
-        #     lower_comprehension[gene.lower()] = allele
         # Freeze the allele comprehension
         frozen_allele_comprehension = json.dumps(
             allele_comprehension,
             sort_keys=True
         )
         # Populate the dictionary with frozen_allele_comprehension: seq_type
         frozen_profiles[frozen_allele_comprehension] = seq_type
@@ -1963,15 +2026,16 @@
         nt_alleles: dict,
         aa_profile_matches: dict,
         aa_alleles: dict,
         report_file: str,
         gene_names: list,
         aa_profile_path: str,
         notes: list,
-        molecule='nt'):
+        molecule='nt',
+        note_update=True):
     """
     Create a STEC-specific report including the allele matches for each gene
     and sequence type for both nucleotide and amino acid sequence information
     :param runmetadata: MetadataObject with list of GenObjects for each query
     :param nt_profile_matches: Dictionary of contig:query_range:nucleotide
     seq_type_match
     :param nt_alleles: Dictionary of nucleotide contig:full_range:nucleotide
@@ -1983,14 +2047,16 @@
     :param report_file: String of the name and path of the report file
     :param gene_names: List of all gene names in the analysis
     :param aa_profile_path: String of the absolute path of the folder in which
     the amino acid profile file is located
     :param notes: List of notes on the alleles
     :param molecule: String of the current molecule being processed. Default
     is "nt"
+    :param note_update: Boolean of whether the notes file needs to be updated
+    with the nt and aa profile linking information. Default is True
     """
     logging.info('Creating report')
     # Set the appropriate order for the genes in the report
     gene_order = {
         'stx1': ['stx1A', 'stx1B'],
         'stx2': ['stx2A', 'stx2B']
     }
@@ -2029,130 +2095,205 @@
         f'Sample\tnt_{ordered_nt[0]}\tnt_{ordered_nt[1]}\t' \
         f'nt_seq_type\taa_{ordered_aa[0]}\taa_{ordered_aa[1]}\t' \
         f'aa_seq_type\tnotes\n'
     # Create a string to store the query information
     data = str()
     # Iterate over the samples
     for sample in runmetadata.samples:
-        # Iterate over all the contigs that had hits
-        for contig, range_dict in nt_profile_matches.items():
-            # Iterate over the ranges: nucleotide profiles that had hits on
-            # this contig
-            for query_range, nt_profile in range_dict.items():
-                # Update the data string with the sample name
-                data += f'{sample.name}\t'
-                # Extract the corresponding amino acid profile from
-                # aa_profile_matches
-                aa_profile = aa_profile_matches[contig][query_range]
-                # Extract the allele dictionaries ({gene name: allele ID})
-                # using the contig and query range
-                nt_allele_dict = nt_alleles[contig][query_range]
-                aa_allele_dict = aa_alleles[contig][query_range]
-                # Iterate over the genes in the analysis to extract their
-                # corresponding nucleotide alleles
-                for gene in ordered_nt:
-                    # Update the string with the nucleotide allele ID
-                    data += f'{nt_allele_dict[gene]}\t'
-                # Update the string with the nucleotide sequence type
-                data += f'{nt_profile}\t'
-                # Iterate over the genes in the analysis to extract their
-                # corresponding amino acid alleles
-                for gene in ordered_aa:
-                    # Update the string with the amino acid allele ID
-                    try:
-                        data += f'{aa_allele_dict[gene]}\t'
-                    except KeyError:
-                        # Allow gene names rather than protein names
-                        gene_name = gene[0].lower() + gene[1:]
-                        data += f'{aa_allele_dict[gene_name]}\t'
-                # Update the string with the amino acid sequence type
-                data += f'{aa_profile}\t'
-                # Create a list to store sample:contig:query_range-specific
-                # notes
-                note_list = []
-                # Determine if there are already notes for this contig in the
-                # notes dictionary
-                if contig in notes:
-                    # Determine if there are already notes for this contig:
-                    # range in the notes dictionary
-                    if query_range in notes[contig]:
-                        # Update the profile linking file. Use notes in the
-                        # notes dictionary
-                        note_list = update_profile_link_file(
-                            nt_seq_type=nt_profile,
-                            aa_seq_type=aa_profile,
-                            aa_profile_path=aa_profile_path,
-                            note=notes[contig][query_range]
-                        )
-                    # If there are no notes for the contig:range, create notes
-                    # from scratch
+        if nt_profile_matches is not None:
+            # Iterate over all the contigs that had hits
+            for contig, range_dict in nt_profile_matches.items():
+                # Iterate over the ranges: nucleotide profiles that had hits on
+                # this contig
+                for query_range, nt_profile in range_dict.items():
+                    # Update the data string with the sample name
+                    data += f'{sample.name}\t'
+                    # Extract the corresponding amino acid profile from
+                    # aa_profile_matches
+                    aa_profile = aa_profile_matches[contig][query_range]
+                    # Extract the allele dictionaries ({gene name: allele ID})
+                    # using the contig and query range
+                    nt_allele_dict = nt_alleles[contig][query_range]
+                    aa_allele_dict = aa_alleles[contig][query_range]
+                    # Iterate over the genes in the analysis to extract their
+                    # corresponding nucleotide alleles
+                    for gene in ordered_nt:
+                        # Update the string with the nucleotide allele ID
+                        data += f'{nt_allele_dict[gene]}\t'
+                    # Update the string with the nucleotide sequence type
+                    data += f'{nt_profile}\t'
+                    # Iterate over the genes in the analysis to extract their
+                    # corresponding amino acid alleles
+                    for gene in ordered_aa:
+                        # Update the string with the amino acid allele ID
+                        try:
+                            data += f'{aa_allele_dict[gene]}\t'
+                        except KeyError:
+                            # Allow gene names rather than protein names
+                            gene_name = gene[0].lower() + gene[1:]
+                            data += f'{aa_allele_dict[gene_name]}\t'
+                    # Update the string with the amino acid sequence type
+                    data += f'{aa_profile}\t'
+                    # Create a list to store sample:contig:query_range-specific
+                    # notes
+                    note_list = []
+                    # Determine if there are already notes for this contig in
+                    # the notes dictionary
+                    if contig in notes:
+                        # Determine if there are already notes for this contig:
+                        # range in the notes dictionary
+                        if query_range in notes[contig]:
+                            # Update the profile linking file. Use notes in the
+                            # notes dictionary
+                            note_list = update_profile_link_file(
+                                nt_seq_type=nt_profile,
+                                aa_seq_type=aa_profile,
+                                aa_profile_path=aa_profile_path,
+                                note=notes[contig][query_range],
+                                note_update=note_update
+                            )
+                        # If there are no notes for the contig:range, create
+                        # notes from scratch
+                        else:
+                            # Update the profile linking file. Use notes in the
+                            # notes_list list
+                            note_list = update_profile_link_file(
+                                nt_seq_type=nt_profile,
+                                aa_seq_type=aa_profile,
+                                aa_profile_path=aa_profile_path,
+                                note=note_list,
+                                note_update=note_update
+                            )
+                    # If there are no notes for the contig, create notes from
+                    # scratch
                     else:
                         # Update the profile linking file. Use notes in the
                         # notes_list list
                         note_list = update_profile_link_file(
                             nt_seq_type=nt_profile,
                             aa_seq_type=aa_profile,
                             aa_profile_path=aa_profile_path,
-                            note=note_list
+                            note=note_list,
+                            note_update=note_update
+                        )
+                    # Get the list of notes into a string
+                    note_str = str()
+                    # If the notes were updated, use the note_list
+                    if note_list:
+                        # Join all the notes from the list with semicolons
+                        note_str = join_notes(
+                            note_list=note_list,
+                            note_str=note_str
                         )
-                # If there are no notes for the contig, create notes from
-                # scratch
-                else:
-                    # Update the profile linking file. Use notes in the
-                    # notes_list list
-                    note_list = update_profile_link_file(
-                        nt_seq_type=nt_profile,
-                        aa_seq_type=aa_profile,
-                        aa_profile_path=aa_profile_path,
-                        note=note_list
-                    )
-                # Join all the notes from the list with semicolons
-                note_str = str()
-                for note in note_list:
-                    if isinstance(note, str):
-                        if note_str:
-                            note_str += f'; {note}'
-                        else:
-                            note_str += note
                     else:
-                        note_str = '; '.join(note)
-                # Update the data string with the notes
-                data += f'{note_str}'
-                # Add a newline to the data string
-                data += '\n'
+                        try:
+                            note_list = notes[contig][query_range]
+                        except KeyError:
+                            note_list = []
+                        if contig in notes:
+                            # Determine if there are already notes for this
+                            # contig: range in the notes dictionary
+                            if query_range in notes[contig]:
+                                note_str = join_notes(
+                                    note_list=note_list,
+                                    note_str=note_str
+                                )
+                    # Update the data string with the notes
+                    data += f'{note_str}'
+                    # Add a newline to the data string
+                    data += '\n'
         # If there were no hits for the sample, add negative values to the
         # data string
         if not data:
-            data = f'{sample.name}\t0\t0\t1\t0\t0\t1\n'
+            # If there are no notes, add a negative result
+            if not notes:
+                data = f'{sample.name}\t0\t0\t1\t0\t0\t1\n'
+            else:
+                # If there are notes, create a string to hold them
+                note_str = str()
+                # Iterate over the notes dictionary
+                for contig, query_dict in notes.items():
+                    # Iterate over the query dictionary
+                    for query_range, note_list in query_dict.items():
+                        # Only proceed if there is a note list
+                        if not note_list:
+                            continue
+                        # Join all the notes in the list with a semicolon
+                        flattened_notes = '; '.join(note_list)
+                        # If there are already notes in the string, add a
+                        # semicolon and a space
+                        if note_str:
+                            note_str += '; '
+                        # Add the contig, query range, and notes to the string
+                        note_str += \
+                            f'{contig}: location {query_range}: ' \
+                            f'notes: {flattened_notes}'
+                # Add the negative result and notes to the data
+                data = f'{sample.name}\t0\t0\t1\t0\t0\t1\t{note_str}\n'
     # If the report file does not already exist, write the header and data
     # strings
     if not os.path.isfile(report_file):
         with open(report_file, 'w', encoding='utf-8') as report:
             report.write(header)
             report.write(data)
     # If the report already exists, write only the data string
     else:
         with open(report_file, 'a+', encoding='utf-8') as report:
             report.write(data)
 
 
+def join_notes(
+        note_list,
+        note_str) -> str:
+    """
+    Joins a list of notes into a single string.
+
+    Parameters:
+    note_list (list): A list of notes. Each note is either a string or a list
+    of strings.
+    note_str (str): An initial string to which the notes will be appended.
+
+    Returns:
+    str: The notes joined into a single string, separated by semicolons.
+    """
+    # Iterate over the list of notes
+    for note in note_list:
+        # If the note is a string
+        if isinstance(note, str):
+            # If there are already notes in the string, add a semicolon and
+            # a space
+            if note_str:
+                note_str += f'; {note}'
+            else:
+                # If there are no notes in the string yet, just add the note
+                note_str += note
+        else:
+            # If the note is a list of strings, join them with semicolons
+            note_str = '; '.join(note)
+    # Return the joined notes
+    return note_str
+
+
 def update_profile_link_file(
         nt_seq_type: str,
         aa_seq_type: str,
         note: list,
-        aa_profile_path: str):
+        aa_profile_path: str,
+        note_update=True):
     """
     Update the file linking amino acid sequence type to the (multiple)
     corresponding nucleotide sequence type(s)
     :param nt_seq_type: String of the nucleotide sequence type
     :param aa_seq_type: String of the amino acid sequence type
     :param note: List of notes on the alleles
     :param aa_profile_path: String of the absolute path of the folder in which
     the amino acid profile file is located
     :return: note: Update list of notes
+    :param note_update: Boolean of whether the notes file needs to be updated
+    with the nt and aa profile linking information. Default is True
     """
     # Set the name of the link file
     link_file = os.path.join(aa_profile_path, 'aa_nt_profile_links.tsv')
     # Create a dictionary of nucleotide sequence type matches
     nt_match = {}
     # Initialise a boolean to track whether the amino acid sequence type is
     # already present in the profile link file
@@ -2191,30 +2332,32 @@
     if aa_match:
         # Check if there was a match of the sample's nucleotide sequence type
         if not nt_match:
             # Append the nucleotide sequence type to the string of nucleotide
             # sequence type matches
             links[aa_seq_type] += f';{nt_seq_type}'
             # Update the note
-            note.append(
-                f'Novel nt_seq_type {nt_seq_type} links to aa_seq '
-                f'type {aa_seq_type}'
-            )
+            if note_update:
+                note.append(
+                    f'Novel nt seq_type {nt_seq_type} links to aa_seq '
+                    f'type {aa_seq_type}'
+                )
     # If no match, this is a novel amino acid sequence type
     else:
         # Update the link dictionary novel amino acid sequence type: novel
         # nucleotide sequence type
         links[aa_seq_type] = nt_seq_type
         # Add the novel sequence type to the list
         records.append(aa_seq_type)
         # Update the notes
-        note.append(
-            f'Novel nt_seq_type {nt_seq_type}, and '
-            f'novel aa_seq_type {aa_seq_type}'
-        )
+        if note_update:
+            note.append(
+                f'Novel nt seq_type {nt_seq_type}, and '
+                f'novel aa seq_type {aa_seq_type}'
+            )
     # Overwrite the profile link file with the updated links
     with open(link_file, 'w', encoding='utf-8') as profile_link:
         for record in records:
             profile_link.write(f'{record}\t{links[record]}\n')
     return note
 
 
@@ -2316,18 +2459,18 @@
             # Add the contig key to the dictionary as required
             if contig not in processed_range_dict:
                 processed_range_dict[contig] = set()
             # Check the processed range dictionary to see if the current range
             # is present
             if processed_range_dict[contig]:
                 for previous_range in processed_range_dict[contig]:
-                    # Allow a small overlap of five bases in case the range of
+                    # Allow a small overlap of 3 bases in case the range of
                     # one query is slightly different
-                    overlap = query_range[1] + 5 >= previous_range[0] and \
-                              previous_range[1] + 5 >= query_range[0]
+                    overlap = query_range[1] + 3 >= previous_range[0] and \
+                              previous_range[1] + 3 >= query_range[0]
                     # If the range is already present in the dictionary,
                     # update the tracking boolean
                     if overlap:
                         processed = True
             # Add the range to the set if it is empty
             else:
                 processed_range_dict[contig].add(query_range_tuple)
@@ -2341,14 +2484,16 @@
                 sample.alleles.blastlist.append(target_id)
                 # Extract the allele number from the subject name e.g.
                 # Stx1A_1|315aa yields Stx1A_1
                 aa_allele = target_id.split('|')[0]
                 # Update the processed boolean to indicate that this region
                 # has been processed
                 processed = True
+                # Update the set to include the range
+                processed_range_dict[contig].add(query_range_tuple)
             # If the match is imperfect, but greater than the cutoff
             elif cutoff < percent_id < 100 and not processed and not filtered:
                 # Determine which gene is being processed by finding the match
                 # of the genes against the allele
                 gene = [
                     gene for gene in gene_names if gene.lower() in
                     target_id.lower()
@@ -2534,27 +2679,25 @@
 
 def translated_update_nucleotide(
         runmetadata: MetadataObject,
         nt_allele_path: str,
         report_path: str,
         notes: dict,
         gene_names: list,
-        filtered: bool,
         overlap_range: int = 50):
     """
     Search nucleotide allele databases to determine whether the corresponding
     allele already exists
     :param runmetadata: MetadataObject with list of GenObjects for each query
     :param nt_allele_path: Name and absolute path to folder containing
     nucleotide alleles
     :param report_path: String of the absolute path to the folder into which
     reports are to be written
     :param notes: List of sample-specific notes
     :param gene_names: List of all gene names in the analysis
-    :param filtered: Boolean of whether the sample fails quality/length checks
     :param overlap_range: Integer of the number of base pairs that must
     overlap for two alleles to be considered
     :return: runmetadata: Updated MetadataObject
     :return: notes: Updated list of sample-specific notes
     """
     # Iterate through all the samples
     colocation_dict = {}
```

### Comparing `allelefinder-0.4.5/allele_tools/profile_reduce.py` & `allelefinder-0.4.6/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/allele_tools/stec.py` & `allelefinder-0.4.6/allele_tools/stec.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     pathfinder,
     profile_allele_check,
     query_prep,
     report_aa_alleles,
     setup_arguments,
     split_alleles,
     translated_update_nucleotide,
+    update_notes,
     write_concatenated_sequences
 )
 
 __author__ = 'adamkoziol'
 
 
 class STEC:
@@ -133,25 +134,25 @@
                 )
             # Freeze the amino acid allele comprehension
             aa_frozen_allele_comprehension = \
                 create_frozen_allele_comprehension(
                     allele_comprehension=aa_allele_comprehension
                 )
             # Find nucleotide profile matches
-            nt_profile_matches, nt_frozen_profiles = match_profile(
+            nt_profile_matches, _, _ = match_profile(
                 profile_data=nt_profile_data,
                 frozen_allele_comprehension=nt_frozen_allele_comprehension,
                 report_path=self.report_path,
                 profile_file=self.nt_profile_file,
                 genes=gene_names,
                 allele_comprehension=nt_allele_comprehension,
                 molecule='nt'
             )
             # Find amino acid profile matches
-            aa_profile_matches, aa_frozen_profiles = match_profile(
+            aa_profile_matches, _, _ = match_profile(
                 profile_data=aa_profile_data,
                 frozen_allele_comprehension=aa_frozen_allele_comprehension,
                 report_path=self.report_path,
                 profile_file=self.aa_profile_file,
                 genes=gene_names,
                 allele_comprehension=aa_allele_comprehension,
                 molecule='aa'
@@ -326,15 +327,15 @@
                 runmetadata=sample,
                 fieldnames=self.fieldnames,
                 extended_fieldnames=self.extended_fieldnames,
                 records=records,
                 cutoff=95
             )
             # Parse the amino acid BLAST results
-            sample, filtered, notes = parse_aa_blast(
+            sample, _, notes = parse_aa_blast(
                 runmetadata=sample,
                 extended_fieldnames=self.extended_fieldnames,
                 fieldnames=self.fieldnames,
                 gene_names=gene_names,
                 notes=notes,
                 aa_allele_path=self.aa_allele_path,
                 report_path=self.report_path,
@@ -343,15 +344,14 @@
             # Update the nucleotide database as required
             sample, notes = translated_update_nucleotide(
                 runmetadata=sample,
                 nt_allele_path=self.nt_allele_path,
                 report_path=self.report_path,
                 notes=notes,
                 gene_names=self.gene_names,
-                filtered=filtered
             )
             # Create nucleotide allele comprehensions from the
             # BLAST outputs
             nt_allele_comprehension = create_nt_allele_comprehension(
                 runmetadata=sample,
                 gene_names=gene_names,
                 translated=True
@@ -369,45 +369,54 @@
                 )
             # Freeze the amino acid allele comprehension
             aa_frozen_allele_comprehension = \
                 create_frozen_allele_comprehension(
                     allele_comprehension=aa_allele_comprehension
                 )
             # Find nucleotide profile matches
-            nt_profile_matches, _ = match_profile(
+            nt_profile_matches, _, nt_novel = match_profile(
                 profile_data=nt_profile_data,
                 frozen_allele_comprehension=nt_frozen_allele_comprehension,
                 report_path=self.report_path,
                 profile_file=self.nt_profile_file,
                 genes=gene_names,
                 allele_comprehension=nt_allele_comprehension,
                 molecule='nt'
             )
             # Find amino acid profile matches
-            aa_profile_matches, _ = match_profile(
+            aa_profile_matches, _, aa_novel = match_profile(
                 profile_data=aa_profile_data,
                 frozen_allele_comprehension=aa_frozen_allele_comprehension,
                 report_path=self.report_path,
                 profile_file=self.aa_profile_file,
                 genes=gene_names,
                 allele_comprehension=aa_allele_comprehension,
                 molecule='aa'
             )
+            # Update the notes with the profile information
+            notes, note_update = update_notes(
+                aa_novel=aa_novel,
+                aa_profile_matches=aa_profile_matches,
+                notes=notes,
+                nt_novel=nt_novel,
+                nt_profile_matches=nt_profile_matches
+            )
             # Create the STEC-specific report
             create_stec_report(
                 runmetadata=sample,
                 nt_profile_matches=nt_profile_matches,
                 nt_alleles=nt_allele_comprehension,
                 aa_profile_matches=aa_profile_matches,
                 aa_alleles=aa_allele_comprehension,
                 report_file=self.report_file,
                 gene_names=gene_names,
                 aa_profile_path=self.aa_profile_path,
                 notes=notes,
-                molecule='aa'
+                molecule='aa',
+                note_update=note_update
             )
 
     def __init__(
             self,
             allele_path: str,
             aa_allele_path: str,
             profile_file: str,
@@ -853,17 +862,17 @@
         'stx1b': 82,
         'stx1A': 313,
         'Stx1A': 313,
         'stx1a': 313,
         'stx2A': 313,
         'Stx2A': 313,
         'stx2a': 313,
-        'stx2B': 84,
-        'Stx2B': 84,
-        'stx2b': 84,
+        'stx2B': 82,
+        'Stx2B': 82,
+        'stx2b': 82,
     }
     allele_translate_reduce = Translate(
         path=args.allele_path,
         profile=args.profile_file,
         report_path=args.report_path,
         translated_path=args.translated_path,
         length_dict=length_dict,
```

### Comparing `allelefinder-0.4.5/setup.py` & `allelefinder-0.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,24 @@
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
     scripts=[
         os.path.join('allele_tools', 'allele_updater.py'),
         os.path.join('allele_tools', 'allele_translate_reduce.py'),
         os.path.join('allele_tools', 'profile_reduce.py'),
-        os.path.join('allele_tools', 'stec.py')
+        os.path.join('allele_tools', 'stec.py'),
+        os.path.join('allele_tools', 'split_db.py'),
     ],
     entry_points={
         'console_scripts': [
             'allele_updater=allele_tools.allele_updater:cli',
             'allele_translate_reduce=allele_tools.allele_translate_reduce:cli',
             'profile_reduce=allele_tools.profile_reduce:cli',
-            'stec=allele_tools.stec:cli'
+            'stec=allele_tools.stec:cli',
+            'split_db=allele_tools.split_db:cli'
         ]
     },
     install_requires=requirements,
     # Classifiers categorize the project for users.
     classifiers=[
         # Specifies the intended audience of the project
         'Intended Audience :: Science/Research',
```

### Comparing `allelefinder-0.4.5/tests/test_0_profile_reduce.py` & `allelefinder-0.4.6/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/tests/test_1_allele_translate_reduce.py` & `allelefinder-0.4.6/tests/test_1_allele_translate_reduce.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             )
 
             # Define length dictionary for testing
             self.length_dict = {
                 'stx1B': 82,
                 'stx1A': 313,
                 'stx2A': 313,
-                'stx2B': 84
+                'stx2B': 82
             }
 
             # Define a fake path for testing
             self.fake_path = os.path.join('~', 'completely_fake_path')
 
     return Variables()
```

### Comparing `allelefinder-0.4.5/tests/test_2_allele_updater.py` & `allelefinder-0.4.6/tests/test_2_allele_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             )
 
             # Define a dictionary for the expected length of each allele
             self.length_dict = {
                 'stx1B': 82,
                 'stx1A': 313,
                 'stx2A': 313,
-                'stx2B': 84
+                'stx2B': 82
             }
 
             # Define a fake path for testing
             self.fake_path = os.path.join('~', 'completely_fake_path')
 
     return Variables()
```

### Comparing `allelefinder-0.4.5/tests/test_3_stec_profile_reduce.py` & `allelefinder-0.4.6/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/tests/test_4_stec_allele_translate_reduce.py` & `allelefinder-0.4.6/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/tests/test_5_stec_allele_find.py` & `allelefinder-0.4.6/tests/test_5_stec_allele_find.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             )
 
             # Define length dictionary for testing
             self.length_dict = {
                 'stx1B': 82,
                 'stx1A': 313,
                 'stx2A': 313,
-                'stx2B': 84
+                'stx2B': 82
             }
 
             # Define a fake path for testing
             self.fake_path = os.path.join('~', 'completely_fake_path')
 
     return Variables()
 
@@ -188,24 +188,22 @@
     """
     # Read the contents of the allele report file
     variables.report_contents = open(
         variables.allele_report,
         'r',
         encoding='utf-8'
     ).readlines()
-
     # Check the contents of the allele report file
     assert variables.report_contents[1] == \
-        '2013-SEQ-0039\t6\t9\t241\t868\t137\t259156\tNovel nt_seq_type ' \
-        '241, and novel aa_seq_type 259156\n'
+        '2013-SEQ-0039\t6\t9\t241\t868\t137\t259156\tNovel nt seq_type ' \
+        '241, and novel aa seq_type 259156\n'
     assert variables.report_contents[16] == \
-        '2017-SEQ-0617	0	2	116	0		N/A	stx2B amino acid ' \
-        'sequence does not start with M; ' \
-        'stx2B amino acid sequence was 13 amino acid residues. ' \
-        'Minimum allowed length is 84 amino acid residues\n'
+        '2017-SEQ-0617\t0\t2\t116\t0\t\tN/A\tstx2B amino acid sequence does ' \
+        'not start with M; stx2B amino acid sequence was 13 amino acid ' \
+        'residues. Minimum allowed length is 82 amino acid residues\n'
 
 
 def test_clean(variables):
     """
     Test the clean up of the outputs.
 
     :param variables: An instance of the Variables class.
```

### Comparing `allelefinder-0.4.5/tests/test_6_stec_aa_allele_find.py` & `allelefinder-0.4.6/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/tests/test_7_stec_allele_split.py` & `allelefinder-0.4.6/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/tests/test_8_stec_allele_concatenate.py` & `allelefinder-0.4.6/tests/test_8_stec_allele_concatenate.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.5/tests/test_9_stec_allele_translate_find.py` & `allelefinder-0.4.6/tests/test_9_stec_allele_translate_find.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             # Get the path to the report file
             self.report_file = os.path.join(self.report_path, 'profiles.tsv')
             # Define the length dictionary
             self.length_dict = {
                 'stx1B': 82,
                 'stx1A': 313,
                 'stx2A': 313,
-                'stx2B': 84
+                'stx2B': 82
             }
             # Define a fake path for testing
             self.fake_path = os.path.join('~', 'completely_fake_path')
 
     return Variables()
 
 
@@ -185,19 +185,26 @@
     """
     # Open the report file and read its contents
     variables.report_contents = open(
         variables.allele_report,
         'r',
         encoding='utf-8'
     ).readlines()
+    print('\n')
+    for line in variables.report_contents:
+        print(line.rstrip())
+    print('\n')
     # Check that the contents of the report are as expected
     assert variables.report_contents[1] == \
-        '2013-SEQ-0039\t875\t137\t259156\t6\t2\t68\tNovel nt_seq_type ' \
-        '259156 links to aa_seq type 68\n'
-    assert variables.report_contents[10] == '2017-SEQ-0617\t0\t0\t1\t0\t0\t1\n'
+        '2013-SEQ-0039\t875\t137\t259156\t6\t2\t68\tNovel nt seq_type ' \
+        '259156 links to aa seq_type 68\n'
+    assert variables.report_contents[16] == \
+        '2017-SEQ-0617\t0\t0\t1\t0\t0\t1\tContig_91_205.85: location ' \
+        '(2, 262): notes: stx2B amino acid sequence does not start with M; ' \
+        'Amino acid allele Filtered_Stx2B_137|87aa is novel\n'
 
 
 def test_clean(variables):
     """
     Test the clean_outputs function.
 
     :param variables: The test variables.
```

