# Comparing `tmp/grid2demand-0.4.2.tar.gz` & `tmp/grid2demand-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2demand-0.4.2.tar", last modified: Sat Apr 20 19:14:37 2024, max compression
+gzip compressed data, was "grid2demand-0.4.3.tar", last modified: Thu May 16 07:20:41 2024, max compression
```

## Comparing `grid2demand-0.4.2.tar` & `grid2demand-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.361894 grid2demand-0.4.2/
--rw-rw-rw-   0        0        0    11558 2023-09-29 02:14:48.000000 grid2demand-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     6317 2024-04-20 19:14:37.361894 grid2demand-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    26191 2024-01-21 21:55:25.000000 grid2demand-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.303118 grid2demand-0.4.2/grid2demand/
--rw-rw-rw-   0        0        0     1008 2024-04-20 19:13:27.000000 grid2demand-0.4.2/grid2demand/__init__.py
--rw-rw-rw-   0        0        0    27826 2024-03-31 03:45:37.000000 grid2demand-0.4.2/grid2demand/_grid2demand.py
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.354932 grid2demand-0.4.2/grid2demand/func_lib/
--rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.2/grid2demand/func_lib/__init__.py
--rw-rw-rw-   0        0        0     2548 2024-03-31 02:03:11.000000 grid2demand-0.4.2/grid2demand/func_lib/gen_agent_demand.py
--rw-rw-rw-   0        0        0    16730 2024-03-31 03:37:37.000000 grid2demand-0.4.2/grid2demand/func_lib/gen_zone.py
--rw-rw-rw-   0        0        0     3818 2024-03-31 02:02:08.000000 grid2demand-0.4.2/grid2demand/func_lib/gravity_model.py
--rw-rw-rw-   0        0        0    14881 2024-03-31 02:36:02.000000 grid2demand-0.4.2/grid2demand/func_lib/read_node_poi.py
--rw-rw-rw-   0        0        0     6994 2024-03-31 03:18:02.000000 grid2demand-0.4.2/grid2demand/func_lib/trip_rate_production_attraction.py
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.361894 grid2demand-0.4.2/grid2demand/utils_lib/
--rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.2/grid2demand/utils_lib/__init__.py
--rw-rw-rw-   0        0        0     6018 2024-03-27 02:20:39.000000 grid2demand-0.4.2/grid2demand/utils_lib/net_utils.py
--rw-rw-rw-   0        0        0     3348 2024-01-21 21:42:52.000000 grid2demand-0.4.2/grid2demand/utils_lib/pkg_settings.py
--rw-rw-rw-   0        0        0     9289 2024-03-27 01:31:34.000000 grid2demand-0.4.2/grid2demand/utils_lib/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.342119 grid2demand-0.4.2/grid2demand.egg-info/
--rw-rw-rw-   0        0        0     6317 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 19:14:37.369293 grid2demand-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1998 2024-04-20 19:14:01.000000 grid2demand-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.361894 grid2demand-0.4.2/tests/
--rw-rw-rw-   0        0        0      552 2024-03-01 23:27:53.000000 grid2demand-0.4.2/tests/test_read_node.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:20:41.245034 grid2demand-0.4.3/
+-rw-rw-rw-   0        0        0    11558 2023-09-29 02:14:48.000000 grid2demand-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     7792 2024-05-16 07:20:41.245034 grid2demand-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    34025 2024-05-16 07:17:35.000000 grid2demand-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 07:20:41.178980 grid2demand-0.4.3/grid2demand/
+-rw-rw-rw-   0        0        0     1689 2024-05-16 07:19:09.000000 grid2demand-0.4.3/grid2demand/__init__.py
+-rw-rw-rw-   0        0        0    53439 2024-05-15 21:11:09.000000 grid2demand-0.4.3/grid2demand/_grid2demand.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:20:41.239868 grid2demand-0.4.3/grid2demand/func_lib/
+-rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.3/grid2demand/func_lib/__init__.py
+-rw-rw-rw-   0        0        0     2548 2024-03-31 02:03:11.000000 grid2demand-0.4.3/grid2demand/func_lib/gen_agent_demand.py
+-rw-rw-rw-   0        0        0    20218 2024-05-15 19:53:14.000000 grid2demand-0.4.3/grid2demand/func_lib/gen_zone.py
+-rw-rw-rw-   0        0        0     4182 2024-05-15 19:53:14.000000 grid2demand-0.4.3/grid2demand/func_lib/gravity_model.py
+-rw-rw-rw-   0        0        0    18686 2024-05-15 19:53:14.000000 grid2demand-0.4.3/grid2demand/func_lib/read_node_poi.py
+-rw-rw-rw-   0        0        0     6991 2024-05-15 19:53:14.000000 grid2demand-0.4.3/grid2demand/func_lib/trip_rate_production_attraction.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:20:41.245034 grid2demand-0.4.3/grid2demand/utils_lib/
+-rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.3/grid2demand/utils_lib/__init__.py
+-rw-rw-rw-   0        0        0     6018 2024-03-27 02:20:39.000000 grid2demand-0.4.3/grid2demand/utils_lib/net_utils.py
+-rw-rw-rw-   0        0        0     3385 2024-05-15 19:53:14.000000 grid2demand-0.4.3/grid2demand/utils_lib/pkg_settings.py
+-rw-rw-rw-   0        0        0     9295 2024-05-15 19:53:14.000000 grid2demand-0.4.3/grid2demand/utils_lib/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:20:41.224750 grid2demand-0.4.3/grid2demand.egg-info/
+-rw-rw-rw-   0        0        0     7792 2024-05-16 07:20:40.000000 grid2demand-0.4.3/grid2demand.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-05-16 07:20:41.000000 grid2demand-0.4.3/grid2demand.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:20:40.000000 grid2demand-0.4.3/grid2demand.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-16 07:20:40.000000 grid2demand-0.4.3/grid2demand.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 07:20:40.000000 grid2demand-0.4.3/grid2demand.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:20:41.245034 grid2demand-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1998 2024-05-16 07:19:28.000000 grid2demand-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:20:41.245034 grid2demand-0.4.3/tests/
+-rw-rw-rw-   0        0        0      552 2024-03-01 23:27:53.000000 grid2demand-0.4.3/tests/test_read_node.py
```

### Comparing `grid2demand-0.4.2/LICENSE` & `grid2demand-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.2/README.md` & `grid2demand-0.4.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,378 +1,446 @@
-**Grid2demand**
 
