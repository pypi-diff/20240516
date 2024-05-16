# Comparing `tmp/epicstore_api-0.1.7.tar.gz` & `tmp/epicstore_api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epicstore_api-0.1.7.tar", last modified: Sun Oct  8 19:20:22 2023, max compression
+gzip compressed data, was "epicstore_api-0.1.8.tar", last modified: Thu May 16 15:32:52 2024, max compression
```

## Comparing `epicstore_api-0.1.7.tar` & `epicstore_api-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-10-08 19:20:22.440441 epicstore_api-0.1.7/
--rw-rw-rw-   0        0        0     1081 2020-10-09 18:33:41.000000 epicstore_api-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     2574 2023-10-08 19:20:22.440441 epicstore_api-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1619 2022-11-21 17:13:50.000000 epicstore_api-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-10-08 19:20:22.435935 epicstore_api-0.1.7/epicstore_api/
--rw-rw-rw-   0        0        0      299 2023-04-29 14:21:08.000000 epicstore_api-0.1.7/epicstore_api/__init__.py
--rw-rw-rw-   0        0        0    19008 2023-10-08 19:11:17.000000 epicstore_api-0.1.7/epicstore_api/api.py
--rw-rw-rw-   0        0        0     1769 2023-04-29 14:21:08.000000 epicstore_api-0.1.7/epicstore_api/exc.py
-drwxrwxrwx   0        0        0        0 2023-10-08 19:20:22.438935 epicstore_api-0.1.7/epicstore_api/models/
--rw-rw-rw-   0        0        0     1258 2023-04-29 14:21:08.000000 epicstore_api-0.1.7/epicstore_api/models/__init__.py
--rw-rw-rw-   0        0        0     2739 2023-04-29 14:21:08.000000 epicstore_api-0.1.7/epicstore_api/models/categories.py
--rw-rw-rw-   0        0        0     1846 2023-04-29 14:21:08.000000 epicstore_api-0.1.7/epicstore_api/models/collection_types.py
--rw-rw-rw-   0        0        0     1475 2023-04-29 14:21:08.000000 epicstore_api-0.1.7/epicstore_api/models/product_types.py
--rw-rw-rw-   0        0        0    18275 2023-04-29 14:21:08.000000 epicstore_api-0.1.7/epicstore_api/queries.py
-drwxrwxrwx   0        0        0        0 2023-10-08 19:20:22.437935 epicstore_api-0.1.7/epicstore_api.egg-info/
--rw-rw-rw-   0        0        0     2574 2023-10-08 19:20:22.000000 epicstore_api-0.1.7/epicstore_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-10-08 19:20:22.000000 epicstore_api-0.1.7/epicstore_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-08 19:20:22.000000 epicstore_api-0.1.7/epicstore_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-10-08 19:20:22.000000 epicstore_api-0.1.7/epicstore_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-10-08 19:20:22.000000 epicstore_api-0.1.7/epicstore_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-08 19:20:22.440441 epicstore_api-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1294 2023-10-08 19:13:13.000000 epicstore_api-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:32:52.631311 epicstore_api-0.1.8/
+-rw-rw-rw-   0        0        0     1081 2020-10-09 18:33:41.000000 epicstore_api-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2574 2024-05-16 15:32:52.630310 epicstore_api-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1619 2022-11-21 17:13:50.000000 epicstore_api-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 15:32:52.622309 epicstore_api-0.1.8/epicstore_api/
+-rw-rw-rw-   0        0        0      308 2024-05-16 15:30:58.000000 epicstore_api-0.1.8/epicstore_api/__init__.py
+-rw-rw-rw-   0        0        0    18838 2024-05-16 15:30:58.000000 epicstore_api-0.1.8/epicstore_api/api.py
+-rw-rw-rw-   0        0        0     1726 2024-05-16 15:30:58.000000 epicstore_api-0.1.8/epicstore_api/exc.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:32:52.629310 epicstore_api-0.1.8/epicstore_api/models/
+-rw-rw-rw-   0        0        0     1288 2024-05-16 15:30:58.000000 epicstore_api-0.1.8/epicstore_api/models/__init__.py
+-rw-rw-rw-   0        0        0     2697 2024-05-16 15:30:58.000000 epicstore_api-0.1.8/epicstore_api/models/categories.py
+-rw-rw-rw-   0        0        0     1822 2024-05-16 15:30:58.000000 epicstore_api-0.1.8/epicstore_api/models/collection_types.py
+-rw-rw-rw-   0        0        0     1424 2024-05-16 15:30:58.000000 epicstore_api-0.1.8/epicstore_api/models/product_types.py
+-rw-rw-rw-   0        0        0    18237 2024-05-16 15:30:58.000000 epicstore_api-0.1.8/epicstore_api/queries.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:32:52.627310 epicstore_api-0.1.8/epicstore_api.egg-info/
+-rw-rw-rw-   0        0        0     2574 2024-05-16 15:32:52.000000 epicstore_api-0.1.8/epicstore_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2024-05-16 15:32:52.000000 epicstore_api-0.1.8/epicstore_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:32:52.000000 epicstore_api-0.1.8/epicstore_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 15:32:52.000000 epicstore_api-0.1.8/epicstore_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-16 15:32:52.000000 epicstore_api-0.1.8/epicstore_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:32:52.631311 epicstore_api-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1303 2024-05-16 15:32:04.000000 epicstore_api-0.1.8/setup.py
```

### Comparing `epicstore_api-0.1.7/LICENSE` & `epicstore_api-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `epicstore_api-0.1.7/PKG-INFO` & `epicstore_api-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: epicstore_api
-Version: 0.1.7
+Version: 0.1.8
 Summary: An API wrapper for Epic Games Store written in Python
 Home-page: https://github.com/SD4RK/epicstore_api
-Download-URL: https://github.com/SD4RK/epicstore_api/archive/v_0.1.7.tar.gz
+Download-URL: https://github.com/SD4RK/epicstore_api/archive/v_0.1.8.tar.gz
 Author: SD4RK
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `epicstore_api-0.1.7/README.md` & `epicstore_api-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `epicstore_api-0.1.7/epicstore_api/api.py` & `epicstore_api-0.1.8/epicstore_api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-"""
-MIT License
+"""MIT License.
 
 Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -20,31 +17,34 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-
 import json
+from typing import NamedTuple
+
 import requests
-from typing import Union, List, NamedTuple
-from .exc import EGSNotFound, EGSException
-from .models import EGSCategory, EGSProductType, EGSCollectionType
-from .queries import (CATALOG_QUERY,
-                      PROMOTIONS_QUERY,
-                      CATALOG_TAGS_QUERY,
-                      FEED_QUERY,
-                      PREREQUISITES_QUERY,
-                      OFFERS_QUERY,
-                      STORE_QUERY,
-                      ADDONS_QUERY,
-                      MEDIA_QUERY,
-                      PRODUCT_REVIEWS_QUERY,
-                      COLLECTION_QUERY)
+
+from epicstore_api.exc import EGSException, EGSNotFound
+from epicstore_api.models import EGSCategory, EGSCollectionType, EGSProductType
+from epicstore_api.queries import (
+    ADDONS_QUERY,
+    CATALOG_QUERY,
+    CATALOG_TAGS_QUERY,
+    COLLECTION_QUERY,
+    FEED_QUERY,
+    MEDIA_QUERY,
+    OFFERS_QUERY,
+    PREREQUISITES_QUERY,
+    PRODUCT_REVIEWS_QUERY,
+    PROMOTIONS_QUERY,
+    STORE_QUERY,
+)
 
 
 class OfferData(NamedTuple):
     namespace: str
     offer_id: str
 
 
@@ -54,152 +54,141 @@
 def _clean_1004_errors(raw):
     # On some responses EGS API returns 1004 errors for no reason, however the responses being sent are valid otherwise.
     # Official launcher ignores those errors, so we probably should do that as well. That function cleans up the mess
     # from raw response so error handling is still possible.
     if 'errors' in raw:
         for error in raw['errors'].copy():
             service_response = json.loads(error.get('serviceResponse', {}))
-            if service_response:
-                if service_response.get('numericErrorCode') == 1004:
-                    raw['errors'].remove(error)
+            if service_response and service_response.get('numericErrorCode') == 1004:
+                raw['errors'].remove(error)
         if not raw['errors']:
             raw.pop('errors')
     return raw
 
 
 class EpicGamesStoreAPI:
-    """
-    Class for interacting with EGS web API without user credentials TODO?
-    """
-    def __init__(self, locale="en-US", country="US", session=None):
-        """
-        :param locale: EGS locale (this parameter depends on responses locale)
+    """Class for interacting with EGS web API without user credentials TODO?."""
+
+    def __init__(self, locale="en-US", country="US", session=None) -> None:
+        """:param locale: EGS locale (this parameter depends on responses locale)
         :param country: EGS country
         """
         self._session = requests.Session() or session
         self.locale = locale
         self.country = country
 
     def get_product_mapping(self) -> dict:
         """Returns product mapping in {namespace: slug} format."""
-        return self._make_api_query(
-            '/content/productmapping', method='GET'
-        )
+        return self._make_api_query('/content/productmapping', method='GET')
 
     def get_product(self, slug: str) -> dict:
         """Returns a product's data by slug.
 
         :param slug: Product's slug.
         """
         return self._make_api_query(
-            f'/content/products/{slug}', method='GET', use_locale=True
+            f'/content/products/{slug}',
+            method='GET',
+            use_locale=True,
         )
 
     def get_store(self) -> dict:
         """Returns a JSON data about store page."""
-        return self._make_api_query(
-            '/content/store', method='GET', use_locale=True
-        )
+        return self._make_api_query('/content/store', method='GET', use_locale=True)
 
-    def get_free_games(self, allow_countries: str = None) -> dict:
+    def get_free_games(self, allow_countries: str | None = None) -> dict:
         """Returns the games from "Free Games" section in the EGS."""
         if allow_countries is None:
             allow_countries = self.country
         api_uri = (
             'https://store-site-backend-static.ak.epicgames.com/'
-            'freeGamesPromotions?locale={}&country={}&allowCountries={}'
+            f'freeGamesPromotions?locale={self.locale}&country={self.country}&allowCountries={allow_countries}'
         )
-        api_uri = api_uri.format(self.locale, self.country, allow_countries)
         data = _clean_1004_errors(self._session.get(api_uri).json())
         self._get_errors(data)
         return data
 
     def get_mver_status(self) -> bool:
-        return self._make_api_query(
-            '/mver-status', method='GET'
-        )['result']
+        return self._make_api_query('/mver-status', method='GET')['result']
 
     def get_epic_store_status(self) -> dict:
         """Returns an Epic Games Store server status."""
         return self._session.get(
-            'https://status.epicgames.com/api/v2/status.json'
+            'https://status.epicgames.com/api/v2/status.json',
         ).json()
 
     def get_offers_data(
         self,
         *offers: OfferData,
         should_calculate_tax: bool = False,
-        include_sub_items: bool = False
+        include_sub_items: bool = False,
     ) -> dict:
         """Get offer(s) full data by offers' id and namespace.
 
         :param offers: Offers you need to get data from.
         :param should_calculate_tax: Should EGS API calculate tax for offers?
         :param include_sub_items: Should EGS API include sub-items for offers?
         """
         return self._make_graphql_query(
             OFFERS_QUERY,
             {},
-            *[{
-                'productNamespace': offer.namespace,
-                'offerId': offer.offer_id,
-                'lineOffers': [{
+            *[
+                {
+                    'productNamespace': offer.namespace,
                     'offerId': offer.offer_id,
-                    'quantity': 1
-                }],
-                'calculateTax': should_calculate_tax,
-                'includeSubItems': include_sub_items
-            } for offer in offers]
+                    'lineOffers': [{'offerId': offer.offer_id, 'quantity': 1}],
+                    'calculateTax': should_calculate_tax,
+                    'includeSubItems': include_sub_items,
+                }
+                for offer in offers
+            ],
         )
 
     def get_collection(self, collection: EGSCollectionType) -> dict:
         """Returns games from the collection by the given collection type
         (see the documentation for CollectionType class).
 
         :param collection: Needed collection type.
         """
         # Cleanup for the 1004 errors that always pop up by default to not mess someone up by this.
-        raw = _clean_1004_errors(self._make_graphql_query(
-            COLLECTION_QUERY,
-            slug=collection.value,
-            # This query always returns 1004 error by default. That is not controlled by us and the error itself
-            # is happening even in the official EGS client itself, they're just ignoring it, so we will too.
-            suppress_errors=True
-        ))
-        return raw
+        return _clean_1004_errors(
+            self._make_graphql_query(
+                COLLECTION_QUERY,
+                slug=collection.value,
+                # This query always returns 1004 error by default. That is not controlled by us and the error itself
+                # is happening even in the official EGS client itself, they're just ignoring it, so we will too.
+                suppress_errors=True,
+            ),
+        )
 
     def fetch_media(self, media_ref_id: str) -> dict:
         """Returns media-file (type of the file, its url and so on) by the
         file's media ref ID.
 
         :param media_ref_id: File's media ref ID.
         """
-        return self._make_graphql_query(
-            MEDIA_QUERY,
-            mediaRefId=media_ref_id
-        )
+        return self._make_graphql_query(MEDIA_QUERY, mediaRefId=media_ref_id)
 
     def fetch_multiple_media_files(self, *media_ref_ids: str):
         """Equivalent to `fetch_media` function, except this one can fetch
-        a few media files at the same moment (using only one request)."""
+        a few media files at the same moment (using only one request).
+        """
         return self._make_graphql_query(
             MEDIA_QUERY,
             {},
-            *[{
-                'mediaRefId': media_ref_id
-            } for media_ref_id in media_ref_ids]
+            *[{'mediaRefId': media_ref_id} for media_ref_id in media_ref_ids],
         )
 
     def get_addons_by_namespace(
         self,
         namespace: str,
         categories: str = 'addons|digitalextras',
         count: int = 250,
         sort_by: str = 'releaseDate',
-        sort_dir: str = 'DESC'
+        sort_dir: str = 'DESC',
     ):
         """Returns product's addons by product's namespace.
 
         :param namespace: Product's namespace, can be obtained using the
         :meth:`epicstore_api.api.EpicGamesStoreAPI.get_product` function.
 
         :param categories: Addon's categories.
@@ -208,107 +197,99 @@
         :param sort_dir: You can use only **ASC** or **DESC**:
 
         - **ASC**: Sorts from higher ``sort_by`` parameter to lower;
         - **DESC**: Sorts from lower ``sort_by`` parameter to higher.
         """
         sort_dir = sort_dir.upper()
         if sort_dir not in ('ASC', 'DESC'):
-            raise ValueError(f'Parameter ``sort_dir`` have to be equals to'
-                             f' ASC or DESC, not to {sort_dir}')
+            msg = (
+                f'Parameter ``sort_dir`` have to be equals to'
+                f' ASC or DESC, not to {sort_dir}'
+            )
+            raise ValueError(
+                msg,
+            )
         return self._make_graphql_query(
             ADDONS_QUERY,
             namespace=namespace,
             count=count,
             categories=categories,
             sortBy=sort_by,
-            sortDir=sort_dir
+            sortDir=sort_dir,
         )
 
     def get_product_reviews(self, product_sku: str) -> dict:
         """Returns product's reviews by product's sku.
 
         :param product_sku: SKU of the Product. Usually just slug of the
-        product with `EPIC_` prefix."""
+        product with `EPIC_` prefix.
+        """
         try:
-            return self._make_graphql_query(
-                PRODUCT_REVIEWS_QUERY,
-                sku=product_sku
-            )
+            return self._make_graphql_query(PRODUCT_REVIEWS_QUERY, sku=product_sku)
         except EGSNotFound as exc:
             exc.message = (
                 'There are no reviews for this product, '
                 f'or the given sku ({product_sku}) is incorrect.'
             )
             raise
 
     def fetch_prerequisites(self, *offers: OfferData) -> dict:
-        """Fetches offer(s) prerequisites
+        """Fetches offer(s) prerequisites.
 
         :param offers: Offer(s) we need to get prerequisites from
         """
         return self._make_graphql_query(
             PREREQUISITES_QUERY,
-            offerParams=[{
-                'offerId': offer.offer_id,
-                'namespace': offer.namespace
-            } for offer in offers]  # OfferData -> dict for every offer in list
+            offerParams=[
+                {'offerId': offer.offer_id, 'namespace': offer.namespace}
+                for offer in offers
+            ],  # OfferData -> dict for every offer in list
         )
 
-    def fetch_feed(
-        self,
-        offset: int = 0,
-        count: int = 10,
-        category: str = ''
-    ) -> dict:
+    def fetch_feed(self, offset: int = 0, count: int = 10, category: str = '') -> dict:
         """Fetches Epic Games Store feed by given params.
 
         :param offset: From which news (index) we need to start.
         :param count: Count of the news we need to fetch.
         :param category: News categories.
         """
         return self._make_graphql_query(
             FEED_QUERY,
             offset=offset,
             countryCode=self.country,
             postsPerPage=count,
-            category=category
+            category=category,
         )
 
     def fetch_catalog_tags(self, namespace: str = 'epic') -> dict:
-        """Fetches tags for a products with namespace ``namespace``
+        """Fetches tags for a products with namespace ``namespace``.
 
         :param namespace: Products' namespace (**epic** = all)
         """
-        return self._make_graphql_query(
-            CATALOG_TAGS_QUERY,
-            namespace=namespace
-        )
+        return self._make_graphql_query(CATALOG_TAGS_QUERY, namespace=namespace)
 
     def fetch_promotions(self, namespace: str = 'epic') -> dict:
         """Fetches a global promotions.
 
         :param namespace: Products' namespace (**epic** = all).
         """
-        return self._make_graphql_query(
-            PROMOTIONS_QUERY,
-            namespace=namespace
-        )
+        return self._make_graphql_query(PROMOTIONS_QUERY, namespace=namespace)
 
     def fetch_catalog(
         self,
         count: int = 30,
-        product_type: Union[EGSProductType, str] = EGSProductType.ALL_PRODUCTS,
+        product_type: EGSProductType | str = EGSProductType.ALL_PRODUCTS,
         namespace: str = 'epic',
         sort_by: str = 'effectiveDate',
         sort_dir: str = 'DESC',
         start: int = 0,
         keywords: str = '',
-        categories: List[EGSCategory] = None
+        categories: list[EGSCategory] | str | None = None,
     ) -> dict:
-        """Fetches a catalog with given parameters
+        """Fetches a catalog with given parameters.
 
         :param count: Count of  products you need to fetch.
         :param product_type: Product type(s) you need to get from EGS.
         :param namespace: Products namespace (epic = all namespaces).
         :param sort_by: Parameter which EGS will use to sort products.
         :param sort_dir: You can use only **ASC** or **DESC**:
 
@@ -319,16 +300,21 @@
         :param keywords: Search keywords.
         :param categories: Categories you need to fetch.
         :rtype: dict
         :raises: ValueError  if ``sort_by`` not equals to **ASC** or **DESC**.
         """
         sort_dir = sort_dir.upper()
         if sort_dir not in ('ASC', 'DESC'):
-            raise ValueError(f'Parameter ``sort_dir`` have to be equals to'
-                             f' ASC or DESC, not to {sort_dir}')
+            msg = (
+                f'Parameter ``sort_dir`` have to be equals to'
+                f' ASC or DESC, not to {sort_dir}'
+            )
+            raise ValueError(
+                msg,
+            )
         if categories is None:
             categories = ''
         else:
             categories = EGSCategory.join_categories(*categories)
         if isinstance(product_type, EGSProductType):
             product_type = product_type.value
         return self._make_graphql_query(
@@ -336,32 +322,33 @@
             count=count,
             category=product_type,
             namespace=namespace,
             sortBy=sort_by,
             sortDir=sort_dir,
             start=start,
             keywords=keywords,
-            tag=categories
+            tag=categories,
         )
 
     def fetch_store_games(
         self,
         count: int = 30,
-        product_type: Union[EGSProductType, str] = EGSProductType.ALL_PRODUCTS,
+        product_type: EGSProductType | str = EGSProductType.ALL_PRODUCTS,
         allow_countries: str = 'US',
         namespace: str = '',
         sort_by: str = 'title',
         sort_dir: str = 'ASC',
-        release_date: str = None,
+        release_date: str | None = None,
         start: int = 0,
         keywords: str = '',
-        categories: List[EGSCategory] = None,
-        with_price: bool = True
+        categories: list[EGSCategory] | str | None = None,
+        *,
+        with_price: bool = True,
     ) -> dict:
-        """Fetches a store games with given parameters
+        """Fetches a store games with given parameters.
 
         :param count: Count of  products you need to fetch.
         :param product_type: Product type(s) you need to get from EGS.
         :param allow_countries: Products in the country. Default to 'US'.
         :param namespace: Products namespace ('' = all namespaces).
         :param sort_by: Parameter which EGS will use to sort products:
 
@@ -384,16 +371,21 @@
         :param categories: Categories you need to fetch.
         :param with_price: To fetch price or not.
         :rtype: dict
         :raises: ValueError  if ``sort_by`` not equals to **ASC** or **DESC**.
         """
         sort_dir = sort_dir.upper()
         if sort_dir not in ('ASC', 'DESC'):
-            raise ValueError(f'Parameter ``sort_dir`` have to be equals to'
-                             f' ASC or DESC, not to {sort_dir}')
+            msg = (
+                f'Parameter ``sort_dir`` have to be equals to'
+                f' ASC or DESC, not to {sort_dir}'
+            )
+            raise ValueError(
+                msg,
+            )
         if categories is None:
             categories = ''
         else:
             categories = EGSCategory.join_categories(*categories)
         if isinstance(product_type, EGSProductType):
             product_type = product_type.value
         return self._make_graphql_query(  # This type of fetch needs headers.
@@ -405,45 +397,46 @@
             namespace=namespace,
             sortBy=sort_by,
             sortDir=sort_dir,
             releaseDate=release_date,
             start=start,
             keywords=keywords,
             tag=categories,
-            withPrice=with_price
+            withPrice=with_price,
         )
 
     def _make_api_query(
         self,
         endpoint: str,
         method: str,
+        *,
         use_locale: bool = False,
-        **variables
+        **variables,
     ) -> dict:
         func = getattr(self._session, method.lower())
         base_url = 'https://store-content.ak.epicgames.com'
         base_url += '/api' if not use_locale else f'/api/{self.locale}'
-        response = func(
-            base_url + endpoint,
-            data=variables
-        )
+        response = func(base_url + endpoint, data=variables)
         if response.status_code == 404:
-            raise EGSException(f'Page with endpoint {endpoint} was not found')
+            msg = f'Page with endpoint {endpoint} was not found'
+            raise EGSException(msg)
         response = response.json()
         self._get_errors(response)
         return response
 
     def _make_graphql_query(
         self,
         query_string,
-        headers={},
-        suppress_errors=False,
+        headers=None,
         *multiple_query_variables,
-        **variables
+        suppress_errors=False,
+        **variables,
     ) -> dict:
+        if headers is None:
+            headers = {}
         if not multiple_query_variables:
             variables.update({'locale': self.locale, 'country': self.country})
             # This variables are default and exist in all graphql queries
             response = self._session.post(
                 'https://graphql.epicgames.com/graphql',
                 json={'query': query_string, 'variables': variables},
                 headers=headers,
@@ -452,50 +445,47 @@
             data = []
             for variables in multiple_query_variables:
                 variables_ = {
                     'locale': self.locale,
                     'country': self.country,
                 }
                 variables_.update(variables)
-                data.append({
-                    'query': query_string,
-                    'variables': variables_
-                })
+                data.append({'query': query_string, 'variables': variables_})
             response = self._session.post(
                 'https://graphql.epicgames.com/graphql',
                 json=data,
-                headers=headers
+                headers=headers,
             ).json()
         if not suppress_errors:
             self._get_errors(response)
         return response
 
     @staticmethod
-    def _get_errors(resp):
+    def _get_errors(resp) -> None:
         r = []
         if not isinstance(resp, list):
             r.append(resp)
         for response in r:
             if response.get('errors'):
                 error = response['errors'][0]
                 if not error['serviceResponse']:
-                    raise EGSException(
-                        error['message'],
-                        service_response=error
-                    )
-                service_response = json.loads(
-                    error['serviceResponse']
-                )
+                    raise EGSException(error['message'], service_response=error)
+                service_response = json.loads(error['serviceResponse'])
                 if isinstance(service_response, dict):
                     if service_response['errorCode'].endswith('not_found'):
                         raise EGSNotFound(
                             service_response['errorMessage'],
                             service_response['numericErrorCode'],
-                            service_response
-                        )
-                elif isinstance(service_response, str):
-                    if service_response == 'not found':
-                        raise EGSNotFound(
-                            'The resource was not found, '
-                            'No more data provided by Epic Games Store.'
+                            service_response,
                         )
+                elif (
+                    isinstance(service_response, str)
+                    and service_response == 'not found'
+                ):
+                    msg = (
+                        'The resource was not found, '
+                        'No more data provided by Epic Games Store.'
+                    )
+                    raise EGSNotFound(
+                        msg,
+                    )
                 # FIXME: Need to handle more errors than the code is handling now
```

