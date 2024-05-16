# Comparing `tmp/synapse_selector-0.2.8.tar.gz` & `tmp/synapse_selector-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapse_selector-0.2.8.tar", max compression
+gzip compressed data, was "synapse_selector-0.2.9.tar", max compression
```

## Comparing `synapse_selector-0.2.8.tar` & `synapse_selector-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/LICENSE
--rw-r--r--   0        0        0     7467 2024-02-21 10:35:33.314369 synapse_selector-0.2.8/README.md
--rw-r--r--   0        0        0      723 2024-02-21 10:31:31.432675 synapse_selector-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/__init__.py
--rw-r--r--   0        0        0      245 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/add.svg
--rw-r--r--   0        0        0      272 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/back.svg
--rw-r--r--   0        0        0      416 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/home.svg
--rw-r--r--   0        0        0      296 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/keep.svg
--rw-r--r--   0        0        0      626 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/open.svg
--rw-r--r--   0        0        0      359 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/peak.svg
--rw-r--r--   0        0        0      646 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/save.svg
--rw-r--r--   0        0        0     1531 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/settings.svg
--rw-r--r--   0        0        0      540 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/assets/trash.svg
--rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/detection/__init__.py
--rw-r--r--   0        0        0      982 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/detection/model_wraper.py
--rw-r--r--   0        0        0     4914 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/detection/model_zoo.py
--rw-r--r--   0        0        0      888 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/detection/peak_detection.py
--rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/gui/__init__.py
--rw-r--r--   0        0        0     6968 2024-01-19 10:47:06.106996 synapse_selector-0.2.8/synapse_selector/gui/add_window.py
--rw-r--r--   0        0        0    22929 2024-02-21 10:51:49.627236 synapse_selector-0.2.8/synapse_selector/gui/gui.py
--rw-r--r--   0        0        0    22917 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/gui/settingswindow.py
--rw-r--r--   0        0        0      957 2024-02-21 10:14:31.732920 synapse_selector-0.2.8/synapse_selector/main.py
--rw-r--r--   0        0        0      892 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/settings/default_settings.json
--rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/utils/__init__.py
--rw-r--r--   0        0        0     2707 2024-02-21 09:59:58.655504 synapse_selector-0.2.8/synapse_selector/utils/configuration.py
--rw-r--r--   0        0        0     5939 2024-02-21 10:25:02.551977 synapse_selector-0.2.8/synapse_selector/utils/export.py
--rw-r--r--   0        0        0      318 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/utils/hash.py
--rw-r--r--   0        0        0     1523 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/utils/normalization.py
--rw-r--r--   0        0        0     3746 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/utils/plot.py
--rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/utils/post_selection/__init__.py
--rw-r--r--   0        0        0      658 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/utils/post_selection/decay_compute.py
--rw-r--r--   0        0        0      712 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/utils/post_selection/failure_rate.py
--rw-r--r--   0        0        0      624 2024-01-19 10:29:46.578545 synapse_selector-0.2.8/synapse_selector/utils/threshold.py
--rw-r--r--   0        0        0    12627 2024-02-21 10:53:30.747468 synapse_selector-0.2.8/synapse_selector/utils/trace_data.py
--rw-r--r--   0        0        0     8278 1970-01-01 00:00:00.000000 synapse_selector-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/LICENSE
+-rw-r--r--   0        0        0     7437 2024-03-06 13:43:36.903180 synapse_selector-0.2.9/README.md
+-rw-r--r--   0        0        0      723 2024-03-06 14:41:48.562765 synapse_selector-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/__init__.py
+-rw-r--r--   0        0        0      245 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/add.svg
+-rw-r--r--   0        0        0      272 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/back.svg
+-rw-r--r--   0        0        0      416 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/home.svg
+-rw-r--r--   0        0        0      296 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/keep.svg
+-rw-r--r--   0        0        0      626 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/open.svg
+-rw-r--r--   0        0        0      359 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/peak.svg
+-rw-r--r--   0        0        0      646 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/save.svg
+-rw-r--r--   0        0        0     1531 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/settings.svg
+-rw-r--r--   0        0        0      540 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/assets/trash.svg
+-rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/detection/__init__.py
+-rw-r--r--   0        0        0      982 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/detection/model_wraper.py
+-rw-r--r--   0        0        0     4914 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/detection/model_zoo.py
+-rw-r--r--   0        0        0      888 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/detection/peak_detection.py
+-rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/gui/__init__.py
+-rw-r--r--   0        0        0     6910 2024-03-06 13:43:36.906513 synapse_selector-0.2.9/synapse_selector/gui/add_window.py
+-rw-r--r--   0        0        0    24028 2024-03-06 14:38:01.657333 synapse_selector-0.2.9/synapse_selector/gui/gui.py
+-rw-r--r--   0        0        0    25976 2024-03-06 14:16:56.734317 synapse_selector-0.2.9/synapse_selector/gui/settingswindow.py
+-rw-r--r--   0        0        0      957 2024-02-21 10:14:31.732920 synapse_selector-0.2.9/synapse_selector/main.py
+-rw-r--r--   0        0        0     1044 2024-03-06 13:58:34.854343 synapse_selector-0.2.9/synapse_selector/settings/default_settings.json
+-rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/utils/__init__.py
+-rw-r--r--   0        0        0     2707 2024-02-21 09:59:58.655504 synapse_selector-0.2.9/synapse_selector/utils/configuration.py
+-rw-r--r--   0        0        0     6421 2024-03-06 14:24:09.578333 synapse_selector-0.2.9/synapse_selector/utils/export.py
+-rw-r--r--   0        0        0      318 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/utils/hash.py
+-rw-r--r--   0        0        0     1523 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/utils/normalization.py
+-rw-r--r--   0        0        0     3759 2024-03-06 13:43:36.906513 synapse_selector-0.2.9/synapse_selector/utils/plot.py
+-rw-r--r--   0        0        0        0 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/utils/post_selection/__init__.py
+-rw-r--r--   0        0        0      658 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/utils/post_selection/decay_compute.py
+-rw-r--r--   0        0        0      712 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/utils/post_selection/failure_rate.py
+-rw-r--r--   0        0        0      624 2024-01-19 10:29:46.578545 synapse_selector-0.2.9/synapse_selector/utils/threshold.py
+-rw-r--r--   0        0        0    13613 2024-03-06 14:39:40.736800 synapse_selector-0.2.9/synapse_selector/utils/trace_data.py
+-rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 synapse_selector-0.2.9/PKG-INFO
```

### Comparing `synapse_selector-0.2.8/LICENSE` & `synapse_selector-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/README.md` & `synapse_selector-0.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -123,30 +123,30 @@
 | Back             | <img src="synapse_selector/assets/back.svg" width="20">     | B        | Go one trace back                                     |
 | Discard          | <img src="synapse_selector/assets/trash.svg" width="20">    | Q        | Discard trace from analysis                           |
 | Accept           | <img src="synapse_selector/assets/keep.svg" width="20">     | E        | Accept trace and keep for analysis                    |
 | Modify Responses | <img src="synapse_selector/assets/peak.svg" width="20">     | W        | Add or remove responses                               |
 
 ### Detailed explanation
 
