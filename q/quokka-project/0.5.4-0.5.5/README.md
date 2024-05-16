# Comparing `tmp/quokka-project-0.5.4.tar.gz` & `tmp/quokka-project-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quokka-project-0.5.4.tar", last modified: Tue Oct 10 15:27:18 2023, max compression
+gzip compressed data, was "quokka-project-0.5.5.tar", last modified: Wed Mar 20 10:50:07 2024, max compression
```

## Comparing `quokka-project-0.5.4.tar` & `quokka-project-0.5.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 15:27:18.980186 quokka-project-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2023-10-10 15:27:17.000000 quokka-project-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2023-10-10 15:27:18.980186 quokka-project-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-10-10 15:27:17.000000 quokka-project-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 15:27:18.976186 quokka-project-0.5.4/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 15:27:18.976186 quokka-project-0.5.4/bindings/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 15:27:18.976186 quokka-project-0.5.4/bindings/python/quokka/
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/addresser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 15:27:18.980186 quokka-project-0.5.4/bindings/python/quokka/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/analysis/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/analysis/calling_convention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/analysis/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/analysis/replacer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/analysis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 15:27:18.980186 quokka-project-0.5.4/bindings/python/quokka/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/backends/capstone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/backends/pypcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)    23300 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    18990 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/program.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25403 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/quokka_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-10-10 15:27:17.000000 quokka-project-0.5.4/bindings/python/quokka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 15:27:18.980186 quokka-project-0.5.4/bindings/python/quokka_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2023-10-10 15:27:18.000000 quokka-project-0.5.4/bindings/python/quokka_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-10-10 15:27:18.000000 quokka-project-0.5.4/bindings/python/quokka_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 15:27:18.000000 quokka-project-0.5.4/bindings/python/quokka_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-10-10 15:27:18.000000 quokka-project-0.5.4/bindings/python/quokka_project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-10 15:27:18.000000 quokka-project-0.5.4/bindings/python/quokka_project.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-10-10 15:27:17.000000 quokka-project-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-10 15:27:18.980186 quokka-project-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-10-10 15:27:17.000000 quokka-project-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:50:07.035616 quokka-project-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-03-20 10:50:04.000000 quokka-project-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-20 10:50:07.035616 quokka-project-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-20 10:50:04.000000 quokka-project-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:50:07.031616 quokka-project-0.5.5/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:50:07.031616 quokka-project-0.5.5/bindings/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:50:07.031616 quokka-project-0.5.5/bindings/python/quokka/
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/addresser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:50:07.035616 quokka-project-0.5.5/bindings/python/quokka/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/analysis/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/analysis/calling_convention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/analysis/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/analysis/replacer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/analysis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:50:07.035616 quokka-project-0.5.5/bindings/python/quokka/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/backends/capstone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/backends/pypcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23300 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18990 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25403 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/quokka_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-20 10:50:04.000000 quokka-project-0.5.5/bindings/python/quokka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:50:07.035616 quokka-project-0.5.5/bindings/python/quokka_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-20 10:50:07.000000 quokka-project-0.5.5/bindings/python/quokka_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-20 10:50:07.000000 quokka-project-0.5.5/bindings/python/quokka_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:50:07.000000 quokka-project-0.5.5/bindings/python/quokka_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-20 10:50:07.000000 quokka-project-0.5.5/bindings/python/quokka_project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 10:50:07.000000 quokka-project-0.5.5/bindings/python/quokka_project.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-20 10:50:04.000000 quokka-project-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:50:07.035616 quokka-project-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-20 10:50:04.000000 quokka-project-0.5.5/setup.py
```

### Comparing `quokka-project-0.5.4/LICENSE` & `quokka-project-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/PKG-INFO` & `quokka-project-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka-project
-Version: 0.5.4
+Version: 0.5.5
 Summary: Quokka: A Fast and Accurate Binary Exporter
 Author-email: Quarkslab <diffing@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/quokka/
 Project-URL: Repository, https://github.com/quarkslab/quokka/
 Project-URL: Documentation, https://quarkslab.github.io/quokka/
 Project-URL: Bug Tracker, https://github.com/quarkslab/quokka/issues
