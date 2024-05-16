# Comparing `tmp/labda-0.0.6.tar.gz` & `tmp/labda-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labda-0.0.6.tar", max compression
+gzip compressed data, was "labda-0.0.7.tar", max compression
```

## Comparing `labda-0.0.6.tar` & `labda-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0      570 2024-04-10 12:25:11.794327 labda-0.0.6/README.md
--rw-r--r--   0        0        0      190 2024-04-23 14:37:04.188505 labda-0.0.6/labda/__init__.py
--rw-r--r--   0        0        0      142 2024-03-26 12:17:08.741130 labda-0.0.6/labda/assets/__init__.py
--rw-r--r--   0        0        0     1195 2024-03-26 15:39:19.404282 labda-0.0.6/labda/assets/counts_cut_points.py
--rw-r--r--   0        0        0      459 2024-04-02 11:28:47.324035 labda-0.0.6/labda/assets/transportation_cut_points.py
--rw-r--r--   0        0        0      152 2024-02-06 17:52:16.176389 labda-0.0.6/labda/expanders/__init__.py
--rw-r--r--   0        0        0      656 2024-03-26 07:45:27.272975 labda-0.0.6/labda/expanders/accelerometer.py
--rw-r--r--   0        0        0      964 2024-03-26 07:45:27.272975 labda-0.0.6/labda/expanders/extras.py
--rw-r--r--   0        0        0     7377 2024-04-02 08:48:51.335892 labda-0.0.6/labda/expanders/spatial.py
--rw-r--r--   0        0        0     1246 2024-04-23 14:37:16.071524 labda-0.0.6/labda/logging.py
--rw-r--r--   0        0        0     1073 2024-04-02 14:15:23.256237 labda-0.0.6/labda/parallel.py
--rw-r--r--   0        0        0      201 2024-04-23 07:15:17.838214 labda-0.0.6/labda/parsers/__init__.py
--rw-r--r--   0        0        0     6854 2024-04-02 08:51:54.456305 labda-0.0.6/labda/parsers/actigraph.py
--rw-r--r--   0        0        0      930 2024-04-02 08:48:51.335892 labda-0.0.6/labda/parsers/bulk.py
--rw-r--r--   0        0        0     6508 2024-04-08 08:01:34.897150 labda-0.0.6/labda/parsers/gadgetbridge.py
--rw-r--r--   0        0        0     2332 2024-02-06 17:52:16.176389 labda-0.0.6/labda/parsers/garmin.py
--rw-r--r--   0        0        0    10952 2024-04-23 07:15:17.838214 labda-0.0.6/labda/parsers/qstarz.py
--rw-r--r--   0        0        0     8602 2024-05-01 11:09:20.815127 labda-0.0.6/labda/parsers/sens.py
--rw-r--r--   0        0        0     8322 2024-05-01 07:54:55.911821 labda-0.0.6/labda/parsers/traccar.py
--rw-r--r--   0        0        0     1737 2024-04-23 07:15:17.838214 labda-0.0.6/labda/parsers/utils.py
--rw-r--r--   0        0        0       36 2024-02-09 10:52:49.204568 labda-0.0.6/labda/processing/__init__.py
--rw-r--r--   0        0        0       88 2024-03-26 13:31:05.536930 labda-0.0.6/labda/processing/accelerometer/__init__.py
--rw-r--r--   0        0        0     1580 2024-03-26 13:51:21.538869 labda-0.0.6/labda/processing/accelerometer/activity_intensity.py
--rw-r--r--   0        0        0      616 2024-03-26 07:45:27.282975 labda-0.0.6/labda/processing/accelerometer/steps.py
--rw-r--r--   0        0        0      913 2024-03-26 07:45:27.282975 labda-0.0.6/labda/processing/accelerometer/wear.py
--rw-r--r--   0        0        0     2803 2024-03-26 07:45:27.282975 labda-0.0.6/labda/processing/bouts.py
--rw-r--r--   0        0        0      860 2024-04-16 07:17:13.024246 labda-0.0.6/labda/processing/domains.py
--rw-r--r--   0        0        0      488 2024-03-26 07:45:27.282975 labda-0.0.6/labda/processing/manipulations.py
--rw-r--r--   0        0        0      197 2024-03-26 14:28:15.353873 labda-0.0.6/labda/processing/spatial/__init__.py
--rw-r--r--   0        0        0     6142 2024-04-02 09:39:10.496322 labda-0.0.6/labda/processing/spatial/manipulations.py
--rw-r--r--   0        0        0     3277 2024-04-03 14:44:06.593954 labda-0.0.6/labda/processing/spatial/timeline.py
--rw-r--r--   0        0        0     3792 2024-05-01 14:19:00.081204 labda-0.0.6/labda/processing/spatial/transportation.py
--rw-r--r--   0        0        0    25960 2024-04-23 07:15:17.848219 labda-0.0.6/labda/processing/spatial/trips.py
--rw-r--r--   0        0        0     2247 2024-03-05 08:22:02.089665 labda-0.0.6/labda/processing/wear_validity.py
--rw-r--r--   0        0        0      250 2024-03-12 09:04:33.383063 labda-0.0.6/labda/structure/__init__.py
--rw-r--r--   0        0        0     4586 2024-04-02 13:58:21.046661 labda-0.0.6/labda/structure/collection.py
--rw-r--r--   0        0        0      704 2024-04-08 08:01:34.897150 labda-0.0.6/labda/structure/domains.py
--rw-r--r--   0        0        0      600 2024-04-08 08:01:34.897150 labda-0.0.6/labda/structure/linkage.py
--rw-r--r--   0        0        0     5000 2024-04-02 08:48:51.335892 labda-0.0.6/labda/structure/merging.py
--rw-r--r--   0        0        0     3008 2024-05-01 14:17:08.613103 labda-0.0.6/labda/structure/resampling.py
--rw-r--r--   0        0        0     9175 2024-05-01 14:20:35.742466 labda-0.0.6/labda/structure/subject.py
--rw-r--r--   0        0        0        0 2024-03-26 07:45:27.282975 labda-0.0.6/labda/structure/validation/__init__.py
--rw-r--r--   0        0        0      963 2024-02-09 12:27:12.019606 labda-0.0.6/labda/structure/validation/domains.py
--rw-r--r--   0        0        0      833 2024-02-09 12:37:10.070190 labda-0.0.6/labda/structure/validation/linkage.py
--rw-r--r--   0        0        0    11122 2024-05-01 14:19:06.349985 labda-0.0.6/labda/structure/validation/subject.py
--rw-r--r--   0        0        0     8345 2024-04-23 07:15:17.848219 labda-0.0.6/labda/utils.py
--rw-r--r--   0        0        0        0 2024-02-06 17:52:16.176389 labda-0.0.6/labda/visualisation/__init__.py
--rw-r--r--   0        0        0     3707 2024-04-08 11:46:48.951159 labda-0.0.6/labda/visualisation/spatial.py
--rw-r--r--   0        0        0     1668 2024-05-01 14:22:23.526187 labda-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2068 1970-01-01 00:00:00.000000 labda-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      548 2024-05-15 11:09:04.880673 labda-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      219 2024-05-15 11:09:04.890673 labda-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0      916 2024-05-15 11:09:04.890673 labda-0.0.7/README.md
+-rw-r--r--   0        0        0      183 2024-05-15 11:09:04.890673 labda-0.0.7/labda/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-26 12:17:08.741130 labda-0.0.7/labda/assets/__init__.py
+-rw-r--r--   0        0        0     1195 2024-03-26 15:39:19.404282 labda-0.0.7/labda/assets/counts_cut_points.py
+-rw-r--r--   0        0        0      808 2024-05-02 13:33:35.759080 labda-0.0.7/labda/assets/transportation_cut_points.py
+-rw-r--r--   0        0        0      152 2024-02-06 17:52:16.176389 labda-0.0.7/labda/expanders/__init__.py
+-rw-r--r--   0        0        0      656 2024-03-26 07:45:27.272975 labda-0.0.7/labda/expanders/accelerometer.py
+-rw-r--r--   0        0        0      964 2024-03-26 07:45:27.272975 labda-0.0.7/labda/expanders/extras.py
+-rw-r--r--   0        0        0     7377 2024-04-02 08:48:51.335892 labda-0.0.7/labda/expanders/spatial.py
+-rw-r--r--   0        0        0     1238 2024-05-16 07:03:10.802566 labda-0.0.7/labda/logging.py
+-rw-r--r--   0        0        0     1163 2024-05-15 11:09:04.890673 labda-0.0.7/labda/parallel.py
+-rw-r--r--   0        0        0      201 2024-04-23 07:15:17.838214 labda-0.0.7/labda/parsers/__init__.py
+-rw-r--r--   0        0        0     6852 2024-05-15 11:09:04.890673 labda-0.0.7/labda/parsers/actigraph.py
+-rw-r--r--   0        0        0     1013 2024-05-15 11:09:04.890673 labda-0.0.7/labda/parsers/bulk.py
+-rw-r--r--   0        0        0     6508 2024-04-08 08:01:34.897150 labda-0.0.7/labda/parsers/gadgetbridge.py
+-rw-r--r--   0        0        0     2332 2024-02-06 17:52:16.176389 labda-0.0.7/labda/parsers/garmin.py
+-rw-r--r--   0        0        0    10993 2024-05-15 11:09:04.890673 labda-0.0.7/labda/parsers/qstarz.py
+-rw-r--r--   0        0        0     8586 2024-05-15 12:06:39.577189 labda-0.0.7/labda/parsers/sens.py
+-rw-r--r--   0        0        0     8898 2024-05-15 12:06:18.811945 labda-0.0.7/labda/parsers/traccar.py
+-rw-r--r--   0        0        0       37 2024-05-15 11:09:04.890673 labda-0.0.7/labda/processing/__init__.py
+-rw-r--r--   0        0        0       88 2024-03-26 13:31:05.536930 labda-0.0.7/labda/processing/accelerometer/__init__.py
+-rw-r--r--   0        0        0     1580 2024-03-26 13:51:21.538869 labda-0.0.7/labda/processing/accelerometer/activity_intensity.py
+-rw-r--r--   0        0        0      616 2024-03-26 07:45:27.282975 labda-0.0.7/labda/processing/accelerometer/steps.py
+-rw-r--r--   0        0        0      913 2024-03-26 07:45:27.282975 labda-0.0.7/labda/processing/accelerometer/wear.py
+-rw-r--r--   0        0        0     2803 2024-03-26 07:45:27.282975 labda-0.0.7/labda/processing/bouts.py
+-rw-r--r--   0        0        0     2635 2024-05-15 11:09:04.890673 labda-0.0.7/labda/processing/context.py
+-rw-r--r--   0        0        0      488 2024-03-26 07:45:27.282975 labda-0.0.7/labda/processing/manipulations.py
+-rw-r--r--   0        0        0      197 2024-03-26 14:28:15.353873 labda-0.0.7/labda/processing/spatial/__init__.py
+-rw-r--r--   0        0        0     6142 2024-04-02 09:39:10.496322 labda-0.0.7/labda/processing/spatial/manipulations.py
+-rw-r--r--   0        0        0     3277 2024-04-03 14:44:06.593954 labda-0.0.7/labda/processing/spatial/timeline.py
+-rw-r--r--   0        0        0     3792 2024-05-01 14:19:00.081204 labda-0.0.7/labda/processing/spatial/transportation.py
+-rw-r--r--   0        0        0    26117 2024-05-02 13:42:51.176141 labda-0.0.7/labda/processing/spatial/trips.py
+-rw-r--r--   0        0        0     2247 2024-03-05 08:22:02.089665 labda-0.0.7/labda/processing/wear_validity.py
+-rw-r--r--   0        0        0      252 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/__init__.py
+-rw-r--r--   0        0        0     4852 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/collection.py
+-rw-r--r--   0        0        0     2595 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/contexts.py
+-rw-r--r--   0        0        0      600 2024-04-08 08:01:34.897150 labda-0.0.7/labda/structure/linkage.py
+-rw-r--r--   0        0        0     8790 2024-05-16 07:03:10.802566 labda-0.0.7/labda/structure/merging.py
+-rw-r--r--   0        0        0     3423 2024-05-16 07:03:10.802566 labda-0.0.7/labda/structure/resampling.py
+-rw-r--r--   0        0        0    15046 2024-05-16 08:08:03.793217 labda-0.0.7/labda/structure/subject.py
+-rw-r--r--   0        0        0        0 2024-03-26 07:45:27.282975 labda-0.0.7/labda/structure/validation/__init__.py
+-rw-r--r--   0        0        0     1337 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/validation/context.py
+-rw-r--r--   0        0        0      833 2024-02-09 12:37:10.070190 labda-0.0.7/labda/structure/validation/linkage.py
+-rw-r--r--   0        0        0    11339 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/validation/subject.py
+-rw-r--r--   0        0        0     9961 2024-05-15 11:09:04.890673 labda-0.0.7/labda/utils.py
+-rw-r--r--   0        0        0        0 2024-02-06 17:52:16.176389 labda-0.0.7/labda/visualisation/__init__.py
+-rw-r--r--   0        0        0     3785 2024-05-15 11:09:04.890673 labda-0.0.7/labda/visualisation/spatial.py
+-rw-r--r--   0        0        0     1670 2024-05-16 08:35:54.413823 labda-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 labda-0.0.7/PKG-INFO
```

### Comparing `labda-0.0.6/labda/assets/counts_cut_points.py` & `labda-0.0.7/labda/assets/counts_cut_points.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/expanders/accelerometer.py` & `labda-0.0.7/labda/expanders/accelerometer.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/expanders/extras.py` & `labda-0.0.7/labda/expanders/extras.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/expanders/spatial.py` & `labda-0.0.7/labda/expanders/spatial.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/parallel.py` & `labda-0.0.7/labda/parallel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import logging
 import multiprocessing as mp
 from functools import partial
 from typing import Any, Callable
 
