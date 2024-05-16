# Comparing `tmp/cpimerge-0.1.1.tar.gz` & `tmp/cpimerge-0.1.2.tar.gz`

## Comparing `cpimerge-0.1.1.tar` & `cpimerge-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.1.1/src/cpimerge/__init__.py
--rw-r--r--   0        0        0    18872 2020-02-02 00:00:00.000000 cpimerge-0.1.1/src/cpimerge/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cpimerge-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.1.1/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.1.2/src/cpimerge/__init__.py
+-rw-r--r--   0        0        0    19050 2020-02-02 00:00:00.000000 cpimerge-0.1.2/src/cpimerge/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cpimerge-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.1.2/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.1.2/PKG-INFO
```

### Comparing `cpimerge-0.1.1/src/cpimerge/main.py` & `cpimerge-0.1.2/src/cpimerge/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -340,76 +340,75 @@
 
     rename_var = tk.BooleanVar(value=False)
     rename_checkbox = tk.Checkbutton(frame, text="Rename ics2 to ics1 after merging", variable=rename_var)
     rename_checkbox.grid(row=4, column=0, columnspan=4, pady=5)
 
     button_frame = tk.Frame(frame)
     button_frame.grid(row=5, column=0, columnspan=4, pady=20)
-# Load initial configuration
-config = load_config()
 
-# Initialize GUI
-root = tk.Tk()
-root.title("CPI iCal Merger")
-
-# GUI elements
-frame = tk.Frame(root, padx=10, pady=10)
-frame.pack(fill=tk.BOTH, expand=True)
-
-tk.Label(frame, text="Previous iCal Export (ics1) (optional):").grid(row=0, column=0, padx=10, pady=5, sticky=tk.W)
-ics1_entry = tk.Entry(frame, width=50)
-ics1_entry.grid(row=0, column=1, padx=10, pady=5, sticky=tk.W+tk.E)
-ics1_entry.insert(0, config.get("ics1_path", ""))
-tk.Button(frame, text="Browse", command=lambda: select_file(ics1_entry)).grid(row=0, column=2, padx=10, pady=5)
-tk.Button(frame, text="?", command=lambda: show_description("The iCal (.ics) file you used for the previous run of this tool.\n\nThis file will automatically be backed-up.\n\nIf no file, or an invalid file, is provided, an empty iCal with no events will be used. This useful for the first run of this program.")).grid(row=0, column=3, padx=10, pady=5)
-
-tk.Label(frame, text="New iCal Export (ics2):").grid(row=1, column=0, padx=10, pady=5, sticky=tk.W)
-ics2_entry = tk.Entry(frame, width=50)
-ics2_entry.grid(row=1, column=1, padx=10, pady=5, sticky=tk.W+tk.E)
-ics2_entry.insert(0, config.get("ics2_path", ""))
-tk.Button(frame, text="Browse", command=lambda: select_file(ics2_entry)).grid(row=1, column=2, padx=10, pady=5)
-tk.Button(frame, text="?", command=lambda: show_description("The new iCal (.ics) file that you'd like to get events from.\n\nThis file will automatically be backed-up.\n\nIf 'Rename ics2 to ics1 after merging' is checked, the file provided in this field will be renamed to the name provided for the ics1 file (e.g., for use in the next run of this program).")).grid(row=1, column=3, padx=10, pady=5)
-
-tk.Label(frame, text="Exclusions File (optional):").grid(row=2, column=0, padx=10, pady=5, sticky=tk.W)
-exclusions_entry = tk.Entry(frame, width=50)
-exclusions_entry.grid(row=2, column=1, padx=10, pady=5, sticky=tk.W+tk.E)
-exclusions_entry.insert(0, config.get("exclusions_path", ""))
-tk.Button(frame, text="Browse", command=lambda: select_file(exclusions_entry)).grid(row=2, column=2, padx=10, pady=5)
-tk.Button(frame, text="?", command=lambda: show_description("An optional file containing sub-strings, one per line. When matched, these sub-strings will cause an event to be excluded from the output.")).grid(row=2, column=3, padx=10, pady=5)
-
-tk.Label(frame, text="Output File:").grid(row=3, column=0, padx=10, pady=5, sticky=tk.W)
-output_entry = tk.Entry(frame, width=50)
-output_entry.grid(row=3, column=1, padx=10, pady=5, sticky=tk.W+tk.E)
-output_entry.insert(0, config.get("output_path", ""))
-tk.Button(frame, text="Browse", command=lambda: select_output_file(output_entry)).grid(row=3, column=2, padx=10, pady=5)
-tk.Button(frame, text="?", command=lambda: show_description("An output iCal (.ics) file, which will contain any new events. This can be imported into to your calendar.")).grid(row=3, column=3, padx=10, pady=5)
-
-rename_var = tk.BooleanVar(value=False)
-rename_checkbox = tk.Checkbutton(frame, text="Rename ics2 to ics1 after merging", variable=rename_var)
-rename_checkbox.grid(row=4, column=0, columnspan=4, pady=5)
-
-button_frame = tk.Frame(frame)
-button_frame.grid(row=5, column=0, columnspan=4, pady=20)
-
-tk.Button(button_frame, text="Load", command=load_files).pack(side=tk.LEFT, padx=10)
-tk.Button(button_frame, text="Merge", command=run_merge).pack(side=tk.LEFT, padx=10)
-
-output_frame = tk.Frame(frame)
-output_frame.grid(row=6, column=0, columnspan=4, padx=10, pady=10, sticky=tk.W+tk.E+tk.N+tk.S)
-
-output_text = tk.Text(output_frame, height=30, width=100)
-output_text.pack(side=tk.LEFT, fill=tk.BOTH, expand=True)
-
-scrollbar = tk.Scrollbar(output_frame, command=output_text.yview)
-scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
-
-output_text.config(yscrollcommand=scrollbar.set)
-
-# Make the grid cells expand with window resizing
-frame.grid_rowconfigure(6, weight=1)
-frame.grid_columnconfigure(1, weight=1)
+if __name__ == "__main__":
+    # Load initial configuration
+    config = load_config()
 
