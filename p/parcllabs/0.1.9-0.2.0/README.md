# Comparing `tmp/parcllabs-0.1.9.tar.gz` & `tmp/parcllabs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parcllabs-0.1.9.tar", last modified: Wed May  1 11:35:03 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `parcllabs-0.1.9.tar` & `parcllabs-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.201737 parcllabs-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 11:34:28.000000 parcllabs-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-01 11:35:03.201737 parcllabs-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-01 11:34:28.000000 parcllabs-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.197737 parcllabs-0.1.9/parcllabs/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/plabs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.197737 parcllabs-0.1.9/parcllabs/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/search/metros.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/search/top_markets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.201737 parcllabs-0.1.9/parcllabs/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-01 11:35:00.000000 parcllabs-0.1.9/parcllabs/services/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/for_sale_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/investor_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/portfolio_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/rental_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.201737 parcllabs-0.1.9/parcllabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:35:03.201737 parcllabs-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-01 11:34:28.000000 parcllabs-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.201737 parcllabs-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-01 11:34:28.000000 parcllabs-0.1.9/tests/test_for_sale_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-01 11:34:28.000000 parcllabs-0.1.9/tests/test_parcl_labs_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 11:34:28.000000 parcllabs-0.1.9/tests/test_parcl_labs_service.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/__version__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/common.py
+-rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/parcllabs_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/search/__init__.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/search/metros.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/search/top_markets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/__init__.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/for_sale_market_metrics.py
+-rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/investor_metrics.py
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/market_metrics.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/parcllabs_service.py
+-rw-r--r--   0        0        0    17702 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/portfolio_metrics.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/price_feed.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/rental_market_metrics.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 parcllabs-0.2.0/parcllabs/services/search.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 parcllabs-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 parcllabs-0.2.0/LICENSE
+-rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 parcllabs-0.2.0/README.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 parcllabs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16712 2020-02-02 00:00:00.000000 parcllabs-0.2.0/PKG-INFO
```

### Comparing `parcllabs-0.1.9/LICENSE` & `parcllabs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.9/parcllabs/plabs_client.py` & `parcllabs-0.2.0/parcllabs/parcllabs_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,153 @@
 import json
 import requests
 from typing import Dict
 from requests.exceptions import RequestException
 
 from parcllabs import api_base
 
+
+from parcllabs.services.price_feed import (
+    PriceFeedBase,
+)
+
 from parcllabs.services.investor_metrics import (
     InvestorMetricsHousingStockOwnership,
     InvesetorMetricsNewListingsForSaleRollingCounts,
     InvestorMetricsPurchaseToSaleRatio,
     InvestorMetricsHousingEventCounts,
+    InvestorMetricsHousingEventPrices,
 )
 
 from parcllabs.services.market_metrics import (
+    MarketMetricsAllCash,
     MarketMetricsHousingEventPrices,
     MarketMetricsHousingStock,
     MarketMetricsHousingEventCounts,
 )
 
 from parcllabs.services.for_sale_market_metrics import (
     ForSaleMarketMetricsNewListingsRollingCounts,
 )
 
 from parcllabs.services.rental_market_metrics import (
     RentalMarketMetricsRentalUnitsConcentration,
     RentalMarketMetricsGrossYield,
+    RentalMarketMetricsNewListingsForRentRollingCounts,
 )
 
-from parcllabs.services.portfolio_metrics import PortfolioMetricsSFHousingStockOwnership
+from parcllabs.services.portfolio_metrics import (
+    PortfolioMetricsSFHousingStockOwnership,
+    PortfolioMetricsSFNewListingsForSaleRollingCounts,
+    PortfolioMetricsSFHousingEventCounts,
+    PortfolioMetricsSFNewListingsForRentRollingCounts,
+)
 from parcllabs.services.search import SearchMarkets
 
 
 class ParclLabsClient:
-    def __init__(self, api_key: str):
-        if api_key is None:
+    def __init__(self, api_key: str, limit: int = 12):
+        """
+        Create a ParclLabsClient client.
+
+        Args:
+            api_key (str): A Parcl Labs API key.
+            limit (int, optional): The number of items to return per page. Defaults to 12.
+
+        Raises:
+            ValueError: If the API key is not provided.
+
+        """
+        if not api_key:
             raise ValueError(
                 "API Key is required. Please visit https://dashboard.parcllabs.com/signup to get an API key."
             )
+
         self.api_key = api_key
         self.api_url = api_base
