# Comparing `tmp/fbmc_linearisation_analysis-0.4.3.tar.gz` & `tmp/fbmc_linearisation_analysis-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbmc_linearisation_analysis-0.4.3.tar", max compression
+gzip compressed data, was "fbmc_linearisation_analysis-0.4.4.tar", max compression
```

## Comparing `fbmc_linearisation_analysis-0.4.3.tar` & `fbmc_linearisation_analysis-0.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/LICENSE
--rw-r--r--   0        0        0      472 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/__init__.py
--rw-r--r--   0        0        0       96 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/dataframe_schemas/__init__.py
--rw-r--r--   0        0        0     1177 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/dataframe_schemas/cache_db/__init__.py
--rw-r--r--   0        0        0      716 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/dataframe_schemas/cache_db/cache_db_functions.py
--rw-r--r--   0        0        0    11762 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/dataframe_schemas/schemas.py
--rw-r--r--   0        0        0     1128 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/datetime_handlers/handle_timezones.py
--rw-r--r--   0        0        0      185 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/entsoe_data/__init__.py
--rw-r--r--   0        0        0     1004 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/entsoe_data/entsoe_store_cli.py
--rw-r--r--   0        0        0    15833 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/entsoe_data/fetch_entsoe_data.py
--rw-r--r--   0        0        0       62 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/enums/__init__.py
--rw-r--r--   0        0        0     6124 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/enums/bidding_zones.py
--rw-r--r--   0        0        0      205 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/exceptions/fbmc_exceptions.py
--rw-r--r--   0        0        0      223 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/jao_data/__init__.py
--rw-r--r--   0        0        0     7252 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/jao_data/analyse_jao_data.py
--rw-r--r--   0        0        0    11497 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/jao_data/fetch_jao_data.py
--rw-r--r--   0        0        0      967 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/jao_data/jao_store_cli.py
--rw-r--r--   0        0        0      452 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_analysis/__init__.py
--rw-r--r--   0        0        0     3425 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_analysis/compute_functions.py
--rw-r--r--   0        0        0     1119 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_analysis/dataclasses.py
--rw-r--r--   0        0        0     6257 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_analysis/process_data.py
--rw-r--r--   0        0        0       63 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_error_app/__init__.py
--rw-r--r--   0        0        0    12901 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_error_app/basic_app.py
--rw-r--r--   0        0        0        0 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/plotting/__init__.py
--rw-r--r--   0        0        0    17762 2023-12-12 13:27:41.583057 fbmc_linearisation_analysis-0.4.3/fbmc_quality/plotting/flow_map.py
--rw-r--r--   0        0        0     2332 2023-12-12 13:27:41.587056 fbmc_linearisation_analysis-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 fbmc_linearisation_analysis-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/LICENSE
+-rw-r--r--   0        0        0      472 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/__init__.py
+-rw-r--r--   0        0        0       96 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/dataframe_schemas/__init__.py
+-rw-r--r--   0        0        0     1198 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/dataframe_schemas/cache_db/__init__.py
+-rw-r--r--   0        0        0      716 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/dataframe_schemas/cache_db/cache_db_functions.py
+-rw-r--r--   0        0        0    10379 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/dataframe_schemas/schemas.py
+-rw-r--r--   0        0        0     1128 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/datetime_handlers/handle_timezones.py
+-rw-r--r--   0        0        0      185 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/entsoe_data/__init__.py
+-rw-r--r--   0        0        0     1004 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/entsoe_data/entsoe_store_cli.py
+-rw-r--r--   0        0        0    15747 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/entsoe_data/fetch_entsoe_data.py
+-rw-r--r--   0        0        0       62 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/enums/__init__.py
+-rw-r--r--   0        0        0     5888 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/enums/bidding_zones.py
+-rw-r--r--   0        0        0      253 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/exceptions/fbmc_exceptions.py
+-rw-r--r--   0        0        0      223 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/jao_data/__init__.py
+-rw-r--r--   0        0        0     7252 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/jao_data/analyse_jao_data.py
+-rw-r--r--   0        0        0    12792 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/jao_data/fetch_jao_data.py
+-rw-r--r--   0        0        0      967 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/jao_data/jao_store_cli.py
+-rw-r--r--   0        0        0      480 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_analysis/__init__.py
+-rw-r--r--   0        0        0     3928 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_analysis/compute_functions.py
+-rw-r--r--   0        0        0     1119 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_analysis/dataclasses.py
+-rw-r--r--   0        0        0     6430 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_analysis/process_data.py
+-rw-r--r--   0        0        0       63 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_error_app/__init__.py
+-rw-r--r--   0        0        0    17541 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_error_app/basic_app.py
+-rw-r--r--   0        0        0        0 2024-05-16 07:44:50.407636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/plotting/__init__.py
+-rw-r--r--   0        0        0    17762 2024-05-16 07:44:50.411636 fbmc_linearisation_analysis-0.4.4/fbmc_quality/plotting/flow_map.py
+-rw-r--r--   0        0        0     2332 2024-05-16 07:44:50.411636 fbmc_linearisation_analysis-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2246 1970-01-01 00:00:00.000000 fbmc_linearisation_analysis-0.4.4/PKG-INFO
```

### Comparing `fbmc_linearisation_analysis-0.4.3/LICENSE` & `fbmc_linearisation_analysis-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/dataframe_schemas/cache_db/__init__.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/dataframe_schemas/cache_db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,7 +30,8 @@
         raise FileNotFoundError(f"No folder named {path_to_db.parent}")
 
 DB_PATH = path_to_db
 
 if multiprocessing.current_process().name == "MainProcess":
     engine = create_engine("duckdb:///" + str(DB_PATH))
     Base.metadata.create_all(engine)
