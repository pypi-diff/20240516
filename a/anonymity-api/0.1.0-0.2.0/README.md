# Comparing `tmp/anonymity_api-0.1.0.tar.gz` & `tmp/anonymity_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonymity_api-0.1.0.tar", last modified: Sun May 12 20:24:54 2024, max compression
+gzip compressed data, was "anonymity_api-0.2.0.tar", last modified: Thu May 16 10:45:02 2024, max compression
```

## Comparing `anonymity_api-0.1.0.tar` & `anonymity_api-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.973447 anonymity_api-0.1.0/
--rw-rw-rw-   0        0        0      127 2024-05-12 20:24:54.972444 anonymity_api-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-05-12 20:24:09.000000 anonymity_api-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.817398 anonymity_api-0.1.0/anonymity_api/
--rw-rw-rw-   0        0        0      199 2024-03-28 13:20:20.000000 anonymity_api-0.1.0/anonymity_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.876340 anonymity_api-0.1.0/anonymity_api/anonymity/
--rw-rw-rw-   0        0        0     1017 2024-04-12 12:51:25.000000 anonymity_api-0.1.0/anonymity_api/anonymity/__init__.py
--rw-rw-rw-   0        0        0     1828 2024-05-12 13:48:46.000000 anonymity_api-0.1.0/anonymity_api/anonymity/_k_anonymity.py
--rw-rw-rw-   0        0        0     5385 2024-05-12 13:48:45.000000 anonymity_api-0.1.0/anonymity_api/anonymity/_l_diversity.py
--rw-rw-rw-   0        0        0     5084 2024-05-12 13:48:45.000000 anonymity_api-0.1.0/anonymity_api/anonymity/_suggestion.py
--rw-rw-rw-   0        0        0     1571 2024-05-12 13:48:44.000000 anonymity_api-0.1.0/anonymity_api/anonymity/_t_closeness.py
--rw-rw-rw-   0        0        0     7407 2024-05-12 13:48:44.000000 anonymity_api-0.1.0/anonymity_api/anonymity/_workload_aware.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.898317 anonymity_api-0.1.0/anonymity_api/anonymity/utils/
--rw-rw-rw-   0        0        0      121 2024-04-26 15:33:33.000000 anonymity_api-0.1.0/anonymity_api/anonymity/utils/__init__.py
--rw-rw-rw-   0        0        0     9622 2024-05-12 13:48:43.000000 anonymity_api-0.1.0/anonymity_api/anonymity/utils/anon_functions.py
--rw-rw-rw-   0        0        0    13285 2024-05-12 15:55:15.000000 anonymity_api-0.1.0/anonymity_api/anonymity/utils/aux_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.919354 anonymity_api-0.1.0/anonymity_api/utility/
--rw-rw-rw-   0        0        0     1138 2024-05-12 13:48:47.000000 anonymity_api-0.1.0/anonymity_api/utility/__analysis.py
--rw-rw-rw-   0        0        0      421 2024-05-12 13:48:47.000000 anonymity_api-0.1.0/anonymity_api/utility/__init__.py
--rw-rw-rw-   0        0        0     3232 2024-05-12 13:48:46.000000 anonymity_api-0.1.0/anonymity_api/utility/__metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.931869 anonymity_api-0.1.0/anonymity_api/utility/utils/
--rw-rw-rw-   0        0        0      119 2024-04-26 15:38:12.000000 anonymity_api-0.1.0/anonymity_api/utility/utils/__init__.py
--rw-rw-rw-   0        0        0     2220 2024-05-12 12:50:44.000000 anonymity_api-0.1.0/anonymity_api/utility/utils/aux_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.958915 anonymity_api-0.1.0/anonymity_api/verify/
--rw-rw-rw-   0        0        0      480 2024-03-16 21:11:13.000000 anonymity_api-0.1.0/anonymity_api/verify/__init__.py
--rw-rw-rw-   0        0        0      428 2024-05-12 13:48:42.000000 anonymity_api-0.1.0/anonymity_api/verify/_k_anonymity.py
--rw-rw-rw-   0        0        0     1580 2024-05-12 13:48:41.000000 anonymity_api-0.1.0/anonymity_api/verify/_l_diversity.py
--rw-rw-rw-   0        0        0      568 2024-05-12 13:48:40.000000 anonymity_api-0.1.0/anonymity_api/verify/_t_closeness.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.971445 anonymity_api-0.1.0/anonymity_api/verify/utils/
--rw-rw-rw-   0        0        0       90 2024-04-26 15:40:04.000000 anonymity_api-0.1.0/anonymity_api/verify/utils/__init__.py
--rw-rw-rw-   0        0        0     4751 2024-04-26 18:07:11.000000 anonymity_api-0.1.0/anonymity_api/verify/utils/aux_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:24:54.834035 anonymity_api-0.1.0/anonymity_api.egg-info/
--rw-rw-rw-   0        0        0      127 2024-05-12 20:24:54.000000 anonymity_api-0.1.0/anonymity_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-05-12 20:24:54.000000 anonymity_api-0.1.0/anonymity_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 20:24:54.000000 anonymity_api-0.1.0/anonymity_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 20:24:54.000000 anonymity_api-0.1.0/anonymity_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 20:24:54.973447 anonymity_api-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-12 20:24:49.000000 anonymity_api-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.052281 anonymity_api-0.2.0/
+-rw-rw-rw-   0        0        0      127 2024-05-16 10:45:02.051280 anonymity_api-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2024-05-12 20:24:09.000000 anonymity_api-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.026282 anonymity_api-0.2.0/anonymity_api/
+-rw-rw-rw-   0        0        0      199 2024-03-28 13:20:20.000000 anonymity_api-0.2.0/anonymity_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.039279 anonymity_api-0.2.0/anonymity_api/anonymity/
+-rw-rw-rw-   0        0        0     1101 2024-05-16 10:35:18.000000 anonymity_api-0.2.0/anonymity_api/anonymity/__init__.py
+-rw-rw-rw-   0        0        0     1828 2024-05-12 13:48:46.000000 anonymity_api-0.2.0/anonymity_api/anonymity/_k_anonymity.py
+-rw-rw-rw-   0        0        0     5385 2024-05-16 10:38:52.000000 anonymity_api-0.2.0/anonymity_api/anonymity/_l_diversity.py
+-rw-rw-rw-   0        0        0     5640 2024-05-16 10:38:09.000000 anonymity_api-0.2.0/anonymity_api/anonymity/_suggestion.py
+-rw-rw-rw-   0        0        0     1571 2024-05-12 13:48:44.000000 anonymity_api-0.2.0/anonymity_api/anonymity/_t_closeness.py
+-rw-rw-rw-   0        0        0    10703 2024-05-16 10:28:02.000000 anonymity_api-0.2.0/anonymity_api/anonymity/_workload_aware.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.041281 anonymity_api-0.2.0/anonymity_api/anonymity/utils/
+-rw-rw-rw-   0        0        0      121 2024-04-26 15:33:33.000000 anonymity_api-0.2.0/anonymity_api/anonymity/utils/__init__.py
+-rw-rw-rw-   0        0        0     9622 2024-05-12 13:48:43.000000 anonymity_api-0.2.0/anonymity_api/anonymity/utils/anon_functions.py
+-rw-rw-rw-   0        0        0    15207 2024-05-16 10:40:05.000000 anonymity_api-0.2.0/anonymity_api/anonymity/utils/aux_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.044280 anonymity_api-0.2.0/anonymity_api/utility/
+-rw-rw-rw-   0        0        0     2188 2024-05-16 09:44:10.000000 anonymity_api-0.2.0/anonymity_api/utility/__analysis.py
+-rw-rw-rw-   0        0        0      421 2024-05-12 13:48:47.000000 anonymity_api-0.2.0/anonymity_api/utility/__init__.py
+-rw-rw-rw-   0        0        0     3232 2024-05-12 13:48:46.000000 anonymity_api-0.2.0/anonymity_api/utility/__metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.045281 anonymity_api-0.2.0/anonymity_api/utility/utils/
+-rw-rw-rw-   0        0        0      119 2024-04-26 15:38:12.000000 anonymity_api-0.2.0/anonymity_api/utility/utils/__init__.py
+-rw-rw-rw-   0        0        0     2220 2024-05-12 12:50:44.000000 anonymity_api-0.2.0/anonymity_api/utility/utils/aux_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.049279 anonymity_api-0.2.0/anonymity_api/verify/
+-rw-rw-rw-   0        0        0      480 2024-03-16 21:11:13.000000 anonymity_api-0.2.0/anonymity_api/verify/__init__.py
+-rw-rw-rw-   0        0        0      428 2024-05-12 13:48:42.000000 anonymity_api-0.2.0/anonymity_api/verify/_k_anonymity.py
+-rw-rw-rw-   0        0        0     1580 2024-05-12 13:48:41.000000 anonymity_api-0.2.0/anonymity_api/verify/_l_diversity.py
+-rw-rw-rw-   0        0        0      568 2024-05-12 13:48:40.000000 anonymity_api-0.2.0/anonymity_api/verify/_t_closeness.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.050279 anonymity_api-0.2.0/anonymity_api/verify/utils/
+-rw-rw-rw-   0        0        0       90 2024-04-26 15:40:04.000000 anonymity_api-0.2.0/anonymity_api/verify/utils/__init__.py
+-rw-rw-rw-   0        0        0     4751 2024-04-26 18:07:11.000000 anonymity_api-0.2.0/anonymity_api/verify/utils/aux_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:02.034279 anonymity_api-0.2.0/anonymity_api.egg-info/
+-rw-rw-rw-   0        0        0      127 2024-05-16 10:45:01.000000 anonymity_api-0.2.0/anonymity_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-05-16 10:45:01.000000 anonymity_api-0.2.0/anonymity_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 10:45:01.000000 anonymity_api-0.2.0/anonymity_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-16 10:45:01.000000 anonymity_api-0.2.0/anonymity_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 10:45:02.052281 anonymity_api-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-16 10:44:39.000000 anonymity_api-0.2.0/setup.py
```

### Comparing `anonymity_api-0.1.0/anonymity_api/anonymity/__init__.py` & `anonymity_api-0.2.0/anonymity_api/anonymity/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 from ._t_closeness import t_closeness
 from ._workload_aware import workload_aware_k_anonymity
 from ._workload_aware import workload_aware_distinct_l_diversity
 from ._workload_aware import workload_aware_entropy_l_diversity
 from ._workload_aware import workload_aware_recursive_c_l_diversity
 from ._workload_aware import workload_aware_t_closeness
 from ._suggestion import suggest_anonymity
