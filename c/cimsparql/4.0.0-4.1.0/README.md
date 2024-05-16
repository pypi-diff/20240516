# Comparing `tmp/cimsparql-4.0.0.tar.gz` & `tmp/cimsparql-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cimsparql-4.0.0.tar", max compression
+gzip compressed data, was "cimsparql-4.1.0.tar", max compression
```

## Comparing `cimsparql-4.0.0.tar` & `cimsparql-4.1.0.tar`

### file list

```diff
@@ -1,56 +1,55 @@
--rw-r--r--   0        0        0     1065 2024-05-13 13:08:10.129235 cimsparql-4.0.0/LICENSE
--rw-r--r--   0        0        0     5195 2024-05-13 13:08:10.129235 cimsparql-4.0.0/README.md
--rw-r--r--   0        0        0       60 2024-05-13 13:08:24.753188 cimsparql-4.0.0/cimsparql/__init__.py
--rw-r--r--   0        0        0     4744 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/adaptions.py
--rw-r--r--   0        0        0     1642 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/constants.py
--rw-r--r--   0        0        0     9739 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/data_models.py
--rw-r--r--   0        0        0    16044 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/graphdb.py
--rw-r--r--   0        0        0    28744 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/model.py
--rw-r--r--   0        0        0     5202 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/ac_lines.sparql
--rw-r--r--   0        0        0      221 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/add_mrid.sparql
--rw-r--r--   0        0        0     1761 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/borders.sparql
--rw-r--r--   0        0        0     2073 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/branch_node_withdraw.sparql
--rw-r--r--   0        0        0     1795 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/bus.sparql
--rw-r--r--   0        0        0      984 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/connections.sparql
--rw-r--r--   0        0        0     1291 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/connectivity_nodes.sparql
--rw-r--r--   0        0        0      737 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/converter_hvdc_bidzones.sparql
--rw-r--r--   0        0        0     2614 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/converters.sparql
--rw-r--r--   0        0        0      588 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/coordinates.sparql
--rw-r--r--   0        0        0     2521 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/dc_active_power_flow.sparql
--rw-r--r--   0        0        0      242 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/disconnected.sparql
--rw-r--r--   0        0        0     3063 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/exchange.sparql
--rw-r--r--   0        0        0      792 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/full_model.sparql
--rw-r--r--   0        0        0     2813 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/loads.sparql
--rw-r--r--   0        0        0      287 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/market_dates.sparql
--rw-r--r--   0        0        0      523 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/power_flow.sparql
--rw-r--r--   0        0        0      397 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/ras_equipment.sparql
--rw-r--r--   0        0        0      573 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/regions.sparql
--rw-r--r--   0        0        0     3655 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/series_compensators.sparql
--rw-r--r--   0        0        0      426 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/station_group_code_and_names.sparql
--rw-r--r--   0        0        0      645 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/substation_voltage_level.sparql
--rw-r--r--   0        0        0     2877 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/sv_branch.sparql
--rw-r--r--   0        0        0      245 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/sv_injection.sparql
--rw-r--r--   0        0        0      781 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/switches.sparql
--rw-r--r--   0        0        0     3285 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/synchronous_machines.sparql
--rw-r--r--   0        0        0      318 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
--rw-r--r--   0        0        0     3461 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformer_branches.sparql
--rw-r--r--   0        0        0     1461 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformer_center_nodes.sparql
--rw-r--r--   0        0        0      363 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformer_windings.sparql
--rw-r--r--   0        0        0     1269 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformers.sparql
--rw-r--r--   0        0        0     1844 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformers_connected_to_converter.sparql
--rw-r--r--   0        0        0     4520 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/two_winding_transformer.sparql
--rw-r--r--   0        0        0      880 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/two_winding_transformer_angle.sparql
--rw-r--r--   0        0        0      461 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/type_mapper.sparql
--rw-r--r--   0        0        0      814 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/wind_generating_units.sparql
--rw-r--r--   0        0        0      944 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/winding.sparql
--rw-r--r--   0        0        0     1277 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/winding_loss.sparql
--rw-r--r--   0        0        0     2298 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql_result_json.py
--rw-r--r--   0        0        0     3193 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/templates.py
--rw-r--r--   0        0        0     5650 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/type_mapper.py
--rw-r--r--   0        0        0      768 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/url.py
--rw-r--r--   0        0        0      616 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/value_mapper.py
--rw-r--r--   0        0        0      459 2024-05-13 13:08:10.141235 cimsparql-4.0.0/pkg_data/blazegraph_repo_config.xml
--rw-r--r--   0        0        0      676 2024-05-13 13:08:10.141235 cimsparql-4.0.0/pkg_data/namespaces.json
--rw-r--r--   0        0        0      805 2024-05-13 13:08:10.141235 cimsparql-4.0.0/pkg_data/native_store_config_template.ttl
--rw-r--r--   0        0        0     4219 2024-05-13 13:08:24.753188 cimsparql-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 cimsparql-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-16 08:56:47.811139 cimsparql-4.1.0/LICENSE
+-rw-r--r--   0        0        0     5195 2024-05-16 08:56:47.811139 cimsparql-4.1.0/README.md
+-rw-r--r--   0        0        0       60 2024-05-16 08:57:06.818949 cimsparql-4.1.0/cimsparql/__init__.py
+-rw-r--r--   0        0        0     4744 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/adaptions.py
+-rw-r--r--   0        0        0     1642 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/constants.py
+-rw-r--r--   0        0        0     9830 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/data_models.py
+-rw-r--r--   0        0        0    16044 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/graphdb.py
+-rw-r--r--   0        0        0    27478 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/model.py
+-rw-r--r--   0        0        0     5202 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/ac_lines.sparql
+-rw-r--r--   0        0        0      221 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/add_mrid.sparql
+-rw-r--r--   0        0        0     1761 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/borders.sparql
+-rw-r--r--   0        0        0     2073 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/branch_node_withdraw.sparql
+-rw-r--r--   0        0        0     1795 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/bus.sparql
+-rw-r--r--   0        0        0      984 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/connections.sparql
+-rw-r--r--   0        0        0     1291 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/connectivity_nodes.sparql
+-rw-r--r--   0        0        0      737 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/converter_hvdc_bidzones.sparql
+-rw-r--r--   0        0        0     2614 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/converters.sparql
+-rw-r--r--   0        0        0      588 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/coordinates.sparql
+-rw-r--r--   0        0        0     1373 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/dc_active_power_flow.sparql
+-rw-r--r--   0        0        0      242 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/disconnected.sparql
+-rw-r--r--   0        0        0     3063 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/exchange.sparql
+-rw-r--r--   0        0        0      792 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/full_model.sparql
+-rw-r--r--   0        0        0     2813 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/loads.sparql
+-rw-r--r--   0        0        0      287 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/market_dates.sparql
+-rw-r--r--   0        0        0      523 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/power_flow.sparql
+-rw-r--r--   0        0        0      397 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/ras_equipment.sparql
+-rw-r--r--   0        0        0      573 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/regions.sparql
+-rw-r--r--   0        0        0     3655 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/series_compensators.sparql
+-rw-r--r--   0        0        0      426 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/station_group_code_and_names.sparql
+-rw-r--r--   0        0        0      645 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/substation_voltage_level.sparql
+-rw-r--r--   0        0        0     2877 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/sv_branch.sparql
+-rw-r--r--   0        0        0      245 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/sv_injection.sparql
+-rw-r--r--   0        0        0      781 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/switches.sparql
+-rw-r--r--   0        0        0     3285 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/synchronous_machines.sparql
+-rw-r--r--   0        0        0      318 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
+-rw-r--r--   0        0        0     3752 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformer_branches.sparql
+-rw-r--r--   0        0        0     1461 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformer_center_nodes.sparql
+-rw-r--r--   0        0        0      720 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformer_winding_angle.sparql
+-rw-r--r--   0        0        0      363 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformer_windings.sparql
+-rw-r--r--   0        0        0     1269 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformers.sparql
+-rw-r--r--   0        0        0     1844 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformers_connected_to_converter.sparql
+-rw-r--r--   0        0        0      461 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/type_mapper.sparql
+-rw-r--r--   0        0        0      814 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/wind_generating_units.sparql
+-rw-r--r--   0        0        0      944 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/winding.sparql
+-rw-r--r--   0        0        0     1189 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/winding_loss.sparql
+-rw-r--r--   0        0        0     2298 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql_result_json.py
+-rw-r--r--   0        0        0     3112 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/templates.py
+-rw-r--r--   0        0        0     5650 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/type_mapper.py
+-rw-r--r--   0        0        0      768 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/url.py
+-rw-r--r--   0        0        0      616 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/value_mapper.py
+-rw-r--r--   0        0        0      459 2024-05-16 08:56:47.823139 cimsparql-4.1.0/pkg_data/blazegraph_repo_config.xml
+-rw-r--r--   0        0        0      676 2024-05-16 08:56:47.823139 cimsparql-4.1.0/pkg_data/namespaces.json
+-rw-r--r--   0        0        0      805 2024-05-16 08:56:47.823139 cimsparql-4.1.0/pkg_data/native_store_config_template.ttl
+-rw-r--r--   0        0        0     4333 2024-05-16 08:57:06.818949 cimsparql-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 cimsparql-4.1.0/PKG-INFO
```

### Comparing `cimsparql-4.0.0/LICENSE` & `cimsparql-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/README.md` & `cimsparql-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/adaptions.py` & `cimsparql-4.1.0/cimsparql/adaptions.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/constants.py` & `cimsparql-4.1.0/cimsparql/constants.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/data_models.py` & `cimsparql-4.1.0/cimsparql/data_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,16 @@
     alias: Series[str] = pa.Field(nullable=True)
     substation_mrid: Series[str] = pa.Field()
     status: Series[bool] = pa.Field()
     node: Series[str] = pa.Field()
     p: Series[float] = pa.Field()
     q: Series[float] = pa.Field()
     connectivity_node: Series[str] = pa.Field()
