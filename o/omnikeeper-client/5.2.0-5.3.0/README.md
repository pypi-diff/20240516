# Comparing `tmp/omnikeeper_client-5.2.0-py3-none-any.whl.zip` & `tmp/omnikeeper_client-5.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 20869 bytes, number of entries: 16
+Zip file size: 21084 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     1265 b- defN 24-May-08 06:45 omnikeeper_client/__init__.py
 -rw-r--r--  2.0 unx     1984 b- defN 24-Mar-14 11:13 omnikeeper_client/apiclient.py
 -rw-r--r--  2.0 unx     5040 b- defN 24-Feb-06 12:05 omnikeeper_client/ci.py
 -rw-r--r--  2.0 unx     3796 b- defN 24-Apr-04 07:13 omnikeeper_client/dataframes.py
 -rw-r--r--  2.0 unx     3232 b- defN 24-Feb-06 12:05 omnikeeper_client/layer.py
 -rw-r--r--  2.0 unx     2765 b- defN 24-Apr-05 10:02 omnikeeper_client/pyd.py
 -rw-r--r--  2.0 unx    10639 b- defN 24-Apr-04 07:14 omnikeeper_client/simple_traits.py
 -rw-r--r--  2.0 unx     4574 b- defN 24-Apr-04 07:13 omnikeeper_client/trait.py
--rw-r--r--  2.0 unx    20532 b- defN 24-May-08 06:54 omnikeeper_client/traitentities.py
+-rw-r--r--  2.0 unx    21202 b- defN 24-May-16 10:22 omnikeeper_client/traitentities.py
 -rw-r--r--  2.0 unx     5262 b- defN 24-Feb-06 12:05 omnikeeper_client/typing.py
 -rw-r--r--  2.0 unx      917 b- defN 24-Feb-06 12:05 omnikeeper_client/util.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      572 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1373 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/RECORD
-16 files, 73418 bytes uncompressed, 18595 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      572 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1373 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/RECORD
+16 files, 74088 bytes uncompressed, 18810 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: omnikeeper_client/typing.py
 Comment: 
 
 Filename: omnikeeper_client/util.py
 Comment: 
 
-Filename: omnikeeper_client-5.2.0.dist-info/LICENSE
+Filename: omnikeeper_client-5.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: omnikeeper_client-5.2.0.dist-info/METADATA
+Filename: omnikeeper_client-5.3.0.dist-info/METADATA
 Comment: 
 
-Filename: omnikeeper_client-5.2.0.dist-info/WHEEL
+Filename: omnikeeper_client-5.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: omnikeeper_client-5.2.0.dist-info/top_level.txt
+Filename: omnikeeper_client-5.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: omnikeeper_client-5.2.0.dist-info/RECORD
+Filename: omnikeeper_client-5.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omnikeeper_client/traitentities.py

```diff
@@ -332,15 +332,15 @@
         readLayers=read_layers, 
         baseCIID=base_ciid,
         relatedCIIDs=related_ciids
         ))
 
     return True
 
-def bulk_replace_traitentity_relations(ok_api_client: okc.OkApiClient, trait_id: str, traitrelation_id: str, input: List[Dict[str, Any]], write_layer: str, read_layers: List[str] = None) -> bool:
+def bulk_replace_traitentity_relations(ok_api_client: okc.OkApiClient, trait_id: str, traitrelation_id: str, input: List[Dict[str, Any]], relevant_ciids: List[str], write_layer: str, read_layers: List[str] = None) -> bool:
     """
     Bulk replaces a particular trait relation of a particular trait for ALL trait entities of that trait
     Adds new traitrelations and deletes all relevant traitrelations not in the provided list
 
     Parameters
     ----------
     ok_api_client : OkApiClient
@@ -351,14 +351,21 @@
 
     traitrelation_id: str
         the id of the trait's traitrelation
         
     input: List[Dict[str, Any]]
         a list of dicts, the dicts in the following form: { "baseCIID" = <ciid>, "relatedCIIDs" = [<ciid>, <ciid>, ...] }
 
+    relevant_ciids: List[str]
+        a list of CIIDs, that specifies which CIs are actually relevant for this operation. This is necessary to let omnikeeper know which CIs it should consider for this operation
+        CIs not in the list of relevant_ciids are not changed
+        depending on your usecase..
+        ...you may want to set relevant_ciids equal to the list of baseCIIDs in input
+        ...or you may want to keep track of the relevant_ciids yourself, because you got an initial list from get_all_traitentity_relations()
+
     write_layer : str
         the id of the layer in which the data should be added
 
     read_layers : [str]
         A list with ids of the layers in which the omnikeeper will look if trait entities already exist
 
     Returns
@@ -366,32 +373,34 @@
     bool 
         True if the update is successful, False otherwise
     """
 
     prefixed_escaped_trait_id = _get_prefixed_trait_id(_get_escaped_trait_id(trait_id))
     escaped_traitrelation_id = _get_escaped_trait_id(traitrelation_id)
     query = gql(f"""
-        mutation($readLayers: [String]!, $writeLayer: String!, $input: [TE_Upsert_Relations_Only_Input]!) {{
+        mutation($readLayers: [String]!, $writeLayer: String!, $input: [TE_Upsert_Relations_Only_Input]!, $relevantCIIDs: [Guid]!) {{
         bulkReplaceRelations_{prefixed_escaped_trait_id}_{escaped_traitrelation_id}(
             layers: $readLayers
             writeLayer: $writeLayer
             input: $input
+            relevantCIIDs: $relevantCIIDs
         ) {{
             success
         }}
         }}
         """)
         
     if read_layers is None:
         read_layers = [write_layer]
 
     result = ok_api_client.execute_graphql(query, variables=dict(
         writeLayer=write_layer, 
         readLayers=read_layers, 
-        input=input
+        input=input,
+        relevantCIIDs=relevant_ciids
         ))
 
     return result[f"bulkReplaceRelations_{prefixed_escaped_trait_id}_{escaped_traitrelation_id}"]["success"]
   
 def _bulk_replace_trait_entities_by_filter(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], id_attributes: List[str], id_relations: List[str], write_layer: str, read_layers: List[str] = None, filter: object = {}) -> bool:
     """
     Internal method used to replace all traitentites in a layer, it can use a filter when updating the trait entities,
```