+    engine.dispose()
```

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/dataframe_schemas/cache_db/cache_db_functions.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/dataframe_schemas/cache_db/cache_db_functions.py`

 * *Files identical despite different names*

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/dataframe_schemas/schemas.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/dataframe_schemas/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     # name = Column(String)
     cnec_id = Column(String)  #: Index value
     time = Column(TIMESTAMP(timezone=True))  #: Index value
     ROW_KEY = Column(String, primary_key=True)
     id = Column(Integer)  #: JAO field value
     dateTimeUtc = Column(TIMESTAMP(timezone=True))  #: JAO field value
     tso = Column(String)  #: JAO field value
+    mrId = Column(String)  #: JAO field value
+    biddingZoneFrom = Column(String)
+    biddingZoneTo = Column(String)
     cnecName = Column(String)  #: JAO field value
     cnecType = Column(String)  #: JAO field value
     cneName = Column(String)  #: JAO field value
     cneType = Column(String)  #: JAO field value
     cneStatus = Column(String)  #: JAO field value
     cneEic = Column(String)  #: JAO field value
     direction = Column(String)  #: JAO field value
@@ -46,17 +49,18 @@
     elementType = Column(String)  #: JAO field value
     fmaxType = Column(String)  #: JAO field value
     contTso = Column(String)  #: JAO field value
     contName = Column(String)  #: JAO field value
     contStatus = Column(String)  #: JAO field value
     contSubstationFrom = Column(String)  #: JAO field value
     contSubstationTo = Column(String)  #: JAO field value
+    contEic = Column(String)
     imaxMethod = Column(String)  #: JAO field value
     contingencies = Column(String)  #: JAO field value
-    presolved = Column(Boolean)  #: JAO field value
+    nonRedundant = Column(Boolean)  #: JAO field value
     significant = Column(Boolean)  #: JAO field value
     ram = Column(Float)  #: JAO field value
     minFlow = Column(Float)  #: JAO field value
     maxFlow = Column(Float)  #: JAO field value
     u = Column(Float)  #: JAO field value
     imax = Column(Float)  #: JAO field value
     fmax = Column(Float)  #: JAO field value
@@ -75,18 +79,18 @@
     ftotalLtn = Column(Float)  #: JAO field value
     fltn = Column(Float)  #: JAO field value
     DK1 = Column(Float)  #: value of bidding zone
     DK1_CO = Column(Float)  #: value of bidding zone
     DK1_DE = Column(Float)  #: value of bidding zone
     DK1_KS = Column(Float)  #: value of bidding zone
     DK1_SK = Column(Float)  #: value of bidding zone
