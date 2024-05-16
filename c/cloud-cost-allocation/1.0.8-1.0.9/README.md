# Comparing `tmp/cloud-cost-allocation-1.0.8.tar.gz` & `tmp/cloud-cost-allocation-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-cost-allocation-1.0.8.tar", last modified: Thu Nov  2 17:01:22 2023, max compression
+gzip compressed data, was "cloud-cost-allocation-1.0.9.tar", last modified: Fri Jan 26 07:43:38 2024, max compression
```

## Comparing `cloud-cost-allocation-1.0.8.tar` & `cloud-cost-allocation-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21472 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20259 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:22.722788 cloud-cost-allocation-1.0.8/cloud_cost_allocation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23985 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/cloud_cost_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44704 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/cost_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/base_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/cloud_cost_allocation/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/cloud_cost_allocation/writer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/writer/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/cloud_cost_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21472 2023-11-02 17:01:22.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-11-02 17:01:22.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 17:01:22.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-02 17:01:22.000000 cloud-cost-allocation-1.0.8/cloud_cost_allocation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/puml/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/puml/cost-allocation-model.puml
--rw-r--r--   0 runner    (1001) docker     (127)    23813 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/puml/cost-allocation-model.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/puml/hierarchical-service-consumption-example.puml
--rw-r--r--   0 runner    (1001) docker     (127)    16917 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/puml/hierarchical-service-consumption-example.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/puml/hierarchical-service-cost-allocation-example.puml
--rw-r--r--   0 runner    (1001) docker     (127)    15996 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/puml/hierarchical-service-cost-allocation-example.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 17:01:22.726788 cloud-cost-allocation-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2023-11-02 17:01:14.000000 cloud-cost-allocation-1.0.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21916 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:38.010173 cloud-cost-allocation-1.0.9/cloud_cost_allocation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28849 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/cloud_cost_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46364 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/cost_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/base_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/cloud_cost_allocation/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/cloud_cost_allocation/writer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/writer/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/cloud_cost_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21916 2024-01-26 07:43:37.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-01-26 07:43:38.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 07:43:37.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-26 07:43:37.000000 cloud-cost-allocation-1.0.9/cloud_cost_allocation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/puml/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/puml/cost-allocation-model.puml
+-rw-r--r--   0 runner    (1001) docker     (127)    23813 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/puml/cost-allocation-model.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/puml/hierarchical-service-consumption-example.puml
+-rw-r--r--   0 runner    (1001) docker     (127)    16917 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/puml/hierarchical-service-consumption-example.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/puml/hierarchical-service-cost-allocation-example.puml
+-rw-r--r--   0 runner    (1001) docker     (127)    15996 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/puml/hierarchical-service-cost-allocation-example.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:43:38.014174 cloud-cost-allocation-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-01-26 07:43:30.000000 cloud-cost-allocation-1.0.9/tests/test.py
```

### Comparing `cloud-cost-allocation-1.0.8/LICENSE` & `cloud-cost-allocation-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/PKG-INFO` & `cloud-cost-allocation-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
@@ -128,15 +128,15 @@
         * This cost allocation cycle *C* -> *M* -> *C* can be broken by specifying a precedence list *C,M*. In this case, *C* is allocated no cost from *M*
     * As another example, see `test5` 
     * The cost allocation could manage cycles in a more sophisticated way in the future
 10. As a general rule, the names of all model objects (products, services, instances, tags, ...) are normalized to lower case, in order avoid low-high case mistakes
 
 ## Bittersweet ways for a service to allocate its cost
 
-The standard way for a service to allocate cost to its consumers is to provide dynamic cost allocation data containing cost allocation keys
+The standard way for a service to its allocate cost is to provide dynamic cost allocation data containing cost allocation keys.
 Three alternatives exist to this, and they should be used carefully:
 1. Use specific configurable *consumer service and product tags*
     * While providing an easy way to dynamically allocate costs, it does not offer any means to track usage and thus provides no hint to consumers on what drives their costs (black box)
     * See section *Consumer service and product tags* for details
 2. Use specific *cost allocation type* in cost allocation data
     * E.g. to allocate a cost share proportional to the amortized costs of the consumers
     * See section *Cost allocation types in cost allocation data* below for details
@@ -155,25 +155,31 @@
 - *ProviderTagSelector*: an expression matching the consumer tags.
 - *ProviderCostAllocationKey*: value 1.0.
 Examples are available in the tests `test3` and `test4`.
 
 ### Cost allocation types in cost allocation data
 
 The default value of *ProviderCostAllocationType* in cost allocation data is *'Key'*.