+from ._suggestion import suggest_anonymity_groups
 
 '''This module holds the functions to anonymize datasets'''
 
 __all__ = [
     'k_anonymity',
     'distinct_l_diversity',
     'entropy_l_diversity',
     'recursive_cl_diversity',
     't_closeness',
     'workload_aware_k_anonymity',
     'workload_aware_distinct_l_diversity',
     'workload_aware_entropy_l_diversity',
     'workload_aware_recursive_c_l_diversity',
     'workload_aware_t_closeness',
-    'suggest_anonymity'
+    'suggest_anonymity',
+    'suggest_anonymity_groups'
 ]
```

### Comparing `anonymity_api-0.1.0/anonymity_api/anonymity/_k_anonymity.py` & `anonymity_api-0.2.0/anonymity_api/anonymity/_k_anonymity.py`

 * *Files identical despite different names*

### Comparing `anonymity_api-0.1.0/anonymity_api/anonymity/_l_diversity.py` & `anonymity_api-0.2.0/anonymity_api/anonymity/_l_diversity.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     :param l: The l to be used in anonymization (each partition should have l distinct values for each sensitive attribute after anonymization)
     :param idents: List with the identifiers of the dataframe, default is the empty list (no identifiers)
     :param corr_att: attempt to preserve the correlation between this attribute and the sensitive attributes
     :param taxonomies: hierarchy to be used for quasi-identifer generalization
     
     :returns: Anonymized dataframe'''
     if (l < 1 or l > data[sens_atts].nunique().min()):
-        raise ValueError(f"Invalid value for L. K must be higher than 0 and lower or equal to the number of different values for the least diverse sensitive attributes: ({data[sens_atts].nunique().min()}).")
+        raise ValueError(f"Invalid value for L. L must be higher than 0 and lower or equal to the number of different values for the least diverse sensitive attributes: ({data[sens_atts].nunique().min()}).")
 
     if(idents != []):
         for sa in idents:
             del(data[sa])
             
     if( taxonomies is not None):
         for key in taxonomies.keys():
```

### Comparing `anonymity_api-0.1.0/anonymity_api/anonymity/_suggestion.py` & `anonymity_api-0.2.0/anonymity_api/anonymity/_suggestion.py`

 * *Files 11% similar despite different names*

```diff
@@ -119,8 +119,20 @@
     print(f'Utility for recursive (c,l)-anonymization: {str(r_cl_utility)}')
     
     if r_cl_utility < min_util:
         min_util = r_cl_utility
         best_df = r_cl
     
     return best_df
-    
+    
+    
+def suggest_anonymity_groups(data, quasi_idents, sens, queries, idents =[], taxonomies = None ):
+    
+    groups, queries_proc = aux_functions.check_group(queries)
+    
+    arg_groups, val_groups = aux_functions.process_groups(groups, quasi_idents)
+    
+    data_frames = aux_functions.get_group_dataframes(data, arg_groups, val_groups)
+    
+    data_frames = [suggest_anonymity(data_frames[i], quasi_idents, sens, idents, None, taxonomies) for i in range(len(data_frames))]
+    
+    return pd.concat(data_frames).reset_index(drop = True)
```

### Comparing `anonymity_api-0.1.0/anonymity_api/anonymity/_t_closeness.py` & `anonymity_api-0.2.0/anonymity_api/anonymity/_t_closeness.py`

 * *Files identical despite different names*

### Comparing `anonymity_api-0.1.0/anonymity_api/anonymity/utils/anon_functions.py` & `anonymity_api-0.2.0/anonymity_api/anonymity/utils/anon_functions.py`

 * *Files identical despite different names*

### Comparing `anonymity_api-0.1.0/anonymity_api/anonymity/utils/aux_functions.py` & `anonymity_api-0.2.0/anonymity_api/anonymity/utils/aux_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -249,14 +249,36 @@
             
         elif (pd.api.types.is_string_dtype(partition[sa])):
             if( not is_t_close_categorical(partition, sa, t, data_set)):
                 return False
              
     return True
 
+def get_group_dataframes(data, group_qi, val):
+    '''Divides the dataframe into groups that respect the given grouping
+    
+    :param data: dataframe to be divided
+    :param group_qi: quasi-identifier to group
+    :param val: value to group by
+    
+    :returns: list of dataframes that respect the grouping'''
+    
+    data = data.copy()
+    total = 0
+    groups = list()
+    
+    while total < data[group_qi].max():
+        
+        old_val = total
+        total += val
+        query = f'{group_qi} <= {total} and {group_qi} > {old_val}'
+        groups.append(data.query(query))
+        
+    groups = [group for group in groups if not group.empty]
+    return groups
 
 def get_query_dataframes(data, querys, quasi_idents):
     '''Executes all querys into the data and the returns two dataframes.
     1. Dataframe of the conjunction of all queries
     2. Rest of the original dataframe
     
     :param data: original dataframe
