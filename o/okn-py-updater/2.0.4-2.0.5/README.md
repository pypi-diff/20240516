# Comparing `tmp/okn_py_updater-2.0.4.tar.gz` & `tmp/okn_py_updater-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okn_py_updater-2.0.4.tar", last modified: Wed May 15 09:25:18 2024, max compression
+gzip compressed data, was "okn_py_updater-2.0.5.tar", last modified: Wed May 15 21:44:48 2024, max compression
```

## Comparing `okn_py_updater-2.0.4.tar` & `okn_py_updater-2.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:25:18.032984 okn_py_updater-2.0.4/
--rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.4/LICENSE
--rw-rw-rw-   0        0        0     3706 2024-05-15 09:25:18.032984 okn_py_updater-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.4/README.md
--rw-rw-rw-   0        0        0      657 2024-05-15 03:12:37.000000 okn_py_updater-2.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 09:25:18.032984 okn_py_updater-2.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 09:25:18.010870 okn_py_updater-2.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 09:25:18.014183 okn_py_updater-2.0.4/src/okn_py_updater/
--rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.4/src/okn_py_updater/__init__.py
--rw-rw-rw-   0        0        0    24885 2024-05-15 09:24:08.000000 okn_py_updater-2.0.4/src/okn_py_updater/okn_py_updater.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:25:18.031987 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/
--rw-rw-rw-   0        0        0     3706 2024-05-15 09:25:17.000000 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-15 09:25:17.000000 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:25:17.000000 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 09:25:17.000000 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 21:44:48.026495 okn_py_updater-2.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3706 2024-05-15 21:44:48.025499 okn_py_updater-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.5/README.md
+-rw-rw-rw-   0        0        0      657 2024-05-15 21:43:24.000000 okn_py_updater-2.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 21:44:48.026495 okn_py_updater-2.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 21:44:47.998412 okn_py_updater-2.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 21:44:48.008542 okn_py_updater-2.0.5/src/okn_py_updater/
+-rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.5/src/okn_py_updater/__init__.py
+-rw-rw-rw-   0        0        0    25479 2024-05-15 21:43:24.000000 okn_py_updater-2.0.5/src/okn_py_updater/okn_py_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:44:48.024501 okn_py_updater-2.0.5/src/okn_py_updater.egg-info/
+-rw-rw-rw-   0        0        0     3706 2024-05-15 21:44:47.000000 okn_py_updater-2.0.5/src/okn_py_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-15 21:44:47.000000 okn_py_updater-2.0.5/src/okn_py_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 21:44:47.000000 okn_py_updater-2.0.5/src/okn_py_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 21:44:47.000000 okn_py_updater-2.0.5/src/okn_py_updater.egg-info/top_level.txt
```

### Comparing `okn_py_updater-2.0.4/LICENSE` & `okn_py_updater-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.4/PKG-INFO` & `okn_py_updater-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `okn_py_updater-2.0.4/README.md` & `okn_py_updater-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.4/pyproject.toml` & `okn_py_updater-2.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "okn_py_updater"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for OKN Data Updater"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `okn_py_updater-2.0.4/src/okn_py_updater/okn_py_updater.py` & `okn_py_updater-2.0.5/src/okn_py_updater/okn_py_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,37 +130,38 @@
         t = data_dict_input[related_column_name_array[0]]
         output_column = filter_config_info["output"]
         # o = data_dict_input[output_column]
         # data_dict_input[output_column] = live_gradient(f, t, o)
         if len(f) >= n_value + 2:
             if "updated_x" in related_column_name_array[1]:
                 f0 = pre_x_nom
-                t0 = pre_time
-                t0 = t[1]
-                f2 = statistics.median(f[1:n_value + 1])
-                # t2 = t[1]
-                t2 = t[3]
+                # t0 = pre_time
+                start_index = int((n_value - 3) / 2)
+                end_index = start_index + 2
+                t0 = t[start_index]
+                n_array = f[1:n_value + 1]
+                f2 = statistics.median(n_array)
+                t2 = t[end_index]
                 out_array = data_dict_input[output_column]
                 out_array[0] = (f2 - f0) / (t2 - t0)
+                # out_array[0] = (f2 - f0) / (t[1] - pre_time)
                 data_dict_input[output_column] = out_array
             elif "updated_y" in related_column_name_array[1]:
                 f0 = pre_y_nom
-                t0 = pre_time
-                t0 = t[1]
-                f2 = statistics.median(f[1:n_value + 1])
-                t2 = t[1]
-                t2 = t[3]
+                start_index = int((n_value - 3) / 2)
+                end_index = start_index + 2
+                t0 = t[start_index]
+                n_array = f[1:n_value + 1]
+                f2 = statistics.median(n_array)
+                t2 = t[end_index]
                 out_array = data_dict_input[output_column]
                 out_array[0] = (f2 - f0) / (t2 - t0)
                 data_dict_input[output_column] = out_array
             else:
                 pass