```

### Comparing `quokka-project-0.5.4/README.md` & `quokka-project-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/__init__.py` & `quokka-project-0.5.5/bindings/python/quokka/__init__.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/addresser.py` & `quokka-project-0.5.5/bindings/python/quokka/addresser.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/analysis/__init__.py` & `quokka-project-0.5.5/bindings/python/quokka/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/analysis/arch.py` & `quokka-project-0.5.5/bindings/python/quokka/analysis/arch.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/analysis/calling_convention.py` & `quokka-project-0.5.5/bindings/python/quokka/analysis/calling_convention.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/analysis/env.py` & `quokka-project-0.5.5/bindings/python/quokka/analysis/env.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/analysis/replacer.py` & `quokka-project-0.5.5/bindings/python/quokka/analysis/replacer.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/analysis/utils.py` & `quokka-project-0.5.5/bindings/python/quokka/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/backends/__init__.py` & `quokka-project-0.5.5/bindings/python/quokka/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/backends/capstone.py` & `quokka-project-0.5.5/bindings/python/quokka/backends/capstone.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/backends/pypcode.py` & `quokka-project-0.5.5/bindings/python/quokka/backends/pypcode.py`

 * *Files 23% similar despite different names*

```diff
@@ -56,29 +56,30 @@
 
     For the moment, only the arch described in quokka.analysis are supported.
     This method is a bit slow because enum are generated by pypcode on the fly but should
     be executed only once.
 
     Arguments:
         arch: Quokka program architecture
+        endian: Architecture endianness
 
     Raises:
         PypcodeError: if the conversion for arch is not found
 
     Returns:
         A pypcode.Context instance
     """
     names: Dict[Type[quokka.analysis.arch.QuokkaArch], str] = {
         quokka.analysis.ArchX64: "x86:LE:64:default",
         quokka.analysis.ArchX86: "x86:LE:32:default",
         quokka.analysis.ArchARM: "ARM:LE:32:v8",
         quokka.analysis.ArchARM64: "AARCH64:LE:64:v8A",
         quokka.analysis.ArchARMThumb: "ARM:LE:32:v8T",
         quokka.analysis.ArchMIPS: "MIPS:LE:32:default",
-        quokka.analysis.ArchMIPS: "MIPS:LE:64:default",
+        quokka.analysis.ArchMIPS64: "MIPS:LE:64:default",
         quokka.analysis.ArchPPC: "PowerPC:LE:32:default",
         quokka.analysis.ArchPPC64: "PowerPC:LE:64:default",
     }
 
     try:
         target_id = names[arch]
     except KeyError as exc:
@@ -89,113 +90,14 @@
     if endian == Endianness.BIG_ENDIAN:
         target_id = target_id.replace(":LE:", ":BE:")
 
     pcode_arch = get_arch_from_string(target_id)
     return pypcode.Context(pcode_arch)
 
 
-def equality(self: pypcode.ContextObj, other: Any) -> bool:
-    """Check if two pypcode objets are the same
-
-    We use monkey patching to attach the equality method to other classes and rely on
-    __slots__ to check which fields to check.
-
-    Arguments:
-        self: First object
-        other: Other variable
-
-    Returns:
-        Boolean for equality
-    """
-    return isinstance(other, self.__class__) and all(
-        getattr(other, attr) == getattr(self, attr)
-        for attr in self.__slots__
-        if attr != "cobj"
-    )
-
-
-def object_hash(obj: pypcode.ContextObj) -> int:
-    """Create a hash value for a pypcode object
-
-    This allows to create set of values.
-
-    Arguments:
-        obj: Object to hash
-
-    Returns:
-        An integer for the hash
-    """
-
-    assert isinstance(obj, pypcode.ContextObj)
-    return sum(hash(getattr(obj, attr)) for attr in obj.__slots__ if attr != "cobj")
-
-
-pypcode.Varnode.__eq__ = equality
-pypcode.Varnode.__hash__ = object_hash
-
-pypcode.AddrSpace.__eq__ = equality
-pypcode.AddrSpace.__hash__ = object_hash
-
-pypcode.PcodeOp.__eq__ = equality
-pypcode.PcodeOp.__hash__ = object_hash
-
-
-def combine_instructions(
-    block: quokka.Block, translated_instructions: Sequence[pypcode.Translation]
-) -> List[pypcode.PcodeOp]:
-    """Combine instructions between the Quokka and PyPcode
-
-    Some instruction are split between IDA and Ghidra, so we have to account for it.
-    A problem for example is the support of prefixes (such LOCK) which are decoded as 2
-    instructions by Ghidra (wrong) but only 1 by IDA (correct).
-
-    Arguments:
-        block: Quokka block
-        translated_instructions: Translated instructions by Pypcode
-
-    Raises
-        PypcodeError: if the combination doesn't work
-
-    Returns:
-        A list of Pypcode statements
-    """
-    pcode_instructions: List[pypcode.PcodeOp] = []
-    translated_instructions = iter(translated_instructions)
-
-    instruction: quokka.Instruction
-    for instruction in block.instructions:
-        instruction._pcode_insts = []
-        remaining_size: int = instruction.size
-        while remaining_size > 0:
-            try:
-                pcode_inst: pypcode.Translation = next(translated_instructions)
-            except StopIteration as exc:
-                logger.error(
-                    "Disassembly discrepancy between Pypcode / IDA: missing inst"
-                )
-                raise quokka.PypcodeError(
-                    f"Decoding error for block at 0x{block.start:x}"
-                ) from exc
-
-            remaining_size -= pcode_inst.length
-            instruction._pcode_insts.extend(pcode_inst.ops)
-
-            if remaining_size < 0:
-                logger.error(
-                    "Disassembly discrepancy between Pypcode / IDA: sizes mismatch"
-                )
-                raise quokka.PypcodeError(
-                    f"Decoding error for block at 0x{block.start:x}"
-                )
-
-            pcode_instructions.extend(list(pcode_inst.ops))
-
-    return pcode_instructions
-
-
 def update_pypcode_context(program: quokka.Program, is_thumb: bool) -> pypcode.Context:
     """Return an appropriate pypcode context for the decoding
 
     For ARM architecture, if the block starts with a Thumb instruction, we must use
     a different pypcode Context.
 
     We use the boolean `is_thumb` directly to allow caching of the call here because it
