# Comparing `tmp/pyqqq-0.9.6.tar.gz` & `tmp/pyqqq-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.9.6.tar", max compression
+gzip compressed data, was "pyqqq-0.9.7.tar", max compression
```

## Comparing `pyqqq-0.9.6.tar` & `pyqqq-0.9.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.6/README.md
--rw-r--r--   0        0        0      791 2024-05-09 05:02:27.715972 pyqqq-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.6/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.6/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.6/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    43409 2024-05-07 06:54:47.220204 pyqqq-0.9.6/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.6/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.9.6/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.6/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.6/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187522 2024-05-07 09:02:33.261786 pyqqq-0.9.6/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.6/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.6/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.9.6/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.6/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.6/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.6/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     5410 2024-05-09 05:02:14.041356 pyqqq-0.9.6/pyqqq/data/daily.py
--rw-r--r--   0        0        0     9684 2024-05-03 09:30:10.903300 pyqqq-0.9.6/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.6/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.6/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.6/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.6/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.6/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.6/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.6/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.6/pyqqq/utils/api_client.py
--rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.6/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.6/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.6/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.6/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.6/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.6/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.6/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.6/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.6/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 pyqqq-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.7/README.md
+-rw-r--r--   0        0        0      791 2024-05-16 01:07:06.025646 pyqqq-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.7/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.7/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.7/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    43409 2024-05-07 06:54:47.220204 pyqqq-0.9.7/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.7/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.9.7/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.7/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.7/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187522 2024-05-07 09:02:33.261786 pyqqq-0.9.7/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.7/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.7/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.9.7/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.7/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.7/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.7/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     5484 2024-05-16 01:05:45.085685 pyqqq-0.9.7/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     9684 2024-05-03 09:30:10.903300 pyqqq-0.9.7/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.7/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.7/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.7/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.7/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.7/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.7/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.7/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.7/pyqqq/utils/api_client.py
+-rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.7/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.7/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.7/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.7/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.7/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.7/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.7/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.7/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.7/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 pyqqq-0.9.7/PKG-INFO
```

### Comparing `pyqqq-0.9.6/README.md` & `pyqqq-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyproject.toml` & `pyqqq-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.9.6"
+version = "0.9.7"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.9.6/pyqqq/__init__.py` & `pyqqq-0.9.7/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.9.7/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.9.7/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.9.7/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.9.7/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.9.7/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.9.7/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.9.7/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.9.7/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.9.7/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/data/daily.py` & `pyqqq-0.9.7/pyqqq/data/daily.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,22 +48,26 @@
         000075  54800  54900  54800  54800     177     9702400  -100      -0.18
     """
     url = f"{c.PYQQQ_API_URL}/domestic-stock/ohlcv/daily/all/{date}"
     r = send_request("GET", url)
     raise_for_status(r)
 
     data = r.json()
+
     cols = data["cols"]
     rows = data["rows"]
 
-    df = pd.DataFrame(rows, columns=cols)
-    df.drop(columns=["date"], inplace=True)
-    df.set_index("code", inplace=True)
+    if not rows:
+        return pd.DataFrame()
+    else:
+        df = pd.DataFrame(rows, columns=cols)
+        df.drop(columns=["date"], inplace=True)
+        df.set_index("code", inplace=True)
 
-    return df
+        return df
 
 
 def get_ohlcv_by_codes_for_period(
     codes: List[str], start_date: dtm.date, end_date: Optional[dtm.date] = None
 ) -> Dict[str, pd.DataFrame]:
     """
     지정된 코드 리스트와 기간에 대한 OHLCV 데이터를 조회합니다.
```

### Comparing `pyqqq-0.9.6/pyqqq/data/domestic.py` & `pyqqq-0.9.7/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/data/minutes.py` & `pyqqq-0.9.7/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/data/realtime.py` & `pyqqq-0.9.7/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/data/ticks.py` & `pyqqq-0.9.7/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/datatypes.py` & `pyqqq-0.9.7/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/executors/hook.py` & `pyqqq-0.9.7/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/api_client.py` & `pyqqq-0.9.7/pyqqq/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/array.py` & `pyqqq-0.9.7/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/compute.py` & `pyqqq-0.9.7/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/display.py` & `pyqqq-0.9.7/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/kvstore.py` & `pyqqq-0.9.7/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/limiter.py` & `pyqqq-0.9.7/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/logger.py` & `pyqqq-0.9.7/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/market_schedule.py` & `pyqqq-0.9.7/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/mock_api.py` & `pyqqq-0.9.7/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/pyqqq/utils/retry.py` & `pyqqq-0.9.7/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.6/PKG-INFO` & `pyqqq-0.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.9.6
+Version: 0.9.7
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