## Comparing `omnikeeper_client-5.2.0.dist-info/LICENSE` & `omnikeeper_client-5.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `omnikeeper_client-5.2.0.dist-info/METADATA` & `omnikeeper_client-5.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnikeeper-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: Python library containing helper functions for implementing omnikeeper clients
 Home-page: UNKNOWN
 Author: Maximilian Csuk
 License: Apache 2.0
 Platform: UNKNOWN
 License-File: LICENSE
 Requires-Dist: appengine-python-standard ~=1.1
```

## Comparing `omnikeeper_client-5.2.0.dist-info/RECORD` & `omnikeeper_client-5.3.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 omnikeeper_client/apiclient.py,sha256=X2NMaqM23pGLmDFDV2ueJnJzGdUEjz1WLrVvlWkYaGA,1984
 omnikeeper_client/ci.py,sha256=hXYsfDbMNvIy32CbStar1ade3ifH6VTL4VjxF9ICy1I,5040
 omnikeeper_client/dataframes.py,sha256=1G-k_IhPejA1UpR0_JYzLSgEBkVymD24gWNpWC5aHC0,3796
 omnikeeper_client/layer.py,sha256=To0INBUjgOiIuwwcMRo3wdT1mIbwcm-cVjJ4Lqh0SwI,3232
 omnikeeper_client/pyd.py,sha256=8AQVtMzxz2tkDP8z-0MCLA0meLOxmtEMBHQxI_f6Uwk,2765
 omnikeeper_client/simple_traits.py,sha256=yduQQKL93hUOBe6NQBBHchrtC8qr-kl8BU29b5cnbls,10639
 omnikeeper_client/trait.py,sha256=mPn46R2Aj5x1F6us_Z5VQ2iXf2pYQW9osSgItcQ8L5Q,4574
-omnikeeper_client/traitentities.py,sha256=icKLKe6zTMbOpsdiLdsFvkerICaw0RmbZ3q2DPH0kTw,20532
+omnikeeper_client/traitentities.py,sha256=avlwArYgTl_pe26lCmmC8cxU1GXWqEE7bvwD8n5xExM,21202
 omnikeeper_client/typing.py,sha256=dLzATV6Ez3VhPMEGdnsLKkZNS1aFgfURYbRKHiAGEFE,5262
 omnikeeper_client/util.py,sha256=Htf_rrlvd6usJ-ONWOU1l0Bz_CnisjQrlRzNODppiZg,917
-omnikeeper_client-5.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-omnikeeper_client-5.2.0.dist-info/METADATA,sha256=ruu5QjK4PWw4RlPhXNfkfAs8S03zaW8cha35-g5lwIE,572
-omnikeeper_client-5.2.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-omnikeeper_client-5.2.0.dist-info/top_level.txt,sha256=3VgpRS-e1mbaX1mKkPt9Mszwazf6tc1Tk3GORBV6ijk,18
-omnikeeper_client-5.2.0.dist-info/RECORD,,
+omnikeeper_client-5.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+omnikeeper_client-5.3.0.dist-info/METADATA,sha256=Alum_tThOsen-sJbejPRFZe1bbJthiym0oF2MfrYUrw,572
+omnikeeper_client-5.3.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+omnikeeper_client-5.3.0.dist-info/top_level.txt,sha256=3VgpRS-e1mbaX1mKkPt9Mszwazf6tc1Tk3GORBV6ijk,18
+omnikeeper_client-5.3.0.dist-info/RECORD,,
```