-\*How to quickly generate **initial origin-destination transportation demand**
-for engaging traffic simulation games such as A/B street and DTALite?
-\*How to teach our undergraduate students the important **trip generation and
-trip distribution steps**, using their own beautiful campus as examples?
-\*How to analyze the resident locations and other land use properties using
-flexible **grid zones, based on POI data from OpenStreetMap** data and using
-**open transportation modeling format**
+- [**Grid2demand**](#grid2demand)
+  - [**Code Examples**](#code-examples)
+    - [**Installation**](#installation)
+    - [**Simple Example**](#simple-example)
+      - [**Generate Demand with node.csv and poi.csv**](#generate-demand-with-nodecsv-and-poicsv)
+      - [**Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)**](#generate-demand-with-nodecsv-poicsv-and-zonecsv-geometry-filed-in-zonecsv)
+      - [**Generate Demand with node.csv, poi.csv and zone.csv (x\_coord, y\_coord fields represent zone centroids)**](#generate-demand-with-nodecsv-poicsv-and-zonecsv-x_coord-y_coord-fields-represent-zone-centroids)
+      - [**Generate Demand with node.csv (if zone\_id field exist, generated zone boundary cover zone\_id that are not empty) and poi.csv**](#generate-demand-with-nodecsv-if-zone_id-field-exist-generated-zone-boundary-cover-zone_id-that-are-not-empty-and-poicsv)
+    - [**Call for Contributions**](#call-for-contributions)
+    - [**Citing grid2demand**](#citing-grid2demand)
+  - [**Starting with Grid2demand - Learning Sources**](#starting-with-grid2demand---learning-sources)
+  - [**Introduction and Background Knowledge**](#introduction-and-background-knowledge)
+    - [**4-step transportation forecasting**](#4-step-transportation-forecasting)
+    - [**Productions and Attractions**](#productions-and-attractions)
+    - [**Estimate Trip Productions/Attractions Using Trip Rates**](#estimate-trip-productionsattractions-using-trip-rates)
+    - [**Accessibility**](#accessibility)
+    - [**Trip distribution**](#trip-distribution)
+  - [**What is grid2demand - the open-source package**](#what-is-grid2demand---the-open-source-package)
+    - [**Flowchart of grid2demand**](#flowchart-of-grid2demand)
+    - [**Grid partition and zone creation**](#grid-partition-and-zone-creation)
+    - [**Trip generation**](#trip-generation)
+    - [**Accessibility and distance computing**](#accessibility-and-distance-computing)
+    - [**Trip distribution**](#trip-distribution-1)
+    - [**OD demand estimation using link counts and different data sources**](#od-demand-estimation-using-link-counts-and-different-data-sources)
+  - [**Quick Implementation and Visualization**](#quick-implementation-and-visualization)
 
-![](doc/media/9ed9631f17469d631f9dfe97e4320c10.png)
 
-**Starting with Grid2demand**
+# **Grid2demand**
+
+GRID2DEMAND: A tool for generating zone-to-zone travel demand based on grid cells or TAZs
+
+## **Code Examples**
+
+### **Installation**
+
+```python
+pip install grid2demand
+```
+
+If you meet installation issues, please refer to the [user guide](https://github.com/asu-trans-ai-lab/grid2demand) for solutions.
+
+### **Simple Example**
+
+#### **Generate Demand with node.csv and poi.csv**
+
+1. Create zone from node.csv (the boundary of nodes), this will generate grid cells (num_x_blocks, num_y_blocks, or x length and y length in km for each grid cell)
+2. Generate demands for between zones (utilize nodes and pois)
+
+```python
+from __future__ import absolute_import
+import grid2demand as gd
+
+if __name__ == "__main__":
+
+    # Specify input directory
+    path_node = "your-path-to-node.csv"
+    path_poi = "your-path-to-poi.csv"
+
+    # Initialize a GRID2DEMAND object
+    gd = GRID2DEMAND(node_file = path_node, poi_file = path_poi)
+
+    # load network: node and poi
+    net = gd.load_network()
+
+    # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
+    gd.net2zone(num_x_blocks=10, num_y_blocks=10)
+    # net.net2zone(cell_width=10, cell_height=10, unit="km")
+
+    # Synchronize geometry info between zone, node and poi
+    net.sync_geometry_between_zone_and_node_poi()
+
+    # Calculate demand by running gravity model
+    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+
+    # Save demand, zone, updated node, updated poi to csv
+    net.save_results_to_csv(overwrite_file=True)
+```
+
+#### **Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)**
+
+```python
+from __future__ import absolute_import
+import grid2demand as gd
+
+if __name__ == "__main__":
+
+    # Specify input directory
+    path_node = "your-path-to-node.csv"
+    path_poi = "your-path-to-poi.csv"
+    path_zone = "your-path-to-zone.csv"  # zone_id, geometry are required columns
+
+    # Initialize a GRID2DEMAND object
+    gd = GRID2DEMAND(zone_file = path_zone, node_file = path_node, poi_file = path_poi)
+
+    # load network: node and poi
+    net = gd.load_network()
+
+    # Generate zone
+    gd.taz2zone()
+
+    # Synchronize geometry info between zone, node and poi
+    net.sync_geometry_between_zone_and_node_poi()
+
+    # Calculate demand by running gravity model
+    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+
+    # Save demand, zone, updated node, updated poi to csv
+    net.save_results_to_csv(overwrite_file=True)
+```
+
+#### **Generate Demand with node.csv, poi.csv and zone.csv (x_coord, y_coord fields represent zone centroids)**
+
+```python
+from __future__ import absolute_import
+import grid2demand as gd
+
+if __name__ == "__main__":
+
+    # Specify input directory
+    path_node = "your-path-to-node.csv"
+    path_poi = "your-path-to-poi.csv"
+    path_zone = "your-path-to-zone.csv"  # zone_id, x_coord, y_coord are required columns
+
+    # Initialize a GRID2DEMAND object
+    gd = GRID2DEMAND(zone_file = path_zone, node_file = path_node, poi_file = path_poi)
+
+    # load network: node and poi
+    net = gd.load_network()
+
+    # Generate zone
+    gd.taz2zone()
+
+    # Synchronize geometry info between zone, node and poi
+    net.sync_geometry_between_zone_and_node_poi()
+
+    # Calculate demand by running gravity model
+    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+
+    # Save demand, zone, updated node, updated poi to csv
+    net.save_results_to_csv(overwrite_file=True)
+```
+
+#### **Generate Demand with node.csv (if zone_id field exist, generated zone boundary cover zone_id that are not empty) and poi.csv**
+
+```python
+from __future__ import absolute_import
+import grid2demand as gd
+
+if __name__ == "__main__":
+
+    # Specify input directory
+    path_node = "your-path-to-node.csv"  # make sure you have zone_id field in node.csv
+    path_poi = "your-path-to-poi.csv"
+
+    # Initialize a GRID2DEMAND object
+    gd = GRID2DEMAND(node_file = path_node, poi_file = path_poi, use_zone_id=True)
+
+    # load network: node and poi
+    net = gd.load_network()
+
+    # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
+    gd.net2zone(num_x_blocks=10, num_y_blocks=10)
+    # net.net2zone(cell_width=10, cell_height=10, unit="km")
+
+    # Synchronize geometry info between zone, node and poi
+    net.sync_geometry_between_zone_and_node_poi()
+
+    # Calculate demand by running gravity model
+    net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+
+    # Save demand, zone, updated node, updated poi to csv
+    net.save_results_to_csv(overwrite_file=True)
+```
+
+### **Call for Contributions**
+
+The grid2demand project welcomes your expertise and enthusiasm!
+
+Small improvements or fixes are always appreciated. If you are considering larger contributions to the source code, please contact us through email: [Xiangyong Luo](mailto:luoxiangyong01@gmail.com), [Dr. Xuesong Simon Zhou](mailto:xzhou74@asu.edu)
+
+Writing code isn't the only way to contribute to grid2demand. You can also:
+
+* review pull requests
+* help us stay on top of new and old issues
+* develop tutorials, presentations, and other educational materials
+* develop graphic design for our brand assets and promotional materials
+* translate website content
+* help with outreach and onboard new contributors
+* write grant proposals and help with other fundraising efforts
+
+For more information about the ways you can contribute to grid2demand, visit [our GitHub](https://github.com/asu-trans-ai-lab/grid2demand). If you' re unsure where to start or how your skills fit in, reach out! You can ask by opening a new issue or leaving a comment on a relevant issue that is already open on GitHub.
+
+### **Citing grid2demand**
+
+If you use grid2demand in your research please use the following BibTeX entry:
+
+```cite
+Xiangyong Luo, Dustin Carlino, and Xuesong Simon Zhou. (2023). xyluo25/grid2demand: new lease to v0.4.1. Zenodo. https://doi.org/10.5281/zenodo.10899860
+```
+
+
+
+## **Starting with Grid2demand - Learning Sources**
+
+-   How to quickly generate **initial origin-destination transportation demand** for engaging traffic simulation games such as A/B street and DTALite?
+-   How to teach our undergraduate students the important **trip generation and trip distribution steps**, using their own beautiful campus as examples?
+-   How to analyze the resident locations and other land use properties using flexible **grid zones, based on POI data from OpenStreetMap** data and using **open transportation modeling format**
+
+<img src="docs/media/9ed9631f17469d631f9dfe97e4320c10.png" style="zoom:80%;" />
+
 If you have not used Grid2demand before, here are some advices to get started.
 
 1. Read the user guide or watch the video at https://www.youtube.com/watch?v=EfjCERQQGTs.
 
 2. Obtain a map.osm or map.osm.pbf file for your area of interest at https://extract.bbbike.org/ or openstreetmap.org
 
 3. Look at the examples at Google colab environment https://github.com/asu-trans-ai-lab/grid2demand/blob/main/grid2demand_tutorial.ipynb
 
 4. Install Python, Grid2demand and QGIS on your computer or using Google Colab environment to modify one of the examples to implement your own model.
 
-5. Post your questions on the users group: 
+5. Post your questions on the users group:
 
      GitHub: https://github.com/asu-trans-ai-lab/grid2demand/issues
 
      Google: groups.google.com/d/forum/grid2demand
 
-Open-source tool of grid2demand aims to provide an open-source quick demand
-generation python package, which can work anywhere in the world, thanks to open
-data from [OpenStreetMap](Openstreetmap) users.
-
-To know more about this tool, please check out the 3rd mini teaching lesson in
-our podcast series, [https://www.youtube.com/watch?v=EfjCERQQGTs](https://www.youtube.com/watch?v=EfjCERQQGTs).
-
-> **Contents**
-
-- **Introduction and Background Knowledge**
-- **What is grid2demand?**
-- **Quick Start**
-
-Gird2demand is an open-source trip generation and distribution tool for teaching
-transportation planning and applications. It generates zone-to-zone travel
-demand based on alphanumeric grid zones. Users can obtain zone-to-zone and
-node-to-node travel demand with a few lines of python code based on
-OpenStreetMap and OSM2GMNS.
-
-For the python source code and sample network files, readers can visit the
-project homepage at ASU Trans+AI Lab Github
-([https://github.com/asu-trans-ai-lab/grid2demand](https://github.com/asu-trans-ai-lab/grid2demand)). The Jupyter notebook
-example can be found at
-[https://github.com/asu-trans-ai-lab/grid2demand/blob/main/grid2demand.ipynb](https://github.com/asu-trans-ai-lab/grid2demand/blob/main/grid2demand_tutorial.ipynb),
-which is also accessible through Google Colab.
+Open-source tool of grid2demand aims to provide an open-source quick demand generation python package, which can work anywhere in the world, thanks to open data from [OpenStreetMap](Openstreetmap) users.
+
+To know more about this tool, please check out the 3rd mini teaching lesson in our podcast series [https://www.youtube.com/watch?v=EfjCERQQGTs](https://www.youtube.com/watch?v=EfjCERQQGTs).
+
+Gird2demand is an open-source trip generation and distribution tool for teaching transportation planning and applications. It generates zone-to-zone travel demand based on alphanumeric grid zones. Users can obtain zone-to-zone and
+node-to-node travel demand with a few lines of python code based on OpenStreetMap and OSM2GMNS.
+
+For the python source code and sample network files, readers can visit the project homepage at ASU Trans+AI Lab Github
+([https://github.com/asu-trans-ai-lab/grid2demand](https://github.com/asu-trans-ai-lab/grid2demand)). The Jupyter notebook example can be found at
+[https://github.com/asu-trans-ai-lab/grid2demand/blob/main/grid2demand.ipynb](https://github.com/asu-trans-ai-lab/grid2demand/blob/main/grid2demand_tutorial.ipynb), which is also accessible through Google Colab.
 
 Mini teaching lesson: [https://www.youtube.com/watch?v=EfjCERQQGTs](https://www.youtube.com/watch?v=EfjCERQQGTs)
 
-**I. Introduction and Background Knowledge**
+## **Introduction and Background Knowledge**
 
-Trip generation and trip distribution are the first 2 steps in the larger
-context of the 4-step process in transportation planning. The standard four
-steps are briefly described below.
-
-- Trip Generation: Estimate how many trips enter or leave a
-  zone/traffic-analysis-zone (TAZ)
-- Trip Distribution: Estimate how many trips from each zone/TAZ end in all
-  zones/TAZs
-- Mode Choice: Estimate which travel-method is used (e.g., vehicle, transit,
-  walk) to complete those trips
-- Traffic Assignment: Distribute vehicles/traffic flow to different paths
-  during travel
-
-![](doc/media/3671eeff70fb8c6f4eb7c86dfb28dcf1.png)
-
-Trip generation is a procedure that uses socioeconomic data (e.g., household
-size, income, etc.) to estimate the number of person trips for a modeled time
-period (e.g., daily, peak hour) at a Traffic Analysis Zone (TAZ) level. A person
-trip involves a single person leaving from an origin and arriving at a single
-destination, and each trip has a classification/purpose based on typical
-classification such as home-based-work (HBW), home-based-other (HBO), and
-non-home-based (NHB).
+###  **4-step transportation forecasting**
 
-![](doc/media/19d7918a267236bd2e454531c6fdad54.png)
+Trip generation and trip distribution are the first 2 steps in the larger context of the 4-step process in transportation planning. The standard four steps are briefly described below.
 
-In the four-step process, there are two typical methods used to predict trips
-based on attributes:
+- Trip Generation: Estimate how many trips enter or leave a zone/traffic-analysis-zone (TAZ)
+- Trip Distribution: Estimate how many trips from each zone/TAZ end in all zones/TAZs
+- Mode Choice: Estimate which travel-method is used (e.g., vehicle, transit, walk) to complete those trips
+- Traffic Assignment: Distribute vehicles/traffic flow to different paths during travel
+
+<img src="docs/media/3671eeff70fb8c6f4eb7c86dfb28dcf1.png" style="zoom:60%;" />
+
+Trip generation is a procedure that uses socioeconomic data (e.g., household size, income, etc.) to estimate the number of person trips for a modeled time period (e.g., daily, peak hour) at a Traffic Analysis Zone (TAZ) level. A person trip involves a single person leaving from an origin and arriving at a single destination, and each trip has a classification/purpose based on typical
+classification such as home-based-work (HBW), home-based-other (HBO), and non-home-based (NHB).
+
+<img src="docs/media/19d7918a267236bd2e454531c6fdad54.png" style="zoom:67%;" />
+
+In the four-step process, there are two typical methods used to predict trips based on attributes:
 
 - [Trip rate method based on regression equations](#id.rjox6xhc6knq)
 - [Cross-classification using category-based trip rates](#id.2d2g6gayq4ya)
 
-After estimating the total number of trips produced, the trips are often
-separated by different purposes (e.g., HBW, HBO, NHB).
+After estimating the total number of trips produced, the trips are often separated by different purposes (e.g., HBW, HBO, NHB).
 
-An alternative approach to modeling trips is to model tours, which can be
-thought of as a series of linked trips. Tours are typically used in
-Activity-Based Models (ABM), where daily travel activities are generated based
-on activity patterns for households.
-
-**Productions and Attractions**
-
-In trip-based transportation planning, for a home-based trip, a production is
-related to the home end/location, while an attraction is related to the non-home
-end/location. For a non-home-based trip, a production is related to the origin
-location, and an attraction is related to the destination location. Trips
-entering and leaving a zone should balance - if a person leaves a zone, they
+An alternative approach to modeling trips is to model tours, which can be thought of as a series of linked trips. Tours are typically used in Activity-Based Models (ABM), where daily travel activities are generated based on activity patterns for households.
+
+### **Productions and Attractions**
+
+In trip-based transportation planning, for a home-based trip, a production is related to the home end/location, while an attraction is related to the non-home end/location. For a non-home-based trip, a production is related to the origin location, and an attraction is related to the destination location. Trips entering and leaving a zone should balance - if a person leaves a zone, they
 should also return; if a person enters a zone, they should also leave.
 
-For example, if a person travels from home to work and then from work to home on
-a certain day, then 2 home-based work trip productions are generated at the home
-TAZ, and two attractions related at his or her work location TAZ.
-
-**Estimate Trip Productions/Attractions Using Trip Rates**
-
-Productions are typically modeled as a function of population and/or number of
-households, as well as income levels or auto ownership. Other explanatory
-variables might be used, such as the number of workers, but we need to make sure
-explanatory variables are often not interrelated and correlated with each other.
-
-Attractions are often modeled as a function of the number of households and/or
-number of employees, where employment may be broken down by different types
-(e.g., retail, office, service, and other). Again, other explanatory variables
-can also be used, such as commercial floor space or CBD (Central Business
-District) variables, but the same checks for correlation between variables
-should be utilized. Attractions tend to be more difficult to measure/estimate,
-and we tend to have less trust in these estimates. For more information, users
-can read [NCHRP Report 365: “Travel Estimation Techniques, CH 3 trip
-generation](http://www.google.com/url?q=http%3A%2F%2Fntl.bts.gov%2Flib%2F21000%2F21500%2F21563%2FPB99126724.pdf&sa=D&sntz=1&usg=AFQjCNG2L127sploJ1a6_-ZmhSt6PnNypA)
-and [NCHRP Report 716: Travel Demand Forecasting: Parameters and Techniques, CH
-4.4 Trip
-Generation](http://onlinepubs.trb.org/onlinepubs/nchrp/nchrp_rpt_716.pdf).
-
-**Accessibility**
-
-In transportation planning, accessibility is first defined as the potential of
-opportunities for traveler interaction. the potential opportunity for traveler
-interaction is positively associated with accessibility. Typically,
-accessibility captures the extent of the attractiveness of each potential
-destination and some researchers represent accessibility as the amount of
-activity locations potentially reachable within a given travel time or distance
-from an origin location.
-
-One of the goals of transportation system construction and management is to
-improve individuals’ accessibility or the ease of reaching desired activities,
-destinations, and services. In general, quantitative accessibility measures
-describe how many and how easily destinations can be reached from a particular
-zone. For more information, users can check
-[https://tfresource.org/topics/Accessibility.html](https://tfresource.org/topics/Accessibility.html).
-
-**Trip distribution**
-
-There are a variety of trip distribution formulations. Among recent travel
-models, two formulations dominate: the gravity model and the destination choice
-model.
-
-![](doc/media/55701539d9bf1b1d46d801cb3c890ef1.png)
-
-For each OD pair, a typical gravity model is applied to calculate zone-to-zone
-demand volume. In the gravity model, the trips produced at an origin and
-attracted to a destination are directly proportional to the total trip
-productions at the origin and the total attractions at the destination with
-"friction factor", which represents the reluctance or impedance of persons to
-make trips of various
-
-duration or distances. A gravity model may be “singly-constrained” or
-“doubly-constrained”. For more information, please visit
-https://tfresource.org/topics/Trip_distribution.html. and
-http://www.princeton.edu/\~alaink/Orf467F12/The%20Gravity%20Model.pdf
-
-![](doc/media/a3b008d9e9f19131bcd3398b156ba1fc.png)
-
-For each OD pair, a **gravity model** to calculate zone-to-zone demand volume is
-formulated as follows.
-
-![](doc/media/b09c688a7fcd2dedb0d76fe1cda393b9.png)
-
-![](doc/media/91a532f54d659bc3a5978f8a48d7b6be.png)
-
-![](doc/media/090d638cdd3a06ea5bdaf96b48821616.png)
-
-**II. What is grid2demand?**
-
-Grid2demand is a quick demand generation tool based on the trip generation and
-trip distribution methods of the standard 4-step travel model for teaching
-transportation planning and applications. By taking advantage of the OSM2GMNS
-tool to obtain a routable transportation network from OpenStreetMap, Grid2demand
-aims to further utilize Point of Interest (POI) data to construct a trip demand
-matrix aligned with standard travel models.
-
-The area of interest is partitioned into an alphanumeric grid (also known as
-atlas grid), in which each cell is identified by a combination of a letter and a
-number. The trip generation step is performed at the POI node level using ITE
-trip generation tables
-(https://www.ite.org/technical-resources/topics/trip-and-parking-generation/trip-generation-10th-edition-formats/)
-or other trip rate references.
-
-When partitioning grid cells and calculating accessibility, World Geodetic
-System-1984 Coordinate System is applied to convert coordinates to length. The
-trip distribution is carried out using a typical gravity model. The data flow
-chart is illustrated in the following table and figure.
+For example, if a person travels from home to work and then from work to home on a certain day, then 2 home-based work trip productions are generated at the home TAZ, and two attractions related at his or her work location TAZ.
+
+### **Estimate Trip Productions/Attractions Using Trip Rates**
+
+Productions are typically modeled as a function of population and/or number of households, as well as income levels or auto ownership. Other explanatory variables might be used, such as the number of workers, but we need to make sure explanatory variables are often not interrelated and correlated with each other.
+
+Attractions are often modeled as a function of the number of households and/or number of employees, where employment may be broken down by different types (e.g., retail, office, service, and other). Again, other explanatory variables can also be used, such as commercial floor space or CBD (Central Business District) variables, but the same checks for correlation between variables should be utilized. Attractions tend to be more difficult to measure/estimate, and we tend to have less trust in these estimates. For more information, users can read [NCHRP Report 365: “Travel Estimation Techniques, CH 3 trip
+generation](http://www.google.com/url?q=http%3A%2F%2Fntl.bts.gov%2Flib%2F21000%2F21500%2F21563%2FPB99126724.pdf&sa=D&sntz=1&usg=AFQjCNG2L127sploJ1a6_-ZmhSt6PnNypA) and [NCHRP Report 716: Travel Demand Forecasting: Parameters and Techniques, CH
+4.4 Trip Generation](http://onlinepubs.trb.org/onlinepubs/nchrp/nchrp_rpt_716.pdf).
+
+### **Accessibility**
+
+In transportation planning, accessibility is first defined as the potential of opportunities for traveler interaction. the potential opportunity for traveler interaction is positively associated with accessibility. Typically, accessibility captures the extent of the attractiveness of each potential destination and some researchers represent accessibility as the amount of activity locations potentially reachable within a given travel time or distance from an origin location.
+
+One of the goals of transportation system construction and management is to improve individuals’ accessibility or the ease of reaching desired activities, destinations, and services. In general, quantitative accessibility measures describe how many and how easily destinations can be reached from a particular zone. For more information, users can check [https://tfresource.org/topics/Accessibility.html](https://tfresource.org/topics/Accessibility.html).
+
+### **Trip distribution**
+
+There are a variety of trip distribution formulations. Among recent travel models, two formulations dominate: the gravity model and the destination choice model.
+
+<img src="docs/media/55701539d9bf1b1d46d801cb3c890ef1.png" style="zoom:67%;" />
+
+For each OD pair, a typical gravity model is applied to calculate zone-to-zone demand volume. In the gravity model, the trips produced at an origin and attracted to a destination are directly proportional to the total trip productions at the origin and the total attractions at the destination with "friction factor", which represents the reluctance or impedance of persons to
+make trips of various duration or distances. A gravity model may be “singly-constrained” or “doubly-constrained”. For more information, please visit https://tfresource.org/topics/Trip_distribution.html. and http://www.princeton.edu/~alaink/Orf467F12/The%20Gravity%20Model.pdf
+
+<img src="docs/media/a3b008d9e9f19131bcd3398b156ba1fc.png" style="zoom:67%;" />
+
+For each OD pair, a **gravity model** to calculate zone-to-zone demand volume is formulated as follows.
+
+<img src="docs/media/b09c688a7fcd2dedb0d76fe1cda393b9.png" style="zoom:67%;" />
+
+<img src="docs/media/91a532f54d659bc3a5978f8a48d7b6be.png" style="zoom:67%;" />
+
+<img src="docs/media/090d638cdd3a06ea5bdaf96b48821616.png" style="zoom:67%;" />
+
+## **What is grid2demand - the open-source package**
+
+Grid2demand is a quick demand generation tool based on the trip generation and trip distribution methods of the standard 4-step travel model for teaching transportation planning and applications. By taking advantage of the OSM2GMNS tool to obtain a routable transportation network from OpenStreetMap, Grid2demand aims to further utilize Point of Interest (POI) data to construct a trip demand matrix aligned with standard travel models.
+
+The area of interest is partitioned into an alphanumeric grid (also known as atlas grid), in which each cell is identified by a combination of a letter and a number. The trip generation step is performed at the POI node level using ITE
+trip generation tables (https://www.ite.org/technical-resources/topics/trip-and-parking-generation/trip-generation-10th-edition-formats/) or other trip rate references.
+
+When partitioning grid cells and calculating accessibility, World Geodetic System-1984 Coordinate System is applied to convert coordinates to length. The trip distribution is carried out using a typical gravity model. The data flow chart is illustrated in the following table and figure.
 
 **Description of Data Files**
 
 | Step | Process                            | Input File or Parameter                                                                    | Output File                                                                                                        | Method                                                                  |
 | ---- | ---------------------------------- | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------- |
 | 0    | Network files preparation          | map file from OpenStreetMap                                                                | *node.csv, link.csv, poi.csv*                                                                                    | Osm2gmns tool                                                           |
 | 1    | Input files reading                | *node.csv, poi.csv*                                                                      |                                                                                                                    |                                                                         |
 | 2    | Zone generation and grid partition | Number of blocks or grid scales in meters with latitude of the area of interest (optional) | *zone,csv, poi.csv* (update with zone id)                                                                        | Alphanumeric grid                                                       |
 | 3    | Trip generation                    | *poi_trip_rate.csv* (optional), trip purpose                                             | *poi_trip_rate.csv* (output/update with utilization notes), *node.csv* (update with zone id and demand values) | Trip rate method                                                        |
 | 4    | Accessibility calculation          | *accessibility.csv* (optional), latitude of the area of interest                         | *accessibility.csv*                                                                                              | Simple straight-line distance between zone centroids                    |
 | 5    | Trip distribution                  | Trip purpose, friction factor coefficients                                                 | *demand.csv, zone,csv* (update with total production and attraction in each zone)                                | Gravity model                                                           |
 | 6    | Agent generation                   | *demand.csv*                                                                             | *agent.csv*                                                                                                      | Random sampling of node-to-node agents according to zone-to-zone demand |
 | 7    | Visualization                      |                                                                                            | QGIS or NEXTA                                                                                                      |                                                                         |
 
-**Flowchart of grid2demand**
+### **Flowchart of grid2demand**
 
-![](doc/media/4b0c64e44d91cae9034ec0cf00352341.png)
+<img src="docs/media/4b0c64e44d91cae9034ec0cf00352341.png" style="zoom:67%;" />
 
-For the entire package, the input files include the network files in GMNS format
-(*node.csv, link.csv*) as well as *poi.csv*, generated by the OSM2GMNS tool.
+For the entire package, the input files include the network files in GMNS format (*node.csv, link.csv*) as well as *poi.csv*, generated by the OSM2GMNS tool.
 
 Users can download a default *poi_trip_rate.csv* from
 https://github.com/asu-trans-ai-lab/grid2demand/blob/main/examples/data_folder/poi_trip_rate.csv
 and apply further adjustments based on local traffic conditions.
 
-The final output files include *zone.csv, accessibility.csv*, *demand.csv* for
-zone-to-zone OD demand matrix, and *input_agent.csv* for node-to-node agent
-files which can be used by agent-based simulators such as AB Street and DTALite.
-Accordingly, *node.csv* and *poi.csv* are updated with assigned zone
-information.
-
-**Grid partition and zone creation**
-
-![](doc/media/4b18b9bbee10d5692d9c907435012e16.png)
-
-To facilitate hierarchical and multi-resolution spatial computing, grid cells
-are used to aggregate trips to traffic analysis zones, while standard TAZs are
-typically defined based on census tracts. Users can specify the number of cells
-per row and per column or the width and height of each grid cell (in meters) for
-the area of interest. To maintain a consistent mapping, we use a fractional
-value in terms of the degree at different latitudes to represent different
-lengths on a flat surface. That is, a value of 0.01 longitudinal degrees at 60
-degrees latitude is equivalent to 0.558 km on a flat surface. Thus, users can
-provide a latitude value of the area of interest, and the software will identify
-the closest latitude in the following table and use the equivalent distance to
+The final output files include *zone.csv, accessibility.csv*, *demand.csv* for zone-to-zone OD demand matrix, and *input_agent.csv* for node-to-node agent files which can be used by agent-based simulators such as AB Street and DTALite. Accordingly, *node.csv* and *poi.csv* are updated with assigned zone information.
+
+### **Grid partition and zone creation**
+
+<img src="docs/media/4b18b9bbee10d5692d9c907435012e16.png" style="zoom:67%;" />
+
+To facilitate hierarchical and multi-resolution spatial computing, grid cells are used to aggregate trips to traffic analysis zones, while standard TAZs are typically defined based on census tracts. Users can specify the number of cells per row and per column or the width and height of each grid cell (in meters) for the area of interest. To maintain a consistent mapping, we use a fractional
+value in terms of the degree at different latitudes to represent different lengths on a flat surface. That is, a value of 0.01 longitudinal degrees at 60 degrees latitude is equivalent to 0.558 km on a flat surface. Thus, users can provide a latitude value of the area of interest, and the software will identify the closest latitude in the following table and use the equivalent distance to
 measure for that area.
 
-![](doc/media/ee61ebb6ce64fbffc4b145c97468d98b.png)
+![](docs/media/ee61ebb6ce64fbffc4b145c97468d98b.png)
+
+Moreover, some nodes in the network are marked as boundary nodes in *node.csv* to describe the entrance or exit points with respect to the area of interest. Thus, we add virtual zones around the grid area’s boundary to aggregate demand from outside the area of interest, which are regarded as “gates” or external stations.
+
+### **Trip generation**
 
-Moreover, some nodes in the network are marked as boundary nodes in *node.csv*
-to describe the entrance or exit points with respect to the area of interest.
-Thus, we add virtual zones around the grid area’s boundary to aggregate demand
-from outside the area of interest, which are regarded as “gates” or external
-stations.
-
-**Trip generation**
-
-To enable detailed modeling of trip generation from parking lots and buildings,
-different types of POI nodes are specifically covered in file *poi.csv*,
-extracted from the original *OSM file*. The user can supply more information in
-*poi.csv* in case of missing values. The trip generation process used in
-grid2demand has the following 3 sub-steps.
-
-1. For each node, the amount of produced or attracted traffic is computed based
-   on the underlying trip purpose and POI type, defined in *poi_trip_rate.csv.*
-2. Update the field of production and attraction for each POI or boundary node
-   in *node*.*csv*.
-3. For each zone, its total production and attraction values can be calculated
-   as the sum of node-based values across all nodes with the corresponding zone
-   id.
+To enable detailed modeling of trip generation from parking lots and buildings, different types of POI nodes are specifically covered in file *poi.csv*, extracted from the original *OSM file*. The user can supply more information in *poi.csv* in case of missing values. The trip generation process used in grid2demand has the following 3 sub-steps.
+
+1. For each node, the amount of produced or attracted traffic is computed based on the underlying trip purpose and POI type, defined in *poi_trip_rate.csv.*
+2. Update the field of production and attraction for each POI or boundary node in *node*.*csv*.
+3. For each zone, its total production and attraction values can be calculated as the sum of node-based values across all nodes with the corresponding zone id.
 
 A sample *poi_trip_rate* table is listed below.
 
-![](doc/media/2e05796ce081da842b82437291652629.emf)
+![](docs/media/2e05796ce081da842b82437291652629.emf)
 
-For each boundary node (such as freeway or arterial’s endpoint at the boundary
-of the area) which stands for a gate to enter or leave the area, the default
-values of production and attraction are set to be 1000.
+For each boundary node (such as freeway or arterial’s endpoint at the boundary of the area) which stands for a gate to enter or leave the area, the default values of production and attraction are set to be 1000.
 
-**Accessibility and distance computing**
+### **Accessibility and distance computing**
 
-In the current version, accessibility is measured by zone-to-zone straight-line
-distance according to zone centroid coordinates. A more advanced version will be
-provided in the future to use the shortest path algorithm for computing
-end-to-end driving or multimodal travelling distance and costs.
+In the current version, accessibility is measured by zone-to-zone straight-line distance according to zone centroid coordinates. A more advanced version will be provided in the future to use the shortest path algorithm for computing end-to-end driving or multimodal travelling distance and costs.
 
-**Trip distribution**
+### **Trip distribution**
 
-As mentioned above, a typical gravity model is applied to calculate zone-to-zone
-demand volume. The trip purpose and friction factor coefficients can be defined
-by users or by default. The default values under three typical trip purposes are
-listed in the following table.
+As mentioned above, a typical gravity model is applied to calculate zone-to-zone demand volume. The trip purpose and friction factor coefficients can be defined by users or by default. The default values under three typical trip purposes are listed in the following table.
 
-![](doc/media/b1e18b1a6a4b0b7e20a09a760ff68130.png)
+![](docs/media/b1e18b1a6a4b0b7e20a09a760ff68130.png)
 
-**OD demand estimation using link counts and different data sources**
+### **OD demand estimation using link counts and different data sources**
 
-In the future, output *demand.csv* can act as one of multiple data sources for a
-hierarchical travel demand estimation and *input_agent.csv* can be directly used
-for assignment by DTALite and for other travel models. For more information,
+In the future, output *demand.csv* can act as one of multiple data sources for a hierarchical travel demand estimation and *input_agent.csv* can be directly used for assignment by DTALite and for other travel models. For more information,
 please visit
 https://www.researchgate.net/publication/325131295_Hierarchical_travel_demand_estimation_using_multiple_data_sources_A_forward_and_backward_propagation_algorithmic_framework_on_a_layered_computational_graph.
 
-**III. Quick start**
+## **Quick Implementation and Visualization**
 
-We will use the University of Maryland, College Park as an example to illustrate
-how to use grid2demand.
+We will use the University of Maryland, College Park as an example to illustrate how to use grid2demand.
 
 **Step 1: Installation**
 
-You can install the latest release of grid2demand at
-[PyPI](https://pypi.org/project/pydriosm/)
-(https://pypi.org/project/grid2demand/) via
-[pip](https://packaging.python.org/key_projects/#pip):
+You can install the latest release of grid2demand at [PyPI](https://pypi.org/project/pydriosm/) (https://pypi.org/project/grid2demand/) via [pip](https://packaging.python.org/key_projects/#pip):
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
 pip install grid2demand
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
-After running the command above, the grid2demand package along with two required
-dependency packages (numpy, pandas) will be installed on your computer (if they
-have not been installed yet).
+After running the command above, the grid2demand package along with two required dependency packages (numpy, pandas) will be installed on your computer (if they have not been installed yet).
 
 **Step 2: Determine the boundary of interest and download .osm file from
 OpenStreetMap (https://www.openstreetmap.org/)**
 
-1. Adjust the map to the location of interest and click on the “Export” button
-   on the top.
+1. Adjust the map to the location of interest and click on the “Export” button on the top.
 
-![地图 描述已自动生成](doc/media/4e7e66963f555d17e4932bd4904cf4f7.png)
+<img src="docs/media/4e7e66963f555d17e4932bd4904cf4f7.png" alt="地图 描述已自动生成 " style="zoom:67%;" />
 
-1. Obtain the latitude and longitude coordinates (users can “manually select a
-   different area”).
-2. Click on the “Export” button found in the middle of the navigator to
-   download an OSM data file.
-3. For a very large area of interest, users need to click the link of “Overpass
-   API” to obtain a map file.
+1. Obtain the latitude and longitude coordinates (users can “manually select a different area”).
+2. Click on the “Export” button found in the middle of the navigator to download an OSM data file.
+3. For a very large area of interest, users need to click the link of “Overpass API” to obtain a map file.
 
-![](doc/media/cbc2a2fc7bb6040d83b0295cdf80fd5d.png)
+![](docs/media/cbc2a2fc7bb6040d83b0295cdf80fd5d.png)
 
 **Step 3: Execute OSM2GMNS to get network files in GMNS format**
 
-Open the Python IDE, such as Pycharm, for a typical configuration. Then, use
-OSM2GMNS to convert the *map.osm* file in OSM format into a network file in GMNS
-format.
+Open the Python IDE, such as Pycharm, for a typical configuration. Then, use OSM2GMNS to convert the *map.osm* file in OSM format into a network file in GMNS format.
 
-Notes: User guide for osm2gmns can be found at
-https://osm2gmns.readthedocs.io/en/latest/.
+Notes: User guide for osm2gmns can be found at https://osm2gmns.readthedocs.io/en/latest/.
 
-![](doc/media/6ea2cbc0b48354d4940c8e4f4c6e9f58.png)
+<img src="docs/media/6ea2cbc0b48354d4940c8e4f4c6e9f58.png" style="zoom:80%;" />
 
-![](doc/media/bc783b917bac32c27b66e4649a472088.png)
+<img src="docs/media/bc783b917bac32c27b66e4649a472088.png" style="zoom:80%;" />
 
-![](doc/media/bff56bb4b68eef97dfb8ee4a337500bb.png)
+<img src="docs/media/bff56bb4b68eef97dfb8ee4a337500bb.png" alt=" " style="zoom:80%;" />
 
 Please note that *poi.csv* might have different degrees of missing information.
 Please supply additional accurate POI-type information if needed.
 
 **Step 4: Execute grid2demand Python code**
 
 1. **Import the package and read input network data**
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
 ```python
-from grid2demand import GRID2DEMAND
+import grid2demand as gd
 
 input_dir = "Path-folder-to-your-node.csv-and-poi.csv"
 
-gd = GRID2DEMAND(input_dir)
+net = gd.GRID2DEMAND(input_dir)
 ```
 
 1. **Partition network into grid cells**
 
 Users can customize the number of grid cells by setting “number_of_x_blocks” and
 “number_of_y_blocks”. On the other hand, users can customize the cell’s width
 and height in meters under the latitude of the area by setting “cell_width”,
@@ -381,147 +449,128 @@
 By default, “cell_width” and “cell_height” are set as the length on a flat
 surface under a specific latitude corresponding to the degree of 0.006
 (equivalent to 400 meters or 0.25 miles at latitude = 45 degree).
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
 ```python
-node_dict, poi_dict = gd.load_network.values()
-
-zone_dict = gd.net2zone(node_dict, num_x_blocks=10,num_y_blocks=10)
-
-# Generate zone based on grid size with 10 km width and 10km height for each zone
-# zone_dict = gd.net2zone(node_dict, cell_width=10, cell_height=10, unit="km")
-
-# if you have your own zone.csv(TAZs), we can generate zones from your personal TAZs
-# zone_dict = gd.taz2zone()
+# load node and poi
+net.load_network()
 
+# create zone
+net.net2zone(num_x_blocks=10,num_y_blocks=10)
 
 # Synchronize geometry info between zone, node and poi
-#       add zone_id to node and poi dictionaries
-#       also add node_list and poi_list to zone dictionary
-updated_dict = gd.sync_geometry_between_zone_and_node_poi(zone_dict, node_dict, poi_dict)
-
-zone_dict_update, node_dict_update, poi_dict_update = updated_dict.values()
+net.sync_geometry_between_zone_and_node_poi()
 
 ```
 
-![](doc/media/d68e685394f3b21c3dfb97ec7b3c331a.png)
+![](docs/media/d68e685394f3b21c3dfb97ec7b3c331a.png)
 
-![](doc/media/dd9989c6abfc2feef6f66f6af63f4182.png)
+![](docs/media/dd9989c6abfc2feef6f66f6af63f4182.png)
 
 1. **Obtain production/attraction rates of each land use type with a specific
    trip purpose**
 
 Users can customize *poi_trip_rate.csv* by adding an external file folder
 location according to different trip purposes. By default, the trip purpose is
 set as purpose 1.
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
-```
+```python
 # Generate poi trip rate for each poi
-
-poi_trip_rate = gd.gen_poi_trip_rate(poi_dict_update, trip_rate_file="", trip_purpose=1)
+net.gen_poi_trip_rate(trip_rate_file="", trip_purpose=1)
 ```
 
-![](doc/media/a9a4ce4b1b2ece11a57b796de71cc0f5.png)
+![](docs/media/a9a4ce4b1b2ece11a57b796de71cc0f5.png)
 
 1. **Compute production/attraction value of each node according to POI type**
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
 ```python
 # Generate node production attraction for each node based on poi_trip_rate
-
-node_prod_attr = gd.gen_node_prod_attr(node_dict_update, poi_trip_rate)
+net.gen_node_prod_attr()
 
 # Calculate zone production and attraction based on node production and attraction
-
-zone_prod_attr = gd.calc_zone_prod_attr(node_prod_attr, zone_dict_update)
+net.calc_zone_prod_attr()
 
 ```
 
-![](doc/media/b7c81fd7f161d9d3008af476b2ac6314.png)
+![](docs/media/b7c81fd7f161d9d3008af476b2ac6314.png)
 
 1. **Calculate zone-to-zone accessibility matrix by centroid-to-centroid
    straight-line distance**
 
 Users need to input the latitude value of the area of interest. A latitude of 30
 degrees is selected as the default. On the other hand, users can customize the
 accessibility matrix by setting the external folder of file *accessibility.csv*.
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
 ```python
 # Calculate zone-to-zone od distance matrix
-
-zone_od_distance_matrix = gd.calc_zone_od_distance_matrix(zone_dict_update)
+net.calc_zone_od_distance_matrix()
 ```
 
-![](doc/media/803976b8470aca4060792d745ccb9182.png)
+![](docs/media/803976b8470aca4060792d745ccb9182.png)
 
 1. **Apply gravity model to perform trip distribution**
 
 Users need to input the trip purpose and the friction factor coefficients. The
 default values of HBW, HBO and NHB are described above.
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
 ```python
 # Run gravity model to generate agent-based demand
-
-df_demand = gd.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
+net.run_gravity_model()
 ```
 
-![](doc/media/54f05724a65916d625ef201196a9c0cb.png)
+![](docs/media/54f05724a65916d625ef201196a9c0cb.png)
 
 1. **Generate agent-based demand**
 
 Agent-based node-to-node demand will be generated randomly according to
 zone-to-zone demand obtained by the gravity model.
 
 \~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~\~
 
-```
+```python
 # generate agent-based demand
-
-df_agent = gd.gen_agent_based_demand(node_prod_attr, zone_prod_attr, df_demand=df_demand)
+net.gen_agent_based_demand()
 ```
 
-![](doc/media/6758fa4a5b00e18bb6d094776a6004a8.png)
+![](docs/media/6758fa4a5b00e18bb6d094776a6004a8.png)
 
 One can configure the working dictionary in the Python IDE (e.g., Pycharm)
 before executing grid2demand. The files in the working folder will be used to
 obtain zone-to-zone demand with generated five output files highlighted in blue
 below. The output files will be saved in the current folder as the working
 dictionary.
 
 ```python
 # You can also view and edit the package setting by using gd.pkg_settings
-print(gd.pkg_settings)
+print(net.pkg_settings)
 
 # Output demand, agent, zone, zone_od_dist_table, zone_od_dist_matrix files
-gd.save_demand
-gd.save_agent
-gd.save_zone
-gd.save_zone_od_dist_table
-gd.save_zone_od_dist_matrix
+net.save_results_to_csv()
 ```
 
-![](doc/media/4c2865c527a29c303ef29e237a91139a.png)
+![](docs/media/4c2865c527a29c303ef29e237a91139a.png)
 
 **Step 5: Visualization in QGIS**
 
 Open QGIS and add Delimited Text Layer to load the *demand.csv* and other files
 (with geometry info).
 
-![](doc/media/7845a6b0be22f6a8cd450fe3a3f8b830.png)
+![](docs/media/7845a6b0be22f6a8cd450fe3a3f8b830.png)
 
 Then open the “Properties” window of the demand layer. Set the symbology as
 graduated symbols by size.
 
-![](doc/media/2369dc93a0f61fc6aaa36adc56915f88.png)
+![](docs/media/2369dc93a0f61fc6aaa36adc56915f88.png)
 
 The zone-to-zone demand volume can be visualized with a base map.
 
-![](doc/media/b2402856b81670aae2208b51658f1457.png)
+![](docs/media/b2402856b81670aae2208b51658f1457.png)
```

### Comparing `grid2demand-0.4.2/grid2demand/func_lib/gen_agent_demand.py` & `grid2demand-0.4.3/grid2demand/func_lib/gen_agent_demand.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.2/grid2demand/func_lib/gen_zone.py` & `grid2demand-0.4.3/grid2demand/func_lib/read_node_poi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,408 +1,500 @@
 # -*- coding:utf-8 -*-
 ##############################################################
-# Created Date: Tuesday, September 5th 2023
+# Created Date: Monday, September 4th 2023
 # Contact Info: luoxiangyong01@gmail.com
 # Author/Copyright: Mr. Xiangyong Luo
 ##############################################################
 
 from __future__ import absolute_import
-import contextlib
-import itertools
 import pandas as pd
 import shapely
-import numpy as np
-from multiprocessing import Pool, cpu_count
+import os
+from multiprocessing import Pool
 
-from grid2demand.utils_lib.net_utils import Zone, Node
+from grid2demand.utils_lib.net_utils import Node, POI, Zone
 from grid2demand.utils_lib.pkg_settings import pkg_settings
+from grid2demand.utils_lib.utils import check_required_files_exist
+from pyufunc import (func_running_time, path2linux,
+                     get_filenames_by_ext,)
 
-from pyufunc import (calc_distance_on_unit_sphere, cvt_int_to_alpha, func_running_time)
+# supporting functions for multiprocessing implementation
 
 
-@func_running_time
-def get_lng_lat_min_max(node_dict: dict[int, Node]) -> list:
-    """Get the boundary of the study area
+def _create_node_from_dataframe(df_node: pd.DataFrame) -> dict[int, Node]:
+    """Create Node from df_node.
 
     Args:
-        node_dict (dict[int, Node]): node_dict {node_id: Node}
+        df_node (pd.DataFrame): the dataframe of node from node.csv
 
     Returns:
-        list: [min_lng, max_lng, min_lat, max_lat]
+        dict[int, Node]: a dict of nodes.{node_id: Node}
     """
-    first_key = list(node_dict.keys())[0]
+    # Reset index to avoid index error
+    df_node = df_node.reset_index(drop=True)
 
-    coord_x_min, coord_x_max = node_dict[first_key].x_coord, node_dict[first_key].x_coord
-    coord_y_min, coord_y_max = node_dict[first_key].y_coord, node_dict[first_key].y_coord
+    node_dict = {}
+    for i in range(len(df_node)):
+        try:
+            # check activity location tab
+            activity_type = df_node.loc[i, 'activity_type']
+            boundary_flag = df_node.loc[i, 'is_boundary']
+            if activity_type in ["residential", "poi"]:
+                activity_location_tab = activity_type
+            elif boundary_flag == 1:
+                activity_location_tab = "boundary"
+            else:
+                activity_location_tab = ''
+
+            # check whether zone_id field in node.csv or not
+            # if zone_id field exists and is not empty, assign it to __zone_id
+            try:
+                _zone_id = df_node.loc[i, 'zone_id']
+
+                # check if _zone is none or empty, assign -1
+                if pd.isna(_zone_id) or not _zone_id:
+                    _zone_id = -1
+
+            except Exception:
+                _zone_id = -1
+
+            node = Node(
+                id=df_node.loc[i, 'node_id'],
+                activity_type=activity_type,
+                activity_location_tab=activity_location_tab,
+                x_coord=df_node.loc[i, 'x_coord'],
+                y_coord=df_node.loc[i, 'y_coord'],
+                poi_id=df_node.loc[i, 'poi_id'],
+                boundary_flag=boundary_flag,
+                geometry=shapely.Point(df_node.loc[i, 'x_coord'], df_node.loc[i, 'y_coord']),
+                _zone_id=_zone_id
+            )
+            node_dict[df_node.loc[i, 'node_id']] = node
+        except Exception as e:
+            print(f"  : Unable to create node: {df_node.loc[i, 'node_id']}, error: {e}")
+    return node_dict
 
-    for node_id in node_dict:
-        if node_dict[node_id].x_coord < coord_x_min:
-            coord_x_min = node_dict[node_id].x_coord
-        if node_dict[node_id].x_coord > coord_x_max:
-            coord_x_max = node_dict[node_id].x_coord
-        if node_dict[node_id].y_coord < coord_y_min:
-            coord_y_min = node_dict[node_id].y_coord
-        if node_dict[node_id].y_coord > coord_y_max:
-            coord_y_max = node_dict[node_id].y_coord
 
-    return [coord_x_min - 0.000001, coord_x_max + 0.000001, coord_y_min - 0.000001, coord_y_max + 0.000001]
+def _create_poi_from_dataframe(df_poi: pd.DataFrame) -> dict[int, POI]:
+    """Create POI from df_poi.
 
+    Args:
+        df_poi (pd.DataFrame): the dataframe of poi from poi.csv
 
-@func_running_time
-def net2zone(node_dict: dict[int, Node],
-             num_x_blocks: int = 0,
-             num_y_blocks: int = 0,
-             cell_width: float = 0,
-             cell_height: float = 0, unit: str = "km",
-             use_zone_id: bool = False,
-             verbose: bool = False) -> dict[str, Zone]:
-    """convert node_dict to zone_dict by grid.
-    The grid can be defined by num_x_blocks and num_y_blocks, or cell_width and cell_height.
-    if num_x_blocks and num_y_blocks are specified, the grid will be divided into num_x_blocks * num_y_blocks.
-    if cell_width and cell_height are specified, the grid will be divided into cells with cell_width * cell_height.
-    Note: num_x_blocks and num_y_blocks have higher priority to cell_width and cell_height.
-            if num_x_blocks and num_y_blocks are specified, cell_width and cell_height will be ignored.
+    Returns:
+        dict[int, POI]: a dict of POIs.{poi_id: POI}
+    """
 
-    Args:
-        node_dict (dict[int, Node]): node_dict {node_id: Node}
-        num_x_blocks (int, optional): total number of blocks/grids from x direction. Defaults to 10.
-        num_y_blocks (int, optional): total number of blocks/grids from y direction. Defaults to 10.
-        cell_width (float, optional): the width for each block/grid . Defaults to 0. unit: km.
-        cell_height (float, optional): the height for each block/grid. Defaults to 0. unit: km.
-        unit (str, optional): the unit of cell_width and cell_height. Defaults to "km". Options:"meter", "km", "mile".
-        use_zone_id (bool, optional): whether to use zone_id in node_dict. Defaults to False.
-        verbose (bool, optional): print processing information. Defaults to False.
+    df_poi = df_poi.reset_index(drop=True)
+    poi_dict = {}
 
-    Raises
-        ValueError: Please provide num_x_blocks and num_y_blocks or cell_width and cell_height
+    for i in range(len(df_poi)):
+        try:
+            centroid = shapely.from_wkt(df_poi.loc[i, 'centroid'])
+            area = df_poi.loc[i, 'area']
+            if area > 90000:
+                area = 0
+            poi = POI(
+                id=df_poi.loc[i, 'poi_id'],
+                x_coord=centroid.x,
+                y_coord=centroid.y,
+                area=[area, area * 10.7639104],  # square meter and square feet
+                poi_type=df_poi.loc[i, 'building'] or "",
+                geometry=df_poi.loc[i, "geometry"]
+            )
+            poi_dict[df_poi.loc[i, 'poi_id']] = poi
+        except Exception as e:
+            print(f"  : Unable to create poi: {df_poi.loc[i, 'poi_id']}, error: {e}")
+    return poi_dict
 
-    Returns
-        Zone: dictionary, Zone cells with keys are zone names, values are Zone
 
-    Examples:
-        >>> zone_dict = net2zone(node_dict, num_x_blocks=10, num_y_blocks=10)
-        >>> zone_dict['A1']
-        Zone(id=0, name='A1', centroid_x=0.05, centroid_y=0.95, centroid='POINT (0.05 0.95)', x_min=0.0, x_max=0.1,
-        y_min=0.9, y_max=1.0, geometry='POLYGON ((0.05 0.9, 0.1 0.9, 0.1 1, 0.05 1, 0.05 0.9))')
+def _create_zone_from_dataframe_by_geometry(df_zone: pd.DataFrame) -> dict[int, Zone]:
+    """Create Zone from df_zone.
+
+    Args:
+        df_zone (pd.DataFrame): the dataframe of zone from zone.csv, the required fields are: [zone_id, geometry]
 
+    Returns:
+        dict[int, Zone]: a dict of Zones.{zone_id: Zone}
     """
+    df_zone = df_zone.reset_index(drop=True)
+    zone_dict = {}
 
-    # # convert node_dict to dataframe
-    # df_node = pd.DataFrame(node_dict.values())
-    # # get the boundary of the study area
-    # coord_x_min, coord_x_max = df_node['x_coord'].min(
-    # ) - 0.000001, df_node['x_coord'].max() + 0.000001
-    # coord_y_min, coord_y_max = df_node['y_coord'].min(
-    # ) - 0.000001, df_node['y_coord'].max() + 0.000001
-
-    # generate zone based on zone_id in node.csv
-    if use_zone_id:
-        node_dict_zone_id = {}
-
-        for node_id in node_dict:
-            with contextlib.suppress(AttributeError):
-                if node_dict[node_id]._zone_id != -1:
-                    node_dict_zone_id[node_id] = node_dict[node_id]
-
-        if not node_dict_zone_id:
-            print("  : No zone_id found in node_dict, will generate zone based on original node_dict")
-        else:
-            node_dict = node_dict_zone_id
-
-    coord_x_min, coord_x_max, coord_y_min, coord_y_max = get_lng_lat_min_max(node_dict)
-
-    # get nodes within the boundary
-    if use_zone_id:
-        node_dict_within_boundary = {}
-        for node_id in node_dict:
-            if node_dict[node_id].x_coord >= coord_x_min and node_dict[node_id].x_coord <= coord_x_max and \
-                    node_dict[node_id].y_coord >= coord_y_min and node_dict[node_id].y_coord <= coord_y_max:
-                node_dict_within_boundary[node_id] = node_dict[node_id]
-    else:
-        node_dict_within_boundary = node_dict
-
-    # Priority: num_x_blocks, number_y_blocks > cell_width, cell_height
-    # if num_x_blocks and num_y_blocks are given, use them to partition the study area
-    # else if cell_width and cell_height are given, use them to partition the study area
-    # else raise error
-
-    if num_x_blocks > 0 and num_y_blocks > 0:
-        x_block_width = (coord_x_max - coord_x_min) / num_x_blocks
-        y_block_height = (coord_y_max - coord_y_min) / num_y_blocks
-    elif cell_width > 0 and cell_height > 0:
-        x_dist_km = calc_distance_on_unit_sphere(
-            (coord_x_min, coord_y_min), (coord_x_max, coord_y_min), unit=unit)
-        y_dist_km = calc_distance_on_unit_sphere(
-            (coord_x_min, coord_y_min), (coord_x_min, coord_y_max), unit=unit)
-
-        num_x_blocks = int(np.ceil(x_dist_km / cell_width))
-        num_y_blocks = int(np.ceil(y_dist_km / cell_height))
-
-        x_block_width = (coord_x_max - coord_x_min) / num_x_blocks
-        y_block_height = (coord_y_max - coord_y_min) / num_y_blocks
-    else:
-        raise ValueError(
-            'Please provide num_x_blocks and num_y_blocks or cell_width and cell_height')
-
-    # partition the study area into zone cells
-    x_block_min_lst = [coord_x_min + i *
-                       x_block_width for i in range(num_x_blocks)]
-    y_block_min_lst = [coord_y_min + i *
-                       y_block_height for i in range(num_y_blocks)]
-
-    x_block_minmax_list = list(zip(
-        x_block_min_lst[:-1], x_block_min_lst[1:])) + [(x_block_min_lst[-1], coord_x_max)]
-    y_block_minmax_list = list(zip(
-        y_block_min_lst[:-1], y_block_min_lst[1:])) + [(y_block_min_lst[-1], coord_y_max)]
-
-    def generate_polygon(x_min, x_max, y_min, y_max) -> shapely.geometry.Polygon:
-        """Generate polygon from min and max coordinates
-
-        Parameters
-            x_min: float, Min x coordinate
-            x_max: float, Max x coordinate
-            y_min: float, Min y coordinate
-            y_max: float, Max y coordinate
+    for i in range(len(df_zone)):
+        try:
+            zone_id = df_zone.loc[i, 'zone_id']
+            zone_geometry = df_zone.loc[i, 'geometry']
+
+            zone_geometry_shapely = shapely.from_wkt(zone_geometry)
+            centroid_wkt = zone_geometry_shapely.centroid.wkt
+            centroid_x = zone_geometry_shapely.centroid.x
+            centroid_y = zone_geometry_shapely.centroid.y
+            zone = Zone(
+                id=zone_id,
+                name=zone_id,
+                centroid_x=centroid_x,
+                centroid_y=centroid_y,
+                centroid=centroid_wkt,
+                x_max=zone_geometry_shapely.bounds[2],
+                x_min=zone_geometry_shapely.bounds[0],
+                y_max=zone_geometry_shapely.bounds[3],
+                y_min=zone_geometry_shapely.bounds[1],
+                node_id_list=[],
+                poi_id_list=[],
+                production=0,
+                attraction=0,
+                production_fixed=0,
+                attraction_fixed=0,
+                geometry=zone_geometry
+            )
+
+            zone_dict[zone_id] = zone
+        except Exception as e:
+            print(f"  : Unable to create zone: {zone_id}, error: {e}")
+    return zone_dict
 
-        Returns
-            polygon: sg.Polygon, Polygon
 
-        """
-        return shapely.geometry.Polygon([(x_min, y_min), (x_max, y_min), (x_max, y_max), (x_min, y_max), (x_min, y_min)])
+def _create_zone_from_dataframe_by_centroid(df_zone: pd.DataFrame) -> dict[int, Zone]:
+    """Create Zone from df_zone.
 
+    Args:
+        df_zone (pd.DataFrame): the dataframe of zone from zone.csv, the required fields are: [zone_id, geometry]
+
+    Returns:
+        dict[int, Zone]: a dict of Zones.{zone_id: Zone}
+    """
+    df_zone = df_zone.reset_index(drop=True)
     zone_dict = {}
-    zone_upper_row = []
-    zone_lower_row = []
-    zone_left_col = []
-    zone_right_col = []
-    zone_id_flag = 0
-
-    # convert y from min-max to max-min
-    y_block_maxmin_list = y_block_minmax_list[::-1]
-
-    # generate zone cells with id and labels
-    # id: A1, A2, A3, ...,
-    #     B1, B2, B3, ...,
-    #     C1, C2, C3, ...
-    for j in range(len(y_block_maxmin_list)):
-        for i in range(len(x_block_minmax_list)):
-            x_min = x_block_minmax_list[i][0]
-            x_max = x_block_minmax_list[i][1]
-            y_min = y_block_maxmin_list[j][0]
-            y_max = y_block_maxmin_list[j][1]
-
-            cell_polygon = generate_polygon(x_min, x_max, y_min, y_max)
-            row_alpha = cvt_int_to_alpha(j)
-            zone_dict[f"{row_alpha}{i}"] = Zone(
-                id=zone_id_flag,
-                name=f"{row_alpha}{i}",
-                centroid_x=cell_polygon.centroid.x,
-                centroid_y=cell_polygon.centroid.y,
-                centroid=cell_polygon.centroid,
-                x_min=x_min,
-                x_max=x_max,
-                y_min=y_min,
-                y_max=y_max,
-                geometry=cell_polygon
+
+    for i in range(len(df_zone)):
+        try:
+            zone_id = df_zone.loc[i, 'zone_id']
+            centroid_x = df_zone.loc[i, 'x_coord']
+            centroid_y = df_zone.loc[i, 'y_coord']
+
+            zone_centroid_shapely = shapely.Point(centroid_x, centroid_y)
+            centroid_wkt = zone_centroid_shapely.wkt
+
+            zone = Zone(
+                id=zone_id,
+                name=zone_id,
+                centroid_x=centroid_x,
+                centroid_y=centroid_y,
+                centroid=centroid_wkt,
+                node_id_list=[],
+                poi_id_list=[],
+                production=0,
+                attraction=0,
+                production_fixed=0,
+                attraction_fixed=0,
             )
 
-            # add boundary zone names to list
-            if j == 0:
-                zone_upper_row.append(f"{row_alpha}{i}")
-            if j == len(y_block_maxmin_list) - 1:
-                zone_lower_row.append(f"{row_alpha}{i}")
-
-            if i == 0:
-                zone_left_col.append(f"{row_alpha}{i}")
-            if i == len(x_block_minmax_list) - 1:
-                zone_right_col.append(f"{row_alpha}{i}")
-
-            # update zone id
-            zone_id_flag += 1
-
-    # generate outside boundary centroids
-    upper_points = [shapely.geometry.Point(zone_dict[zone_name].centroid_x,
-                                           zone_dict[zone_name].centroid_y + y_block_height
-                                           ) for zone_name in zone_upper_row]
-    lower_points = [shapely.geometry.Point(zone_dict[zone_name].centroid_x,
-                                           zone_dict[zone_name].centroid_y - y_block_height
-                                           ) for zone_name in zone_lower_row]
-    left_points = [shapely.geometry.Point(zone_dict[zone_name].centroid_x - x_block_width,
-                                          zone_dict[zone_name].centroid_y
-                                          ) for zone_name in zone_left_col]
-    right_points = [shapely.geometry.Point(zone_dict[zone_name].centroid_x + x_block_width,
-                                           zone_dict[zone_name].centroid_y
-                                           ) for zone_name in zone_right_col]
-    points_lst = upper_points + lower_points + left_points + right_points
-    for i in range(len(points_lst)):
-        zone_dict[f"gate{i}"] = Zone(
-            id=zone_id_flag,
-            name=f"gate{i}",
-            centroid_x=points_lst[i].x,
-            centroid_y=points_lst[i].y,
-            centroid=points_lst[i],
-            geometry=points_lst[i]
-        )
-        zone_id_flag += 1
-
-    if verbose:
-        print(f"  : Successfully generated zone dictionary: {len(zone_dict) - 4 * len(zone_upper_row)} Zones generated, \
-            \n    plus {4 * len(zone_upper_row)} boundary gates (points))")
-    return (zone_dict, node_dict_within_boundary)
-
-
-def sync_node_with_zones(args: tuple) -> tuple:
-    node_id, node, zone_dict = args
-    for zone_name in zone_dict:
-        if isinstance(node.geometry, str):
-            node.geometry = shapely.from_wkt(node.geometry)
-        if isinstance(zone_dict[zone_name].geometry, str):
-            zone_dict[zone_name].geometry = shapely.from_wkt(
-                zone_dict[zone_name].geometry)
-
-        if shapely.within(node.geometry, zone_dict[zone_name].geometry):
-            node.zone_id = zone_dict[zone_name].id
-            zone_dict[zone_name].node_id_list.append(node_id)
-            return node_id, node, zone_name
+            zone_dict[zone_id] = zone
+        except Exception as e:
+            print(f"  : Unable to create zone: {zone_id}, error: {e}")
+    return zone_dict
+
 
-    return node_id, node, None
+# main functions for reading node, poi, zone files and network
 
 
 @func_running_time
-def sync_zone_and_node_geometry(zone_dict: dict, node_dict: dict, cpu_cores: int = 1, verbose: bool = False) -> dict:
-    """Map nodes to zone cells
+def read_node(node_file: str = "", cpu_cores: int = 1, verbose: bool = False) -> dict[int: Node]:
+    """Read node.csv file and return a dict of nodes.
 
-    Parameters
-        node_dict: dict, Nodes
-        zone_dict: dict, zone cells
+    Args:
+        node_file (str, optional): node file path. Defaults to "".
+        cpu_cores (int, optional): number of cpu cores for parallel processing. Defaults to 1.
+        verbose (bool, optional): print processing information. Defaults to False.
+
+    Raises:
+        FileNotFoundError: File: {node_file} does not exist.
 
-    Returns
-        node_dict and zone_dict: dict, Update Nodes with zone id, update zone cells with node id list
+    Returns:
+        dict: a dict of nodes.
 
+    Examples:
+        >>> node_dict = read_node(node_file = r"../dataset/ASU/node.csv")
+        >>> node_dict[1]
+        Node(id=1, zone_id=0, x_coord=0.0, y_coord=0.0, boundary_flag=0, geometry='POINT (0 0)',...)
+
+        # if node_file does not exist, raise error
+        >>> node_dict = read_node(node_file = r"../dataset/ASU/node.csv")
+        FileNotFoundError: File: ../dataset/ASU/node.csv does not exist.
     """
-    # Create a pool of worker processes
+
+    # convert path to linux path
+    node_file = path2linux(node_file)
+
+    # check if node_file exists
+    if not os.path.exists(node_file):
+        raise FileNotFoundError(f"File: {node_file} does not exist.")
+
+    # read node.csv with specified columns and chunksize for iterations
+    node_required_cols = pkg_settings["node_fields"]
+    chunk_size = pkg_settings["data_chunk_size"]
+
+    # read first two rows to check whether required fields are in node.csv
+    df_node_2rows = pd.read_csv(node_file, nrows=2)
+    col_names = df_node_2rows.columns.tolist()
+    if "zone_id" in col_names:
+        node_required_cols.append("zone_id")
+
     if verbose:
-        print(f"  : Parallel synchronizing Nodes and Zones using Pool with {cpu_cores} CPUs. Please wait...")
-    # Prepare arguments for the pool
-    args_list = [(node_id, node, zone_dict)
-                 for node_id, node in node_dict.items()]
+        print(f"  : Reading node.csv with specified columns: {node_required_cols} \
+                    \n    and chunksize {chunk_size} for iterations...")
+    df_node_chunk = pd.read_csv(node_file, usecols=node_required_cols, chunksize=chunk_size)
 
-    with Pool(processes=cpu_cores) as pool:
-        results = pool.map(sync_node_with_zones, args_list)
+    if verbose:
+        print(f"  : Parallel creating Nodes using Pool with {cpu_cores} CPUs. Please wait...")
+    node_dict_final = {}
 
-    # Gather results
-    for node_id, node, zone_name in results:
-        if zone_name is not None:
-            zone_dict[zone_name].node_id_list.append(node_id)
-        node_dict[node_id] = node
+    # Parallel processing using Pool
+    with Pool(cpu_cores) as pool:
+        results = pool.map(_create_node_from_dataframe, df_node_chunk)
+
+    for node_dict in results:
+        node_dict_final.update(node_dict)
 
     if verbose:
-        print("  : Successfully synchronized zone and node geometry")
+        print(f"  : Successfully loaded node.csv: {len(node_dict_final)} Nodes loaded.")
+    return node_dict_final
+
 
-    return {"node_dict": node_dict, "zone_dict": zone_dict}
+@func_running_time
+def read_poi(poi_file: str = "", cpu_cores: int = 1, verbose: bool = False) -> dict[int: POI]:
+    """Read poi.csv file and return a dict of POIs.
 
+    Args:
+        poi_file (str): The poi.csv file path. default is "".
+        cpu_cores (int, optional): number of cpu cores for parallel processing. Defaults to 1.
+        verbose (bool, optional): print processing information. Defaults to False.
 
-def sync_poi_with_zones(args: tuple) -> tuple:
-    poi_id, poi, zone_dict = args
-    for zone_name in zone_dict:
-        if isinstance(poi.geometry, str):
-            poi.geometry = shapely.from_wkt(poi.geometry)
-        if isinstance(zone_dict[zone_name].geometry, str):
-            zone_dict[zone_name].geometry = shapely.from_wkt(
-                zone_dict[zone_name].geometry)
+    Raises:
+        FileNotFoundError: if poi_file does not exist.
 
-        if shapely.within(poi.geometry, zone_dict[zone_name].geometry):
-            poi.zone_id = zone_dict[zone_name].id
-            zone_dict[zone_name].poi_id_list.append(poi_id)
-            return poi_id, poi, zone_name
+    Returns:
+        dict: A dict of POIs.
 
-    return poi_id, poi, None
+    Examples:
+        >>> poi_dict = read_poi(poi_file = r"../dataset/ASU/poi.csv")
+        >>> poi_dict[1]
+        POI(id=1, x_coord=0.0, y_coord=0.0, area=[0, 0.0], poi_type='residential', geometry='POINT (0 0)')
+
+        # if poi_file does not exist, raise error
+        >>> poi_dict = read_poi(poi_file = r"../dataset/ASU/poi.csv")
+        FileNotFoundError: File: ../dataset/ASU/poi.csv does not exist.
+
+    """
+
+    # convert path to linux path
+    poi_file = path2linux(poi_file)
+
+    # check if poi_file exists
+    if not os.path.exists(poi_file):
+        raise FileNotFoundError(f"File: {poi_file} does not exist.")
+
+    # Read poi.csv with specified columns and chunksize for iterations
+    poi_required_cols = pkg_settings["poi_fields"]
+    chunk_size = pkg_settings["data_chunk_size"]
+
+    if verbose:
+        print(f"  : Reading poi.csv with specified columns: {poi_required_cols} \
+                    \n    and chunksize {chunk_size} for iterations...")
+    df_poi_chunk = pd.read_csv(poi_file, usecols=poi_required_cols, chunksize=chunk_size)
+
+    # Parallel processing using Pool
+    if verbose:
+        print(f"  : Parallel creating POIs using Pool with {cpu_cores} CPUs. Please wait...")
+    poi_dict_final = {}
+
+    with Pool(cpu_cores) as pool:
+        results = pool.map(_create_poi_from_dataframe, df_poi_chunk)
+
+    for poi_dict in results:
+        poi_dict_final.update(poi_dict)
+
+    if verbose:
+        print(f"  : Successfully loaded poi.csv: {len(poi_dict_final)} POIs loaded.")
+
+    return poi_dict_final
 
 
 @func_running_time
-def sync_zone_and_poi_geometry(zone_dict: dict, poi_dict: dict, cpu_cores: int = 1, verbose: bool = False) -> dict:
-    """Synchronize zone cells and POIs to update zone_id attribute for POIs and poi_id_list attribute for zone cells
+def read_zone_by_geometry(zone_file: str = "", cpu_cores: int = 1, verbose: bool = False) -> dict[int: Zone]:
+    """Read zone.csv file and return a dict of Zones.
+
+    Raises:
+        FileNotFoundError: _description_
+        FileNotFoundError: _description_
 
     Args:
-        zone_dict (dict): Zone cells
-        poi_dict (dict): POIs
+        zone_file (str, optional): the input zone file path. Defaults to "".
+        cpu_cores (int, optional): number of cpu cores for parallel processing. Defaults to 1.
+        verbose (bool, optional): print processing information. Defaults to False.
 
     Returns:
-        dict: the updated zone_dict and poi_dict
+        _type_: _description_
     """
 
-    # Create a pool of worker processes
+    # convert path to linux path
+    zone_file = path2linux(zone_file)
+
+    # check if zone_file exists
+    if not os.path.exists(zone_file):
+        raise FileNotFoundError(f"File: {zone_file} does not exist.")
+
+    # load default settings for zone required fields and chunk size
+    zone_required_cols = pkg_settings["zone_geometry_fields"]
+    chunk_size = pkg_settings["data_chunk_size"]
+
     if verbose:
-        print(f"  : Parallel synchronizing POIs and Zones using Pool with {cpu_cores} CPUs. Please wait...")
-    # Prepare arguments for the pool
-    args_list = [(poi_id, poi, zone_dict) for poi_id, poi in poi_dict.items()]
-
-    with Pool(processes=cpu_cores) as pool:
-        # Distribute work to the pool
-        results = pool.map(sync_poi_with_zones, args_list)
-
-    # Gather results
-    for poi_id, poi, zone_name in results:
-        if zone_name is not None:
-            zone_dict[zone_name].poi_id_list.append(poi_id)
-        poi_dict[poi_id] = poi
-
-    if verbose:
-        print("  : Successfully synchronized zone and poi geometry")
-    return {"poi_dict": poi_dict, "zone_dict": zone_dict}
-
-
-def distance_calculation(args: tuple) -> tuple:
-    i, j, df_zone = args
-    return (
-        (df_zone.loc[i, 'name'], df_zone.loc[j, 'name']),
-        {
-            "o_zone_id": df_zone.loc[i, 'id'],
-            "o_zone_name": df_zone.loc[i, 'name'],
-            "d_zone_id": df_zone.loc[j, 'id'],
-            "d_zone_name": df_zone.loc[j, 'name'],
-            "dist_km": calc_distance_on_unit_sphere(
-                df_zone.loc[i, 'centroid'],
-                df_zone.loc[j, 'centroid'],
-                unit='km'),
-            "volume": 0,
-            "geometry": shapely.LineString(
-                [df_zone.loc[i, 'centroid'], df_zone.loc[j, 'centroid']]),
-        }
-    )
+        print(f"  : Reading zone.csv with specified columns: {zone_required_cols} \
+                \n   and chunksize {chunk_size} for iterations...")
+
+    # check whether required fields are in zone.csv
+    df_zone = pd.read_csv(zone_file, nrows=1)
+    col_names = df_zone.columns.tolist()
+    for col in zone_required_cols:
+        if col not in col_names:
+            raise FileNotFoundError(f"Required column: {col} is not in zone.csv. \
+                Please make sure you have {zone_required_cols} in zone.csv.")
+
+    # load zone.csv with specified columns and chunksize for iterations
+    df_zone_chunk = pd.read_csv(zone_file, usecols=zone_required_cols, chunksize=chunk_size)
+
+    # Parallel processing using Pool
+    if verbose:
+        print(f"  : Parallel creating Zones using Pool with {cpu_cores} CPUs. Please wait...")
+    zone_dict_final = {}
+
+    with Pool(cpu_cores) as pool:
+        results = pool.map(_create_zone_from_dataframe_by_geometry, df_zone_chunk)
+
+    for zone_dict in results:
+        zone_dict_final.update(zone_dict)
+
+    if verbose:
+        print(f"  : Successfully loaded zone.csv: {len(zone_dict_final)} Zones loaded.")
+
+    return zone_dict_final
 
 
 @func_running_time
-def calc_zone_od_matrix(zone_dict: dict, cpu_cores: int = 1, verbose: bool = False) -> dict[tuple[str, str], dict]:
-    """Calculate the zone-to-zone distance matrix
+def read_zone_by_centroid(zone_file: str = "", cpu_cores: int = 1, verbose: bool = False) -> dict[int: Zone]:
+    """Read zone.csv file and return a dict of Zones.
 
     Args:
-        zone_dict (dict): Zone cells
+        zone_file (str, optional): the input zone file path. Defaults to "".
+        cpu_cores (int, optional): number of cpu cores for parallel processing. Defaults to 1.
+        verbose (bool, optional): print processing information. Defaults to False.
+
+    Raises:
+        FileNotFoundError: File: {zone_file} does not exist.
+        FileNotFoundError: Required column: {col} is not in zone.csv. Please make sure zone_required_cols in zone.csv.
 
     Returns:
-        dict: the zone-to-zone distance matrix
+        dict: a dict of Zones.
     """
 
-    # convert zone_dict to dataframe
-    df_zone = pd.DataFrame(zone_dict.values())
+    # convert path to linux path
+    zone_file = path2linux(zone_file)
 
-    # convert centroid from str to shapely.geometry.Point
-    if isinstance(df_zone.loc[0, 'centroid'], str):
-        df_zone['centroid'] = df_zone["centroid"].apply(shapely.from_wkt)
+    # check if zone_file exists
+    if not os.path.exists(zone_file):
+        raise FileNotFoundError(f"File: {zone_file} does not exist.")
+
+    # load default settings for zone required fields and chunk size
+    zone_required_cols = pkg_settings["zone_centroid_fields"]
+    chunk_size = pkg_settings["data_chunk_size"]
 
-    len_df_zone = len(df_zone)
+    if verbose:
+        print(f"  : Reading zone.csv with specified columns: {zone_required_cols} \
+                \n   and chunksize {chunk_size} for iterations...")
+
+    # check whether required fields are in zone.csv
+    df_zone = pd.read_csv(zone_file, nrows=1)
+    col_names = df_zone.columns.tolist()
+    for col in zone_required_cols:
+        if col not in col_names:
+            raise FileNotFoundError(f"Required column: {col} is not in zone.csv. \
+                Please make sure you have {zone_required_cols} in zone.csv.")
+
+    # load zone.csv with specified columns and chunksize for iterations
+    df_zone_chunk = pd.read_csv(zone_file, usecols=zone_required_cols, chunksize=chunk_size)
 
-    # Prepare arguments for the pool
+    # Parallel processing using Pool
     if verbose:
-        print(f"  : Parallel calculating zone-to-zone distance matrix using Pool with {cpu_cores} CPUs. Please wait...")
-    args_list = [(i, j, df_zone) for i, j in itertools.product(range(len_df_zone), range(len_df_zone))]
+        print(f"  : Parallel creating Zones using Pool with {cpu_cores} CPUs. Please wait...")
 
-    with Pool(processes=cpu_cores) as pool:
-        # Distribute work to the pool
-        results = pool.map(distance_calculation, args_list)
+    zone_dict_final = {}
 
-    # Gather results
-    dist_dict = dict(results)
+    with Pool(cpu_cores) as pool:
+        results = pool.map(_create_zone_from_dataframe_by_centroid, df_zone_chunk)
+
+    for zone_dict in results:
+        zone_dict_final.update(zone_dict)
 
     if verbose:
-        print("  : Successfully calculated zone-to-zone distance matrix")
-    return dist_dict
+        print(f"  : Successfully loaded zone.csv: {len(zone_dict_final)} Zones loaded.")
+
+    return zone_dict_final
+
+
+def read_network(input_folder: str = "", cpu_cores: int = 1, verbose: bool = False) -> dict[str: dict]:
+    """Read node.csv and poi.csv files and return a dict of nodes and a dict of POIs.
+
+    Args:
+        input_folder (str, optional): required files within this folder. Defaults to current folder.
+        cpu_cores (int, optional): number of cpu cores for parallel processing. Defaults to 1.
+        verbose (bool, optional): print processing information. Defaults to False.
+
+    Raises:
+        FileNotFoundError: if input_folder does not exist.
+
+    Returns:
+        dict: a dict of nodes and a dict of POIs.
+
+    Examples:
+        >>> node_dict, poi_dict = read_network(input_folder = r"../dataset/ASU")
+        >>> node_dict[1]
+        Node(id=1, zone_id=0, x_coord=0.0, y_coord=0.0, production=0.0, attraction=0.0, boundary_flag=0,
+        >>> poi_dict[1]
+        POI(id=1, x_coord=0.0, y_coord=0.0, area=[0, 0.0], poi_type='residential', geometry='POINT (0 0)')
+
+        # if input_folder is not specified, use current folder
+        >>> node_dict, poi_dict = read_network()
+
+        # if required files are not satisfied, raise error
+        >>> node_dict, poi_dict = read_network(input_folder = r"../dataset/ASU")
+        FileNotFoundError: Required files: ['node.csv', 'poi.csv'] are not satisfied, please check your input folder.
+    """
+
+    # set input folder to current folder if not specified
+    if not input_folder:
+        input_folder = os.getcwd()
+
+    # convert path to linux path
+    input_folder = path2linux(input_folder)
+
+    # check if input_folder exists
+    if not os.path.isdir(input_folder):
+        raise FileNotFoundError(f"Input folder: {input_folder} does not exist.")
+
+    # get all csv files in the folder
+    dir_files = get_filenames_by_ext(input_folder, "csv")
+
+    # check if required files exist
+    is_required_files_exist = check_required_files_exist(pkg_settings["required_files"], dir_files)
+
+    # if not all required files exist, raise error
+    if not is_required_files_exist:
+        raise FileNotFoundError(
+            f"Required files: {pkg_settings['required_files']} are not satisfied, please check your input folder.")
+
+    node_dict = read_node(input_folder + "/node.csv", cpu_cores, verbose=verbose)
+    poi_dict = read_poi(input_folder + "/poi.csv", cpu_cores, verbose=verbose)
+
+    if verbose:
+        print(f"  : Successfully loaded node.csv and poi.csv: {len(node_dict)} Nodes and {len(poi_dict)} POIs.")
+
+    return {"node_dict": node_dict, "poi_dict": poi_dict}
```

### Comparing `grid2demand-0.4.2/grid2demand/func_lib/gravity_model.py` & `grid2demand-0.4.3/grid2demand/func_lib/gravity_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
     if verbose:
         print("  : Successfully calculated zone production and attraction based on node production and attraction.")
 
     return zone_dict
 
 
-def calc_zone_od_friction_attraction(zone_od_friction_matrix_dict: dict, zone_dict: dict, verbose: bool = False) -> dict:
+def calc_zone_od_friction_attraction(zone_od_friction_matrix_dict: dict,
+                                     zone_dict: dict,
+                                     verbose: bool = False) -> dict:
     zone_od_friction_attraction_dict = {}
     for zone_name, friction_val in zone_od_friction_matrix_dict.items():
         if zone_name[0] not in zone_od_friction_attraction_dict:
             zone_od_friction_attraction_dict[zone_name[0]] = friction_val * zone_dict[zone_name[1]].attraction
         else:
             zone_od_friction_attraction_dict[zone_name[0]] += friction_val * zone_dict[zone_name[1]].attraction
 
@@ -55,27 +57,33 @@
         gamma = trip_purpose_dict[trip_purpose]["gamma"]
 
     # update zone attraction and production
     # zone_dict = calc_zone_production_attraction(node_dict, zone_dict)
 
     # perform zone od friction matrix
     zone_od_friction_matrix_dict = {
-        zone_name_pair: alpha * (od_dist["dist_km"] ** beta) * (np.exp(od_dist["dist_km"] * gamma)) if od_dist["dist_km"] != 0 else 0
+        zone_name_pair: alpha * (od_dist["dist_km"] ** beta) * (
+            np.exp(od_dist["dist_km"] * gamma)) if od_dist["dist_km"] != 0 else 0
         for zone_name_pair, od_dist in zone_od_dist_matrix.items()
     }
 
     # perform attraction calculation
-    zone_od_friction_attraction_dict = calc_zone_od_friction_attraction(zone_od_friction_matrix_dict, zone_dict, verbose=verbose)
+    zone_od_friction_attraction_dict = calc_zone_od_friction_attraction(zone_od_friction_matrix_dict,
+                                                                        zone_dict,
+                                                                        verbose=verbose)
 
     # perform od trip flow (volume) calculation
     for zone_name_pair in zone_od_friction_matrix_dict:
-        zone_od_dist_matrix[zone_name_pair]["volume"] = float(zone_dict[zone_name_pair[0]].production *
-                                                              zone_dict[zone_name_pair[1]].attraction *
-                                                              zone_od_friction_matrix_dict[zone_name_pair] /
-                                                              zone_od_friction_attraction_dict[zone_name_pair[0]])
+        try:
+            zone_od_dist_matrix[zone_name_pair]["volume"] = float(zone_dict[zone_name_pair[0]].production *
+                                                                  zone_dict[zone_name_pair[1]].attraction *
+                                                                  zone_od_friction_matrix_dict[zone_name_pair] /
+                                                                  zone_od_friction_attraction_dict[zone_name_pair[0]])
+        except ZeroDivisionError:
+            zone_od_dist_matrix[zone_name_pair]["volume"] = 0
 
     # Generate demand.csv
     if verbose:
         print("  : Successfully run gravity model to generate demand.csv.")
 
     # return pd.DataFrame(list(zone_od_matrix_dict.values()))
     return zone_od_dist_matrix
```

### Comparing `grid2demand-0.4.2/grid2demand/func_lib/trip_rate_production_attraction.py` & `grid2demand-0.4.3/grid2demand/func_lib/trip_rate_production_attraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     Returns:
         dict: the dictionary of poi with trip rate
 
     Examples:
         >>> poi_dict = gd.read_poi("./dataset/ASU/poi.csv")
         >>> poi_trip_rate = gd.gen_poi_trip_rate(poi_dict, trip_rate_file="./dataset/ASU/trip_rate.csv", trip_purpose=1)
         >>> poi_trip_rate[0]
-        POI(poi_id=0, poi_type='residential', x=0.0, y=0.0, area=(0.0, 0.0), trip_rate={'building': 'residential', 'unit_of_measure': '1,000 Sq. Ft. GFA', 'trip_purpose': 1, 'production_rate1': 10.0, 'attraction_rate1': 10.0, 'production_notes': 1, 'attraction_notes': 1})
+        POI(poi_id=0, poi_type='residential', x=0.0, y=0.0, area=(0.0, 0.0), trip_rate={'building': 'residential',
+        'unit_of_measure': '1,000 Sq. Ft. GFA', 'trip_purpose': 1, 'production_rate1': 10.0,
+        'attraction_rate1': 10.0, 'production_notes': 1, 'attraction_notes': 1})
     """
     poi_purpose_prod_dict = pkg_settings.get("poi_purpose_prod_dict")
     poi_purpose_attr_dict = pkg_settings.get("poi_purpose_attr_dict")
 
     default_flag = False
 
     # if no poi trip rate file provided, use default trip rate
@@ -106,24 +108,25 @@
     """Generate production and attraction for each node.
 
     Args:
         node_dict (dict): Node dictionary
         poi_dict (dict): POI dictionary
         residential_production (float, optional): the production of residential area. Defaults to 10.0.
         residential_attraction (float, optional): the attraction of residential area. Defaults to 10.0.
-        boundary_production (float, optional): the boundary production, also known as the outside production. Defaults to 1000.0.
-        boundary_attraction (float, optional): the boundary attraction, also known as the outside attraction. Defaults to 1000.0.
+        boundary_production (float, optional): boundary production, also outside production. Defaults to 1000.0.
+        boundary_attraction (float, optional): boundary attraction, also the outside attraction. Defaults to 1000.0.
 
     Returns:
         dict: Node dictionary with generated production and attraction
 
     Examples:
         >>> node_dict = gd.read_node("./dataset/ASU/node.csv")
         >>> poi_dict = gd.read_poi("./dataset/ASU/poi.csv")
-        >>> node_prod_attr = gd.gen_node_prod_attr(node_dict, poi_dict, residential_production=10.0, residential_attraction=10.0, boundary_production=1000.0, boundary_attraction=1000.0)
+        >>> node_prod_attr = gd.gen_node_prod_attr(node_dict, poi_dict, residential_production=10.0,
+        residential_attraction=10.0, boundary_production=1000.0, boundary_attraction=1000.0)
         >>> node_prod_attr[1]
         Node(node_id=1, poi_id=0, x=0.0, y=0.0, activity_location_tab='residential', production=10.0, attraction=10.0)
     """
 
     for node in node_dict.values():
         if node.activity_location_tab == "residential":
             node.production = residential_production
```

### Comparing `grid2demand-0.4.2/grid2demand/utils_lib/net_utils.py` & `grid2demand-0.4.3/grid2demand/utils_lib/net_utils.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.2/grid2demand/utils_lib/pkg_settings.py` & `grid2demand-0.4.3/grid2demand/utils_lib/pkg_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 pkg_settings = {
     # specify required files for grid2demand, and optional files for grid2demand
     "required_files": ["node.csv", "poi.csv"],
     "optional_files": ["zone.csv"],
 
     # specify required fields for node.csv and poi.csv and zone.csv (optional)
-    "node_required_fields": ["node_id", "x_coord", "y_coord",
-                             "activity_type", "is_boundary", "poi_id"],
-    "poi_required_fields": ["poi_id", "building", "centroid", "area", "geometry"],
-    "zone_required_fields": ["zone_id", "geometry"],
+    "node_fields": ["node_id", "x_coord", "y_coord",
+                    "activity_type", "is_boundary", "poi_id"],
+    "poi_fields": ["poi_id", "building", "centroid", "area", "geometry"],
+    "zone_geometry_fields": ["zone_id", "geometry"],
+    "zone_centroid_fields": ["zone_id", "x_coord", "y_coord"],
 
     # if input data is too large, you can split the input data into chunks and process them separately
     "data_chunk_size": 10000,
 
     # run the program in parallel mode, if cpu_cores > 1
     "set_cpu_cores": os.cpu_count(),
```

### Comparing `grid2demand-0.4.2/grid2demand/utils_lib/utils.py` & `grid2demand-0.4.3/grid2demand/utils_lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,21 +159,23 @@
 
     try:
         return path.replace("\\", "/")
     except Exception:
         return str(path).replace("\\", "/")
 
 
-def get_filenames_from_folder_by_type(dir_name: str, file_type: str = "txt", isTraverseSubdirectory: bool = False) -> list:
+def get_filenames_from_folder_by_type(dir_name: str,
+                                      file_type: str = "txt",
+                                      isTraverseSubdirectory: bool = False) -> list:
     """Get all files in the folder with the specified file type
 
     Args:
         dir_name (str): the folder path
-        file_type (str, optional): the exact file type to specify, if file_type is "*" or "all", return all files in the folder. Defaults to "txt".
-        isTraverseSubdirectory (bool, optional): get files inside the subfolder or not, if True, will traverse all subfolders. Defaults to False.
+        file_type (str, optional): file type to specify, if "*" or "all", return all files in folder. Defaults to "txt".
+        isTraverseSubdirectory (bool, optional): traverse all sub-folders or not. Defaults to False.
 
     Returns:
         list: a list of file paths
 
     Examples:
         # get all files in the folder without traversing subfolder
         >>> from pyhelpers.dirs import get_filenames_from_folder_by_type
```

### Comparing `grid2demand-0.4.2/grid2demand.egg-info/SOURCES.txt` & `grid2demand-0.4.3/grid2demand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.2/setup.py` & `grid2demand-0.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in f.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="grid2demand",  # Replace with your own username
-    version="0.4.2",
+    version="0.4.3",
     author="Xiangyong Luo, Dr.Xuesong(Simon) Zhou, Anjun Li, Entai Wang, Taehooie Kim",
     author_email="luoxiangyong01@gmail.com, xzhou74@asu.edu",
     description="A tool for generating zone-to-zone travel demand based on grid zones and gravity model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xyluo25/grid2demand",
```

### Comparing `grid2demand-0.4.2/tests/test_read_node.py` & `grid2demand-0.4.3/tests/test_read_node.py`

 * *Files identical despite different names*

