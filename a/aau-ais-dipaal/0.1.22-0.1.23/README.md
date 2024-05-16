# Comparing `tmp/aau_ais_dipaal-0.1.22.tar.gz` & `tmp/aau_ais_dipaal-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_ais_dipaal-0.1.22.tar", last modified: Fri May  3 12:26:08 2024, max compression
+gzip compressed data, was "aau_ais_dipaal-0.1.23.tar", last modified: Thu May 16 07:03:42 2024, max compression
```

## Comparing `aau_ais_dipaal-0.1.22.tar` & `aau_ais_dipaal-0.1.23.tar`

### file list

```diff
@@ -1,13 +1,23 @@
--rw-r--r--   0        0        0      130 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/README.md
--rw-r--r--   0        0        0      692 2024-05-03 12:26:08.257387 aau_ais_dipaal-0.1.22/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/__init__.py
--rw-r--r--   0        0        0      237 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/convert/__init__.py
--rw-r--r--   0        0        0     1161 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/convert/callsign.py
--rw-r--r--   0        0        0     1540 2024-05-03 12:25:02.814192 aau_ais_dipaal-0.1.22/src/dipaal/convert/converter.py
--rw-r--r--   0        0        0     1132 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/convert/imo.py
--rw-r--r--   0        0        0     1142 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/convert/mmsi.py
--rw-r--r--   0        0        0        0 2024-05-03 12:25:02.814192 aau_ais_dipaal-0.1.22/src/dipaal/export/__init__.py
--rw-r--r--   0        0        0     7939 2024-05-03 12:25:02.815185 aau_ais_dipaal-0.1.22/src/dipaal/export/map_exporter.py
--rw-r--r--   0        0        0     5863 2024-05-03 12:25:02.815185 aau_ais_dipaal-0.1.22/src/dipaal/export/sql_map.py
--rw-r--r--   0        0        0      389 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.22/src/dipaal/settings.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0      130 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/README.md
+-rw-r--r--   0        0        0      713 2024-05-16 07:03:42.525052 aau_ais_dipaal-0.1.23/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/__init__.py
+-rw-r--r--   0        0        0      237 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/convert/__init__.py
+-rw-r--r--   0        0        0     1161 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/convert/callsign.py
+-rw-r--r--   0        0        0     1546 2024-05-16 05:24:21.673162 aau_ais_dipaal-0.1.23/src/dipaal/convert/converter.py
+-rw-r--r--   0        0        0     1132 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/convert/imo.py
+-rw-r--r--   0        0        0     1142 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/convert/mmsi.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:25:02.814192 aau_ais_dipaal-0.1.23/src/dipaal/export/__init__.py
+-rw-r--r--   0        0        0     8050 2024-05-03 14:00:48.480144 aau_ais_dipaal-0.1.23/src/dipaal/export/map_exporter.py
+-rw-r--r--   0        0        0     6170 2024-05-16 06:59:44.399530 aau_ais_dipaal-0.1.23/src/dipaal/export/sql_map.py
+-rw-r--r--   0        0        0       52 2024-05-16 05:47:45.666615 aau_ais_dipaal-0.1.23/src/dipaal/list/__init__.py
+-rw-r--r--   0        0        0     1598 2024-05-16 06:07:58.761276 aau_ais_dipaal-0.1.23/src/dipaal/list/lister.py
+-rw-r--r--   0        0        0       50 2024-05-16 05:38:16.272469 aau_ais_dipaal-0.1.23/src/dipaal/list/sql/enc.sql
+-rw-r--r--   0        0        0        0 2024-05-16 05:27:13.493857 aau_ais_dipaal-0.1.23/src/dipaal/list/sql/ship_type.sql
+-rw-r--r--   0        0        0      124 2024-05-14 11:53:55.399670 aau_ais_dipaal-0.1.23/src/dipaal/load/__init__.py
+-rw-r--r--   0        0        0     4751 2024-05-14 19:29:40.057506 aau_ais_dipaal-0.1.23/src/dipaal/load/loader.py
+-rw-r--r--   0        0        0     2026 2024-05-14 11:53:55.400692 aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/02.load.fact_depth_50m.sql
+-rw-r--r--   0        0        0     2556 2024-05-14 11:53:55.401684 aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/04.update.confidence.fact_depth_50m.sql
+-rw-r--r--   0        0        0     1973 2024-05-14 11:53:55.402694 aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/06.load.fact_raster_confidence.sql
+-rw-r--r--   0        0        0      976 2024-05-14 12:45:57.777054 aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/08.load.fact_raster_confidence_month.sql
+-rw-r--r--   0        0        0     1118 2024-05-14 11:53:55.403671 aau_ais_dipaal-0.1.23/src/dipaal/settings.py
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.23/PKG-INFO
```

### Comparing `aau_ais_dipaal-0.1.22/pyproject.toml` & `aau_ais_dipaal-0.1.23/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "aau-ais-dipaal"
-version = "0.1.22"
+version = "0.1.23"
 description = "TODO: Add a description of your project."
 authors = [
     { name = "Mikael Vind Mikkelsen", email = "mvmi@cs.aau.dk" },
 ]
 dependencies = [
     "aau-ais-utilities==0.1.*",
     "pydantic==2.7.*",
     "pydantic-settings==2.2.*",
     "jinjasql==0.1.*",
     "jinja2==3.0.*",
+    "pandas==2.2.*",
 ]
 requires-python = "==3.12.*"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `aau_ais_dipaal-0.1.22/src/dipaal/convert/callsign.py` & `aau_ais_dipaal-0.1.23/src/dipaal/convert/callsign.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.22/src/dipaal/convert/converter.py` & `aau_ais_dipaal-0.1.23/src/dipaal/convert/converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,10 +29,10 @@
 
         result = self.connection.execute(
             sql=sql_statement,
             params={'VALUE': value}
         ).fetchone()
 
         if result is None:
-            return "No value found in the database for the given input."
+            raise KeyError(f"No {to_format} found for {from_format} {value}.")
 
         return str(result[0])
```

