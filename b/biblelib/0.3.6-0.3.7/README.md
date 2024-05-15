# Comparing `tmp/biblelib-0.3.6.tar.gz` & `tmp/biblelib-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblelib-0.3.6.tar", max compression
+gzip compressed data, was "biblelib-0.3.7.tar", max compression
```

## Comparing `biblelib-0.3.6.tar` & `biblelib-0.3.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.6/LICENSE.md
--rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.6/LICENSE.md~
--rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.6/README.md
--rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.6/biblelib/__init__.py
--rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.6/biblelib/book/ReadMe.md
--rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.6/biblelib/book/__init__.py
--rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.6/biblelib/book/book.py
--rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.6/biblelib/book/books.tsv
--rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.6/biblelib/sources.py
--rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.6/biblelib/unit/__init__.py
--rw-r--r--   0        0        0     5936 2024-04-23 02:01:59.233109 biblelib-0.3.6/biblelib/unit/book.py
--rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.6/biblelib/unit/bookchapters.tsv
--rw-r--r--   0        0        0     7217 2024-04-23 02:09:13.463233 biblelib-0.3.6/biblelib/unit/chapter.py
--rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.6/biblelib/unit/chapters.tsv
--rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.6/biblelib/unit/chapterverses.tsv
--rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.6/biblelib/unit/pericope.py
--rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.6/biblelib/unit/tempchapter.py
--rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.6/biblelib/unit/unit.py
--rw-r--r--   0        0        0     6339 2024-04-23 02:09:29.760805 biblelib-0.3.6/biblelib/unit/unitrange.py
--rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.6/biblelib/unit/verse.py
--rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.6/biblelib/versification/Enumerator.py
--rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.6/biblelib/versification/Mapper.py
--rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.6/biblelib/versification/ReadMe.md
--rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.6/biblelib/versification/VrefReader.py
--rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.6/biblelib/versification/__init__.py
--rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.6/biblelib/versification/eng-nt-vref.txt
--rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.6/biblelib/versification/eng-ot-vref.txt
--rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.6/biblelib/versification/eng-protestant-vref.txt
--rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.6/biblelib/versification/org-nt-vref.txt
--rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.6/biblelib/versification/org-ot-vref.txt
--rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.6/biblelib/versification/org-protestant-vref.txt
--rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.6/biblelib/versification/rso-nt-vref.txt
--rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.6/biblelib/versification/rso-ot-vref.txt
--rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.6/biblelib/versification/rso-protestant-vref.txt
--rw-r--r--   0        0        0      910 2024-05-06 23:25:56.736634 biblelib-0.3.6/biblelib/word/__init__.py
--rw-r--r--   0        0        0    25630 2024-05-09 21:24:01.299209 biblelib-0.3.6/biblelib/word/bcvwpid.py
--rw-r--r--   0        0        0      356 2024-05-06 23:17:32.231962 biblelib-0.3.6/biblelib/word/mappings/__init__.py
--rw-r--r--   0        0        0     5513 2024-05-06 22:42:51.746991 biblelib-0.3.6/biblelib/word/mappings/gnt.py
--rw-r--r--   0        0        0     1189 2024-05-07 00:20:11.048356 biblelib-0.3.6/biblelib/word/mappings/marble.py
--rw-r--r--   0        0        0     3671 2024-05-06 21:44:17.650867 biblelib-0.3.6/biblelib/word/mappings/wlcm.py
--rw-r--r--   0        0        0     1324 2024-05-09 21:35:48.550711 biblelib-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.7/LICENSE.md
+-rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.7/LICENSE.md~
+-rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.7/README.md
+-rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.7/biblelib/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.7/biblelib/book/ReadMe.md
+-rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.7/biblelib/book/__init__.py
+-rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.7/biblelib/book/book.py
+-rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.7/biblelib/book/books.tsv
+-rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.7/biblelib/sources.py
+-rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.7/biblelib/unit/__init__.py
+-rw-r--r--   0        0        0     5936 2024-04-23 02:01:59.233109 biblelib-0.3.7/biblelib/unit/book.py
+-rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.7/biblelib/unit/bookchapters.tsv
+-rw-r--r--   0        0        0     7217 2024-04-23 02:09:13.463233 biblelib-0.3.7/biblelib/unit/chapter.py
+-rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.7/biblelib/unit/chapters.tsv
+-rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.7/biblelib/unit/chapterverses.tsv
+-rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.7/biblelib/unit/pericope.py
+-rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.7/biblelib/unit/tempchapter.py
+-rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.7/biblelib/unit/unit.py
+-rw-r--r--   0        0        0     6339 2024-04-23 02:09:29.760805 biblelib-0.3.7/biblelib/unit/unitrange.py
+-rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.7/biblelib/unit/verse.py
+-rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.7/biblelib/versification/Enumerator.py
+-rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.7/biblelib/versification/Mapper.py
+-rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.7/biblelib/versification/ReadMe.md
+-rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.7/biblelib/versification/VrefReader.py
+-rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.7/biblelib/versification/__init__.py
+-rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.7/biblelib/versification/eng-nt-vref.txt
+-rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.7/biblelib/versification/eng-ot-vref.txt
+-rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.7/biblelib/versification/eng-protestant-vref.txt
+-rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.7/biblelib/versification/org-nt-vref.txt
+-rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.7/biblelib/versification/org-ot-vref.txt
+-rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.7/biblelib/versification/org-protestant-vref.txt
+-rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.7/biblelib/versification/rso-nt-vref.txt
+-rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.7/biblelib/versification/rso-ot-vref.txt
+-rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.7/biblelib/versification/rso-protestant-vref.txt
+-rw-r--r--   0        0        0      910 2024-05-06 23:25:56.736634 biblelib-0.3.7/biblelib/word/__init__.py
+-rw-r--r--   0        0        0    25767 2024-05-15 20:27:09.391972 biblelib-0.3.7/biblelib/word/bcvwpid.py
+-rw-r--r--   0        0        0      356 2024-05-06 23:17:32.231962 biblelib-0.3.7/biblelib/word/mappings/__init__.py
+-rw-r--r--   0        0        0     5513 2024-05-06 22:42:51.746991 biblelib-0.3.7/biblelib/word/mappings/gnt.py
+-rw-r--r--   0        0        0     1217 2024-05-15 21:20:20.778262 biblelib-0.3.7/biblelib/word/mappings/marble.py
+-rw-r--r--   0        0        0     3671 2024-05-06 21:44:17.650867 biblelib-0.3.7/biblelib/word/mappings/wlcm.py
+-rw-r--r--   0        0        0     1324 2024-05-15 21:22:55.351544 biblelib-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.7/PKG-INFO
```

### Comparing `biblelib-0.3.6/LICENSE.md` & `biblelib-0.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/LICENSE.md~` & `biblelib-0.3.7/LICENSE.md~`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/README.md` & `biblelib-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/book/ReadMe.md` & `biblelib-0.3.7/biblelib/book/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/book/book.py` & `biblelib-0.3.7/biblelib/book/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/book/books.tsv` & `biblelib-0.3.7/biblelib/book/books.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/sources.py` & `biblelib-0.3.7/biblelib/sources.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/__init__.py` & `biblelib-0.3.7/biblelib/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/book.py` & `biblelib-0.3.7/biblelib/unit/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/bookchapters.tsv` & `biblelib-0.3.7/biblelib/unit/bookchapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/chapter.py` & `biblelib-0.3.7/biblelib/unit/chapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/chapters.tsv` & `biblelib-0.3.7/biblelib/unit/chapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/chapterverses.tsv` & `biblelib-0.3.7/biblelib/unit/chapterverses.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/pericope.py` & `biblelib-0.3.7/biblelib/unit/pericope.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/tempchapter.py` & `biblelib-0.3.7/biblelib/unit/tempchapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/unit.py` & `biblelib-0.3.7/biblelib/unit/unit.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/unitrange.py` & `biblelib-0.3.7/biblelib/unit/unitrange.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/unit/verse.py` & `biblelib-0.3.7/biblelib/unit/verse.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/Enumerator.py` & `biblelib-0.3.7/biblelib/versification/Enumerator.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/Mapper.py` & `biblelib-0.3.7/biblelib/versification/Mapper.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/ReadMe.md` & `biblelib-0.3.7/biblelib/versification/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/VrefReader.py` & `biblelib-0.3.7/biblelib/versification/VrefReader.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/eng-nt-vref.txt` & `biblelib-0.3.7/biblelib/versification/eng-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/eng-ot-vref.txt` & `biblelib-0.3.7/biblelib/versification/eng-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/eng-protestant-vref.txt` & `biblelib-0.3.7/biblelib/versification/eng-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/org-nt-vref.txt` & `biblelib-0.3.7/biblelib/versification/org-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/org-ot-vref.txt` & `biblelib-0.3.7/biblelib/versification/org-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/org-protestant-vref.txt` & `biblelib-0.3.7/biblelib/versification/org-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/rso-nt-vref.txt` & `biblelib-0.3.7/biblelib/versification/rso-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/rso-ot-vref.txt` & `biblelib-0.3.7/biblelib/versification/rso-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/versification/rso-protestant-vref.txt` & `biblelib-0.3.7/biblelib/versification/rso-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/word/__init__.py` & `biblelib-0.3.7/biblelib/word/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/word/bcvwpid.py` & `biblelib-0.3.7/biblelib/word/bcvwpid.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,18 @@
         # also test that they're all digits, in the right range, etc.
 
     @property
     def to_bcvid(self) -> str:
         """Return string for the book, chapter, and verse ID."""
         return self.book_ID + self.chapter_ID + self.verse_ID
 
+    def get_id(self) -> str:
+        """Return BCVID string. For compatibility with BCVWPID."""
+        return self.to_bcvid
+
     def includes(self, other: Any) -> bool:
         """Return True if other is included in the scope of self.
 
         Simply based on substring matching. Any instance includes
         itself therefore.
 
         """
@@ -357,16 +361,16 @@
     - BB identifies a book
     - CCC identifies a chapter number
     - VVV identifies a verse number
     - WWW identifies a word number
     - P optionally identifies a word part: this is optional for NT
       books, where it defaults to 1 if output.
 
-    Identifiers may have an optional corpus prefix. This is removed
-    from the ID but retained as self.corpus_prefix.
+    Identifiers may have an optional canon prefix ("o" or "n"). This
+    is removed from the ID but retained as self.canon_prefix.
 
     This dataclass does not validate whether any identifiers are in
     the correct range: it only records the data. Validation is planned
     for a future version.
 
     All sequence indices are one-based, not zero-based, and derived
     from the tokenization of the input text (which should be specified
```