-1. **Open a File** pressing the open button <img src="synapse_selector/assets/open.svg" "raw" width="20"> in the top bar.
+1. **Open a File** pressing the open button <img src="synapse_selector/assets/open.svg" width="20"> in the top bar.
    - Synapse Selector will visualize the first column of the file that is not a meta column.
    - All detected responses will be annotated.
    - If specified in the settings, a horizontal, red dashed line will be shown
 
-2. **Modify responses** pressing the modify response button <img src="synapse_selector/assets/peak.svg" "raw" width="20"> in the top bar
+2. **Modify responses** pressing the modify response button <img src="synapse_selector/assets/peak.svg" width="20"> in the top bar
    - A window with all detected responses will be opened
    - Deselect false-positive responses
    - Add false-negative responses
 
 3. **Accept or Discard a trace**
-   - To **accept** a trace and subsequently include it in the analysis: <img src="synapse_selector/assets/keep.svg" "raw" width="20">
-   - To **discard** a trace from analysis: <img src="synapse_selector/assets/trash.svg" "raw" width="20">
+   - To **accept** a trace and subsequently include it in the analysis: <img src="synapse_selector/assets/keep.svg" width="20">
+   - To **discard** a trace from analysis: <img src="synapse_selector/assets/trash.svg" width="20">
 
 4. **Change certantiy threshold** (only when using ML-based detection):
    - Use the slider at the bottom to adjust the certantiy threshold used in the model. A lower threshold will lead to more detections, possibly, to more false-positives.
 