+    controller: Series[str] = pa.Field()
+    controller_factor: Series[float] = pa.Field()
 
 
 ConvertersDataFrame = DataFrame[ConvertersSchema]
 
 
 class TransfConToConverterSchema(NamedResourceSchema):
     t_mrid: Series[str] = pa.Field()
```

### Comparing `cimsparql-4.0.0/cimsparql/graphdb.py` & `cimsparql-4.1.0/cimsparql/graphdb.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/model.py` & `cimsparql-4.1.0/cimsparql/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,46 +433,17 @@
         Args:
            region: Limit to region
         """
         query = self.transformers_query(region, rate)
         df = self.get_table_and_convert(query)
         return TransformersDataFrame(df)
 
-    def two_winding_transformers_query(
-        self, region: str | None = None, rate: str | None = None
-    ) -> str:
-        substitutes = {"region": region or ".*", "rate": rate or "Normal@20"}
-        return self.template_to_query(templates.TWO_WINDING_QUERY, substitutes)
-
-    def two_winding_angle_query(self, region: str | None = None) -> str:
+    def winding_angle_query(self, region: str | None = None) -> str:
         substitutes = {"region": region or ".*"}
-        return self.template_to_query(templates.TWO_WINDING_ANGLE_QUERY, substitutes)
-
-    @time_it
-    def two_winding_transformers(
-        self, region: str | None = None, rate: str | None = None
-    ) -> TransformerWindingDataFrame:
-        """Query two-winding transformer.
-
-        Args:
-           region: Limit to region
-
-        Example:
-            >>> from cimsparql.model import get_single_client_model
-            >>> server_url = "127.0.0.1:7200"
-            >>> model = get_single_client_model(server_url, "LATEST")
-            >>> model.two_winding_transformers()
-        """
-        query = self.two_winding_transformers_query(region, rate)
-        query_angle = self.two_winding_angle_query(region)
-        data = self.get_table_and_convert(query, index="mrid")
-        angle = self.get_table_and_convert(query_angle, index="mrid")
-        if not angle.empty:
-            data["angle"] += angle.reindex(index=data.index, fill_value=0.0).squeeze()
-        return TransformerWindingDataFrame(data)
+        return self.template_to_query(templates.TRANSFORMER_WINDING_ANGLE_QUERY, substitutes)
 
     @property
     def winding_query(self) -> str:
         return self.template_to_query(templates.WINDING)
 
     def winding_loss_query(self, region: str | None = None) -> str:
         substitutes = {"region": region or ".*"}
@@ -505,19 +476,19 @@
             >>> model = get_single_client_model(server_url, "LATEST")
             >>> model.transformer_branches()
         """
         query = self.transformer_branches_query(region, rate)
         data = self.get_table_and_convert(query, index="mrid")
         query_loss = self.winding_loss_query(region)
         loss = self.get_table_and_convert(query_loss, index="mrid")
