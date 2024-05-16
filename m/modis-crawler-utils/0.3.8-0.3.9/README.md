# Comparing `tmp/modis_crawler_utils-0.3.8.tar.gz` & `tmp/modis_crawler_utils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modis_crawler_utils-0.3.8.tar", max compression
+gzip compressed data, was "modis_crawler_utils-0.3.9.tar", max compression
```

## Comparing `modis_crawler_utils-0.3.8.tar` & `modis_crawler_utils-0.3.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1784 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/README.md
--rw-r--r--   0        0        0     1050 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/__init__.py
--rw-r--r--   0        0        0     1193 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/cloudflare_captcha_bypass.py
--rw-r--r--   0        0        0      262 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/credentials/__init__.py
--rw-r--r--   0        0        0     2962 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/credentials/credential.py
--rw-r--r--   0        0        0     5975 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/credentials/manager.py
--rw-r--r--   0        0        0     1263 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/credentials/store/__init__.py
--rw-r--r--   0        0        0     4407 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/credentials/store/local.py
--rw-r--r--   0        0        0     3533 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/credentials/store/talisman.py
--rw-r--r--   0        0        0        0 2023-12-05 13:00:03.996835 modis_crawler_utils-0.3.8/crawler_utils/deploy/__init__.py
--rw-r--r--   0        0        0      437 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/deploy/bump_version.py
--rw-r--r--   0        0        0     4155 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/deploy/create_egg.py
--rw-r--r--   0        0        0     3113 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/deploy/make_arguments_md_file.py
--rw-r--r--   0        0        0      533 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/domains.py
--rw-r--r--   0        0        0     1422 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/echo.py
--rw-r--r--   0        0        0      265 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/__init__.py
--rw-r--r--   0        0        0     8012 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter.py
--rw-r--r--   0        0        0     3040 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
--rw-r--r--   0        0        0     3961 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
--rw-r--r--   0        0        0      835 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
--rw-r--r--   0        0        0     5023 2023-12-05 13:00:03.944834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
--rw-r--r--   0        0        0     2167 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/items_pipeline.py
--rw-r--r--   0        0        0     1513 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/request_fingerprint.py
--rw-r--r--   0        0        0     3083 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/requests_middleware.py
--rw-r--r--   0        0        0     4314 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/storage.py
--rw-r--r--   0        0        0    29874 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/files.py
--rw-r--r--   0        0        0     5002 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/images.py
--rw-r--r--   0        0        0     2647 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/kafka.py
--rw-r--r--   0        0        0     3073 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/logstash.py
--rw-r--r--   0        0        0     1495 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/misc.py
--rw-r--r--   0        0        0     4862 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/mongodb.py
--rw-r--r--   0        0        0     4915 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/proxypy.py
--rw-r--r--   0        0        0        0 2023-12-05 13:00:03.996835 modis_crawler_utils-0.3.8/crawler_utils/social_media/__init__.py
--rw-r--r--   0        0        0    20503 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/social_media/items.py
--rw-r--r--   0        0        0     4274 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/socks.py
--rw-r--r--   0        0        0      499 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/splash_proxy.py
--rw-r--r--   0        0        0     1955 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/states/__init__.py
--rw-r--r--   0        0        0     4489 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/states/local_store.py
--rw-r--r--   0        0        0     7705 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/states/talisman_states_api.py
--rw-r--r--   0        0        0     4171 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/talisman_controller.py
--rw-r--r--   0        0        0     1255 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/talisman_job_env.py
--rw-r--r--   0        0        0    14744 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/talisman_proxy.py
--rw-r--r--   0        0        0     2332 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/talisman_spider_state.py
--rw-r--r--   0        0        0       60 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/text_captcha_bypass/__init__.py
--rw-r--r--   0        0        0     3369 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/text_captcha_bypass/captchaMiddleware.py
--rw-r--r--   0        0        0     2128 2023-12-05 13:00:03.948834 modis_crawler_utils-0.3.8/crawler_utils/text_captcha_bypass/captchaRule.py
--rw-r--r--   0        0        0      179 2023-12-05 13:00:03.952834 modis_crawler_utils-0.3.8/crawler_utils/timestamp.py
--rw-r--r--   0        0        0      635 2023-12-05 13:00:03.952834 modis_crawler_utils-0.3.8/crawler_utils/trust_level.py
--rw-r--r--   0        0        0      281 2023-12-05 13:00:03.952834 modis_crawler_utils-0.3.8/crawler_utils/uuid.py
--rw-r--r--   0        0        0     2332 2023-12-05 13:00:03.952834 modis_crawler_utils-0.3.8/crawler_utils/validate_input.py
--rw-r--r--   0        0        0     1499 2023-12-05 13:00:32.741194 modis_crawler_utils-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 modis_crawler_utils-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1784 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/README.md
+-rw-r--r--   0        0        0     1050 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/__init__.py
+-rw-r--r--   0        0        0     1193 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/cloudflare_captcha_bypass.py
+-rw-r--r--   0        0        0      262 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/credentials/__init__.py
+-rw-r--r--   0        0        0     2962 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/credentials/credential.py
+-rw-r--r--   0        0        0     5975 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/credentials/manager.py
+-rw-r--r--   0        0        0     1263 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/credentials/store/__init__.py
+-rw-r--r--   0        0        0     4407 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/credentials/store/local.py
+-rw-r--r--   0        0        0     3533 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/credentials/store/talisman.py
+-rw-r--r--   0        0        0        0 2023-12-21 14:45:02.506100 modis_crawler_utils-0.3.9/crawler_utils/deploy/__init__.py
+-rw-r--r--   0        0        0      437 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/deploy/bump_version.py
+-rw-r--r--   0        0        0     4155 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/deploy/create_egg.py
+-rw-r--r--   0        0        0     3113 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/deploy/make_arguments_md_file.py
+-rw-r--r--   0        0        0      533 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/domains.py
+-rw-r--r--   0        0        0     1422 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/echo.py
+-rw-r--r--   0        0        0      265 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     8012 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter.py
+-rw-r--r--   0        0        0     3040 2023-12-21 14:44:27.665688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py
+-rw-r--r--   0        0        0     3961 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py
+-rw-r--r--   0        0        0      835 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py
+-rw-r--r--   0        0        0     5023 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py
+-rw-r--r--   0        0        0     2167 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/items_pipeline.py
+-rw-r--r--   0        0        0     1513 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/request_fingerprint.py
+-rw-r--r--   0        0        0     3083 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/requests_middleware.py
+-rw-r--r--   0        0        0     4314 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/storage.py
+-rw-r--r--   0        0        0    29874 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/files.py
+-rw-r--r--   0        0        0     5002 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/images.py
+-rw-r--r--   0        0        0     2647 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/kafka.py
+-rw-r--r--   0        0        0     3073 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/logstash.py
+-rw-r--r--   0        0        0     1495 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/misc.py
+-rw-r--r--   0        0        0     4862 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/mongodb.py
+-rw-r--r--   0        0        0     4915 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/proxypy.py
+-rw-r--r--   0        0        0        0 2023-12-21 14:45:02.510100 modis_crawler_utils-0.3.9/crawler_utils/social_media/__init__.py
+-rw-r--r--   0        0        0    20677 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/social_media/items.py
+-rw-r--r--   0        0        0     4274 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/socks.py
+-rw-r--r--   0        0        0      499 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/splash_proxy.py
+-rw-r--r--   0        0        0     1955 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/states/__init__.py
+-rw-r--r--   0        0        0     4489 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/states/local_store.py
+-rw-r--r--   0        0        0     7705 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/states/talisman_states_api.py
+-rw-r--r--   0        0        0     4171 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/talisman_controller.py
+-rw-r--r--   0        0        0     1255 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/talisman_job_env.py
+-rw-r--r--   0        0        0    14744 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/talisman_proxy.py
+-rw-r--r--   0        0        0     2332 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/talisman_spider_state.py
+-rw-r--r--   0        0        0       60 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/text_captcha_bypass/__init__.py
+-rw-r--r--   0        0        0     3369 2023-12-21 14:44:27.669688 modis_crawler_utils-0.3.9/crawler_utils/text_captcha_bypass/captchaMiddleware.py
+-rw-r--r--   0        0        0     2128 2023-12-21 14:44:27.673688 modis_crawler_utils-0.3.9/crawler_utils/text_captcha_bypass/captchaRule.py
+-rw-r--r--   0        0        0      179 2023-12-21 14:44:27.673688 modis_crawler_utils-0.3.9/crawler_utils/timestamp.py
+-rw-r--r--   0        0        0      635 2023-12-21 14:44:27.673688 modis_crawler_utils-0.3.9/crawler_utils/trust_level.py
+-rw-r--r--   0        0        0      281 2023-12-21 14:44:27.673688 modis_crawler_utils-0.3.9/crawler_utils/uuid.py
+-rw-r--r--   0        0        0     2332 2023-12-21 14:44:27.673688 modis_crawler_utils-0.3.9/crawler_utils/validate_input.py
+-rw-r--r--   0        0        0     1499 2023-12-21 14:45:37.634517 modis_crawler_utils-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 modis_crawler_utils-0.3.9/PKG-INFO
```

### Comparing `modis_crawler_utils-0.3.8/README.md` & `modis_crawler_utils-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/__init__.py` & `modis_crawler_utils-0.3.9/crawler_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/cloudflare_captcha_bypass.py` & `modis_crawler_utils-0.3.9/crawler_utils/cloudflare_captcha_bypass.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/credentials/credential.py` & `modis_crawler_utils-0.3.9/crawler_utils/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/credentials/manager.py` & `modis_crawler_utils-0.3.9/crawler_utils/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/credentials/store/__init__.py` & `modis_crawler_utils-0.3.9/crawler_utils/credentials/store/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/credentials/store/local.py` & `modis_crawler_utils-0.3.9/crawler_utils/credentials/store/local.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/credentials/store/talisman.py` & `modis_crawler_utils-0.3.9/crawler_utils/credentials/store/talisman.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/deploy/create_egg.py` & `modis_crawler_utils-0.3.9/crawler_utils/deploy/create_egg.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/deploy/make_arguments_md_file.py` & `modis_crawler_utils-0.3.9/crawler_utils/deploy/make_arguments_md_file.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/domains.py` & `modis_crawler_utils-0.3.9/crawler_utils/domains.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/echo.py` & `modis_crawler_utils-0.3.9/crawler_utils/echo.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter_strategies/delta_fetch_items.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter_strategies/depth_based.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/dupefilter_strategies/drop_unproductive_requests.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/items_pipeline.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/items_pipeline.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/request_fingerprint.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/request_fingerprint.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/requests_middleware.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/requests_middleware.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/elasticsearch/storage.py` & `modis_crawler_utils-0.3.9/crawler_utils/elasticsearch/storage.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/files.py` & `modis_crawler_utils-0.3.9/crawler_utils/files.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/images.py` & `modis_crawler_utils-0.3.9/crawler_utils/images.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/kafka.py` & `modis_crawler_utils-0.3.9/crawler_utils/kafka.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/logstash.py` & `modis_crawler_utils-0.3.9/crawler_utils/logstash.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/misc.py` & `modis_crawler_utils-0.3.9/crawler_utils/misc.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/mongodb.py` & `modis_crawler_utils-0.3.9/crawler_utils/mongodb.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/proxypy.py` & `modis_crawler_utils-0.3.9/crawler_utils/proxypy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/social_media/items.py` & `modis_crawler_utils-0.3.9/crawler_utils/social_media/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 
 def class_output(item: BaseSMModel) -> dict:
     """
     Serializes item to dict, removing None or empty values
     """
     serialized_item = item.model_dump(by_alias=True)
     item.model_validate(serialized_item)  # to revalidate mutable fields, e.g. lists of attachments