@@ -293,14 +315,34 @@
             corrs.append(query)
             
     for query in corrs:
         aux.remove(query)
             
     return corrs, aux
 
+def check_group( queries ):
+    '''Receives all the queries and if verifies if any of them is a grouping
+    
+    :param queries: the queries to analyze
+    
+    :returns: the grouping if it exists, and the rest of the querys'''
+    
+    aux = queries.copy()
+    
+    groups = list()
+    
+    for query in aux:
+        if query.strip().find('group') == 0:
+            groups.append(query)
+            
+    for query in groups:
+        aux.remove(query)
+        
+    return groups, aux
+
 def process_corr( corrs, quasi_idents ):
     '''Receives the correlation to be done and retreives the quasi-identifier
     in the correlation
     
     :param corrs: correlation to analyze
     :param quasi_idents: all the quasi-identifiers
     
@@ -316,14 +358,36 @@
         for qi in quasi_idents:
             for arg in params:
                 if qi == arg:
                     args.append(qi)
                     
     return args
             
+def process_groups( groups, quasi_idents ):
+    '''Receives the grouping to be done and retreives the quasi-identifier
+    in the grouping
+    
+    :param groups: grouping to analyze
+    :param quasi_idents: all the quasi-identifiers
+    
+    :returns: the quasi-identifier in the grouping'''
+    
+    args = None
+    vals = None
+    
+    for group in groups:
+    
+        params = group.split('(')[1].split(')')[0].split(',')
+        params = [param.strip() for param in params]
+        
+        if params[0] in quasi_idents:
+            args = params[0]
+            vals = params[1]
+                    
+    return args, int(vals)
             
 def find_k( data, quasi_idents ):
     '''Tries to find a k to use in k-anonymization.
     Chooses the k has being the average number of unique values for all quasi-identifiers
     
     :param data: the dataframe
     :param quasi_idents: quasi-identifiers of the dataframe
