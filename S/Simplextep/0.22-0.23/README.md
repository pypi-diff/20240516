# Comparing `tmp/Simplextep-0.22-py3-none-any.whl.zip` & `tmp/Simplextep-0.23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9620 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    40147 b- defN 24-May-16 08:16 Simplextep/Simplextep.py
--rw-rw-rw-  2.0 fat      162 b- defN 24-May-16 08:35 Simplextep/__init__.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      316 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      555 b- defN 24-May-16 08:35 Simplextep-0.22.dist-info/RECORD
-7 files, 42373 bytes uncompressed, 8636 bytes compressed:  79.6%
+Zip file size: 10069 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    40147 b- defN 24-May-16 08:39 Simplextep/Simplextep.py
+-rw-rw-rw-  2.0 fat     1621 b- defN 24-May-16 08:39 Simplextep/__init__.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-16 08:39 Simplextep-0.23.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      316 b- defN 24-May-16 08:39 Simplextep-0.23.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:39 Simplextep-0.23.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-16 08:39 Simplextep-0.23.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      556 b- defN 24-May-16 08:39 Simplextep-0.23.dist-info/RECORD
+7 files, 43833 bytes uncompressed, 9085 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Simplextep/Simplextep.py
 Comment: 
 
 Filename: Simplextep/__init__.py
 Comment: 
 
-Filename: Simplextep-0.22.dist-info/LICENSE
+Filename: Simplextep-0.23.dist-info/LICENSE
 Comment: 
 
-Filename: Simplextep-0.22.dist-info/METADATA
+Filename: Simplextep-0.23.dist-info/METADATA
 Comment: 
 
-Filename: Simplextep-0.22.dist-info/WHEEL
+Filename: Simplextep-0.23.dist-info/WHEEL
 Comment: 
 
-Filename: Simplextep-0.22.dist-info/top_level.txt
+Filename: Simplextep-0.23.dist-info/top_level.txt
 Comment: 
 
-Filename: Simplextep-0.22.dist-info/RECORD
+Filename: Simplextep-0.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Simplextep/__init__.py

```diff
@@ -1,7 +1,48 @@
 import Simplextep
 from Simplextep import Simplextep
 from Simplextep.Simplextep import Simplex, Problem_Prepration, Dual, Me_Plot, Sensitivity_Analysis
 
+"""Examples:
+    1) Solve Simplex.
+    objective_function = [0, 2, 1]
+    constraints = [[4, 1, 1], [2, 1, -1]]
+    equality = ["ineq", "ineq"]
+    parameters = [("x1", "+"), ("x2", "+")]
+    mode = "max"
+
+
+
+    simplex = Simplex(problem=problem, number_of_dashes=15)
+    simplex.fit()
+
+    simplex.make_table(format_="github") # This line will show all the steps.
+
+    2) Solve Dual Simplex:
+    dual_problem = Dual(objective_function=objective_function, constraints=constraints, equality=equality, parameters=parameters, mode=mode)
+    dual_problem.fit()
+    simplex = Simplex(problem=dual_problem.problem)
+    simplex.fit(max_iterations=10)
+    simplex.make_table() # This line will show all the steps.
+
+    3) Simplex Analyse:
+    objective_function = [0, 5, 4.5, 6]
+    constraints = [[60, 6, 5, 8], [150, 10, 20, 10], [8, 1, 0, 0]]
+    equality = ["ineq", "ineq", "ineq"]
+    parameters = [("x1", "+"), ("x2", "+"), ("x3", "+")]
+
+    problem = Problem_Prepration(objective_function=objective_function,
+                             constraints=constraints,
+                             equality=equality,
+                             parameters=parameters,
+                             mode="max")
+
+    simplex = Simplex(problem=problem)
+    simplex.fit()
+    # simplex.make_table(format_="github")
+
+    analysis = Sensitivity_Analysis(simplex)
+    analysis.change_righthand(righthands_at_first=[0, 1, 0, 0])
+"""
```

## Comparing `Simplextep-0.22.dist-info/LICENSE` & `Simplextep-0.23.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Simplextep-0.22.dist-info/RECORD` & `Simplextep-0.23.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Simplextep/Simplextep.py,sha256=PqYgAThB7Cw0e54ZrrW9qkgXmtS01R3AO0FCO6cANZ4,40147
-Simplextep/__init__.py,sha256=3pWby11wt-R4M9HH3UTgHGyySP2jhJ_n9C-S8qLX9Us,162
-Simplextep-0.22.dist-info/LICENSE,sha256=b2VoRh9bDRx45zuP3PupJSUhXQs02fsqkTq12Zfvpgw,1090
-Simplextep-0.22.dist-info/METADATA,sha256=a9g8rLhc7kBtsIBqBzM9gwCVIyljhFgk39KcySlOBko,316
-Simplextep-0.22.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-Simplextep-0.22.dist-info/top_level.txt,sha256=cjFeBT4iM91GKp3ILfRMRHbovS0crlNrlJjUrqe07lQ,11
-Simplextep-0.22.dist-info/RECORD,,
+Simplextep/__init__.py,sha256=xG1GueloSkGwDQH4NHipmpAmMJigO6fiwlot4SuCpqQ,1621
+Simplextep-0.23.dist-info/LICENSE,sha256=b2VoRh9bDRx45zuP3PupJSUhXQs02fsqkTq12Zfvpgw,1090
+Simplextep-0.23.dist-info/METADATA,sha256=Vsio2yxA4QTbiHZPLxtejSaM92O3jY5gkcngoGKslIs,316
+Simplextep-0.23.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+Simplextep-0.23.dist-info/top_level.txt,sha256=cjFeBT4iM91GKp3ILfRMRHbovS0crlNrlJjUrqe07lQ,11
+Simplextep-0.23.dist-info/RECORD,,
```