### Comparing `epicstore_api-0.1.7/epicstore_api/exc.py` & `epicstore_api-0.1.8/epicstore_api/exc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-"""
-MIT License
+"""MIT License.
 
 Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -22,28 +19,24 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 
 class EGSException(Exception):
-    """
-    Class for EGS errors, all data about error is placed in ``exception_data``
-    """
-    def __init__(self, message, error_code=None, service_response=None):
+    """Class for EGS errors, all data about error is placed in ``exception_data``."""
+
+    def __init__(self, message, error_code=None, service_response=None) -> None:
         super().__init__(message)
         self.message = (
             f'Error code: '
             f'{error_code if error_code is not None else "unknown"}. '
             f'{message.capitalize()}'
         )
         self.exception_data = service_response
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.message
 
 
 class EGSNotFound(EGSException):
-    """
-    All errors which error code ends with `not_found`
-    """
-    pass
+    """All errors which error code ends with `not_found`."""
```

### Comparing `epicstore_api-0.1.7/epicstore_api/models/__init__.py` & `epicstore_api-0.1.8/epicstore_api/models/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-"""
-MIT License
+"""MIT License.
 
 Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -20,11 +17,10 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-
-from .categories import EGSCategory
-from .product_types import EGSProductType
-from .collection_types import EGSCollectionType
+from epicstore_api.models.categories import EGSCategory
+from epicstore_api.models.collection_types import EGSCollectionType
+from epicstore_api.models.product_types import EGSProductType
```

### Comparing `epicstore_api-0.1.7/epicstore_api/models/categories.py` & `epicstore_api-0.1.8/epicstore_api/models/categories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-"""
-MIT License
+"""MIT License.
 
 Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -20,28 +17,27 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-
 from enum import Enum
 
 
 class EGSCategory(Enum):
-    """
-    Class that provides a code for every category in the EGS with
-    a human-readable name and a few useful methods
+    """Class that provides a code for every category in the EGS with
+    a human-readable name and a few useful methods.
 
     .. note::
       Here you can see only that categories that are displayed in EGS,
       for other categories you can call an API function
       :meth:`epicstore_api.api.EpicGamesStoreAPI.fetch_catalog_tags`
     """