### Comparing `aau_ais_dipaal-0.1.22/src/dipaal/convert/imo.py` & `aau_ais_dipaal-0.1.23/src/dipaal/convert/imo.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.22/src/dipaal/convert/mmsi.py` & `aau_ais_dipaal-0.1.23/src/dipaal/convert/mmsi.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.22/src/dipaal/export/map_exporter.py` & `aau_ais_dipaal-0.1.23/src/dipaal/export/map_exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,37 +32,38 @@
     confidence: Optional[float] = None
     mobile_type: Optional[str] = None
     ship_type: Optional[str] = None
     monthly: Optional[bool] = False
 
     @staticmethod
     @field_validator("confidence")
-    def validate_confidence(value):
+    def validate_confidence(value) -> float:
         if value < 0 or value > 1:
             raise ValueError("Confidence must be between 0 and 1.")
         return value
 
     @staticmethod
     @field_validator("start_date", "end_date")
-    def validate_dates(values):
+    def validate_dates(values) -> dict:
         if values["start_date"] > values["end_date"]:
             raise ValueError("Start date must be before or equal to the end date.")
         if len(str(values["start_date"])) != 8 or len(str(values["end_date"])) != 8:
             raise ValueError("Dates must be in the format YYYYMMDD.")
         return values
 
     @staticmethod
     @field_validator("resolution")
-    def validate_resolution(value):
+    def validate_resolution(value) -> int:
         if value not in [50, 200, 1000, 5000]:
             raise ValueError("Resolution must be one of 50, 200, 1000, or 5000.")
         return value
 
 
 class MapExporter:
+    """Exporter for raster data from the DIPAAL data warehouse."""
 
     def __init__(self, engine: Engine = get_dipaal_engine(), *, export_path: Path = None) -> None:
         """Initialize the exporter with the given configuration.
 
         Args:
             export_path: The path to the directory to export the data to.
             engine: The engine to use for connecting to the data warehouse.
@@ -195,15 +196,15 @@
 
         self._get_file_path().parent.mkdir(parents=True, exist_ok=True)
 
         with open(self._get_file_path(), "wb") as file:
             file.write(result)
 
     def export(self, params: dict) -> CursorResult:
-        """Export the raw data as
+        """Export the raw data as a cursor result.
 
         Args:
             params: A dictionary of parameters to use for the export.
         """
         self.set_params(params)
 
         base_query = self.get_query()
@@ -224,8 +225,8 @@
     exporter.save_export({
         "start_date": 20220101,
         "end_date": 20220131,
         "resolution": 50,
         "raster_type": "draught",
         "enc": "Hanstholm"
     })
-    print("Exported successfully.")
+    print("Exported successfully.")
```

### Comparing `aau_ais_dipaal-0.1.22/src/dipaal/export/sql_map.py` & `aau_ais_dipaal-0.1.23/src/dipaal/export/sql_map.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,42 +12,46 @@
     FROM depth.fact_depth_50m AS fd50m
     INNER JOIN public.dim_cell_50m AS dc50m
         ON fd50m.cell_x = dc50m.x
         AND fd50m.cell_y = dc50m.y
         AND fd50m.division_id = dc50m.partition_id
     INNER JOIN public.dim_ship as ds
         ON fd50m.ship_id = ds.ship_id
-    
-    {% if mobile_type %}
+
+    {% if mobile_type or ship_type %}
     INNER JOIN public.dim_ship_type AS dst
         ON fd50m.ship_type_id = dst.ship_type_id
     {% endif %}
-    
-    WHERE fd50m.draught IS NOT NULL 
-    
+
+    WHERE fd50m.draught IS NOT NULL
+
     {% if start_date and end_date %}
     AND fd50m.date_id BETWEEN {{start_date}} AND {{end_date}}
     {% endif %}
-    
+
     {% if confidence %}
     AND fd50m.confidence_depth_01 >= {{confidence}}
     {% endif %}
-    
+
     {% if mobile_type %}
     AND dst.mobile_type = 'Class ' || {{mobile_type}}
     {% endif %}
