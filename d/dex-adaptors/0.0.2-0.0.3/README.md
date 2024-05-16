# Comparing `tmp/dex-adaptors-0.0.2.tar.gz` & `tmp/dex-adaptors-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dex-adaptors-0.0.2.tar", last modified: Wed May 15 03:43:25 2024, max compression
+gzip compressed data, was "dex-adaptors-0.0.3.tar", last modified: Thu May 16 04:08:51 2024, max compression
```

## Comparing `dex-adaptors-0.0.2.tar` & `dex-adaptors-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-05-15 03:43:25.800683 dex-adaptors-0.0.2/
--rw-r--r--   0 davidding   (501) staff       (20)      112 2024-05-15 03:43:25.800581 dex-adaptors-0.0.2/PKG-INFO
--rw-r--r--   0 davidding   (501) staff       (20)       14 2024-05-09 03:24:01.000000 dex-adaptors-0.0.2/README.md
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-05-15 03:43:25.797132 dex-adaptors-0.0.2/dex_adaptors/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)      260 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/aave_v3.py
--rw-r--r--   0 davidding   (501) staff       (20)      348 2024-05-15 03:39:03.000000 dex-adaptors-0.0.2/dex_adaptors/balancer_v2.py
--rw-r--r--   0 davidding   (501) staff       (20)      307 2024-05-15 03:39:03.000000 dex-adaptors-0.0.2/dex_adaptors/curve.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-05-15 03:43:25.799403 dex-adaptors-0.0.2/dex_adaptors/exchange/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/exchange/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)      679 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/exchange/aave_v3.py
--rw-r--r--   0 davidding   (501) staff       (20)      825 2024-05-15 03:39:03.000000 dex-adaptors-0.0.2/dex_adaptors/exchange/balancer_v2.py
--rw-r--r--   0 davidding   (501) staff       (20)     1924 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/exchange/base.py
--rw-r--r--   0 davidding   (501) staff       (20)      317 2024-05-15 03:39:03.000000 dex-adaptors-0.0.2/dex_adaptors/exchange/curve.py
--rw-r--r--   0 davidding   (501) staff       (20)     1839 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/exchange/morpho.py
--rw-r--r--   0 davidding   (501) staff       (20)      374 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/exchange/pendle.py
--rw-r--r--   0 davidding   (501) staff       (20)     3619 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/exchange/uniswap_v3.py
--rw-r--r--   0 davidding   (501) staff       (20)      666 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/morpho.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-05-15 03:43:25.800410 dex-adaptors-0.0.2/dex_adaptors/parsers/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/parsers/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)     1068 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/parsers/aave_v3.py
--rw-r--r--   0 davidding   (501) staff       (20)     1028 2024-05-15 03:39:03.000000 dex-adaptors-0.0.2/dex_adaptors/parsers/balancer_v2.py
--rw-r--r--   0 davidding   (501) staff       (20)      766 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/parsers/base.py
--rw-r--r--   0 davidding   (501) staff       (20)     1440 2024-05-15 03:39:03.000000 dex-adaptors-0.0.2/dex_adaptors/parsers/curve.py
--rw-r--r--   0 davidding   (501) staff       (20)     1633 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/parsers/morpho.py
--rw-r--r--   0 davidding   (501) staff       (20)     1929 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/parsers/pendle.py
--rw-r--r--   0 davidding   (501) staff       (20)     1762 2024-05-15 03:39:03.000000 dex-adaptors-0.0.2/dex_adaptors/parsers/uniswap_v3.py
--rw-r--r--   0 davidding   (501) staff       (20)      557 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/pendle.py
--rw-r--r--   0 davidding   (501) staff       (20)      869 2024-05-14 07:06:24.000000 dex-adaptors-0.0.2/dex_adaptors/uniswap_v3.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-05-15 03:43:25.797763 dex-adaptors-0.0.2/dex_adaptors.egg-info/
--rw-r--r--   0 davidding   (501) staff       (20)      112 2024-05-15 03:43:25.000000 dex-adaptors-0.0.2/dex_adaptors.egg-info/PKG-INFO
--rw-r--r--   0 davidding   (501) staff       (20)      906 2024-05-15 03:43:25.000000 dex-adaptors-0.0.2/dex_adaptors.egg-info/SOURCES.txt
--rw-r--r--   0 davidding   (501) staff       (20)        1 2024-05-15 03:43:25.000000 dex-adaptors-0.0.2/dex_adaptors.egg-info/dependency_links.txt
--rw-r--r--   0 davidding   (501) staff       (20)      320 2024-05-15 03:43:25.000000 dex-adaptors-0.0.2/dex_adaptors.egg-info/requires.txt
--rw-r--r--   0 davidding   (501) staff       (20)       13 2024-05-15 03:43:25.000000 dex-adaptors-0.0.2/dex_adaptors.egg-info/top_level.txt
--rw-r--r--   0 davidding   (501) staff       (20)      615 2024-05-09 03:24:01.000000 dex-adaptors-0.0.2/pyproject.toml
--rw-r--r--   0 davidding   (501) staff       (20)       38 2024-05-15 03:43:25.800723 dex-adaptors-0.0.2/setup.cfg
--rw-r--r--   0 davidding   (501) staff       (20)      380 2024-05-15 03:39:20.000000 dex-adaptors-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:08:51.035125 dex-adaptors-0.0.3/
+-rw-rw-rw-   0        0        0      118 2024-05-16 04:08:51.035125 dex-adaptors-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-05-10 08:02:18.000000 dex-adaptors-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 04:08:50.986656 dex-adaptors-0.0.3/dex_adaptors/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.3/dex_adaptors/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-05-13 11:38:21.000000 dex-adaptors-0.0.3/dex_adaptors/aave_v3.py
+-rw-rw-rw-   0        0        0      358 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/balancer_v2.py
+-rw-rw-rw-   0        0        0      353 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/compound_v2.py
+-rw-rw-rw-   0        0        0      317 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/curve.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:08:51.014368 dex-adaptors-0.0.3/dex_adaptors/exchange/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/__init__.py
+-rw-rw-rw-   0        0        0      705 2024-05-13 11:38:21.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/aave_v3.py
+-rw-rw-rw-   0        0        0      857 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/balancer_v2.py
+-rw-rw-rw-   0        0        0     1980 2024-05-13 11:35:28.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/base.py
+-rw-rw-rw-   0        0        0     1050 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/compound_v2.py
+-rw-rw-rw-   0        0        0      329 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/curve.py
+-rw-rw-rw-   0        0        0     1906 2024-05-13 01:53:02.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/morpho.py
+-rw-rw-rw-   0        0        0      386 2024-05-13 11:35:28.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/pendle.py
+-rw-rw-rw-   0        0        0     3746 2024-05-12 10:42:13.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/uniswap_v3.py
+-rw-rw-rw-   0        0        0      681 2024-05-13 01:53:02.000000 dex-adaptors-0.0.3/dex_adaptors/morpho.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:08:51.034123 dex-adaptors-0.0.3/dex_adaptors/parsers/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-05-13 11:38:21.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/aave_v3.py
+-rw-rw-rw-   0        0        0     1057 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/balancer_v2.py
+-rw-rw-rw-   0        0        0      798 2024-05-12 10:42:13.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/base.py
+-rw-rw-rw-   0        0        0     1096 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/compound_v2.py
+-rw-rw-rw-   0        0        0     1477 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/curve.py
+-rw-rw-rw-   0        0        0     1678 2024-05-13 01:53:02.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/morpho.py
+-rw-rw-rw-   0        0        0     1980 2024-05-13 11:35:28.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/pendle.py
+-rw-rw-rw-   0        0        0     1808 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/uniswap_v3.py
+-rw-rw-rw-   0        0        0      569 2024-05-13 11:35:28.000000 dex-adaptors-0.0.3/dex_adaptors/pendle.py
+-rw-rw-rw-   0        0        0      890 2024-05-12 10:42:13.000000 dex-adaptors-0.0.3/dex_adaptors/uniswap_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:08:51.000028 dex-adaptors-0.0.3/dex_adaptors.egg-info/
+-rw-rw-rw-   0        0        0      118 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1412 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2024-05-10 08:02:18.000000 dex-adaptors-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 04:08:51.035125 dex-adaptors-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-05-16 04:06:01.000000 dex-adaptors-0.0.3/setup.py
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/exchange/aave_v3.py` & `dex-adaptors-0.0.3/dex_adaptors/exchange/aave_v3.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from .base import GqlClient
-
-
-class AaveV3Unified(GqlClient):
-    BASE_ENDPOINT = "https://api.thegraph.com/subgraphs/name/aave/protocol-v3"
-
-    def __init__(self):
-        super().__init__(self.BASE_ENDPOINT)
-
-    async def _get_reserves(self, num: int = 1000):
-        query = f"""
-        query {{
-            reserves(first: {num}) {{
-                id
-                isActive
-                liquidityRate
-                name
-                stableBorrowRate
-                symbol
-                utilizationRate
-                variableBorrowRate
-                lastUpdateTimestamp
-            }}
-        }}
-        """
-        return await self.request(query=query)
+from .base import GqlClient
+
+
+class AaveV3Unified(GqlClient):
+    BASE_ENDPOINT = "https://api.thegraph.com/subgraphs/name/aave/protocol-v3"
+
+    def __init__(self):
+        super().__init__(self.BASE_ENDPOINT)
+
+    async def _get_reserves(self, num: int = 1000):
+        query = f"""
+        query {{
+            reserves(first: {num}) {{
+                id
+                isActive
+                liquidityRate
+                name
+                stableBorrowRate
+                symbol
+                utilizationRate
+                variableBorrowRate
+                lastUpdateTimestamp
+            }}
+        }}
+        """
+        return await self.request(query=query)
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/exchange/base.py` & `dex-adaptors-0.0.3/dex_adaptors/exchange/base.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import json
-
-from aiohttp import ClientResponse, ClientSession
-from gql import Client, gql
-from gql.transport.aiohttp import AIOHTTPTransport
-
-
-class GqlClient:
-    def __init__(self, base_endpoint: str):
-        self.base_endpoint = base_endpoint
-        self.transport = AIOHTTPTransport(url=self.base_endpoint)
-        self.client = Client(transport=self.transport, fetch_schema_from_transport=True)
-
-    async def request(self, query: str) -> dict:
-        query = gql(query)
-        return await self.handle_response(await self.client.execute_async(query))
-
-    async def handle_response(self, response: dict) -> dict:
-        return response
-
-
-class HttpsBase(object):
-    def __init__(self, base_endpoint: str):
-        self.session = ClientSession()
-        self.base_endpoint = base_endpoint
-
-    async def close(self):
-        await self.session.close()
-
-    async def get(self, url: str, **kwargs):
-        return await self._request("GET", url, **kwargs)
-
-    async def post(self):
-        pass
-
-    async def _request(self, method: str, url: str, **kwargs):
-        request_url = self.base_endpoint + url
-        if method == "GET":
-            async with self.session.get(request_url, **kwargs) as response:
-                return await self._handle_response(response)
-
-        elif method == "POST":
-            async with self.session.post(request_url, **kwargs) as response:
-                return await self._handle_response(response)
-        else:
-            raise ValueError(f"Invalid method: {method}")
-
-    async def _handle_response(self, response: ClientResponse) -> dict:
-        if response.status == 200:
-            try:
-                return await response.json()
-            except Exception as e:
-                print(e)
-                return json.loads(await response.text())
-        else:
-            raise Exception(f"Error {response.status} {response.reason} {await response.text()}")
+import json
+
+from aiohttp import ClientResponse, ClientSession
+from gql import Client, gql
+from gql.transport.aiohttp import AIOHTTPTransport
+
+
+class GqlClient:
+    def __init__(self, base_endpoint: str):
+        self.base_endpoint = base_endpoint
+        self.transport = AIOHTTPTransport(url=self.base_endpoint)
+        self.client = Client(transport=self.transport, fetch_schema_from_transport=True)
+
+    async def request(self, query: str) -> dict:
+        query = gql(query)
+        return await self.handle_response(await self.client.execute_async(query))
+
+    async def handle_response(self, response: dict) -> dict:
+        return response
+
+
+class HttpsBase(object):
+    def __init__(self, base_endpoint: str):
+        self.session = ClientSession()
+        self.base_endpoint = base_endpoint
+
+    async def close(self):
+        await self.session.close()
+
+    async def get(self, url: str, **kwargs):
+        return await self._request("GET", url, **kwargs)
+
+    async def post(self):
+        pass
+
+    async def _request(self, method: str, url: str, **kwargs):
+        request_url = self.base_endpoint + url
+        if method == "GET":
+            async with self.session.get(request_url, **kwargs) as response:
+                return await self._handle_response(response)
+
+        elif method == "POST":
+            async with self.session.post(request_url, **kwargs) as response:
+                return await self._handle_response(response)
+        else:
+            raise ValueError(f"Invalid method: {method}")
+
+    async def _handle_response(self, response: ClientResponse) -> dict:
+        if response.status == 200:
+            try:
+                return await response.json()
+            except Exception as e:
+                print(e)
+                return json.loads(await response.text())
+        else:
+            raise Exception(f"Error {response.status} {response.reason} {await response.text()}")
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/exchange/morpho.py` & `dex-adaptors-0.0.3/dex_adaptors/exchange/morpho.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from .base import GqlClient
-
-
-class MorphoUnified(GqlClient):
-    BASE_ENDPOINT = "https://blue-api.morpho.org/graphql"
-
-    def __init__(self):
-        super().__init__(self.BASE_ENDPOINT)
-
-    async def _get_vault_by_address(self, chain_id: str, address: str):
-        query = f"""
-        query {{
-            vaultByAddress(
-                address: "{address}"
-                chainId: {chain_id}
-            )
-            {{
-                id
-                state {{
-                    allocation {{
-                        market {{
-                            uniqueKey
-                        }}
-                        supplyCap
-                        supplyAssets
-                        supplyAssetsUsd
-                    }}
-                }}
-            }}
-        }}
-        """
-        return await self.request(query=query)
-
-    async def _get_markets_info(self) -> dict:
-        query = """
-        query {
-            markets {
-                items {
-                    uniqueKey
-                    lltv
-                    oracleAddress
-                    irmAddress
-                    loanAsset {
-                        address
-                        symbol
-                        decimals
-                    }
-                    collateralAsset {
-                        address
-                        symbol
-                        decimals
-                    }
-                    state {
-                        borrowApy
-                        borrowAssets
-                        borrowAssetsUsd
-                        supplyApy
-                        supplyAssets
-                        supplyAssetsUsd
-                        fee
-                        utilization
-                    }
-                }
-            }
-        }
-        """
-        return await self.request(query=query)
+from .base import GqlClient
+
+
+class MorphoUnified(GqlClient):
+    BASE_ENDPOINT = "https://blue-api.morpho.org/graphql"
+
+    def __init__(self):
+        super().__init__(self.BASE_ENDPOINT)
+
+    async def _get_vault_by_address(self, chain_id: str, address: str):
+        query = f"""
+        query {{
+            vaultByAddress(
+                address: "{address}"
+                chainId: {chain_id}
+            )
+            {{
+                id
+                state {{
+                    allocation {{
+                        market {{
+                            uniqueKey
+                        }}
+                        supplyCap
+                        supplyAssets
+                        supplyAssetsUsd
+                    }}
+                }}
+            }}
+        }}
+        """
+        return await self.request(query=query)
+
+    async def _get_markets_info(self) -> dict:
+        query = """
+        query {
+            markets {
+                items {
+                    uniqueKey
+                    lltv
+                    oracleAddress
+                    irmAddress
+                    loanAsset {
+                        address
+                        symbol
+                        decimals
+                    }
+                    collateralAsset {
+                        address
+                        symbol
+                        decimals
+                    }
+                    state {
+                        borrowApy
+                        borrowAssets
+                        borrowAssetsUsd
+                        supplyApy
+                        supplyAssets
+                        supplyAssetsUsd
+                        fee
+                        utilization
+                    }
+                }
+            }
+        }
+        """
+        return await self.request(query=query)
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/morpho.py` & `dex-adaptors-0.0.3/dex_adaptors/morpho.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from .exchange.morpho import MorphoUnified
-from .parsers.morpho import MorphoParser
-
-
-class Morpho(MorphoUnified, MorphoParser):
-    async def get_vault_by_address(self, chain: str, address: str) -> dict:
-        if chain not in self.CHAIN_ID_MAP.keys():
-            raise ValueError(f"Chain {chain} not supported. Supported chains: {self.CHAIN_ID_MAP.keys()}")
-        chain_id = self.CHAIN_ID_MAP[chain]
-
-        params = {"chain_id": chain_id, "address": address}
-        return self.parse_vault_by_address(await self._get_vault_by_address(**params))
-
-    async def get_exchange_info(self):
-        return self.parse_exchange_info(await self._get_markets_info())
+from .exchange.morpho import MorphoUnified
+from .parsers.morpho import MorphoParser
+
+
+class Morpho(MorphoUnified, MorphoParser):
+    async def get_vault_by_address(self, chain: str, address: str) -> dict:
+        if chain not in self.CHAIN_ID_MAP.keys():
+            raise ValueError(f"Chain {chain} not supported. Supported chains: {self.CHAIN_ID_MAP.keys()}")
+        chain_id = self.CHAIN_ID_MAP[chain]
+
+        params = {"chain_id": chain_id, "address": address}
+        return self.parse_vault_by_address(await self._get_vault_by_address(**params))
+
+    async def get_exchange_info(self):
+        return self.parse_exchange_info(await self._get_markets_info())
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/parsers/balancer_v2.py` & `dex-adaptors-0.0.3/dex_adaptors/parsers/balancer_v2.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from .base import Parser
-
-
-class BalancerV2Parser(Parser):
-    def __init__(self):
-        super().__init__(name="balancer_v2")
-
-    def parse_pool_data(self, response: dict) -> dict:
-        data = response["pool"]
-        return {
-            "timestamp": self.get_timestamp(),
-            "active": not data["isPaused"],
-            "instrument_id": data["symbol"],
-            "address": data["address"],
-            "symbol": data["name"],
-            "currency": [
-                {
-                    "symbol": currency["symbol"],
-                    "address": currency["address"],
-                    "decimals": self.parse_str(currency["decimals"], int),
-                    "price_usd": None,
-                    "liquidity": self.parse_str(currency["balance"], float),
-                }
-                for currency in data["tokens"]
-            ],
-            "pool_usd": self.parse_str(data["totalLiquidity"], float),
-            "updated_timestamp": self.get_timestamp(),
-            "raw_data": data,
-        }
+from .base import Parser
+
+
+class BalancerV2Parser(Parser):
+    def __init__(self):
+        super().__init__(name="balancer_v2")
+
+    def parse_pool_data(self, response: dict) -> dict:
+        data = response["pool"]
+        return {
+            "timestamp": self.get_timestamp(),
+            "active": not data["isPaused"],
+            "instrument_id": data["symbol"],
+            "address": data["address"],
+            "symbol": data["name"],
+            "currency": [
+                {
+                    "symbol": currency["symbol"],
+                    "address": currency["address"],
+                    "decimals": self.parse_str(currency["decimals"], int),
+                    "price_usd": None,
+                    "liquidity": self.parse_str(currency["balance"], float),
+                }
+                for currency in data["tokens"]
+            ],
+            "pool_usd": self.parse_str(data["totalLiquidity"], float),
+            "updated_timestamp": self.get_timestamp(),
+            "raw_data": data,
+        }
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/parsers/curve.py` & `dex-adaptors-0.0.3/dex_adaptors/parsers/compound_v2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,27 @@
-from .base import Parser
-
-
-class CurveParser(Parser):
-    def __init__(self):
-        super().__init__(name="curve")
-
-    def parse_pools(self, response: dict) -> dict:
-        updated_timestamp = response["generatedTimeMs"]
-        datas = response["data"]["poolData"]
-
-        results = {}
-        for data in datas:
-            instrument_id = data["name"]
-
-            results[instrument_id] = {
-                "timestamp": self.get_timestamp(),
-                "active": not data["isBroken"],
-                "instrument_id": instrument_id,
-                "address": data["address"].lower(),
-                "symbol": data["symbol"] if "symbol" in data else None,
-                "currency": [
-                    {
-                        "symbol": currency["symbol"],
-                        "address": currency["address"],
-                        "decimals": self.parse_str(currency["decimals"], int),
-                        "price_usd": self.parse_str(currency["usdPrice"], float),
-                        "liquidity": self.parse_str(currency["poolBalance"], float)
-                        / 10 ** self.parse_str(currency["decimals"], int),
-                    }
-                    for currency in data["coins"]
-                ],
-                "pool_usd": self.parse_str(data["usdTotal"], float),
-                "updated_timestamp": updated_timestamp,
-                "raw_data": data,
-            }
-        return results
+from .base import Parser
+
+
+class CompoundV2Parser(Parser):
+    def __init__(self):
+        super().__init__(name="compound_v2")
+
+    def parse_markets_data(self, response: dict) -> dict:
+        datas = response["markets"]
+
+        results = {}
+        for data in datas:
+            currency = data["underlyingSymbol"]
+            results[currency] = {
+                "timestamp": self.get_timestamp(),
+                "currency": currency,
+                "currency_address": data["underlyingAddress"],
+                "ctoken_symbol": data["symbol"],
+                "ctoken_address": data["id"],
+                "borrow_rate": self.parse_str(data["borrowRate"], float),
+                "supply_rate": self.parse_str(data["supplyRate"], float),
+                "total_borrowed": self.parse_str(data["totalBorrows"], float),
+                "total_supply": self.parse_str(data["totalSupply"], float),
+                "updated_timestamp": int(self.parse_str(data["blockTimestamp"], int) * 1000),
+                "raw_data": data,
+            }
+        return results
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/parsers/uniswap_v3.py` & `dex-adaptors-0.0.3/dex_adaptors/parsers/uniswap_v3.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from .base import Parser
-
-
-class UniswapV3Parser(Parser):
-    def __init__(self):
-        super().__init__(name="uniswap_v3")
-
-    @staticmethod
-    def parse_pool_name(datas: dict) -> str:
-        return f"{datas['token0']['symbol']}-{datas['token1']['symbol']}"
-
-    def parse_pool_data(self, response: dict) -> dict:
-        datas = response["pool"]
-        return {
-            "timestamp": self.get_timestamp(),
-            "pool_name": self.parse_pool_name(datas),
-            "pool_address": datas["id"],
-            "token1": {
-                "name": datas["token0"]["symbol"],
-                "address": datas["token0"]["id"],
-                "decimals": self.parse_str(datas["token0"]["decimals"], int),
-                "price": self.parse_str(datas["token0Price"], float),
-                "tvl": self.parse_str(datas["totalValueLockedToken0"], float),
-                "tvl_usd": None,
-            },
-            "token2": {
-                "name": datas["token1"]["symbol"],
-                "address": datas["token1"]["id"],
-                "decimals": self.parse_str(datas["token1"]["decimals"], int),
-                "price": self.parse_str(datas["token1Price"], float),
-                "tvl": self.parse_str(datas["totalValueLockedToken1"], float),
-                "tvl_usd": None,
-            },
-            "tvl_eth": self.parse_str(datas["totalValueLockedETH"], float),
-            "tvl_usd": self.parse_str(datas["totalValueLockedUSD"], float),
-            "raw_data": datas,
-        }
-
-    def parse_pool_token_candlesticks(self, response: dict) -> list:
-        datas = response["pool"]
-
-        return datas
-
-    def parse_pool_price_candlesticks(self, response: dict) -> list:
-        datas = response["poolDayDatas"]
-        return datas
+from .base import Parser
+
+
+class UniswapV3Parser(Parser):
+    def __init__(self):
+        super().__init__(name="uniswap_v3")
+
+    @staticmethod
+    def parse_pool_name(datas: dict) -> str:
+        return f"{datas['token0']['symbol']}-{datas['token1']['symbol']}"
+
+    def parse_pool_data(self, response: dict) -> dict:
+        datas = response["pool"]
+        return {
+            "timestamp": self.get_timestamp(),
+            "pool_name": self.parse_pool_name(datas),
+            "pool_address": datas["id"],
+            "token1": {
+                "name": datas["token0"]["symbol"],
+                "address": datas["token0"]["id"],
+                "decimals": self.parse_str(datas["token0"]["decimals"], int),
+                "price": self.parse_str(datas["token0Price"], float),
+                "tvl": self.parse_str(datas["totalValueLockedToken0"], float),
+                "tvl_usd": None,
+            },
+            "token2": {
+                "name": datas["token1"]["symbol"],
+                "address": datas["token1"]["id"],
+                "decimals": self.parse_str(datas["token1"]["decimals"], int),
+                "price": self.parse_str(datas["token1Price"], float),
+                "tvl": self.parse_str(datas["totalValueLockedToken1"], float),
+                "tvl_usd": None,
+            },
+            "tvl_eth": self.parse_str(datas["totalValueLockedETH"], float),
+            "tvl_usd": self.parse_str(datas["totalValueLockedUSD"], float),
+            "raw_data": datas,
+        }
+
+    def parse_pool_token_candlesticks(self, response: dict) -> list:
+        datas = response["pool"]
+
+        return datas
+
+    def parse_pool_price_candlesticks(self, response: dict) -> list:
+        datas = response["poolDayDatas"]
+        return datas
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/pendle.py` & `dex-adaptors-0.0.3/dex_adaptors/pendle.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .exchange.pendle import PendleUnified
-from .parsers.pendle import PendleParser
-
-
-class Pendle(PendleUnified, PendleParser):
-    async def get_market_by_address(self, chain: str, address: str) -> dict:
-        if chain not in self.CHAIN_ID_MAP.keys():
-            raise ValueError(f"Chain {chain} not supported. Supported chains: {self.CHAIN_ID_MAP.keys()}")
-        chain_id = self.CHAIN_ID_MAP[chain]
-
-        params = {"chain_id": chain_id, "address": address}
-        return self.parse_market_by_address(await self._get_market_by_address(**params))
+from .exchange.pendle import PendleUnified
+from .parsers.pendle import PendleParser
+
+
+class Pendle(PendleUnified, PendleParser):
+    async def get_market_by_address(self, chain: str, address: str) -> dict:
+        if chain not in self.CHAIN_ID_MAP.keys():
+            raise ValueError(f"Chain {chain} not supported. Supported chains: {self.CHAIN_ID_MAP.keys()}")
+        chain_id = self.CHAIN_ID_MAP[chain]
+
+        params = {"chain_id": chain_id, "address": address}
+        return self.parse_market_by_address(await self._get_market_by_address(**params))
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors/uniswap_v3.py` & `dex-adaptors-0.0.3/dex_adaptors/uniswap_v3.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from .exchange.uniswap_v3 import UniswapV3Unified
-from .parsers.uniswap_v3 import UniswapV3Parser
-
-
-class UniswapV3(UniswapV3Unified, UniswapV3Parser):
-    async def get_pool_data(self, pool_address: str) -> dict:
-        return self.parse_pool_data(await self._get_pool_data(address=pool_address))
-
-    async def get_pool_token_candlesticks(self, pool_address: str, num: int) -> list:
-        limit = 1000
-        results = self.parse_pool_token_candlesticks(
-            await self._get_pool_token_candlesticks(pool_address=pool_address, num=limit)
-        )
-        return results
-
-    async def get_pool_price_candlesticks(self, pool_address: str, num: int) -> list:
-        limit = 1000
-        results = self.parse_pool_price_candlesticks(
-            await self._get_pool_price_candlesticks(pool_address=pool_address, num=limit)
-        )
-        return results
+from .exchange.uniswap_v3 import UniswapV3Unified
+from .parsers.uniswap_v3 import UniswapV3Parser
+
+
+class UniswapV3(UniswapV3Unified, UniswapV3Parser):
+    async def get_pool_data(self, pool_address: str) -> dict:
+        return self.parse_pool_data(await self._get_pool_data(address=pool_address))
+
+    async def get_pool_token_candlesticks(self, pool_address: str, num: int) -> list:
+        limit = 1000
+        results = self.parse_pool_token_candlesticks(
+            await self._get_pool_token_candlesticks(pool_address=pool_address, num=limit)
+        )
+        return results
+
+    async def get_pool_price_candlesticks(self, pool_address: str, num: int) -> list:
+        limit = 1000
+        results = self.parse_pool_price_candlesticks(
+            await self._get_pool_price_candlesticks(pool_address=pool_address, num=limit)
+        )
+        return results
```

### Comparing `dex-adaptors-0.0.2/dex_adaptors.egg-info/SOURCES.txt` & `dex-adaptors-0.0.3/dex_adaptors.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 README.md
 pyproject.toml
 setup.py
 dex_adaptors/__init__.py
 dex_adaptors/aave_v3.py
 dex_adaptors/balancer_v2.py