+        self.limit = limit
+
+        # price feed services
+        self.price_feed = PriceFeedBase(
+            url="/v1/price_feed/{parcl_id}/price_feed", client=self
+        )
+        self.price_feed_volatility = PriceFeedBase(
+            url="/v1/price_feed/{parcl_id}/volatility", client=self
+        )
 
         # top-level services: The client is responsible for creating instances of these services
         self.investor_metrics_housing_stock_ownership = (
             InvestorMetricsHousingStockOwnership(client=self)
         )
         self.investor_metrics_new_listings_for_sale_rolling_counts = (
             InvesetorMetricsNewListingsForSaleRollingCounts(client=self)
         )
         self.investor_metrics_purchase_to_sale_ratio = (
             InvestorMetricsPurchaseToSaleRatio(client=self)
         )
         self.investor_metrics_housing_event_counts = InvestorMetricsHousingEventCounts(
             client=self
         )
+        self.investor_metrics_housing_event_prices = InvestorMetricsHousingEventPrices(
+            client=self
+        )
         self.market_metrics_housing_event_prices = MarketMetricsHousingEventPrices(
             client=self
         )
+        self.market_metrics_all_cash = MarketMetricsAllCash(client=self)
         self.market_metrics_housing_stock = MarketMetricsHousingStock(client=self)
         self.market_metrics_housing_event_counts = MarketMetricsHousingEventCounts(
             client=self
         )
         self.for_sale_market_metrics_new_listings_rolling_counts = (
             ForSaleMarketMetricsNewListingsRollingCounts(client=self)
         )
         self.rental_market_metrics_rental_units_concentration = (
             RentalMarketMetricsRentalUnitsConcentration(client=self)
         )
         self.rental_market_metrics_gross_yield = RentalMarketMetricsGrossYield(
             client=self
         )
+        self.rental_market_metrics_new_listings_for_rent_rolling_counts = (
+            RentalMarketMetricsNewListingsForRentRollingCounts(client=self)
+        )
         self.portfolio_metrics_sf_housing_stock_ownership = (
             PortfolioMetricsSFHousingStockOwnership(client=self)
         )
+        self.portfolio_metrics_new_listings_for_sale_rolling_counts = (
+            PortfolioMetricsSFNewListingsForSaleRollingCounts(client=self)
+        )
+        self.portfolio_metrics_sf_new_listings_for_rent_rolling_counts = (
+            PortfolioMetricsSFNewListingsForRentRollingCounts(client=self)
+        )
+        self.portfolio_metrics_sf_housing_event_counts = (
+            PortfolioMetricsSFHousingEventCounts(client=self)
+        )
         self.search_markets = SearchMarkets(client=self)
 
-    def get(self, url: str, params: dict = None):
+    def get(self, url: str, params: dict = None, is_next: bool = False):
         """
         Send a GET request to the specified URL with the given parameters.
 
         Args:
             url (str): The URL endpoint to request.
             params (dict, optional): The parameters to send in the query string.
 
         Returns:
             dict: The JSON response as a dictionary.
         """
+
+        if params:
+            if not params.get("limit"):
+                params["limit"] = self.limit
         try:
-            full_url = self.api_url + url
+            if is_next:
+                full_url = url
+            else:
+                full_url = self.api_url + url
             headers = self._get_headers()
             response = requests.get(full_url, headers=headers, params=params)
             response.raise_for_status()
             return response.json()
         except requests.exceptions.HTTPError:
             try:
                 error_details = response.json()
```

### Comparing `parcllabs-0.1.9/parcllabs/search/metros.py` & `parcllabs-0.2.0/parcllabs/search/metros.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.9/parcllabs/services/for_sale_market_metrics.py` & `parcllabs-0.2.0/parcllabs/services/for_sale_market_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Mapping, Optional, List
 
 import pandas as pd
 
-from parcllabs.services.base_service import ParclLabsService
+
+from parcllabs.services.parcllabs_service import ParclLabsService
 
 
 class ForSaleMarketMetricsNewListingsRollingCounts(ParclLabsService):
     """
     Gets weekly updated rolling counts of newly listed for sale properties, segmented into 7, 30, 60, and 90 day periods ending on a specified date, based on a given <parcl_id>.
     """
 
@@ -52,17 +53,14 @@
         property_type = self.validate_property_type(property_type)
         params = {
             "start_date": start_date,
             "end_date": end_date,
             "property_type": property_type,
             **(params or {}),
         }
-        results = {}
-        for parcl_id in parcl_ids:
-            results[parcl_id] = self.retrieve(parcl_id=parcl_id, params=params).get(
-                "items"
-            )
+
+        results, _ = self.retrieve_many_items(parcl_ids=parcl_ids, params=params)
 
         if as_dataframe:
             return self._as_pd_dataframe(results)
 
         return results