### Comparing `biblelib-0.3.6/biblelib/word/mappings/gnt.py` & `biblelib-0.3.7/biblelib/word/mappings/gnt.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/biblelib/word/mappings/marble.py` & `biblelib-0.3.7/biblelib/word/mappings/marble.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         bcvwpid.from_ubs() to handle the more general case of BCV
         references.
 
         """
         # some UBS DGNT references have this as a suffix: fragile
         if re.search(r"\({N:00\d}\)$", marbleid) or re.search(r"{N:00\d}$", marbleid):
             marbleid = marbleid[:14]
-        assert len(marbleid) == 14, f"Not a UBS reference: {marbleid}"
+        assert len(marbleid) == 14, f"{len(marbleid)} characters, not a UBS reference: {marbleid}"
 
         bookid = marbleid[:3]
         if "000" < bookid < "040":
             return self.wlcm.marble2macula(marbleid)
         elif "039" < bookid < "067":
             sblgnt = self.gnt.marble2sblgnt(marbleid)
             return [sblgnt] if sblgnt else []
```

### Comparing `biblelib-0.3.6/biblelib/word/mappings/wlcm.py` & `biblelib-0.3.7/biblelib/word/mappings/wlcm.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.6/pyproject.toml` & `biblelib-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biblelib"
-version = "0.3.6"
+version = "0.3.7"
 description = "Utilities for working with metadata for Bible books, references, pericopes, and other units."
 authors = ["Sean Boisen <sean.boisen@gmail.com>"]
 repository = "https://github.com/Clear-Bible/Biblelib/"
 # documentation = "https://sboisen.github.io/Biblelib/"
 readme = "README.md"
 # apparently text files are also shipped?
 # include = [
```

### Comparing `biblelib-0.3.6/PKG-INFO` & `biblelib-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblelib
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utilities for working with metadata for Bible books, references, pericopes, and other units.
 Home-page: https://github.com/Clear-Bible/Biblelib/
 Author: Sean Boisen
 Author-email: sean.boisen@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

