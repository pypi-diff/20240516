# Comparing `tmp/metalarchivist-0.3.3.tar.gz` & `tmp/metalarchivist-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.3.3.tar", last modified: Wed May 15 23:40:10 2024, max compression
+gzip compressed data, was "metalarchivist-0.3.4.tar", last modified: Thu May 16 14:49:27 2024, max compression
```

## Comparing `metalarchivist-0.3.3.tar` & `metalarchivist-0.3.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.399529 metalarchivist-0.3.3/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-15 23:40:10.399529 metalarchivist-0.3.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 23:40:10.399529 metalarchivist-0.3.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.391529 metalarchivist-0.3.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.392529 metalarchivist-0.3.3/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.395529 metalarchivist-0.3.3/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.395529 metalarchivist-0.3.3/src/metalarchivist/export/data/
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/data/user-agents.json
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     9505 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/label.py
--rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.397529 metalarchivist-0.3.3/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6842 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/album.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.397529 metalarchivist-0.3.3/src/metalarchivist/interface/api/
--rw-rw-rw-   0 root         (0) root         (0)     3092 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4836 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/api/page.py
--rwxrwxrwx   0 root         (0) root         (0)     8469 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/label.py
--rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3645 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.399529 metalarchivist-0.3.3/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.398529 metalarchivist-0.3.3/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10013 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     4731 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_labels.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.889763 metalarchivist-0.3.4/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-16 14:49:27.889763 metalarchivist-0.3.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 14:49:27.889763 metalarchivist-0.3.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.881763 metalarchivist-0.3.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.883763 metalarchivist-0.3.4/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.885763 metalarchivist-0.3.4/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.885763 metalarchivist-0.3.4/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     9505 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.887763 metalarchivist-0.3.4/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6842 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.887763 metalarchivist-0.3.4/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3113 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4836 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8472 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     8106 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3645 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.888763 metalarchivist-0.3.4/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-16 14:49:27.000000 metalarchivist-0.3.4/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-05-16 14:49:27.000000 metalarchivist-0.3.4/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 14:49:27.000000 metalarchivist-0.3.4/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-16 14:49:27.000000 metalarchivist-0.3.4/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-16 14:49:27.000000 metalarchivist-0.3.4/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:49:27.888763 metalarchivist-0.3.4/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10013 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-16 14:49:14.000000 metalarchivist-0.3.4/src/test/test_themes.py
```

### Comparing `metalarchivist-0.3.3/LICENSE` & `metalarchivist-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/PKG-INFO` & `metalarchivist-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.3.3/pyproject.toml` & `metalarchivist-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.3.3"
+version = "0.3.4"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.3.3/src/metalarchivist/export/album.py` & `metalarchivist-0.3.4/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/export/band.py` & `metalarchivist-0.3.4/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/export/data/user-agents.json` & `metalarchivist-0.3.4/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/export/genre.py` & `metalarchivist-0.3.4/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/export/label.py` & `metalarchivist-0.3.4/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/export/util.py` & `metalarchivist-0.3.4/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.3.4/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/interface/album.py` & `metalarchivist-0.3.4/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/interface/api/base.py` & `metalarchivist-0.3.4/src/metalarchivist/interface/api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from abc import ABC
 from dataclasses import dataclass, field, InitVar, asdict
 from typing import ClassVar, Any
 
 from Crypto.Hash import BLAKE2s
 
 
+UNKNOWN = 'Unknown'
+
+
 def create_key(metallum_id: int, name: str) -> str:
     metallum_id_bytes = struct.pack('>Q', metallum_id)
     hash_obj = BLAKE2s.new(data=name.encode('utf-8'), digest_bytes=12, key=metallum_id_bytes)
     return hash_obj.hexdigest()
 
-
 @dataclass
 class PageDataType(ABC):
     ...
 
 
 @dataclass
 class Page(ABC):
```

### Comparing `metalarchivist-0.3.3/src/metalarchivist/interface/api/page.py` & `metalarchivist-0.3.4/src/metalarchivist/interface/api/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/interface/band.py` & `metalarchivist-0.3.4/src/metalarchivist/interface/band.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         desc_titles = profile_document.xpath(desc_titles_xpath)
         desc_titles = [re.sub(r'[^\w\s]+', '', title) for title in desc_titles]
         desc_titles = [re.sub(r'\s+', '_', title).lower() for title in desc_titles]
         return desc_titles
 
     @staticmethod
     def _parse_description_details(profile_document: lxml.etree.ElementBase) -> list[str]:
-        desc_detail_xpath = '//div[@id="band_stats"]/dl/dt/following-sibling::dd'
+        desc_detail_xpath = '//div[@id="band_stats"]/dl/dt/following-sibling::dd[1]'
         desc_detail = profile_document.xpath(desc_detail_xpath)
         desc_detail = [node.xpath('.//text()') for node in desc_detail]
         desc_detail = [''.join(text).replace('\n', ' ').strip() for text in desc_detail]
         desc_detail = ['Unknown' if detail == 'N/A' else detail for detail in desc_detail]
 
         return desc_detail