+
     CATEGORY_ACTION = "1216"  #: Action games
     CATEGORY_EDITOR = "9559"  #: Editors for games
     CATEGORY_ADVENTURE = "1117"  #: Adventure games
     CATEGORY_PUZZLE = "1298"  #: Puzzle games
     CATEGORY_RACING = "1212"  #: Racing games
     CATEGORY_RPG = "1367"  #: RPG games
     CATEGORY_SHOOTER = "1210"  #: Shooter games
@@ -50,19 +46,18 @@
     CATEGORY_OSX = "9548"  #: Games for OSX (Mac OS)
     CATEGORY_WINDOWS = "9547"  #: Games for Windows
     CATEGORY_SINGLE_PLAYER = "1370"  #: Single-player games
     CATEGORY_MULTIPLAYER = "1203"  #: Multiplayer games
 
     @staticmethod
     def join_categories(*categories_list) -> str:
-        """
-        Joins the given categories into a string for EGS API queries
+        """Joins the given categories into a string for EGS API queries
         :param categories_list: list of categories you need
         :type categories_list: List[EGSCategory]
-        :rtype: str
+        :rtype: str.
         """
         return '|'.join([category.value for category in categories_list])
 
     def __add__(self, other):
         if isinstance(other, EGSCategory):
             return self.join_categories(self, other)
         raise NotImplementedError
```

### Comparing `epicstore_api-0.1.7/epicstore_api/models/collection_types.py` & `epicstore_api-0.1.8/epicstore_api/models/collection_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-"""
-MIT License
+"""MIT License.
 
 Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -20,23 +17,23 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-
 from enum import Enum
 
 
 class EGSCollectionType(Enum):
     """A helper enum that is used for the collections query
     (see :meth:`epicstore_api.api.EpicGamesStoreAPI.get_collection`). You can see the game that fall under particular
     collections under the free games on the main page of the Epic Games Store. Collections that are not included
     (such as New Releases and Coming Soon can be obtained through catalog query with specific sort queries such as
-    sortBy=releaseDate and sortBy=comingSoon)."""
+    sortBy=releaseDate and sortBy=comingSoon).
+    """
+
     TOP_SELLERS = "top-sellers"
     MOST_PLAYED = "most-played"
     TOP_UPCOMING_WISHLISTED = "top-wishlisted"
     MOST_POPULAR = "most-popular"
     TOP_PLAYER_RATED = "top-player-reviewed"
