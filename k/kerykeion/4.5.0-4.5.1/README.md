# Comparing `tmp/kerykeion-4.5.0.tar.gz` & `tmp/kerykeion-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerykeion-4.5.0.tar", max compression
+gzip compressed data, was "kerykeion-4.5.1.tar", max compression
```

## Comparing `kerykeion-4.5.0.tar` & `kerykeion-4.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.5.0/LICENSE
--rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.5.0/README.md
--rw-r--r--   0        0        0     3917 2024-05-13 20:03:16.435516 kerykeion-4.5.0/kerykeion/__init__.py
--rw-r--r--   0        0        0      293 2024-03-05 19:18:31.414757 kerykeion-4.5.0/kerykeion/aspects/__init__.py
--rw-r--r--   0        0        0     5832 2024-03-05 19:18:31.414940 kerykeion-4.5.0/kerykeion/aspects/aspects_utils.py
--rw-r--r--   0        0        0     4507 2024-03-05 19:18:31.415083 kerykeion-4.5.0/kerykeion/aspects/natal_aspects.py
--rw-r--r--   0        0        0     3993 2024-03-05 19:18:31.415179 kerykeion-4.5.0/kerykeion/aspects/synastry_aspects.py
--rw-r--r--   0        0        0    25672 2024-05-13 20:03:16.435931 kerykeion-4.5.0/kerykeion/astrological_subject.py
--rw-r--r--   0        0        0      127 2024-03-05 19:18:31.415447 kerykeion-4.5.0/kerykeion/charts/__init__.py
--rw-r--r--   0        0        0     3197 2024-03-05 19:18:31.415523 kerykeion-4.5.0/kerykeion/charts/charts_utils.py
--rwxr-xr-x   0        0        0    65295 2024-03-19 11:01:58.830365 kerykeion-4.5.0/kerykeion/charts/kerykeion_chart_svg.py
--rwxr-xr-x   0        0        0    69874 2024-03-05 19:18:31.416341 kerykeion-4.5.0/kerykeion/charts/templates/chart.xml
--rw-r--r--   0        0        0      965 2024-05-13 20:03:16.436187 kerykeion-4.5.0/kerykeion/enums.py
--rw-r--r--   0        0        0     4444 2024-03-05 19:18:31.416503 kerykeion-4.5.0/kerykeion/fetch_geonames.py
--rw-r--r--   0        0        0      205 2024-03-05 19:18:31.416620 kerykeion-4.5.0/kerykeion/kr_types/__init__.py
--rw-r--r--   0        0        0     1945 2024-03-05 19:18:31.416709 kerykeion-4.5.0/kerykeion/kr_types/chart_types.py
--rw-r--r--   0        0        0      314 2024-03-05 19:18:31.416783 kerykeion-4.5.0/kerykeion/kr_types/kerykeion_exception.py
--rw-r--r--   0        0        0     1034 2024-03-05 19:18:31.416860 kerykeion-4.5.0/kerykeion/kr_types/kr_literals.py
--rw-r--r--   0        0        0     4100 2024-05-13 20:03:16.436568 kerykeion-4.5.0/kerykeion/kr_types/kr_models.py
--rw-r--r--   0        0        0    12737 2024-03-05 19:18:31.417044 kerykeion-4.5.0/kerykeion/kr_types/settings_models.py
--rw-r--r--   0        0        0     6794 2024-03-05 19:18:31.417198 kerykeion-4.5.0/kerykeion/relationship_score.py
--rw-r--r--   0        0        0     2565 2024-03-05 19:18:31.417278 kerykeion-4.5.0/kerykeion/report.py
--rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.5.0/kerykeion/settings/__init__.py
--rw-r--r--   0        0        0     2341 2024-03-05 19:18:31.417455 kerykeion-4.5.0/kerykeion/settings/kerykeion_settings.py
--rw-r--r--   0        0        0    12282 2024-03-05 19:18:31.417645 kerykeion-4.5.0/kerykeion/settings/kr.config.json
--rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.5.0/kerykeion/sweph/README.md
--rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.5.0/kerykeion/sweph/seas_18.se1
--rw-r--r--   0        0        0     6207 2024-05-13 20:03:16.436971 kerykeion-4.5.0/kerykeion/utilities.py
--rw-r--r--   0        0        0     2354 2024-05-13 20:03:16.437302 kerykeion-4.5.0/pyproject.toml
--rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.5.1/LICENSE
+-rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.5.1/README.md
+-rw-r--r--   0        0        0     3917 2024-05-13 20:03:16.435516 kerykeion-4.5.1/kerykeion/__init__.py
+-rw-r--r--   0        0        0      293 2024-03-05 19:18:31.414757 kerykeion-4.5.1/kerykeion/aspects/__init__.py
+-rw-r--r--   0        0        0     5832 2024-03-05 19:18:31.414940 kerykeion-4.5.1/kerykeion/aspects/aspects_utils.py
+-rw-r--r--   0        0        0     4507 2024-03-05 19:18:31.415083 kerykeion-4.5.1/kerykeion/aspects/natal_aspects.py
+-rw-r--r--   0        0        0     3993 2024-03-05 19:18:31.415179 kerykeion-4.5.1/kerykeion/aspects/synastry_aspects.py
+-rw-r--r--   0        0        0    25678 2024-05-16 19:08:55.018893 kerykeion-4.5.1/kerykeion/astrological_subject.py
+-rw-r--r--   0        0        0      127 2024-03-05 19:18:31.415447 kerykeion-4.5.1/kerykeion/charts/__init__.py
+-rw-r--r--   0        0        0     3197 2024-03-05 19:18:31.415523 kerykeion-4.5.1/kerykeion/charts/charts_utils.py
+-rwxr-xr-x   0        0        0    65295 2024-03-19 11:01:58.830365 kerykeion-4.5.1/kerykeion/charts/kerykeion_chart_svg.py
+-rwxr-xr-x   0        0        0    69874 2024-03-05 19:18:31.416341 kerykeion-4.5.1/kerykeion/charts/templates/chart.xml
+-rw-r--r--   0        0        0      965 2024-05-13 20:03:16.436187 kerykeion-4.5.1/kerykeion/enums.py
+-rw-r--r--   0        0        0     4444 2024-03-05 19:18:31.416503 kerykeion-4.5.1/kerykeion/fetch_geonames.py
+-rw-r--r--   0        0        0      205 2024-03-05 19:18:31.416620 kerykeion-4.5.1/kerykeion/kr_types/__init__.py
+-rw-r--r--   0        0        0     1945 2024-03-05 19:18:31.416709 kerykeion-4.5.1/kerykeion/kr_types/chart_types.py
+-rw-r--r--   0        0        0      314 2024-03-05 19:18:31.416783 kerykeion-4.5.1/kerykeion/kr_types/kerykeion_exception.py
+-rw-r--r--   0        0        0     1034 2024-03-05 19:18:31.416860 kerykeion-4.5.1/kerykeion/kr_types/kr_literals.py
+-rw-r--r--   0        0        0     4106 2024-05-16 19:08:55.019127 kerykeion-4.5.1/kerykeion/kr_types/kr_models.py
+-rw-r--r--   0        0        0    12737 2024-03-05 19:18:31.417044 kerykeion-4.5.1/kerykeion/kr_types/settings_models.py
+-rw-r--r--   0        0        0     6794 2024-03-05 19:18:31.417198 kerykeion-4.5.1/kerykeion/relationship_score.py
+-rw-r--r--   0        0        0     2565 2024-03-05 19:18:31.417278 kerykeion-4.5.1/kerykeion/report.py
+-rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.5.1/kerykeion/settings/__init__.py
+-rw-r--r--   0        0        0     2341 2024-03-05 19:18:31.417455 kerykeion-4.5.1/kerykeion/settings/kerykeion_settings.py
+-rw-r--r--   0        0        0    12282 2024-03-05 19:18:31.417645 kerykeion-4.5.1/kerykeion/settings/kr.config.json
+-rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.5.1/kerykeion/sweph/README.md
+-rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.5.1/kerykeion/sweph/seas_18.se1
+-rw-r--r--   0        0        0     6207 2024-05-13 20:03:16.436971 kerykeion-4.5.1/kerykeion/utilities.py
+-rw-r--r--   0        0        0     2354 2024-05-16 19:08:55.019261 kerykeion-4.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.5.1/PKG-INFO
```

### Comparing `kerykeion-4.5.0/LICENSE` & `kerykeion-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/README.md` & `kerykeion-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/__init__.py` & `kerykeion-4.5.1/kerykeion/__init__.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/aspects/aspects_utils.py` & `kerykeion-4.5.1/kerykeion/aspects/aspects_utils.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/aspects/natal_aspects.py` & `kerykeion-4.5.1/kerykeion/aspects/natal_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/aspects/synastry_aspects.py` & `kerykeion-4.5.1/kerykeion/aspects/synastry_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/astrological_subject.py` & `kerykeion-4.5.1/kerykeion/astrological_subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     jupiter: KerykeionPointModel
     saturn: KerykeionPointModel
     uranus: KerykeionPointModel
     neptune: KerykeionPointModel
     pluto: KerykeionPointModel
     true_node: KerykeionPointModel
     mean_node: KerykeionPointModel