```

### Comparing `metalarchivist-0.3.3/src/metalarchivist/interface/genre.py` & `metalarchivist-0.3.4/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/interface/label.py` & `metalarchivist-0.3.4/src/metalarchivist/interface/label.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 import re
 from dataclasses import dataclass, field, InitVar, asdict
 
 import lxml.html
 import lxml.etree
+from lxml.etree import ElementBase
 
 from .api.base import create_key
 from .band import BandLink
 from .album import AlbumLink
 from .genre import Subgenres
 
 
+
+class LabelXPath:
+    EXTERNAL_LINKS = '//table[@id = "linksTablemain"]//td/a'
+    LABEL_NAME = '//h1[@class="label_name"]/text()[1]'
+    DESCRIPTION_TITLES = '//div[@id="label_info"]/dl/dt//text()'
+    DESCRIPTION_DETAILS = '//div[@id="label_info"]/dl/dt/following-sibling::dd[1]'
+    PARENT_LABEL = '//div[@id="label_info"]/dl/dt[text()="Parent label:"]/following-sibling::dd[1]/a'
+    SUBLABELS = '//div[@id="label_info"]/dl/dt[text()="Sub-labels:"]/following-sibling::dd[1]/a'
+
+
 @dataclass
 class LabelRosterMember:
     metallum_id: int
     band: BandLink
     subgenres: Subgenres
     country_of_origin: str
 
@@ -45,15 +56,20 @@
     label_key: str = field(init=False)
 
     def __post_init__(self, html: str):
         html_anchor = lxml.html.fragment_fromstring(html)
         self.name = html_anchor.text
         self.link = link = html_anchor.attrib['href']
         self.metallum_id = int(link.split('/').pop())
-        self.label_key = create_key(self.metallum_id, self.label_key)
+        self.label_key = create_key(self.metallum_id, self.name)
+
+    @classmethod
+    def from_element(cls, element: ElementBase):
+        kwargs = dict(method='html', with_tail=False)
+        return cls(lxml.etree.tostring(element, **kwargs))
 
 
 @dataclass
 class LabelRelease:
     band: BandLink
     album: AlbumLink
     release_type: str
@@ -64,36 +80,33 @@
 
     year: int = field(init=False)
 
     def __post_init__(self, year: str):
         self.year = int(year)
 
 
-
 @dataclass
 class LabelExternalLink:
     """ An HTML anchor tag pointing to a label's profile outside of metal-archives.com """
 
     name: str
     url: str
 
 
-
-
 @dataclass
 class LabelExternalLinks:
     """ A collection of profiles pertaining to a single band, defined by metallum_id """
 
     metallum_id: int
     html: InitVar[bytes]
     links: list = field(init=False)
 
     def __post_init__(self, links_html: bytes):
         links_document = lxml.html.document_fromstring(links_html)
-        anchors: list = links_document.xpath('//table[@id = "linksTablemain"]//td/a')
+        anchors: list = links_document.xpath(LabelXPath.EXTERNAL_LINKS)
         
         links = list()
         for link in anchors:
             try:
                 links.append(LabelExternalLink(link.text.strip(), link.attrib['href']))
             except AttributeError:
                 alt_name = link.attrib['title'].replace('Go to:', '').strip()
@@ -109,71 +122,108 @@
     has_shop: bool
 
     specialisation: str | None
     country: str | None
     website: str | None
 
 
-@dataclass(frozen=True)
+@dataclass
 class LabelDescription:
     """ Additional information pertaining to a unique label """
     address: str = field(kw_only=True)
     country: str = field(kw_only=True)
     phone_number: str = field(kw_only=True)
     status: str = field(kw_only=True)
     styles_and_specialties: str = field(kw_only=True)
     founding_date: str = field(kw_only=True)
     online_shopping: str = field(kw_only=True)
+    
+    parent_label: str | None = field(kw_only=True, default=None)
+    sublabels: str | None = field(kw_only=True, default=None)
+
+
+@dataclass
+class AssociatedLabels:
+    parent: LabelLink
+    children: list[LabelLink]
 
 
 @dataclass
 class LabelProfile:
     url: str
     html: InitVar[bytes]
 
     name: str = field(init=False)
     metallum_id: int = field(init=False)
     label_key: str = field(init=False)
     description: LabelDescription = field(init=False)
+    associated: AssociatedLabels | None = field(init=False, default=None)
 
     def __post_init__(self, profile_html: bytes):
         profile_document = lxml.html.fromstring(profile_html)
 
         if isinstance(profile_document, lxml.etree.ElementBase):
-            self.name = name = profile_document.xpath('//h1[@class="label_name"]/text()[1]').pop()
+            self.name = name = profile_document.xpath(LabelXPath.LABEL_NAME).pop()
             self.metallum_id = metallum_id = int(self.url.split('/')[-1])
             self.label_key = create_key(metallum_id, name)
 
             description_titles = self._parse_description_titles(profile_document)
             description_details = self._parse_description_details(profile_document)
             self.description = self._parse_description(description_titles, description_details)
 