-def main():
-    root.mainloop()
+    # Initialize GUI
+    root = tk.Tk()
+    root.title("CPI iCal Merger")
+
+    # GUI elements
+    frame = tk.Frame(root, padx=10, pady=10)
+    frame.pack(fill=tk.BOTH, expand=True)
+
+    tk.Label(frame, text="Previous iCal Export (ics1) (optional):").grid(row=0, column=0, padx=10, pady=5, sticky=tk.W)
+    ics1_entry = tk.Entry(frame, width=50)
+    ics1_entry.grid(row=0, column=1, padx=10, pady=5, sticky=tk.W+tk.E)
+    ics1_entry.insert(0, config.get("ics1_path", ""))
+    tk.Button(frame, text="Browse", command=lambda: select_file(ics1_entry)).grid(row=0, column=2, padx=10, pady=5)
+    tk.Button(frame, text="?", command=lambda: show_description("The iCal (.ics) file you used for the previous run of this tool.\n\nThis file will automatically be backed-up.\n\nIf no file, or an invalid file, is provided, an empty iCal with no events will be used. This useful for the first run of this program.")).grid(row=0, column=3, padx=10, pady=5)
+
+    tk.Label(frame, text="New iCal Export (ics2):").grid(row=1, column=0, padx=10, pady=5, sticky=tk.W)
+    ics2_entry = tk.Entry(frame, width=50)
+    ics2_entry.grid(row=1, column=1, padx=10, pady=5, sticky=tk.W+tk.E)
+    ics2_entry.insert(0, config.get("ics2_path", ""))
+    tk.Button(frame, text="Browse", command=lambda: select_file(ics2_entry)).grid(row=1, column=2, padx=10, pady=5)
+    tk.Button(frame, text="?", command=lambda: show_description("The new iCal (.ics) file that you'd like to get events from.\n\nThis file will automatically be backed-up.\n\nIf 'Rename ics2 to ics1 after merging' is checked, the file provided in this field will be renamed to the name provided for the ics1 file (e.g., for use in the next run of this program).")).grid(row=1, column=3, padx=10, pady=5)
+
+    tk.Label(frame, text="Exclusions File (optional):").grid(row=2, column=0, padx=10, pady=5, sticky=tk.W)
+    exclusions_entry = tk.Entry(frame, width=50)
+    exclusions_entry.grid(row=2, column=1, padx=10, pady=5, sticky=tk.W+tk.E)
+    exclusions_entry.insert(0, config.get("exclusions_path", ""))
+    tk.Button(frame, text="Browse", command=lambda: select_file(exclusions_entry)).grid(row=2, column=2, padx=10, pady=5)
+    tk.Button(frame, text="?", command=lambda: show_description("An optional file containing sub-strings, one per line. When matched, these sub-strings will cause an event to be excluded from the output.")).grid(row=2, column=3, padx=10, pady=5)
+
+    tk.Label(frame, text="Output File:").grid(row=3, column=0, padx=10, pady=5, sticky=tk.W)
+    output_entry = tk.Entry(frame, width=50)
+    output_entry.grid(row=3, column=1, padx=10, pady=5, sticky=tk.W+tk.E)
+    output_entry.insert(0, config.get("output_path", ""))
+    tk.Button(frame, text="Browse", command=lambda: select_output_file(output_entry)).grid(row=3, column=2, padx=10, pady=5)
+    tk.Button(frame, text="?", command=lambda: show_description("An output iCal (.ics) file, which will contain any new events. This can be imported into to your calendar.")).grid(row=3, column=3, padx=10, pady=5)
 
-if __name__ == "__main__":
-    main()
+    rename_var = tk.BooleanVar(value=False)
+    rename_checkbox = tk.Checkbutton(frame, text="Rename ics2 to ics1 after merging", variable=rename_var)
+    rename_checkbox.grid(row=4, column=0, columnspan=4, pady=5)
+
+    button_frame = tk.Frame(frame)
+    button_frame.grid(row=5, column=0, columnspan=4, pady=20)
+
+    tk.Button(button_frame, text="Load", command=load_files).pack(side=tk.LEFT, padx=10)
+    tk.Button(button_frame, text="Merge", command=run_merge).pack(side=tk.LEFT, padx=10)
+
+    output_frame = tk.Frame(frame)
+    output_frame.grid(row=6, column=0, columnspan=4, padx=10, pady=10, sticky=tk.W+tk.E+tk.N+tk.S)
+
+    output_text = tk.Text(output_frame, height=30, width=100)
+    output_text.pack(side=tk.LEFT, fill=tk.BOTH, expand=True)
+
+    scrollbar = tk.Scrollbar(output_frame, command=output_text.yview)
+    scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
+
+    output_text.config(yscrollcommand=scrollbar.set)
+
+    # Make the grid cells expand with window resizing
+    frame.grid_rowconfigure(6, weight=1)
+    frame.grid_columnconfigure(1, weight=1)
+
+    root.mainloop()
+
```

### Comparing `cpimerge-0.1.1/.gitignore` & `cpimerge-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cpimerge-0.1.1/LICENSE` & `cpimerge-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpimerge-0.1.1/pyproject.toml` & `cpimerge-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpimerge"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
   "icalendar",
   "appdirs",
 ]
 authors = [
   { name="Kirk Coombs", email="cpimerge@coombscloud.com" },
 ]
```