-
```

### Comparing `epicstore_api-0.1.7/epicstore_api/models/product_types.py` & `epicstore_api-0.1.8/epicstore_api/models/product_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-"""
-MIT License
+"""MIT License.
 
 Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -20,20 +17,17 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-
 from enum import Enum
 
 
 class EGSProductType(Enum):
     PRODUCT_ENGINE = "engines"  #: Engines for developing games
     PRODUCT_GAME = "games"  #: Games
     PRODUCT_BUNDLE = "bundles"  #: An EGS bundle
-    ALL_PRODUCTS = "|".join([
-        PRODUCT_ENGINE,
-        PRODUCT_GAME,
-        PRODUCT_BUNDLE
-    ])  #: All possible products
+    ALL_PRODUCTS = (
+        f"{PRODUCT_ENGINE}|{PRODUCT_GAME}|{PRODUCT_BUNDLE}"  #: All possible products
+    )
```

### Comparing `epicstore_api-0.1.7/epicstore_api/queries.py` & `epicstore_api-0.1.8/epicstore_api/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-"""
-MIT License
+"""MIT License.
 
 Copyright (c) 2020-2023 SD4RK
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -20,20 +17,19 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-
 CATALOG_QUERY = "\n            query catalogQuery(\n                $category:String,\n                $count:Int,\n                $country:String!,\n                $keywords: String,\n                $locale:String,\n                $namespace:String!,\n                $sortBy:String,\n                $sortDir:String,\n                $start:Int,\n                $tag:String\n            ) {\n                Catalog {\n                    catalogOffers(\n                        namespace: $namespace,\n                        locale: $locale,\n                        params: {\n                            count: $count,\n                            country: $country,\n                            category: $category,\n                            keywords: $keywords,\n                            sortBy: $sortBy,\n                            sortDir: $sortDir,\n                            start: $start,\n                            tag: $tag\n                        }\n                    ) {\n                        elements {\n                            isFeatured\n                            collectionOfferIds\n                            \n          title\n          id\n          namespace\n          description\n          keyImages {\n            type\n            url\n          }\n          seller {\n              id\n              name\n          }\n          productSlug\n          urlSlug\n          items {\n            id\n            namespace\n          }\n          customAttributes {\n            key\n            value\n          }\n          categories {\n            path\n          }\n          price(country: $country) {\n            totalPrice {\n              discountPrice\n              originalPrice\n              voucherDiscount\n              discount\n              fmtPrice(locale: $locale) {\n                originalPrice\n                discountPrice\n                intermediatePrice\n              }\n            }\n            lineOffers {\n              appliedRules {\n                id\n                endDate\n              }\n            }\n          }\n          linkedOfferId\n          linkedOffer {\n            effectiveDate\n            customAttributes {\n              key\n              value\n            }\n          }\n        \n                        }\n                        paging {\n                            count,\n                            total\n                        }\n                    }\n                }\n            }\n        "
 STORE_QUERY = "query searchStoreQuery($allowCountries: String, $category: String, $count: Int, $country: String!, $keywords: String, $locale: String, $namespace: String, $itemNs: String, $sortBy: String, $sortDir: String, $start: Int, $tag: String, $releaseDate: String, $withPrice: Boolean = false, $withPromotions: Boolean = false) {\n  Catalog {\n    searchStore(allowCountries: $allowCountries, category: $category, count: $count, country: $country, keywords: $keywords, locale: $locale, namespace: $namespace, itemNs: $itemNs, sortBy: $sortBy, sortDir: $sortDir, releaseDate: $releaseDate, start: $start, tag: $tag) {\n      elements {\n        title\n        id\n        namespace\n        description\n        effectiveDate\n        keyImages {\n          type\n          url\n        }\n        seller {\n          id\n          name\n        }\n        productSlug\n        urlSlug\n        url\n        tags {\n          id\n        }\n        items {\n          id\n          namespace\n        }\n        customAttributes {\n          key\n          value\n        }\n        categories {\n          path\n        }\n        price(country: $country) @include(if: $withPrice) {\n          totalPrice {\n            discountPrice\n            originalPrice\n            voucherDiscount\n            discount\n            currencyCode\n            currencyInfo {\n              decimals\n            }\n            fmtPrice(locale: $locale) {\n              originalPrice\n              discountPrice\n              intermediatePrice\n            }\n          }\n          lineOffers {\n            appliedRules {\n              id\n              endDate\n              discountSetting {\n                discountType\n              }\n            }\n          }\n        }\n        promotions(category: $category) @include(if: $withPromotions) {\n          promotionalOffers {\n            promotionalOffers {\n              startDate\n              endDate\n              discountSetting {\n                discountType\n                discountPercentage\n              }\n            }\n          }\n          upcomingPromotionalOffers {\n            promotionalOffers {\n              startDate\n              endDate\n              discountSetting {\n                discountType\n                discountPercentage\n              }\n            }\n          }\n        }\n      }\n      paging {\n        count\n        total\n      }\n    }\n  }\n}\n"