+            self.associated = self._parse_associations(profile_document)
+
     @staticmethod
     def _parse_description_titles(profile_document: lxml.etree.ElementBase) -> list[str]:
-        desc_titles_xpath = '//div[@id="label_info"]/dl/dt//text()'
-        desc_titles = profile_document.xpath(desc_titles_xpath)
+        desc_titles = profile_document.xpath(LabelXPath.DESCRIPTION_TITLES)
         desc_titles = [re.sub(r'\/', ' and ', title) for title in desc_titles]
         desc_titles = [re.sub(r'[^\w\s]+', '', title) for title in desc_titles]
         desc_titles = [re.sub(r'\s+', '_', title.strip()).lower() for title in desc_titles]
         return desc_titles
 
     @staticmethod
     def _parse_description_details(profile_document: lxml.etree.ElementBase) -> list[str]:
-        desc_detail_xpath = '//div[@id="label_info"]/dl/dt/following-sibling::dd'
-        desc_detail = profile_document.xpath(desc_detail_xpath)
+        nonword_pattern = re.compile(r'\w')
+
+        desc_detail = profile_document.xpath(LabelXPath.DESCRIPTION_DETAILS)
         desc_detail = [node.xpath('./text()|./a/text()|./span/text()') for node in desc_detail]
-        desc_detail = [', '.join(filter(lambda n: n != '', map(str.strip, text))) for text in desc_detail]
+        desc_detail = [map(str.strip, filter(nonword_pattern.search, text)) for text in desc_detail]
+        desc_detail = [', '.join(filter(lambda n: n != '', text)) for text in desc_detail]
         desc_detail = ['Unknown' if detail == 'N/A' else detail for detail in desc_detail]
 
         return desc_detail
 
     @staticmethod
     def _parse_description(description_titles, description_details) -> LabelDescription:
         description = {dt: dd for dt, dd in zip(description_titles, description_details)}
         return LabelDescription(**description)
+    
+    @staticmethod
+    def _parse_associations(profile_document) -> AssociatedLabels | None:
+        
+        parent_label_link, children_label_links = None, None
+
+        try:            
+            parent_label_element = profile_document.xpath(LabelXPath.PARENT_LABEL).pop()
+        except IndexError:
+            pass
+        else:
+            parent_label_link = LabelLink.from_element(parent_label_element)
+
+        try:            
+            children_label_elements = profile_document.xpath(LabelXPath.SUBLABELS)
+        except IndexError:
+            pass
+        else:
+            children_label_links = [LabelLink.from_element(child) for child in children_label_elements]
+
+        if parent_label_link and children_label_links:
+            return AssociatedLabels(parent_label_link, children_label_links)
+        else:
+            return None
 
 
 @dataclass
 class LabelContainer:
     profile: LabelProfile
 
     roster_current: InitVar[list[LabelRosterMember]]
```

### Comparing `metalarchivist-0.3.3/src/metalarchivist/interface/theme.py` & `metalarchivist-0.3.4/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist/report.py` & `metalarchivist-0.3.4/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.3.4/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.3.3/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.3.4/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/test/test_albums.py` & `metalarchivist-0.3.4/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/test/test_bands.py` & `metalarchivist-0.3.4/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/test/test_genres.py` & `metalarchivist-0.3.4/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.3/src/test/test_labels.py` & `metalarchivist-0.3.4/src/test/test_labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,25 @@
         self.assertEqual(description.country, 'Germany')
         self.assertEqual(description.phone_number, '+49 371 26 22 800')
         self.assertEqual(description.status, 'active')
         self.assertEqual(description.styles_and_specialties, 'Music with far-right ideologies, NS metal, RAC')
         self.assertEqual(description.founding_date, 'Unknown')
         self.assertEqual(description.online_shopping, 'Yes')
 
+        label_profile = self.export.Label.get_profile('https://www.metal-archives.com/labels/The_Orchard/24316')
+        description = label_profile.description
+        self.assertIsNotNone(description.parent_label)
+        self.assertEqual(description.parent_label, 'Sony Music')
+        self.assertEqual(description.sublabels, 'Infernal Racket, TVT Records')
+
+        self.assertIsNotNone(label_profile.associated)
+        self.assertEqual(label_profile.associated.parent.name, 'Sony Music')
+        self.assertEqual(label_profile.associated.children[0].name, 'Infernal Racket')
+        self.assertEqual(label_profile.associated.children[1].name, 'TVT Records')
+
     def test_label_roster_current(self):
         label_roster = self.export.Label.get_label_roster_current(17802)
         self.assertIsNotNone(label_roster)
         self.assertGreater(len(label_roster.data), 0)
         
         label_roster_member = label_roster.data[0]
         self.assertIsNotNone(label_roster_member.band.band_key)
```

### Comparing `metalarchivist-0.3.3/src/test/test_themes.py` & `metalarchivist-0.3.4/src/test/test_themes.py`

 * *Files identical despite different names*