-                # # Not tested in live updater
-        # print(grad(f, t))
-
     else:
         print(f"Function:{match_item} is not found")
 
     return data_dict_input
 
 
 # def spike_remover(f):
@@ -282,30 +283,30 @@
 
 def dshift(f):
     y = np.nanmean(f)
     f1 = f - y
     return f1
 
 
-def grad(f, t):
-    try:
-        df = np.gradient(f)
-        dt = np.gradient(t)
-        dfdt = df / dt
-        # print("dfdt", dfdt)
-        for ind, value in enumerate(dfdt):
-            if math.isinf(value):
-                dfdt[ind] = 0
-            if np.isnan(value):
-                dfdt[ind] = 0
-        return dfdt
-    except ValueError:
-        return 0
-    except RuntimeWarning:
-        return 0
+# def grad(f, t):
+#     try:
+#         df = np.gradient(f)
+#         dt = np.gradient(t)
+#         dfdt = df / dt
+#         # print("dfdt", dfdt)
+#         for ind, value in enumerate(dfdt):
+#             if math.isinf(value):
+#                 dfdt[ind] = 0
+#             if np.isnan(value):
+#                 dfdt[ind] = 0
+#         return dfdt
+#     except ValueError:
+#         return 0
+#     except RuntimeWarning:
+#         return 0
 
 
 # def live_gradient(f, t, out_array):
 #     # print("live grad")
 #     # print(f)
 #     # print(t)
 #     # print(out_array)
@@ -328,53 +329,53 @@
 #             out_array[mid_index] = dfdt
 #             # print("Grad", out_array)
 #             return out_array
 #     else:
 #         raise ValueError("Displacement and time array lengths must be the same.")
 
 
-def live_gradient(f, t):
-    f_length = len(f)
-    t_length = len(t)
-    if f_length == t_length:
-        if f_length > 0:
-            data_info_array = []
-            for pos, time in zip(f, t):
-                temp_dict = {}
-                temp_dict["position"] = float(pos)
-                temp_dict["time"] = float(time)
-                data_info_array.append(temp_dict)
-            info_array_length = len(data_info_array)
-            if info_array_length > 2:
-                return_array = []
-                for ind in range(info_array_length):
-                    if ind == 0:
-                        return_array.append(0)
-                    elif ind == 1:
-                        edge_grad_val = grad_by_edge_equation(data_info_array[0],
-                                                              data_info_array[1])
-                        return_array.append(edge_grad_val)
-                    else:
-                        interior_grad_val = grad_by_interior_equation(data_info_array[ind - 2],
-                                                                      data_info_array[ind - 1],
-                                                                      data_info_array[ind])
-                        return_array.append(interior_grad_val)
-                return return_array
-            else:
-                if info_array_length == 2:
-                    edge_grad_val = grad_by_edge_equation(data_info_array[0],
-                                                          data_info_array[1])
-                    return [0, edge_grad_val]
-                else:
-                    if info_array_length == 1:
-                        return [0]
-                    else:
-                        pass
-    else:
-        raise ValueError("Displacement and time array lengths must be the same.")
+# def live_gradient(f, t):
+#     f_length = len(f)
+#     t_length = len(t)
+#     if f_length == t_length:
+#         if f_length > 0:
+#             data_info_array = []
+#             for pos, time in zip(f, t):
+#                 temp_dict = {}
+#                 temp_dict["position"] = float(pos)
+#                 temp_dict["time"] = float(time)
+#                 data_info_array.append(temp_dict)
+#             info_array_length = len(data_info_array)
+#             if info_array_length > 2:
+#                 return_array = []
+#                 for ind in range(info_array_length):
+#                     if ind == 0:
+#                         return_array.append(0)
+#                     elif ind == 1:
+#                         edge_grad_val = grad_by_edge_equation(data_info_array[0],
+#                                                               data_info_array[1])
+#                         return_array.append(edge_grad_val)
+#                     else:
+#                         interior_grad_val = grad_by_interior_equation(data_info_array[ind - 2],
+#                                                                       data_info_array[ind - 1],
+#                                                                       data_info_array[ind])
+#                         return_array.append(interior_grad_val)
+#                 return return_array
+#             else:
+#                 if info_array_length == 2:
+#                     edge_grad_val = grad_by_edge_equation(data_info_array[0],
+#                                                           data_info_array[1])
+#                     return [0, edge_grad_val]
+#                 else:
+#                     if info_array_length == 1:
+#                         return [0]
+#                     else:
+#                         pass
+#     else:
+#         raise ValueError("Displacement and time array lengths must be the same.")
 
 
 def grad_by_edge_equation(first_ele, second_ele):
     displacement = second_ele["position"] - first_ele["position"]
     time_diff = second_ele["time"] - first_ele["time"]
     return displacement / time_diff
 