-from .logging import logger
 from .structure.subject import Subject
 
+logger = logging.getLogger("default")
+
 
 def process_obj(obj: Any, func: Callable, **kwargs) -> Any | None:
     try:
         if isinstance(obj, Subject):
             func(obj, **kwargs)
             return obj
-
-        return func(obj, **kwargs)
+        else:
+            return func(obj, **kwargs)
     except Exception as e:
+        # FIX: This could be probably removed.
         logger.error(f"{func.__module__}:{func.__name__} | {obj} | {e}")
 
 
 def parallel_processing(
     func: Callable,
     objs: list[Any],
     n_cores: int | str = "max",
```

### Comparing `labda-0.0.6/labda/parsers/actigraph.py` & `labda-0.0.7/labda/parsers/actigraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Tuple
 
 import pandas as pd
 from dateutil.parser import parse as parse_dt
 
-from ..logging import success_parsing_log
+from ..logging import log_successfully_parsed_subject
 from ..structure.subject import Metadata, Sensor, Subject, Vendor
 from ..structure.validation.subject import SCHEMA, Column
 from ..utils import (
     align_datetimes,
     filter_datetime,
     get_sampling_frequency,
+    set_timezone,
 )
-from .utils import set_timezone
 
 # TODO: Add param for column mapping if there is no header.
 # TODO: It is not perfect, but it is a start and it should be able to parse automatically almost all ActiGraph files from SDU.
 
 
 def get_metadata(metadata: list[str]) -> dict[str, Any]:
     model = metadata[0].split("ActiGraph")[-1].split()[0].strip()
@@ -215,12 +215,10 @@
         id=subject_id,
         sensor=[sensor],
         sampling_frequency=sampling_frequency,
         timezone=timezone,
     )  # type: ignore
 
     subject = Subject(metadata=metadata, df=df)  # type: ignore
