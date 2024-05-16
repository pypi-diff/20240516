# Comparing `tmp/inception_reports-0.2.tar.gz` & `tmp/inception_reports-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inception_reports-0.2.tar", last modified: Tue May  7 01:02:34 2024, max compression
+gzip compressed data, was "inception_reports-0.3.tar", last modified: Wed May 15 12:08:50 2024, max compression
```

## Comparing `inception_reports-0.2.tar` & `inception_reports-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-07 01:02:34.953213 inception_reports-0.2/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    11357 2023-09-25 12:56:28.000000 inception_reports-0.2/LICENSE
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      752 2023-11-07 13:15:00.000000 inception_reports-0.2/NOTICE.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2073 2024-05-07 01:02:34.953213 inception_reports-0.2/PKG-INFO
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1376 2024-04-30 00:10:18.000000 inception_reports-0.2/README.md
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-07 01:02:34.953213 inception_reports-0.2/inception_reports/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-04-02 01:14:36.000000 inception_reports-0.2/inception_reports/__init__.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1704 2024-04-29 23:24:38.000000 inception_reports-0.2/inception_reports/__main__.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     7094 2024-04-29 23:24:38.000000 inception_reports-0.2/inception_reports/generate_reports_lead.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    14011 2024-05-07 01:00:49.000000 inception_reports-0.2/inception_reports/generate_reports_manager.py
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-07 01:02:34.953213 inception_reports-0.2/inception_reports.egg-info/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2073 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/PKG-INFO
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      515 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/SOURCES.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)        1 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/dependency_links.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       70 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/entry_points.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       56 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/requires.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       18 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/top_level.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      802 2024-05-07 01:02:30.000000 inception_reports-0.2/pyproject.toml
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       38 2024-05-07 01:02:34.953213 inception_reports-0.2/setup.cfg
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-07 01:02:34.953213 inception_reports-0.2/tests/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     3551 2024-04-29 23:24:38.000000 inception_reports-0.2/tests/test_generate_reports_lead.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     4262 2024-05-07 01:00:49.000000 inception_reports-0.2/tests/test_generate_reports_manager.py
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-15 12:08:50.084482 inception_reports-0.3/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    11357 2023-09-25 12:56:28.000000 inception_reports-0.3/LICENSE
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      752 2023-11-07 13:15:00.000000 inception_reports-0.3/NOTICE.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2063 2024-05-15 12:08:50.084482 inception_reports-0.3/PKG-INFO
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1376 2024-04-30 00:10:18.000000 inception_reports-0.3/README.md
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-15 12:08:50.080482 inception_reports-0.3/inception_reports/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-04-02 01:14:36.000000 inception_reports-0.3/inception_reports/__init__.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1704 2024-04-29 23:24:38.000000 inception_reports-0.3/inception_reports/__main__.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     6889 2024-05-15 10:52:10.000000 inception_reports-0.3/inception_reports/generate_reports_lead.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    17113 2024-05-15 10:59:21.000000 inception_reports-0.3/inception_reports/generate_reports_manager.py
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-15 12:08:50.084482 inception_reports-0.3/inception_reports.egg-info/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2063 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/PKG-INFO
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      515 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)        1 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       70 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/entry_points.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       52 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/requires.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       18 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/top_level.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      792 2024-05-15 12:08:08.000000 inception_reports-0.3/pyproject.toml
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       38 2024-05-15 12:08:50.084482 inception_reports-0.3/setup.cfg
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-15 12:08:50.084482 inception_reports-0.3/tests/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     3565 2024-05-15 09:37:35.000000 inception_reports-0.3/tests/test_generate_reports_lead.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     4262 2024-05-07 01:00:49.000000 inception_reports-0.3/tests/test_generate_reports_manager.py
```

### Comparing `inception_reports-0.2/LICENSE` & `inception_reports-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inception_reports-0.2/NOTICE.txt` & `inception_reports-0.3/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `inception_reports-0.2/PKG-INFO` & `inception_reports-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: inception_reports
-Version: 0.2
+Version: 0.3
 Summary: Generate plots that report the progress of an INCEpTION project.
-Author-email: Serwar Basch <serwar.basch@tu-darmstadt.de>
+Author-email: Serwar <serwar.basch@tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/inception-project/inception-reporting-dashboard
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
 Requires-Dist: streamlit
 Requires-Dist: pandas
-Requires-Dist: matplotlib
+Requires-Dist: plotly
 Requires-Dist: numpy
 Requires-Dist: dkpro-cassis
 Requires-Dist: pycaprio
 
 # INCEpTION Reporting Dashboard
 
 This package will generate plots to track the progress of your INCEpTION project(s).
```