-    DK1_ST = Column(Float)  #: value of bidding zone
+    DK1_SB = Column(Float)  #: value of bidding zone
     DK2 = Column(Float)  #: value of bidding zone
     DK2_KO = Column(Float)  #: value of bidding zone
-    DK2_ST = Column(Float)  #: value of bidding zone
+    DK2_SB = Column(Float)  #: value of bidding zone
     FI = Column(Float)  #: value of bidding zone
     FI_EL = Column(Float)  #: value of bidding zone
     FI_FS = Column(Float)  #: value of bidding zone
     NO1 = Column(Float)  #: value of bidding zone
     NO2 = Column(Float)  #: value of bidding zone
     NO2_ND = Column(Float)  #: value of bidding zone
     NO2_SK = Column(Float)  #: value of bidding zone
@@ -133,62 +137,45 @@
     tso: Series[pd.StringDtype] = pa.Field(coerce=True)  #: JAO field value
     cnecName: Series[pd.StringDtype] = pa.Field(coerce=True)  #: JAO field value
     cnecType: Series[pd.StringDtype] = pa.Field(coerce=True)  #: JAO field value
     cneName: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
     cneType: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
     cneStatus: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
     cneEic: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
-    direction: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
-    hubFrom: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
-    hubTo: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
     substationFrom: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
     substationTo: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
-    elementType: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
-    fmaxType: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
-    contTso: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
     contName: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
     contStatus: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
-    contSubstationFrom: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
-    contSubstationTo: Series[pd.StringDtype] = pa.Field(coerce=True, nullable=True)  #: JAO field value
     imaxMethod: Series[pd.StringDtype] = pa.Field(coerce=True)  #: JAO field value
     contingencies: Series[pd.StringDtype] = pa.Field(coerce=True)  #: JAO field value
-    presolved: Series[pd.BooleanDtype] = pa.Field(coerce=True)  #: JAO field value
+    nonRedundant: Series[pd.BooleanDtype] = pa.Field(coerce=True)  #: JAO field value
     significant: Series[pd.BooleanDtype] = pa.Field(coerce=True)  #: JAO field value
     ram: Series[float]  #: JAO field value
     minFlow: Series[float]  #: JAO field value
     maxFlow: Series[float]  #: JAO field value
     u: Series[float]  #: JAO field value
     imax: Series[float]  #: JAO field value
     fmax: Series[float]  #: JAO field value
     frm: Series[float]  #: JAO field value
-    frefInit: Series[float] = pa.Field(nullable=True, coerce=True)  #: JAO field value
     fnrao: Series[float]  #: JAO field value
     fref: Series[float]  #: JAO field value
-    fcore: Series[float] = pa.Field(nullable=True, coerce=True)  #: JAO field value
     fall: Series[float]  #: JAO field value
-    fuaf: Series[float] = pa.Field(nullable=True, coerce=True)  #: JAO field value
     amr: Series[float]  #: JAO field value
     aac: Series[float]  #: JAO field value
-    ltaMargin: Series[float] = pa.Field(nullable=True, coerce=True)  #: JAO field value
-    cva: Series[float] = pa.Field(nullable=True, coerce=True)  #: JAO field value
     iva: Series[float]  #: JAO field value
-    ftotalLtn: Series[float] = pa.Field(nullable=True, coerce=True)  #: JAO field value
-    fltn: Series[float] = pa.Field(nullable=True, coerce=True)  #: JAO field value
 
 
 class BiddingZones(pa.DataFrameModel):
     DK1: Optional[Series[float]] = pa.Field(nullable=True)  #: value of bidding zone
     DK1_CO: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     DK1_DE: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     DK1_KS: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     DK1_SK: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
-    DK1_ST: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     DK2: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     DK2_KO: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
-    DK2_ST: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     FI: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     FI_EL: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     FI_FS: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     NO1: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     NO2: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     NO2_ND: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
     NO2_SK: Series[float] = pa.Field(nullable=True)  #: value of bidding zone