-
-    func = f"{__name__}:from_csv"
-    success_parsing_log(subject, path, func)
+    log_successfully_parsed_subject(subject, f"{__name__}.from_csv", path.name)
 
     return subject
```

### Comparing `labda-0.0.6/labda/parsers/bulk.py` & `labda-0.0.7/labda/parsers/bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,10 +30,13 @@
         results = parallel_processing(parser, files, n_cores, **kwargs)
     else:
         results = [process_obj(file, parser, **kwargs) for file in files]
 
     # Remove None values from results
     results = list(filter(None, results))
 
+    if not results:
+        raise ValueError(f"No subjects found in '{folder}'.")
+
     collection = Collection(id=id, subjects=results)
 
     return collection
```

### Comparing `labda-0.0.6/labda/parsers/gadgetbridge.py` & `labda-0.0.7/labda/parsers/gadgetbridge.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/parsers/garmin.py` & `labda-0.0.7/labda/parsers/garmin.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/parsers/qstarz.py` & `labda-0.0.7/labda/parsers/qstarz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 
-from ..logging import success_parsing_log
+from ..logging import log_successfully_parsed_subject
 from ..structure.subject import Metadata, Sensor, Subject, Vendor
 from ..structure.validation.subject import SCHEMA, Column
 from ..utils import (
     align_datetimes,
     columns_exists,
     filter_datetime,
     get_sampling_frequency,
+    set_crs,
+    set_timezone,
 )