-        df = pd.concat([data.assign(ploss_1=0.0), loss.loc[data.index]], axis=1)
-        query_angle = self.two_winding_angle_query(region)
+        df = data.assign(ploss_1=0.0, ploss_2=lambda df: df["node_2"].map(loss["ploss_2"]))
+        query_angle = self.winding_angle_query(region)
         angle = self.get_table_and_convert(query_angle, index="mrid")
         if not angle.empty:
-            data["angle"] += angle.reindex(index=data.index, fill_value=0.0).squeeze()
+            data.loc[angle.index, "angle"] = angle
         return TransformerWindingDataFrame(df)
 
     @property
     def substation_voltage_level_query(self) -> str:
         return self.template_to_query(templates.SUBSTATION_VOLTAGE_LEVEL_QUERY)
 
     def substation_voltage_level(self) -> SubstationVoltageDataFrame:
@@ -771,15 +742,14 @@
         "SV branch",
         "Power flow",
         "SvInjection",
         "Switches",
         "Transformer branches",
         "Transformer branches loss",
         "Transformer center nodes",
-        "Two winding transformer",
         "Synchronous machines",
         "Windings",
         "Winding transformer angle",
     )
     for query in exec_from_tpssvssh:
         clients[query] = tpsvssh_client
     return Model(clients, model_cfg, mapper)