-PROMOTIONS_QUERY = "\n          query promotionsQuery($namespace: String!, $country: String!, $locale: String!) {\n            Catalog {\n              catalogOffers(namespace: $namespace, locale: $locale, params: {category: \"freegames\", country: $country, sortBy: \"effectiveDate\", sortDir: \"asc\"}) {\n                elements {\n                  title\n                  description\n                  id\n                  namespace\n                  categories {\n                    path\n                  }\n                  linkedOfferNs\n                  linkedOfferId\n                  keyImages {\n                    type\n                    url\n                  }\n                  productSlug\n                  promotions {\n                    promotionalOffers {\n                      promotionalOffers {\n                        startDate\n                        endDate\n                        discountSetting {\n                          discountType\n                          discountPercentage\n                        }\n                      }\n                    }\n                    upcomingPromotionalOffers {\n                      promotionalOffers {\n                        startDate\n                        endDate\n                        discountSetting {\n                          discountType\n                          discountPercentage\n                        }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        "
+PROMOTIONS_QUERY = '\n          query promotionsQuery($namespace: String!, $country: String!, $locale: String!) {\n            Catalog {\n              catalogOffers(namespace: $namespace, locale: $locale, params: {category: "freegames", country: $country, sortBy: "effectiveDate", sortDir: "asc"}) {\n                elements {\n                  title\n                  description\n                  id\n                  namespace\n                  categories {\n                    path\n                  }\n                  linkedOfferNs\n                  linkedOfferId\n                  keyImages {\n                    type\n                    url\n                  }\n                  productSlug\n                  promotions {\n                    promotionalOffers {\n                      promotionalOffers {\n                        startDate\n                        endDate\n                        discountSetting {\n                          discountType\n                          discountPercentage\n                        }\n                      }\n                    }\n                    upcomingPromotionalOffers {\n                      promotionalOffers {\n                        startDate\n                        endDate\n                        discountSetting {\n                          discountType\n                          discountPercentage\n                        }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        '
 CATALOG_TAGS_QUERY = "\n            query catalogTags($namespace: String!)\n            {\n                Catalog {\n                    tags (\n                        namespace: $namespace,\n                        start: 0,\n                        count: 999\n                    ) {\n                        elements {\n                            aliases,\n                            id,\n                            name,\n                            referenceCount,\n                            status\n                        }\n                    }\n                }\n            }\n            "
 FEED_QUERY = "\n            query feedQuery($locale: String!, $countryCode: String, $offset: Int, $postsPerPage: Int, $category: String) {\n                TransientStream {\n                    myTransientFeed(countryCode: $countryCode, locale: $locale) {\n                        id\n                        activity {\n                            # TODO Comment in to enable welcome post when requirements are finalized\n                            # ...on SimpleActivity {\n                            #     type\n                            #     created_at\n                            # }\n                            ...on LinkAccountActivity {\n                                type\n                                created_at\n                                platforms\n                            }\n                            ...on SuggestedFriendsActivity {\n                                type\n                                created_at\n                                platform\n                                suggestions {\n                                    epicId\n                                    epicDisplayName\n                                    platformFullName\n                                    platformAvatar\n                                }\n                            }\n                            ...on IncomingInvitesActivity {\n                                type\n                                created_at\n                                invites {\n                                    epicId\n                                    epicDisplayName\n                                }\n                            }\n                            ...on RecentPlayersActivity {\n                                type\n                                created_at\n                                players {\n                                    epicId\n                                    epicDisplayName\n                                    playedGameName\n                                }\n                            }\n                        }\n                    }\n                }\n                Blog {\n                    dieselBlogPosts: getPosts(locale: $locale, offset: $offset, postsPerPage: $postsPerPage, category: $category) {\n                        blogList {\n                            _id\n                            author\n                            category\n                            content\n                            urlPattern\n                            slug\n                            sticky\n                            title\n                            date\n                            image\n                            shareImage\n                            trendingImage\n                            url\n                            featured\n                            link\n                            externalLink\n                        }\n                    }\n                }\n            }"
 PREREQUISITES_QUERY = "\n    query fetchPrerequisites($offerParams: [OfferParams]) {\n        Launcher{\n            prerequisites(offerParams:$offerParams) {\n                namespace,\n                offerId,\n                missingPrerequisiteItems\n                satisfiesPrerequisites\n            }\n        }\n    }\n"
 OFFERS_QUERY = "\n    query catalogQuery($productNamespace: String!, $offerId: String!, $locale: String, $country: String!, $includeSubItems: Boolean!) {\n  Catalog {\n    catalogOffer(namespace: $productNamespace, id: $offerId, locale: $locale) {\n      title\n      id\n      namespace\n      description\n      effectiveDate\n      expiryDate\n      isCodeRedemptionOnly\n      keyImages {\n        type\n        url\n      }\n      seller {\n        id\n        name\n      }\n      productSlug\n      urlSlug\n      url\n      tags {\n        id\n      }\n      items {\n        id\n        namespace\n      }\n      customAttributes {\n        key\n        value\n      }\n      categories {\n        path\n      }\n      price(country: $country) {\n        totalPrice {\n          discountPrice\n          originalPrice\n          voucherDiscount\n          discount\n          currencyCode\n          currencyInfo {\n            decimals\n          }\n          fmtPrice(locale: $locale) {\n            originalPrice\n            discountPrice\n            intermediatePrice\n          }\n        }\n        lineOffers {\n          appliedRules {\n            id\n            endDate\n            discountSetting {\n              discountType\n            }\n          }\n        }\n      }\n    }\n    offerSubItems(namespace: $productNamespace, id: $offerId) @include(if: $includeSubItems) {\n      namespace\n      id\n      releaseInfo {\n        appId\n        platform\n      }\n    }\n  }\n}\n"
 MEDIA_QUERY = "\n    query fetchMediaRef($mediaRefId: String!) {\n      Media {\n        getMediaRef(mediaRefId: $mediaRefId) {\n          accountId\n          outputs {\n            duration\n            url\n            width\n            height\n            key\n            contentType\n          }\n          namespace\n        }\n      }\n    }\n"
 PRODUCT_REVIEWS_QUERY = "\n            query productReviewsQuery($sku: String!) {\n                OpenCritic {\n                    productReviews(sku: $sku) {\n                        id\n                        name\n                        openCriticScore\n                        reviewCount\n                        percentRecommended\n                        openCriticUrl\n                        award\n                        topReviews {\n                            publishedDate\n                            externalUrl\n                            snippet\n                            language\n                            score\n                            author\n                            ScoreFormat {\n                                id\n                                description\n                            }\n                            OutletId\n                            outletName\n                            displayScore\n                        }\n                    }\n                }\n            }\n        "
 ADDONS_QUERY = "query getAddonsByNamespace($categories: String!, $count: Int!, $country: String!, $locale: String!, $namespace: String!, $sortBy: String!, $sortDir: String!) {\n  Catalog {\n    catalogOffers(namespace: $namespace, locale: $locale, params: {category: $categories, count: $count, country: $country, sortBy: $sortBy, sortDir: $sortDir}) {\n      elements {\n        countriesBlacklist\n        customAttributes {\n          key\n          value\n        }\n        description\n        developer\n        effectiveDate\n        id\n        isFeatured\n        keyImages {\n          type\n          url\n        }\n        lastModifiedDate\n        longDescription\n        namespace\n        offerType\n        productSlug\n        releaseDate\n        status\n        technicalDetails\n        title\n        urlSlug\n      }\n    }\n  }\n}\n"