-from .utils import set_crs, set_timezone
 
 # TODO: Can be refactored.,
 
 
 def detect_environment_from_gps_signal(
     df: pd.DataFrame,
     method: str,
@@ -87,24 +88,24 @@
     return df
 
 
 def parse_nsat(df: pd.DataFrame) -> pd.DataFrame:
     df = df.copy()
 
     possible_columns = ["NSAT (USED/VIEW)", "NSAT(USED/VIEW)", "NSAT(USED/VIEWED)"]
+    nsat_uv = None
+    nsat = "NSAT"
 
     for column in possible_columns:
         if column in df.columns:
             nsat_uv = "NSAT (USED/VIEW)"
             df.rename(columns={column: nsat_uv}, inplace=True)
             break
 
-    nsat = "NSAT"
-
-    if nsat_uv in df.columns:
+    if nsat_uv:
         if df[nsat_uv].str.contains("/").any():
             df[nsat_uv] = df[nsat_uv].str.split("/")
         elif df[nsat_uv].str.contains(r"\(").any():  # Maybe this is wrong
             df[nsat_uv] = df[nsat_uv].str.replace(")", "").str.split("(")
         df[Column.NSAT_USED] = pd.to_numeric(df[nsat_uv].str[0])
         df[Column.NSAT_VIEWED] = pd.to_numeric(df[nsat_uv].str[1])
     elif nsat in df.columns:
@@ -270,14 +271,15 @@
         None
     """
     header = pd.Series(df.columns, df.columns)
     same_as_header = df[df.eq(header).all(axis=1)].index
     df.drop(same_as_header, inplace=True)
 
 
+# @log_successfully_parsed_subject
 def from_csv(
     path: str | Path,
     *,
     subject_id: str | None = None,
     sensor_id: str | None = None,
     serial_number: str | None = None,
     model: str | None = None,
@@ -369,12 +371,10 @@
         sensor=[sensor],
         sampling_frequency=sampling_frequency,
         crs=crs,
         timezone=timezone,
     )
 
     subject = Subject(metadata=metadata, df=df)
-
-    func = f"{__name__}:from_csv"
-    success_parsing_log(subject, path, func)
+    log_successfully_parsed_subject(subject, f"{__name__}.from_csv", path.name)
 
     return subject
```

### Comparing `labda-0.0.6/labda/parsers/sens.py` & `labda-0.0.7/labda/parsers/sens.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import time
 from datetime import datetime
 from pathlib import Path
-from typing import Tuple
 
 import pandas as pd
 
-from ..logging import success_parsing_log
+from ..logging import log_successfully_parsed_subject
 from ..structure.subject import Metadata, Sensor, Subject, Vendor
 from ..structure.validation.subject import SCHEMA, Column
 from ..utils import (
     align_datetimes,
     filter_datetime,
     get_sampling_frequency,
+    set_timezone,
 )
-from .utils import set_timezone
 
 
 def _parse_csv(path: Path) -> pd.DataFrame:
     df = pd.read_csv(
         path,
         engine="pyarrow",
         dtype={
@@ -153,15 +152,16 @@
         firmware_version (str, optional): The firmware version of the sensor.
 
 
     Returns:
         Subject: A Subject object containing the fetched and processed dataframe containing information: datetime, wear, position, steps, activity_intensity, activity_value and activity.
 
     Raises:
-        ValueError: If the path is not a file or the file format is not CSV.
+        FileNotFoundError: File not found.
+        ValueError: File format not CSV.
 
     Examples:
         Here's how to call the function with just the minimum required parameters.
 
         ```python
         from labda.parsers import Sens
 
@@ -172,15 +172,15 @@
     """
     #
 
     if isinstance(path, str):
         path = Path(path)
 
     if not path.is_file():
-        raise ValueError(f"Invalid file path: {path}")
+        raise FileNotFoundError(f"File not found: {path}")
 
     if path.suffix != ".csv":
         raise ValueError(f"Invalid file format: {path.suffix}")
 
     df = _parse_csv(path)
 
     if timezone:
@@ -223,12 +223,10 @@
         id=subject_id,
         sensor=[sensor],
         sampling_frequency=sampling_frequency,
         timezone=timezone,
     )
 
     subject = Subject(metadata=metadata, df=df)