```

### Comparing `cimsparql-4.0.0/cimsparql/sparql/ac_lines.sparql` & `cimsparql-4.1.0/cimsparql/sparql/ac_lines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/borders.sparql` & `cimsparql-4.1.0/cimsparql/sparql/borders.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/branch_node_withdraw.sparql` & `cimsparql-4.1.0/cimsparql/sparql/branch_node_withdraw.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/bus.sparql` & `cimsparql-4.1.0/cimsparql/sparql/bus.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/connections.sparql` & `cimsparql-4.1.0/cimsparql/sparql/connections.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/connectivity_nodes.sparql` & `cimsparql-4.1.0/cimsparql/sparql/connectivity_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/converter_hvdc_bidzones.sparql` & `cimsparql-4.1.0/cimsparql/sparql/converter_hvdc_bidzones.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/converters.sparql` & `cimsparql-4.1.0/cimsparql/sparql/converters.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/coordinates.sparql` & `cimsparql-4.1.0/cimsparql/sparql/coordinates.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/exchange.sparql` & `cimsparql-4.1.0/cimsparql/sparql/exchange.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/full_model.sparql` & `cimsparql-4.1.0/cimsparql/sparql/full_model.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/loads.sparql` & `cimsparql-4.1.0/cimsparql/sparql/loads.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/power_flow.sparql` & `cimsparql-4.1.0/cimsparql/sparql/power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/regions.sparql` & `cimsparql-4.1.0/cimsparql/sparql/regions.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/series_compensators.sparql` & `cimsparql-4.1.0/cimsparql/sparql/series_compensators.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/substation_voltage_level.sparql` & `cimsparql-4.1.0/cimsparql/sparql/substation_voltage_level.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/sv_branch.sparql` & `cimsparql-4.1.0/cimsparql/sparql/sv_branch.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/switches.sparql` & `cimsparql-4.1.0/cimsparql/sparql/switches.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/synchronous_machines.sparql` & `cimsparql-4.1.0/cimsparql/sparql/synchronous_machines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/transformer_branches.sparql` & `cimsparql-4.1.0/cimsparql/sparql/transformer_branches.sparql`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 # Name: Transformer branches
 PREFIX cim: <${cim}>
 PREFIX SN: <${SN}>
 PREFIX xsd: <${xsd}>
 # Name: Transformer branches
 select ?node_1 ?node_2 ?status ?name ?mrid ?un ?r ?x ?b ?g ?rate (?bidzone as ?bidzone_1) (?bidzone as ?bidzone_2) ?angle ?ratio ?connectivity_node_1 (?node_2 as ?connectivity_node_2)
 where {
-  ?con_node cim:ConnectivityNode.TopologicalNode/cim:IdentifiedObject.mRID ?node_1 .
+
+  {
+    ?con_node cim:ConnectivityNode.TopologicalNode ?top_node
+  } union {
+    # Get topological node directly from the terminal when it does not
+    # exist via the connectivity node
+    filter not exists {?con_node cim:ConnectivityNode.TopologicalNode ?top_node }
+    ?terminal cim:Terminal.TopologicalNode ?top_node
+  }.
+
+  ?top_node cim:IdentifiedObject.mRID ?node_1 .
   ?terminal cim:ACDCTerminal.connected ?connected .
   optional {?winding ^cim:SvStatus.ConductingEquipment/cim:SvStatus.inService ?in_service} .
 
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
     # Use mrid of transformer as dummy node
     ?p_transformer cim:IdentifiedObject.mRID ?node_2;
```