-5. **Save and skip rest**: press the save button  <img src="synapse_selector/assets/save.svg" "raw" width="20"> in the top bar. All remaining traces of the file will be discarded.
+5. **Save and skip rest**: press the save button  <img src="synapse_selector/assets/save.svg" width="20"> in the top bar. All remaining traces of the file will be discarded.
 
 ## Train a custom Model
 See the[ Synapse Selector Detect](https://github.com/s-weissbach/synapse_selector_detect/tree/main) for detailed tutorial on how to train a custom model.
 > [!Tip]
 > You can share your model with the community - submit it to [Synapse Selector Modelzoo](https://github.com/s-weissbach/synapse_selector_modelzoo/tree/main).[GitHub - s-weissbach/synapse_selector_modelzoo](https://github.com/s-weissbach/synapse_selector_modelzoo/tree/main).
```

### Comparing `synapse_selector-0.2.8/pyproject.toml` & `synapse_selector-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synapse-selector"
-version = "0.2.8"
+version = "0.2.9"
 description = "Small internal package for post-selection of Glutmate/Calcium signal responses."
 authors = ["Stephan Weissbach <s.weissbach@uni-mainz.de>"]
 readme = "README.md"
 packages = [{include = "synapse_selector"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `synapse_selector-0.2.8/synapse_selector/assets/open.svg` & `synapse_selector-0.2.9/synapse_selector/assets/open.svg`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/assets/save.svg` & `synapse_selector-0.2.9/synapse_selector/assets/save.svg`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/assets/settings.svg` & `synapse_selector-0.2.9/synapse_selector/assets/settings.svg`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/assets/trash.svg` & `synapse_selector-0.2.9/synapse_selector/assets/trash.svg`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/detection/model_wraper.py` & `synapse_selector-0.2.9/synapse_selector/detection/model_wraper.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/detection/model_zoo.py` & `synapse_selector-0.2.9/synapse_selector/detection/model_zoo.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/detection/peak_detection.py` & `synapse_selector-0.2.9/synapse_selector/detection/peak_detection.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/gui/add_window.py` & `synapse_selector-0.2.9/synapse_selector/gui/add_window.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         scroll.setWidgetResizable(True)
         scroll.setWidget(peak_widget_wrapper_widget)
 
         main_layout.addWidget(scroll)
 
     def __update_button_text(self):
         val = self.get_input()
-        if self.parent.settings.config["peak_detection_type"] != "Thresholding":
+        if self.parent.is_ml_detection_activated():
             self.add_button.setText(
                 f"Add Response (Int.: {np.round(self.intensities[val], 2)} | Conf.: {np.round(self.preds[val] * 100, 2)})"
             )
         else:
             self.add_button.setText(
                 f"Add Response (Int.: {np.round(self.intensities[val], 2)})"
             )
@@ -118,15 +118,15 @@
 
     def __add_peak_widget(self, peak_value: int):
         # create layout
         widget_layout = QHBoxLayout()
         widget_layout_wrapper = QWidget()
         widget_layout_wrapper.setLayout(widget_layout)
         # create widgets
-        if self.parent.settings.config["peak_detection_type"] != "Thresholding":
+        if self.parent.is_ml_detection_activated():
             label = QLabel(
                 f"[Frame: {peak_value} | Int.: {np.round(self.intensities[peak_value], 2)} | Conf.: {np.round(self.preds[peak_value] * 100, 2)}]"
             )
         else:
             label = QLabel(
                 f"[Frame: {peak_value} | Int.: {np.round(self.intensities[peak_value], 2)}"
             )
```

### Comparing `synapse_selector-0.2.8/synapse_selector/gui/gui.py` & `synapse_selector-0.2.9/synapse_selector/gui/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         # --- variables ---
         self.directory = None
         self.synapse_response = SynapseResponseData()
 
         self.model = torch_model()
         # load weights for CNN
-        if self.get_setting("peak_detection_type") == "ML-based":
+        if self.is_ml_detection_activated():
             self.model.load_weights(self.get_setting("model_path"))
 
         stim_frames = self.get_setting("stim_frames")
         self.stim_frames = (
             sorted([int(frame) for frame in stim_frames.split(",")])
             if len(stim_frames) > 0
             else []
@@ -366,14 +366,20 @@
         self.main_layout.setStretch(0, 1)
         self.main_layout.setStretch(1, 10)
         self.main_layout.setStretch(2, 1)
 
     def get_setting(self, setting_key: str) -> Union[str, int, float, bool]:
         return self.settings.config[setting_key]
 
+    def is_ml_detection_activated(self):
+        return self.get_setting("ml_detection")
+
+    def is_th_detection_activated(self):
+        return self.get_setting("th_detection")
+
     def reset(self) -> None:
         self.switch_to_start_layout()
         self.close_add_window()
         self.filepath = ""
         self.update_file_path_label("")
 
     def open_file(self) -> None:
@@ -405,26 +411,27 @@
             return
 
         self.filename = os.path.basename(self.filepath)
         self.directory = os.path.dirname(self.filepath)
         self.update_file_path_label(self.filepath)
 
         self.synapse_response.open_file(
-            self.filepath, self.filename, self.get_setting("meta_columns")
+            self.filepath, self.filename, self.get_setting("meta_columns"),
+            self.get_setting("normalization_use_median"),self.get_setting("normalization_sliding_window_size")
         )
         self.labels = []
 
         self.switch_to_main_layout()
         self.plot()
         self.current_roi_label.setText(
             f"Current ROI: {self.synapse_response.columns[self.synapse_response.idx]}"
         )
 
     def add_slider(self):
-        if self.settings.config["peak_detection_type"] != "Thresholding":
+        if self.is_ml_detection_activated():
             self.remove_slider()
 
             self.probability_layout_wrapper.show()
             self.main_layout.addWidget(self.probability_layout_wrapper)
             self.main_layout.setAlignment(
                 self.probability_layout_wrapper,
                 Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignVCenter,
@@ -481,39 +488,28 @@
             self.get_setting("threshold_mult"),
             self.get_setting("threshold_start"),
             self.get_setting("threshold_stop"),
         )
 
         self.peak_detection()
         self.add_window.update_information(
-            self.model.preds
-            if self.settings.config["peak_detection_type"] != "Thresholding"
-            else [],
+            self.model.preds if self.is_ml_detection_activated() else [],
             trace,
         )
         self.initialize_add_window(self.synapse_response.peaks, new_sample=new_sample)
 
         # create plot depending on mode
-        if self.settings.config["peak_detection_type"] == "Thresholding":
-            self.tr_plot = trace_plot(
-                time=self.synapse_response.time,
-                intensity=trace,
-                threshold=self.threshold,
-                peak_detection_type=self.get_setting("peak_detection_type"),
-                always_show_threshold=self.get_setting("always_show_threshold"),
-            )
-        else:
-            self.tr_plot = trace_plot(
-                time=self.synapse_response.time,
-                intensity=trace,
-                threshold=self.threshold,
-                probabilities=self.model.preds,
-                peak_detection_type=self.get_setting("peak_detection_type"),
-                always_show_threshold=self.get_setting("always_show_threshold"),
-            )
+        self.tr_plot = trace_plot(
+            time=self.synapse_response.time,
+            intensity=trace,
+            threshold=self.threshold,
+            threshold_detection_activated=self.is_th_detection_activated(),
+            probabilities=self.model.preds if self.is_ml_detection_activated() else [],
+            always_show_threshold=self.get_setting("always_show_threshold"),
+        )
         self.tr_plot.create_plot()
 
         # add responses
         if self.settings.config["select_responses"]:
             self.stim_frames = self.settings_window.stimframes
             if self.settings.config["stim_used"]:
                 if (
@@ -546,15 +542,15 @@
             self.add_window.get_peak_dict(), self.settings.config["nms"]
         )
 
         # set plot
         self.trace_plot.setHtml(self.tr_plot.fig.to_html(include_plotlyjs="cdn"))
         self.current_state_indicator.setText(self.synapse_response.return_state())
 
-        if self.settings.config["peak_detection_type"] == "Thresholding":
+        if not self.is_ml_detection_activated():
             self.remove_slider()
         else:
             self.add_slider()
 
     def next(self):
         """
         Opens next trace and if this is the last trace, it opens a new file.
@@ -590,53 +586,87 @@
             # tell the user that the file was done and it has been saved
             msg = QMessageBox(self)
             msg.setWindowTitle("Info")
             msg.setText(
                 "You reached the end of the file. Your data will be saved at the set output path"
             )
             msg.exec()
-            self.synapse_response.save(
-                self.stim_frames,
-                self.settings.config,
-                self
-            )
+            self.synapse_response.save(self.stim_frames, self.settings.config, self)
             # self.clear_selection_buttons()
             self.reset()
             self.open_file()
             return
 
         # advance to next trace if file isn't at eof
-        self.synapse_response.next()
+        self.synapse_response.next(self.get_setting("normalization_use_median"),self.get_setting("normalization_sliding_window_size"))
         self.plot()
         self.current_roi_label.setText(
             f"Current ROI: {self.synapse_response.columns[self.synapse_response.idx]}"
         )
         # = QLabel("Current ROI:")
         # self.clear_selection_buttons()
 
     def peak_detection(self):
         """
         Runs peak detection and hands peaks to synapse_response data class.
         """
-        if self.settings.config["peak_detection_type"] == "Thresholding":
-            automatic_peaks = peak_detection_scipy(
+        peaks = []
+        if self.is_th_detection_activated():
+            peaks += peak_detection_scipy(
                 self.synapse_response.norm_intensity,
                 self.threshold,
                 self.settings.config["stim_used"],
                 self.stim_frames,
                 self.settings.config["stim_frames_patience"],
             )
-        else:
+
+        if self.is_ml_detection_activated():
             if not self.model.weights_loaded:
                 self.model.load_weights(self.settings.config["model_path"])
-            automatic_peaks = self.model.predict(
+            peaks += self.model.predict(
                 self.synapse_response.norm_intensity,
                 self.settings.config["threshold_slider_ml"] / 100,
             )
-        self.synapse_response.add_automatic_peaks(automatic_peaks)
+
+        unique_peaks = list(set(peaks))
+        unique_peaks.sort()
+
+        # nms
+        if self.get_setting("nms"):
+            result_arr = []
+            processed_peaks = []
+            window_size = self.get_setting("nms_window")
+
+            # iterate over all peaks
+            for idx, peak in enumerate(unique_peaks):
+                if peak in processed_peaks:
+                    continue
+                # get all peaks within the nms window
+                # as we are starting from the front we only have to look half the window size towards the front
+                tmp_arr = []
+                for inner_idx in range(idx, len(unique_peaks)):
+                    if unique_peaks[inner_idx] <= peak + (window_size // 2):
+                        tmp_arr.append(unique_peaks[inner_idx])
+
+                # element itself is always tmp_arr
+                max_idx = tmp_arr[0]
+
+                for peak_idx in tmp_arr:
+                    if (
+                        self.synapse_response.norm_intensity[peak_idx]
+                        >= self.synapse_response.norm_intensity[max_idx]
+                    ):
+                        max_idx = peak_idx
+                    processed_peaks.append(peak_idx)
+
+                result_arr.append(max_idx)
+
+            unique_peaks = result_arr
+
+        self.synapse_response.add_automatic_peaks(unique_peaks)
 
     def update_probability_label(self) -> None:
         # self.current_threshold.setText(f"{self.threshold_slider.value()}%")
         automatic_peaks = self.model.update_predictions(
             self.settings.config["threshold_slider_ml"] / 100
         )
         self.synapse_response.automatic_peaks = []
```

### Comparing `synapse_selector-0.2.8/synapse_selector/gui/settingswindow.py` & `synapse_selector-0.2.9/synapse_selector/gui/settingswindow.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,14 +57,19 @@
         set_path_layout.addStretch()
         set_path_layout.addWidget(self.button_reset_output_path)
         set_path_layout.addStretch()
         general_layout.addLayout(set_path_layout)
 
         self.add_line_to_layout(general_layout)
 
+        self.export_normalized_traces = QCheckBox("Export normalized traces")
+        self.export_normalized_traces.setToolTip("Absolute traces will be exported as well.")
+        self.export_normalized_traces.clicked.connect(self.handle_settings_toggle)
+        general_layout.addWidget(self.export_normalized_traces)
+
         self.xlsx_export_box = QCheckBox("Export as .xlsx")
         self.xlsx_export_box.clicked.connect(self.handle_settings_toggle)
         general_layout.addWidget(self.xlsx_export_box)
 
         column_list_layout = QVBoxLayout(self)
         column_label = QLabel("Add or remove meta columns for your data:")
         column_list_layout.addWidget(column_label)
@@ -102,26 +107,34 @@
 
         general_wrapper_widget = QWidget()
         general_wrapper_widget.setLayout(general_layout)
 
         # --- response settings ---
         response_layout = QVBoxLayout()
 
-        peak_detection_type_label = QLabel("Select Detection Method:")
-        response_layout.addWidget(peak_detection_type_label)
+        # peak_detection_type_label = QLabel("Select Detection Method:")
+        # response_layout.addWidget(peak_detection_type_label)
 
-        dropdown_layout = QHBoxLayout()
-        self.peak_detection_type = QComboBox()
-        self.peak_detection_type.addItems(["Thresholding", "ML-based"])
-        self.peak_detection_type.currentIndexChanged.connect(
-            self.handle_settings_toggle
-        )
-        dropdown_layout.addWidget(self.peak_detection_type)
-        dropdown_layout.addStretch()
-        response_layout.addLayout(dropdown_layout)
+        self.th_detection_toggle = QCheckBox("Activate Thresholding Detection")
+        self.th_detection_toggle.clicked.connect(self.handle_settings_toggle)
+        response_layout.addWidget(self.th_detection_toggle)
+
+        self.ml_detection_toggle = QCheckBox("Activate ML-Based Detection")
+        self.ml_detection_toggle.clicked.connect(self.handle_settings_toggle)
+        response_layout.addWidget(self.ml_detection_toggle)
+
+        # dropdown_layout = QHBoxLayout()
+        # self.peak_detection_type = QComboBox()
+        # self.peak_detection_type.addItems(["Thresholding", "ML-based"])
+        # self.peak_detection_type.currentIndexChanged.connect(
+        #     self.handle_settings_toggle
+        # )
+        # dropdown_layout.addWidget(self.peak_detection_type)
+        # dropdown_layout.addStretch()
+        # response_layout.addLayout(dropdown_layout)
 
         self.ml_model_used = QLabel("Select Deep Learning Model:")
         response_layout.addWidget(self.ml_model_used)
 
         model_dropdown_layout = QHBoxLayout()
         self.ml_model = QComboBox()
         self.ml_model.addItems(self.settings.modelzoo.available_models.keys())
@@ -164,28 +177,51 @@
         self.frames_for_decay.valueChanged.connect(self.handle_settings_toggle)
         frames_for_decay_layout.addWidget(self.frames_for_decay)
         frames_for_decay_layout.addStretch()
         response_layout.addLayout(frames_for_decay_layout)
 
         self.add_line_to_layout(response_layout)
 
+        self.non_max_supression_button = QCheckBox("Use Non-Maximum Supression")
+        self.non_max_supression_button.stateChanged.connect(self.handle_settings_toggle)
+        response_layout.addWidget(self.non_max_supression_button)
+
+        nms_desc = QLabel("Window for Non-Maximum Supression")
+        response_layout.addWidget(nms_desc)
+
+        nms_window_layout = QHBoxLayout()
+        self.nms_window = QSpinBox()
+        self.nms_window.setToolTip("Window to be used for non-maximum supression")
+        self.nms_window.valueChanged.connect(self.handle_settings_toggle)
+        nms_window_layout.addWidget(self.nms_window)
+        nms_window_layout.addStretch()
+        response_layout.addLayout(nms_window_layout)
+
+        self.add_line_to_layout(response_layout)
+
+        self.normalization_use_median = QCheckBox("Use median for normalization")
+        self.normalization_use_median.clicked.connect(self.handle_settings_toggle)
+        response_layout.addWidget(self.normalization_use_median)
+
+        self.normalization_sliding_window_size = QSpinBox()
+        self.normalization_sliding_window_size.setMinimum(2)
+        self.normalization_sliding_window_size.setMaximum(200)
+        self.normalization_sliding_window_size.valueChanged.connect(self.handle_settings_toggle)
+        response_layout.addWidget(self.normalization_sliding_window_size)
+
         self.normalized_trace_toggle = QCheckBox("Show normalized trace")
         self.normalized_trace_toggle.clicked.connect(self.handle_settings_toggle)
         response_layout.addWidget(self.normalized_trace_toggle)
 
         self.activate_response_selection = QCheckBox("Enable response editing")
         self.activate_response_selection.stateChanged.connect(
             self.handle_settings_toggle
         )
         response_layout.addWidget(self.activate_response_selection)
 
-        self.non_max_supression_button = QCheckBox("Use Non-Maximum Supression")
-        self.non_max_supression_button.stateChanged.connect(self.handle_settings_toggle)
-        response_layout.addWidget(self.non_max_supression_button)
-
         self.compute_ppr = QCheckBox("Compute PPR")
         self.compute_ppr.stateChanged.connect(self.handle_settings_toggle)
         response_layout.addWidget(self.compute_ppr)
 
         response_layout.addStretch()
 
         response_wrapper_widget = QWidget()
@@ -351,29 +387,35 @@
 
     def initialize_widget_values(self):
         self.patience_input.setValue(self.settings.config["stim_frames_patience"])
         self.stimframes_input.setText(self.settings.config["stim_frames"])
         self.stim_used_box.setChecked(self.settings.config["stim_used"])
         self.threshold_input.setValue(self.settings.config["threshold_mult"])
         self.xlsx_export_box.setChecked(self.settings.config["export_xlsx"])
-        if self.settings.config["peak_detection_type"] == "Thresholding":
-            idx = 0
-        else:
-            idx = 1
-        self.peak_detection_type.setCurrentIndex(idx)
+        self.export_normalized_traces.setChecked(self.settings.config["export_normalized_traces"])
+        self.normalization_sliding_window_size.setValue(self.settings.config["normalization_sliding_window_size"])
+        self.normalization_use_median.setChecked(self.settings.config["normalization_use_median"])
+        # if self.settings.config["peak_detection_type"] == "Thresholding":
+        #     idx = 0
+        # else:
+        #     idx = 1
+        # self.peak_detection_type.setCurrentIndex(idx)
+        self.ml_detection_toggle.setChecked(self.settings.config["ml_detection"])
+        self.th_detection_toggle.setChecked(self.settings.config["th_detection"])
         self.ml_model.setCurrentIndex(0)
         self.threshold_slider.setValue(self.settings.config["threshold_slider_ml"])
         self.frames_for_decay.setValue(self.settings.config["frames_for_decay"])
         self.normalized_trace_toggle.setChecked(
             self.settings.config["normalized_trace"]
         )
         self.activate_response_selection.setChecked(
             self.settings.config["select_responses"]
         )
         self.non_max_supression_button.setChecked(self.settings.config["nms"])
+        self.nms_window.setValue(self.settings.config["nms_window"])
         self.use_nms = self.settings.config["nms"]
         self.compute_ppr.setChecked(self.settings.config["compute_ppr"])
         self.threshold_start_input.setValue(self.settings.config["threshold_start"])
         self.threshold_stop_input.setValue(self.settings.config["threshold_stop"])
         self.threshold_input.setSingleStep(self.settings.config["threshold_step"])
         self.show_threshold.setChecked(self.settings.config["always_show_threshold"])
         self.start_stimulation_input.setValue(self.settings.config["stim_frames_start"])
@@ -426,28 +468,31 @@
         # update all values that might have been changed
         self.settings.config["threshold_mult"] = self.threshold_input.value()
         self.settings.config["threshold_start"] = self.threshold_start_input.value()
         self.settings.config["threshold_stop"] = self.threshold_stop_input.value()
         self.settings.config["stim_frames_patience"] = self.patience_input.value()
         self.settings.config["frames_for_decay"] = self.frames_for_decay.value()
         self.settings.config["stim_frames"] = self.stimframes_input.text()
-        self.settings.config[
-            "peak_detection_type"
-        ] = self.peak_detection_type.currentText()
+        self.settings.config["th_detection"] = self.th_detection_toggle.isChecked()
+        self.settings.config["ml_detection"] = self.ml_detection_toggle.isChecked()
         model_path = self.settings.modelzoo.available_models[
             self.ml_model.currentText()
         ]["filepath"]
         self.settings.config["model_path"] = model_path
         self.settings.config["nms"] = self.non_max_supression_button.isChecked()
+        self.settings.config["nms_window"] = self.nms_window.value()
         self.settings.config["stim_used"] = self.stim_used_box.isChecked()
         self.settings.config[
             "select_responses"
         ] = self.activate_response_selection.isChecked()
         self.settings.config["compute_ppr"] = self.compute_ppr.isChecked()
+        self.settings.config["export_normalized_traces"] = self.export_normalized_traces.isChecked()
         self.settings.config["export_xlsx"] = self.xlsx_export_box.isChecked()
+        self.settings.config["normalization_use_median"] = self.normalization_use_median.isChecked()
+        self.settings.config["normalization_sliding_window_size"] = self.normalization_sliding_window_size.value()
         self.settings.config[
             "normalized_trace"
         ] = self.normalized_trace_toggle.isChecked()
         self.settings.config["threshold_slider_ml"] = self.threshold_slider.value()
         self.settings.config["always_show_threshold"] = self.show_threshold.isChecked()
         self.settings.config["stim_frames_start"] = self.start_stimulation_input.value()
         self.settings.config["stim_frames_step"] = self.step_stimulation_input.value()
@@ -464,19 +509,20 @@
         self.settings.config["meta_columns"] = new_meta_columns
 
         self.parse_stim_frames()
         self.handle_settings_toggle()
         self.check_patience()
 
         if (
-            self.settings.config["peak_detection_type"] == "ML-based"
+            self.settings.config["ml_detection"]
+            and not self.settings.config["th_detection"]
             and self.settings.config["model_path"] == ""
         ):
-            warnings.warn("No model selected. Will switch to thresholding.")
-            self.settings.config["peak_detection_type"] = "Thresholding"
+            warnings.warn("No model selected. Will activate thresholding")
+            self.settings.config["th_detection"] = True
 
         # update settings
         self.parent.settings = self.settings
         self.settings.write_settings()
         self.parent.stimframes = self.stimframes
 
         # replot whenever any setting is changed
@@ -507,21 +553,20 @@
             self.patience_input.setStyleSheet(
                 "QSpinBox" "{" "background : #ff5959;" "}"
             )
 
     def handle_settings_toggle(self) -> None:
         self.current_threshold_label.setText(f"{self.threshold_slider.value()}%")
 
-        if self.peak_detection_type.currentText() == "ML-based":
+        if self.ml_detection_toggle.isChecked():
             self.ml_model.setEnabled(True)
             self.ml_model_used.setEnabled(True)
             self.threshold_label.setEnabled(True)
             self.current_threshold_label.setEnabled(True)
             self.threshold_slider.setEnabled(True)
-
         else:
             self.ml_model.setEnabled(False)
             self.ml_model_used.setEnabled(False)
             self.threshold_label.setEnabled(False)
             self.current_threshold_label.setEnabled(False)
             self.threshold_slider.setEnabled(False)
 
@@ -534,14 +579,19 @@
         else:
             self.stimframes_input.setEnabled(False)
             self.stimframes_label.setEnabled(False)
             self.patience_label.setEnabled(False)
             self.patience_input.setEnabled(False)
             self.compute_ppr.setEnabled(False)
 
+        if self.non_max_supression_button.isChecked():
+            self.nms_window.setEnabled(True)
+        else:
+            self.nms_window.setEnabled(False)
+
         # activate add response button depending on setting
         if self.activate_response_selection.isChecked():
             self.parent.button_add.setEnabled(True)
             self.compute_ppr.setEnabled(True)
             self.non_max_supression_button.setEnabled(True)
         else:
             self.parent.button_add.setDisabled(True)
```

### Comparing `synapse_selector-0.2.8/synapse_selector/main.py` & `synapse_selector-0.2.9/synapse_selector/main.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/settings/default_settings.json` & `synapse_selector-0.2.9/synapse_selector/settings/default_settings.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'export_normalized_traces'": 'True',*

 * * "'ml_detection'": 'True',*

 * * "'nms_window'": '10',*

 * * "'normalization_sliding_window_size'": '50',*

 * * "'normalization_use_median'": 'True',*

 * * "'th_detection'": 'True',*

 * * 'delete': "['peak_detection_type']"}*

```diff
@@ -1,10 +1,11 @@
 {
     "always_show_threshold": false,
     "compute_ppr": false,
+    "export_normalized_traces": true,
     "export_xlsx": false,
     "frames_for_decay": 6,
     "meta_columns": [
         "file name",
         "total frames",
         "macro version",
         "xSD ROI",
@@ -13,25 +14,29 @@
         "frames baseline",
         "frames response",
         "abs frame #",
         "rel frame #",
         "empty",
         "average Z"
     ],
+    "ml_detection": true,
     "model_path": "",
     "nms": false,
+    "nms_window": 10,
+    "normalization_sliding_window_size": 50,
+    "normalization_use_median": true,
     "normalized_trace": true,
     "output_filepath": "",
-    "peak_detection_type": "Thresholding",
     "select_responses": false,
     "stim_frames": "",
     "stim_frames_patience": 10,
     "stim_frames_start": 0,
     "stim_frames_step": 30,
     "stim_used": false,
+    "th_detection": true,
     "threshold_mult": 4.0,
     "threshold_slider_ml": 50,
     "threshold_start": 0,
     "threshold_step": 0.1,
     "threshold_stop": 50,
     "use_manual_stim_frames": false
 }
```

### Comparing `synapse_selector-0.2.8/synapse_selector/utils/configuration.py` & `synapse_selector-0.2.9/synapse_selector/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/utils/export.py` & `synapse_selector-0.2.9/synapse_selector/utils/export.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 import pandas as pd
 import numpy as np
+from synapse_selector.utils.normalization import sliding_window_normalization
+
+
+def normalized_trace_df(
+        trace_df: pd.DataFrame,
+        normalization_use_median: bool,
+        normalization_sliding_window_size: int
+) -> pd.DataFrame:
+    norm_trace_df = pd.DataFrame()
+    for col in trace_df.columns:
+        norm_trace_df[col] = sliding_window_normalization(trace_df[col].to_numpy(), normalization_use_median, normalization_sliding_window_size)
+    return norm_trace_df
+
 
 def create_peak_df(
         selected_peaks: list
 ) -> pd.DataFrame:
     peak_df = pd.DataFrame(
                 selected_peaks,
                 columns=[
```

### Comparing `synapse_selector-0.2.8/synapse_selector/utils/normalization.py` & `synapse_selector-0.2.9/synapse_selector/utils/normalization.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/utils/plot.py` & `synapse_selector-0.2.9/synapse_selector/utils/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 class trace_plot:
     def __init__(
         self,
         time: np.ndarray,
         intensity: np.ndarray,
         threshold: float,
-        peak_detection_type="Thresholding",
+        threshold_detection_activated: bool,
         probabilities=[],
         always_show_threshold=False,
     ):
         self.time = time
         self.intensity = intensity
         self.threshold = threshold
-        self.peak_detection_type = peak_detection_type
+        self.threshold_detection_activated = threshold_detection_activated
         self.always_show_threshold = always_show_threshold
 
         if len(probabilities) == 0:
             self.probabilities = [0 for _ in range(len(time))]
         else:
             self.probabilities = [f"{np.round(p*100,2)}%" for p in probabilities]
         self.plot_df = pd.DataFrame(
@@ -40,15 +40,15 @@
             self.plot_df, x="Time", y="Intensity", hover_data="Confidence"
         )
         self.fig.update_layout(
             template="plotly_white",
             xaxis=dict(rangeslider=dict(visible=True), type="linear"),
         )
 
-        if self.peak_detection_type == "Thresholding" or self.always_show_threshold:
+        if self.threshold_detection_activated or self.always_show_threshold:
             self.fig.add_hline(y=self.threshold, line_color="red", line_dash="dash")
 
     def add_stimulation_window(
         self, frames: list[int], patience: int, start: int = 0, step: int = 30
     ) -> None:
         """
         Adds the stimulation window in yellow after each stimulation for the time
```

### Comparing `synapse_selector-0.2.8/synapse_selector/utils/post_selection/decay_compute.py` & `synapse_selector-0.2.9/synapse_selector/utils/post_selection/decay_compute.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/utils/post_selection/failure_rate.py` & `synapse_selector-0.2.9/synapse_selector/utils/post_selection/failure_rate.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/utils/threshold.py` & `synapse_selector-0.2.9/synapse_selector/utils/threshold.py`

 * *Files identical despite different names*

### Comparing `synapse_selector-0.2.8/synapse_selector/utils/trace_data.py` & `synapse_selector-0.2.9/synapse_selector/utils/trace_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import os
 from PyQt6.QtWidgets import QMessageBox
 
 from synapse_selector.utils.post_selection.decay_compute import compute_tau
 from synapse_selector.utils.post_selection.failure_rate import failure_rate
 from synapse_selector.utils.normalization import sliding_window_normalization
-from synapse_selector.utils.export import create_stimulation_df, create_peak_df, create_ppr_df, create_fraction_first_pulse_df, create_settings_df, write_excel_output
+from synapse_selector.utils.export import create_stimulation_df, create_peak_df, create_ppr_df, create_fraction_first_pulse_df, create_settings_df, write_excel_output, normalized_trace_df
 
 
 class SynapseResponseData:
     def __init__(self) -> None:
         self.filename = ""
         self.df = pd.DataFrame()
         self.meta_columns = []
@@ -25,15 +25,15 @@
         self.selected_peaks = []
         self.intensity = np.empty(0, dtype=np.float64)
         self.norm_intensity = np.empty(0, dtype=np.float64)
         self.time = np.empty(0, dtype=np.float64)
         self.automatic_peaks = []
         self.file_opened = False
 
-    def open_file(self, filepath: str, filename: str, meta_columns: list[str]):
+    def open_file(self, filepath: str, filename: str, meta_columns: list[str], normalization_use_median: bool, normalization_sliding_window: int):
         self.filename = filename
         if filepath.endswith(".txt") or filepath.endswith(".csv"):
             self.df = pd.read_csv(filepath, sep=",")
         else:
             self.df = pd.read_excel(filepath)
         self.meta_columns = [
             col
@@ -46,15 +46,16 @@
         self.idx = 0
         self.last = []
         self.peaks = []
         self.manual_peaks = []
         self.selected_peaks = []
         self.intensity = self.df[self.columns[self.idx]].to_numpy(dtype=np.float64)
         self.norm_intensity = sliding_window_normalization(
-            self.df[self.columns[self.idx]].to_numpy()
+            self.df[self.columns[self.idx]].to_numpy(),
+            normalization_use_median, normalization_sliding_window
         )
         self.time = np.arange(len(self.intensity))
         self.automatic_peaks = []
         self.file_opened = True
 
     def __len__(self) -> int:
         """
@@ -86,14 +87,19 @@
         ppr = settings["compute_ppr"]
         patience = settings["stim_frames_patience"]
         os.makedirs(keep_path, exist_ok=True)
         os.makedirs(discard_path, exist_ok=True)
         keep_df = self.df[self.meta_columns + self.keep_data]
         discard_df = self.df[self.meta_columns + self.discard_data]
         file_prefix = '.'.join(self.filename.split('.')[:-1])
+        if settings["export_normalized_traces"]:
+            normalized_keep_df = normalized_trace_df(keep_df[self.keep_data],settings["normalization_use_median"],settings["normalization_sliding_window_size"])
+            # instert meta_columns
+            for i,col in enumerate(self.meta_columns):
+                normalized_keep_df.insert(i,col,self.df[col])
         if (
             export_xlsx
             or self.filename.endswith(".xlsx")
             or self.filename.endswith(".xls")
         ):
             output_name = f"{file_prefix}.xlsx"
             output_path = os.path.join(keep_path, output_name)
@@ -109,15 +115,17 @@
                 msg = QMessageBox(parent)
                 msg.setIcon(QMessageBox.Icon.Warning)
                 msg.setWindowTitle("Warning")
                 msg.setText(
                     f"The file {original_output_name} alreads exists in {keep_path}. Saved as {output_name}"
                 )
                 msg.exec()
-                keep_df.to_excel(output_name, index=False)
+            keep_df.to_excel(output_path, index=False)
+            if settings["export_normalized_traces"]:
+                normalized_keep_df.to_excel(os.path.join(keep_path, f"{file_prefix}_normalized.xlsx"), index=False)
             discard_df.to_excel(os.path.join(discard_path, output_name), index=False)
         else:
             output_name = f"{file_prefix}.csv"
             output_path = os.path.join(keep_path, output_name)
             if os.path.exists(output_path):
                 i = 1
                 original_output_name = output_name
@@ -131,14 +139,16 @@
                 msg.setIcon(QMessageBox.Icon.Warning)
                 msg.setWindowTitle("Warning")
                 msg.setText(
                     f"The file {original_output_name} alreads exists in {keep_path}. Saved as {output_name}"
                 )
                 msg.exec()
             keep_df.to_csv(output_path, index=False)
+            if settings["export_normalized_traces"]:
+                normalized_keep_df.to_excel(os.path.join(keep_path, f"{file_prefix}_normalized.csv"), index=False)
             discard_df.to_csv(os.path.join(discard_path, output_name), index=False)
         analysis_dfs = []
         analysis_names = []
         settings_df = create_settings_df(settings)
         analysis_dfs.append(settings_df)
         analysis_names.append('parameters')
         if len(self.selected_peaks) > 0:
@@ -169,24 +179,25 @@
             f"{file_prefix}_analysis.xlsx"
         )
         analysis_outputpath = os.path.join(keep_path, output_name)
         if len(analysis_dfs) > 0:
             write_excel_output(analysis_dfs,analysis_names,analysis_outputpath)
             
 
-    def next(self) -> None:
+    def next(self, normalization_use_median: bool, normalization_sliding_window: int) -> None:
         """
         Go to next trace and load the data
         """
         self.idx += 1
         self.peaks = []
         self.manual_peaks = []
         self.intensity = self.df[self.columns[self.idx]].to_numpy()
         self.norm_intensity = sliding_window_normalization(
-            self.df[self.columns[self.idx]].to_numpy()
+            self.df[self.columns[self.idx]].to_numpy(),
+            normalization_use_median, normalization_sliding_window
         )
         self.time = np.arange(len(self.intensity))
 
     def back(self) -> bool:
         """
         Go back one trace and undo the selection. If it is the first trace of
         the file, nothing is done.
```

### Comparing `synapse_selector-0.2.8/PKG-INFO` & `synapse_selector-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapse-selector
-Version: 0.2.8
+Version: 0.2.9
 Summary: Small internal package for post-selection of Glutmate/Calcium signal responses.
 Author: Stephan Weissbach
 Author-email: s.weissbach@uni-mainz.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -144,31 +144,31 @@
 | Back             | <img src="synapse_selector/assets/back.svg" width="20">     | B        | Go one trace back                                     |
 | Discard          | <img src="synapse_selector/assets/trash.svg" width="20">    | Q        | Discard trace from analysis                           |
 | Accept           | <img src="synapse_selector/assets/keep.svg" width="20">     | E        | Accept trace and keep for analysis                    |
 | Modify Responses | <img src="synapse_selector/assets/peak.svg" width="20">     | W        | Add or remove responses                               |
 
 ### Detailed explanation
 
-1. **Open a File** pressing the open button <img src="synapse_selector/assets/open.svg" "raw" width="20"> in the top bar.
+1. **Open a File** pressing the open button <img src="synapse_selector/assets/open.svg" width="20"> in the top bar.
    - Synapse Selector will visualize the first column of the file that is not a meta column.
    - All detected responses will be annotated.
    - If specified in the settings, a horizontal, red dashed line will be shown
 
-2. **Modify responses** pressing the modify response button <img src="synapse_selector/assets/peak.svg" "raw" width="20"> in the top bar
+2. **Modify responses** pressing the modify response button <img src="synapse_selector/assets/peak.svg" width="20"> in the top bar
    - A window with all detected responses will be opened
    - Deselect false-positive responses
    - Add false-negative responses
 
 3. **Accept or Discard a trace**
-   - To **accept** a trace and subsequently include it in the analysis: <img src="synapse_selector/assets/keep.svg" "raw" width="20">
-   - To **discard** a trace from analysis: <img src="synapse_selector/assets/trash.svg" "raw" width="20">
+   - To **accept** a trace and subsequently include it in the analysis: <img src="synapse_selector/assets/keep.svg" width="20">
+   - To **discard** a trace from analysis: <img src="synapse_selector/assets/trash.svg" width="20">
 
 4. **Change certantiy threshold** (only when using ML-based detection):
    - Use the slider at the bottom to adjust the certantiy threshold used in the model. A lower threshold will lead to more detections, possibly, to more false-positives.
 
-5. **Save and skip rest**: press the save button  <img src="synapse_selector/assets/save.svg" "raw" width="20"> in the top bar. All remaining traces of the file will be discarded.
+5. **Save and skip rest**: press the save button  <img src="synapse_selector/assets/save.svg" width="20"> in the top bar. All remaining traces of the file will be discarded.
 
 ## Train a custom Model
 See the[ Synapse Selector Detect](https://github.com/s-weissbach/synapse_selector_detect/tree/main) for detailed tutorial on how to train a custom model.
 > [!Tip]
 > You can share your model with the community - submit it to [Synapse Selector Modelzoo](https://github.com/s-weissbach/synapse_selector_modelzoo/tree/main).[GitHub - s-weissbach/synapse_selector_modelzoo](https://github.com/s-weissbach/synapse_selector_modelzoo/tree/main).
```

