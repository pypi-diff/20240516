# Comparing `tmp/umlcharter-0.0.4.tar.gz` & `tmp/umlcharter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umlcharter-0.0.4.tar", last modified: Thu Apr  4 18:52:17 2024, max compression
+gzip compressed data, was "umlcharter-0.0.5.tar", last modified: Mon Apr  8 14:41:36 2024, max compression
```

## Comparing `umlcharter-0.0.4.tar` & `umlcharter-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 18:52:13.000000 umlcharter-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-04 18:52:17.279878 umlcharter-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-04 18:52:13.000000 umlcharter-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:52:17.279878 umlcharter-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-04 18:52:13.000000 umlcharter-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.275878 umlcharter-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-04 18:52:13.000000 umlcharter-0.0.4/tests/test_sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.275878 umlcharter-0.0.4/umlcharter/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/charts/sequence_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/charts/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter/generators/mermaid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/mermaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/mermaid/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/mermaid/sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter/generators/plantuml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/plantuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/plantuml/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/plantuml/sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-04 18:52:17.000000 umlcharter-0.0.4/umlcharter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-04 18:52:17.000000 umlcharter-0.0.4/umlcharter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:52:17.000000 umlcharter-0.0.4/umlcharter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 18:52:17.000000 umlcharter-0.0.4/umlcharter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.869531 umlcharter-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 14:41:33.000000 umlcharter-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-08 14:41:36.869531 umlcharter-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-08 14:41:33.000000 umlcharter-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:41:36.869531 umlcharter-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 14:41:33.000000 umlcharter-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.865530 umlcharter-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:33.000000 umlcharter-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15879 2024-04-08 14:41:33.000000 umlcharter-0.0.5/tests/test_sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.865530 umlcharter-0.0.5/umlcharter/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.869531 umlcharter-0.0.5/umlcharter/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/charts/sequence_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/charts/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.869531 umlcharter-0.0.5/umlcharter/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.869531 umlcharter-0.0.5/umlcharter/generators/d2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/d2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/d2/d2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/d2/sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.869531 umlcharter-0.0.5/umlcharter/generators/mermaid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/mermaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/mermaid/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/mermaid/sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.869531 umlcharter-0.0.5/umlcharter/generators/plantuml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/plantuml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/plantuml/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 14:41:33.000000 umlcharter-0.0.5/umlcharter/generators/plantuml/sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:36.869531 umlcharter-0.0.5/umlcharter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-08 14:41:36.000000 umlcharter-0.0.5/umlcharter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 14:41:36.000000 umlcharter-0.0.5/umlcharter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:41:36.000000 umlcharter-0.0.5/umlcharter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 14:41:36.000000 umlcharter-0.0.5/umlcharter.egg-info/top_level.txt
```

### Comparing `umlcharter-0.0.4/LICENSE` & `umlcharter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `umlcharter-0.0.4/PKG-INFO` & `umlcharter-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umlcharter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for quick diagrams creation without a need to learn new DSL
 Home-page: https://github.com/mikalaiyurkin/charter
 Author: Mikalai Yurkin
 Author-email: yurkin.mikalai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,8 +26,8 @@
 Python package for quick diagrams creation without a need to learn a new DSL.
 
 The goal of this package is to provide a tool for convenient and quick creation of the diagrams as a code
 in the popular DSLs (PlantUML, Mermaid, D2, etc) using simple python constructions.
 
 For the examples of how this package can be used and the list of exactly supported DSLs, 
 please check the documentation:
-- [Sequence Diagrams](docs/sequence_diagram/README.md)
+- [Sequence Diagrams](https://github.com/mikalaiyurkin/umlcharter/blob/master/docs/sequence_diagram/README.md)
```

### Comparing `umlcharter-0.0.4/setup.py` & `umlcharter-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `umlcharter-0.0.4/tests/test_sequence_diagram.py` & `umlcharter-0.0.5/tests/test_sequence_diagram.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from umlcharter import SequenceDiagram, Mermaid, PlantUML
+from umlcharter import SequenceDiagram, Mermaid, PlantUML, D2
 
 
 class TestSequenceDiagram:
     @pytest.mark.parametrize(
         "generator_cls,output",
         (
             (
@@ -16,14 +16,21 @@
             (
                 PlantUML,
                 """@startuml
 title: Diagram Empty
 @enduml
 """,
             ),
+            (
+                D2,
+                """title: Diagram Empty {
+shape: sequence_diagram
+}
+"""
+            )
         ),
     )
     def test_no_participants(self, generator_cls, output):
         sd = SequenceDiagram("Diagram Empty", generator_cls=generator_cls)
         assert str(sd) == output
 
     @pytest.mark.parametrize(
@@ -42,14 +49,23 @@
                 """@startuml
 title: Diagram Only Participants
 participant "First" as p1
 participant "Second" as p2
 @enduml
 """,
             ),
+            (
+                D2,
+                """title: Diagram Only Participants {
+shape: sequence_diagram
+p1: First
+p2: Second
+}
+"""
+            )
         ),
     )
     def test_only_participants(self, generator_cls, output):
         sd = SequenceDiagram("Diagram Only Participants", generator_cls=generator_cls)
         sd.participant("First")
         sd.participant("Second")
         assert str(sd) == output