+dex_adaptors/compound_v2.py
 dex_adaptors/curve.py
 dex_adaptors/morpho.py
 dex_adaptors/pendle.py
 dex_adaptors/uniswap_v3.py
 dex_adaptors.egg-info/PKG-INFO
 dex_adaptors.egg-info/SOURCES.txt
 dex_adaptors.egg-info/dependency_links.txt
 dex_adaptors.egg-info/requires.txt
 dex_adaptors.egg-info/top_level.txt
 dex_adaptors/exchange/__init__.py
 dex_adaptors/exchange/aave_v3.py
 dex_adaptors/exchange/balancer_v2.py
 dex_adaptors/exchange/base.py
+dex_adaptors/exchange/compound_v2.py
 dex_adaptors/exchange/curve.py
 dex_adaptors/exchange/morpho.py
 dex_adaptors/exchange/pendle.py
 dex_adaptors/exchange/uniswap_v3.py
 dex_adaptors/parsers/__init__.py
 dex_adaptors/parsers/aave_v3.py
 dex_adaptors/parsers/balancer_v2.py
 dex_adaptors/parsers/base.py
+dex_adaptors/parsers/compound_v2.py
 dex_adaptors/parsers/curve.py
 dex_adaptors/parsers/morpho.py
 dex_adaptors/parsers/pendle.py
 dex_adaptors/parsers/uniswap_v3.py