-
-    func = f"{__name__}:from_csv"
-    success_parsing_log(subject, path, func)
+    log_successfully_parsed_subject(subject, f"{__name__}.from_csv", path.name)
 
     return subject
```

### Comparing `labda-0.0.6/labda/parsers/traccar.py` & `labda-0.0.7/labda/parsers/traccar.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,52 +4,61 @@
 from urllib.parse import urljoin
 
 import pandas as pd
 import requests
 from pytz import UTC
 from requests.auth import HTTPBasicAuth
 
-from ..logging import success_parsing_log
+from ..logging import log_successfully_parsed_subject
 from ..structure.subject import SCHEMA, Column, Metadata, Sensor, Subject, Vendor
 from ..utils import (
     align_datetimes,
+    change_crs,
+    change_timezone,
+    get_crs,
     get_sampling_frequency,
+    get_timezone,
 )
-from .utils import change_crs, change_timezone, get_crs, get_timezone
 
 
 def _knots_to_kmh(knots):
     return knots * 1.852
 
 
 def _get_device(
     url: str,
     username: str,
     password: str,
     subject_id: str,
 ) -> dict[str, Any]:
-    url = urljoin(url, "api/devices")
-
+    endpoint = urljoin(url, "api/devices")
     params = {"uniqueId": subject_id}
 
     headers = {
         "Accept": "application/json",
     }
 
-    response = requests.get(
-        url,
-        params,
-        auth=HTTPBasicAuth(username, password),
-        headers=headers,
-    )
+    try:
+        response = requests.get(
+            endpoint,
+            params,
+            auth=HTTPBasicAuth(username, password),
+            headers=headers,
+        )
+        response.raise_for_status()
+    except requests.exceptions.HTTPError:
+        message = f"HTTP error {response.status_code} when trying to get device with subject_id {subject_id} from Traccar server {url}. Propably wrong credentials or url."
+
+        raise
 
     response_json = response.json()
 
     if not response_json:
-        raise ValueError(f"Device with subject_id {subject_id} not found")
+        message = f"No device found with subject_id {subject_id}"
+        raise ValueError(message)
 
     device = response_json[0]
     phone = device["phone"]
     model = device["model"]
 
     if phone and model:
         model = f"{phone} ({model})"
@@ -90,15 +99,16 @@
         auth=HTTPBasicAuth(username, password),
         headers=headers,
     )
 
     response_json = response.json()
 
     if not response_json:
-        raise ValueError(f"No records found for device with id {id}")
+        message = f"No records found for device with id {id}."
+        raise ValueError(message)
 
     return response_json
 
 
 def _parse_records(response_json: dict[str, Any]) -> pd.DataFrame:
     df = pd.DataFrame(response_json)
     attributes = pd.json_normalize(df["attributes"]).add_prefix("attributes_")  # type: ignore
@@ -174,14 +184,20 @@
         model (str, optional): The model of the device. If not provided, it will be fetched from the Traccar server (device - extra, phone + model) if available.
         serial_number (str, optional): The serial number of the device.
         firmware_version (str, optional): The firmware version of the device.
 
     Returns:
         Subject: A Subject object containing the fetched and processed dataframe containing information: datetime, latitude, longitude, gps_accuracy, distance, elevation, and speed.
 
+
+    Raises:
+        HTTPError: HTTP request to the Traccar server failed.
+        ValueError: No device is found for the specified subject ID.
+        ValueError: No records are found for the specified device.
+
     Examples:
         Here's how to call the function with just the minimum required parameters.
 
         ```python
         from labda.parsers import Traccar
 
         subject = Traccar.from_server(
@@ -252,12 +268,10 @@
         sensor=[sensor],
         sampling_frequency=sampling_frequency,
         crs=crs,
         timezone=timezone,
     )
 
     subject = Subject(metadata=metadata, df=df)
-
-    func = f"{__name__}:from_server"
-    success_parsing_log(subject, url, func)
+    log_successfully_parsed_subject(subject, f"{__name__}.from_server", url)
 
     return subject
```

### Comparing `labda-0.0.6/labda/processing/accelerometer/activity_intensity.py` & `labda-0.0.7/labda/processing/accelerometer/activity_intensity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/processing/accelerometer/steps.py` & `labda-0.0.7/labda/processing/accelerometer/steps.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/processing/accelerometer/wear.py` & `labda-0.0.7/labda/processing/accelerometer/wear.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/processing/bouts.py` & `labda-0.0.7/labda/processing/bouts.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/processing/spatial/manipulations.py` & `labda-0.0.7/labda/processing/spatial/manipulations.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/processing/spatial/timeline.py` & `labda-0.0.7/labda/processing/spatial/timeline.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/processing/spatial/transportation.py` & `labda-0.0.7/labda/processing/spatial/transportation.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/processing/spatial/trips.py` & `labda-0.0.7/labda/processing/spatial/trips.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,14 +481,17 @@
         how="left",
     )
 
     return origin
 
 
 # TODO: Fix docstring.