@@ -148,14 +164,53 @@
 p3->p4: Go to fourth
 p4->p4: Go to self
 p4-->p3: Return to third
 p3-->p1: Return to first
 @enduml
 """,
             ),
+            (
+                D2,
+                True,
+                """title: Diagram Interaction\\nand Auto Activation {
+shape: sequence_diagram
+p1: First\\nParticipant
+p2: Second\\nParticipant
+p3: Third\\nParticipant
+p4: Fourth\\nParticipant
+p1.0 -> p2.1: Go to second
+p2.1 -> p1.0: Return to first {style.stroke-dash: 3}
+p1.2 -> p3.3: Go to third
+p3.3 -> p4.4: Go to fourth
+p4.4 -> p4.4: Go to self
+p4.4 -> p3.3: Return to third {style.stroke-dash: 3}
+p3.3 -> p1.2: Return to first {style.stroke-dash: 3}
+}
+"""
+            ),
+            (
+                D2,
+                False,
+                """title: Diagram Interaction\\nand Auto Activation {
+shape: sequence_diagram
+p1: First\\nParticipant
+p2: Second\\nParticipant
+p3: Third\\nParticipant
+p4: Fourth\\nParticipant
+p1 -> p2: Go to second
+p2 -> p1: Return to first {style.stroke-dash: 3}
+p1 -> p3: Go to third
+p3 -> p4: Go to fourth
+p4 -> p4: Go to self
+p4 -> p3: Return to third {style.stroke-dash: 3}
+p3 -> p1: Return to first {style.stroke-dash: 3}
+}
+"""
+            )
+
         ),
     )
     def test_simple_interaction_and_auto_activation(
         self, generator_cls, auto_activation, output
     ):
         sd = SequenceDiagram(
             "Diagram Interaction\nand Auto Activation",
@@ -204,14 +259,26 @@
 p2->p2: Go to self
 p2-->p1: Return to first
 deactivate p2
 deactivate p1
 @enduml
 """,
             ),
+            (
+                D2,
+                """title: Diagram Interaction and Manual Activation {
+shape: sequence_diagram
+p1: First
+p2: Second
+p1.0 -> p2.1: Go to second
+p2.1 -> p2.1: Go to self
+p2.1 -> p1.0: Return to first {style.stroke-dash: 3}
+}
+"""
+            )
         ),
     )
     def test_simple_interaction_and_manual_activation(self, generator_cls, output):
         sd = SequenceDiagram(
             "Diagram Interaction and Manual Activation",
             generator_cls=generator_cls,
             auto_activation=False,
@@ -275,14 +342,32 @@
 p2-->p1: Return to first
 deactivate p2
 deactivate p1
 end
 @enduml
 """,
             ),
+            (
+                D2,
+                """title: Diagram Interaction and Grouping {
+shape: sequence_diagram
+p1: First
+p2: Second
+p3: Third
+Group enclosing everything: {
+p1.0 -> p2.1: Go to second
+Group enclosing interaction\\nbetween second and third: {
+p2.1 -> p3.2: Go to third
+p3.2 -> p2.1: Return to second {style.stroke-dash: 3}
+}
+p2.1 -> p1.0: Return to first {style.stroke-dash: 3}
+}
+}
+"""
+            )
         ),
     )
     def test_grouping(self, generator_cls, output):
         sd = SequenceDiagram(
             "Diagram Interaction and Grouping", generator_cls=generator_cls
         )
 
@@ -335,14 +420,38 @@
 p2-->p1: Return response
 deactivate p2
 deactivate p1
 end
 @enduml
 """,
             ),
+            (
+                D2,
+                """title: Diagram Interaction and Loops {
+shape: sequence_diagram
+p1: First
+p2: Second
+LOOP Infinite loop: {
+style: {
+border-radius: 50
+fill: "#ffdfbf"
+}
+p1.0 -> p2.1: Send request to second
+LOOP Repeat\\nuntil available: {
+style: {
+border-radius: 50
+fill: "#ffdfbf"
+}
+p2.1 -> p2.1: Check internal state
+}
+p2.1 -> p1.0: Return response {style.stroke-dash: 3}
+}
+}
+"""
+            )
         ),
     )
     def test_loop(self, generator_cls, output):
         sd = SequenceDiagram(
             "Diagram Interaction and Loops", generator_cls=generator_cls
         )
 