@@ -242,61 +144,61 @@
         return []
 
     # Retrieve the context from the instruction
     context: pypcode.Context = update_pypcode_context(
         block.program, first_instruction.thumb
     )
 
-    # Translate
-    translation = context.translate(
-        code=block.bytes,
-        base=block.start,
-        max_inst=0,
-    )
-
-    if translation.error:
-        logger.error(translation.error.explain)
-        raise quokka.PypcodeError(f"Decoding error for block at 0x{block.start:x}")
+    try:
+        # Translate
+        translation = context.translate(
+            block.bytes,  # buf
+            block.start,  # base_address
+            0,  # max_bytes
+            0,  # max_instructions
+        )
+        return translation.ops
 
-    pcode_instructions = combine_instructions(block, translation.instructions)
-    return pcode_instructions
+    except pypcode.BadDataError as e:
+        logger.error(e)
+        raise quokka.PypcodeError(f"Decoding error for block at 0x{block.start:x} (BadDataError)")
+    except pypcode.UnimplError as e:
+        logger.error(e)
+        raise quokka.PypcodeError(f"Decoding error for block at 0x{block.start:x} (UnimplError)")
 
 
 def pypcode_decode_instruction(
     inst: quokka.Instruction,
 ) -> Sequence[pypcode.PcodeOp]:
     """Decode an instruction using Pypcode
 
     This will return the list of Pcode operations done for the instruction.
     Note that a (binary) instruction is expected to have several pcode instructions
-    associated.
+    associated. When decoding a single instruction IMARK instructions are excluded!
 
     Arguments:
         inst: Instruction to translate
 
     Raises:
         PypcodeError: if the decoding fails
 
     Returns:
         A sequence of PcodeOp
     """
 
     context: pypcode.Context = update_pypcode_context(inst.program, inst.thumb)