### Comparing `cimsparql-4.0.0/cimsparql/sparql/transformer_center_nodes.sparql` & `cimsparql-4.1.0/cimsparql/sparql/transformer_center_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/transformers.sparql` & `cimsparql-4.1.0/cimsparql/sparql/transformers.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/transformers_connected_to_converter.sparql` & `cimsparql-4.1.0/cimsparql/sparql/transformers_connected_to_converter.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/two_winding_transformer_angle.sparql` & `cimsparql-4.1.0/cimsparql/sparql/transformer_winding_angle.sparql`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Name: Winding transformer angle
 PREFIX cim: <${cim}>
-PREFIX rdf: <${rdf}>
 PREFIX xsd: <${xsd}>
 select ?mrid ?angle
 where {
   ?tap_changer cim:TapChanger.step ?ssh_position .
   optional{ ?tap_changer ^cim:SvTapStep.TapChanger/cim:SvTapStep.position ?sv_position } .
 
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
-    ?winding cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
-              cim:IdentifiedObject.mRID ?mrid .
     ?tap_changer cim:PhaseTapChangerLinear.stepPhaseShiftIncrement ?inc;
-                cim:TapChanger.normalStep ?normalstep;
-                ^cim:PhaseTapChanger.TransformerEnd/cim:PowerTransformerEnd.PowerTransformer ?p_transformer .
+                cim:TapChanger.neutralStep ?neutralstep;
+                ^cim:TransformerEnd.PhaseTapChanger/cim:IdentifiedObject.mRID ?mrid .
   }
 
   bind(coalesce(?sv_position, ?ssh_position) as ?position)
-  bind((xsd:double(str(?position)) - xsd:double(str(?normalstep))) * xsd:double(str(?inc)) as ?angle)
+  bind((xsd:double(str(?position)) - xsd:double(str(?neutralstep))) * xsd:double(str(?inc)) as ?angle)
 }
```

### Comparing `cimsparql-4.0.0/cimsparql/sparql/wind_generating_units.sparql` & `cimsparql-4.1.0/cimsparql/sparql/wind_generating_units.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/winding.sparql` & `cimsparql-4.1.0/cimsparql/sparql/winding.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/sparql/winding_loss.sparql` & `cimsparql-4.1.0/cimsparql/sparql/winding_loss.sparql`

 * *Files 21% similar despite different names*

```diff
@@ -8,20 +8,20 @@
   ?terminal cim:ACDCTerminal.connected ?connected .
   optional {?terminal ^cim:SvPowerFlow.Terminal/cim:SvPowerFlow.p ?_sv_p  .}
   optional {?winding ^cim:SvStatus.ConductingEquipment/cim:SvStatus.inService ?_in_service}.
 
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
     # Extract mRID and area for each power transformer
-    ?p_transformer a cim:PowerTransformer;
-            ^cim:PowerTransformerEnd.PowerTransformer/cim:IdentifiedObject.mRID ?mrid;
-            cim:Equipment.EquipmentContainer/cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area .
-    filter(regex(?area, '.*'))
+
     ?winding cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
