# Comparing `tmp/cameo_geo_query-1.0.7.tar.gz` & `tmp/cameo_geo_query-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cameo_geo_query-1.0.7.tar", last modified: Thu Feb 15 01:51:46 2024, max compression
+gzip compressed data, was "cameo_geo_query-1.0.8.tar", last modified: Wed Mar 27 12:04:21 2024, max compression
```

## Comparing `cameo_geo_query-1.0.7.tar` & `cameo_geo_query-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-02-15 01:51:46.678071 cameo_geo_query-1.0.7/
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-02-15 01:51:46.676536 cameo_geo_query-1.0.7/Cameo_geo_query.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)      212 2024-02-15 01:51:46.000000 cameo_geo_query-1.0.7/Cameo_geo_query.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      469 2024-02-15 01:51:46.000000 cameo_geo_query-1.0.7/Cameo_geo_query.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2024-02-15 01:51:46.000000 cameo_geo_query-1.0.7/Cameo_geo_query.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       20 2024-02-15 01:51:46.000000 cameo_geo_query-1.0.7/Cameo_geo_query.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)       16 2024-02-15 01:51:46.000000 cameo_geo_query-1.0.7/Cameo_geo_query.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)      212 2024-02-15 01:51:46.677718 cameo_geo_query-1.0.7/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)       17 2023-10-24 01:32:25.000000 cameo_geo_query-1.0.7/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-02-15 01:51:46.677119 cameo_geo_query-1.0.7/cameo_geo_query/
--rw-r--r--   0 apple      (501) staff       (20)      106 2024-02-15 01:51:22.000000 cameo_geo_query-1.0.7/cameo_geo_query/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     8477 2024-02-15 01:35:36.000000 cameo_geo_query-1.0.7/cameo_geo_query/cameo_geo_query.py
--rw-r--r--   0 apple      (501) staff       (20)       38 2024-02-15 01:51:46.678165 cameo_geo_query-1.0.7/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      357 2024-02-15 01:51:43.000000 cameo_geo_query-1.0.7/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-03-27 12:04:21.749194 cameo_geo_query-1.0.8/
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-03-27 12:04:21.747905 cameo_geo_query-1.0.8/Cameo_geo_query.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)      212 2024-03-27 12:04:21.000000 cameo_geo_query-1.0.8/Cameo_geo_query.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      469 2024-03-27 12:04:21.000000 cameo_geo_query-1.0.8/Cameo_geo_query.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-03-27 12:04:21.000000 cameo_geo_query-1.0.8/Cameo_geo_query.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       20 2024-03-27 12:04:21.000000 cameo_geo_query-1.0.8/Cameo_geo_query.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)       16 2024-03-27 12:04:21.000000 cameo_geo_query-1.0.8/Cameo_geo_query.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)      212 2024-03-27 12:04:21.748946 cameo_geo_query-1.0.8/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)       17 2023-10-24 01:32:25.000000 cameo_geo_query-1.0.8/README.md
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-03-27 12:04:21.748396 cameo_geo_query-1.0.8/cameo_geo_query/
+-rw-r--r--   0 apple      (501) staff       (20)      106 2024-02-15 01:54:04.000000 cameo_geo_query-1.0.8/cameo_geo_query/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     9866 2024-03-27 12:01:59.000000 cameo_geo_query-1.0.8/cameo_geo_query/cameo_geo_query.py
+-rw-r--r--   0 apple      (501) staff       (20)       38 2024-03-27 12:04:21.749281 cameo_geo_query-1.0.8/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      357 2024-03-27 12:04:08.000000 cameo_geo_query-1.0.8/setup.py
```

### Comparing `cameo_geo_query-1.0.7/cameo_geo_query/cameo_geo_query.py` & `cameo_geo_query-1.0.8/cameo_geo_query/cameo_geo_query.py`

 * *Files 16% similar despite different names*

```diff
@@ -135,39 +135,74 @@
                             size_max=15, color_continuous_scale=custom_color_scale)
 
     fig.update_layout(mapbox_style='open-street-map')  # carto-positron
 
     initial_center = {"lat": lat, "lon": lon}  # Example coordinates
     initial_zoom = 14  # Example zoom level
     fig.update_layout(mapbox_center=initial_center, mapbox_zoom=initial_zoom)
-
     fig.update_layout(margin={'r': 0, 't': 0, 'l': 0, 'b': 0})
-
-
     # Save to html
     fig.write_html(file_path, include_plotlyjs=True)
 
     return file_path
 