```

### Comparing `parcllabs-0.1.9/parcllabs/services/market_metrics.py` & `parcllabs-0.2.0/parcllabs/services/market_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,70 @@
 from typing import Any, Mapping, Optional, List
 
 import pandas as pd
 
-from parcllabs.services.base_service import ParclLabsService
+from parcllabs.services.parcllabs_service import ParclLabsService
+
+
+class MarketMetricsAllCash(ParclLabsService):
+    """
+    Gets monthly counts of all cash transactions and their percentage share of total sales, based on a specified <parcl_id> .
+    """
+
+    def retrieve(
+        self,
+        parcl_id: int,
+        start_date: str = None,
+        end_date: str = None,
+        property_type: str = None,
+        params: Optional[Mapping[str, Any]] = None,
+        as_dataframe: bool = False,
+    ):
+        start_date = self.validate_date(start_date)
+        end_date = self.validate_date(end_date)
+        property_type = self.validate_property_type(property_type)
+        params = {
+            "start_date": start_date,
+            "end_date": end_date,
+            "property_type": property_type,
+            **(params or {}),
+        }
+        results = self._request(
+            url=f"/v1/market_metrics/{parcl_id}/all_cash", params=params
+        )
+
+        if as_dataframe:
+            fmt = {results.get("parcl_id"): results.get("items")}
+            return self._as_pd_dataframe(fmt)
+        return results
+
+    def retrieve_many(
+        self,
+        parcl_ids: List[int],
+        start_date: str = None,
+        end_date: str = None,
+        property_type: str = None,
+        params: Optional[Mapping[str, Any]] = None,
+        as_dataframe: bool = False,
+    ):
+        start_date = self.validate_date(start_date)
+        end_date = self.validate_date(end_date)
+        property_type = self.validate_property_type(property_type)
+        params = {
+            "start_date": start_date,
+            "end_date": end_date,
+            "property_type": property_type,
+            **(params or {}),
+        }
+        results, _ = self.retrieve_many_items(parcl_ids=parcl_ids, params=params)
+
+        if as_dataframe:
+            return self._as_pd_dataframe(results)
+
+        return results
 
 
 class MarketMetricsHousingEventCounts(ParclLabsService):
     """
     Gets monthly counts of housing events, including sales, new sale listings, and new rental listings, based on a specified <parcl_id>.
     """
 
@@ -51,19 +109,15 @@
         property_type = self.validate_property_type(property_type)
         params = {
             "start_date": start_date,
             "end_date": end_date,
             "property_type": property_type,
             **(params or {}),
         }
-        results = {}
-        for parcl_id in parcl_ids:
-            results[parcl_id] = self.retrieve(parcl_id=parcl_id, params=params).get(
-                "items"
-            )
+        results, _ = self.retrieve_many_items(parcl_ids=parcl_ids, params=params)
 
         if as_dataframe:
             return self._as_pd_dataframe(results)
 
         return results
 
 
@@ -99,19 +153,15 @@
         end_date: str = None,
         params: Optional[Mapping[str, Any]] = None,
         as_dataframe: bool = False,
     ):
         start_date = self.validate_date(start_date)
         end_date = self.validate_date(end_date)
         params = {"start_date": start_date, "end_date": end_date, **(params or {})}
-        results = {}
-        for parcl_id in parcl_ids:
-            results[parcl_id] = self.retrieve(parcl_id=parcl_id, params=params).get(
-                "items"
-            )
+        results, _ = self.retrieve_many_items(parcl_ids=parcl_ids, params=params)
 
         if as_dataframe:
             return self._as_pd_dataframe(results)
 
         return results
 
 
@@ -243,15 +293,15 @@
                         "price_per_square_foot_percentile_80th_new_listings_for_sale": price_per_square_foot_percentile_80th_new_listings_for_sale,
                         "price_per_square_foot_percentile_80th_new_rental_listings": price_per_square_foot_percentile_80th_new_rental_listings,
                     },
                     index=[0],
                 )
                 tmp["parcl_id"] = k
                 out.append(tmp)
