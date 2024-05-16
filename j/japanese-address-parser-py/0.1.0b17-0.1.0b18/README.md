# Comparing `tmp/japanese_address_parser_py-0.1.0b17.tar.gz` & `tmp/japanese_address_parser_py-0.1.0b18.tar.gz`

## Comparing `japanese_address_parser_py-0.1.0b17.tar` & `japanese_address_parser_py-0.1.0b18.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0     1001      127      788 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/Cargo.toml
--rw-r--r--   0     1001      127     1065 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/LICENSE
--rw-r--r--   0     1001      127     4500 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/api/city_master_api.rs
--rw-r--r--   0     1001      127     4988 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/api/prefecture_master_api.rs
--rw-r--r--   0     1001      127     2094 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/api.rs
--rw-r--r--   0     1001      127     1794 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/entity.rs
--rw-r--r--   0     1001      127     1326 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/err.rs
--rw-r--r--   0     1001      127      206 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/lib.rs
--rw-r--r--   0     1001      127     3131 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/adapter/orthographical_variant_adapter.rs
--rw-r--r--   0     1001      127     2794 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/adapter/vague_expression_adapter.rs
--rw-r--r--   0     1001      127       74 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/adapter.rs
--rw-r--r--   0     1001      127      570 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/filter/fullwidth_character.rs
--rw-r--r--   0     1001      127     7292 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/filter/invalid_town_name_format.rs
--rw-r--r--   0     1001      127     3393 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/filter/non_kanji_block_number.rs
--rw-r--r--   0     1001      127      162 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/filter.rs
--rw-r--r--   0     1001      127     3739 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/read_city.rs
--rw-r--r--   0     1001      127     2293 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/read_house_number.rs
--rw-r--r--   0     1001      127     1739 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/read_prefecture.rs
--rw-r--r--   0     1001      127     7090 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/read_town.rs
--rw-r--r--   0     1001      127    10962 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser.rs
--rw-r--r--   0     1001      127     3695 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/util/converter.rs
--rw-r--r--   0     1001      127     8133 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/util/sequence_matcher.rs
--rw-r--r--   0     1001      127       45 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/util.rs
--rw-r--r--   0     1001      127     2794 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/README.md
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b17/python/Cargo.toml
--rw-r--r--   0     1001      127     3302 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/python/README.md
--rw-r--r--   0     1001      127     1265 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/python/japanese_address_parser_py.pyi
--rw-r--r--   0     1001      127     1703 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/python/src/lib.rs
--rw-r--r--   0     1001      127    35921 2024-04-28 17:41:07.000000 japanese_address_parser_py-0.1.0b17/Cargo.lock
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b17/Cargo.toml
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b17/pyproject.toml
--rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b17/PKG-INFO
+-rw-r--r--   0     1001      127      788 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/Cargo.toml
+-rw-r--r--   0     1001      127     1065 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/LICENSE
+-rw-r--r--   0     1001      127     4386 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/api/city_master_api.rs
+-rw-r--r--   0     1001      127     4823 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/api/prefecture_master_api.rs
+-rw-r--r--   0     1001      127     1325 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/api.rs
+-rw-r--r--   0     1001      127     1794 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/entity.rs
+-rw-r--r--   0     1001      127     1326 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/err.rs
+-rw-r--r--   0     1001      127      206 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/lib.rs
+-rw-r--r--   0     1001      127     3131 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/adapter/orthographical_variant_adapter.rs
+-rw-r--r--   0     1001      127     2791 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/adapter/vague_expression_adapter.rs
+-rw-r--r--   0     1001      127       74 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/adapter.rs
+-rw-r--r--   0     1001      127      570 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/filter/fullwidth_character.rs
+-rw-r--r--   0     1001      127     7292 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/filter/invalid_town_name_format.rs
+-rw-r--r--   0     1001      127     3393 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/filter/non_kanji_block_number.rs
+-rw-r--r--   0     1001      127      162 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/filter.rs
+-rw-r--r--   0     1001      127     3752 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/read_city.rs
+-rw-r--r--   0     1001      127     2293 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/read_house_number.rs
+-rw-r--r--   0     1001      127     1739 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/read_prefecture.rs
+-rw-r--r--   0     1001      127     7116 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser/read_town.rs
+-rw-r--r--   0     1001      127    11109 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/parser.rs
+-rw-r--r--   0     1001      127     3695 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/util/converter.rs
+-rw-r--r--   0     1001      127     8133 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/util/sequence_matcher.rs
+-rw-r--r--   0     1001      127       45 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/core/src/util.rs
+-rw-r--r--   0     1001      127     2820 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/README.md
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b18/python/Cargo.toml
+-rw-r--r--   0     1001      127     3302 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/python/README.md
+-rw-r--r--   0     1001      127     1265 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/python/japanese_address_parser_py.pyi
+-rw-r--r--   0     1001      127     1721 2024-05-05 18:31:56.000000 japanese_address_parser_py-0.1.0b18/python/src/lib.rs
+-rw-r--r--   0     1001      127    35921 2024-05-05 18:32:00.000000 japanese_address_parser_py-0.1.0b18/Cargo.lock
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b18/Cargo.toml
+-rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b18/pyproject.toml
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b18/PKG-INFO
```

### Comparing `japanese_address_parser_py-0.1.0b17/core/Cargo.toml` & `japanese_address_parser_py-0.1.0b18/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/LICENSE` & `japanese_address_parser_py-0.1.0b18/core/LICENSE`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/api/city_master_api.rs` & `japanese_address_parser_py-0.1.0b18/core/src/api/city_master_api.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 use crate::entity::{City, Town};
 use crate::err::{ApiErrorKind, Error};
 
 pub struct CityMasterApi {
     pub server_url: &'static str,
 }
 
+impl Default for CityMasterApi {
+    fn default() -> Self {
+        Self {
+            server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
+        }
+    }
+}
+
 impl CityMasterApi {
     pub async fn get(&self, prefecture_name: &str, city_name: &str) -> Result<City, Error> {
         let endpoint = format!("{}/{}/{}.json", self.server_url, prefecture_name, city_name);
         let response = match reqwest::get(&endpoint).await {
             Ok(result) => result,
             Err(_) => return Err(Error::new_api_error(ApiErrorKind::Deserialize(endpoint))),
         };
@@ -48,34 +56,30 @@
 #[cfg(all(test, not(feature = "blocking")))]
 mod tests {
     use crate::api::city_master_api::CityMasterApi;
     use crate::entity::Town;
 
     #[tokio::test]
     async fn 非同期_石川県羽咋郡志賀町_成功() {
-        let city_master_api = CityMasterApi {
-            server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
-        };
+        let city_master_api: CityMasterApi = Default::default();
         let result = city_master_api.get("石川県", "羽咋郡志賀町").await;
         let city = result.unwrap();
         assert_eq!(city.name, "羽咋郡志賀町");
         let town = Town {
             name: "末吉".to_string(),
             koaza: "千古".to_string(),
             lat: Some(37.006235),
             lng: Some(136.779155),
         };
         assert!(city.towns.contains(&town));
     }
 
     #[tokio::test]
     async fn 非同期_誤った市区町村名_失敗() {
-        let city_master_api = CityMasterApi {
-            server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
-        };
+        let city_master_api: CityMasterApi = Default::default();
         let result = city_master_api.get("石川県", "敦賀市").await;
         assert!(result.is_err());
         assert_eq!(
             result.err().unwrap().error_message,
             format!(
                 "{}/石川県/敦賀市.jsonを取得できませんでした",
                 city_master_api.server_url
@@ -87,34 +91,30 @@
 #[cfg(all(test, feature = "blocking"))]
 mod blocking_tests {
     use crate::api::city_master_api::CityMasterApi;
     use crate::entity::Town;
 
     #[test]
     fn 同期_石川県羽咋郡志賀町_成功() {
-        let city_master_api = CityMasterApi {
-            server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
-        };
+        let city_master_api: CityMasterApi = Default::default();
         let result = city_master_api.get_blocking("石川県", "羽咋郡志賀町");
         let city = result.unwrap();
         assert_eq!(city.name, "羽咋郡志賀町");
         let town = Town {
             name: "末吉".to_string(),
             koaza: "千古".to_string(),
             lat: Some(37.006235),
             lng: Some(136.779155),
         };
         assert!(city.towns.contains(&town));
     }
 
     #[test]
     fn 同期_誤った市区町村名_失敗() {
-        let city_master_api = CityMasterApi {
-            server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
-        };
+        let city_master_api: CityMasterApi = Default::default();
         let result = city_master_api.get_blocking("石川県", "敦賀市");
         assert!(result.is_err());
         assert_eq!(
             result.err().unwrap().error_message,
             format!(
                 "{}/石川県/敦賀市.jsonを取得できませんでした",
                 city_master_api.server_url
```

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/api/prefecture_master_api.rs` & `japanese_address_parser_py-0.1.0b18/core/src/api/prefecture_master_api.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 use crate::entity::Prefecture;
 use crate::err::{ApiErrorKind, Error};
 
 pub struct PrefectureMasterApi {
     pub server_url: &'static str,
 }
 