@@ -413,14 +522,44 @@
 p3-->p1: Laugh a lot
 deactivate p3
 deactivate p1
 end
 @enduml
 """,
             ),
+            (
+                D2,
+                """title: Diagram Interaction and Conditions {
+shape: sequence_diagram
+p1: Viewer
+p2: Drama
+p3: Comedy
+p1.0 -> p1.0: What would I like to watch today?
+alt1: ALT {
+style: {
+fill: "#ffdfbf"
+}
+CASE Want a drama: {
+style: {
+fill: "#f6c5c2"
+}
+p1.1 -> p2.2: Watch drama
+p2.2 -> p1.1: Tears and sadness {style.stroke-dash: 3}
+}
+CASE Want a comedy: {
+style: {
+fill: "#f6c5c2"
+}
+p1.3 -> p3.4: Watch comedy
+p3.4 -> p1.3: Laugh a lot {style.stroke-dash: 3}
+}
+}
+}
+"""
+            )
         ),
     )
     def test_condition(self, generator_cls, output):
         sd = SequenceDiagram(
             "Diagram Interaction and Conditions",
             generator_cls=generator_cls,
             auto_activation=False,
@@ -479,14 +618,28 @@
 p2-->p1: A bad day\\nfor the Gotham :(
 deactivate p2
 deactivate p1
 note right of p1: Batman is sad now
 @enduml
 """,
             ),
+            (
+                D2,
+                """title: Diagram Interaction and Notes {
+shape: sequence_diagram
+p1: Batman
+p2: Bandit
+p1."Batman is throwing\\na batarang at the bandit"
+p1.0 -> p2.1: Pheeeeeeu!
+p2.1."Batman has missed!"
+p2.1 -> p1.0: A bad day\\nfor the Gotham :( {style.stroke-dash: 3}
+p1."Batman is sad now"
+}
+"""
+            )
         ),
     )
     def test_note(self, generator_cls, output):
         sd = SequenceDiagram(
             "Diagram Interaction and Notes",
             generator_cls,
         )
@@ -495,9 +648,8 @@
         bandit = sd.participant("Bandit")
 
         sd.note("Batman is throwing\na batarang at the bandit")
         batman.go_to(bandit, "Pheeeeeeu!")
         sd.note("Batman has missed!")
         sd.return_("A bad day\nfor the Gotham :(")
         sd.note("Batman is sad now")
-        print(sd)
         assert str(sd) == output
```

### Comparing `umlcharter-0.0.4/umlcharter/charts/sequence_diagram.py` & `umlcharter-0.0.5/umlcharter/charts/sequence_diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,9 +299,12 @@
                 self.__sequence.append(step)
         else:
             self.__sequence.append(step)
 
     def generate(self) -> str:
         return self.__generator.generate_sequence_diagram()
 
+    def __repr__(self):
+        return f"'{self.title}', {self.generator_cls.__name__}"
+
     def __str__(self):
         return self.generate()
```

### Comparing `umlcharter-0.0.4/umlcharter/generators/mermaid/sequence_diagram.py` & `umlcharter-0.0.5/umlcharter/generators/mermaid/sequence_diagram.py`

 * *Files identical despite different names*

### Comparing `umlcharter-0.0.4/umlcharter/generators/plantuml/sequence_diagram.py` & `umlcharter-0.0.5/umlcharter/generators/plantuml/sequence_diagram.py`

 * *Files identical despite different names*

### Comparing `umlcharter-0.0.4/umlcharter.egg-info/PKG-INFO` & `umlcharter-0.0.5/umlcharter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umlcharter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for quick diagrams creation without a need to learn new DSL
 Home-page: https://github.com/mikalaiyurkin/charter
 Author: Mikalai Yurkin
 Author-email: yurkin.mikalai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,8 +26,8 @@
 Python package for quick diagrams creation without a need to learn a new DSL.
 
 The goal of this package is to provide a tool for convenient and quick creation of the diagrams as a code
 in the popular DSLs (PlantUML, Mermaid, D2, etc) using simple python constructions.
 
 For the examples of how this package can be used and the list of exactly supported DSLs, 
 please check the documentation:
-- [Sequence Diagrams](docs/sequence_diagram/README.md)
+- [Sequence Diagrams](https://github.com/mikalaiyurkin/umlcharter/blob/master/docs/sequence_diagram/README.md)
```

### Comparing `umlcharter-0.0.4/umlcharter.egg-info/SOURCES.txt` & `umlcharter-0.0.5/umlcharter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,13 +9,16 @@
 umlcharter.egg-info/dependency_links.txt
 umlcharter.egg-info/top_level.txt
 umlcharter/charts/__init__.py
 umlcharter/charts/sequence_diagram.py
 umlcharter/charts/types.py
 umlcharter/generators/__init__.py
 umlcharter/generators/base.py
+umlcharter/generators/d2/__init__.py
+umlcharter/generators/d2/d2.py
+umlcharter/generators/d2/sequence_diagram.py
 umlcharter/generators/mermaid/__init__.py
 umlcharter/generators/mermaid/mermaid.py
 umlcharter/generators/mermaid/sequence_diagram.py
 umlcharter/generators/plantuml/__init__.py
 umlcharter/generators/plantuml/plantuml.py
 umlcharter/generators/plantuml/sequence_diagram.py
```