-    translation = context.translate(
-        code=inst.bytes,
-        base=inst.address,
-        max_inst=1,
-    )
-
-    if not translation.error:
-
-        instructions = translation.instructions
-        if len(instructions) > 1:
-            logger.warning("Mismatch of instruction size IDA/Pypcode")
-
-        instructions = list(
-            itertools.chain.from_iterable(inst.ops for inst in instructions)
+    try:
+        translation = context.translate(
+            inst.bytes,  # buf
+            inst.address,  # base_address
+            0,  # max_bytes
+            1,  # max_instructions
         )
-        return instructions
 
-    logger.error(translation.error.explain)
-    raise quokka.PypcodeError("Unable to decode instruction")
+        return [x for x in translation.ops if x.opcode != pypcode.OpCode.IMARK]
+
+    except pypcode.BadDataError as e:
+        logger.error(e)
+        raise quokka.PypcodeError(f"Unable to decode instruction (BadDataError)")
+    except pypcode.UnimplError as e:
+        logger.error(e)
+        raise quokka.PypcodeError(f"Unable to decode instruction (UnimplError)")
```

### Comparing `quokka-project-0.5.4/bindings/python/quokka/block.py` & `quokka-project-0.5.5/bindings/python/quokka/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         block_bytes = self.program.executable.read_bytes(
             offset=file_offset,
             size=self.size,
         )
 
         return block_bytes
 
-    @property
+    @cached_property
     def pcode_insts(self) -> List[pypcode.PcodeOp]:
         """Generate PCode instructions for the block
 
         This method will call the backend Pypcode and generate the instruction for the
         whole block, updating all the instruction inside the block as well.
 
         However, all instructions will from now be attached to the block itself, and not
```

### Comparing `quokka-project-0.5.4/bindings/python/quokka/data.py` & `quokka-project-0.5.5/bindings/python/quokka/data.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/exc.py` & `quokka-project-0.5.5/bindings/python/quokka/exc.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/executable.py` & `quokka-project-0.5.5/bindings/python/quokka/executable.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/function.py` & `quokka-project-0.5.5/bindings/python/quokka/function.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/instruction.py` & `quokka-project-0.5.5/bindings/python/quokka/instruction.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/program.py` & `quokka-project-0.5.5/bindings/python/quokka/program.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/quokka_pb2.py` & `quokka-project-0.5.5/bindings/python/quokka/quokka_pb2.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/reference.py` & `quokka-project-0.5.5/bindings/python/quokka/reference.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/segment.py` & `quokka-project-0.5.5/bindings/python/quokka/segment.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/structure.py` & `quokka-project-0.5.5/bindings/python/quokka/structure.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/types.py` & `quokka-project-0.5.5/bindings/python/quokka/types.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/utils.py` & `quokka-project-0.5.5/bindings/python/quokka/utils.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/bindings/python/quokka/version.py` & `quokka-project-0.5.5/bindings/python/quokka/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.5.4"
+__version__ = "0.5.5"
```

### Comparing `quokka-project-0.5.4/bindings/python/quokka_project.egg-info/PKG-INFO` & `quokka-project-0.5.5/bindings/python/quokka_project.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka-project
-Version: 0.5.4
+Version: 0.5.5
 Summary: Quokka: A Fast and Accurate Binary Exporter
 Author-email: Quarkslab <diffing@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/quokka/
 Project-URL: Repository, https://github.com/quarkslab/quokka/
 Project-URL: Documentation, https://quarkslab.github.io/quokka/
 Project-URL: Bug Tracker, https://github.com/quarkslab/quokka/issues
```

### Comparing `quokka-project-0.5.4/bindings/python/quokka_project.egg-info/SOURCES.txt` & `quokka-project-0.5.5/bindings/python/quokka_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.4/pyproject.toml` & `quokka-project-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-mock",
     "pytest-cov",
     "coverage[toml]",
-    "pypcode>=1.1.1",
+    "pypcode>=2.0.0",
 ]
-pypcode = ["pypcode>=1.1.1"]
+pypcode = ["pypcode>=2.0.0"]
 doc = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings",
     "mkdocstrings-python",
     "mkdocs-literate-nav",
     "mkdocs-git-revision-date-localized-plugin",
@@ -41,14 +41,14 @@
     "black",
     "ipython",
     "flake8",
     "flake8-black",
     "mypy",
     "mypy-protobuf",
     "nox",
-    "pypcode>=1.1.1",
+    "pypcode>=2.0.0",
 ]
 
 [tool.setuptools]
 packages = ["quokka", "quokka.analysis", "quokka.backends"]
 package-dir = { "" = "bindings/python/" }
 package-data = { "quokka" = ["*.pyi", "*.typed"] }
```

### Comparing `quokka-project-0.5.4/setup.py` & `quokka-project-0.5.5/setup.py`

 * *Files identical despite different names*

