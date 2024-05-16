# Comparing `tmp/sonus-0.6.2.tar.gz` & `tmp/sonus-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonus-0.6.2.tar", last modified: Tue Feb 21 03:56:01 2023, max compression
+gzip compressed data, was "sonus-0.6.3.tar", last modified: Thu Mar  2 05:08:53 2023, max compression
```

## Comparing `sonus-0.6.2.tar` & `sonus-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 03:56:01.878293 sonus-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-02-21 03:55:52.000000 sonus-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-21 03:55:52.000000 sonus-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-02-21 03:56:01.878293 sonus-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-02-21 03:55:52.000000 sonus-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-21 03:55:52.000000 sonus-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 03:56:01.878293 sonus-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-21 03:55:52.000000 sonus-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 03:56:01.874292 sonus-0.6.2/sonus/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-21 03:55:52.000000 sonus-0.6.2/sonus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-21 03:55:52.000000 sonus-0.6.2/sonus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-02-21 03:55:52.000000 sonus-0.6.2/sonus/chapterizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-02-21 03:55:52.000000 sonus-0.6.2/sonus/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-02-21 03:55:52.000000 sonus-0.6.2/sonus/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 03:56:01.874292 sonus-0.6.2/sonus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-02-21 03:56:01.000000 sonus-0.6.2/sonus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-21 03:56:01.000000 sonus-0.6.2/sonus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 03:56:01.000000 sonus-0.6.2/sonus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-21 03:56:01.000000 sonus-0.6.2/sonus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-21 03:56:01.000000 sonus-0.6.2/sonus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-21 03:56:01.000000 sonus-0.6.2/sonus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:08:53.128912 sonus-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-03-02 05:08:40.000000 sonus-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-02 05:08:40.000000 sonus-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-03-02 05:08:53.128912 sonus-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-02 05:08:40.000000 sonus-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-02 05:08:40.000000 sonus-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 05:08:53.128912 sonus-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-02 05:08:40.000000 sonus-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:08:53.128912 sonus-0.6.3/sonus/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-02 05:08:40.000000 sonus-0.6.3/sonus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-02 05:08:40.000000 sonus-0.6.3/sonus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-03-02 05:08:40.000000 sonus-0.6.3/sonus/chapterizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-03-02 05:08:40.000000 sonus-0.6.3/sonus/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-03-02 05:08:40.000000 sonus-0.6.3/sonus/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:08:53.128912 sonus-0.6.3/sonus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-03-02 05:08:53.000000 sonus-0.6.3/sonus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-02 05:08:53.000000 sonus-0.6.3/sonus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 05:08:53.000000 sonus-0.6.3/sonus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-02 05:08:53.000000 sonus-0.6.3/sonus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-02 05:08:53.000000 sonus-0.6.3/sonus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-02 05:08:53.000000 sonus-0.6.3/sonus.egg-info/top_level.txt
```

### Comparing `sonus-0.6.2/LICENSE` & `sonus-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sonus-0.6.2/PKG-INFO` & `sonus-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonus
-Version: 0.6.2
+Version: 0.6.3
 Summary: Cross-platform OverDrive audiobook client and chapterizer written in Python. 
 Home-page: https://github.com/digitalec/sonus
 Author: digitalec
 License: GPL3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
```

### Comparing `sonus-0.6.2/README.md` & `sonus-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `sonus-0.6.2/setup.py` & `sonus-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `sonus-0.6.2/sonus/chapterizer.py` & `sonus-0.6.3/sonus/chapterizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import xmltodict
 from mutagen.mp3 import MP3
 from mutagen.id3 import ID3
 import ffmpeg
 from pathlib import Path
 
+import sys
+
 logger = logging.getLogger(__name__)
 
 
 def scan_overdrive_metadata(file_list):
     all_markers = []
     for file in file_list:
         file_marker = {'file': file, 'markers': []}
@@ -19,14 +21,16 @@
         xmlstring = str(tag_data['TXXX:OverDrive MediaMarkers'])
         audio_data = xmltodict.parse(xmlstring)
         for k, v in audio_data.items():
             for key, val in v.items():
                 if not isinstance(val, list):
                     val = [val]
                 for marker in val:
+                    # Clean Name (Chapter) and Time
+                    marker['Name'] = clean_file_string(marker['Name'])
                     marker['Time'] = convert_timestamp_to_secs(marker['Time'])
                     file_marker['markers'].append(dict(marker))
         all_markers.append(file_marker)
     return all_markers
 
 
 def convert_timestamp_to_secs(ts):
@@ -108,26 +112,48 @@
             stream = ffmpeg.overwrite_output(stream)
             ffmpeg.run(stream)
         except FileNotFoundError as e:
             if 'ffmpeg' in str(e):
                 print(" --- ERROR! Please make sure ffmpeg is installed")
 
 