-Two other types of cost allocation are supported:
+Three other types of cost allocation are supported:
 1. *'CloudTagSelector'*
     * The consumer service instances are not explicitly specified in the cost allocation data
         * They are inferred as the ones consuming the cloud cost items whose tags match the *ProviderCostAllocationCloudTagSelector* expression
     * The cost allocation keys are set as the amortized costs of the matching cloud cost items
     * This type of cost allocation is convenient to allocate costs to consumer services that run directly on the cloud proportionally to their cloud costs
+    * See example in the test `test3`
 2. *'Cost'*
     * The cost is allocated to the consumer services proportionally to their amortized costs
     * Technically, amortized costs are globally allocated to service instances in a first time, while ignoring this type of cost allocation
     * The amortized costs resulting from this cost allocation are used in a second pass as cost allocation keys to perform the actual cost allocation
     * Although this type of cost allocation is convenient to avoid bothering about cost allocation keys, it can produce results that are hardly predictable and understandable, depending on the complexity of the global cost allocation graph
+    * See example in the test `test3`
+3. *'DefaultProduct'*
+    * By default, the cost of the provider service is allocated to the specified product(s)
+    * This type of cost allocation is convenient to implement centrally a default cost allocation to products, which is overriden by service owners when the latter provide cost allocation data
+    * See example in the test `test8`
 
 Examples of *'CloudTagSelector'* and *'Cost'* cost allocation types are available in the test `test3`.
 
 In theory, an even more general type of cost allocation could be considered:
 - *'ConsumerTagSelector'*
     * Cost would be allocated to service instances whose cost items match the *ProviderCostAllocationConsumerTagSelector* expression proportionally to their amortized costs
     * While being more generic, this type of cost allocation can be even less predictable
@@ -198,14 +204,17 @@
 # The format uses Python datetime syntax
 # Do not forget to escape the % character
 DateFormat = %%Y-%%m-%%d.
 
 # The name of the default service to use for cost allocation when the service tag is missing
 DefaultService = x
 
+# The name of the default product to allocate costs (optional)
+DefaultProduct = x
+
 # The dimensions
 Dimensions = Component,Environment
 
 # The number of provider meter columns in input cost allocation data and output allocated cost data
 NumberOfProviderMeters = 2
 
 # The number of product dimensions in input cost allocation data and output allocated cost data