@@ -408,28 +409,24 @@
     #         idx = ~shifted_array.mask * input_array.mask
     #         input_array[idx] = shifted_array[idx]
     return input_array
 
 
 def get_out_header_array(header_array_input, filter_config_input):
     data_id_array = ["id"]
-    print(data_id_array)
     output_header_array = [header for header in header_array_input]
-    print(output_header_array)
     output_header_array = data_id_array + output_header_array
-    print(output_header_array)
     for filter_info in filter_config_input:
         if filter_info["Enabled"]:
             try:
                 output_header = filter_info["output"]
             except KeyError:
                 output_header = None
             if output_header is not None:
                 if output_header not in output_header_array:
-                    print(output_header)
                     output_header_array.append(output_header)
 
     return output_header_array
 
 
 class Updater:
     def __init__(self, config, circular_buffer_length, header_array, drop_rate=0):
@@ -514,35 +511,34 @@
             converting_array = []
             for index in range(len(data_dict[self.out_header_array[0]])):
                 temp_dict = {}
                 for header in self.out_header_array:
                     temp_dict[header] = (data_dict[header][index])
                 converting_array.append(temp_dict)
 
-            # print("C before")
-            # for d in self.circular_buffer:
-            #     print(d)
-            # print("C before")
             for d_dict in self.circular_buffer:
                 d_id = d_dict["id"]
                 for con_dict in converting_array:
                     con_id = con_dict["id"]
                     if d_id == con_id:
                         for att in d_dict:
                             d_dict[att] = con_dict[att]
                         break
-            # print("C After")
-            # for d in self.circular_buffer:
-            #     print(d)
-            # print("C After")
 
             first_data = self.circular_buffer[0]
             self.pre_x_nom = first_data["updated_x_nom"]
             self.pre_y_nom = first_data["updated_y_nom"]
             self.pre_time = first_data["record_timestamp"]
+            n_data_index = int((self.n_value - 3) / 2) + 1
+            n_related_data = self.circular_buffer[n_data_index]
+            first_data["x_nom"] = n_related_data["x_nom"]
+            first_data["y_nom"] = n_related_data["y_nom"]
+            first_data["record_timestamp"] = n_related_data["record_timestamp"]
+            first_data["sensor_timestamp"] = n_related_data["sensor_timestamp"]
+            first_data["direction"] = n_related_data["direction"]
             out_array = []
             for header in self.out_header_array:
                 out_array.append(first_data[header])
             return out_array
         else:
             if self.count == 0:
                 data_input.insert(0, self.data_id)
@@ -575,37 +571,36 @@
                 converting_array = []
                 for index in range(len(data_dict[self.out_header_array[0]])):
                     temp_dict = {}
                     for header in self.out_header_array:
                         temp_dict[header] = (data_dict[header][index])
                     converting_array.append(temp_dict)
 
-                # print("C before")
-                # for d in self.circular_buffer:
-                #     print(d)
-                # print("C before")
                 for d_dict in self.circular_buffer:
                     d_id = d_dict["id"]
                     for con_dict in converting_array:
                         con_id = con_dict["id"]
                         if d_id == con_id:
                             for att in d_dict:
                                 d_dict[att] = con_dict[att]
                             break
-                # print("C After")
-                # for d in self.circular_buffer:
-                #     print(d)
-                # print("C After")
 
                 self.count = 1
                 if len(self.circular_buffer) == self.buffer_max_length:
                     first_data = self.circular_buffer[0]
                     self.pre_x_nom = first_data["updated_x_nom"]
                     self.pre_y_nom = first_data["updated_y_nom"]
                     self.pre_time = first_data["record_timestamp"]
+                    n_data_index = int((self.n_value - 3) / 2) + 1
+                    n_related_data = self.circular_buffer[n_data_index]
+                    first_data["x_nom"] = n_related_data["x_nom"]
+                    first_data["y_nom"] = n_related_data["y_nom"]
+                    first_data["record_timestamp"] = n_related_data["record_timestamp"]
+                    first_data["sensor_timestamp"] = n_related_data["sensor_timestamp"]
+                    first_data["direction"] = n_related_data["direction"]
                     out_array = []
                     for header in self.out_header_array:
                         out_array.append(first_data[header])
                     return out_array
                 else:
                     return None
             else:
```

### Comparing `okn_py_updater-2.0.4/src/okn_py_updater.egg-info/PKG-INFO` & `okn_py_updater-2.0.5/src/okn_py_updater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