-    		     cim:TransformerEnd.Terminal ?terminal .
+    	cim:TransformerEnd.Terminal ?terminal .
+    ?p_transformer cim:IdentifiedObject.mRID ?mrid ;
+      cim:Equipment.EquipmentContainer/cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area .
+    filter(regex(?area, '.*'))
     optional {?p_transformer SN:Equipment.networkAnalysisEnable ?_network_analysis}
   }
 
   bind(if(coalesce(?_in_service, ?connected), 1, 0) as ?in_service) .
   bind(coalesce(?_sv_p, xsd:double(0.0)) as ?sv_p)
   bind(coalesce(?_network_analysis, True) as ?network_analysis)
   filter(?network_analysis)
```

### Comparing `cimsparql-4.0.0/cimsparql/sparql_result_json.py` & `cimsparql-4.1.0/cimsparql/sparql_result_json.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/templates.py` & `cimsparql-4.1.0/cimsparql/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,13 @@
 SWITCHES_QUERY = _read_template(sparql_folder / "switches.sparql")
 TRANSFORMER_BRANCHES_QUERY = _read_template(sparql_folder / "transformer_branches.sparql")
 TRANSFORMER_CENTER_NODES_QUERY = _read_template(sparql_folder / "transformer_center_nodes.sparql")
 TRANSFORMERS_QUERY = _read_template(sparql_folder / "transformers.sparql")
 TRANSFORMERS_CONNECTED_TO_CONVERTER_QUERY = _read_template(
     sparql_folder / "transformers_connected_to_converter.sparql"
 )
-TWO_WINDING_ANGLE_QUERY = _read_template(sparql_folder / "two_winding_transformer_angle.sparql")
-TWO_WINDING_QUERY = _read_template(sparql_folder / "two_winding_transformer.sparql")
+TRANSFORMER_WINDING_ANGLE_QUERY = _read_template(sparql_folder / "transformer_winding_angle.sparql")
 TYPE_MAPPER_QUERY = _read_template(sparql_folder / "type_mapper.sparql")
 WIND_GENERATING_UNITS_QUERY = _read_template(sparql_folder / "wind_generating_units.sparql")
 TRANSFORMER_WINDINGS_QUERY = _read_template(sparql_folder / "transformer_windings.sparql")
 WINDING = _read_template(sparql_folder / "winding.sparql")
 WINDING_LOSS_QUERY = _read_template(sparql_folder / "winding_loss.sparql")
```

### Comparing `cimsparql-4.0.0/cimsparql/type_mapper.py` & `cimsparql-4.1.0/cimsparql/type_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/url.py` & `cimsparql-4.1.0/cimsparql/url.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/cimsparql/value_mapper.py` & `cimsparql-4.1.0/cimsparql/value_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/pkg_data/namespaces.json` & `cimsparql-4.1.0/pkg_data/namespaces.json`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/pkg_data/native_store_config_template.ttl` & `cimsparql-4.1.0/pkg_data/native_store_config_template.ttl`

 * *Files identical despite different names*

### Comparing `cimsparql-4.0.0/pyproject.toml` & `cimsparql-4.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cimsparql"
-version = "4.0.0"
+version = "4.1.0"
 description = "CIM query utilities"
 readme = "README.md"
 authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>"]
 repository = "https://github.com/statnett/cimsparql.git"
 include = ["pkg_data/*"]
 exclude = ["tests/*"]
 
@@ -158,14 +158,18 @@
 
 [tool.pytest.ini_options]
 asyncio_mode = 'auto'
 log_file = "pytest.log"
 log_level = "DEBUG"
 log_file_format = "%(asctime)s - %(name)s - %(levelname)s: %(message)s"
 norecursedirs = "_build tmp*  __pycache__ src prof wheel_files tests/t_utils"
+filterwarnings = [
+  "ignore: NQuadsSerializer does not use custom encoding. Given encoding was.*:UserWarning"
+]
+
 markers = [
   "integration: Mark test as an integration test",
   "slow: marks tests as slow (deselect with '-m \"not slow\"')"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
```

### Comparing `cimsparql-4.0.0/PKG-INFO` & `cimsparql-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cimsparql
-Version: 4.0.0
+Version: 4.1.0
 Summary: CIM query utilities
 Home-page: https://github.com/statnett/cimsparql.git
 Author: Statnett Datascience
 Author-email: Datascience.Drift@Statnett.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