+impl Default for PrefectureMasterApi {
+    fn default() -> Self {
+        Self {
+            server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
+        }
+    }
+}
+
 impl PrefectureMasterApi {
     pub async fn get(&self, prefecture_name: &str) -> Result<Prefecture, Error> {
         let endpoint = format!("{}/{}/master.json", self.server_url, prefecture_name);
         let response = match reqwest::get(&endpoint).await {
             Ok(result) => result,
             Err(_) => return Err(Error::new_api_error(ApiErrorKind::Fetch(endpoint))),
         };
@@ -41,17 +49,15 @@
 
 #[cfg(all(test, not(feature = "blocking")))]
 mod tests {
     use crate::api::prefecture_master_api::PrefectureMasterApi;
 
     #[tokio::test]
     async fn 非同期_富山県_成功() {
-        let prefecture_master_api = PrefectureMasterApi {
-            server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
-        };
+        let prefecture_master_api: PrefectureMasterApi = Default::default();
         let result = prefecture_master_api.get("富山県").await;
         let prefecture = result.unwrap();
         assert_eq!(prefecture.name, "富山県");
         let cities = vec![
             "富山市",
             "高岡市",
             "魚津市",
@@ -71,17 +77,15 @@
         for city in cities {
             assert!(prefecture.cities.contains(&city.to_string()));
         }
     }
 
     #[tokio::test]
     async fn 非同期_誤った都道府県名_失敗() {
-        let prefecture_master_api = PrefectureMasterApi {
-            server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
-        };
+        let prefecture_master_api: PrefectureMasterApi = Default::default();
         let result = prefecture_master_api.get("大阪都").await;
         assert!(result.is_err());
         assert_eq!(
             result.err().unwrap().error_message,
             format!(
                 "{}/大阪都/master.jsonを取得できませんでした",
                 prefecture_master_api.server_url
@@ -92,17 +96,15 @@
 
 #[cfg(all(test, feature = "blocking"))]
 mod blocking_tests {
     use crate::api::prefecture_master_api::PrefectureMasterApi;
 
     #[test]
     fn 同期_富山県_成功() {
-        let prefecture_master_api = PrefectureMasterApi {
-            server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
-        };
+        let prefecture_master_api: PrefectureMasterApi = Default::default();
         let result = prefecture_master_api.get_blocking("富山県");
         let prefecture = result.unwrap();
         assert_eq!(prefecture.name, "富山県");
         let cities = vec![
             "富山市",
             "高岡市",
             "魚津市",
@@ -122,17 +124,15 @@
         for city in cities {
             assert!(prefecture.cities.contains(&city.to_string()));
         }
     }
 
     #[test]
     fn 同期_誤った都道府県名_失敗() {
-        let prefecture_master_api = PrefectureMasterApi {
-            server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
-        };
+        let prefecture_master_api: PrefectureMasterApi = Default::default();
         let result = prefecture_master_api.get_blocking("大阪都");
         assert!(result.is_err());
         assert_eq!(
             result.err().unwrap().error_message,
             format!(
                 "{}/大阪都/master.jsonを取得できませんでした",
                 prefecture_master_api.server_url
```

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/api.rs` & `japanese_address_parser_py-0.1.0b18/core/src/api.rs`

 * *Files 26% similar despite different names*

```diff
@@ -2,65 +2,43 @@
 pub mod prefecture_master_api;
 
 use crate::api::city_master_api::CityMasterApi;
 use crate::api::prefecture_master_api::PrefectureMasterApi;
 use crate::entity::{City, Prefecture};
 use crate::err::Error;
 
+#[derive(Default)]
 pub struct AsyncApi {
     pub prefecture_master_api: PrefectureMasterApi,
     pub city_master_api: CityMasterApi,
 }
 
 impl AsyncApi {
-    pub fn new() -> Self {
-        AsyncApi {
-            prefecture_master_api: PrefectureMasterApi {
-                server_url:
-                    "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
-            },
-            city_master_api: CityMasterApi {
-                server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
-            },
-        }
-    }
-
     pub async fn get_prefecture_master(&self, prefecture_name: &str) -> Result<Prefecture, Error> {
         self.prefecture_master_api.get(prefecture_name).await
     }
 
     pub async fn get_city_master(
         &self,
         prefecture_name: &str,
         city_name: &str,
     ) -> Result<City, Error> {
         self.city_master_api.get(prefecture_name, city_name).await
     }
 }
 
 #[cfg(feature = "blocking")]
+#[derive(Default)]
 pub struct BlockingApi {
     prefecture_master_api: PrefectureMasterApi,
     city_master_api: CityMasterApi,
 }
 
 #[cfg(feature = "blocking")]
 impl BlockingApi {
-    pub fn new() -> Self {
-        BlockingApi {
-            prefecture_master_api: PrefectureMasterApi {
-                server_url:
-                    "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
-            },
-            city_master_api: CityMasterApi {
-                server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
-            },
-        }
-    }
-
     pub fn get_prefecture_master(&self, prefecture_name: &str) -> Result<Prefecture, Error> {
         self.prefecture_master_api.get_blocking(prefecture_name)
     }
 
     pub fn get_city_master(&self, prefecture_name: &str, city_name: &str) -> Result<City, Error> {
         self.city_master_api
             .get_blocking(prefecture_name, city_name)
```

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/entity.rs` & `japanese_address_parser_py-0.1.0b18/core/src/entity.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/err.rs` & `japanese_address_parser_py-0.1.0b18/core/src/err.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/adapter/orthographical_variant_adapter.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/adapter/orthographical_variant_adapter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/adapter/vague_expression_adapter.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/adapter/vague_expression_adapter.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use nom::combinator::rest;
 use nom::error::Error;
 use nom::sequence::tuple;
 
 pub struct VagueExpressionAdapter;
 
 impl VagueExpressionAdapter {
-    pub fn apply(self, input: &str, region_name_list: &Vec<String>) -> Option<(String, String)> {
+    pub fn apply(self, input: &str, region_name_list: &[String]) -> Option<(String, String)> {
         if let Ok(highest_match) =
             SequenceMatcher::get_most_similar_match(input, region_name_list, None)
         {
             let mut parser = tuple((
                 is_not::<&str, &str, Error<&str>>("町村"),
                 is_a::<&str, &str, Error<&str>>("町村"),
                 rest,
```

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/filter/fullwidth_character.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/filter/fullwidth_character.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/filter/invalid_town_name_format.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/filter/invalid_town_name_format.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/filter/non_kanji_block_number.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/filter/non_kanji_block_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/read_city.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/read_city.rs`

 * *Files 2% similar despite different names*

```diff
@@ -58,13 +58,13 @@
     #[test_case("茨城県", "龍ヶ崎市佐貫町647", "龍ヶ崎市"; "success_龍ヶ崎市")]
     #[test_case("茨城県", "龍ケ崎市佐貫町647", "龍ヶ崎市"; "success_龍ケ崎市_表記ゆれ")]
     #[test_case("茨城県", "竜ヶ崎市佐貫町647", "龍ヶ崎市"; "success_竜ヶ崎市_表記ゆれ")]
     #[test_case("茨城県", "竜ケ崎市佐貫町647", "龍ヶ崎市"; "success_竜ケ崎市_表記ゆれ")]
     #[test_case("群馬県", "みなかみ町後閑318", "利根郡みなかみ町"; "success_利根郡みなかみ町_郡名が省略されている")]
     #[test_case("埼玉県", "東秩父村大字御堂634番地", "秩父郡東秩父村"; "success_秩父郡東秩父村_郡名が省略されている")]
     fn test_read_city(prefecture_name: &str, input: &str, expected: &str) {
-        let api = BlockingApi::new();
+        let api: BlockingApi = Default::default();
         let prefecture = api.get_prefecture_master(prefecture_name).unwrap();
         let (_, city_name) = read_city(input, prefecture).unwrap();
         assert_eq!(city_name, expected);
     }
 }
```

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/read_house_number.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/read_house_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/read_prefecture.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/read_prefecture.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser/read_town.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser/read_town.rs`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         assert_eq!(town, "薮田南二丁目");
         let (_, town) = read_town("籔田南二丁目", &city).unwrap();
         assert_eq!(town, "薮田南二丁目");
     }
 
     #[test]
     fn read_town_丁目が算用数字の場合_京都府京都市東山区n丁目() {
-        let client = BlockingApi::new();
+        let client: BlockingApi = Default::default();
         let city = client.get_city_master("京都府", "京都市東山区").unwrap();
         let test_cases = vec![
             ("本町1丁目45番", "本町一丁目"),
             ("本町2丁目64番", "本町二丁目"),
             ("本町10丁目169番", "本町十丁目"),
             ("本町12丁目224番", "本町十二丁目"),
             ("本町20丁目435番", "本町二十丁目"),
@@ -167,15 +167,15 @@
             let (_, town) = read_town(input, &city).unwrap();
             assert_eq!(town, town_name);
         }
     }
 
     #[test]
     fn read_town_大字の省略_東京都西多摩郡日の出町大字平井() {
-        let blocking_api = BlockingApi::new();
+        let blocking_api: BlockingApi = Default::default();
         let city = blocking_api
             .get_city_master("東京都", "西多摩郡日の出町")
             .unwrap();
 
         let (rest, town) = read_town("大字平井2780番地", &city).unwrap();
         assert_eq!(town, "大字平井");
         assert_eq!(rest, "2780番地");
```

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/parser.rs` & `japanese_address_parser_py-0.1.0b18/core/src/parser.rs`

 * *Files 12% similar despite different names*

```diff
@@ -19,43 +19,44 @@
 /// An asynchronous `Parser` to process addresses.
 ///
 /// # Example
 /// ```
 /// use japanese_address_parser::parser::Parser;
 ///
 /// async fn example() {
-///     let parser = Parser::new();
+///     let parser : Parser = Default::default();
 ///     let result = parser.parse("東京都新宿区西新宿2-8-1").await;
 ///     println!("{:?}", result);
 /// }
 /// ```
 pub struct Parser {
     async_api: Arc<AsyncApi>,
     #[cfg(feature = "blocking")]
     blocking_api: Arc<BlockingApi>,
 }
 
-impl Parser {
+impl Default for Parser {
     /// Constructs a new `Parser`.
     #[cfg(feature = "blocking")]
-    pub fn new() -> Self {
-        Parser {
-            async_api: Arc::new(AsyncApi::new()),
-            blocking_api: Arc::new(BlockingApi::new()),
+    fn default() -> Self {
+        Self {
+            async_api: Arc::new(Default::default()),
+            blocking_api: Arc::new(Default::default()),
         }
     }
-
     /// Constructs a new `Parser`.
     #[cfg(not(feature = "blocking"))]
-    pub fn new() -> Self {
-        Parser {
-            async_api: Arc::new(AsyncApi::new()),
+    fn default() -> Self {
+        Self {
+            async_api: Arc::new(Default::default()),
         }
     }
+}
 
+impl Parser {
     /// Parses the given `address` asynchronously.
     pub async fn parse(&self, address: &str) -> ParseResult {
         parse(self.async_api.clone(), address).await
     }
 
     /// Parses the given `address` synchronously.
     #[cfg(feature = "blocking")]
@@ -129,75 +130,75 @@
     use crate::api::AsyncApi;
     use crate::err::ParseErrorKind;
     use crate::parser::parse;
     use wasm_bindgen_test::{wasm_bindgen_test, wasm_bindgen_test_configure};
 
     #[tokio::test]
     async fn 都道府県名が誤っている場合() {
-        let api = AsyncApi::new();
+        let api: AsyncApi = Default::default();
         let result = parse(api.into(), "青盛県青森市長島１丁目１−１").await;
         assert_eq!(result.address.prefecture, "");
         assert_eq!(result.address.city, "");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "青盛県青森市長島１丁目１−１");
         assert_eq!(result.error.is_some(), true);
         assert_eq!(
             result.error.unwrap().error_message,
             ParseErrorKind::Prefecture.to_string()
         );
     }
 
     #[tokio::test]
     async fn 都道府県マスタが取得できない場合() {
-        let mut api = AsyncApi::new();
+        let mut api: AsyncApi = Default::default();
         api.prefecture_master_api = PrefectureMasterApi {
             server_url: "https://example.com/invalid_url/api/",
         };
 
         let result = parse(api.into(), "青森県青森市長島１丁目１−１").await;
         assert_eq!(result.error.is_some(), true);
         assert_eq!(result.address.prefecture, "青森県");
         assert_eq!(result.address.city, "");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "青森市長島１丁目１−１");
     }
 
     #[tokio::test]
     async fn 市区町村名が誤っている場合() {
-        let api = AsyncApi::new();
+        let api: AsyncApi = Default::default();
         let result = parse(api.into(), "青森県青盛市長島１丁目１−１").await;
         assert_eq!(result.address.prefecture, "青森県");
         assert_eq!(result.address.city, "");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "青盛市長島１丁目１−１");
         assert_eq!(result.error.is_some(), true);
         assert_eq!(
             result.error.unwrap().error_message,
             ParseErrorKind::City.to_string()
         );
     }
 
     #[tokio::test]
     async fn 市区町村マスタが取得できない場合() {
-        let mut api = AsyncApi::new();
+        let mut api: AsyncApi = Default::default();
         api.city_master_api = CityMasterApi {
             server_url: "https://example.com/invalid_url/api/",
         };
 
         let result = parse(api.into(), "青森県青森市長島１丁目１−１").await;
         assert_eq!(result.error.is_some(), true);
         assert_eq!(result.address.prefecture, "青森県");
         assert_eq!(result.address.city, "青森市");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "長島１丁目１−１");
     }
 
     #[tokio::test]
     async fn 町名が誤っている場合() {
-        let api = AsyncApi::new();
+        let api: AsyncApi = Default::default();
         let result = parse(api.into(), "青森県青森市永嶋１丁目１−１").await;
         assert_eq!(result.address.prefecture, "青森県");
         assert_eq!(result.address.city, "青森市");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "永嶋１丁目１−１");
         assert_eq!(result.error.is_some(), true);
         assert_eq!(
@@ -206,15 +207,15 @@
         );
     }
 
     wasm_bindgen_test_configure!(run_in_browser);
 
     #[wasm_bindgen_test]
     async fn parse_wasm_success() {
-        let api = AsyncApi::new();
+        let api: AsyncApi = Default::default();
         let result = parse(api.into(), "兵庫県淡路市生穂新島8番地").await;
         assert_eq!(result.address.prefecture, "兵庫県".to_string());
         assert_eq!(result.address.city, "淡路市".to_string());
         assert_eq!(result.address.town, "生穂".to_string());
         assert_eq!(result.address.rest, "新島8番地".to_string());
         assert_eq!(result.error, None);
     }
@@ -281,26 +282,26 @@
 mod blocking_tests {
     use crate::api::BlockingApi;
     use crate::err::ParseErrorKind;
     use crate::parser::parse_blocking;
 
     #[test]
     fn parse_blocking_success_埼玉県秩父市熊木町8番15号() {
-        let client = BlockingApi::new();
+        let client: BlockingApi = Default::default();
         let result = parse_blocking(client.into(), "埼玉県秩父市熊木町8番15号");
         assert_eq!(result.address.prefecture, "埼玉県");
         assert_eq!(result.address.city, "秩父市");
         assert_eq!(result.address.town, "熊木町");
         assert_eq!(result.address.rest, "8番15号");
         assert_eq!(result.error, None);
     }
 
     #[test]
     fn parse_blocking_fail_市町村名が間違っている場合() {
-        let client = BlockingApi::new();
+        let client: BlockingApi = Default::default();
         let result = parse_blocking(client.into(), "埼玉県秩父柿熊木町8番15号");
         assert_eq!(result.address.prefecture, "埼玉県");
         assert_eq!(result.address.city, "");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "秩父柿熊木町8番15号");
         assert_eq!(
             result.error.unwrap().error_message,
```

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/util/converter.rs` & `japanese_address_parser_py-0.1.0b18/core/src/util/converter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/core/src/util/sequence_matcher.rs` & `japanese_address_parser_py-0.1.0b18/core/src/util/sequence_matcher.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/README.md` & `japanese_address_parser_py-0.1.0b18/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 ### Async Version
 
 ```rust
 use japanese_address_parser::parser::Parser;
 
 #[tokio::main]
 async fn main() {
-    let parser = Parser::new();
+    let parser: Parser = Default::default();
     let parse_result = parser.parse("東京都千代田区丸の内1-1-1").await;
     println!("{:?}", parse_result);
 }
 ```
 
 ### Blocking Version
 
 ```rust
 use japanese_address_parser::parser::Parser;
 
 fn main() {
-    let parser = Parser::new();
+    let parser: Parser = Default::default();
     let parse_result = parser.parse_blocking("東京都千代田区丸の内1-1-1"); // `parse_blocking()` is available on `blocking` feature only
     println!("{:?}", parse_result);
 }
 ```
 
 ## Wasm support
```

### Comparing `japanese_address_parser_py-0.1.0b17/python/README.md` & `japanese_address_parser_py-0.1.0b18/python/README.md`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/python/japanese_address_parser_py.pyi` & `japanese_address_parser_py-0.1.0b18/python/japanese_address_parser_py.pyi`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b17/python/src/lib.rs` & `japanese_address_parser_py-0.1.0b18/python/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -35,26 +35,26 @@
 }
 
 #[pymethods]
 impl PyParser {
     #[new]
     fn default() -> Self {
         PyParser {
-            parser: Parser::new(),
+            parser: Default::default(),
         }
     }
 
     fn parse(&self, address: &str) -> PyParseResult {
         self.parser.parse_blocking(address).into()
     }
 }
 
 #[pyfunction]
 fn parse(address: &str) -> PyParseResult {
-    let parser = Parser::new();
+    let parser: Parser = Default::default();
     parser.parse_blocking(address).into()
 }
 
 #[pymodule]
 #[pyo3(name = "japanese_address_parser_py")]
 fn python_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyParseResult>()?;
```

### Comparing `japanese_address_parser_py-0.1.0b17/Cargo.lock` & `japanese_address_parser_py-0.1.0b18/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -45,17 +45,17 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.22.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
@@ -69,17 +69,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -345,15 +345,15 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "japanese-address-parser"
-version = "0.1.0-beta.17"
+version = "0.1.0-beta.18"
 dependencies = [
  "itertools",
  "js-sys",
  "nom",
  "rapidfuzz",
  "regex",
  "reqwest",
@@ -370,17 +370,17 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
@@ -613,15 +613,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python"
-version = "0.1.0-beta.17"
+version = "0.1.0-beta.18"
 dependencies = [
  "japanese-address-parser",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -796,17 +796,17 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.6.5"
@@ -816,17 +816,17 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -865,17 +865,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
@@ -943,15 +943,15 @@
  "quote",
  "syn",
  "test-case-core",
 ]
 
 [[package]]
 name = "tests"
-version = "0.1.0-beta.17"
+version = "0.1.0-beta.18"
 dependencies = [
  "csv",
  "japanese-address-parser",
  "serde",
  "tokio",
 ]
 
@@ -1120,15 +1120,15 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm"
-version = "0.1.0-beta.17"
+version = "0.1.0-beta.18"
 dependencies = [
  "console_error_panic_hook",
  "japanese-address-parser",
  "serde-wasm-bindgen",
  "wasm-bindgen",
  "wasm-bindgen-futures",
 ]
```

### Comparing `japanese_address_parser_py-0.1.0b17/PKG-INFO` & `japanese_address_parser_py-0.1.0b18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: japanese-address-parser-py
-Version: 0.1.0b17
+Version: 0.1.0b18
 Classifier: Topic :: Text Processing
 Classifier: Programming Language :: Rust
 Classifier: Typing :: Typed
 Summary: A Rust Library to parse japanese addresses.
 Keywords: converter,utility,geo,rust
 Author: Yuuki Toriyama <github@toriyama.dev>
 Author-email: Yuuki Toriyama <github@toriyama.dev>
```

