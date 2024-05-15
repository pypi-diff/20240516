# Comparing `tmp/procedure_data_tool-0.0.4.tar.gz` & `tmp/procedure_data_tool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procedure_data_tool-0.0.4.tar", last modified: Mon May 13 18:37:32 2024, max compression
+gzip compressed data, was "procedure_data_tool-0.0.6.tar", last modified: Wed May 15 22:14:27 2024, max compression
```

## Comparing `procedure_data_tool-0.0.4.tar` & `procedure_data_tool-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:37:32.903132 procedure_data_tool-0.0.4/
--rw-rw-rw-   0        0        0        0 2024-05-09 22:58:17.000000 procedure_data_tool-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      318 2024-05-13 18:37:32.903132 procedure_data_tool-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 23:00:28.000000 procedure_data_tool-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 18:37:32.889313 procedure_data_tool-0.0.4/procedure_data_tool/
--rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.4/procedure_data_tool/__init__.py
--rw-rw-rw-   0        0        0     2650 2024-05-08 20:03:38.000000 procedure_data_tool-0.0.4/procedure_data_tool/excelData.py
--rw-rw-rw-   0        0        0     5015 2024-05-13 15:53:37.000000 procedure_data_tool-0.0.4/procedure_data_tool/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:37:32.902130 procedure_data_tool-0.0.4/procedure_data_tool.egg-info/
--rw-rw-rw-   0        0        0      318 2024-05-13 18:37:32.000000 procedure_data_tool-0.0.4/procedure_data_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-05-13 18:37:32.000000 procedure_data_tool-0.0.4/procedure_data_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:37:32.000000 procedure_data_tool-0.0.4/procedure_data_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-13 18:37:32.000000 procedure_data_tool-0.0.4/procedure_data_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 18:37:32.000000 procedure_data_tool-0.0.4/procedure_data_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 18:37:32.000000 procedure_data_tool-0.0.4/procedure_data_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      132 2024-05-13 18:37:32.904638 procedure_data_tool-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      791 2024-05-13 18:36:44.000000 procedure_data_tool-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:14:27.392218 procedure_data_tool-0.0.6/
+-rw-rw-rw-   0        0        0        0 2024-05-09 22:58:17.000000 procedure_data_tool-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       54 2024-05-15 14:25:33.000000 procedure_data_tool-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2024-05-15 22:14:27.392218 procedure_data_tool-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 23:00:28.000000 procedure_data_tool-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 22:14:27.360553 procedure_data_tool-0.0.6/procedure_data_tool/
+-rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.6/procedure_data_tool/__init__.py
+-rw-rw-rw-   0        0        0     5996 2024-05-15 21:17:11.000000 procedure_data_tool-0.0.6/procedure_data_tool/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:14:27.391088 procedure_data_tool-0.0.6/procedure_data_tool/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/__init__.py
+-rw-rw-rw-   0        0        0     4641 2024-05-15 21:42:42.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/docwriter.py
+-rw-rw-rw-   0        0        0     2693 2024-05-15 18:45:51.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/excelData.py
+-rw-rw-rw-   0        0        0     1054 2024-05-15 21:25:54.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/graph.py
+-rw-rw-rw-   0        0        0     2764 2024-05-15 21:29:01.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/node.py
+-rw-rw-rw-   0        0        0      531 2024-05-15 14:27:17.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/pit.py
+-rw-rw-rw-   0        0        0      504 2024-05-15 21:28:27.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/pump.py
+-rw-rw-rw-   0        0        0      479 2024-05-15 22:00:26.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/split.py
+-rw-rw-rw-   0        0        0      601 2024-05-15 21:28:41.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/tankreturn.py
+-rw-rw-rw-   0        0        0      497 2024-05-15 15:35:12.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/valve.py
+-rw-rw-rw-   0        0        0      606 2024-05-15 21:31:22.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/valve2.py
+-rw-rw-rw-   0        0        0     1171 2024-05-15 22:09:15.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/valve3.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:14:27.372393 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2024-05-15 22:14:27.393309 procedure_data_tool-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-05-15 20:49:25.000000 procedure_data_tool-0.0.6/setup.py
```

### Comparing `procedure_data_tool-0.0.4/procedure_data_tool/excelData.py` & `procedure_data_tool-0.0.6/procedure_data_tool/utils/excelData.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 globals().clear()
 from openpyxl import load_workbook
-from classes.valve import Valve
-from classes.valve2 import Valve2
-from classes.valve3 import Valve3
-from classes.split import Split
-from classes.pump import Pump
-from classes.tankreturn import TankReturn
-from classes.pit import Pit
+from procedure_data_tool.utils.valve import Valve
+from procedure_data_tool.utils.valve2 import Valve2
+from procedure_data_tool.utils.valve3 import Valve3
+from procedure_data_tool.utils.split import Split
+from procedure_data_tool.utils.pump import Pump
+from procedure_data_tool.utils.tankreturn import TankReturn
+from procedure_data_tool.utils.pit import Pit
 