-        return pd.concat(out)
+        return pd.concat(out).reset_index(drop=True)
 
     def retrieve(
         self,
         parcl_id: int,
         start_date: str = None,
         end_date: str = None,
         property_type: str = None,
@@ -290,17 +340,13 @@
         property_type = self.validate_property_type(property_type)
         params = {
             "start_date": start_date,
             "end_date": end_date,
             "property_type": property_type,
             **(params or {}),
         }
-        results = {}
-        for parcl_id in parcl_ids:
-            results[parcl_id] = self.retrieve(parcl_id=parcl_id, params=params).get(
-                "items"
-            )
+        results, _ = self.retrieve_many_items(parcl_ids=parcl_ids, params=params)
 
         if as_dataframe:
             return self._as_pd_dataframe(results)
 
         return results
```

### Comparing `parcllabs-0.1.9/parcllabs/services/rental_market_metrics.py` & `parcllabs-0.2.0/parcllabs/services/rental_market_metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Mapping, Optional, List
 
-from parcllabs.services.base_service import ParclLabsService
+from parcllabs.services.parcllabs_service import ParclLabsService
 
 
 class RentalMarketMetricsGrossYield(ParclLabsService):
     """
     Gets weekly updated rolling counts of newly listed for sale properties, segmented into 7, 30, 60, and 90 day periods ending on a specified date, based on a given <parcl_id>.
     """
 
@@ -49,19 +49,15 @@
         property_type = self.validate_property_type(property_type)
         params = {
             "start_date": start_date,
             "end_date": end_date,
             "property_type": property_type,
             **(params or {}),
         }
-        results = {}
-        for parcl_id in parcl_ids:
-            results[parcl_id] = self.retrieve(parcl_id=parcl_id, params=params).get(
-                "items"
-            )
+        results, _ = self.retrieve_many_items(parcl_ids=parcl_ids, params=params)
 
         if as_dataframe:
             return self._as_pd_dataframe(results)
 
         return results
 
 
@@ -85,15 +81,15 @@
         params = {
             "start_date": start_date,
             "end_date": end_date,
             "property_type": property_type,
             **(params or {}),
         }
         results = self._request(
-            url=f"/v1/rental_market_metrics/{parcl_id}/rental_units_concentation",
+            url=f"/v1/rental_market_metrics/{parcl_id}/rental_units_concentration",
             params=params,
         )
 
         if as_dataframe:
             fmt = {results.get("parcl_id"): results.get("items")}
             return self._as_pd_dataframe(fmt)
         return results
@@ -112,17 +108,72 @@
         property_type = self.validate_property_type(property_type)
         params = {
             "start_date": start_date,
             "end_date": end_date,
             "property_type": property_type,
             **(params or {}),
         }
-        results = {}
-        for parcl_id in parcl_ids:
-            results[parcl_id] = self.retrieve(parcl_id=parcl_id, params=params).get(
-                "items"
-            )
+        results, _ = self.retrieve_many_items(parcl_ids=parcl_ids, params=params)
+
+        if as_dataframe:
+            return self._as_pd_dataframe(results)
+
+        return results
+
+
+class RentalMarketMetricsNewListingsForRentRollingCounts(ParclLabsService):
+    """
+    Gets weekly updated rolling counts of newly listed for sale properties, segmented into 7, 30, 60, and 90 day periods ending on a specified date, based on a given <parcl_id>.
+    """
+
+    def retrieve(
+        self,
+        parcl_id: int,
+        start_date: str = None,
+        end_date: str = None,
+        property_type: str = None,
+        params: Optional[Mapping[str, Any]] = None,
+        as_dataframe: bool = False,
+    ):
+        start_date = self.validate_date(start_date)
+        end_date = self.validate_date(end_date)
+        property_type = self.validate_property_type(property_type)
+        params = {
+            "start_date": start_date,
+            "end_date": end_date,
+            "property_type": property_type,
+            **(params or {}),
+        }
+        results = self._request(
+            url=f"/v1/rental_market_metrics/{parcl_id}/new_listings_for_rent_rolling_counts",
+            params=params,
+        )
+
+        if as_dataframe:
+            fmt = {results.get("parcl_id"): results.get("items")}
+            return self._as_pd_dataframe(fmt)
+        return results
+
+    def retrieve_many(
+        self,
+        parcl_ids: List[int],
+        start_date: str = None,
+        end_date: str = None,
+        property_type: str = None,
+        params: Optional[Mapping[str, Any]] = None,
+        as_dataframe: bool = False,
+    ):
+        start_date = self.validate_date(start_date)
+        end_date = self.validate_date(end_date)
+        property_type = self.validate_property_type(property_type)
+        params = {
+            "start_date": start_date,
+            "end_date": end_date,
+            "property_type": property_type,
+            **(params or {}),
+        }
+        results, _ = self.retrieve_many_items(parcl_ids=parcl_ids, params=params)
 
         if as_dataframe:
             return self._as_pd_dataframe(results)
 
         return results
```