-    chiron: KerykeionPointModel | None
+    chiron: Union[KerykeionPointModel, None]
 
     # Houses
     first_house: KerykeionPointModel
     second_house: KerykeionPointModel
     third_house: KerykeionPointModel
     fourth_house: KerykeionPointModel
     fifth_house: KerykeionPointModel
```

### Comparing `kerykeion-4.5.0/kerykeion/charts/charts_utils.py` & `kerykeion-4.5.1/kerykeion/charts/charts_utils.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/charts/kerykeion_chart_svg.py` & `kerykeion-4.5.1/kerykeion/charts/kerykeion_chart_svg.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/charts/templates/chart.xml` & `kerykeion-4.5.1/kerykeion/charts/templates/chart.xml`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/enums.py` & `kerykeion-4.5.1/kerykeion/enums.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/fetch_geonames.py` & `kerykeion-4.5.1/kerykeion/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/kr_types/chart_types.py` & `kerykeion-4.5.1/kerykeion/kr_types/chart_types.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/kr_types/kr_literals.py` & `kerykeion-4.5.1/kerykeion/kr_types/kr_literals.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/kr_types/kr_models.py` & `kerykeion-4.5.1/kerykeion/kr_types/kr_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     venus: KerykeionPointModel
     mars: KerykeionPointModel
     jupiter: KerykeionPointModel
     saturn: KerykeionPointModel
     uranus: KerykeionPointModel
     neptune: KerykeionPointModel
     pluto: KerykeionPointModel
-    chiron: KerykeionPointModel | None
+    chiron: Union[KerykeionPointModel, None]
 
     # Houses
     first_house: KerykeionPointModel
     second_house: KerykeionPointModel
     third_house: KerykeionPointModel
     fourth_house: KerykeionPointModel
     fifth_house: KerykeionPointModel
```