+    if isinstance(item, SocialMediaItem) and not isinstance(item, SocialConnection):
+        serialized_item.setdefault('url', item.url)  # ensure sm entities have url field
     return compact(serialized_item)
 
 
 def list_of_types_output(list_of_objects: Sequence[BaseSMModel]) -> list[dict]:
     """
     Serializes list of items, removing None or empty values
     """
```

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/socks.py` & `modis_crawler_utils-0.3.9/crawler_utils/socks.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/states/__init__.py` & `modis_crawler_utils-0.3.9/crawler_utils/states/__init__.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/states/local_store.py` & `modis_crawler_utils-0.3.9/crawler_utils/states/local_store.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/states/talisman_states_api.py` & `modis_crawler_utils-0.3.9/crawler_utils/states/talisman_states_api.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/talisman_controller.py` & `modis_crawler_utils-0.3.9/crawler_utils/talisman_controller.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/talisman_job_env.py` & `modis_crawler_utils-0.3.9/crawler_utils/talisman_job_env.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/talisman_proxy.py` & `modis_crawler_utils-0.3.9/crawler_utils/talisman_proxy.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/talisman_spider_state.py` & `modis_crawler_utils-0.3.9/crawler_utils/talisman_spider_state.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/text_captcha_bypass/captchaMiddleware.py` & `modis_crawler_utils-0.3.9/crawler_utils/text_captcha_bypass/captchaMiddleware.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/text_captcha_bypass/captchaRule.py` & `modis_crawler_utils-0.3.9/crawler_utils/text_captcha_bypass/captchaRule.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/trust_level.py` & `modis_crawler_utils-0.3.9/crawler_utils/trust_level.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/crawler_utils/validate_input.py` & `modis_crawler_utils-0.3.9/crawler_utils/validate_input.py`

 * *Files identical despite different names*

### Comparing `modis_crawler_utils-0.3.8/pyproject.toml` & `modis_crawler_utils-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modis-crawler-utils"
-version = "0.3.8"
+version = "0.3.9"
 description = "Scrapy utils for Modis crawlers projects."
 authors = [
     "Varlamov <varlamov@ispras.ru>",
     "Yatskov <yatskov@ispras.ru>"
 ]
 readme = "README.md"
 repository = "https://gitlab.at.ispras.ru/crawlers/crawler-utils"
```

### Comparing `modis_crawler_utils-0.3.8/PKG-INFO` & `modis_crawler_utils-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modis-crawler-utils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Scrapy utils for Modis crawlers projects.
 Home-page: https://gitlab.at.ispras.ru/crawlers/crawler-utils
 License: BSD
 Author: Varlamov
 Author-email: varlamov@ispras.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

