# Comparing `tmp/continuedfractions-0.12.5.tar.gz` & `tmp/continuedfractions-0.12.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.12.5.tar", last modified: Wed May 15 13:05:06 2024, max compression
+gzip compressed data, was "continuedfractions-0.12.6.tar", last modified: Thu May 16 20:08:41 2024, max compression
```

## Comparing `continuedfractions-0.12.5.tar` & `continuedfractions-0.12.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.5/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.5/LICENSE
--rw-r--r--   0        0        0     3203 2024-05-15 09:03:15.320566 continuedfractions-0.12.5/README.md
--rw-r--r--   0        0        0     3203 2024-05-15 09:03:15.320566 continuedfractions-0.12.5/README.md
--rw-r--r--   0        0        0     3506 2024-05-15 13:05:06.132645 continuedfractions-0.12.5/pyproject.toml
--rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.5/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.5/src/continuedfractions/lib.py
--rw-r--r--   0        0        0    40745 2024-05-15 08:31:34.637882 continuedfractions-0.12.5/src/continuedfractions/sequences.py
--rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.5/src/continuedfractions/utils.py
--rw-r--r--   0        0        0       23 2024-05-15 12:17:34.995308 continuedfractions-0.12.5/src/continuedfractions/version.py
--rw-r--r--   0        0        0    24187 1970-01-01 00:00:00.000000 continuedfractions-0.12.5/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.6/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.6/LICENSE
+-rw-r--r--   0        0        0     3436 2024-05-16 13:59:15.488030 continuedfractions-0.12.6/README.md
+-rw-r--r--   0        0        0     3436 2024-05-16 13:59:15.488030 continuedfractions-0.12.6/README.md
+-rw-r--r--   0        0        0     3506 2024-05-16 20:08:41.167105 continuedfractions-0.12.6/pyproject.toml
+-rw-r--r--   0        0        0    31312 2024-05-15 20:00:55.929517 continuedfractions-0.12.6/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.6/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    40762 2024-05-16 20:02:30.426192 continuedfractions-0.12.6/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.6/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-05-16 12:25:39.833527 continuedfractions-0.12.6/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24420 1970-01-01 00:00:00.000000 continuedfractions-0.12.6/PKG-INFO
```

### Comparing `continuedfractions-0.12.5/LICENSE` & `continuedfractions-0.12.6/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.5/README.md` & `continuedfractions-0.12.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,13 +29,20 @@
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
 The `continuedfractions` package is designed for:
 
 * working with (finite) continued fractions as Python objects
 * exploring their key properties, such as elements/coefficients, convergents, segments, remainders, and others
 * operating on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
-* supporting approximations and experimental computations for irrational numbers
+* supporting approximations of and experimental computations for irrational numbers
 * exploring other related objects, such as mediants, and special sequences of rational numbers such as Farey sequences
 
+Currently, it does **not** support the following features:
+
+* infinite and generalised continued fractions
+* symbolic computations
+
+These are [planned](https://github.com/sr-murthy/continuedfractions/issues) for future releases.
+
 The project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
```

#### html2text {}

```diff
@@ -31,11 +31,15 @@
 numbers](https://en.wikipedia.org/wiki/
 Continued_fraction#Best_rational_approximations). The `continuedfractions`
 package is designed for: * working with (finite) continued fractions as Python
 objects * exploring their key properties, such as elements/coefficients,
 convergents, segments, remainders, and others * operating on them as rationals
 and instances of the standard library [`fractions.Fraction`](https://
 docs.python.org/3/library/fractions.html#fractions.Fraction) class * supporting
-approximations and experimental computations for irrational numbers * exploring
-other related objects, such as mediants, and special sequences of rational
-numbers such as Farey sequences The project is [licensed](LICENSE) under the
-[Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
+approximations of and experimental computations for irrational numbers *
+exploring other related objects, such as mediants, and special sequences of
+rational numbers such as Farey sequences Currently, it does **not** support the
+following features: * infinite and generalised continued fractions * symbolic
+computations These are [planned](https://github.com/sr-murthy/
+continuedfractions/issues) for future releases. The project is [licensed]
+(LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/
+licenses/MPL-2.0).
```

### Comparing `continuedfractions-0.12.5/pyproject.toml` & `continuedfractions-0.12.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.12.5"
+version = "0.12.6"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
```

### Comparing `continuedfractions-0.12.5/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.12.6/src/continuedfractions/continuedfraction.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.5/src/continuedfractions/lib.py` & `continuedfractions-0.12.6/src/continuedfractions/lib.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.5/src/continuedfractions/sequences.py` & `continuedfractions-0.12.6/src/continuedfractions/sequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 # has the effect of caching the function for the values of ``n`` which are
 # are used below: 1 to 1000, and then 10 ^^ 4, 10 ^^ 5, 10 ^^ 6, 10 ^^ 7.
 [coprime_integers(n) for n in range(1, 1001)]
 [coprime_integers(10 ** k) for k in range(4, 8)]
 
 
 class KSRMTree:
-    """An implicit/generative tree class implementation of the Kanga-Saunders-Randall-Mitchell (KSRM) disjointed ternary tree for pairs of (positive) coprime integers.
+    """An implicit/generative class implementation of the Kanga-Saunders-Randall-Mitchell (KSRM) ternary trees for representing and generating pairs of all (positive) coprime integers.
 
     The term "KSRM trees" is the author's, and refers to the trees presented in the following papers:
 
     * Kanga, A. R. (1990). The Family Tree of Pythagorean Triplets. The Mathematical Gazette, 26(15), 15-17.
     * Mitchell, D. W. (2001). An Alternative Characterisation of All Primitive Pythagorean Triples. The Mathematical Gazette, 85(503), 273-275. https://doi.org/10.2307/3622017
     * Saunders, R., & Randall, T. (1994). The family tree of the Pythagorean triplets revisited. The Mathematical Gazette, 78(482), 190-193. https://doi.org/10.2307/3618576
```

### Comparing `continuedfractions-0.12.5/src/continuedfractions/utils.py` & `continuedfractions-0.12.6/src/continuedfractions/utils.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.5/PKG-INFO` & `continuedfractions-0.12.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.12.5
+Version: 0.12.6
 Summary: Object-oriented continued fractions with Python.
 Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
 Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
@@ -427,13 +427,20 @@
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
 The `continuedfractions` package is designed for:
 
 * working with (finite) continued fractions as Python objects
 * exploring their key properties, such as elements/coefficients, convergents, segments, remainders, and others
 * operating on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
-* supporting approximations and experimental computations for irrational numbers
+* supporting approximations of and experimental computations for irrational numbers
 * exploring other related objects, such as mediants, and special sequences of rational numbers such as Farey sequences
 
+Currently, it does **not** support the following features:
+
+* infinite and generalised continued fractions
+* symbolic computations
+
+These are [planned](https://github.com/sr-murthy/continuedfractions/issues) for future releases.
+
 The project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
```