### Comparing `kerykeion-4.5.0/kerykeion/kr_types/settings_models.py` & `kerykeion-4.5.1/kerykeion/kr_types/settings_models.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/relationship_score.py` & `kerykeion-4.5.1/kerykeion/relationship_score.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/report.py` & `kerykeion-4.5.1/kerykeion/report.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/settings/kerykeion_settings.py` & `kerykeion-4.5.1/kerykeion/settings/kerykeion_settings.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/settings/kr.config.json` & `kerykeion-4.5.1/kerykeion/settings/kr.config.json`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/sweph/seas_18.se1` & `kerykeion-4.5.1/kerykeion/sweph/seas_18.se1`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/kerykeion/utilities.py` & `kerykeion-4.5.1/kerykeion/utilities.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.0/pyproject.toml` & `kerykeion-4.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kerykeion"
-version = "4.5.0"
+version = "4.5.1"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>"]
 description = "A python library for astrology."
 license = "AGPL-3.0"
 homepage = "https://github.com/g-battaglia/kerykeion"
 repository = "https://github.com/g-battaglia/kerykeion"
 keywords = [
     "astrology",
```

### Comparing `kerykeion-4.5.0/PKG-INFO` & `kerykeion-4.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerykeion
-Version: 4.5.0
+Version: 4.5.1
 Summary: A python library for astrology.
 Home-page: https://github.com/g-battaglia/kerykeion
 License: AGPL-3.0
 Keywords: astrology,ephemeris,astrology library,birtchart,svg,zodiac,zodiac-sing,astronomical-algorithms,synastry,astrology-calculator
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kerykeion Version: 4.5.0 Summary: A python library
+Metadata-Version: 2.1 Name: kerykeion Version: 4.5.1 Summary: A python library
 for astrology. Home-page: https://github.com/g-battaglia/kerykeion License:
 AGPL-3.0 Keywords: astrology,ephemeris,astrology
 library,birtchart,svg,zodiac,zodiac-sing,astronomical-
 algorithms,synastry,astrology-calculator Author: Giacomo Battaglia Author-
 email: battaglia.giacomo@yahoo.it Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
```