-def ImportComponents(filepath = '//hanford/data/sitedata/WasteTransferEng/Waste Transfer Engineering/1 Transfers/1C - Procedure Review Tools/MasterProcedureData.xlsx'):
+def importComponents(filepath = '//hanford/data/sitedata/WasteTransferEng/Waste Transfer Engineering/1 Transfers/1C - Procedure Review Tools/MasterProcedureData.xlsx'):
     try:
         wb = load_workbook(filename = filepath, data_only=True)
     except FileNotFoundError as e:
         raise e
     pits = {}
     for row in wb["Pits"].iter_rows(min_row=3, values_only= True):
         pit = row[1]
@@ -53,22 +53,20 @@
             None: Valve 
     }
 
     #key = EIN, value = component object
     inventory = {}
 
     cnx = wb['Connections']
-    conections_matrix=cnx["D3:F200"]
+    conections_matrix=cnx["G3:I200"]
 
     for row in cnx.iter_rows(min_row=3, values_only= True):
-        component = row[1]
-        component_type = row[2]
-        inventory[component] = component_types[component_type](component)
-        inventory[component].setPit(row[6])
-        inventory[component].setJumper(row[7])
+        name = row[1]
+        type = row[2]
+        inventory[name] = component_types[type](name, pit = row[3], jumper = row[4], dvi = row[5])
 
     for component, connections in zip(inventory.values(), conections_matrix):
         for connection in connections:
             if connection.value in inventory:
                 if connection.value:
                     component.connect(inventory[connection.value])
```

### Comparing `procedure_data_tool-0.0.4/procedure_data_tool/main.py` & `procedure_data_tool-0.0.6/procedure_data_tool/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from classes.docwriter import DocWriter 
-import excelData as ex
+from procedure_data_tool.utils.docwriter import DocWriter 
+import procedure_data_tool.utils.excelData as ex
+import procedure_data_tool.utils.graph as gr
 import tkinter as tk
 from tkinter import messagebox
 from tkinter import filedialog
 
 import os
 
-def makeDocumentFromRoute(source, destination, alternatives = 1):
+def find_routes(source, destination, alternatives = 1):
     src = source.get()
     dst = destination.get()
     alts = 1
     try:
         alts = int(alternatives)
     except ValueError:
         messagebox.showwarning("Warning", "Valid number of alternatives not specified, showing shortest route available.")
     writer = DocWriter(src + " to " + dst + " draft procedure data:")
     #route is found here:
     routes = components[src].routesTo(components[dst], alts)
-    #change this to use a selected route from the options instead!
+    #change this to use a selected route from a list of route options instead!
+    gr.makeGraph(components, routes[0])
     for route in routes:
         for i in range(1,len(route)-2):
             route[i].setPosition(route)
         writer.buildDocument(route,pits)
     filename = src +"_to_"+ dst + ".docx"
     writer.save(filename)
     os.system(f'start {filename}')
+    
 
 def src_filter(*args):
     query = src_entry.get().lower() 
     src_dropdown['menu'].delete(0, tk.END)
     for node in nodes:
         # if query in node.lower() and (components[node].in_tank or select_from_all):
         if query in node.lower():
@@ -38,27 +41,51 @@
     query = dst_entry.get().lower() 
     dst_dropdown['menu'].delete(0, tk.END)
     for node in nodes:
         # if query in node.lower() and (components[node].in_tank or select_from_all):
         if query in node.lower():
             dst_dropdown['menu'].add_command(label=node, command=tk._setit(destination, node))
 
+def browse_file(*args):
+    filename = filedialog.askopenfilename(defaultextension="xlsx", title = "Select Procedure Data Excel file")
+    return filename
+
+def load_new_file(*args):
+    new_file_path = None
+    try:
+        new_file_path = browse_file()
+        if (new_file_path):
+            header_message.set("Using data from: "+ new_file_path)
+            components, pits =  ex.importComponents(new_file_path)
+    except:
+        messagebox.warning("Warning", "File not supported")
+        return
+
 def main():
     window = tk.Tk()
     window.title("Waste Transfer Procedure Data Tool")
-    filename = '//hanford/data/sitedata/WasteTransferEng/Waste Transfer Engineering/1 Transfers/1C - Procedure Review Tools/MasterProcedureData.xlsx'
+    global file_path
+    file_path = '//hanford/data/sitedata/WasteTransferEng/Waste Transfer Engineering/1 Transfers/1C - Procedure Review Tools/MasterProcedureData.xlsx'
     global components
     global pits 
     try: 
-        components, pits =  ex.ImportComponents(filename)
+        components, pits =  ex.importComponents(file_path)
     except Exception as e:
-        filewarning ="Unable to find file at:\n\n" + filename + "\n\n Please browse for Excel data file"
+        filewarning ="Unable to find file at:\n\n" + file_path + "\n\n Please browse for Excel data file"
         messagebox.showwarning("Warning", filewarning)
-        filename = filedialog.askopenfilename(defaultextension="xlsx" ,title = "Select Procedure Data Excel file")
-        components, pits =  ex.ImportComponents(filename)
+        components, pits =  ex.importComponents(browse_file())
+    
+    global header_message 
+    header_message = tk.StringVar()
+    header_message.set("Using data from: "+ file_path)
+    label3 = tk.Label(window, textvariable = header_message, wraplength=400, anchor="w")
+    label3.grid(row = 0, columnspan=3, rowspan=1, padx=10, pady=20,sticky = "w")
+
+    file_button = tk.Button(window, text= "Use a different file", command=lambda: load_new_file())
+    file_button.grid(row = 0, column = 4, padx= 10)
 
     def toggle_boolean(*args):
         if select_from_all:
             nodes = components.keys()
             for node in nodes:
                 # dst_dropdown['menu'].delete(0, tk.END)
                 src_dropdown['menu'].add_command(label=node, command=tk._setit(source, node))
@@ -72,58 +99,57 @@
         if components[item].in_tank:
             items_to_tank.add(item)
     
     global nodes 
     nodes = items_to_tank
 
     label0 = tk.Label(window, text="Select transfer origin:")
-    label0.grid(row=0, column= 0, pady = 2, padx=10,sticky = "w")
+    label0.grid(row=2, column= 0, pady = 2, padx=10,sticky = "w")
 
     global source
     source = tk.StringVar(window)
     global src_dropdown
     src_dropdown = tk.OptionMenu(window, source, *nodes)
-    src_dropdown.grid(row=0, column= 2, pady=2)
+    src_dropdown.grid(row=2, column= 2, pady=2)
     global src_entry
     src_entry = tk.Entry(window)
-    src_entry.grid(row=0, column= 1, pady=5, padx=4)
+    src_entry.grid(row=2, column= 1, pady=5, padx=4, sticky="w")
 
     label1 = tk.Label(window, text="Select transfer destination:")
-    label1.grid(row=2, column= 0, pady = 2, padx=10, sticky = "w")
+    label1.grid(row=3, column= 0, pady = 2, padx=10, sticky = "w")
 
     global destination
     destination = tk.StringVar(window)
     global dst_dropdown
     dst_dropdown = tk.OptionMenu(window, destination, *nodes)
-    dst_dropdown.grid(row=2, column= 2, pady=2)
+    dst_dropdown.grid(row=3, column= 2, pady=2)
     global dst_entry
     dst_entry = tk.Entry(window)
-    dst_entry.grid(row=2, column= 1, pady=5, padx=4)
+    dst_entry.grid(row=3, column= 1, pady=5, padx=4, sticky="w")
 
     global select_from_all
     select_from_all = tk.BooleanVar()
     select_from_all.set(False)
 
-    checkbox = tk.Checkbutton(window, text="Include Valves", variable=select_from_all, command = toggle_boolean)
-    checkbox.grid(row=0, column=4)
+    checkbox = tk.Checkbutton(window, text="Show valves", variable=select_from_all, command = toggle_boolean)
+    checkbox.grid(row=2, column=4)
 
     label2 = tk.Label(window, text="Number of route alternatives:")
-    label2.grid(row=4, column= 0, pady = 5, padx=10, sticky = "w")
+    label2.grid(row=5, column= 0, pady = 5, padx=10, sticky = "w")
 
     global alternatives 
-    alternatives = tk.Entry(window)
-    alternatives.grid(row=4, column= 1, columnspan=1, pady=2)
-
-    label3 = tk.Label(window, text= "Using data from: "+ filename, wraplength=600)
-    label3.grid(row = 5, columnspan=9, rowspan=3, padx=10, pady=20,sticky = "n")
+    alternatives = tk.Entry(window, width= 7, relief="groove")
+    alternatives.insert(0, "1") 
+    alternatives.grid(row=5, column= 1, columnspan=1, padx=4, pady=2, sticky="w")
+   
+    find_routes_button = tk.Button(window, text="Find routes", command=lambda: find_routes(source, destination, alternatives.get()))
+    find_routes_button.grid(row=5, column= 4, padx = 10, pady=15)
 
     src_entry.bind("<KeyRelease>", src_filter)
     dst_entry.bind("<KeyRelease>", dst_filter)
 
-    printButton = tk.Button(window, text="Find Routes", command=lambda: makeDocumentFromRoute(source, destination, alternatives.get()))
-    printButton.grid(row=4, column= 2, pady=5)
     window.mainloop()
 
 if __name__== '__main__':   
     main()
 
 # TO DO: FIGURE OUT DVI, FIGURE OUT SPLITS NECESSARY??
```