```

### Comparing `dex-adaptors-0.0.2/pyproject.toml` & `dex-adaptors-0.0.3/pyproject.toml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-[tool.black]
-line-length = 120
-include = "\\.pyi?$"
-exclude = """
-(
-   /(
-      \\.eggs         # exclude a few common directories in the
-    | \\.git          # root of the project
-    | \\.hg
-    | \\.mypy_cache
-    | \\.tox
-    | \\.venv
-    | _build
-    | buck-out
-    | build
-    | dist
-    )/
-)
-"""
-
-[tool.isort]
-# black compatibility
-profile = "black"
-# cuctom section
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
-known_third_party = []
-known_local_folder = []
-
-[tool.mypy]
-python_version = "3.10"
-warn_return_any = true
-warn_unused_configs = true
-ignore_missing_imports = true
+[tool.black]
+line-length = 120
+include = "\\.pyi?$"
+exclude = """
+(
+   /(
+      \\.eggs         # exclude a few common directories in the
+    | \\.git          # root of the project
+    | \\.hg
+    | \\.mypy_cache
+    | \\.tox
+    | \\.venv
+    | _build
+    | buck-out
+    | build
+    | dist
+    )/
+)
+"""
+
+[tool.isort]
+# black compatibility
+profile = "black"
+# cuctom section
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
+known_third_party = []
+known_local_folder = []
+
+[tool.mypy]
+python_version = "3.10"
+warn_return_any = true
+warn_unused_configs = true
+ignore_missing_imports = true
```

