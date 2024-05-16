# Comparing `tmp/cpimerge-0.0.9.tar.gz` & `tmp/cpimerge-0.1.0.tar.gz`

## Comparing `cpimerge-0.0.9.tar` & `cpimerge-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.9/src/cpimerge/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cpimerge-0.0.9/src/cpimerge/__main__.py
--rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 cpimerge-0.0.9/src/cpimerge/cpimerge.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cpimerge-0.0.9/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.0.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.9/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpimerge-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.1.0/src/cpimerge/__init__.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 cpimerge-0.1.0/src/cpimerge/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cpimerge-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.1.0/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.1.0/PKG-INFO
```

### Comparing `cpimerge-0.0.9/src/cpimerge/cpimerge.py` & `cpimerge-0.1.0/src/cpimerge/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 # Backup file
 def backup_file(file_path):
     backup_path = f"{file_path}.{datetime.now().strftime('%Y%m%d_%H%M%S')}.bak"
     shutil.copy2(file_path, backup_path)
     return backup_path
 
 # Main function to merge calendars
-def main(ics1_path, ics2_path, exclusions_path, output_path, output_text, rename_ics2):
+def mainmerge(ics1_path, ics2_path, exclusions_path, output_path, output_text, rename_ics2):
     try:
         if os.path.exists(ics1_path):
             backup_ics1_path = backup_file(ics1_path)
             output_text.insert(tk.END, f"Backup of '{ics1_path}' created: {backup_ics1_path}\n")
             cal1 = load_ics(ics1_path)
         else:
             output_text.insert(tk.END, f"No ics1 provided. Using an empty iCal.\n")
@@ -263,15 +263,15 @@
         return
 
     if exclusions_path and not os.path.exists(exclusions_path):
         messagebox.showerror("Error", f"File not found: {exclusions_path}")
         return
 
     output_text.delete(1.0, tk.END)
-    main(ics1_path, ics2_path, exclusions_path if exclusions_path else None, output_path, output_text, rename_ics2)
+    mainmerge(ics1_path, ics2_path, exclusions_path if exclusions_path else None, output_path, output_text, rename_ics2)
     output_text.insert(tk.END, f"\nCalendars merged successfully.\n\n** You can now import the new events from {output_path} **")
 
     # Save the configuration
     config = {
         "ics1_path": ics1_path,
         "ics2_path": ics2_path,
         "exclusions_path": exclusions_path,
@@ -295,75 +295,76 @@
 def save_config(config):
     try:
         with open(config_path, 'w') as f:
             json.dump(config, f, indent=4)
     except Exception as e:
         messagebox.showerror("Error", f"Failed to save configuration file: {e}")
 
-# Load initial configuration
-config = load_config()
+def main():
+    # Load initial configuration
+    config = load_config()
+
+    # Initialize GUI
+    root = tk.Tk()
+    root.title("CPI iCal Merger")
 
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
+
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
 
-root.mainloop()
+    root.mainloop()
 
 if __name__ == "__main__":
     main()
```

### Comparing `cpimerge-0.0.9/.gitignore` & `cpimerge-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cpimerge-0.0.9/LICENSE` & `cpimerge-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpimerge-0.0.9/pyproject.toml` & `cpimerge-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpimerge"
-
-version = "0.0.9"
-
+version = "0.1.0"
 dependencies = [
   "icalendar",
   "appdirs",
 ]
-
 authors = [
   { name="Kirk Coombs", email="cpimerge@coombscloud.com" },
 ]
-
 description = "Merge iCal files generated by CPI"
-
 readme = "README.md"
-
 requires-python = ">=3.8"
-
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-
 [project.urls]
 Homepage = "https://github.com/kcoombs/cpimerge"
-
 [project.scripts]
-cpimerge = "cpimerge.cpimerge:main"
+cpimerge = "cpimerge.main:main"
```