```

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/datetime_handlers/handle_timezones.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/datetime_handlers/handle_timezones.py`

 * *Files identical despite different names*

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/entsoe_data/entsoe_store_cli.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/entsoe_data/entsoe_store_cli.py`

 * *Files identical despite different names*

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/entsoe_data/fetch_entsoe_data.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/entsoe_data/fetch_entsoe_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,14 @@
     BiddingZonesEnum.DK2_SB: (Area.DK_1, Area.DK_2),
     BiddingZonesEnum.DK2_KO: (Area.DE_LU, Area.DK_2),
     BiddingZonesEnum.DK1_SB: (Area.DK_2, Area.DK_1),
     BiddingZonesEnum.DK1_CO: (Area.NL, Area.DK_1),
     BiddingZonesEnum.DK1_DE: (Area.DE_LU, Area.DK_1),
     BiddingZonesEnum.DK1_KS: (Area.SE_3, Area.DK_1),
     BiddingZonesEnum.DK1_SK: (Area.NO_2, Area.DK_1),
-    BiddingZonesEnum.DK1_ST: (Area.DK_2, Area.DK_1),
-    BiddingZonesEnum.DK2_ST: (Area.DK_1, Area.DK_2),
 }
 
 
 def get_from_to_bz_from_name(cnecName: str) -> tuple[BiddingZonesEnum, BiddingZonesEnum] | tuple[None, None]:
     bz1, bz2 = regex_get_from_to_bz_from_name(cnecName)
     if bz1 is None or bz2 is None:
         return substring_get_from_to_bz_from_name(cnecName)
@@ -200,15 +198,15 @@
         data = data.resample("H", label="left").mean()
     return data
 
 
 def _get_cross_border_flow(
     start: pd.Timestamp, end: pd.Timestamp, area_from: Area, area_to: Area, _recurse: bool = True
 ) -> "pd.Series[float]":
-    connection = duckdb.connect(str(DB_PATH), read_only=False)
+    connection = duckdb.connect(str(DB_PATH), read_only=True)
     cached_data = None
     with suppress(duckdb.CatalogException):
         cached_data = connection.sql(
             (
                 "SELECT * FROM ENTSOE WHERE time BETWEEN "
                 f"TIMESTAMPTZ '{start.isoformat()}' AND TIMESTAMPTZ '{end.isoformat()}'"
                 f"AND area_from='{area_from.value}' AND area_to='{area_to.value}'"
@@ -224,14 +222,15 @@
         quarters = (end - start).total_seconds() // (60 * 15)
 
         if len(unique_timestamps) == hours or len(unique_timestamps) == quarters:
             return cached_retval
 
     engine = create_engine("duckdb:///" + str(DB_PATH))
     query_and_cache_data(start, end, area_from, area_to, engine)
+    engine.dispose()
 
     if not _recurse:
         raise RuntimeError("Recurse calls did not yield all data from ENTSOE - report this error to the maintainer")
     return _get_cross_border_flow(start, end, area_from, area_to, _recurse=False)
 
 
 def cast_cache_to_correct_types(cached_data: pd.DataFrame) -> "pd.Series[float]":
```

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/enums/bidding_zones.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/enums/bidding_zones.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 class BiddingZonesEnum(str, Enum):
     DK1 = "DK1"
     DK1_SB = "DK1_SB"
     DK1_CO = "DK1_CO"
     DK1_DE = "DK1_DE"
     DK1_KS = "DK1_KS"
     DK1_SK = "DK1_SK"
-    DK1_ST = "DK1_ST"
     DK2_SB = "DK2_SB"
     DK2_KO = "DK2_KO"
-    DK2_ST = "DK2_ST"
     DK2 = "DK2"
     FI = "FI"
     FI_EL = "FI_EL"
     FI_FS = "FI_FS"
     NO1 = "NO1"
     NO2 = "NO2"
     NO2_ND = "NO2_ND"
@@ -91,20 +89,14 @@
         ("Border_CNEC_DK1_SK-DK1", BiddingZonesEnum.DK1_SK),
     ],
     BiddingZonesEnum.DK2: [
         ("Border_CNEC_DK2_SB-DK2", BiddingZonesEnum.DK2_SB),
         ("Border_CNEC_DK2_KO-DK2", BiddingZonesEnum.DK2_KO),
         ("Border_CNEC_SE4-DK2", BiddingZonesEnum.SE4),
     ],