### Comparing `inception_reports-0.2/README.md` & `inception_reports-0.3/README.md`

 * *Files identical despite different names*

### Comparing `inception_reports-0.2/inception_reports/__init__.py` & `inception_reports-0.3/inception_reports/__init__.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.2/inception_reports/__main__.py` & `inception_reports-0.3/inception_reports/__main__.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.2/inception_reports/generate_reports_manager.py` & `inception_reports-0.3/inception_reports/generate_reports_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,214 +10,135 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
 import json
 import os
 import shutil
-import warnings
+import time
 import zipfile
+from datetime import datetime
 
 import cassis
-import matplotlib.pyplot as plt
-import numpy as np
+import pandas as pd
+import plotly.express as px
+import plotly.graph_objects as go
 import streamlit as st
-from matplotlib import gridspec
 from pycaprio import Pycaprio
-from datetime import datetime
+import importlib.resources
 
-# suppress deprecation warnings related to the use of the pyplot
-# can be solved by sending the fig instead of the plt to streamlit
-st.set_option("deprecation.showPyplotGlobalUse", False)
-st.set_page_config(page_title="INCEpTION Reporting Dashboard", layout="centered")
-css = """
-<style>
-    section.main > div {max-width:50%}
-</style>
-"""
-st.markdown(css, unsafe_allow_html=True)
-warnings.filterwarnings(
-    "ignore", message="Boolean Series key will be reindexed to match DataFrame index"
+st.set_page_config(
+    page_title="INCEpTION Reporting Dashboard",
+    layout="centered",
+    initial_sidebar_state=st.session_state.setdefault("sidebar_state", "expanded"),
 )
 
-
-def plot_project_progress(project) -> None:
-    """
-    Generate a visual representation of project progress based on a DataFrame of log data.
-
-    This function takes a DataFrame containing log data and generates
-    visualizations to represent the progress of different documents. It calculates the
-    total time spent on each document, divides it into sessions based on a specified
-    threshold, and displays a pie chart showing the percentage of finished and remaining
-    documents, along with a bar chart showing the total time spent on finished documents
-    compared to the estimated time for remaining documents.
-
-    Parameters:
-        project (dict): A dict containing project information, namely the name, tags, annotations, and logs.
-
-    """
-
-    # df = project["logs"]
-    project_name = project["name"].strip(".zip")
-    project_tags = project["tags"]
-    project_annotations = project["annotations"]
-    project_documents = project["documents"]
-
-    doc_categories = {
-        "ANNOTATION_IN_PROGRESS": 0,
-        "ANNOTATION_FINISHED": 0,
-        "CURATION_IN_PROGRESS": 0,
-        "CURATION_FINISHED": 0,
-        "NEW": 0,
-    }
-
-    for doc in project_documents:
-        state = doc["state"]
-        if state in doc_categories:
-            doc_categories[state] += 1
-
-    project_data = {
-        "project_name": project_name,
-        "project_tags": project_tags,
-        "doc_categories": doc_categories,
-    }
-
-
-
-    type_counts = get_type_counts(project_annotations)
-    selected_annotation_types = st.multiselect(
-        f"Which annotation types would you like to see for {project_name}?",
-        list(type_counts.keys()),
-        list(type_counts.keys())
-    )
-    type_counts = {k: v for k, v in type_counts.items() if k in selected_annotation_types}
-
-    data_sizes = [
-        project_data["doc_categories"]["NEW"],
-        project_data["doc_categories"]["ANNOTATION_IN_PROGRESS"],
-        project_data["doc_categories"]["ANNOTATION_FINISHED"],
-        project_data["doc_categories"]["CURATION_IN_PROGRESS"],
-        project_data["doc_categories"]["CURATION_FINISHED"],
-    ]
-
-    pie_labels = [
-        "New",
-        "Annotation In Progress",
-        "Annotation Finished",
-        "Curation In Progress",
-        "Curation Finished",
-    ]
-    pie_colors = [
-        "tab:red",
-        "cornflowerblue",
-        "royalblue",
-        "limegreen",
-        "forestgreen",
-    ]
-    pie_percentages = 100.0 * np.array(data_sizes) / np.array(data_sizes).sum()
-    fig = plt.figure(figsize=(15, 9))
-    gs = gridspec.GridSpec(1, 3, width_ratios=[1, 0.01, 1])
-
-    ax1 = plt.subplot(gs[0])
-
-    wedges, _ = ax1.pie(
-        data_sizes, colors=pie_colors, startangle=90, radius=2, counterclock=False
-    )
-
-    ax1.axis("equal")
-    total_annotations = sum(
-        [len(cas_file.select_all()) for cas_file in project_annotations.values()]
+if st.session_state.get("flag"):
+    st.session_state.sidebar_state = st.session_state.flag
+    del st.session_state.flag
+    time.sleep(0.01)
+    st.rerun()
+
+
+def startup():
+
+    st.markdown(
+        """
+        <style>
+        body {
+            cursor: url('https://cdn-icons-png.flaticon.com/64/5198/5198523.png'), auto !important;
+        }
+
+        rect.legendtoggle {
+            cursor: url('https://cdn-icons-png.flaticon.com/32/12179/12179477.png'), pointer !important;
+        }
+
+        rect.nsewdrag.drag {
+            cursor: url('https://cdn-icons-png.flaticon.com/32/10263/10263093.png'), pointer !important;
+        }
+        </style>
+
+        <style>
+        .block-container {
+            padding-top: 0rem;
+            padding-bottom: 5rem;
+            padding-left: 5rem;
+            padding-right: 5rem;
+        }
+        </style>
+
+        <style>
+        div[data-testid="stHorizontalBlock"] {
+            margin-top: 1rem;
+            border: thick double #999999;
+            box-shadow: 0px 0px 10px #999999;
+        }
+        </style>
+
+        <style>
+        section.main > div {max-width:90%}
+        </style>
+        """,
+        unsafe_allow_html=True,
     )
-    ax1.set_title("Documents Status")
 
-    legend_labels = [
-        f"{label} ({percent:.2f}% / {size} files)"
-        for label, size, percent in zip(pie_labels, data_sizes, pie_percentages)
-    ]
-    ax1.legend(
-        wedges,
-        legend_labels,
-        title="Categories",
-        loc="center left",
-        bbox_to_anchor=(1, 0.5),
-    )
-
-    ax2 = plt.subplot(gs[2])
-    colors = plt.cm.tab10(range(len(type_counts.keys())))
-    ax2.set_title("Types of Annotations")
-    ax2.barh(
-        [f"{type} = {value}" for type, value in type_counts.items()],
-        list(type_counts.values()),
-        color=colors,
-    )
-    ax2.set_xlabel("Number of Annotations")
-    
-    fig.suptitle(
-        f'{project_name.split(".")[0]}\nTotal Annotations: {total_annotations}',
-        fontsize=16,
-    )
-    fig.tight_layout()
-    st.pyplot()
-
-    export_data(project_data)
 
-
-def find_element_by_name(element_list, name):
+def create_directory_in_home():
     """
-    Finds an element in the given element list by its name.
-
-    Args:
-        element_list (list): A list of elements to search through.
-        name (str): The name of the element to find.
-
-    Returns:
-        str: The UI name of the found element, or the last part of the name if not found.
+    Creates a directory in the user's home directory for storing Inception reports imported over the API.
     """
-    for element in element_list:
-        if element.name == name:
-            return element.uiName
-    return name.split(".")[-1]
+    home_dir = os.path.expanduser("~")
+    new_dir_path = os.path.join(home_dir, ".inception_reports")
+    try:
+        os.makedirs(new_dir_path)
+        os.makedirs(os.path.join(new_dir_path, "projects"))
+    except FileExistsError:
+        pass
 
 
-def get_type_counts(annotations):
-    """
-    Calculate the count of each type in the given annotations. Each annotation is a CAS object.
+def set_sidebar_state(value):
+    if st.session_state.sidebar_state == value:
+        st.session_state.flag = value
+        st.session_state.sidebar_state = (
+            "expanded" if value == "collapsed" else "collapsed"
+        )
+    else:
+        st.session_state.sidebar_state = value
+    st.rerun()
 
-    Args:
-        annotations (dict): A dictionary containing the annotations.
 
-    Returns:
-        dict: A dictionary containing the count of each type.
+def translate_tag(tag, translation_path=None):
+    """
+    Translate the given tag to a human-readable format.
     """
-    count_dict = {}
-
-    layerDefinition = annotations.popitem()[1].select(
-        "de.tudarmstadt.ukp.clarin.webanno.api.type.LayerDefinition"
-    )
-    for doc in annotations:
-        type_names = [
-            (
-                find_element_by_name(layerDefinition, t.name),
-                len(annotations[doc].select(t.name)),
-            )
-            for t in annotations[doc].typesystem.get_types()
-            if t.name != "de.tudarmstadt.ukp.clarin.webanno.api.type.LayerDefinition"
-        ]
-
-        for type_name, count in type_names:
-            if type_name not in count_dict:
-                count_dict[type_name] = 0
-            count_dict[type_name] += count
-    count_dict = {k: v for k, v in count_dict.items() if v > 0}
-    count_dict = dict(sorted(count_dict.items(), key=lambda item: item[1]))
 
-    return count_dict
+    if translation_path:
+        with open(translation_path, "r") as f:
+            translation = json.load(f)
+        if tag in translation:
+            return translation[tag]
+        else:
+            return tag
+    else:
+        data_path = importlib.resources.files('inception_reports.data')
+        with open(data_path.joinpath("specialties.json"), "r") as f:
+            specialties = json.load(f)
+        with open(data_path.joinpath("document_types.json"), "r") as f:
+            document_types = json.load(f)
+
+        if tag in specialties:
+            return specialties[tag]
+        elif tag in document_types:
+            return document_types[tag]
+        else:
+            return tag
 
 
 def read_dir(dir_path: str) -> list[dict]:
     """
     Reads a directory containing zip files, extracts the contents, and retrieves project metadata and annotations.
 
     Args:
@@ -241,15 +162,15 @@
 
                 # Find project metadata file
                 project_meta_path = os.path.join(zip_path, "exportedproject.json")
                 if os.path.exists(project_meta_path):
                     with open(project_meta_path, "r") as project_meta_file:
                         project_meta = json.load(project_meta_file)
                         project_tags = [
-                            word.strip("#")
+                            translate_tag(word.strip("#"))
                             for word in project_meta["description"].split()
                             if word.startswith("#")
                         ]
                         project_documents = project_meta["source_documents"]
 
                 annotations = {}
                 # Find annotation folders
@@ -277,15 +198,14 @@
 
                 # Clean up extracted files
                 shutil.rmtree(zip_path)
 
     return projects
 
 
-
 def login_to_inception(api_url, username, password):
     """
     Logs in to the Inception API using the provided API URL, username, and password.
 
     Args:
         api_url (str): The URL of the Inception API.
         username (str): The username for authentication.
@@ -293,101 +213,310 @@
 
     Returns:
         tuple: A tuple containing a boolean value indicating whether the login was successful and an instance of the Inception client.
 
     """
     if "http" not in api_url:
         api_url = f"http://{api_url}"
-    if st.sidebar.button("Login"):
+    button = st.sidebar.button("Login")
+    if button:
         inception_client = Pycaprio(api_url, (username, password))
         st.sidebar.success("Login successful ✅")
+        button = False
         return True, inception_client
     return False, None
 
 
-
 def select_method_to_import_data():
     """
     Allows the user to select a method to import data for generating reports.
     """
-    
-    method = st.sidebar.radio("Choose your method to import data:", ('Manually', 'API'), index=0)
 
-    if method == 'Manually':
-        st.sidebar.write("Please input the path to the folder containing the INCEpTION projects.")
-        projects_folder = st.sidebar.text_input("Projects Folder:", value="data/dresden_projects/")
-        if st.sidebar.button("Generate Reports"):
-            st.session_state['initialized'] = True
-            st.session_state['method'] = 'Manually'
-            st.session_state['projects_folder'] = projects_folder
-    elif method == 'API':
+    method = st.sidebar.radio(
+        "Choose your method to import data:", ("Manually", "API"), index=0
+    )
+
+    if method == "Manually":
+        st.sidebar.write(
+            "Please input the path to the folder containing the INCEpTION projects."
+        )
+        projects_folder = st.sidebar.text_input(
+            "Projects Folder:", value="data/gemtex_demo_projects/"
+        )
+        button = st.sidebar.button("Generate Reports")
+        if button:
+            st.session_state["initialized"] = True
+            st.session_state["method"] = "Manually"
+            st.session_state["projects"] = read_dir(projects_folder)
+            button = False
+            set_sidebar_state("collapsed")
+    elif method == "API":
         api_url = st.sidebar.text_input("Enter API URL:", "")
         username = st.sidebar.text_input("Username:", "")
         password = st.sidebar.text_input("Password:", type="password", value="")
-        inception_status, inception_client = login_to_inception(api_url, username, password)
+        inception_status, inception_client = login_to_inception(
+            api_url, username, password
+        )
         if inception_status:
             inception_projects = inception_client.api.projects()
             st.sidebar.write("Following projects got imported:")
             for inception_project in inception_projects:
                 st.sidebar.write(inception_project.project_name)
-                project_export = inception_client.api.export_project(inception_project, "jsoncas")
-                with open(f"{os.path.expanduser('~')}/.inception_reports/projects/{inception_project}.zip", "wb") as f:
+                project_export = inception_client.api.export_project(
+                    inception_project, "jsoncas"
+                )
+                with open(
+                    f"{os.path.expanduser('~')}/.inception_reports/projects/{inception_project}.zip",
+                    "wb",
+                ) as f:
                     f.write(project_export)
-            st.session_state['initialized'] = True
-            st.session_state['method'] = 'API'
-            st.session_state['projects_folder'] = f"{os.path.expanduser('~')}/.inception_reports/projects"
+            st.session_state["initialized"] = True
+            st.session_state["method"] = "API"
+            st.session_state["projects"] = read_dir(projects_folder)
+            set_sidebar_state("collapsed")
+
+
+def find_element_by_name(element_list, name):
+    """
+    Finds an element in the given element list by its name.
 
+    Args:
+        element_list (list): A list of elements to search through.
+        name (str): The name of the element to find.
 
+    Returns:
+        str: The UI name of the found element, or the last part of the name if not found.
+    """
+    for element in element_list:
+        if element.name == name:
+            return element.uiName
+    return name.split(".")[-1]
 
-def create_directory_in_home():
+
+def get_type_counts(annotations):
     """
-    Creates a directory in the user's home directory for storing Inception reports imported over the API.
+    Calculate the count of each type in the given annotations. Each annotation is a CAS object.
+
+    Args:
+        annotations (dict): A dictionary containing the annotations.
+
+    Returns:
+        dict: A dictionary containing the count of each type.
     """
-    home_dir = os.path.expanduser("~")
-    new_dir_path = os.path.join(home_dir, ".inception_reports")
-    try:
-        os.makedirs(new_dir_path)
-        os.makedirs(os.path.join(new_dir_path, "projects"))
-    except FileExistsError:
-        pass
+    count_dict = {}
+
+    layerDefinition = annotations.popitem()[1].select(
+        "de.tudarmstadt.ukp.clarin.webanno.api.type.LayerDefinition"
+    )
+    for doc in annotations:
+        type_names = [
+            (
+                find_element_by_name(layerDefinition, t.name),
+                len(annotations[doc].select(t.name)),
+            )
+            for t in annotations[doc].typesystem.get_types()
+            if t.name != "de.tudarmstadt.ukp.clarin.webanno.api.type.LayerDefinition"
+        ]
+
+        for type_name, count in type_names:
+            if type_name not in count_dict:
+                count_dict[type_name] = 0
+            count_dict[type_name] += count
+    count_dict = {k: v for k, v in count_dict.items() if v > 0}
+    count_dict = dict(sorted(count_dict.items(), key=lambda item: item[1]))
+
+    return count_dict
 
 
 def export_data(project_data, output_directory=None):
     """
     Export project data to a JSON file, and store it in a directory named after the project and the current date.
 
     Parameters:
         project_data (dict): The data to be exported.
     """
     current_date = datetime.now().strftime("%Y_%m_%d")
-    directory_name = f'exported_data_{current_date}'
+    directory_name = f"exported_data_{current_date}"
 
     if output_directory is None:
         output_directory = os.path.join(os.getcwd(), directory_name)
     else:
         output_directory = os.path.join(output_directory, directory_name)
-    
+
     if not os.path.exists(output_directory):
         os.makedirs(output_directory)
 
     project_name = project_data["project_name"]
-    with open(f"{output_directory}/{project_name.split('.')[0]}_data_{current_date}.json", "w") as output_file:
+    with open(
+        f"{output_directory}/{project_name.split('.')[0]}_data_{current_date}.json", "w"
+    ) as output_file:
         json.dump(project_data, output_file, indent=4)
-    st.success(f"{project_name.split('.')[0]} documents status exported successfully ✅")
+    st.success(
+        f"{project_name.split('.')[0]} documents status exported successfully ✅"
+    )
+
+
+def plot_project_progress(project) -> None:
+    """
+    Generate a visual representation of project progress based on a DataFrame of log data.
+
+    This function takes a DataFrame containing log data and generates
+    visualizations to represent the progress of different documents. It calculates the
+    total time spent on each document, divides it into sessions based on a specified
+    threshold, and displays a pie chart showing the percentage of finished and remaining
+    documents, along with a bar chart showing the total time spent on finished documents
+    compared to the estimated time for remaining documents.
+
+    Parameters:
+        project (dict): A dict containing project information, namely the name, tags, annotations, and logs.
+
+    """
+
+    st.write(
+        f"<div style='text-align: center; font-size: 18px;'><b>Project Name</b>: {project['name']} <br> <b>Tags</b>: {', '.join(project['tags'])}</div>",
+        unsafe_allow_html=True,
+    )
+
+    # df = project["logs"]
+    project_name = project["name"].strip(".zip")
+    project_tags = project["tags"]
+    project_annotations = project["annotations"]
+    project_documents = project["documents"]
+
+    doc_categories = {
+        "ANNOTATION_IN_PROGRESS": 0,
+        "ANNOTATION_FINISHED": 0,
+        "CURATION_IN_PROGRESS": 0,
+        "CURATION_FINISHED": 0,
+        "NEW": 0,
+    }
+
+    for doc in project_documents:
+        state = doc["state"]
+        if state in doc_categories:
+            doc_categories[state] += 1
+
+    project_data = {
+        "project_name": project_name,
+        "project_tags": project_tags,
+        "doc_categories": doc_categories,
+    }
+
+    type_counts = get_type_counts(project_annotations)
+
+    data_sizes = [
+        project_data["doc_categories"]["NEW"],
+        project_data["doc_categories"]["ANNOTATION_IN_PROGRESS"],
+        project_data["doc_categories"]["ANNOTATION_FINISHED"],
+        project_data["doc_categories"]["CURATION_IN_PROGRESS"],
+        project_data["doc_categories"]["CURATION_FINISHED"],
+    ]
+
+    pie_labels = [
+        "New",
+        "Annotation In Progress",
+        "Annotation Finished",
+        "Curation In Progress",
+        "Curation Finished",
+    ]
+
+    df_pie = pd.DataFrame({"Labels": pie_labels, "Sizes": data_sizes}).sort_values(
+        by="Labels", ascending=True
+    )
+
+    df_bar = pd.DataFrame(
+        {
+            "Types": [type for type, _ in type_counts.items()],
+            "Counts": list(type_counts.values()),
+        }
+    )
+
+    pie_chart = go.Figure(
+        go.Pie(
+            labels=df_pie['Labels'],
+            values=df_pie['Sizes'],
+            sort=False,
+            hole=0.4,
+            hoverinfo="label+value"
+        )
+    )
+
+    pie_chart.update_layout(
+        title=dict(
+            text="Documents Status",
+            font=dict(size=24),
+            y=0.95,
+            x=0.5,
+            xanchor="center",
+        ),
+        font=dict(size=18),
+        legend=dict(font=dict(size=12), y=0.5),
+        paper_bgcolor="rgba(0,0,0,0)",
+        plot_bgcolor="rgba(0,0,0,0)",
+        margin=dict(l=40, r=40)
+    )
+
+    bar_chart = go.Figure()
+
+    for _, row in df_bar.iterrows():
+        bar_chart.add_trace(
+            go.Bar(
+                y=[row["Types"]],
+                x=[row["Counts"]],
+                orientation="h",
+                name=row["Types"],
+                legendgroup=row["Types"],
+                showlegend=True,
+                hoverinfo="x+y"
+            )
+        )
+
+    bar_chart.update_layout(
+        title=dict(
+            text="Types of Annotations",
+            font=dict(size=24),
+            y=0.95,
+            x=0.45,
+            xanchor="center",
+        ),
+        xaxis_title="Number of Annotations",
+        barmode="overlay",
+        height=50 * len(df_bar),
+        font=dict(size=18),
+        legend=dict(font=dict(size=12)),
+        paper_bgcolor="rgba(0,0,0,0)",
+        plot_bgcolor="rgba(0,0,0,0)",
+        margin=dict(l=40, r=40),
+        colorway=px.colors.qualitative.Plotly,
+    )
+
+    col1, _, col3 = st.columns([1, 0.1, 1])
+    with col1:
+        st.plotly_chart(pie_chart, use_container_width=True)
+    with col3:
+        st.plotly_chart(bar_chart, use_container_width=True)
+
+    export_data(project_data)
+
 
 def main():
+    startup()
     create_directory_in_home()
-    
-    st.title("INCEpTION Projects Statistics")
 
-    if 'initialized' not in st.session_state:
-        select_method_to_import_data()
+    st.write(
+        "<style> h1 {text-align: center; margin-bottom: 50px, } </style>",
+        unsafe_allow_html=True,
+    )
+    st.title("INCEpTION Reporting Dashboard")
+    st.write("<hr>", unsafe_allow_html=True)
+
+    select_method_to_import_data()
 
-    if 'method' in st.session_state:
-        projects = read_dir(st.session_state.projects_folder)
-        projects.sort(key=lambda x: x["name"])
+    if "method" in st.session_state and "projects" in st.session_state:
+        projects = [copy.deepcopy(project) for project in st.session_state["projects"]]
+        projects = sorted(projects, key=lambda x: x["name"])
         for project in projects:
             plot_project_progress(project)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `inception_reports-0.2/inception_reports.egg-info/PKG-INFO` & `inception_reports-0.3/inception_reports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: inception_reports
-Version: 0.2
+Version: 0.3
 Summary: Generate plots that report the progress of an INCEpTION project.
-Author-email: Serwar Basch <serwar.basch@tu-darmstadt.de>
+Author-email: Serwar <serwar.basch@tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/inception-project/inception-reporting-dashboard
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
 Requires-Dist: streamlit
 Requires-Dist: pandas
-Requires-Dist: matplotlib
+Requires-Dist: plotly
 Requires-Dist: numpy
 Requires-Dist: dkpro-cassis
 Requires-Dist: pycaprio
 
 # INCEpTION Reporting Dashboard
 
 This package will generate plots to track the progress of your INCEpTION project(s).
```

### Comparing `inception_reports-0.2/inception_reports.egg-info/SOURCES.txt` & `inception_reports-0.3/inception_reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inception_reports-0.2/pyproject.toml` & `inception_reports-0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inception_reports"
 description = "Generate plots that report the progress of an INCEpTION project."
-version = "0.2"
+version = "0.3"
 authors = [
-    { name = "Serwar Basch", email = "serwar.basch@tu-darmstadt.de" }
+    { name = "Serwar", email = "serwar.basch@tu-darmstadt.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
     "streamlit",
     "pandas",
-    "matplotlib",
+    "plotly",
     "numpy",
     "dkpro-cassis",
     "pycaprio",
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `inception_reports-0.2/tests/test_generate_reports_lead.py` & `inception_reports-0.3/tests/test_generate_reports_lead.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from unittest.mock import MagicMock, patch
 
-from inception_reports.generate_reports_lead import get_unique_tags, plot_project_progress, read_dir
+from inception_reports.generate_reports_lead import get_unique_tags, plot_multiples, read_dir
 
 
 def test_get_unique_tags():
     """
     Test case for the get_unique_tags function.
     
     This test case verifies that the get_unique_tags function returns the expected result
@@ -103,9 +103,9 @@
             "ANNOTATION_FINISHED": 5,
             "CURATION_IN_PROGRESS": 0,
             "CURATION_FINISHED": 0,
             "NEW": 4,
         },
     }
 
-    plot_project_progress(project_data)
+    plot_multiples([project_data], ["tag1", "tag2", "tag3"])
     assert True, "Should not raise any exceptions"
```

### Comparing `inception_reports-0.2/tests/test_generate_reports_manager.py` & `inception_reports-0.3/tests/test_generate_reports_manager.py`

 * *Files identical despite different names*