@@ -372,14 +436,16 @@
         
         
         if med_vc > least_common:
             least_common = med_vc
         
     l_val = recur_l = int(len(data) // 10) if int(least_common) == 1 else int(min(least_common , data[sens].nunique().min()))
     
+    l_val = recur_l = max(l_val, data[sens].nunique().min())
+    
     entropy_l = max(math.log(unique_sas.mean()), 1.1)
      
     while sum(value_counts[recur_l-1:]) < threshold:
         recur_l -= 1
     
     c_val = int(len(data) / sum(value_counts[recur_l-1:]))
```

### Comparing `anonymity_api-0.1.0/anonymity_api/utility/__analysis.py` & `anonymity_api-0.2.0/anonymity_api/utility/__analysis.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 from anonymity_api.utility.utils import aux_functions
 import random
 
-def generalize_intervals( data, qis ):
+def generalize_intervals( data, qis, decimals = None ):
     '''This function receives an anonymized dataset and replaces the generalized values ( intervals or a list of possible values ) with a random value.
     This allows the data to be used in data analysis functions such as correlations, or means that will evaluate these values'''
     
     df = data.copy()
     
-    for index, row in df.iterrows():
-        for i in range(len(qis)):
-            value = str(row[qis[i]]).rstrip()
-            value_str = value.split('-')
-            
-            if len(value_str) > 1:
-                if len(value_str) > 2:
-                    df.loc[index, qis[i]] = value_str[random.randint(0, len(value_str) - 1)]
-                else:
-                    if aux_functions.is_num(value_str[0]):
-                        df.loc[index, qis[i]] = random.randint(int(float(value_str[0])), int(float(value_str[1])))
+    if( decimals is None ):
+        for index, row in df.iterrows():
+            for i in range(len(qis)):
+                value = str(row[qis[i]]).rstrip()
+                value_str = value.split('-')
+                
+                if len(value_str) > 1:
+                    if len(value_str) > 2:
+                        df.loc[index, qis[i]] = value_str[random.randint(0, len(value_str) - 1)]
                     else:
+                        if aux_functions.is_num(value_str[0]):
+                            df.loc[index, qis[i]] = random.randint(int(float(value_str[0])), int(float(value_str[1])))
+                        else:
+                            df.loc[index, qis[i]] = value_str[random.randint(0, len(value_str) - 1)]
+    else:
+        for index, row in df.iterrows():
+            for i in range(len(qis)):
+                value = str(row[qis[i]]).rstrip()
+                value_str = value.split('-')
+                
+                if len(value_str) > 1:
+                    if len(value_str) > 2:
                         df.loc[index, qis[i]] = value_str[random.randint(0, len(value_str) - 1)]
+                    else:
+                        if aux_functions.is_num(value_str[0]):
+                            if qis[i] in decimals:
+                                df.loc[index, qis[i]] = random.uniform(int(float(value_str[0])), int(float(value_str[1])))
+                            else:    
+                                df.loc[index, qis[i]] = random.randint(int(float(value_str[0])), int(float(value_str[1])))
+                        else:
+                            df.loc[index, qis[i]] = value_str[random.randint(0, len(value_str) - 1)]
                         
     return df
```

### Comparing `anonymity_api-0.1.0/anonymity_api/utility/__metrics.py` & `anonymity_api-0.2.0/anonymity_api/utility/__metrics.py`

 * *Files identical despite different names*

### Comparing `anonymity_api-0.1.0/anonymity_api/utility/utils/aux_functions.py` & `anonymity_api-0.2.0/anonymity_api/utility/utils/aux_functions.py`

 * *Files identical despite different names*

### Comparing `anonymity_api-0.1.0/anonymity_api/verify/_l_diversity.py` & `anonymity_api-0.2.0/anonymity_api/verify/_l_diversity.py`

 * *Files identical despite different names*

### Comparing `anonymity_api-0.1.0/anonymity_api/verify/_t_closeness.py` & `anonymity_api-0.2.0/anonymity_api/verify/_t_closeness.py`

 * *Files identical despite different names*

### Comparing `anonymity_api-0.1.0/anonymity_api/verify/utils/aux_functions.py` & `anonymity_api-0.2.0/anonymity_api/verify/utils/aux_functions.py`

 * *Files identical despite different names*

### Comparing `anonymity_api-0.1.0/anonymity_api.egg-info/SOURCES.txt` & `anonymity_api-0.2.0/anonymity_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