-    
+
     {% if enc %}
     AND st_intersects(geom,
                   (SELECT st_transform(geom, 3034)
                    FROM public.enc
                    WHERE title = {{enc}}
                    AND country = 'Denmark'))
     {% endif %}
     
+    {% if ship_type %}
+    AND dst.ship_type = {{ship_type}}
+    {% endif %}
+
     GROUP BY cell_x, cell_y, geom, division_id
 ),
 
 rasters AS (
     SELECT
         ST_Union(
             ST_AsRaster(
@@ -81,42 +85,46 @@
         fd50m.division_id,
         count(*) AS cnt
     FROM depth.fact_depth_50m AS fd50m
     INNER JOIN public.dim_cell_50m AS dc50m
         ON fd50m.cell_x = dc50m.x
         AND fd50m.cell_y = dc50m.y
         AND fd50m.division_id = dc50m.partition_id
-    
-    {% if mobile_type %}
+
+    {% if mobile_type or ship_type %}
     INNER JOIN public.dim_ship_type AS dst
         ON fd50m.ship_type_id = dst.ship_type_id
     {% endif %}
-    
-    WHERE fd50m.draught IS NOT NULL 
-    
+
+    WHERE fd50m.draught IS NOT NULL
+
     {% if start_date and end_date %}
     AND fd50m.date_id BETWEEN {{start_date}} AND {{end_date}}
     {% endif %}
-    
+
     {% if confidence %}
     AND fd50m.confidence_depth_01 >= {{confidence}}
     {% endif %}
-    
+
     {% if mobile_type %}
     AND dst.mobile_type = 'Class ' || {{mobile_type}}
     {% endif %}
-    
+
     {% if enc %}
     AND st_intersects(geom,
                   (SELECT st_transform(geom, 3034)
                    FROM public.enc
                    WHERE title = {{enc}}
                    AND country = 'Denmark'))
     {% endif %}
     
+    {% if ship_type %}
+    AND dst.ship_type = {{ship_type}}
+    {% endif %}
+
     GROUP BY cell_x, cell_y, geom, division_id
 ),
 
 rasters AS (
     SELECT
         ST_Union(
             ST_AsRaster(
@@ -142,40 +150,49 @@
 
 # noinspection SqlNoDataSourceInspection
 query_draught_month = """
 SELECT st_asgdalraster(st_union(rast, 'MAX'), 'GTiff', ARRAY['COMPRESS=DEFLATE', 'NUM_THREADS=ALL_CPUS']) as tiff
 FROM (
     SELECT st_union(fr_month.rast, 'MAX') AS rast
     FROM depth.fact_raster_cfd_month AS fr_month
-    WHERE TRUE 
     
+    {% if ship_type %}
+    INNER JOIN public.dim_ship_type AS dst ON fr_month.ship_type_id = dst.ship_type_id
+    {% endif %}
+        
+    WHERE TRUE
+
     {% if confidence %}
     AND fr_month.cfd_gte = {{confidence}}
     {% endif %}
-    
+
     {% if start_month and end_month %}
     AND fr_month.month BETWEEN {{start_month}} AND {{end_month}}
     {% endif %}
-    
+
     {% if start_year and end_year %}
     AND fr_month.year BETWEEN {{start_year}} AND {{end_year}}
     {% endif %}
-    
+
     {% if enc %}
     AND st_intersects(rast,
                       (SELECT st_transform(geom, 3034)
                              FROM public.enc
                              WHERE title = {{enc}}
                              AND country = 'Denmark'))
     {% endif %}
     
+    {% if ship_type %}
+    AND dst.ship_type = {{ship_type}}
+    {% endif %}
+
 ) AS fr;
 """
 
-# TODO: Implement this query, may need to create a new table for this.
+# TODO: Implement this query.
 confidence = """
 """
 
 if __name__ == "__main__":
     from jinjasql import JinjaSql
 
     j = JinjaSql(param_style='named')
@@ -203,8 +220,7 @@
 
     query, bind_params = j.prepare_query(sql, params)
 
     result = connection.execute(sql=query, params=bind_params)
 
     for row in result.fetchall():
         print(row)
-
```

### Comparing `aau_ais_dipaal-0.1.22/PKG-INFO` & `aau_ais_dipaal-0.1.23/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: aau-ais-dipaal
-Version: 0.1.22
+Version: 0.1.23
 Summary: TODO: Add a description of your project.
 Author-Email: Mikael Vind Mikkelsen <mvmi@cs.aau.dk>
 License: MIT
 Requires-Python: ==3.12.*
 Requires-Dist: aau-ais-utilities==0.1.*
 Requires-Dist: pydantic==2.7.*
 Requires-Dist: pydantic-settings==2.2.*
 Requires-Dist: jinjasql==0.1.*
 Requires-Dist: jinja2==3.0.*
+Requires-Dist: pandas==2.2.*
 Description-Content-Type: text/markdown
 
 # Convert Package
 
 ## Overview
 
 ## Usage
```

