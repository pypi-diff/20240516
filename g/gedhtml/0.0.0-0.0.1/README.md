# Comparing `tmp/gedhtml-0.0.0.tar.gz` & `tmp/gedhtml-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gedhtml-0.0.0.tar", max compression
+gzip compressed data, was "gedhtml-0.0.1.tar", max compression
```

## Comparing `gedhtml-0.0.0.tar` & `gedhtml-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-05-09 11:08:48.471264 gedhtml-0.0.0/gedhtml/__init__.py
--rw-r--r--   0        0        0     1003 2024-05-11 21:16:45.255272 gedhtml-0.0.0/gedhtml/__main__.py
--rw-r--r--   0        0        0     3095 2024-05-11 22:40:28.770393 gedhtml-0.0.0/gedhtml/describe.py
--rw-r--r--   0        0        0     5258 2024-05-11 22:40:28.770393 gedhtml-0.0.0/gedhtml/family_tree.py
--rw-r--r--   0        0        0     2626 2024-05-15 19:25:45.092758 gedhtml-0.0.0/gedhtml/file.py
--rw-r--r--   0        0        0     1883 2024-05-11 22:40:28.781927 gedhtml-0.0.0/gedhtml/html_template.py
--rw-r--r--   0        0        0     3308 2024-05-11 22:40:28.783570 gedhtml-0.0.0/gedhtml/language.py
--rw-r--r--   0        0        0     3372 2024-05-11 22:40:48.653999 gedhtml-0.0.0/gedhtml/pedigree.py
--rw-r--r--   0        0        0      150 2024-05-11 22:40:48.653999 gedhtml-0.0.0/gedhtml/utils.py
--rw-r--r--   0        0        0    10360 2024-05-15 18:54:04.030585 gedhtml-0.0.0/gedhtml/webpage.py
--rw-r--r--   0        0        0     1088 2024-05-05 18:54:47.967253 gedhtml-0.0.0/LICENSE
--rw-r--r--   0        0        0      647 2024-05-15 19:00:29.400739 gedhtml-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 gedhtml-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-15 20:30:56.134940 gedhtml-0.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/__main__.py
+-rw-r--r--   0        0        0     3017 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/describe.py
+-rw-r--r--   0        0        0     5089 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/family_tree.py
+-rw-r--r--   0        0        0     2537 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/file.py
+-rw-r--r--   0        0        0     1826 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/html_template.py
+-rw-r--r--   0        0        0     3163 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/language.py
+-rw-r--r--   0        0        0     3277 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/pedigree.py
+-rw-r--r--   0        0        0      146 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/utils.py
+-rw-r--r--   0        0        0    10100 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/webpage.py
+-rw-r--r--   0        0        0      618 2024-05-15 20:31:05.282926 gedhtml-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 gedhtml-0.0.1/PKG-INFO
```

### Comparing `gedhtml-0.0.0/gedhtml/__main__.py` & `gedhtml-0.0.1/gedhtml/__main__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import argparse
-
-import gedhtml.file
-import gedhtml.language
-import gedhtml.webpage
-
-
-parser = argparse.ArgumentParser(description="GED to static HTML converter")
-parser.add_argument("filename", help="GED filename")
-parser.add_argument("-s", "--startid", help="ID of person for start page")
-parser.add_argument("-o", "--outputdir", help="Output directory", default="")
-parser.add_argument("-t", "--title", help="Website title", default="My<br>genealogy")
-parser.add_argument("-d", "--description", help="Website description", default="My genealogy page")
-parser.add_argument("-l", "--language", help="Language: NL or EN", default="NL")
-args = parser.parse_args()
-
-fam_tree = gedhtml.file.load(args.filename)
-if args.startid:
-    id = args.startid
-else:
-    ref = list(fam_tree.individuals.keys())[0]
-    id = fam_tree.individuals[ref].id
-
-lang = gedhtml.language.choose(args.language)
-
-gedhtml.webpage.generate(fam_tree, id, args.outputdir, args.title, args.description, lang)
+import argparse
+
+import gedhtml.file
+import gedhtml.language
+import gedhtml.webpage
+
+
+parser = argparse.ArgumentParser(description="GED to static HTML converter")
+parser.add_argument("filename", help="GED filename")
+parser.add_argument("-s", "--startid", help="ID of person for start page")
+parser.add_argument("-o", "--outputdir", help="Output directory", default="")
+parser.add_argument("-t", "--title", help="Website title", default="My<br>genealogy")
+parser.add_argument("-d", "--description", help="Website description", default="My genealogy page")
+parser.add_argument("-l", "--language", help="Language: NL or EN", default="NL")
+args = parser.parse_args()
+
+fam_tree = gedhtml.file.load(args.filename)
+if args.startid:
+    id = args.startid
+else:
+    ref = list(fam_tree.individuals.keys())[0]
+    id = fam_tree.individuals[ref].id
+
+lang = gedhtml.language.choose(args.language)
+
+gedhtml.webpage.generate(fam_tree, id, args.outputdir, args.title, args.description, lang)
```

### Comparing `gedhtml-0.0.0/gedhtml/family_tree.py` & `gedhtml-0.0.1/gedhtml/family_tree.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-from dataclasses import dataclass
-
-
-def _truncate_names(names):
-    for name in names:
-        if len(name) > 0:
-            if name[0].isalpha() and name[-1].isalpha():
-                yield name
-
-
-@dataclass 
-class Individual:
-    ref: str
-    notes: list[str]
-    fam_child_refs: list[str]
-    fam_spouse_refs: list[str]
-    sex: str = "U"
-    first_name: str = ""
-    last_name_prefix: str = ""
-    last_name: str = ""
-    birth_date: str = ""
-    birth_place: str = ""
-    baptism_date: str = ""
-    baptism_place: str = ""
-    death_date: str = ""
-    death_place: str = ""
-    burial_date: str = ""
-    burial_place: str = ""
-
-    @property
-    def id(self) -> str:
-        return self.ref[1:-1]
-    
-    @property
-    def link(self) -> str:
-        return f"{self.id}.html"
-
-    @property
-    def birth_year(self) -> int | None:
-        if self.birth_date == "":
-            return None
-        for part in reversed(self.birth_date.split(' ')):
-            try:
-                return int(part)
-            except ValueError:
-                pass
-        return None
-    
-    @property
-    def private(self) -> bool:
-        for note in self.notes:
-            if note == "private":
-                return True
-        if self.birth_year is None or self.birth_year < 1940:
-            return False
-        return True
-
-    @property
-    def name(self) -> str:
-        if self.private:
-            return self.initial
-        else:
-            return self.full_name
-
-    @property
-    def full_name(self) -> str:
-        if self.last_name_prefix == "":
-            return f"{self.first_name} {self.last_name}"
-        else:
-            return f"{self.first_name} {self.last_name_prefix} {self.last_name}"
-    
-    @property
-    def newline_name(self) -> str:
-        short_first_name, short_last_name = self.short_name
-        if self.private:
-            return self.initial
-        else:
-            return f"{short_first_name}\\n{short_last_name}"
-
-    @property
-    def short_name(self) -> tuple[str, str]:
-
-        first_names = self.first_name.split(' ')
-        short_first_name = first_names[0]
-        for name in _truncate_names(first_names[1:]):
-            short_first_name += f" {name[0]}."
-
-        short_last_name = ""
-        for prefix in _truncate_names(self.last_name_prefix.split(' ')):
-            short_last_name += f"{prefix[0]}. "
-        last_names = self.last_name.split(' ')
-        short_last_name += last_names[0]
-        for name in _truncate_names(last_names[1:]):
-            short_last_name += f" {name}"
-
-        return short_first_name, short_last_name
-    
-    @property
-    def first_last_name(self):
-        return self.last_name.split(' ')[0]
-
-    @property
-    def initial(self) -> str:
-        if len(self.first_name) > 0:
-            return self.first_name[0]
-        else:
-            return ""
-
-
-@dataclass
-class Family:
-    ref: str
-    child_refs: list[str]
-    husband_ref: str = ""
-    wife_ref: str = ""
-    marriage_date: str = ""
-    marriage_place: str = ""
-
-
-class FamilyTree:
-
-    def __init__(self):
-        self.individuals = dict()  # Keys: Individual.ref; values: Individual
-        self.families = dict()  # Keys: Family.ref; values: Family
-
-    def add_individual(self, individual: Individual):
-        self.individuals[individual.ref] = individual
-
-    def add_family(self, family: Family):
-        self.families[family.ref] = family
-
-    def get_children(self, individual: Individual) -> list[Individual]:
-        children = []
-        for ref in individual.fam_spouse_refs:
-            family = self.families[ref]
-            for child_ref in family.child_refs:
-                children.append(self.individuals[child_ref])
-        return children
-
-    def get_parents(self, individual: Individual) -> list[Individual]:
-        parents = []
-        for ref in individual.fam_child_refs:
-            family = self.families[ref]
-            if family.husband_ref != "":
-                parents.append(self.individuals[family.husband_ref])
-            if family.wife_ref != "":
-                parents.append(self.individuals[family.wife_ref])
-        return parents
-
-    def get_spouses(self, individual: Individual) -> tuple[list[Individual], list[Family]]:
-        spouses = []
-        marriages = []
-        for ref in individual.fam_spouse_refs:
-            family = self.families[ref]
-            if family.husband_ref != "" and family.husband_ref != individual.ref:
-                spouses.append(self.individuals[family.husband_ref])
-            elif family.wife_ref != "" and family.wife_ref != individual.ref:
-                spouses.append(self.individuals[family.wife_ref])
-            marriages.append(family)
-        return spouses, marriages
-
-    def get_siblings(self, individual: Individual) -> list[Individual]:
-        siblings = []
-        for ref in individual.fam_child_refs:
-            family = self.families[ref]
-            for child_ref in family.child_refs:
-                if child_ref != individual.ref:
-                    siblings.append(self.individuals[child_ref])
-        return siblings
+from dataclasses import dataclass
+
+
+def _truncate_names(names):
+    for name in names:
+        if len(name) > 0:
+            if name[0].isalpha() and name[-1].isalpha():
+                yield name
+
+
+@dataclass 
+class Individual:
+    ref: str
+    notes: list[str]
+    fam_child_refs: list[str]
+    fam_spouse_refs: list[str]
+    sex: str = "U"
+    first_name: str = ""
+    last_name_prefix: str = ""
+    last_name: str = ""
+    birth_date: str = ""
+    birth_place: str = ""
+    baptism_date: str = ""
+    baptism_place: str = ""
+    death_date: str = ""
+    death_place: str = ""
+    burial_date: str = ""
+    burial_place: str = ""
+
+    @property
+    def id(self) -> str:
+        return self.ref[1:-1]
+    
+    @property
+    def link(self) -> str:
+        return f"{self.id}.html"
+
+    @property
+    def birth_year(self) -> int | None:
+        if self.birth_date == "":
+            return None
+        for part in reversed(self.birth_date.split(' ')):
+            try:
+                return int(part)
+            except ValueError:
+                pass
+        return None
+    
+    @property
+    def private(self) -> bool:
+        for note in self.notes:
+            if note == "private":
+                return True
+        if self.birth_year is None or self.birth_year < 1940:
+            return False
+        return True
+
+    @property
+    def name(self) -> str:
+        if self.private:
+            return self.initial
+        else:
+            return self.full_name
+
+    @property
+    def full_name(self) -> str:
+        if self.last_name_prefix == "":
+            return f"{self.first_name} {self.last_name}"
+        else:
+            return f"{self.first_name} {self.last_name_prefix} {self.last_name}"
+    
+    @property
+    def newline_name(self) -> str:
+        short_first_name, short_last_name = self.short_name
+        if self.private:
+            return self.initial
+        else:
+            return f"{short_first_name}\\n{short_last_name}"
+
+    @property
+    def short_name(self) -> tuple[str, str]:
+
+        first_names = self.first_name.split(' ')
+        short_first_name = first_names[0]
+        for name in _truncate_names(first_names[1:]):
+            short_first_name += f" {name[0]}."
+
+        short_last_name = ""
+        for prefix in _truncate_names(self.last_name_prefix.split(' ')):
+            short_last_name += f"{prefix[0]}. "
+        last_names = self.last_name.split(' ')
+        short_last_name += last_names[0]
+        for name in _truncate_names(last_names[1:]):
+            short_last_name += f" {name}"
+
+        return short_first_name, short_last_name
+    
+    @property
+    def first_last_name(self):
+        return self.last_name.split(' ')[0]
+
+    @property
+    def initial(self) -> str:
+        if len(self.first_name) > 0:
+            return self.first_name[0]
+        else:
+            return ""
+
+
+@dataclass
+class Family:
+    ref: str
+    child_refs: list[str]
+    husband_ref: str = ""
+    wife_ref: str = ""
+    marriage_date: str = ""
+    marriage_place: str = ""
+
+
+class FamilyTree:
+
+    def __init__(self):
+        self.individuals = dict()  # Keys: Individual.ref; values: Individual
+        self.families = dict()  # Keys: Family.ref; values: Family
+
+    def add_individual(self, individual: Individual):
+        self.individuals[individual.ref] = individual
+
+    def add_family(self, family: Family):
+        self.families[family.ref] = family
+
+    def get_children(self, individual: Individual) -> list[Individual]:
+        children = []
+        for ref in individual.fam_spouse_refs:
+            family = self.families[ref]
+            for child_ref in family.child_refs:
+                children.append(self.individuals[child_ref])
+        return children
+
+    def get_parents(self, individual: Individual) -> list[Individual]:
+        parents = []
+        for ref in individual.fam_child_refs:
+            family = self.families[ref]
+            if family.husband_ref != "":
+                parents.append(self.individuals[family.husband_ref])
+            if family.wife_ref != "":
+                parents.append(self.individuals[family.wife_ref])
+        return parents
+
+    def get_spouses(self, individual: Individual) -> tuple[list[Individual], list[Family]]:
+        spouses = []
+        marriages = []
+        for ref in individual.fam_spouse_refs:
+            family = self.families[ref]
+            if family.husband_ref != "" and family.husband_ref != individual.ref:
+                spouses.append(self.individuals[family.husband_ref])
+            elif family.wife_ref != "" and family.wife_ref != individual.ref:
+                spouses.append(self.individuals[family.wife_ref])
+            marriages.append(family)
+        return spouses, marriages
+
+    def get_siblings(self, individual: Individual) -> list[Individual]:
+        siblings = []
+        for ref in individual.fam_child_refs:
+            family = self.families[ref]
+            for child_ref in family.child_refs:
+                if child_ref != individual.ref:
+                    siblings.append(self.individuals[child_ref])
+        return siblings
```

### Comparing `gedhtml-0.0.0/gedhtml/html_template.py` & `gedhtml-0.0.1/gedhtml/html_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,115 @@
 00000000: 6465 6620 6d61 696e 2874 6974 6c65 2c20  def main(title, 
 00000010: 6465 7363 7269 7074 696f 6e2c 206d 656e  description, men
 00000020: 752c 2068 6561 6465 722c 2063 6f6e 7465  u, header, conte
-00000030: 6e74 293a 0d0a 2020 2020 7265 7475 726e  nt):..    return
-00000040: 2066 2222 220d 0a20 2020 2020 2020 203c   f"""..        <
-00000050: 2164 6f63 7479 7065 2068 746d 6c3e 0d0a  !doctype html>..
-00000060: 2020 2020 2020 2020 3c68 746d 6c20 6c61          <html la
-00000070: 6e67 3d22 656e 223e 0d0a 2020 2020 2020  ng="en">..      
-00000080: 2020 3c68 6561 643e 0d0a 2020 2020 2020    <head>..      
-00000090: 2020 2020 2020 3c6d 6574 6120 6368 6172        <meta char
-000000a0: 7365 743d 2275 7466 2d38 223e 0d0a 2020  set="utf-8">..  
-000000b0: 2020 2020 2020 2020 2020 3c6d 6574 6120            <meta 
-000000c0: 6e61 6d65 3d22 7669 6577 706f 7274 2220  name="viewport" 
-000000d0: 636f 6e74 656e 743d 2277 6964 7468 3d64  content="width=d
-000000e0: 6576 6963 652d 7769 6474 682c 2069 6e69  evice-width, ini
-000000f0: 7469 616c 2d73 6361 6c65 3d31 2e30 223e  tial-scale=1.0">
-00000100: 0d0a 2020 2020 2020 2020 2020 2020 3c6d  ..            <m
-00000110: 6574 6120 6e61 6d65 3d22 6465 7363 7269  eta name="descri
-00000120: 7074 696f 6e22 2063 6f6e 7465 6e74 3d22  ption" content="
-00000130: 7b64 6573 6372 6970 7469 6f6e 7d22 3e0d  {description}">.
-00000140: 0a20 2020 2020 2020 2020 2020 203c 7469  .            <ti
-00000150: 746c 653e 7b74 6974 6c65 7d3c 2f74 6974  tle>{title}</tit
-00000160: 6c65 3e0d 0a20 2020 2020 2020 2020 2020  le>..           
-00000170: 203c 6c69 6e6b 2072 656c 3d22 7374 796c   <link rel="styl
-00000180: 6573 6865 6574 2220 6872 6566 3d22 7075  esheet" href="pu
-00000190: 7265 2d6d 696e 2e63 7373 223e 0d0a 2020  re-min.css">..  
-000001a0: 2020 2020 2020 2020 2020 3c6c 696e 6b20            <link 
-000001b0: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
-000001c0: 2068 7265 663d 2273 7479 6c65 2e63 7373   href="style.css
-000001d0: 223e 0d0a 2020 2020 2020 2020 3c2f 6865  ">..        </he
-000001e0: 6164 3e0d 0a20 2020 2020 2020 203c 626f  ad>..        <bo
-000001f0: 6479 3e0d 0a0d 0a20 2020 2020 2020 203c  dy>....        <
-00000200: 7363 7269 7074 2073 7263 3d22 6368 6172  script src="char
-00000210: 742e 6a73 223e 3c2f 7363 7269 7074 3e0d  t.js"></script>.
-00000220: 0a20 2020 2020 2020 203c 7363 7269 7074  .        <script
-00000230: 2073 7263 3d22 6368 6172 746a 732d 706c   src="chartjs-pl
-00000240: 7567 696e 2d64 6174 616c 6162 656c 732e  ugin-datalabels.
-00000250: 6a73 223e 3c2f 7363 7269 7074 3e0d 0a20  js"></script>.. 
-00000260: 2020 2020 2020 203c 7363 7269 7074 2073         <script s
-00000270: 7263 3d22 7065 6469 6772 6565 2e6a 7322  rc="pedigree.js"
-00000280: 3e3c 2f73 6372 6970 743e 0d0a 2020 2020  ></script>..    
-00000290: 2020 2020 3c73 6372 6970 7420 7372 633d      <script src=
-000002a0: 2275 692e 6a73 223e 3c2f 7363 7269 7074  "ui.js"></script
-000002b0: 3e0d 0a0d 0a20 2020 2020 2020 203c 6469  >....        <di
-000002c0: 7620 6964 3d22 6c61 796f 7574 223e 0d0a  v id="layout">..
-000002d0: 0d0a 2020 2020 2020 2020 2020 2020 3c61  ..            <a
-000002e0: 2068 7265 663d 2223 6d65 6e75 2220 6964   href="#menu" id
-000002f0: 3d22 6d65 6e75 4c69 6e6b 2220 636c 6173  ="menuLink" clas
-00000300: 733d 226d 656e 752d 6c69 6e6b 223e 0d0a  s="menu-link">..
-00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000320: 3c73 7061 6e3e 3c2f 7370 616e 3e0d 0a20  <span></span>.. 
-00000330: 2020 2020 2020 2020 2020 203c 2f61 3e0d             </a>.
-00000340: 0a0d 0a20 2020 2020 2020 2020 2020 203c  ...            <
-00000350: 6469 7620 6964 3d22 6d65 6e75 223e 0d0a  div id="menu">..
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 3c64 6976 2063 6c61 7373 3d22 7075 7265  <div class="pure
-00000380: 2d6d 656e 7522 3e0d 0a20 2020 2020 2020  -menu">..       
-00000390: 2020 2020 2020 2020 2020 2020 203c 6120               <a 
-000003a0: 636c 6173 733d 2270 7572 652d 6d65 6e75  class="pure-menu
-000003b0: 2d68 6561 6469 6e67 2220 6872 6566 3d22  -heading" href="
-000003c0: 696e 6465 782e 6874 6d6c 223e 7b74 6974  index.html">{tit
-000003d0: 6c65 7d3c 2f61 3e0d 0a0d 0a20 2020 2020  le}</a>....     
-000003e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000003f0: 6d65 6e75 7d0d 0a20 2020 2020 2020 2020  menu}..         
-00000400: 2020 2020 2020 203c 2f64 6976 3e0d 0a20         </div>.. 
-00000410: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00000420: 3e0d 0a0d 0a20 2020 2020 2020 2020 2020  >....           
-00000430: 203c 6469 7620 6964 3d22 6d61 696e 223e   <div id="main">
-00000440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000450: 2020 3c64 6976 2063 6c61 7373 3d22 6865    <div class="he
-00000460: 6164 6572 223e 0d0a 2020 2020 2020 2020  ader">..        
-00000470: 2020 2020 2020 2020 2020 2020 7b68 6561              {hea
-00000480: 6465 727d 0d0a 2020 2020 2020 2020 2020  der}..          
-00000490: 2020 2020 2020 3c2f 6469 763e 0d0a 0d0a        </div>....
+00000030: 6e74 293a 0a20 2020 2072 6574 7572 6e20  nt):.    return 
+00000040: 6622 2222 0a20 2020 2020 2020 203c 2164  f""".        <!d
+00000050: 6f63 7479 7065 2068 746d 6c3e 0a20 2020  octype html>.   
+00000060: 2020 2020 203c 6874 6d6c 206c 616e 673d       <html lang=
+00000070: 2265 6e22 3e0a 2020 2020 2020 2020 3c68  "en">.        <h
+00000080: 6561 643e 0a20 2020 2020 2020 2020 2020  ead>.           
+00000090: 203c 6d65 7461 2063 6861 7273 6574 3d22   <meta charset="
+000000a0: 7574 662d 3822 3e0a 2020 2020 2020 2020  utf-8">.        
+000000b0: 2020 2020 3c6d 6574 6120 6e61 6d65 3d22      <meta name="
+000000c0: 7669 6577 706f 7274 2220 636f 6e74 656e  viewport" conten
+000000d0: 743d 2277 6964 7468 3d64 6576 6963 652d  t="width=device-
+000000e0: 7769 6474 682c 2069 6e69 7469 616c 2d73  width, initial-s
+000000f0: 6361 6c65 3d31 2e30 223e 0a20 2020 2020  cale=1.0">.     
+00000100: 2020 2020 2020 203c 6d65 7461 206e 616d         <meta nam
+00000110: 653d 2264 6573 6372 6970 7469 6f6e 2220  e="description" 
+00000120: 636f 6e74 656e 743d 227b 6465 7363 7269  content="{descri
+00000130: 7074 696f 6e7d 223e 0a20 2020 2020 2020  ption}">.       
+00000140: 2020 2020 203c 7469 746c 653e 7b74 6974       <title>{tit
+00000150: 6c65 7d3c 2f74 6974 6c65 3e0a 2020 2020  le}</title>.    
+00000160: 2020 2020 2020 2020 3c6c 696e 6b20 7265          <link re
+00000170: 6c3d 2273 7479 6c65 7368 6565 7422 2068  l="stylesheet" h
+00000180: 7265 663d 2270 7572 652d 6d69 6e2e 6373  ref="pure-min.cs
+00000190: 7322 3e0a 2020 2020 2020 2020 2020 2020  s">.            
+000001a0: 3c6c 696e 6b20 7265 6c3d 2273 7479 6c65  <link rel="style
+000001b0: 7368 6565 7422 2068 7265 663d 2273 7479  sheet" href="sty
+000001c0: 6c65 2e63 7373 223e 0a20 2020 2020 2020  le.css">.       
+000001d0: 203c 2f68 6561 643e 0a20 2020 2020 2020   </head>.       
+000001e0: 203c 626f 6479 3e0a 0a20 2020 2020 2020   <body>..       
+000001f0: 203c 7363 7269 7074 2073 7263 3d22 6368   <script src="ch
+00000200: 6172 742e 6a73 223e 3c2f 7363 7269 7074  art.js"></script
+00000210: 3e0a 2020 2020 2020 2020 3c73 6372 6970  >.        <scrip
+00000220: 7420 7372 633d 2263 6861 7274 6a73 2d70  t src="chartjs-p
+00000230: 6c75 6769 6e2d 6461 7461 6c61 6265 6c73  lugin-datalabels
+00000240: 2e6a 7322 3e3c 2f73 6372 6970 743e 0a20  .js"></script>. 
+00000250: 2020 2020 2020 203c 7363 7269 7074 2073         <script s
+00000260: 7263 3d22 7065 6469 6772 6565 2e6a 7322  rc="pedigree.js"
+00000270: 3e3c 2f73 6372 6970 743e 0a20 2020 2020  ></script>.     
+00000280: 2020 203c 7363 7269 7074 2073 7263 3d22     <script src="
+00000290: 7569 2e6a 7322 3e3c 2f73 6372 6970 743e  ui.js"></script>
+000002a0: 0a0a 2020 2020 2020 2020 3c64 6976 2069  ..        <div i
+000002b0: 643d 226c 6179 6f75 7422 3e0a 0a20 2020  d="layout">..   
+000002c0: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
+000002d0: 3d22 236d 656e 7522 2069 643d 226d 656e  ="#menu" id="men
+000002e0: 754c 696e 6b22 2063 6c61 7373 3d22 6d65  uLink" class="me
+000002f0: 6e75 2d6c 696e 6b22 3e0a 2020 2020 2020  nu-link">.      
+00000300: 2020 2020 2020 2020 2020 3c73 7061 6e3e            <span>
+00000310: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+00000320: 2020 2020 3c2f 613e 0a0a 2020 2020 2020      </a>..      
+00000330: 2020 2020 2020 3c64 6976 2069 643d 226d        <div id="m
+00000340: 656e 7522 3e0a 2020 2020 2020 2020 2020  enu">.          
+00000350: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000360: 3d22 7075 7265 2d6d 656e 7522 3e0a 2020  ="pure-menu">.  
+00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000380: 2020 3c61 2063 6c61 7373 3d22 7075 7265    <a class="pure
+00000390: 2d6d 656e 752d 6865 6164 696e 6722 2068  -menu-heading" h
+000003a0: 7265 663d 2269 6e64 6578 2e68 746d 6c22  ref="index.html"
+000003b0: 3e7b 7469 746c 657d 3c2f 613e 0a0a 2020  >{title}</a>..  
+000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003d0: 2020 7b6d 656e 757d 0a20 2020 2020 2020    {menu}.       
+000003e0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+000003f0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000400: 763e 0a0a 2020 2020 2020 2020 2020 2020  v>..            
+00000410: 3c64 6976 2069 643d 226d 6169 6e22 3e0a  <div id="main">.
+00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000430: 3c64 6976 2063 6c61 7373 3d22 6865 6164  <div class="head
+00000440: 6572 223e 0a20 2020 2020 2020 2020 2020  er">.           
+00000450: 2020 2020 2020 2020 207b 6865 6164 6572           {header
+00000460: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000470: 2020 3c2f 6469 763e 0a0a 2020 2020 2020    </div>..      
+00000480: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000490: 6c61 7373 3d22 636f 6e74 656e 7422 3e0a  lass="content">.
 000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004b0: 3c64 6976 2063 6c61 7373 3d22 636f 6e74  <div class="cont
-000004c0: 656e 7422 3e0d 0a20 2020 2020 2020 2020  ent">..         
-000004d0: 2020 2020 2020 2020 2020 207b 636f 6e74             {cont
-000004e0: 656e 747d 0d0a 2020 2020 2020 2020 2020  ent}..          
-000004f0: 2020 2020 2020 3c2f 6469 763e 0d0a 2020        </div>..  
-00000500: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000510: 0d0a 2020 2020 2020 2020 3c2f 6469 763e  ..        </div>
-00000520: 0d0a 0d0a 2020 2020 2020 2020 3c2f 626f  ....        </bo
-00000530: 6479 3e0d 0a20 2020 2020 2020 203c 2f68  dy>..        </h
-00000540: 746d 6c3e 0d0a 0d0a 2020 2020 2020 2020  tml>....        
-00000550: 2222 220d 0a20 2020 200d 0a64 6566 206d  """..    ..def m
-00000560: 656e 7528 7374 6172 745f 7061 6765 2c20  enu(start_page, 
-00000570: 6e61 6d65 5f69 6e64 6578 2c20 6162 6f75  name_index, abou
-00000580: 745f 7061 6765 293a 0d0a 2020 2020 7265  t_page):..    re
-00000590: 7475 726e 2066 2222 220d 0a20 2020 2020  turn f"""..     
-000005a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000005b0: 756c 2063 6c61 7373 3d22 7075 7265 2d6d  ul class="pure-m
-000005c0: 656e 752d 6c69 7374 223e 0d0a 2020 2020  enu-list">..    
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 2020 2020 3c6c 6920 636c 6173 733d 2270      <li class="p
-000005f0: 7572 652d 6d65 6e75 2d69 7465 6d22 3e3c  ure-menu-item"><
-00000600: 6120 6872 6566 3d22 696e 6465 782e 6874  a href="index.ht
-00000610: 6d6c 2220 636c 6173 733d 2270 7572 652d  ml" class="pure-
-00000620: 6d65 6e75 2d6c 696e 6b22 3e7b 7374 6172  menu-link">{star
-00000630: 745f 7061 6765 7d3c 2f61 3e3c 2f6c 693e  t_page}</a></li>
-00000640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000650: 2020 2020 2020 2020 2020 3c6c 6920 636c            <li cl
-00000660: 6173 733d 2270 7572 652d 6d65 6e75 2d69  ass="pure-menu-i
-00000670: 7465 6d22 3e3c 6120 6872 6566 3d22 6e61  tem"><a href="na
-00000680: 6d65 5f69 6e64 6578 2e68 746d 6c22 2063  me_index.html" c
-00000690: 6c61 7373 3d22 7075 7265 2d6d 656e 752d  lass="pure-menu-
-000006a0: 6c69 6e6b 223e 7b6e 616d 655f 696e 6465  link">{name_inde
-000006b0: 787d 3c2f 613e 3c2f 6c69 3e0d 0a20 2020  x}</a></li>..   
-000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006d0: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
-000006e0: 7075 7265 2d6d 656e 752d 6974 656d 223e  pure-menu-item">
-000006f0: 3c61 2068 7265 663d 2261 626f 7574 2e68  <a href="about.h
-00000700: 746d 6c22 2063 6c61 7373 3d22 7075 7265  tml" class="pure
-00000710: 2d6d 656e 752d 6c69 6e6b 223e 7b61 626f  -menu-link">{abo
-00000720: 7574 5f70 6167 657d 3c2f 613e 3c2f 6c69  ut_page}</a></li
-00000730: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00000740: 2020 2020 2020 203c 2f75 6c3e 0d0a 2020         </ul>..  
-00000750: 2020 2020 2020 2222 220d 0a                    """..
+000004b0: 2020 2020 7b63 6f6e 7465 6e74 7d0a 2020      {content}.  
+000004c0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000004d0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000004e0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000004f0: 3c2f 6469 763e 0a0a 2020 2020 2020 2020  </div>..        
+00000500: 3c2f 626f 6479 3e0a 2020 2020 2020 2020  </body>.        
+00000510: 3c2f 6874 6d6c 3e0a 0a20 2020 2020 2020  </html>..       
+00000520: 2022 2222 0a20 2020 200a 6465 6620 6d65   """.    .def me
+00000530: 6e75 2873 7461 7274 5f70 6167 652c 206e  nu(start_page, n
+00000540: 616d 655f 696e 6465 782c 2061 626f 7574  ame_index, about
+00000550: 5f70 6167 6529 3a0a 2020 2020 7265 7475  _page):.    retu
+00000560: 726e 2066 2222 220a 2020 2020 2020 2020  rn f""".        
+00000570: 2020 2020 2020 2020 2020 2020 3c75 6c20              <ul 
+00000580: 636c 6173 733d 2270 7572 652d 6d65 6e75  class="pure-menu
+00000590: 2d6c 6973 7422 3e0a 2020 2020 2020 2020  -list">.        
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005b0: 3c6c 6920 636c 6173 733d 2270 7572 652d  <li class="pure-
+000005c0: 6d65 6e75 2d69 7465 6d22 3e3c 6120 6872  menu-item"><a hr
+000005d0: 6566 3d22 696e 6465 782e 6874 6d6c 2220  ef="index.html" 
+000005e0: 636c 6173 733d 2270 7572 652d 6d65 6e75  class="pure-menu
+000005f0: 2d6c 696e 6b22 3e7b 7374 6172 745f 7061  -link">{start_pa
+00000600: 6765 7d3c 2f61 3e3c 2f6c 693e 0a20 2020  ge}</a></li>.   
+00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000620: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
+00000630: 7075 7265 2d6d 656e 752d 6974 656d 223e  pure-menu-item">
+00000640: 3c61 2068 7265 663d 226e 616d 655f 696e  <a href="name_in
+00000650: 6465 782e 6874 6d6c 2220 636c 6173 733d  dex.html" class=
+00000660: 2270 7572 652d 6d65 6e75 2d6c 696e 6b22  "pure-menu-link"
+00000670: 3e7b 6e61 6d65 5f69 6e64 6578 7d3c 2f61  >{name_index}</a
+00000680: 3e3c 2f6c 693e 0a20 2020 2020 2020 2020  ></li>.         
+00000690: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000006a0: 6c69 2063 6c61 7373 3d22 7075 7265 2d6d  li class="pure-m
+000006b0: 656e 752d 6974 656d 223e 3c61 2068 7265  enu-item"><a hre
+000006c0: 663d 2261 626f 7574 2e68 746d 6c22 2063  f="about.html" c
+000006d0: 6c61 7373 3d22 7075 7265 2d6d 656e 752d  lass="pure-menu-
+000006e0: 6c69 6e6b 223e 7b61 626f 7574 5f70 6167  link">{about_pag
+000006f0: 657d 3c2f 613e 3c2f 6c69 3e0a 2020 2020  e}</a></li>.    
+00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000710: 3c2f 756c 3e0a 2020 2020 2020 2020 2222  </ul>.        ""
+00000720: 220a                                     ".
```

### Comparing `gedhtml-0.0.0/gedhtml/language.py` & `gedhtml-0.0.1/gedhtml/language.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-from typing import Protocol
-
-
-class Language(Protocol):
-
-    link_text_start_page: str
-    link_text_name_index: str
-    link_text_about_page: str
-
-    header_name_index: str
-    header_pedigree: str
-    header_children: str
-    header_parents: str
-    header_siblings: str
-    header_spouses: str
-    header_notes: str
-
-    date_unknown: str
-    person_unknown: str
-
-    default_content_about: str
-
-    date_mapping: dict
-
-    prepositions: dict
-
-    participles: dict
-
-
-class Dutch:
-
-    link_text_start_page = "Startpagina"
-    link_text_name_index = "Namenindex"
-    link_text_about_page = "About"
-
-    header_pedigree = "Voorouders"
-    header_children = "Kinderen"
-    header_parents = "Ouders"
-    header_siblings = "Broers en zussen"
-    header_spouses = "Echtgenoten"
-    header_notes = "Notities"
-    header_name_index = "Namenindex"
-    
-    date_unknown = "onbekend"
-    person_unknown = "onbekend"
-
-    default_content_about = "Nou gewoon, voor de leuk."
-
-    date_mapping = {
-        'ABOUT': 'ongeveer',
-        'BEFORE': 'vóór',
-        'AFTER': 'na',
-        'BET': 'tussen',
-        'AND': 'en',
-        'JAN': 'januari',
-        'FEB': 'februari',
-        'MAR': 'maart',
-        'APR': 'april',
-        'MAY': 'mei',
-        'JUN': 'juni',
-        'JUL': 'juli',
-        'AUG': 'augustus',
-        'SEP': 'september',
-        'OCT': 'oktober',
-        'NOV': 'november',
-        'DEC': 'december'
-    }
-    
-    prepositions = {
-        'on': 'op',
-        'in': 'in',
-        'at': 'te'
-    }
-    
-    participles = {
-        'born': 'geboren',
-        'baptised': 'gedoopt',
-        'died': 'gestorven',
-        'buried': 'begraven',
-        'Married': 'Getrouwd'
-    }
-    
-
-class English:
-
-    link_text_start_page = "Start page"
-    link_text_name_index = "Name index"
-    link_text_about_page = "About"
-
-    header_pedigree = "Ancestors"
-    header_children = "Children"
-    header_parents = "Parents"
-    header_siblings = "Siblings"
-    header_spouses = "Spouses"
-    header_notes = "Notes"
-    header_name_index = "Name index"
-
-    date_unknown = "unknown"
-    person_unknown = "unknown"
-
-    default_content_about = "Now ordinary, for the nice."
-
-    date_mapping = {
-        'ABOUT': 'about',
-        'BEFORE': 'before',
-        'AFTER': 'after',
-        'BET': 'between',
-        'AND': 'and',
-        'JAN': 'January',
-        'FEB': 'February',
-        'MAR': 'March',
-        'APR': 'April',
-        'MAY': 'May',
-        'JUN': 'June',
-        'JUL': 'July',
-        'AUG': 'August',
-        'SEP': 'September',
-        'OCT': 'October',
-        'NOV': 'November',
-        'DEC': 'December'
-    }
-    
-    prepositions = {
-        'on': 'on',
-        'in': 'in',
-        'at': 'at'
-    }
-    
-    participles = {
-        'born': 'born',
-        'baptised': 'baptised',
-        'died': 'died',
-        'buried': 'buried',
-        'Married': 'Married'
-    }
-
-
-def choose(lang: str="NL") -> Language:
-    if lang == "NL":
-        return Dutch
-    elif lang == "EN":
-        return English
-    else:
-        raise ValueError("Language support only for Dutch ('NL') "
-                         "and (steenkolen-) English ('EN').")
+from typing import Protocol
+
+
+class Language(Protocol):
+
+    link_text_start_page: str
+    link_text_name_index: str
+    link_text_about_page: str
+
+    header_name_index: str
+    header_pedigree: str
+    header_children: str
+    header_parents: str
+    header_siblings: str
+    header_spouses: str
+    header_notes: str
+
+    date_unknown: str
+    person_unknown: str
+
+    default_content_about: str
+
+    date_mapping: dict
+
+    prepositions: dict
+
+    participles: dict
+
+
+class Dutch:
+
+    link_text_start_page = "Startpagina"
+    link_text_name_index = "Namenindex"
+    link_text_about_page = "About"
+
+    header_pedigree = "Voorouders"
+    header_children = "Kinderen"
+    header_parents = "Ouders"
+    header_siblings = "Broers en zussen"
+    header_spouses = "Echtgenoten"
+    header_notes = "Notities"
+    header_name_index = "Namenindex"
+    
+    date_unknown = "onbekend"
+    person_unknown = "onbekend"
+
+    default_content_about = "Nou gewoon, voor de leuk."
+
+    date_mapping = {
+        'ABOUT': 'ongeveer',
+        'BEFORE': 'vóór',
+        'AFTER': 'na',
+        'BET': 'tussen',
+        'AND': 'en',
+        'JAN': 'januari',
+        'FEB': 'februari',
+        'MAR': 'maart',
+        'APR': 'april',
+        'MAY': 'mei',
+        'JUN': 'juni',
+        'JUL': 'juli',
+        'AUG': 'augustus',
+        'SEP': 'september',
+        'OCT': 'oktober',
+        'NOV': 'november',
+        'DEC': 'december'
+    }
+    
+    prepositions = {
+        'on': 'op',
+        'in': 'in',
+        'at': 'te'
+    }
+    
+    participles = {
+        'born': 'geboren',
+        'baptised': 'gedoopt',
+        'died': 'gestorven',
+        'buried': 'begraven',
+        'Married': 'Getrouwd'
+    }
+    
+
+class English:
+
+    link_text_start_page = "Start page"
+    link_text_name_index = "Name index"
+    link_text_about_page = "About"
+
+    header_pedigree = "Ancestors"
+    header_children = "Children"
+    header_parents = "Parents"
+    header_siblings = "Siblings"
+    header_spouses = "Spouses"
+    header_notes = "Notes"
+    header_name_index = "Name index"
+
+    date_unknown = "unknown"
+    person_unknown = "unknown"
+
+    default_content_about = "Now ordinary, for the nice."
+
+    date_mapping = {
+        'ABOUT': 'about',
+        'BEFORE': 'before',
+        'AFTER': 'after',
+        'BET': 'between',
+        'AND': 'and',
+        'JAN': 'January',
+        'FEB': 'February',
+        'MAR': 'March',
+        'APR': 'April',
+        'MAY': 'May',
+        'JUN': 'June',
+        'JUL': 'July',
+        'AUG': 'August',
+        'SEP': 'September',
+        'OCT': 'October',
+        'NOV': 'November',
+        'DEC': 'December'
+    }
+    
+    prepositions = {
+        'on': 'on',
+        'in': 'in',
+        'at': 'at'
+    }
+    
+    participles = {
+        'born': 'born',
+        'baptised': 'baptised',
+        'died': 'died',
+        'buried': 'buried',
+        'Married': 'Married'
+    }
+
+
+def choose(lang: str="NL") -> Language:
+    if lang == "NL":
+        return Dutch
+    elif lang == "EN":
+        return English
+    else:
+        raise ValueError("Language support only for Dutch ('NL') "
+                         "and (steenkolen-) English ('EN').")
```

### Comparing `gedhtml-0.0.0/gedhtml/pedigree.py` & `gedhtml-0.0.1/gedhtml/pedigree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,211 +1,205 @@
 00000000: 6672 6f6d 2067 6564 6874 6d6c 2e75 7469  from gedhtml.uti
 00000010: 6c73 2069 6d70 6f72 7420 636f 6e63 6174  ls import concat
-00000020: 0d0a 0d0a 0d0a 6465 6620 5f74 656d 706c  ......def _templ
-00000030: 6174 6528 6661 6d5f 6e61 6d65 732c 206c  ate(fam_names, l
-00000040: 696e 6b73 2c20 636f 6c6f 7273 293a 0d0a  inks, colors):..
-00000050: 0d0a 2020 2020 6e61 6d65 5f73 7472 203d  ..    name_str =
-00000060: 2063 6f6e 6361 7428 5b66 2722 7b66 7d22   concat([f'"{f}"
-00000070: 2720 666f 7220 6620 696e 2066 616d 5f6e  ' for f in fam_n
-00000080: 616d 6573 5d2c 2027 2c20 2729 0d0a 2020  ames], ', ')..  
-00000090: 2020 6c69 6e6b 5f73 7472 203d 2063 6f6e    link_str = con
-000000a0: 6361 7428 5b66 2722 7b61 7d22 2720 666f  cat([f'"{a}"' fo
-000000b0: 7220 6120 696e 206c 696e 6b73 5d2c 2027  r a in links], '
-000000c0: 2c20 2729 0d0a 2020 2020 636f 6c6f 725f  , ')..    color_
-000000d0: 7374 7220 3d20 636f 6e63 6174 285b 6627  str = concat([f'
-000000e0: 227b 637d 2227 2066 6f72 2063 2069 6e20  "{c}"' for c in 
-000000f0: 636f 6c6f 7273 5d2c 2027 2c20 2729 0d0a  colors], ', ')..
-00000100: 0d0a 2020 2020 7265 7475 726e 2028 0d0a  ..    return (..
-00000110: 2020 2020 2020 2020 2720 2020 2020 2020          '       
-00000120: 2020 203c 6361 6e76 6173 2069 643d 2270     <canvas id="p
-00000130: 6564 6967 7265 6522 3e3c 2f63 616e 7661  edigree"></canva
-00000140: 733e 5c6e 270d 0a20 2020 2020 2020 2027  s>\n'..        '
-00000150: 2020 2020 2020 2020 2020 3c73 6372 6970            <scrip
-00000160: 743e 5c6e 270d 0a20 2020 2020 2020 6627  t>\n'..       f'
-00000170: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00000180: 7420 6e61 6d65 7320 3d20 5b7b 6e61 6d65  t names = [{name
-00000190: 5f73 7472 7d5d 3b5c 6e27 0d0a 2020 2020  _str}];\n'..    
-000001a0: 2020 2066 2720 2020 2020 2020 2020 2020     f'           
-000001b0: 2063 6f6e 7374 206c 696e 6b73 203d 205b   const links = [
-000001c0: 7b6c 696e 6b5f 7374 727d 5d3b 5c6e 270d  {link_str}];\n'.
-000001d0: 0a20 2020 2020 2020 6627 2020 2020 2020  .       f'      
-000001e0: 2020 2020 2020 636f 6e73 7420 636f 6c6f        const colo
-000001f0: 7273 203d 205b 7b63 6f6c 6f72 5f73 7472  rs = [{color_str
-00000200: 7d5d 3b5c 6e27 0d0a 2020 2020 2020 2066  }];\n'..       f
-00000210: 2720 2020 2020 2020 2020 2020 2064 7261  '            dra
-00000220: 7743 6861 7274 2822 7065 6469 6772 6565  wChart("pedigree
-00000230: 222c 206e 616d 6573 2c20 6c69 6e6b 732c  ", names, links,
-00000240: 2063 6f6c 6f72 7329 3b5c 6e27 0d0a 2020   colors);\n'..  
-00000250: 2020 2020 2020 2720 2020 2020 2020 2020        '         
-00000260: 203c 2f73 6372 6970 743e 5c6e 270d 0a20   </script>\n'.. 
-00000270: 2020 2020 2020 2029 0d0a 0d0a 0d0a 6465         )......de
-00000280: 6620 5f63 6f75 6e74 5f6d 6178 5f61 6e63  f _count_max_anc
-00000290: 6573 746f 7273 2866 616d 696c 795f 7472  estors(family_tr
-000002a0: 6565 2c20 7265 6629 3a0d 0a20 2020 200d  ee, ref):..    .
-000002b0: 0a20 2020 2071 7565 7565 203d 205b 6661  .    queue = [fa
-000002c0: 6d69 6c79 5f74 7265 652e 696e 6469 7669  mily_tree.indivi
-000002d0: 6475 616c 735b 7265 665d 5d0d 0a20 2020  duals[ref]]..   
-000002e0: 206d 6178 5f67 656e 203d 2030 0d0a 2020   max_gen = 0..  
-000002f0: 2020 7768 696c 6520 6c65 6e28 7175 6575    while len(queu
-00000300: 6529 203e 2030 3a0d 0a20 2020 2020 2020  e) > 0:..       
-00000310: 2071 7565 7565 5f70 6172 656e 7473 203d   queue_parents =
-00000320: 205b 5d0d 0a20 2020 2020 2020 2066 6f72   []..        for
-00000330: 2069 6e64 6976 2069 6e20 7175 6575 653a   indiv in queue:
-00000340: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
-00000350: 7265 6e74 7320 3d20 6661 6d69 6c79 5f74  rents = family_t
-00000360: 7265 652e 6765 745f 7061 7265 6e74 7328  ree.get_parents(
-00000370: 696e 6469 7629 0d0a 2020 2020 2020 2020  indiv)..        
-00000380: 2020 2020 666f 7220 7061 7265 6e74 2069      for parent i
-00000390: 6e20 7061 7265 6e74 733a 0d0a 2020 2020  n parents:..    
-000003a0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-000003b0: 6172 656e 7420 6973 206e 6f74 204e 6f6e  arent is not Non
-000003c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000003d0: 2020 2020 2020 2020 7175 6575 655f 7061          queue_pa
-000003e0: 7265 6e74 732e 6170 7065 6e64 2870 6172  rents.append(par
-000003f0: 656e 7429 0d0a 2020 2020 2020 2020 6966  ent)..        if
-00000400: 206c 656e 2871 7565 7565 5f70 6172 656e   len(queue_paren
-00000410: 7473 2920 3e20 303a 0d0a 2020 2020 2020  ts) > 0:..      
-00000420: 2020 2020 2020 6d61 785f 6765 6e20 2b3d        max_gen +=
-00000430: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00000440: 7175 6575 6520 3d20 7175 6575 655f 7061  queue = queue_pa
-00000450: 7265 6e74 735b 3a5d 0d0a 2020 2020 2020  rents[:]..      
-00000460: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00000470: 2020 2020 2071 7565 7565 203d 205b 5d0d       queue = [].
-00000480: 0a20 2020 2072 6574 7572 6e20 6d61 785f  .    return max_
-00000490: 6765 6e0d 0a0d 0a0d 0a64 6566 206d 616b  gen......def mak
-000004a0: 655f 706c 6f74 2866 616d 696c 795f 7472  e_plot(family_tr
-000004b0: 6565 2c20 7265 6629 3a0d 0a0d 0a20 2020  ee, ref):....   
-000004c0: 2069 6e64 6976 6964 7561 6c20 3d20 6661   individual = fa
-000004d0: 6d69 6c79 5f74 7265 652e 696e 6469 7669  mily_tree.indivi
-000004e0: 6475 616c 735b 7265 665d 0d0a 0d0a 2020  duals[ref]....  
-000004f0: 2020 6261 7365 5f63 6f6c 6f72 7320 3d20    base_colors = 
-00000500: 5b5b 2223 4146 4445 3433 222c 2022 2343  [["#AFDE43", "#C
-00000510: 3245 4136 3322 5d2c 0d0a 2020 2020 2020  2EA63"],..      
-00000520: 2020 2020 2020 2020 2020 2020 205b 2223               ["#
-00000530: 4439 4442 3442 222c 2022 2345 3845 4136  D9DB4B", "#E8EA6
-00000540: 3322 5d2c 0d0a 2020 2020 2020 2020 2020  3"],..          
-00000550: 2020 2020 2020 2020 205b 2223 4439 3944           ["#D99D
-00000560: 3336 222c 2022 2345 4142 3836 3322 5d2c  36", "#EAB863"],
-00000570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000580: 2020 2020 205b 2223 4439 3742 3431 222c       ["#D97B41",
-00000590: 2022 2345 4139 3736 3322 5d5d 0d0a 2020   "#EA9763"]]..  
-000005a0: 2020 6e6f 5f63 6f6c 6f72 203d 2022 7472    no_color = "tr
-000005b0: 616e 7370 6172 656e 7422 0d0a 2020 2020  ansparent"..    
-000005c0: 696e 6469 7669 6475 616c 7320 3d20 5b69  individuals = [i
-000005d0: 6e64 6976 6964 7561 6c5d 0d0a 2020 2020  ndividual]..    
-000005e0: 6e61 6d65 7320 3d20 5b5d 0d0a 2020 2020  names = []..    
-000005f0: 6c69 6e6b 7320 3d20 5b5d 0d0a 2020 2020  links = []..    
-00000600: 636f 6c6f 7273 203d 205b 5d0d 0a0d 0a20  colors = [].... 
-00000610: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00000620: 6528 3429 3a0d 0a20 2020 2020 2020 206e  e(4):..        n
-00000630: 5f70 7265 7620 3d20 322a 2a69 0d0a 2020  _prev = 2**i..  
-00000640: 2020 2020 2020 696e 6469 7669 6475 616c        individual
-00000650: 735f 7072 6576 203d 2069 6e64 6976 6964  s_prev = individ
-00000660: 7561 6c73 5b2d 6e5f 7072 6576 3a5d 0d0a  uals[-n_prev:]..
-00000670: 2020 2020 2020 2020 666f 7220 7065 7273          for pers
-00000680: 6f6e 2069 6e20 696e 6469 7669 6475 616c  on in individual
-00000690: 735f 7072 6576 3a0d 0a20 2020 2020 2020  s_prev:..       
-000006a0: 2020 2020 2069 6620 7065 7273 6f6e 2069       if person i
-000006b0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-000006c0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-000006d0: 656e 7473 203d 2066 616d 696c 795f 7472  ents = family_tr
-000006e0: 6565 2e67 6574 5f70 6172 656e 7473 2870  ee.get_parents(p
-000006f0: 6572 736f 6e29 0d0a 2020 2020 2020 2020  erson)..        
-00000700: 2020 2020 2020 2020 6966 206c 656e 2870          if len(p
-00000710: 6172 656e 7473 2920 3d3d 2032 3a0d 0a20  arents) == 2:.. 
-00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000730: 2020 2069 6e64 6976 6964 7561 6c73 202b     individuals +
-00000740: 3d20 7061 7265 6e74 730d 0a20 2020 2020  = parents..     
-00000750: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000760: 6f6c 6f72 7320 2b3d 2062 6173 655f 636f  olors += base_co
-00000770: 6c6f 7273 5b69 5d0d 0a20 2020 2020 2020  lors[i]..       
-00000780: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00000790: 6573 202b 3d20 5b70 6172 656e 7473 5b30  es += [parents[0
-000007a0: 5d2e 6e65 776c 696e 655f 6e61 6d65 2c0d  ].newline_name,.
-000007b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000007d0: 6172 656e 7473 5b31 5d2e 6e65 776c 696e  arents[1].newlin
-000007e0: 655f 6e61 6d65 5d0d 0a20 2020 2020 2020  e_name]..       
-000007f0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-00000800: 6b73 202b 3d20 5b70 6172 656e 7473 5b30  ks += [parents[0
-00000810: 5d2e 6c69 6e6b 2c20 7061 7265 6e74 735b  ].link, parents[
-00000820: 315d 2e6c 696e 6b5d 0d0a 2020 2020 2020  1].link]..      
-00000830: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
-00000840: 656e 2870 6172 656e 7473 2920 3d3d 2031  en(parents) == 1
-00000850: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000860: 2020 2020 2020 2069 6620 7061 7265 6e74         if parent
-00000870: 735b 305d 2e73 6578 203d 3d20 274d 273a  s[0].sex == 'M':
-00000880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000890: 2020 2020 2020 2020 2020 696e 6469 7669            indivi
-000008a0: 6475 616c 7320 2b3d 205b 7061 7265 6e74  duals += [parent
-000008b0: 735b 305d 2c20 4e6f 6e65 5d0d 0a20 2020  s[0], None]..   
+00000020: 0a0a 0a64 6566 205f 7465 6d70 6c61 7465  ...def _template
+00000030: 2866 616d 5f6e 616d 6573 2c20 6c69 6e6b  (fam_names, link
+00000040: 732c 2063 6f6c 6f72 7329 3a0a 0a20 2020  s, colors):..   
+00000050: 206e 616d 655f 7374 7220 3d20 636f 6e63   name_str = conc
+00000060: 6174 285b 6627 227b 667d 2227 2066 6f72  at([f'"{f}"' for
+00000070: 2066 2069 6e20 6661 6d5f 6e61 6d65 735d   f in fam_names]
+00000080: 2c20 272c 2027 290a 2020 2020 6c69 6e6b  , ', ').    link
+00000090: 5f73 7472 203d 2063 6f6e 6361 7428 5b66  _str = concat([f
+000000a0: 2722 7b61 7d22 2720 666f 7220 6120 696e  '"{a}"' for a in
+000000b0: 206c 696e 6b73 5d2c 2027 2c20 2729 0a20   links], ', '). 
+000000c0: 2020 2063 6f6c 6f72 5f73 7472 203d 2063     color_str = c
+000000d0: 6f6e 6361 7428 5b66 2722 7b63 7d22 2720  oncat([f'"{c}"' 
+000000e0: 666f 7220 6320 696e 2063 6f6c 6f72 735d  for c in colors]
+000000f0: 2c20 272c 2027 290a 0a20 2020 2072 6574  , ', ')..    ret
+00000100: 7572 6e20 280a 2020 2020 2020 2020 2720  urn (.        ' 
+00000110: 2020 2020 2020 2020 203c 6361 6e76 6173           <canvas
+00000120: 2069 643d 2270 6564 6967 7265 6522 3e3c   id="pedigree"><
+00000130: 2f63 616e 7661 733e 5c6e 270a 2020 2020  /canvas>\n'.    
+00000140: 2020 2020 2720 2020 2020 2020 2020 203c      '          <
+00000150: 7363 7269 7074 3e5c 6e27 0a20 2020 2020  script>\n'.     
+00000160: 2020 6627 2020 2020 2020 2020 2020 2020    f'            
+00000170: 636f 6e73 7420 6e61 6d65 7320 3d20 5b7b  const names = [{
+00000180: 6e61 6d65 5f73 7472 7d5d 3b5c 6e27 0a20  name_str}];\n'. 
+00000190: 2020 2020 2020 6627 2020 2020 2020 2020        f'        
+000001a0: 2020 2020 636f 6e73 7420 6c69 6e6b 7320      const links 
+000001b0: 3d20 5b7b 6c69 6e6b 5f73 7472 7d5d 3b5c  = [{link_str}];\
+000001c0: 6e27 0a20 2020 2020 2020 6627 2020 2020  n'.       f'    
+000001d0: 2020 2020 2020 2020 636f 6e73 7420 636f          const co
+000001e0: 6c6f 7273 203d 205b 7b63 6f6c 6f72 5f73  lors = [{color_s
+000001f0: 7472 7d5d 3b5c 6e27 0a20 2020 2020 2020  tr}];\n'.       
+00000200: 6627 2020 2020 2020 2020 2020 2020 6472  f'            dr
+00000210: 6177 4368 6172 7428 2270 6564 6967 7265  awChart("pedigre
+00000220: 6522 2c20 6e61 6d65 732c 206c 696e 6b73  e", names, links
+00000230: 2c20 636f 6c6f 7273 293b 5c6e 270a 2020  , colors);\n'.  
+00000240: 2020 2020 2020 2720 2020 2020 2020 2020        '         
+00000250: 203c 2f73 6372 6970 743e 5c6e 270a 2020   </script>\n'.  
+00000260: 2020 2020 2020 290a 0a0a 6465 6620 5f63        )...def _c
+00000270: 6f75 6e74 5f6d 6178 5f61 6e63 6573 746f  ount_max_ancesto
+00000280: 7273 2866 616d 696c 795f 7472 6565 2c20  rs(family_tree, 
+00000290: 7265 6629 3a0a 2020 2020 0a20 2020 2071  ref):.    .    q
+000002a0: 7565 7565 203d 205b 6661 6d69 6c79 5f74  ueue = [family_t
+000002b0: 7265 652e 696e 6469 7669 6475 616c 735b  ree.individuals[
+000002c0: 7265 665d 5d0a 2020 2020 6d61 785f 6765  ref]].    max_ge
+000002d0: 6e20 3d20 300a 2020 2020 7768 696c 6520  n = 0.    while 
+000002e0: 6c65 6e28 7175 6575 6529 203e 2030 3a0a  len(queue) > 0:.
+000002f0: 2020 2020 2020 2020 7175 6575 655f 7061          queue_pa
+00000300: 7265 6e74 7320 3d20 5b5d 0a20 2020 2020  rents = [].     
+00000310: 2020 2066 6f72 2069 6e64 6976 2069 6e20     for indiv in 
+00000320: 7175 6575 653a 0a20 2020 2020 2020 2020  queue:.         
+00000330: 2020 2070 6172 656e 7473 203d 2066 616d     parents = fam
+00000340: 696c 795f 7472 6565 2e67 6574 5f70 6172  ily_tree.get_par
+00000350: 656e 7473 2869 6e64 6976 290a 2020 2020  ents(indiv).    
+00000360: 2020 2020 2020 2020 666f 7220 7061 7265          for pare
+00000370: 6e74 2069 6e20 7061 7265 6e74 733a 0a20  nt in parents:. 
+00000380: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000390: 6620 7061 7265 6e74 2069 7320 6e6f 7420  f parent is not 
+000003a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000003b0: 2020 2020 2020 2020 2020 7175 6575 655f            queue_
+000003c0: 7061 7265 6e74 732e 6170 7065 6e64 2870  parents.append(p
+000003d0: 6172 656e 7429 0a20 2020 2020 2020 2069  arent).        i
+000003e0: 6620 6c65 6e28 7175 6575 655f 7061 7265  f len(queue_pare
+000003f0: 6e74 7329 203e 2030 3a0a 2020 2020 2020  nts) > 0:.      
+00000400: 2020 2020 2020 6d61 785f 6765 6e20 2b3d        max_gen +=
+00000410: 2031 0a20 2020 2020 2020 2020 2020 2071   1.            q
+00000420: 7565 7565 203d 2071 7565 7565 5f70 6172  ueue = queue_par
+00000430: 656e 7473 5b3a 5d0a 2020 2020 2020 2020  ents[:].        
+00000440: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00000450: 2020 7175 6575 6520 3d20 5b5d 0a20 2020    queue = [].   
+00000460: 2072 6574 7572 6e20 6d61 785f 6765 6e0a   return max_gen.
+00000470: 0a0a 6465 6620 6d61 6b65 5f70 6c6f 7428  ..def make_plot(
+00000480: 6661 6d69 6c79 5f74 7265 652c 2072 6566  family_tree, ref
+00000490: 293a 0a0a 2020 2020 696e 6469 7669 6475  ):..    individu
+000004a0: 616c 203d 2066 616d 696c 795f 7472 6565  al = family_tree
+000004b0: 2e69 6e64 6976 6964 7561 6c73 5b72 6566  .individuals[ref
+000004c0: 5d0a 0a20 2020 2062 6173 655f 636f 6c6f  ]..    base_colo
+000004d0: 7273 203d 205b 5b22 2341 4644 4534 3322  rs = [["#AFDE43"
+000004e0: 2c20 2223 4332 4541 3633 225d 2c0a 2020  , "#C2EA63"],.  
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000500: 205b 2223 4439 4442 3442 222c 2022 2345   ["#D9DB4B", "#E
+00000510: 3845 4136 3322 5d2c 0a20 2020 2020 2020  8EA63"],.       
+00000520: 2020 2020 2020 2020 2020 2020 5b22 2344              ["#D
+00000530: 3939 4433 3622 2c20 2223 4541 4238 3633  99D36", "#EAB863
+00000540: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+00000550: 2020 2020 2020 205b 2223 4439 3742 3431         ["#D97B41
+00000560: 222c 2022 2345 4139 3736 3322 5d5d 0a20  ", "#EA9763"]]. 
+00000570: 2020 206e 6f5f 636f 6c6f 7220 3d20 2274     no_color = "t
+00000580: 7261 6e73 7061 7265 6e74 220a 2020 2020  ransparent".    
+00000590: 696e 6469 7669 6475 616c 7320 3d20 5b69  individuals = [i
+000005a0: 6e64 6976 6964 7561 6c5d 0a20 2020 206e  ndividual].    n
+000005b0: 616d 6573 203d 205b 5d0a 2020 2020 6c69  ames = [].    li
+000005c0: 6e6b 7320 3d20 5b5d 0a20 2020 2063 6f6c  nks = [].    col
+000005d0: 6f72 7320 3d20 5b5d 0a0a 2020 2020 666f  ors = []..    fo
+000005e0: 7220 6920 696e 2072 616e 6765 2834 293a  r i in range(4):
+000005f0: 0a20 2020 2020 2020 206e 5f70 7265 7620  .        n_prev 
+00000600: 3d20 322a 2a69 0a20 2020 2020 2020 2069  = 2**i.        i
+00000610: 6e64 6976 6964 7561 6c73 5f70 7265 7620  ndividuals_prev 
+00000620: 3d20 696e 6469 7669 6475 616c 735b 2d6e  = individuals[-n
+00000630: 5f70 7265 763a 5d0a 2020 2020 2020 2020  _prev:].        
+00000640: 666f 7220 7065 7273 6f6e 2069 6e20 696e  for person in in
+00000650: 6469 7669 6475 616c 735f 7072 6576 3a0a  dividuals_prev:.
+00000660: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00000670: 6572 736f 6e20 6973 206e 6f74 204e 6f6e  erson is not Non
+00000680: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00000690: 2020 2070 6172 656e 7473 203d 2066 616d     parents = fam
+000006a0: 696c 795f 7472 6565 2e67 6574 5f70 6172  ily_tree.get_par
+000006b0: 656e 7473 2870 6572 736f 6e29 0a20 2020  ents(person).   
+000006c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000006d0: 6c65 6e28 7061 7265 6e74 7329 203d 3d20  len(parents) == 
+000006e0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+000006f0: 2020 2020 2020 2069 6e64 6976 6964 7561         individua
+00000700: 6c73 202b 3d20 7061 7265 6e74 730a 2020  ls += parents.  
+00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000720: 2020 636f 6c6f 7273 202b 3d20 6261 7365    colors += base
+00000730: 5f63 6f6c 6f72 735b 695d 0a20 2020 2020  _colors[i].     
+00000740: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00000750: 616d 6573 202b 3d20 5b70 6172 656e 7473  ames += [parents
+00000760: 5b30 5d2e 6e65 776c 696e 655f 6e61 6d65  [0].newline_name
+00000770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000790: 7061 7265 6e74 735b 315d 2e6e 6577 6c69  parents[1].newli
+000007a0: 6e65 5f6e 616d 655d 0a20 2020 2020 2020  ne_name].       
+000007b0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+000007c0: 6b73 202b 3d20 5b70 6172 656e 7473 5b30  ks += [parents[0
+000007d0: 5d2e 6c69 6e6b 2c20 7061 7265 6e74 735b  ].link, parents[
+000007e0: 315d 2e6c 696e 6b5d 0a20 2020 2020 2020  1].link].       
+000007f0: 2020 2020 2020 2020 2065 6c69 6620 6c65           elif le
+00000800: 6e28 7061 7265 6e74 7329 203d 3d20 313a  n(parents) == 1:
+00000810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000820: 2020 2020 2069 6620 7061 7265 6e74 735b       if parents[
+00000830: 305d 2e73 6578 203d 3d20 274d 273a 0a20  0].sex == 'M':. 
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 2020 2020 2069 6e64 6976 6964 7561         individua
+00000860: 6c73 202b 3d20 5b70 6172 656e 7473 5b30  ls += [parents[0
+00000870: 5d2c 204e 6f6e 655d 0a20 2020 2020 2020  ], None].       
+00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000890: 2063 6f6c 6f72 7320 2b3d 205b 6261 7365   colors += [base
+000008a0: 5f63 6f6c 6f72 735b 695d 5b30 5d2c 206e  _colors[i][0], n
+000008b0: 6f5f 636f 6c6f 725d 0a20 2020 2020 2020  o_color].       
 000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 2020 2063 6f6c 6f72 7320 2b3d 205b       colors += [
-000008e0: 6261 7365 5f63 6f6c 6f72 735b 695d 5b30  base_colors[i][0
-000008f0: 5d2c 206e 6f5f 636f 6c6f 725d 0d0a 2020  ], no_color]..  
+000008d0: 206e 616d 6573 202b 3d20 5b70 6172 656e   names += [paren
+000008e0: 7473 5b30 5d2e 6e65 776c 696e 655f 6e61  ts[0].newline_na
+000008f0: 6d65 2c20 2222 5d0a 2020 2020 2020 2020  me, ""].        
 00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 2020 2020 6e61 6d65 7320 2b3d 205b        names += [
-00000920: 7061 7265 6e74 735b 305d 2e6e 6577 6c69  parents[0].newli
-00000930: 6e65 5f6e 616d 652c 2022 225d 0d0a 2020  ne_name, ""]..  
-00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 2020 2020 2020 6c69 6e6b 7320 2b3d 205b        links += [
-00000960: 7061 7265 6e74 735b 305d 2e6c 696e 6b2c  parents[0].link,
-00000970: 2022 225d 0d0a 2020 2020 2020 2020 2020   ""]..          
-00000980: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00000990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009a0: 2020 2020 2020 2020 2069 6e64 6976 6964           individ
-000009b0: 7561 6c73 202b 3d20 5b4e 6f6e 652c 2070  uals += [None, p
-000009c0: 6172 656e 7473 5b30 5d5d 0d0a 2020 2020  arents[0]]..    
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2020 2020 636f 6c6f 7273 202b 3d20 5b6e      colors += [n
-000009f0: 6f5f 636f 6c6f 722c 2062 6173 655f 636f  o_color, base_co
-00000a00: 6c6f 7273 5b69 5d5b 315d 5d0d 0a20 2020  lors[i][1]]..   
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a20: 2020 2020 206e 616d 6573 202b 3d20 5b22       names += ["
-00000a30: 222c 2070 6172 656e 7473 5b30 5d2e 6e65  ", parents[0].ne
-00000a40: 776c 696e 655f 6e61 6d65 5d0d 0a20 2020  wline_name]..   
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a60: 2020 2020 206c 696e 6b73 202b 3d20 5b22       links += ["
-00000a70: 222c 2070 6172 656e 7473 5b30 5d2e 6c69  ", parents[0].li
-00000a80: 6e6b 5d0d 0a20 2020 2020 2020 2020 2020  nk]..           
-00000a90: 2020 2020 2065 6c69 6620 6c65 6e28 7061       elif len(pa
-00000aa0: 7265 6e74 7329 203d 3d20 303a 0d0a 2020  rents) == 0:..  
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ac0: 2020 696e 6469 7669 6475 616c 7320 2b3d    individuals +=
-00000ad0: 205b 4e6f 6e65 2c20 4e6f 6e65 5d0d 0a20   [None, None].. 
-00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 2020 2063 6f6c 6f72 7320 2b3d 205b 6e6f     colors += [no
-00000b00: 5f63 6f6c 6f72 2c20 6e6f 5f63 6f6c 6f72  _color, no_color
-00000b10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00000b20: 2020 2020 2020 206e 616d 6573 202b 3d20         names += 
-00000b30: 5b22 222c 2022 225d 0d0a 2020 2020 2020  ["", ""]..      
-00000b40: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00000b50: 6e6b 7320 2b3d 205b 2222 2c20 2222 5d0d  nks += ["", ""].
-00000b60: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00000b70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000b80: 2020 2020 696e 6469 7669 6475 616c 7320      individuals 
-00000b90: 2b3d 205b 4e6f 6e65 2c20 4e6f 6e65 5d0d  += [None, None].
-00000ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bb0: 2063 6f6c 6f72 7320 2b3d 205b 6e6f 5f63   colors += [no_c
-00000bc0: 6f6c 6f72 2c20 6e6f 5f63 6f6c 6f72 5d0d  olor, no_color].
-00000bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000be0: 206e 616d 6573 202b 3d20 5b22 222c 2022   names += ["", "
-00000bf0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00000c00: 2020 2020 6c69 6e6b 7320 2b3d 205b 2222      links += [""
-00000c10: 2c20 2222 5d0d 0a0d 0a20 2020 2066 6f75  , ""]....    fou
-00000c20: 7274 685f 6765 6e20 3d20 696e 6469 7669  rth_gen = indivi
-00000c30: 6475 616c 735b 2d31 363a 5d0d 0a0d 0a20  duals[-16:].... 
-00000c40: 2020 2066 6f72 2069 2c20 696e 6469 7620     for i, indiv 
-00000c50: 696e 2065 6e75 6d65 7261 7465 2866 6f75  in enumerate(fou
-00000c60: 7274 685f 6765 6e29 3a0d 0a20 2020 2020  rth_gen):..     
-00000c70: 2020 2069 6620 696e 6469 7620 6973 206e     if indiv is n
-00000c80: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00000c90: 2020 2020 2020 6d61 785f 6765 6e20 3d20        max_gen = 
-00000ca0: 5f63 6f75 6e74 5f6d 6178 5f61 6e63 6573  _count_max_ances
-00000cb0: 746f 7273 2866 616d 696c 795f 7472 6565  tors(family_tree
-00000cc0: 2c20 696e 6469 762e 7265 6629 0d0a 2020  , indiv.ref)..  
-00000cd0: 2020 2020 2020 2020 2020 6e61 6d65 735b            names[
-00000ce0: 2d31 362b 695d 202b 3d20 6622 5c5c 6e28  -16+i] += f"\\n(
-00000cf0: 2b7b 6d61 785f 6765 6e7d 2922 0d0a 0d0a  +{max_gen})"....
-00000d00: 2020 2020 7265 7475 726e 205f 7465 6d70      return _temp
-00000d10: 6c61 7465 286e 616d 6573 2c20 6c69 6e6b  late(names, link
-00000d20: 732c 2063 6f6c 6f72 7329 0d0a            s, colors)..
+00000910: 6c69 6e6b 7320 2b3d 205b 7061 7265 6e74  links += [parent
+00000920: 735b 305d 2e6c 696e 6b2c 2022 225d 0a20  s[0].link, ""]. 
+00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000940: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000960: 2069 6e64 6976 6964 7561 6c73 202b 3d20   individuals += 
+00000970: 5b4e 6f6e 652c 2070 6172 656e 7473 5b30  [None, parents[0
+00000980: 5d5d 0a20 2020 2020 2020 2020 2020 2020  ]].             
+00000990: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+000009a0: 7320 2b3d 205b 6e6f 5f63 6f6c 6f72 2c20  s += [no_color, 
+000009b0: 6261 7365 5f63 6f6c 6f72 735b 695d 5b31  base_colors[i][1
+000009c0: 5d5d 0a20 2020 2020 2020 2020 2020 2020  ]].             
+000009d0: 2020 2020 2020 2020 2020 206e 616d 6573             names
+000009e0: 202b 3d20 5b22 222c 2070 6172 656e 7473   += ["", parents
+000009f0: 5b30 5d2e 6e65 776c 696e 655f 6e61 6d65  [0].newline_name
+00000a00: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00000a10: 2020 2020 2020 2020 2020 6c69 6e6b 7320            links 
+00000a20: 2b3d 205b 2222 2c20 7061 7265 6e74 735b  += ["", parents[
+00000a30: 305d 2e6c 696e 6b5d 0a20 2020 2020 2020  0].link].       
+00000a40: 2020 2020 2020 2020 2065 6c69 6620 6c65           elif le
+00000a50: 6e28 7061 7265 6e74 7329 203d 3d20 303a  n(parents) == 0:
+00000a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a70: 2020 2020 2069 6e64 6976 6964 7561 6c73       individuals
+00000a80: 202b 3d20 5b4e 6f6e 652c 204e 6f6e 655d   += [None, None]
+00000a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000aa0: 2020 2020 2063 6f6c 6f72 7320 2b3d 205b       colors += [
+00000ab0: 6e6f 5f63 6f6c 6f72 2c20 6e6f 5f63 6f6c  no_color, no_col
+00000ac0: 6f72 5d0a 2020 2020 2020 2020 2020 2020  or].            
+00000ad0: 2020 2020 2020 2020 6e61 6d65 7320 2b3d          names +=
+00000ae0: 205b 2222 2c20 2222 5d0a 2020 2020 2020   ["", ""].      
+00000af0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+00000b00: 6e6b 7320 2b3d 205b 2222 2c20 2222 5d0a  nks += ["", ""].
+00000b10: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00000b20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000b30: 2020 696e 6469 7669 6475 616c 7320 2b3d    individuals +=
+00000b40: 205b 4e6f 6e65 2c20 4e6f 6e65 5d0a 2020   [None, None].  
+00000b50: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00000b60: 6c6f 7273 202b 3d20 5b6e 6f5f 636f 6c6f  lors += [no_colo
+00000b70: 722c 206e 6f5f 636f 6c6f 725d 0a20 2020  r, no_color].   
+00000b80: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00000b90: 6573 202b 3d20 5b22 222c 2022 225d 0a20  es += ["", ""]. 
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00000bb0: 696e 6b73 202b 3d20 5b22 222c 2022 225d  inks += ["", ""]
+00000bc0: 0a0a 2020 2020 666f 7572 7468 5f67 656e  ..    fourth_gen
+00000bd0: 203d 2069 6e64 6976 6964 7561 6c73 5b2d   = individuals[-
+00000be0: 3136 3a5d 0a0a 2020 2020 666f 7220 692c  16:]..    for i,
+00000bf0: 2069 6e64 6976 2069 6e20 656e 756d 6572   indiv in enumer
+00000c00: 6174 6528 666f 7572 7468 5f67 656e 293a  ate(fourth_gen):
+00000c10: 0a20 2020 2020 2020 2069 6620 696e 6469  .        if indi
+00000c20: 7620 6973 206e 6f74 204e 6f6e 653a 0a20  v is not None:. 
+00000c30: 2020 2020 2020 2020 2020 206d 6178 5f67             max_g
+00000c40: 656e 203d 205f 636f 756e 745f 6d61 785f  en = _count_max_
+00000c50: 616e 6365 7374 6f72 7328 6661 6d69 6c79  ancestors(family
+00000c60: 5f74 7265 652c 2069 6e64 6976 2e72 6566  _tree, indiv.ref
+00000c70: 290a 2020 2020 2020 2020 2020 2020 6e61  ).            na
+00000c80: 6d65 735b 2d31 362b 695d 202b 3d20 6622  mes[-16+i] += f"
+00000c90: 5c5c 6e28 2b7b 6d61 785f 6765 6e7d 2922  \\n(+{max_gen})"
+00000ca0: 0a0a 2020 2020 7265 7475 726e 205f 7465  ..    return _te
+00000cb0: 6d70 6c61 7465 286e 616d 6573 2c20 6c69  mplate(names, li
+00000cc0: 6e6b 732c 2063 6f6c 6f72 7329 0a         nks, colors).
```

### Comparing `gedhtml-0.0.0/gedhtml/webpage.py` & `gedhtml-0.0.1/gedhtml/webpage.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-import os
-import os.path
-import shutil
-from typing import Callable
-
-from yattag import indent
-from yattag.indentation import XMLTokenError
-
-from gedhtml.describe import individual_text, marriage_text
-from gedhtml.family_tree import FamilyTree, Individual
-from gedhtml.language import Language, Dutch
-import gedhtml.html_template as template
-import gedhtml.pedigree as pedigree
-from gedhtml.utils import concat
-
-
-class _HtmlTagger:
-    """Wrap a string argument with an html tag, given by any method name.
-    Keywords will be turned into html tag attributes; if you want to use the
-    keyword 'class', use 'klass' instead, because the former is a reserved
-    word in Python.
-    
-    >>> html = _HtmlTagger()
-    >>> html.a('link text', klass='my-class', href='https://www.python.org')
-    \"<a class='my-class' href='https://www.python.org'>link text</a>\\n\"
-    """
-    def __getattr__(self, tag: str) -> Callable:
-        def wrapper(content: str, **kwargs: str) -> str:
-            attribute_text = ""
-            for key, value in kwargs.items():
-                attribute_text += f" {"class" if key == "klass" else key}='{value}'"
-            return f"<{tag}{attribute_text}>{content}</{tag}>\n"
-        return wrapper
-
-
-class _NameCounter:
-    """Group individuals in a family tree by initial and last name."""
-    
-    def __init__(self, family_tree: FamilyTree, unknown_str="unknown"):
-        self.family_tree = family_tree
-        self.unknown_str = unknown_str
-
-        # Main data structure in this class.
-        # key: initial
-        # value: dict with:
-        #     key: last name
-        #     value: list of individuals, sorted by full name
-        self._data = self._group_names()
-
-    def _group_names(self):
-
-        data = dict()
-        for individual in self.family_tree.individuals.values():
-
-            # Skip private individuals.
-            if individual.private:
-                continue
-            last_name = individual.first_last_name
-
-            # Do some filtering on last name.
-            if last_name == '':
-                add_name = self.unknown_str
-            elif not last_name[0].isalpha():
-                name_split = last_name.split(' ')
-                if len(name_split) > 1:
-                    add_name = name_split[1]
-            else:
-                add_name = last_name
-            initial = add_name[0]
-
-            # Add to data structure.
-            if initial not in data.keys():
-                data[initial] = dict()
-
-            if add_name not in data[initial].keys():
-                data[initial][add_name] = [individual]
-            else:
-                data[initial][add_name].append(individual)
-
-        # Data is complete but needs to be sorted.
-        data = dict(sorted(data.items()))  # Sort initials
-        for initial in data.keys():
-            data[initial] = dict(sorted(data[initial].items()))  # Sort last names.
-            for last_name in data[initial].keys():
-                data[initial][last_name].sort(key=lambda x: x.name)  # Sort first names.
-
-        return data
-
-    def items(self):
-        for initial, name_dict in self._data.items():
-            yield initial, name_dict
-
-    def initials(self):
-        return self._data.keys()
-
-
-def generate_individual_page(fam_tree: FamilyTree, ref: str,
-                             title="My genealogy", description="My genealogy",
-                             lang: Language=Dutch):
-
-    individual = fam_tree.individuals[ref]
-    html = _HtmlTagger()
-
-    header = html.h1(individual.name)
-    header += html.h2(individual_text(fam_tree, ref, lang, False))
-
-    content = html.h2(lang.header_pedigree)
-    content += pedigree.make_plot(fam_tree, ref)
-
-    content += html.h2(lang.header_children)
-    content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang))
-                                     for f in fam_tree.get_children(individual)]))
-
-    content += html.h2(lang.header_parents)
-    content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang))
-                                     for f in fam_tree.get_parents(individual)]))
-
-    content += html.h2(lang.header_siblings)
-    content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang))
-                                     for f in fam_tree.get_siblings(individual)]))
-
-    content += html.h2(lang.header_spouses)
-    spouses, marriages = fam_tree.get_spouses(individual)
-    if individual.private:
-        content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang))
-                                         for f in spouses]))
-    else:
-        content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang)
-                                                 + " " + marriage_text(m, lang))
-                                         for f, m in zip(spouses, marriages)]))
-
-    content += html.h2(lang.header_notes)
-    if not individual.private:
-        content += html.p(concat([note.replace('\n', '<br>')
-                                        for note in individual.notes]))
-
-    menu = template.menu(lang.link_text_start_page,
-                         lang.link_text_name_index,
-                         lang.link_text_about_page)
-    html_page = template.main(title, description, menu, header, content)
-
-    try:
-        return indent(html_page)
-    except XMLTokenError:
-        print(f"Indentation issue encountered for {individual.link}")
-        return html_page
-    
-
-def generate_name_index(fam_tree: FamilyTree, title: str, description: str,
-                        language: Language=Dutch):
-    html = _HtmlTagger()
-    name_counter = _NameCounter(fam_tree, language.person_unknown)
-
-    # Generate html for index at top of page.
-    header = html.h1(language.header_name_index)
-    initials = name_counter.initials()
-    content = html.p(
-        html.center(
-            concat([html.a(init, href=f"#{init}").rstrip() for init in initials], " - ")
-        ))
-
-    # Generate html for full list of names.
-    dunk = language.date_unknown  # Mike, I'm open! Never mind.
-    for initial, last_names in name_counter.items():
-        content += html.h2(initial, id=f"{initial}")
-        for last_name, individuals in last_names.items():
-            content += html.details(
-                html.summary(f"{last_name} ({len(individuals)})") +
-                html.p(
-                    html.ul(
-                        concat([
-                            html.li(html.a(i.name, href=i.link).rstrip() +
-                                    f" ({dunk if i.birth_year is None else i.birth_year})")
-                            for i in individuals])
-                    )
-                )
-            )
-    
-    menu = template.menu(language.link_text_start_page,
-                         language.link_text_name_index,
-                         language.link_text_about_page)
-    html_page = template.main(title, description, menu, header, content)
-
-    return indent(html_page)
-    
-
-def generate_about_page_placeholder(title: str, description: str,
-                                    language: Language=Dutch):
-    html = _HtmlTagger()
-    header = html.h1(language.link_text_about_page)
-    content = html.p(language.default_content_about)
-    menu = template.menu(language.link_text_start_page,
-                         language.link_text_name_index,
-                         language.link_text_about_page)
-    html_page = template.main(title, description, menu, header, content)
-    return indent(html_page)
-
-
-def generate(family_tree: FamilyTree, id: str, output_dir: str="", title: str="",
-             description: str="", language: Language=Dutch,
-             filter_ids: list[str] | None=None):
-
-    ref = f"@{id}@"
-    if filter_ids is None:
-        filter_refs = None
-    else:
-        filter_refs = [f"@{id}@" for id in filter_ids]
-
-    root_dir = os.path.dirname(os.path.dirname(__file__))
-    webfiles_dir = os.path.join(root_dir, 'webfiles')
-    webfiles = os.listdir(webfiles_dir)
-    for f in webfiles:
-        shutil.copy2(os.path.join(webfiles_dir, f), output_dir)
-
-    html_doc = generate_individual_page(family_tree, ref, title, description, language)
-    path_index = os.path.join(output_dir, "index.html")
-    with open(path_index, "w", encoding="utf-8") as file:
-        file.write(html_doc)
-
-    html_doc = generate_name_index(family_tree, title, description, language)
-    path_name_index = os.path.join(output_dir, "name_index.html")
-    with open(path_name_index, "w", encoding="utf-8") as file:
-        file.write(html_doc)
-
-    html_doc = generate_about_page_placeholder(title, description, language)
-    path_name_index = os.path.join(output_dir, "about.html")
-    with open(path_name_index, "w", encoding="utf-8") as file:
-        file.write(html_doc)
-
-    refs = list(family_tree.individuals.keys())
-    for ref in refs:
-        include = True
-        if filter_refs is not None:
-
-            i = family_tree.individuals[ref]
-
-            spouses, _ = family_tree.get_spouses(i)
-            children = family_tree.get_children(i)
-            siblings = family_tree.get_siblings(i)
-
-            # We want ancestors going back 4 generations,
-            # because that's how deep the pedigree chart goes.
-            ancestors: list[list[Individual]] = [[] for _ in range(4)]
-            ancestors[0] = family_tree.get_parents(i)
-            for p in range(1, 4):
-                for kid in ancestors[p-1]:
-                    ancestors[p] += family_tree.get_parents(kid)
-
-            family = [i] + children + spouses + siblings + \
-                     ancestors[0] + ancestors[1] + ancestors[2] + ancestors[3]
-            include = False
-            for fam in family:
-                if fam.ref in filter_refs:
-                    include = True
-        if include:
-            i = family_tree.individuals[ref]
-            html_doc = generate_individual_page(family_tree, ref, title, description, language)
-            path_individual = os.path.join(output_dir, i.link)
-            with open(path_individual, "w", encoding="utf-8") as file:
-                file.write(html_doc)
+import os
+import os.path
+import shutil
+from typing import Callable
+
+from yattag import indent
+from yattag.indentation import XMLTokenError
+
+from gedhtml.describe import individual_text, marriage_text
+from gedhtml.family_tree import FamilyTree, Individual
+from gedhtml.language import Language, Dutch
+import gedhtml.html_template as template
+import gedhtml.pedigree as pedigree
+from gedhtml.utils import concat
+
+
+class _HtmlTagger:
+    """Wrap a string argument with an html tag, given by any method name.
+    Keywords will be turned into html tag attributes; if you want to use the
+    keyword 'class', use 'klass' instead, because the former is a reserved
+    word in Python.
+    
+    >>> html = _HtmlTagger()
+    >>> html.a('link text', klass='my-class', href='https://www.python.org')
+    \"<a class='my-class' href='https://www.python.org'>link text</a>\\n\"
+    """
+    def __getattr__(self, tag: str) -> Callable:
+        def wrapper(content: str, **kwargs: str) -> str:
+            attribute_text = ""
+            for key, value in kwargs.items():
+                attribute_text += f" {"class" if key == "klass" else key}='{value}'"
+            return f"<{tag}{attribute_text}>{content}</{tag}>\n"
+        return wrapper
+
+
+class _NameCounter:
+    """Group individuals in a family tree by initial and last name."""
+    
+    def __init__(self, family_tree: FamilyTree, unknown_str="unknown"):
+        self.family_tree = family_tree
+        self.unknown_str = unknown_str
+
+        # Main data structure in this class.
+        # key: initial
+        # value: dict with:
+        #     key: last name
+        #     value: list of individuals, sorted by full name
+        self._data = self._group_names()
+
+    def _group_names(self):
+
+        data = dict()
+        for individual in self.family_tree.individuals.values():
+
+            # Skip private individuals.
+            if individual.private:
+                continue
+            last_name = individual.first_last_name
+
+            # Do some filtering on last name.
+            if last_name == '':
+                add_name = self.unknown_str
+            elif not last_name[0].isalpha():
+                name_split = last_name.split(' ')
+                if len(name_split) > 1:
+                    add_name = name_split[1]
+            else:
+                add_name = last_name
+            initial = add_name[0]
+
+            # Add to data structure.
+            if initial not in data.keys():
+                data[initial] = dict()
+
+            if add_name not in data[initial].keys():
+                data[initial][add_name] = [individual]
+            else:
+                data[initial][add_name].append(individual)
+
+        # Data is complete but needs to be sorted.
+        data = dict(sorted(data.items()))  # Sort initials
+        for initial in data.keys():
+            data[initial] = dict(sorted(data[initial].items()))  # Sort last names.
+            for last_name in data[initial].keys():
+                data[initial][last_name].sort(key=lambda x: x.name)  # Sort first names.
+
+        return data
+
+    def items(self):
+        for initial, name_dict in self._data.items():
+            yield initial, name_dict
+
+    def initials(self):
+        return self._data.keys()
+
+
+def generate_individual_page(fam_tree: FamilyTree, ref: str,
+                             title="My genealogy", description="My genealogy",
+                             lang: Language=Dutch):
+
+    individual = fam_tree.individuals[ref]
+    html = _HtmlTagger()
+
+    header = html.h1(individual.name)
+    header += html.h2(individual_text(fam_tree, ref, lang, False))
+
+    content = html.h2(lang.header_pedigree)
+    content += pedigree.make_plot(fam_tree, ref)
+
+    content += html.h2(lang.header_children)
+    content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang))
+                                     for f in fam_tree.get_children(individual)]))
+
+    content += html.h2(lang.header_parents)
+    content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang))
+                                     for f in fam_tree.get_parents(individual)]))
+
+    content += html.h2(lang.header_siblings)
+    content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang))
+                                     for f in fam_tree.get_siblings(individual)]))
+
+    content += html.h2(lang.header_spouses)
+    spouses, marriages = fam_tree.get_spouses(individual)
+    if individual.private:
+        content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang))
+                                         for f in spouses]))
+    else:
+        content += html.ul(concat([html.li(individual_text(fam_tree, f.ref, lang)
+                                                 + " " + marriage_text(m, lang))
+                                         for f, m in zip(spouses, marriages)]))
+
+    content += html.h2(lang.header_notes)
+    if not individual.private:
+        content += html.p(concat([note.replace('\n', '<br>')
+                                        for note in individual.notes]))
+
+    menu = template.menu(lang.link_text_start_page,
+                         lang.link_text_name_index,
+                         lang.link_text_about_page)
+    html_page = template.main(title, description, menu, header, content)
+
+    try:
+        return indent(html_page)
+    except XMLTokenError:
+        print(f"Indentation issue encountered for {individual.link}")
+        return html_page
+    
+
+def generate_name_index(fam_tree: FamilyTree, title: str, description: str,
+                        language: Language=Dutch):
+    html = _HtmlTagger()
+    name_counter = _NameCounter(fam_tree, language.person_unknown)
+
+    # Generate html for index at top of page.
+    header = html.h1(language.header_name_index)
+    initials = name_counter.initials()
+    content = html.p(
+        html.center(
+            concat([html.a(init, href=f"#{init}").rstrip() for init in initials], " - ")
+        ))
+
+    # Generate html for full list of names.
+    dunk = language.date_unknown  # Mike, I'm open! Never mind.
+    for initial, last_names in name_counter.items():
+        content += html.h2(initial, id=f"{initial}")
+        for last_name, individuals in last_names.items():
+            content += html.details(
+                html.summary(f"{last_name} ({len(individuals)})") +
+                html.p(
+                    html.ul(
+                        concat([
+                            html.li(html.a(i.name, href=i.link).rstrip() +
+                                    f" ({dunk if i.birth_year is None else i.birth_year})")
+                            for i in individuals])
+                    )
+                )
+            )
+    
+    menu = template.menu(language.link_text_start_page,
+                         language.link_text_name_index,
+                         language.link_text_about_page)
+    html_page = template.main(title, description, menu, header, content)
+
+    return indent(html_page)
+    
+
+def generate_about_page_placeholder(title: str, description: str,
+                                    language: Language=Dutch):
+    html = _HtmlTagger()
+    header = html.h1(language.link_text_about_page)
+    content = html.p(language.default_content_about)
+    menu = template.menu(language.link_text_start_page,
+                         language.link_text_name_index,
+                         language.link_text_about_page)
+    html_page = template.main(title, description, menu, header, content)
+    return indent(html_page)
+
+
+def generate(family_tree: FamilyTree, id: str, output_dir: str="", title: str="",
+             description: str="", language: Language=Dutch,
+             filter_ids: list[str] | None=None):
+
+    ref = f"@{id}@"
+    if filter_ids is None:
+        filter_refs = None
+    else:
+        filter_refs = [f"@{id}@" for id in filter_ids]
+
+    root_dir = os.path.dirname(os.path.dirname(__file__))
+    webfiles_dir = os.path.join(root_dir, 'webfiles')
+    webfiles = os.listdir(webfiles_dir)
+    for f in webfiles:
+        shutil.copy2(os.path.join(webfiles_dir, f), output_dir)
+
+    html_doc = generate_individual_page(family_tree, ref, title, description, language)
+    path_index = os.path.join(output_dir, "index.html")
+    with open(path_index, "w", encoding="utf-8") as file:
+        file.write(html_doc)
+
+    html_doc = generate_name_index(family_tree, title, description, language)
+    path_name_index = os.path.join(output_dir, "name_index.html")
+    with open(path_name_index, "w", encoding="utf-8") as file:
+        file.write(html_doc)
+
+    html_doc = generate_about_page_placeholder(title, description, language)
+    path_name_index = os.path.join(output_dir, "about.html")
+    with open(path_name_index, "w", encoding="utf-8") as file:
+        file.write(html_doc)
+
+    refs = list(family_tree.individuals.keys())
+    for ref in refs:
+        include = True
+        if filter_refs is not None:
+
+            i = family_tree.individuals[ref]
+
+            spouses, _ = family_tree.get_spouses(i)
+            children = family_tree.get_children(i)
+            siblings = family_tree.get_siblings(i)
+
+            # We want ancestors going back 4 generations,
+            # because that's how deep the pedigree chart goes.
+            ancestors: list[list[Individual]] = [[] for _ in range(4)]
+            ancestors[0] = family_tree.get_parents(i)
+            for p in range(1, 4):
+                for kid in ancestors[p-1]:
+                    ancestors[p] += family_tree.get_parents(kid)
+
+            family = [i] + children + spouses + siblings + \
+                     ancestors[0] + ancestors[1] + ancestors[2] + ancestors[3]
+            include = False
+            for fam in family:
+                if fam.ref in filter_refs:
+                    include = True
+        if include:
+            i = family_tree.individuals[ref]
+            html_doc = generate_individual_page(family_tree, ref, title, description, language)
+            path_individual = os.path.join(output_dir, i.link)
+            with open(path_individual, "w", encoding="utf-8") as file:
+                file.write(html_doc)
```

### Comparing `gedhtml-0.0.0/LICENSE` & `gedhtml-0.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 edovanveen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 edovanveen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `gedhtml-0.0.0/PKG-INFO` & `gedhtml-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gedhtml
-Version: 0.0.0
+Version: 0.0.1
 Summary: Converting GED files to static web pages.
 Author: Edo van Veen
 Author-email: edo@vanveen.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