+# TODO: Add max change in elevation
+# TODO: Add noise removal based on min distance (three points removal as in PALMS)
+# TODO: Remove lone fixes as in PALMS
 def detect_trips(
     df: pd.DataFrame,
     *,
     crs: str,
     sampling_frequency: float,
     gap_duration: timedelta,
     stop_radius: int | float,
```

### Comparing `labda-0.0.6/labda/processing/wear_validity.py` & `labda-0.0.7/labda/processing/wear_validity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/structure/collection.py` & `labda-0.0.7/labda/structure/collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import logging
 import secrets
 from functools import partial
 from pathlib import Path
 from typing import Optional
 
+import pandas as pd
 from pydantic import BaseModel, Field
 
 from ..parallel import parallel_processing
 from .subject import Subject
 
+logger = logging.getLogger("default")
+
 
 def _to_parquet_with_path(subject, path, overwrite):
     subject_path = path / f"{subject.metadata.id}.parquet"
     return Subject.to_parquet(subject, path=subject_path, overwrite=overwrite)
 
 
 class Collection(BaseModel):
@@ -112,35 +116,46 @@
                 n_cores,
                 **kwargs,
             )
         else:
             for subject in self.subjects:
                 subject.detect_activity_intensity(**kwargs)
 
-    # TODO: Rework whole consistency check
-    # TODO: Add also check columns consistency
-    # TODO: Check if collection is not empty.
-    def _check_consistency(self, attribute, error_message):
-        # TODO: Add docstring, better name for method
-        values = [getattr(subject.metadata, attribute) for subject in self.subjects]
-        unique = set(values)
+    def _check_atribute_consistency(self, metadata: pd.DataFrame, attribute):
+        unique = metadata[attribute].unique()
 
         if len(unique) != 1:
-            print(f"{error_message}: {unique}")
-
-    def _check_consistent_sampling_frequencies(self):
-        self._check_consistency(
-            "sampling_frequency", "Sampling frequencies are not consistent"
-        )
-
-    def _check_consistent_crs(self):
-        self._check_consistency("crs", "CRS are not consistent")
+            origin = f"{self.__class__.__name__}.check_consistency[{attribute}]"
+            logger.error(
+                f"{attribute}: {unique}",
+                extra={"origin": origin, "object": self.id},
+            )
 
-    def _check_consistent_timezones(self):
-        self._check_consistency("timezone", "Timezones are not consistent")
+            return True
 
-    def check_consistency(self):
-        self._check_consistent_sampling_frequencies()
-        self._check_consistent_crs()
-        self._check_consistent_timezones()
+    def consistency(self):
+        # TODO: Add also check columns consistency
+        attributes = ["sampling_frequency", "crs", "timezone"]
+
+        metadata = pd.DataFrame(
+            [
+                s.metadata.model_dump(include=set(["id"] + attributes))
+                for s in self.subjects
+            ]
+        )
+        metadata.set_index("id", inplace=True)
 
-        print("Consistency check finished.")
+        consistency_results = [
+            self._check_atribute_consistency(metadata, attr) for attr in attributes
+        ]
+
+        origin = f"{__name__}.check_consistency"
+        extra = {"origin": origin, "object": self.id}
+
+        if any(consistency_results):
+            message = ""
+            logger.error(message, extra=extra)
+        else:
+            logger.info(
+                "Consistency check finished.",
+                extra=extra,
+            )
```

### Comparing `labda-0.0.6/labda/structure/linkage.py` & `labda-0.0.7/labda/structure/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/structure/resampling.py` & `labda-0.0.7/labda/structure/resampling.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+import logging
 from typing import Any
 
 import pandas as pd
 
 from ..structure.validation.subject import Column
 
 # TODO: Create one big configuration with SCHEMA (validation) and RESAMPLING
 
+logger = logging.getLogger("default")
+
+
+def log_upsample(id: str, from_sf: float, to_sf: float, origin: str):
+    message = f"Subject's data upsampled from {from_sf}s to {to_sf}s."
+
+    logger.info(message, extra={"origin": origin, "object": id})
+
 
 def mode(x):
     vals = x.to_list()
     return max(vals, key=vals.count)
 
 
 UPSAMPLING = [
@@ -50,22 +59,24 @@
     # TODO: ACTIVITY_VALUE - This is should be discussed a lot.
     {"column": Column.ACTIVITY_VALUE, "method": "mean"},
     {"column": Column.ACTIVITY, "method": mode},
 ]
 
 
 def upsample(
+    id: str,
     df: pd.DataFrame,
     from_sf: float,
     to_sf: float,
     mapper: list[dict[str, Any]] | None = None,
 ) -> pd.DataFrame:
     if from_sf > to_sf:
         raise ValueError(f"Downsampling is not supported | {from_sf} > {to_sf}")
     elif from_sf == to_sf:
+        print(f"Sampling frequencies are the same | {from_sf} = {to_sf}")
         return df
 
     df = df.copy()
 
     if not mapper:
         mapper = UPSAMPLING
 