@@ -305,11 +314,10 @@
 Please keep in mind that the cost allocation model is intended to be as minimal as possible.
 
 ### Code contributions
 When contributing code, please follow [this project-agnostic contribution guide](<http://contribution-guide.org/>).
 
 ## TODO
 
-- Cost readers for GCP and AWS.
+- Cost reader for FOCUS
 - Split and dispatch of the provider meter values when CloudTagSelector is used.
 - Support product dimension in cloud tags
-- Unit test for further amount allocation
```

### Comparing `cloud-cost-allocation-1.0.8/README.md` & `cloud-cost-allocation-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         * This cost allocation cycle *C* -> *M* -> *C* can be broken by specifying a precedence list *C,M*. In this case, *C* is allocated no cost from *M*
     * As another example, see `test5` 
     * The cost allocation could manage cycles in a more sophisticated way in the future
 10. As a general rule, the names of all model objects (products, services, instances, tags, ...) are normalized to lower case, in order avoid low-high case mistakes
 
 ## Bittersweet ways for a service to allocate its cost
 
-The standard way for a service to allocate cost to its consumers is to provide dynamic cost allocation data containing cost allocation keys
+The standard way for a service to its allocate cost is to provide dynamic cost allocation data containing cost allocation keys.
 Three alternatives exist to this, and they should be used carefully:
 1. Use specific configurable *consumer service and product tags*
     * While providing an easy way to dynamically allocate costs, it does not offer any means to track usage and thus provides no hint to consumers on what drives their costs (black box)
     * See section *Consumer service and product tags* for details
 2. Use specific *cost allocation type* in cost allocation data
     * E.g. to allocate a cost share proportional to the amortized costs of the consumers
     * See section *Cost allocation types in cost allocation data* below for details
@@ -127,25 +127,31 @@
 - *ProviderTagSelector*: an expression matching the consumer tags.
 - *ProviderCostAllocationKey*: value 1.0.
 Examples are available in the tests `test3` and `test4`.
 
 ### Cost allocation types in cost allocation data
 
 The default value of *ProviderCostAllocationType* in cost allocation data is *'Key'*.
-Two other types of cost allocation are supported:
+Three other types of cost allocation are supported:
 1. *'CloudTagSelector'*
     * The consumer service instances are not explicitly specified in the cost allocation data
         * They are inferred as the ones consuming the cloud cost items whose tags match the *ProviderCostAllocationCloudTagSelector* expression
     * The cost allocation keys are set as the amortized costs of the matching cloud cost items
     * This type of cost allocation is convenient to allocate costs to consumer services that run directly on the cloud proportionally to their cloud costs
+    * See example in the test `test3`
 2. *'Cost'*
     * The cost is allocated to the consumer services proportionally to their amortized costs
     * Technically, amortized costs are globally allocated to service instances in a first time, while ignoring this type of cost allocation
     * The amortized costs resulting from this cost allocation are used in a second pass as cost allocation keys to perform the actual cost allocation
     * Although this type of cost allocation is convenient to avoid bothering about cost allocation keys, it can produce results that are hardly predictable and understandable, depending on the complexity of the global cost allocation graph
+    * See example in the test `test3`
+3. *'DefaultProduct'*
+    * By default, the cost of the provider service is allocated to the specified product(s)
+    * This type of cost allocation is convenient to implement centrally a default cost allocation to products, which is overriden by service owners when the latter provide cost allocation data
+    * See example in the test `test8`
 
 Examples of *'CloudTagSelector'* and *'Cost'* cost allocation types are available in the test `test3`.
 
 In theory, an even more general type of cost allocation could be considered:
 - *'ConsumerTagSelector'*
     * Cost would be allocated to service instances whose cost items match the *ProviderCostAllocationConsumerTagSelector* expression proportionally to their amortized costs
     * While being more generic, this type of cost allocation can be even less predictable
@@ -170,14 +176,17 @@
 # The format uses Python datetime syntax
 # Do not forget to escape the % character
 DateFormat = %%Y-%%m-%%d.
 
 # The name of the default service to use for cost allocation when the service tag is missing
 DefaultService = x
 
+# The name of the default product to allocate costs (optional)
+DefaultProduct = x
+
 # The dimensions
 Dimensions = Component,Environment
 
 # The number of provider meter columns in input cost allocation data and output allocated cost data
 NumberOfProviderMeters = 2
 
 # The number of product dimensions in input cost allocation data and output allocated cost data
@@ -277,11 +286,10 @@
 Please keep in mind that the cost allocation model is intended to be as minimal as possible.
 
 ### Code contributions
 When contributing code, please follow [this project-agnostic contribution guide](<http://contribution-guide.org/>).
 
 ## TODO
 
-- Cost readers for GCP and AWS.
+- Cost reader for FOCUS
 - Split and dispatch of the provider meter values when CloudTagSelector is used.
-- Support product dimension in cloud tags
-- Unit test for further amount allocation
+- Support product dimension in cloud tags
```

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/cloud_cost_allocator.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/cloud_cost_allocator.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,30 +39,47 @@
             error("CloudCostAllocator.currency must be set, for date " + self.date_str)
             return False
 
         # Initiate cost items with cloud cost items
         cost_items = []
         cost_items.extend(cloud_cost_items)
 
-        # Process cloud tag selectors
-        info("Processing cloud tag selectors, for date" + self.date_str)
+        # Identify cloud tag selectors and  default product consumer cost items
         cloud_tag_selector_consumer_cost_items = []
+        default_product_consumer_cost_items = {}
+        default_product_allocation_keys = {}
         for consumer_cost_item in consumer_cost_items:
             if consumer_cost_item.provider_cost_allocation_type == "CloudTagSelector":
                 cloud_tag_selector_consumer_cost_items.append(consumer_cost_item)
+            elif consumer_cost_item.provider_cost_allocation_type == "DefaultProduct":
+                provider_service = consumer_cost_item.provider_service
+                if provider_service in default_product_consumer_cost_items:
+                    default_product_consumer_cost_items[provider_service].append(consumer_cost_item)
+                    default_product_allocation_keys[provider_service] += consumer_cost_item.allocation_keys[0]
+                else:
+                    default_product_consumer_cost_items[provider_service] = [consumer_cost_item]
+                    default_product_allocation_keys[provider_service] = consumer_cost_item.allocation_keys[0]
             else:
                 cost_items.append(consumer_cost_item)
+
+        # Process cloud tag selectors
+        info("Processing cloud tag selectors, for date" + self.date_str)
         self.process_cloud_tag_selectors(cost_items, cloud_tag_selector_consumer_cost_items, cloud_cost_items)
 
         # Create and add cloud consumer cost item from tags
         info("Creating consumer cost items from tags, for date " + self.date_str)
         new_consumer_cost_items = []
         self.create_consumer_cost_items_from_tags(new_consumer_cost_items, cost_items)
         cost_items.extend(new_consumer_cost_items)
 
+        # Process default products
+        cost_items = self.process_default_products(cost_items,
+                                                   default_product_consumer_cost_items,
+                                                   default_product_allocation_keys)
+
         # Check dates
         cleansed_cost_items = []
         different_date_str_dict = {}
         for cost_item in cost_items:
             if cost_item.date_str == self.date_str:
                 cleansed_cost_items.append(cost_item)
             else:
@@ -99,19 +116,16 @@
 
         # Break cycles
         # When a cycle is broken, ConsumerCostItem.is_removed_from_cycle is set to True at the cycle break point
         info("Breaking cycles, for date " + self.date_str)
         if not self.break_cycles(cost_items):
             return False
 
-        # Initialize instances and set cost item links
-        self.service_instances = {}
-        for cost_item in cost_items:
-            if not cost_item.is_consumer_cost_item_removed_for_cycle():
-                cost_item.set_instance_links(self)
+        # Reset instances
+        self.reset_instances(cost_items)
 
         # Protect against unexpected cycles
         try:
 
             # Compute service amortized cost, ignoring the keys that are using cost, and then
             # set these keys from the allocated cost
             amounts = ['AmortizedCost', 'OnDemandCost']
@@ -142,18 +156,16 @@
 
         # Build amount allocation key indexes dictionary
         amount_to_allocation_key_indexes = {}
         if not self.cost_item_factory.config.build_amount_to_allocation_key_indexes(amount_to_allocation_key_indexes,
                                                                                     amounts):
             return False
 
-        # Initialize instances and set cost item links
-        self.service_instances = {}
-        for cost_item in cost_items:
-            cost_item.set_instance_links(self)
+        # Reset instances
+        self.reset_instances(cost_items)
 
         # Visit, by protecting against unexpected cycles
         try:
             self.visit_for_allocation(False, True, amount_to_allocation_key_indexes)
         except CycleException:
             return False
 
@@ -176,19 +188,16 @@
         # Break cycles
         nb_breaks = 0
         while nb_breaks < max_breaks:
 
             # Log
             info("Detecting and breaking cycles, for date " + self.date_str + ": pass " + str(nb_breaks))
 
-            # Initialize instances and set cost item links
-            self.service_instances = {}
-            for cost_item in cost_items:
-                if not cost_item.is_consumer_cost_item_removed_for_cycle():
-                    cost_item.set_instance_links(self)
+            # Reset instances
+            self.reset_instances(cost_items)
 
             # Reset visit
             for service_instance in self.service_instances.values():
                 service_instance.reset_visit()
 
             # Visit cycles
             try:
@@ -446,14 +455,85 @@
                   ", for date " + self.date_str)
 
         # Clean-up for the sake of memory
         evaluation_error_dict.clear()
         cloud_tag_dict.clear()
         new_consumer_cost_items.clear()
 
+    def reset_instances(self, cost_items: list[CostItem]):
+        self.service_instances = {}
+        for cost_item in cost_items:
+            if not cost_item.is_consumer_cost_item_removed_for_cycle():
+                cost_item.set_instance_links(self)
+
+    def process_default_products(self,
+                                 cost_items: list[CostItem],
+                                 default_product_consumer_cost_items: dict[str, list[ConsumerCostItem]],
+                                 default_product_allocation_keys: dict[str, float]):
+
+        # Reset instances
+        self.reset_instances(cost_items)
+
+        # Add default products for consumer cost items with no product
+        new_cost_items = []
+        for cost_item in cost_items:
+            provider_service = cost_item.get_provider_service()
+            if (provider_service and
+                    not cost_item.get_product() and
+                    cost_item.provider_service in default_product_consumer_cost_items):
+                for default_product_consumer_cost_item\
+                        in default_product_consumer_cost_items[cost_item.provider_service]:
+                    new_consumer_cost_item = self.cost_item_factory.create_consumer_cost_item()
+                    new_consumer_cost_item.copy(cost_item)
+                    new_consumer_cost_item.product = default_product_consumer_cost_item.product
+                    new_consumer_cost_item.product_dimensions =\
+                        default_product_consumer_cost_item.product_dimensions.copy()
+                    new_consumer_cost_item.allocation_keys[0] *=\
+                        default_product_consumer_cost_item.allocation_keys[0] /\
+                        default_product_allocation_keys[cost_item.provider_service]
+                    new_cost_items.append(new_consumer_cost_item)
+            else:
+                new_cost_items.append(cost_item)
+
+        # Set global default product for self consumption
+        default_product = self.cost_item_factory.config.default_product
+        if default_product:
+            for cost_item in new_cost_items:
+                if cost_item.is_self_consumption():
+                    if not cost_item.get_product():
+                        cost_item.set_product(default_product)
+
+        # Add consumer cost items with default products for final service instances with no product
+        for service_instance in self.service_instances.values():
+            if not service_instance.is_provider():
+                new_consumer_cost_item = self.cost_item_factory.create_consumer_cost_item()
+                new_consumer_cost_item.date_str = self.date_str
+                new_consumer_cost_item.provider_service = service_instance.service
+                new_consumer_cost_item.provider_instance = service_instance.instance
+                new_consumer_cost_item.service = service_instance.service
+                new_consumer_cost_item.instance = service_instance.instance
+                new_consumer_cost_item.provider_cost_allocation_type = "DefaultProduct"
+                new_consumer_cost_item.allocation_keys[0] = 1.0
+                if service_instance.service in default_product_consumer_cost_items:
+                    for default_product_consumer_cost_item\
+                            in default_product_consumer_cost_items[service_instance.service]:
+                        new_consumer_cost_item_with_product = self.cost_item_factory.create_consumer_cost_item()
+                        new_consumer_cost_item_with_product.copy(new_consumer_cost_item)
+                        new_consumer_cost_item_with_product.product = default_product_consumer_cost_item.product
+                        new_consumer_cost_item_with_product.allocation_keys[0] *=\
+                            default_product_consumer_cost_item.allocation_keys[0] /\
+                            default_product_allocation_keys[service_instance.service]
+                        new_cost_items.append(new_consumer_cost_item_with_product)
+                elif default_product:
+                    new_consumer_cost_item.product = default_product
+                    new_cost_items.append(new_consumer_cost_item)
+
+        # Return
+        return new_cost_items
+
     def visit_for_allocation(self,
                              ignore_cost_as_key: bool,
                              increment_amounts: bool,
                              amount_allocation_to_key_indexes: dict[int]) -> None:
         for service_instance in self.service_instances.values():
             service_instance.reset_visit()
         for service_instance in self.service_instances.values():
```

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/config.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Guess what it is
     """
 
     __slots__ = (
         'config',                                # type: ConfigParser
         'date_format',                           # type: str
         'default_service',                       # type: str
+        'default_product',                       # type: str
         'service_tag_keys',                      # type: list[str]
         'instance_tag_keys',                     # type: list[str]
         'consumer_service_tag_keys',             # type: list[str]
         'consumer_service_ignored_tag_values',   # type: list[str]
         'consumer_instance_tag_keys',            # type: list[str]
         'product_tag_keys',                      # type: list[str]
         'dimensions',                            # type: list[str]
@@ -53,14 +54,20 @@
             error("Missing date format, assuming %Y-%m-%d")
             self.date_format = "%Y-%m-%d"
 
         # Default service
         if 'General' in config and 'DefaultService' in config['General']:
             self.default_service = config['General']['DefaultService'].strip().lower()
 
+        # Default product
+        if 'General' in config and 'DefaultProduct' in config['General']:
+            self.default_product = config['General']['DefaultProduct'].strip().lower()
+        else:
+            self.default_product = ''
+
         # Service tag keys
         self.service_tag_keys = []
         if 'TagKey' in config and 'Service' in config['TagKey']:
             for service_tag_key in self.config['TagKey']['Service'].split(","):
                 self.service_tag_keys.append(service_tag_key.strip().lower())
 
         # Instance tag keys
```

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/cost_items.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/cost_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,22 @@
         self.instance = ""
         self.dimensions = {}
         self.tags = {}
         self.amounts = None
         self.currency = ""
         self.nb_matching_provider_tag_selectors = 0
 
+    def copy(self, cost_item: 'CostItem'):
+        self.date_str = cost_item.date_str
+        self.service = cost_item.service
+        self.instance = cost_item.instance
+        self.dimensions = cost_item.dimensions.copy()
+        self.tags = cost_item.tags.copy()
+        self.currency = cost_item.currency
+
     def get_consumer_cost_item_provider_service_instance(self) -> 'ServiceInstance':
         # Default behavior, overridden in child classes
         return None
 
     def get_product(self) -> str:
         # Default behavior, overridden in child classes
         return ''
@@ -58,14 +66,18 @@
         # Default behavior, overridden in child classes
         return []
 
     def get_product_meters(self) -> list[dict[str, str]]:
         # Default behavior, overridden in child classes
         return []
 
+    def get_provider_service(self) -> str:
+        # Default behavior, overridden in child classes
+        return ''
+
     def get_unallocated_product_amount(self, index: int) -> float:
         # Default behavior, overridden in child classes
         return 0.0
 
     def initialize(self, config: Config) -> None:
         self.amounts = [0.0] * config.nb_amounts
 
@@ -81,14 +93,18 @@
         # Default behavior, overridden in child classes
         return
 
     def set_instance_links(self, cloud_cost_allocator: 'CloudCostAllocator') -> None:
         # Default behavior, overridden in child classes
         cloud_cost_allocator.get_service_instance(self.service, self.instance).cost_items.append(self)
 
+    def set_product(self, product: str) -> None:
+        # Default behavior, overridden in child classes
+        return
+
     # Must be implemented in child classes
     @abstractmethod
     def visit_for_allocation(self,
                              visited_service_instance_list: list['ServiceInstance'],
                              ignore_cost_as_key: bool,
                              process_self_consumption: bool,
                              increment_amounts: bool,
@@ -174,14 +190,28 @@
         self.product_dimensions = None
         self.product_meters = None
         self.product_amounts = None
         self.unallocated_product_amounts = None
         self.is_removed_from_cycle = False
         self.provider_service_instance = None
 
+    def copy(self, consumer_cost_item: 'ConsumerCostItem'):
+        super().copy(consumer_cost_item)
+        self.provider_service = consumer_cost_item.provider_service
+        self.provider_instance = consumer_cost_item.provider_instance
+        self.provider_tag_selector = consumer_cost_item.provider_tag_selector
+        self.provider_cost_allocation_type = consumer_cost_item.provider_cost_allocation_type
+        self.allocation_keys = consumer_cost_item.allocation_keys.copy()
+        self.provider_cost_allocation_cloud_tag_selector =\
+            consumer_cost_item.provider_cost_allocation_cloud_tag_selector
+        self.provider_meters = consumer_cost_item.provider_meters.copy()
+        self.product = consumer_cost_item.product
+        self.product_dimensions = consumer_cost_item.product_dimensions.copy()
+        self.product_meters = consumer_cost_item.product_meters.copy()
+
     def get_consumer_cost_item_provider_service_instance(self) -> 'ServiceInstance':
         return self.provider_service_instance
 
     def get_product(self) -> str:
         return self.product
 
     def get_product_amount(self, index: int) -> float:
@@ -189,14 +219,18 @@
 
     def get_product_dimensions(self) -> list[dict[str, str]]:
         return self.product_dimensions
 
     def get_product_meters(self) -> list[dict[str, str]]:
         return self.product_meters
 
+    def get_provider_service(self) -> str:
+        # Default behavior, overridden in child classes
+        return self.provider_service
+
     def get_unallocated_product_amount(self, index: int) -> float:
         return self.unallocated_product_amounts[index]
 
     def initialize(self, config: Config) -> None:
         super().initialize(config)
         self.allocation_keys = [0.0] * config.nb_allocation_keys
         self.provider_meters = [{}] * config.nb_provider_meters
@@ -217,14 +251,17 @@
 
     def set_instance_links(self, cloud_cost_allocator: 'CloudCostAllocator') -> None:
         super().set_instance_links(cloud_cost_allocator)
         self.provider_service_instance = cloud_cost_allocator.get_service_instance(self.provider_service,
                                                                                    self.provider_instance)
         self.provider_service_instance.consumer_cost_items.append(self)
 
+    def set_product(self, product: str) -> None:
+        self.product = product
+
     def visit_for_allocation(self,
                              visited_service_instance_list: list['ServiceInstance'],
                              ignore_cost_as_key: bool,
                              process_self_consumption: bool,
                              increment_amounts: bool,
                              amount_to_allocation_key_indexes: dict[int]) -> None:
```

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/main.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/main.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/base_reader.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/base_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/csv_allocated_cost_reader.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/csv_allocated_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,22 @@
         if "ProviderTagSelector" in line:
             consumer_cost_item.provider_tag_selector = line["ProviderTagSelector"].lower()
 
         # Provider cost allocation type and related fields
         consumer_cost_item.provider_cost_allocation_type = "Key"  # Default value
         if 'ProviderCostAllocationType' in line:
             consumer_cost_item.provider_cost_allocation_type = line['ProviderCostAllocationType']
-            if consumer_cost_item.provider_cost_allocation_type not in ("Key", "Cost", "CloudTagSelector"):
+            if consumer_cost_item.provider_cost_allocation_type not in ("Key",
+                                                                        "Cost",
+                                                                        "CloudTagSelector",
+                                                                        "DefaultProduct"):
                 error("Unknown ProviderCostAllocationType '" + consumer_cost_item.provider_cost_allocation_type +
                       "' for ProviderService '" + consumer_cost_item.provider_service + "'")
                 return None
-        if consumer_cost_item.provider_cost_allocation_type == 'Key':
+        if consumer_cost_item.provider_cost_allocation_type in ['Key', 'DefaultProduct']:
             if 'ProviderCostAllocationKey' in line:
                 key_str = line['ProviderCostAllocationKey']
                 if utils.is_float(key_str):
                     consumer_cost_item.allocation_keys[0] = float(key_str)
             if consumer_cost_item.allocation_keys[0] == 0.0:
                 error("Skipping cost allocation key line with non-float " +
                       " ProviderCostAllocationKey: '" + key_str + "'" +
```

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/utils/utils.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/writer/base_writer.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/writer/base_writer.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation/writer/csv_allocated_cost_writer.py` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation/writer/csv_allocated_cost_writer.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation.egg-info/PKG-INFO` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
@@ -128,15 +128,15 @@
         * This cost allocation cycle *C* -> *M* -> *C* can be broken by specifying a precedence list *C,M*. In this case, *C* is allocated no cost from *M*
     * As another example, see `test5` 
     * The cost allocation could manage cycles in a more sophisticated way in the future
 10. As a general rule, the names of all model objects (products, services, instances, tags, ...) are normalized to lower case, in order avoid low-high case mistakes
 
 ## Bittersweet ways for a service to allocate its cost
 
-The standard way for a service to allocate cost to its consumers is to provide dynamic cost allocation data containing cost allocation keys
+The standard way for a service to its allocate cost is to provide dynamic cost allocation data containing cost allocation keys.
 Three alternatives exist to this, and they should be used carefully:
 1. Use specific configurable *consumer service and product tags*
     * While providing an easy way to dynamically allocate costs, it does not offer any means to track usage and thus provides no hint to consumers on what drives their costs (black box)
     * See section *Consumer service and product tags* for details
 2. Use specific *cost allocation type* in cost allocation data
     * E.g. to allocate a cost share proportional to the amortized costs of the consumers
     * See section *Cost allocation types in cost allocation data* below for details
@@ -155,25 +155,31 @@
 - *ProviderTagSelector*: an expression matching the consumer tags.
 - *ProviderCostAllocationKey*: value 1.0.
 Examples are available in the tests `test3` and `test4`.
 
 ### Cost allocation types in cost allocation data
 
 The default value of *ProviderCostAllocationType* in cost allocation data is *'Key'*.
-Two other types of cost allocation are supported:
+Three other types of cost allocation are supported:
 1. *'CloudTagSelector'*
     * The consumer service instances are not explicitly specified in the cost allocation data
         * They are inferred as the ones consuming the cloud cost items whose tags match the *ProviderCostAllocationCloudTagSelector* expression
     * The cost allocation keys are set as the amortized costs of the matching cloud cost items
     * This type of cost allocation is convenient to allocate costs to consumer services that run directly on the cloud proportionally to their cloud costs
+    * See example in the test `test3`
 2. *'Cost'*
     * The cost is allocated to the consumer services proportionally to their amortized costs
     * Technically, amortized costs are globally allocated to service instances in a first time, while ignoring this type of cost allocation
     * The amortized costs resulting from this cost allocation are used in a second pass as cost allocation keys to perform the actual cost allocation
     * Although this type of cost allocation is convenient to avoid bothering about cost allocation keys, it can produce results that are hardly predictable and understandable, depending on the complexity of the global cost allocation graph
+    * See example in the test `test3`
+3. *'DefaultProduct'*
+    * By default, the cost of the provider service is allocated to the specified product(s)
+    * This type of cost allocation is convenient to implement centrally a default cost allocation to products, which is overriden by service owners when the latter provide cost allocation data
+    * See example in the test `test8`
 
 Examples of *'CloudTagSelector'* and *'Cost'* cost allocation types are available in the test `test3`.
 
 In theory, an even more general type of cost allocation could be considered:
 - *'ConsumerTagSelector'*
     * Cost would be allocated to service instances whose cost items match the *ProviderCostAllocationConsumerTagSelector* expression proportionally to their amortized costs
     * While being more generic, this type of cost allocation can be even less predictable
@@ -198,14 +204,17 @@
 # The format uses Python datetime syntax
 # Do not forget to escape the % character
 DateFormat = %%Y-%%m-%%d.
 
 # The name of the default service to use for cost allocation when the service tag is missing
 DefaultService = x
 
+# The name of the default product to allocate costs (optional)
+DefaultProduct = x
+
 # The dimensions
 Dimensions = Component,Environment
 
 # The number of provider meter columns in input cost allocation data and output allocated cost data
 NumberOfProviderMeters = 2
 
 # The number of product dimensions in input cost allocation data and output allocated cost data
@@ -305,11 +314,10 @@
 Please keep in mind that the cost allocation model is intended to be as minimal as possible.
 
 ### Code contributions
 When contributing code, please follow [this project-agnostic contribution guide](<http://contribution-guide.org/>).
 
 ## TODO
 
-- Cost readers for GCP and AWS.
+- Cost reader for FOCUS
 - Split and dispatch of the provider meter values when CloudTagSelector is used.
 - Support product dimension in cloud tags
-- Unit test for further amount allocation
```

### Comparing `cloud-cost-allocation-1.0.8/cloud_cost_allocation.egg-info/SOURCES.txt` & `cloud-cost-allocation-1.0.9/cloud_cost_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/puml/cost-allocation-model.puml` & `cloud-cost-allocation-1.0.9/puml/cost-allocation-model.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/puml/cost-allocation-model.svg` & `cloud-cost-allocation-1.0.9/puml/cost-allocation-model.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/puml/hierarchical-service-consumption-example.puml` & `cloud-cost-allocation-1.0.9/puml/hierarchical-service-consumption-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/puml/hierarchical-service-consumption-example.svg` & `cloud-cost-allocation-1.0.9/puml/hierarchical-service-consumption-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/puml/hierarchical-service-cost-allocation-example.puml` & `cloud-cost-allocation-1.0.9/puml/hierarchical-service-cost-allocation-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/puml/hierarchical-service-cost-allocation-example.svg` & `cloud-cost-allocation-1.0.9/puml/hierarchical-service-cost-allocation-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/setup.cfg` & `cloud-cost-allocation-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.8/setup.py` & `cloud-cost-allocation-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Import readme
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme_file:
     readme = readme_file.read()
 
 # Setup
 setup(
     name='cloud-cost-allocation',
-    version='1.0.8',
+    version='1.0.9',
     description='Python library for shared, hierarchical cost allocation based on user-defined usage metrics.',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=['cloud_cost_allocation',
               'cloud_cost_allocation.reader',
               'cloud_cost_allocation.utils',
               'cloud_cost_allocation.writer'],
```

### Comparing `cloud-cost-allocation-1.0.8/tests/test.py` & `cloud-cost-allocation-1.0.9/tests/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,17 @@
 
     def test_test6(self):
         self.run_allocation('test6')
 
     def test_test7(self):
         self.run_further_allocation('test7', self.load_further_amount_test7)
 
+    def test_test8(self):
+        self.run_allocation('test8')
+
     # Auxiliary methods
     def load_further_amount_test7(self, cost_items: list[CostItem]):
         for cost_item in cost_items:
 
             # Populate CO2 amount (index 2) and CO2 allocation key (index 1)
             if cost_item.service == 'container':  # CO2 set at IaaS level
                 cost_item.set_amount(2, 10)
```