-    BiddingZonesEnum.DK2_ST: [
-        ("Border_CNEC_DK2-DK2_ST", BiddingZonesEnum.DK2),
-    ],
-    BiddingZonesEnum.DK1_ST: [
-        ("Border_CNEC_DK1-DK1_ST", BiddingZonesEnum.DK1),
-    ],
     BiddingZonesEnum.DK1_CO: [
         ("Border_CNEC_DK1-DK1_CO", BiddingZonesEnum.DK1),
     ],
     BiddingZonesEnum.DK1_DE: [
         ("Border_CNEC_DK1-DK1_DE", BiddingZonesEnum.DK1),
     ],
     BiddingZonesEnum.DK1_KS: [
```

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/jao_data/analyse_jao_data.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/jao_data/analyse_jao_data.py`

 * *Files identical despite different names*

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/jao_data/fetch_jao_data.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/jao_data/fetch_jao_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,107 @@
 import asyncio
 import hashlib
 import logging
 import uuid
 import warnings
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import Hashable, Iterable, TypeVar
 
 import aiohttp
 import duckdb
 import pandas as pd
 from pandera.typing import DataFrame
 from pytz import AmbiguousTimeError
 from sqlalchemy import Engine, create_engine
 
 from fbmc_quality.dataframe_schemas.cache_db import DB_PATH
 from fbmc_quality.dataframe_schemas.cache_db.cache_db_functions import store_df_in_table
 from fbmc_quality.dataframe_schemas.schemas import JaoData
 from fbmc_quality.datetime_handlers.handle_timezones import convert_date_to_utc_pandas
-from fbmc_quality.exceptions.fbmc_exceptions import WrongTimezoneException
+from fbmc_quality.exceptions.fbmc_exceptions import JAOLookupException, WrongTimezoneException
 
 warnings.filterwarnings(
     "ignore",
     message=".*Unverified",
 )
 
 timedata = TypeVar("timedata", pd.Timestamp, datetime)
 
 
 def create_uuid_from_string(val: str) -> str:
     hex_string = hashlib.md5(val.encode("UTF-8"), usedforsecurity=False).hexdigest()
     return str(uuid.UUID(hex=hex_string))
 
 
-async def get_ptdfs(date: timedata, session: aiohttp.ClientSession) -> dict[str, object]:
+async def get_ptdfs(date: timedata, session: aiohttp.ClientSession) -> pd.DataFrame:
     """get PTDFs from JAO, query by datetime
 
     Args:
         date (datetime): date to query the JAO by
 
     Returns:
         Dict[str, object]: HTTP payload from the API request
     """
     session.verify = False
-    date_str = date.strftime("%Y-%m-%dT%H")
 
-    url = f"https://test-publicationtool.jao.eu/nordic/api/nordic/finalComputation/index?date={date_str}%3A00%3A00.000Z&search=&skip=0"  # noqa
+    date_str = date.strftime("%Y-%m-%dT%H:%M:%S.000Z")
+    to_date_str = (date + timedelta(hours=1)).strftime("%Y-%m-%dT%H:%M:%S.000Z")
 
-    async with session.get(url=url) as response:
-        return await response.json()
+    url = "https://test-publicationtool.jao.eu/nordic/api/data/finalComputation"
+    headers = {
+        "Accept": "application/json, text/plain, */*",
+        "Accept-Encoding": "gzip, deflate, br, zstd",
+        "Accept-Language": "nb-NO,nb;q=0.9,no;q=0.8,nn;q=0.7,en-US;q=0.6,en;q=0.5",
+        "Origin": "https://test-publicationtool.jao.eu",
+        "Referer": "https://test-publicationtool.jao.eu/nordic/flowbasedDomain",
+        "Sec-Fetch-Dest": "empty",
+        "Sec-Fetch-Mode": "cors",
+        "Sec-Fetch-Site": "same-origin",
+        "X-Requested-With": "XMLHttpRequest",
+    }
+
+    data = {
+        "FromUtc": date_str,
+        "ToUtc": to_date_str,
+        "Filter": "{}",
+        "Skip": "0",
+        "Take": "0",
+    }
+
+    async with session.get(url=url, data=data, headers=headers) as response:
+        json = await response.json()
+        if json["totalRowsWithFilter"] == 0:
+            raise JAOLookupException(f"No data for {date_str} to {to_date_str}")
+        else:
+            total_num_data = json["totalRowsWithFilter"]
+
+    df = pd.DataFrame()  # type: ignore
+    args = []
+
+    for i in range(0, total_num_data, 100):
+        args.append({"FromUtc": date_str, "ToUtc": to_date_str, "Filter": "{}", "Skip": i, "Take": 100})
+
+    for arg in args:
+        async with session.get(url=url, data=arg, headers=headers) as response:
+            json = await response.json()
+            df = pd.concat([df, pd.DataFrame(json["data"])])
+    return df
 
 
 async def _fetch_jao_dataframe_from_datetime(
     date: timedata, engine: Engine, session: aiohttp.ClientSession | None = None
 ) -> DataFrame[JaoData]:
     """Fetches a dataframe representation of JAO data"""
 
     if session is None:
         async with aiohttp.ClientSession() as new_session:
-            data_from_jao = await get_ptdfs(date, new_session)
+            df = await get_ptdfs(date, new_session)
     else:
-        data_from_jao = await get_ptdfs(date, session)
+        df = await get_ptdfs(date, session)
 
-    df = pd.DataFrame(data_from_jao["data"])  # type: ignore
     df = df.loc[df[JaoData.cnecName].notnull(), :]
     df[JaoData.cnec_id] = df.apply(
         lambda row: create_uuid_from_string(row[JaoData.cnecName] + row[JaoData.contName]), axis=1
     )
     df[JaoData.time] = pd.to_datetime(df[JaoData.dateTimeUtc])
     col = df.columns.to_list()
 
@@ -90,14 +126,15 @@
     engine = create_engine("duckdb:///" + str(DB_PATH))
 
     async with aiohttp.ClientSession() as session:
         for time_point in time_points:
             results = await _fetch_jao_dataframe_from_datetime(time_point, engine, session)
             all_results.append(results)
 
+    engine.dispose()
     if all_results:
         return_frame = pd.concat(all_results)
         return return_frame  # type: ignore
     else:
         return None
 
 
@@ -120,15 +157,15 @@
 
     loop_time = dt_from_time
     time_range: list[datetime] = []
     while loop_time < (dt_to_time):
         time_range.append(loop_time)
         loop_time += pd.Timedelta(hours=1)
 
-    connection = duckdb.connect(str(DB_PATH), read_only=False)
+    connection = duckdb.connect(str(DB_PATH), read_only=True)
     try:
         cached_data = (
             connection.sql(
                 (
                     "SELECT * FROM JAO WHERE time BETWEEN"
                     f" TIMESTAMPTZ '{from_time.isoformat()}'"
                     f"AND TIMESTAMPTZ '{(to_time + pd.Timedelta(1, unit='minutes')).isoformat()}'"
```

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/jao_data/jao_store_cli.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/jao_data/jao_store_cli.py`

 * *Files identical despite different names*

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_analysis/compute_functions.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_analysis/compute_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Union
+from typing import Literal, Union
 
+import numpy as np
 import pandas as pd
 from pandera.typing import DataFrame
 
 from fbmc_quality.dataframe_schemas import CnecData, JaoData, NetPosition
 from fbmc_quality.entsoe_data.fetch_entsoe_data import resample_to_hour_and_replace
 
 
@@ -37,23 +38,32 @@
         target_net_positions (DataFrame[NetPosition]): net positions to use for the linearisation
         target_flow (pd.Series[pd.Float64Dtype]): observed flow at the given net positions
 
     Returns:
         pd.Series[pd.Float64Dtype]: linearisation error
     """
     linear_flow = compute_linearised_flow(cnec_data, target_net_positions)
+    max_flow: "pd.Series[pd.Float64Dtype]" = cnec_data[JaoData.maxFlow]
+    if max_flow.shape == linear_flow.shape:
+        linear_flow = np.minimum(max_flow.to_numpy(), linear_flow.to_numpy())
+    else:
+        lin_flow_arr = linear_flow.to_numpy()
+        max_flow_arr = np.ones_like(lin_flow_arr)
+        max_flow_arr[:] = max_flow.mean()
+        linear_flow = np.minimum(max_flow_arr, lin_flow_arr)
     rel_error = target_flow - linear_flow
     return rel_error
 
 
 def compute_cnec_vulnerability_to_err(
     cnec_data: DataFrame[CnecData],
     target_net_positions: DataFrame[NetPosition],
     target_flow: "pd.Series[pd.Float64Dtype]",
     alt_fmax: Union["pd.Series[pd.Float64Dtype]", None] = None,
+    relative_or_absolute: Literal["relative", "absolute"] = "relative",
 ) -> pd.DataFrame:
     r"""returns the mean value of the vulnerability score, and mean basecase relative margin
 
     vulnerability is the fraction of linearisation-error to the margin in MW in the target situation:
         `v = linearisation-error/(f_max - target-flow)`
 
     basecase relative margin is the
```

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_analysis/dataclasses.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_analysis/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/linearisation_analysis/process_data.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/linearisation_analysis/process_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Callable
+from typing import Callable, Iterable
 
 import numpy as np
 import pandas as pd
 from pandera.typing import DataFrame
 
 from fbmc_quality.dataframe_schemas import BiddingZones, JaoData, NetPosition
 
@@ -93,38 +93,31 @@
         fetch_cnec_data (Callable[[date, date, str], pd.DataFrame]): Callable that queries for cnec data
         jaodata_and_net_positions (JaoDataAndNPS): Data from JAO and target Net Positions
 
     Returns:
         CnecDataAndNPS | None: Data on the CNEC and with relevant net_positions
     """
     cnec_id = get_cnec_id_from_name(cnecName, jaodata_and_net_positions.jaoData)
-    cnec_ds = jaodata_and_net_positions.jaoData.xs(cnec_id, level=JaoData.cnec_id)
-
+    cnec_ds: pd.DataFrame = jaodata_and_net_positions.jaoData.xs(cnec_id, level=JaoData.cnec_id)
     times: "pd.DatetimeIndex" = jaodata_and_net_positions.jaoData.index.get_level_values("time")
     freq = pd.infer_freq(times.unique().sort_values())
     if freq is None:
         raise NoInferrableFrequency(f"Cant infer frequency from {times.unique().sort_values()}")
 
     period_dt = pd.to_timedelta("1" + freq)
     end = (times.max() + period_dt).to_pydatetime()
     start = times.min().to_pydatetime()
 
     observed_flow = fetch_cnec_data(start, end, cnecName)
     if observed_flow is None or observed_flow.empty or cnec_ds.empty:
         return None
 
-    index_alignment = pd.DatetimeIndex(
-        (
-            set(cnec_ds.index.get_level_values(JaoData.time))
-            .intersection(observed_flow.index)
-            .intersection(jaodata_and_net_positions.observedNPs.index)
-            .intersection(jaodata_and_net_positions.basecaseNPs.index)
-        )
-    ).sort_values()
-
+    index_alignment = align_by_index_overlap(
+        jaodata_and_net_positions.basecaseNPs, jaodata_and_net_positions.observedNPs, cnec_ds, observed_flow
+    )
     cnec_ds = cnec_ds.loc[index_alignment, :]
     observed_flow = observed_flow.loc[index_alignment, :]
     jaodata_and_net_positions = JaoDataAndNPS(
         jaodata_and_net_positions.jaoData,
         jaodata_and_net_positions.basecaseNPs.loc[index_alignment, :],  # type: ignore
         jaodata_and_net_positions.observedNPs.loc[index_alignment, :],  # type: ignore
     )
@@ -135,14 +128,22 @@
         cnec_ds,
         jaodata_and_net_positions.basecaseNPs,
         jaodata_and_net_positions.observedNPs,
         observed_flow,
     )
 
 
+def align_by_index_overlap(*dataframes: pd.DataFrame | pd.Series) -> pd.DatetimeIndex:
+    aligmnent_set = dataframes[0].index
+    for frame in dataframes[1:]:
+        aligmnent_set = aligmnent_set.intersection(frame.index)
+    index_alignment = pd.DatetimeIndex(aligmnent_set).sort_values()
+    return index_alignment
+
+
 def load_data_for_corridor_cnec(cnecName: str, jaodata_and_net_positions: JaoDataAndNPS) -> CnecDataAndNPS | None:
     """Loads data for a given cnec from its name as it appears in the  JAO API
 
     Args:
         cnecName (str): Name of the CNEC as it appears in the JAO API
         jao_and_entsoe_data (JaoDataAndNPS): Data from JAO and Entsoe APIs
```

### Comparing `fbmc_linearisation_analysis-0.4.3/fbmc_quality/plotting/flow_map.py` & `fbmc_linearisation_analysis-0.4.4/fbmc_quality/plotting/flow_map.py`

 * *Files identical despite different names*

### Comparing `fbmc_linearisation_analysis-0.4.3/pyproject.toml` & `fbmc_linearisation_analysis-0.4.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "fbmc-linearisation-analysis"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["Robert Solli <robert@xal.no>", "Kristan Authen <kristian.authen@statnett.no>"]
 readme = "README.md"
 packages = [{include = "fbmc_quality"}]
 
 [tool.poetry.scripts]
 fetch_jao_data = 'fbmc_quality.jao_data.jao_store_cli:app'
 fetch_entsoe_data = 'fbmc_quality.entsoe_data.entsoe_store_cli:app'
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11.0 || >3.11.0,<4.0"
 requests = "^2.31.0"
-polars = "^0.18.3"
+polars = "^0.20.3"
 beautifulsoup4 = "^4.12.2"
-entsoe-py = "^0.5.9"
+entsoe-py = ">=0.6.2"
 matplotlib = "^3.7.2"
 tzlocal = "^5.0.1"
 pytz = "^2023.3"
-pyarrow = "^12.0.1"
+pyarrow = "16.1.0"
 scikit-learn = "^1.3.0"
-pandera = {extras = ["mypy"], version = "^0.16.1"}
+pandera = {extras = ["mypy"], version = "^0.17.0"}
 typer = {extras = ["all"], version = "^0.9.0"}
 aiohttp = "^3.8.5"
 pandas = "^2.1.0"
 levenshtein = "^0.22.0"
-duckdb = "^0.9.0"
+duckdb = "0.10.2"
 duckdb-engine = "^0.9.2"
 plotly = {version="^5.17.0", optional=true}
 streamlit = {version = "^1.27.1", optional=true}
 geopandas = {version="*", optional=true}
 shapely = {version="*", optional=true}
 geojson-rewind = {version="*", optional=true}
 cache_to_disk = {version='*', optional=true}
```

### Comparing `fbmc_linearisation_analysis-0.4.3/PKG-INFO` & `fbmc_linearisation_analysis-0.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: fbmc-linearisation-analysis
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: Robert Solli
 Author-email: robert@xal.no
 Requires-Python: >=3.10, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*, !=3.9.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: app-template
 Provides-Extra: plotting
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: cache_to_disk
-Requires-Dist: duckdb (>=0.9.0,<0.10.0)
+Requires-Dist: duckdb (==0.10.2)
 Requires-Dist: duckdb-engine (>=0.9.2,<0.10.0)
-Requires-Dist: entsoe-py (>=0.5.9,<0.6.0)
+Requires-Dist: entsoe-py (>=0.6.2)
 Requires-Dist: geojson-rewind ; extra == "app-template" or extra == "plotting" or extra == "all"
 Requires-Dist: geopandas ; extra == "app-template" or extra == "plotting" or extra == "all"
 Requires-Dist: levenshtein (>=0.22.0,<0.23.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.0,<3.0.0)
-Requires-Dist: pandera[mypy] (>=0.16.1,<0.17.0)
+Requires-Dist: pandera[mypy] (>=0.17.0,<0.18.0)
 Requires-Dist: pillow ; extra == "app-template" or extra == "plotting" or extra == "all"
 Requires-Dist: plotly (>=5.17.0,<6.0.0) ; extra == "app-template" or extra == "plotting" or extra == "all"
-Requires-Dist: polars (>=0.18.3,<0.19.0)
-Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: polars (>=0.20.3,<0.21.0)
+Requires-Dist: pyarrow (==16.1.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Requires-Dist: shapely ; extra == "app-template" or extra == "plotting" or extra == "all"
 Requires-Dist: streamlit (>=1.27.1,<2.0.0) ; extra == "app-template" or extra == "all"
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: tzlocal (>=5.0.1,<6.0.0)
```

