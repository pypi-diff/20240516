# Comparing `tmp/cdnmon-0.4.1.tar.gz` & `tmp/cdnmon-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.4.1.tar", max compression
+gzip compressed data, was "cdnmon-0.5.0.tar", max compression
```

## Comparing `cdnmon-0.4.1.tar` & `cdnmon-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0     1098 2024-05-15 01:02:08.908555 cdnmon-0.4.1/README.md
--rw-r--r--   0        0        0     1610 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/__init__.py
--rw-r--r--   0        0        0     5532 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/__init__.py
--rw-r--r--   0        0        0      338 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/advancedhosting.py
--rw-r--r--   0        0        0     1766 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/akamai.py
--rw-r--r--   0        0        0     7896 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/alibaba_cdn.py
--rw-r--r--   0        0        0      980 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/alibaba_dcdn.py
--rw-r--r--   0        0        0      543 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/alibaba_waf.py
--rw-r--r--   0        0        0      302 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/asia_isp.py
--rw-r--r--   0        0        0      390 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/baidu.py
--rw-r--r--   0        0        0      342 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/baishan.py
--rw-r--r--   0        0        0      205 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/beluga.py
--rw-r--r--   0        0        0      292 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/bunny.py
--rw-r--r--   0        0        0      211 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cachefly.py
--rw-r--r--   0        0        0      202 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cdn77.py
--rw-r--r--   0        0        0      217 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cdnetworks.py
--rw-r--r--   0        0        0      211 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cdnvideo.py
--rw-r--r--   0        0        0      217 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/chinacache.py
--rw-r--r--   0        0        0     1087 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cloudflare.py
--rw-r--r--   0        0        0     1283 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cloudfront.py
--rw-r--r--   0        0        0      359 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/ctyun.py
--rw-r--r--   0        0        0      202 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/dnion.py
--rw-r--r--   0        0        0      324 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/douyin.py
--rw-r--r--   0        0        0      307 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/edgecast.py
--rw-r--r--   0        0        0      211 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/edgenext.py
--rw-r--r--   0        0        0      202 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/edgio.py
--rw-r--r--   0        0        0     1549 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/fastly.py
--rw-r--r--   0        0        0      309 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/fastly_edge_compute.py
--rw-r--r--   0        0        0      350 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/frontdoor.py
--rw-r--r--   0        0        0     1481 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/gcore.py
--rw-r--r--   0        0        0     1620 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/google.py
--rw-r--r--   0        0        0     5969 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/huawei.py
--rw-r--r--   0        0        0      208 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/imperva.py
--rw-r--r--   0        0        0      307 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/incapsula.py
--rw-r--r--   0        0        0      470 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/jingdong.py
--rw-r--r--   0        0        0      295 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/keycdn.py
--rw-r--r--   0        0        0      375 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/kingsoft.py
--rw-r--r--   0        0        0      227 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/leaseweb.py
--rw-r--r--   0        0        0      218 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/lumen.py
--rw-r--r--   0        0        0     1438 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/maxcdn.py
--rw-r--r--   0        0        0      230 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/medianova.py
--rw-r--r--   0        0        0      311 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/qiniu.py
--rw-r--r--   0        0        0      230 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/tata_communications.py
--rw-r--r--   0        0        0      883 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/tencent.py
--rw-r--r--   0        0        0      407 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/ucloud.py
--rw-r--r--   0        0        0      328 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/upyun.py
--rw-r--r--   0        0        0      224 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/verizon.py
--rw-r--r--   0        0        0      318 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/volc.py
--rw-r--r--   0        0        0      748 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/wangsu.py
--rw-r--r--   0        0        0      691 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/util/aws.py
--rw-r--r--   0        0        0      897 2024-05-15 01:02:08.912555 cdnmon-0.4.1/cdnmon/util/bgpview.py
--rw-r--r--   0        0        0      389 2024-05-15 01:02:08.912555 cdnmon-0.4.1/cdnmon/util/cidr.py
--rw-r--r--   0        0        0      436 2024-05-15 01:02:08.912555 cdnmon-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 cdnmon-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      636 2024-05-15 11:44:57.697212 cdnmon-0.5.0/README.md
+-rw-r--r--   0        0        0      536 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/__init__.py
+-rw-r--r--   0        0        0     6863 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/__init__.py
+-rw-r--r--   0        0        0      338 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/advancedhosting.py
+-rw-r--r--   0        0        0     1766 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/akamai.py
+-rw-r--r--   0        0        0     7896 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/alibaba_cdn.py
+-rw-r--r--   0        0        0      980 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/alibaba_dcdn.py
+-rw-r--r--   0        0        0      543 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/alibaba_waf.py
+-rw-r--r--   0        0        0      302 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/asia_isp.py
+-rw-r--r--   0        0        0      390 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/baidu.py
+-rw-r--r--   0        0        0      342 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/baishan.py
+-rw-r--r--   0        0        0      205 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/beluga.py
+-rw-r--r--   0        0        0      292 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/bunny.py
+-rw-r--r--   0        0        0      211 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/cachefly.py
+-rw-r--r--   0        0        0      202 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/cdn77.py
+-rw-r--r--   0        0        0      217 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/cdnetworks.py
+-rw-r--r--   0        0        0      211 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/cdnvideo.py
+-rw-r--r--   0        0        0      217 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/chinacache.py
+-rw-r--r--   0        0        0     1087 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/cloudflare.py
+-rw-r--r--   0        0        0     1283 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/cloudfront.py
+-rw-r--r--   0        0        0      359 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/ctyun.py
+-rw-r--r--   0        0        0      202 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/dnion.py
+-rw-r--r--   0        0        0      324 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/douyin.py
+-rw-r--r--   0        0        0      307 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/edgecast.py
+-rw-r--r--   0        0        0      211 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/edgenext.py
+-rw-r--r--   0        0        0      202 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/edgio.py
+-rw-r--r--   0        0        0     1549 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/fastly.py
+-rw-r--r--   0        0        0      309 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/fastly_edge_compute.py
+-rw-r--r--   0        0        0      350 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/frontdoor.py
+-rw-r--r--   0        0        0     1481 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/gcore.py
+-rw-r--r--   0        0        0     1620 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/google.py
+-rw-r--r--   0        0        0     5969 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/huawei.py
+-rw-r--r--   0        0        0      208 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/imperva.py
+-rw-r--r--   0        0        0      307 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/incapsula.py
+-rw-r--r--   0        0        0      470 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/jingdong.py
+-rw-r--r--   0        0        0      295 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/keycdn.py
+-rw-r--r--   0        0        0      375 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/kingsoft.py
+-rw-r--r--   0        0        0      227 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/leaseweb.py
+-rw-r--r--   0        0        0      218 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/lumen.py
+-rw-r--r--   0        0        0     1438 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/maxcdn.py
+-rw-r--r--   0        0        0      230 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/medianova.py
+-rw-r--r--   0        0        0      311 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/qiniu.py
+-rw-r--r--   0        0        0      230 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/tata_communications.py
+-rw-r--r--   0        0        0      883 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/tencent.py
+-rw-r--r--   0        0        0      407 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/ucloud.py
+-rw-r--r--   0        0        0      328 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/upyun.py
+-rw-r--r--   0        0        0      224 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/verizon.py
+-rw-r--r--   0        0        0      318 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/volc.py
+-rw-r--r--   0        0        0      748 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/model/cdn/wangsu.py
+-rw-r--r--   0        0        0      691 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/util/aws.py
+-rw-r--r--   0        0        0     1076 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/util/bgpview.py
+-rw-r--r--   0        0        0      389 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/util/cidr.py
+-rw-r--r--   0        0        0      258 2024-05-15 11:44:57.701212 cdnmon-0.5.0/cdnmon/util/db.py
+-rw-r--r--   0        0        0      513 2024-05-15 11:44:57.701212 cdnmon-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 cdnmon-0.5.0/PKG-INFO
```

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/__init__.py` & `cdnmon-0.5.0/cdnmon/model/cdn/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import datetime
 import functools
 import ipaddress
 import os
+import sys
 import tempfile
 from dataclasses import dataclass
 from dataclasses import field
 from typing import List
 
+import humanize
 import requests
 import yaml
+from loguru import logger
 
 from cdnmon.util import bgpview
+from cdnmon.util import db
 from cdnmon.util.cidr import deduplicate_networks
 
+logger.remove()
+logger.add(sys.stderr, level="INFO")
+
 
 class ETL:
     def extract(self):
         raise NotImplementedError
 
     def transform(self, data):
         raise NotImplementedError
@@ -34,15 +41,19 @@
 
     @functools.lru_cache(maxsize=None)
     def http_get(self, url):
         headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
             "Chrome/107.0.0.0 Safari/537.36 "
         }
-        return requests.get(url, headers=headers)
+        response = requests.get(url, headers=headers)
+        logger.info(
+            f"{response.status_code} {response.reason} | GET {url}  ({humanize.naturalsize(len(response.content))} Bytes)"
+        )
+        return response
 
 
 class BGPViewCIDR(CIDR):
     def __init__(self, query_term_list: List[str] = []):
         self.query_term_list = query_term_list
         self.bgpview_client = bgpview.BGPViewClient()
 
@@ -64,29 +75,48 @@
 
 
 @dataclass
 class CNAMEPattern:
     suffix: str = ""
     pattern: str = ""
     source: str = ""
-    examples: list[str] = field(default_factory=list)
 
     def __str__(self) -> str:
         return self.suffix
 
     def __repr__(self) -> str:
         return self.suffix
 
     def marshal(self) -> dict:
         return {
             "suffix": self.suffix,
             "pattern": self.pattern,
             "source": self.source,
-            "examples": self.examples,
+            "subscribers": self.subscribers(),
+        }
+
+    def subscribers(self) -> List[str]:
+        if not os.getenv("MONGODB_URI"):
+            logger.warning("MONGODB_URI is not set")
+            return []
+
+        suffix = self.suffix if self.suffix.endswith(".") else self.suffix + "."
+        pattern = f'^{suffix[::-1].replace(".", chr(92)+".")}'
+        filter = {
+            "task.qtype": "A",
+            "task.dns.response.answers.cname_reverse": {"$regex": pattern},
+            "task.dns.response.answers.a": {"$exists": True, "$ne": []},
         }
+        collection = db.get_mongo_collection("kepler", "dns")
+        domain_set = set()
+        for item in collection.find(filter).limit(1):
+            qname = item["task"]["qname"]
+            logger.warning("{} | {}", qname, self.suffix)
+            domain_set.add(qname)
+        return list(domain_set)
 
 
 @dataclass
 class CommonCDN:
     name: str
     asn_patterns: list[str] = field(default_factory=list)
     cname_suffixes: list[CNAMEPattern] = field(default_factory=list)
@@ -105,14 +135,21 @@
 
     def ipv4_prefixes(self) -> List[str]:
         return self.cidr.ipv4_prefixes()
 
     def ipv6_prefixes(self) -> List[str]:
         return self.cidr.ipv6_prefixes()
 
+    def subscribers(self) -> List[str]:
+        results = set()
+        for cname_suffix in self.cname_suffixes:
+            for subscriber in cname_suffix.subscribers():
+                results.add(subscriber)
+        return list(results)
+
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
 
     def dump(self) -> bool:
```

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/akamai.py` & `cdnmon-0.5.0/cdnmon/model/cdn/akamai.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/alibaba_cdn.py` & `cdnmon-0.5.0/cdnmon/model/cdn/alibaba_cdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/alibaba_dcdn.py` & `cdnmon-0.5.0/cdnmon/model/cdn/alibaba_dcdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/alibaba_waf.py` & `cdnmon-0.5.0/cdnmon/model/cdn/alibaba_waf.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/cloudflare.py` & `cdnmon-0.5.0/cdnmon/model/cdn/cloudflare.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/cloudfront.py` & `cdnmon-0.5.0/cdnmon/model/cdn/cloudfront.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/fastly.py` & `cdnmon-0.5.0/cdnmon/model/cdn/fastly.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/gcore.py` & `cdnmon-0.5.0/cdnmon/model/cdn/gcore.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/google.py` & `cdnmon-0.5.0/cdnmon/model/cdn/google.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/huawei.py` & `cdnmon-0.5.0/cdnmon/model/cdn/huawei.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/maxcdn.py` & `cdnmon-0.5.0/cdnmon/model/cdn/maxcdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/tencent.py` & `cdnmon-0.5.0/cdnmon/model/cdn/tencent.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/model/cdn/wangsu.py` & `cdnmon-0.5.0/cdnmon/model/cdn/wangsu.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.1/cdnmon/util/aws.py` & `cdnmon-0.5.0/cdnmon/util/aws.py`

 * *Files identical despite different names*