@@ -80,8 +91,10 @@
         )  # TODO: Write warning what columns are dropped.
 
     df = df.resample(f"{to_sf}s").agg(resampling)  # type: ignore
     df.dropna(
         axis=0, how="all", inplace=True
     )  # Dropping rows with all NaN values - they were created by resampling.
 
+    log_upsample(id, from_sf, to_sf, origin="Subject.upsample")
+
     return df
```

### Comparing `labda-0.0.6/labda/structure/validation/domains.py` & `labda-0.0.7/labda/structure/validation/context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,53 @@
-from pandera import Column, DataFrameSchema
+from enum import StrEnum
 
-# TODO: Refactor...
+import pandera as pr
 
-SCHEMA = DataFrameSchema(
+
+class Column(StrEnum):
+    SUBJECT_ID = "subject_id"
+    CONTEXT = "context"
+    PRIORITY = "priority"
+    START = "start"
+    END = "end"
+    GEOMETRY = "geometry"
+
+
+SCHEMA = pr.DataFrameSchema(
     columns={
-        "subject_id": Column(
+        Column.SUBJECT_ID: pr.Column(
             dtype="string",
-            description="Unique ID of the dataframe (participant)",
+            description="Unique ID of the dataframe (subject)",
             required=False,
             nullable=True,
         ),
-        "domain": Column(
+        Column.CONTEXT: pr.Column(
             dtype="string",
-            description="Name of the domain",
+            description="Name of the context",
+        ),
+        Column.PRIORITY: pr.Column(
+            dtype="Int64",
+            description="Priority of the context",
+            required=False,
+            nullable=True,
         ),
-        "start": Column(
+        Column.START: pr.Column(
             dtype="datetime64[ns]",
-            description="Start time of the domain",
+            description="Start time of the context",
             required=False,
             nullable=True,
         ),
-        "end": Column(
+        Column.END: pr.Column(
             dtype="datetime64[ns]",
-            description="End time of the domain",
+            description="End time of the context",
             required=False,
             nullable=True,
         ),
-        "geometry": Column(
+        Column.GEOMETRY: pr.Column(
             dtype="geometry",
-            description="Geometry of the domain",
+            description="Geometry of the context",
             required=False,
             nullable=True,
         ),
     },
     coerce=True,
 )
```

### Comparing `labda-0.0.6/labda/structure/validation/linkage.py` & `labda-0.0.7/labda/structure/validation/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.6/labda/structure/validation/subject.py` & `labda-0.0.7/labda/structure/validation/subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     # ---
     HEART_RATE = "heart_rate"
     LUX = "lux"
     # ---
     ACTIVITY_INTENSITY = "activity_intensity"
     ACTIVITY_VALUE = "activity_value"
     ACTIVITY = "activity"
+    # ---
+    CONTEXT = "context"
 
 
 SCHEMA = pr.DataFrameSchema(
     index=pr.Index(
         name=Column.DATETIME,
         dtype="datetime64[ns]",
         description="Datetime in timezone where data was collected.",
@@ -358,11 +360,17 @@
                             "vigorous",
                             "very_vigorous",
                         ]
                     ),
                 )
             ],
         ),
+        Column.CONTEXT: pr.Column(
+            dtype="category",
+            description="Spatiotemporal context.",
+            required=False,
+            nullable=False,
+        ),
     },
     coerce=True,
     strict=False,
 )
```

### Comparing `labda-0.0.6/labda/utils.py` & `labda-0.0.7/labda/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import secrets
 from datetime import datetime
+from typing import Tuple
 
 import geopandas as gpd
 import pandas as pd
 import pyproj
 from timezonefinder import TimezoneFinder
 
 from .structure.validation.subject import Column
 
+DEFAULT_CRS_SENSOR = "EPSG:4326"
+
 
 def columns_exists(
     df: pd.DataFrame,
     columns: list[Column | str],
 ) -> None:
     """
     Checks if the given columns exist in the DataFrame.
@@ -268,7 +271,60 @@
     if start:
         df = df[df.index >= start]
 
     if end:
         df = df[df.index <= end]
 
     return df
+
+
+# TODO: Maybe those functions should be refactored, i.e. if (None, timezone) -> timezone would be guessed from the data and then changed to the target timezone. Same for CRS.
+
+
+def set_timezone(
+    df: pd.DataFrame,
+    timezone: str | None | Tuple[str, str] = None,
+) -> Tuple[pd.DataFrame, str | None]:
+    if (
+        isinstance(timezone, tuple)
+        and len(timezone) == 2
+        and all(isinstance(tz, str) for tz in timezone)
+    ):
+        source_tz = timezone[0]
+        target_tz = timezone[1]
+        df = change_timezone(df, source_tz, target_tz)
+        timezone = target_tz
+    elif isinstance(timezone, str):
+        pass
+    elif not timezone:
+        if "latitude" in df.columns and "longitude" in df.columns:
+            timezone = get_timezone(df)
+        else:
+            timezone = None
+    else:
+        raise ValueError(f"Invalid value for timezone: {timezone}")
+
+    return df, timezone
+
+
+def set_crs(
+    df: pd.DataFrame,
+    crs: str | None | Tuple[str, str] = None,
+) -> Tuple[pd.DataFrame, str]:
+    if (
+        isinstance(crs, tuple)
+        and len(crs) == 2
+        and all(isinstance(c, str) for c in crs)
+    ):
+        source_crs = crs[0]
+        target_crs = crs[1]
+        df = change_crs(df, source_crs, target_crs)
+        crs = target_crs
+    elif isinstance(crs, str):
+        df = change_crs(df, DEFAULT_CRS_SENSOR, crs)
+    elif not crs:
+        crs = get_crs(df)
+        df = change_crs(df, DEFAULT_CRS_SENSOR, crs)
+    else:
+        raise ValueError(f"Invalid value for crs: {crs}")
+
+    return df, crs
```

### Comparing `labda-0.0.6/labda/visualisation/spatial.py` & `labda-0.0.7/labda/visualisation/spatial.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     tooltip = {
         "html": """<strong>Status:</strong> {status_text}<br/>
         <strong>Start:</strong> {start}<br/>
         <strong>End:</strong> {end}<br/>
         <strong>Duration:</strong> {duration}<br/>
         <strong>Distance:</strong> {distance}<br/>
-        <strong>Mode:</strong> {mode}<br/>
+        <strong>Mode:</strong> {mode}
         """,
     }
 
     return layer, tooltip, center
 
 
 def gps_layer(
@@ -93,15 +93,15 @@
         pickable=True,
         auto_highlight=True,
     )
 
     tooltip = {
         "html": """<strong>Datetime:</strong> {datetime}<br/>
         <strong>Latitude:</strong> {latitude}<br/>
-        <strong>Longitude:</strong> {longitude}<br/>
+        <strong>Longitude:</strong> {longitude}
         """,
     }
 
     return layer, tooltip, center
 
 
 def plot(
@@ -111,14 +111,16 @@
     crs: str | None = None,
 ) -> str:
     match kind:
         case "timeline":
             layer, tooltip, center = timeline_layer(df, crs)
         case "gps":
             layer, tooltip, center = gps_layer(df, crs)
+        # case "context":
+        #     layer, tooltip, center = context_layer(df, crs)
         case _:
             raise ValueError(f"Kind '{kind}' not supported.")
 
     # Set the viewport location
     view_state = pdk.ViewState(longitude=center.x, latitude=center.y, zoom=10)
 
     # Render
```

### Comparing `labda-0.0.6/pyproject.toml` & `labda-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labda"
-version = "0.0.6"
+version = "0.0.7"
 description = "Library for Advanced Behavioural Data Analysis"
 authors = ["Josef Heidler <jheidler@health.sdu.dk>"]
 maintainers = ["Josef Heidler <jheidler@health.sdu.dk>"]
 
 readme = "README.md"
 license = "	CC-BY-SA-4.0"
 homepage = "https://labda.josefheidler.cz"
@@ -32,19 +32,19 @@
 geopandas = "^0.14.2"
 timezonefinder = "^6.2.0"
 pyarrow = "^15.0.0"
 pandera = "^0.18.0"
 openpyxl = "^3.1.2"
 sqlalchemy = "^2.0.25"
 pydeck = "^0.8.0"
-loguru = "^0.7.2"
 actipy = "^3.0.5"
 black = "^24.4.0"
 plotly = "^5.21.0"
 requests = "^2.31.0"
+colorlog = "^6.8.2"
 
 
 [tool.poetry.group.dev.dependencies]
 mkdocs-material = "^9.5.6"
 mkdocstrings = { extras = ["python"], version = "^0.24.3" }
 scikit-learn = "^1.4.0"
 resampy = "^0.4.2"                                          # Remove after Axivity CWA/CSV parser and RAW to counts conversion is implemented
```

### Comparing `labda-0.0.6/PKG-INFO` & `labda-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labda
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library for Advanced Behavioural Data Analysis
 Home-page: https://labda.josefheidler.cz
 License: 	CC-BY-SA-4.0
 Keywords: analysis,health,behaviour,data,spatial,temporal
 Author: Josef Heidler
 Author-email: jheidler@health.sdu.dk
 Maintainer: Josef Heidler
@@ -17,16 +17,16 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: actipy (>=3.0.5,<4.0.0)
 Requires-Dist: black (>=24.4.0,<25.0.0)
+Requires-Dist: colorlog (>=6.8.2,<7.0.0)
 Requires-Dist: geopandas (>=0.14.2,<0.15.0)
-Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pandera (>=0.18.0,<0.19.0)
 Requires-Dist: plotly (>=5.21.0,<6.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydeck (>=0.8.0,<0.9.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -34,14 +34,19 @@
 Requires-Dist: timezonefinder (>=6.2.0,<7.0.0)
 Project-URL: Documentation, https://labda.josefheidler.cz
 Project-URL: Repository, https://github.com/josefheidler/labda
 Description-Content-Type: text/markdown
 
 # LABDA: Library for Advanced Behavioural Data Analysis
 
+[![pypi](https://img.shields.io/pypi/v/labda.svg)](https://pypi.python.org/pypi/labda)
+[![downloads](https://static.pepy.tech/badge/labda/month)](https://pepy.tech/project/labda)
+[![versions](https://img.shields.io/pypi/pyversions/labda.svg)](https://github.com/josefheidler/labda)
+![discord](https://img.shields.io/discord/1165947556807848016)
+
 **LABDA is currently under development and may undergo significant API changes that could result in breaking changes.**
 
 ## What is it?
 
 TO-DO...
 
 ## Main Features
```