-COLLECTION_QUERY = "query collectionLayoutQuery($locale: String, $country: String!, $slug: String) {\n  Storefront {\n    collectionLayout(locale: $locale, slug: $slug) {\n      _activeDate\n      _locale\n      _metaTags\n      _slug\n      _title\n      _urlPattern\n      lastModified\n      regionBlock\n      affiliateId\n      takeover {\n        banner {\n          altText\n          src\n        }\n        description\n        eyebrow\n        title\n      }\n      seo {\n        title\n        description\n        keywords\n        image {\n          src\n          altText\n        }\n        twitter {\n          title\n          description\n        }\n        og {\n          title\n          description\n          image {\n            src\n            alt\n          }\n        }\n      }\n      collectionOffers {\n        title\n        id\n        namespace\n        description\n        effectiveDate\n        countriesBlacklist\n        countriesWhitelist\n        developerDisplayName\n        publisherDisplayName\n        keyImages {\n          type\n          url\n        }\n        seller {\n          id\n          name\n        }\n        releaseDate\n        pcReleaseDate\n        approximateReleasePlan {\n          day\n          month\n          quarter\n          year\n          releaseDateType\n        }\n        prePurchase\n        productSlug\n        urlSlug\n        url\n        items {\n          id\n          namespace\n        }\n        customAttributes {\n          key\n          value\n        }\n        categories {\n          path\n        }\n        linkedOfferId\n        linkedOffer {\n          effectiveDate\n          customAttributes {\n            key\n            value\n          }\n        }\n        catalogNs {\n          mappings(pageType: \"productHome\") {\n            pageSlug\n            pageType\n          }\n        }\n        offerMappings {\n          pageSlug\n          pageType\n        }\n        price(country: $country) {\n          totalPrice {\n            currencyCode\n            currencyInfo {\n              decimals\n              symbol\n            }\n            discountPrice\n            originalPrice\n            voucherDiscount\n            discount\n            fmtPrice(locale: $locale) {\n              originalPrice\n              discountPrice\n              intermediatePrice\n            }\n          }\n          lineOffers {\n            appliedRules {\n              id\n              endDate\n            }\n          }\n        }\n      }\n      pageTheme {\n        preferredMode\n        light {\n          theme\n          accent\n        }\n        dark {\n          theme\n          accent\n        }\n      }\n      redirect {\n        code\n        url\n      }\n    }\n  }\n}\n"
+COLLECTION_QUERY = 'query collectionLayoutQuery($locale: String, $country: String!, $slug: String) {\n  Storefront {\n    collectionLayout(locale: $locale, slug: $slug) {\n      _activeDate\n      _locale\n      _metaTags\n      _slug\n      _title\n      _urlPattern\n      lastModified\n      regionBlock\n      affiliateId\n      takeover {\n        banner {\n          altText\n          src\n        }\n        description\n        eyebrow\n        title\n      }\n      seo {\n        title\n        description\n        keywords\n        image {\n          src\n          altText\n        }\n        twitter {\n          title\n          description\n        }\n        og {\n          title\n          description\n          image {\n            src\n            alt\n          }\n        }\n      }\n      collectionOffers {\n        title\n        id\n        namespace\n        description\n        effectiveDate\n        countriesBlacklist\n        countriesWhitelist\n        developerDisplayName\n        publisherDisplayName\n        keyImages {\n          type\n          url\n        }\n        seller {\n          id\n          name\n        }\n        releaseDate\n        pcReleaseDate\n        approximateReleasePlan {\n          day\n          month\n          quarter\n          year\n          releaseDateType\n        }\n        prePurchase\n        productSlug\n        urlSlug\n        url\n        items {\n          id\n          namespace\n        }\n        customAttributes {\n          key\n          value\n        }\n        categories {\n          path\n        }\n        linkedOfferId\n        linkedOffer {\n          effectiveDate\n          customAttributes {\n            key\n            value\n          }\n        }\n        catalogNs {\n          mappings(pageType: "productHome") {\n            pageSlug\n            pageType\n          }\n        }\n        offerMappings {\n          pageSlug\n          pageType\n        }\n        price(country: $country) {\n          totalPrice {\n            currencyCode\n            currencyInfo {\n              decimals\n              symbol\n            }\n            discountPrice\n            originalPrice\n            voucherDiscount\n            discount\n            fmtPrice(locale: $locale) {\n              originalPrice\n              discountPrice\n              intermediatePrice\n            }\n          }\n          lineOffers {\n            appliedRules {\n              id\n              endDate\n            }\n          }\n        }\n      }\n      pageTheme {\n        preferredMode\n        light {\n          theme\n          accent\n        }\n        dark {\n          theme\n          accent\n        }\n      }\n      redirect {\n        code\n        url\n      }\n    }\n  }\n}\n'
 # XXX: This code violates PEP 8, line > 79 chars
```

### Comparing `epicstore_api-0.1.7/epicstore_api.egg-info/PKG-INFO` & `epicstore_api-0.1.8/epicstore_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: epicstore-api
-Version: 0.1.7
+Version: 0.1.8
 Summary: An API wrapper for Epic Games Store written in Python
 Home-page: https://github.com/SD4RK/epicstore_api
-Download-URL: https://github.com/SD4RK/epicstore_api/archive/v_0.1.7.tar.gz
+Download-URL: https://github.com/SD4RK/epicstore_api/archive/v_0.1.8.tar.gz
 Author: SD4RK
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `epicstore_api-0.1.7/setup.py` & `epicstore_api-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from pathlib import Path
+
 import setuptools
 
 AUTHOR = 'SD4RK'
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+long_description = Path("README.md").read_text()
 
 setuptools.setup(
     name='epicstore_api',
     version=VERSION,
     author=AUTHOR,
     description='An API wrapper for Epic Games Store written in Python',
     long_description=long_description,
@@ -29,9 +30,9 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Internet',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Utilities',
     ],
-    python_requires='>=3.7'
+    python_requires='>=3.7',
 )
```