+def clean_data(data_dict, start_time, end_time):
+    # 這裡確保傳入的是字典中的資料列表
+    data_list = data_dict['data']
+
+    # 過濾資料
+    cleaned_data_list = [item for item in data_list if
+                         start_time <= datetime.strptime(item['time'], "%Y-%m-%d %H:%M:%S") <= end_time]
+    # 更新字典
+    cleaned_data_dict = {
+        'count': len(cleaned_data_list),
+        'data': cleaned_data_list
+    }
+
+    return cleaned_data_dict
+
 def get_cwb_wind_data(int_lat, int_lon, str_datetime):
     event_loc = (int_lat, int_lon)
     event_time = datetime.strptime(str_datetime, "%Y-%m-%d %H:%M:%S")
 
+    # 建立一個特定時間點用於判斷
+    time_threshold = datetime.strptime("2023-11-15 13:00:00", "%Y-%m-%d %H:%M:%S")
+
+    time_clean_start_threshold = datetime.strptime("2023-11-15 00:00:00", "%Y-%m-%d %H:%M:%S")
+    time_clean_end_threshold = datetime.strptime("2023-11-16 00:00:00", "%Y-%m-%d %H:%M:%S")
+
     t = (event_time + timedelta(minutes=-event_time.minute, seconds=-event_time.second))
     str_result = "無氣象局測站資料"
     for _ in range(3):
-        start_time, end_time = t.strftime("%Y-%m-%d %H:%M:%S"), (t + timedelta(hours=1)).strftime("%Y-%m-%d %H:%M:%S")
+        start_time, end_time = t, (t + timedelta(hours=1))
+        print('start_time', start_time)
+
+        # 如果 start_time 或 end_time 大於設定的時間點，則減少 8 小時
+        if start_time > time_threshold and end_time > time_threshold:
+            start_time -= timedelta(hours=8)
+            end_time -= timedelta(hours=8)
+
+        formatted_start_time = start_time.strftime("%Y-%m-%d %H:%M:%S")
+        formatted_end_time = end_time.strftime("%Y-%m-%d %H:%M:%S")
+
         t = t - timedelta(hours=1)
-        cwb_api = f'https://aiot.moenv.gov.tw/_/api/v2/epa_station/wind?fields=wind_direct%2Cwind_speed&sources=中央氣象局&min_lat=-90&max_lat=90&min_lon=-180&max_lon=180&start_time={start_time}&end_time={end_time}'
+        cwb_api = f'https://aiot.moenv.gov.tw/_/api/v2/epa_station/wind?fields=wind_direct%2Cwind_speed&sources=中央氣象局&min_lat=-90&max_lat=90&min_lon=-180&max_lon=180&start_time={formatted_start_time}&end_time={formatted_end_time}'
         response = requests.get(cwb_api)
         j = response.json()
+
+        try:
+            if event_time > time_clean_start_threshold and event_time < time_clean_end_threshold:
+                j = clean_data(j, t, (t + timedelta(hours=2)))
+        except:
+            pass
+
         if len(j['data']) != 0:
             nearest_site, nearest_dist = None, None
             for i in range(len(j['data'])):
-                site_loc = (j['data'][i]['lat'],j['data'][i]['lon'])
+                site_loc = (j['data'][i]['lat'], j['data'][i]['lon'])
                 dist = geodesic(event_loc, site_loc).km
                 if nearest_dist is None or dist < nearest_dist:
                     nearest_site, nearest_dist = j['data'][i], dist
             str_result = f"以下為距離最近的氣象局測站資料:\n測站: {nearest_site['name']}(距離{nearest_dist:.2f}公里)\n資料時間: {nearest_site['time']}\n風向: {nearest_site['wind_direct']}\n風速: {nearest_site['wind_speed']}"
             break
         else:
             continue
@@ -180,15 +215,15 @@
     lat = 25.0669
     df_deviceid_file_path = '/Users/apple/Desktop/project_device_table_20231017.csv'
     result_lst_device_id = calculate_distance(lat, lon, df_deviceid_file_path, 1)
     print(result_lst_device_id)
     
     # Example of filter_data_for_device_time usage:
     df_device_file_path = '/Users/apple/Desktop/iot_data'
-    time = '2023-11-03 08:35:00'
+    time = '2023-11-15 08:35:00'
     df = filter_data_for_device(result_lst_device_id, time,df_device_file_path)
     print(df.localTime.min())
     print(df.localTime.max())
     print(df.columns)
     
     file_path = '/Users/apple/Desktop/test.html'
     url = create_pm25_map(df,lat, lon, file_path, row_value='value', row_deviceId='deviceId', row_lat='lat', row_lon='lon', row_time='localTime')
```