+def clean_file_string(file_string):
+    invalid_chars = [
+        ['!', ''],
+        ['?', ''],
+        [':', '-'],
+        ['/', '-'],
+        ['\\', ' '],
+        ['"', ' '],
+        ['<', ' '],
+        ['>', ' '],
+        ['|', ' '],
+        ['*', ' '],
+        ['?', ' ']
+    ]
+    
+    for i in invalid_chars:
+        file_string = file_string.replace(i[0], i[1])
+    
+    return file_string
+
+
 def merge_chapter_parts(file_list, output_dir, generic=False):
     author, title = None, None
     current_chapter = None
     current_track = None
     temp_chapter_file = None
     generic = generic
 
     for i, file in enumerate(file_list):
+
         tag_data = ID3(file)
         if not author:
             author = tag_data.get('TPE1')
-            title = tag_data.get('TALB')
+            title = tag_data.get('TALB').text[0]
             logger.info(f"Processing audiobook \"{title}\" by {author}")
         last_track = False
 
         if current_chapter is None:
             current_chapter = tag_data.get('TIT2').text[0]
             current_track = int(tag_data.get('TRCK').text[0])
             if generic:
@@ -159,35 +185,25 @@
             ffmpeg.run(stream)
         else:
             if not temp_chapter_file:
                 temp_chapter_file = file
 
             author = str(author).split("/")[0]
 
+            author = clean_file_string(author)
+            title = clean_file_string(title)
+
             # Create output dir if it doesn't exist
             output_to = f"{output_dir}/{author}/{title}"
+
             Path(output_to).mkdir(parents=True, exist_ok=True)
             if generic:
                 chapter_filename = f"Chapter {current_track}"
             else:
-                invalid_chars = [
-                    ['!', ''],
-                    ['?', ''],
-                    [':', ' -'],
-                    ['/', ' - '],
-                    ['\\', ' '],
-                    ['"', ' '],
-                    ['<', ' '],
-                    ['>', ' '],
-                    ['|', ' '],
-                    ['*', ' '],
-                    ['?', ' ']
-                ]
-                for i in invalid_chars:
-                    current_chapter = current_chapter.replace(i[0], i[1])
+                current_chapter = clean_file_string(current_chapter)
                 chapter_filename = str(current_track) + " " + current_chapter
             logger.info(f"Saving chapter to {output_to}/{chapter_filename}.mp3")
 
             # Save chapter to output directory
             shutil.copy(temp_chapter_file, f"{output_dir}/{author}/{title}/{chapter_filename}.mp3")
             if not last_track:
                 logger.debug(f"Next track is different, track {next_track}")
```

### Comparing `sonus-0.6.2/sonus/downloader.py` & `sonus-0.6.3/sonus/downloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 import re
 import sys
 import uuid
 import xml.etree.ElementTree as ET
 from concurrent.futures import ThreadPoolExecutor
 
+from .chapterizer import clean_file_string
+
 import requests
 
 from os.path import (abspath, basename, expanduser, getsize, isdir, isfile, sep)
 from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 
@@ -107,41 +109,19 @@
                 logger.debug('Saving as {}'.format(cover_path))
                 fd.write(r.content)
         else:
             logger.debug('Could not download cover. Status code: {}'.format(
                 r.status_code))
 
 
-    @staticmethod
-    def clean_title(title):
-        invalid_chars = [
-            ['!', ''],
-            ['?', ''],
-            [':', ' -'],
-            ['/', ' - '],
-            ['\\', ' '],
-            ['"', ' '],
-            ['<', ' '],
-            ['>', ' '],
-            ['|', ' '],
-            ['*', ' '],
-            ['?', ' ']
-        ]
-
-        for i in invalid_chars:
-            title = title.replace(i[0], i[1])
-        
-        return title
-
-
     def _extract_author_title_urls_parts(self, odm_filename):
         odm_root, metadata = self._get_odm_root_and_metadata(odm_filename)
         author = self._get_author_from_metadata(metadata)
         title = metadata.findtext('Title')
-        title = self.clean_title(title)
+        title = clean_file_string(title)
         cover_url = metadata.findtext('CoverUrl', '')
         logger.info('Got title "{}" and author'.format(title)
                      + ('s' if ';' in author else '')
                      + ' {} from ODM file {}'.format(
             ', '.join(author.split(';')),
             basename(odm_filename)))
```

### Comparing `sonus-0.6.2/sonus/main.py` & `sonus-0.6.3/sonus/main.py`

 * *Files identical despite different names*

### Comparing `sonus-0.6.2/sonus.egg-info/PKG-INFO` & `sonus-0.6.3/sonus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonus
-Version: 0.6.2
+Version: 0.6.3
 Summary: Cross-platform OverDrive audiobook client and chapterizer written in Python. 
 Home-page: https://github.com/digitalec/sonus
 Author: digitalec
 License: GPL3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
```

