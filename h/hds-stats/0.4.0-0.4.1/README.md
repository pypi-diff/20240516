# Comparing `tmp/hds_stats-0.4.0.tar.gz` & `tmp/hds_stats-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds_stats-0.4.0.tar", last modified: Tue May 14 21:44:31 2024, max compression
+gzip compressed data, was "hds_stats-0.4.1.tar", last modified: Thu May 16 11:10:50 2024, max compression
```

## Comparing `hds_stats-0.4.0.tar` & `hds_stats-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-14 21:44:31.822028 hds_stats-0.4.0/
--rw-------   0 seonghona   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds_stats-0.4.0/LICENSE
--rw-r--r--   0 seonghona   (501) staff       (20)      829 2024-05-14 21:44:31.821457 hds_stats-0.4.0/PKG-INFO
--rw-------   0 seonghona   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds_stats-0.4.0/README.md
-drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-14 21:44:31.818495 hds_stats-0.4.0/hds_stats/
--rw-------   0 seonghona   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds_stats-0.4.0/hds_stats/__init__.py
--rw-------   0 seonghona   (501) staff       (20)    10483 2024-05-14 03:26:39.000000 hds_stats-0.4.0/hds_stats/ml.py
--rw-------   0 seonghona   (501) staff       (20)    13163 2024-05-14 03:26:38.000000 hds_stats-0.4.0/hds_stats/plot.py
--rw-------   0 seonghona   (501) staff       (20)    28176 2024-05-14 03:26:38.000000 hds_stats-0.4.0/hds_stats/stat.py
-drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-14 21:44:31.820936 hds_stats-0.4.0/hds_stats.egg-info/
--rw-r--r--   0 seonghona   (501) staff       (20)      829 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/PKG-INFO
--rw-------   0 seonghona   (501) staff       (20)      279 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/SOURCES.txt
--rw-------   0 seonghona   (501) staff       (20)        1 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/dependency_links.txt
--rw-------   0 seonghona   (501) staff       (20)       72 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/requires.txt
--rw-------   0 seonghona   (501) staff       (20)       23 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/top_level.txt
--rw-------   0 seonghona   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds_stats-0.4.0/pyproject.toml
--rw-r--r--   0 seonghona   (501) staff       (20)       38 2024-05-14 21:44:31.822156 hds_stats-0.4.0/setup.cfg
--rw-------   0 seonghona   (501) staff       (20)     1210 2024-05-13 23:36:17.000000 hds_stats-0.4.0/setup.py
+drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-16 11:10:50.225015 hds_stats-0.4.1/
+-rw-------   0 seonghona   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds_stats-0.4.1/LICENSE
+-rw-r--r--   0 seonghona   (501) staff       (20)      829 2024-05-16 11:10:50.224514 hds_stats-0.4.1/PKG-INFO
+-rw-------   0 seonghona   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds_stats-0.4.1/README.md
+drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-16 11:10:50.221363 hds_stats-0.4.1/hds_stats/
+-rw-------   0 seonghona   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds_stats-0.4.1/hds_stats/__init__.py
+-rw-------   0 seonghona   (501) staff       (20)    10483 2024-05-14 03:26:39.000000 hds_stats-0.4.1/hds_stats/ml.py
+-rw-------   0 seonghona   (501) staff       (20)    13223 2024-05-16 11:07:48.000000 hds_stats-0.4.1/hds_stats/plot.py
+-rw-------   0 seonghona   (501) staff       (20)    28176 2024-05-14 03:26:38.000000 hds_stats-0.4.1/hds_stats/stat.py
+drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-16 11:10:50.224008 hds_stats-0.4.1/hds_stats.egg-info/
+-rw-r--r--   0 seonghona   (501) staff       (20)      829 2024-05-16 11:10:50.000000 hds_stats-0.4.1/hds_stats.egg-info/PKG-INFO
+-rw-------   0 seonghona   (501) staff       (20)      279 2024-05-16 11:10:50.000000 hds_stats-0.4.1/hds_stats.egg-info/SOURCES.txt
+-rw-------   0 seonghona   (501) staff       (20)        1 2024-05-16 11:10:50.000000 hds_stats-0.4.1/hds_stats.egg-info/dependency_links.txt
+-rw-------   0 seonghona   (501) staff       (20)       72 2024-05-16 11:10:50.000000 hds_stats-0.4.1/hds_stats.egg-info/requires.txt
+-rw-------   0 seonghona   (501) staff       (20)       23 2024-05-16 11:10:50.000000 hds_stats-0.4.1/hds_stats.egg-info/top_level.txt
+-rw-------   0 seonghona   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds_stats-0.4.1/pyproject.toml
+-rw-r--r--   0 seonghona   (501) staff       (20)       38 2024-05-16 11:10:50.225115 hds_stats-0.4.1/setup.cfg
+-rw-------   0 seonghona   (501) staff       (20)     1210 2024-05-16 11:10:02.000000 hds_stats-0.4.1/setup.py
```

### Comparing `hds_stats-0.4.0/LICENSE` & `hds_stats-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hds_stats-0.4.0/PKG-INFO` & `hds_stats-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.4.0
+Version: 0.4.1
 Summary: Useful functions for EDA, Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds_stats-0.4.0/hds_stats/ml.py` & `hds_stats-0.4.1/hds_stats/ml.py`

 * *Files identical despite different names*

### Comparing `hds_stats-0.4.0/hds_stats/plot.py` & `hds_stats-0.4.1/hds_stats/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,18 +143,18 @@
     # x_max = data[x].max()
     # plt.xlim(x_min * 0.9, x_max * 1.1)
     
     plt.title(label = f'{x}와(과) {y}의 관계', 
               fontdict = {'fontweight': 'bold'});
 
 
-# 범주형 변수의 빈도수로 막대 그래프를 그리는 함수
+# 범주형 변수의 도수로 막대 그래프를 그리는 함수
 def bar_freq(data, x: str, color: str = None, pal: list = None) -> None:
     '''
-    이 함수는 범주형 변수의 빈도수를 내림차순 정렬한 막대 그래프를 그립니다.
+    이 함수는 범주형 변수의 도수를 내림차순 정렬한 막대 그래프를 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 범주형 변수명을 문자열로 지정합니다.
         color: 점의 채우기 색을 문자열로 지정합니다.
         pal: 팔레트를 리스트로 지정합니다.
     
@@ -192,22 +192,22 @@
             c = 'black', 
             fontsize = 8, 
             fontweight = 'bold'
         )
     
     plt.ylim(0, v_max * 1.2)
     
-    plt.title(label = '목표변수의 범주별 빈도수 비교', 
+    plt.title(label = '목표변수의 범주별 도수 비교', 
               fontdict = {'fontweight': 'bold'});
 
 
-# 범주형 변수를 소그룹으로 나누고 빈도수로 펼친 막대 그래프를 그리는 함수
+# 범주형 변수를 소그룹으로 나누고 도수로 펼친 막대 그래프를 그리는 함수
 def bar_dodge_freq(data, x: str, group: str, pal: list = None) -> None:
     '''
-    이 함수는 범주형 변수를 소그룹으로 나누고 빈도수로 펼친 막대 그래프를 그립니다.
+    이 함수는 범주형 변수를 소그룹으로 나누고 도수로 펼친 막대 그래프를 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 범주형 변수명을 문자열로 지정합니다.
         group: x를 소그룹으로 나눌 범주형 변수명을 문자열로 지정합니다.
         pal: 팔레트를 리스트로 지정합니다.
     
@@ -248,26 +248,26 @@
             va = 'bottom', 
             fontsize = 8, 
             fontweight = 'bold'
         )
     
     plt.ylim(0, v_max * 1.2)
     
-    plt.title(label = f'{x}의 범주별 {group}의 빈도수 비교', 
+    plt.title(label = f'{x}의 범주별 {group}의 도수 비교', 
               fontdict = {'fontweight': 'bold'})
     
     plt.legend(loc = 'center left', 
                bbox_to_anchor = (1, 0.5), 
                fontsize = 8);
 
 
-# 범주형 변수를 소그룹으로 나누고 빈도수로 쌓은 막대 그래프를 그리는 함수
+# 범주형 변수를 소그룹으로 나누고 도수로 쌓은 막대 그래프를 그리는 함수
 def bar_stack_freq(data, x: str, group: str, kind: str = 'bar', pal: list = None) -> None:
     '''
-    이 함수는 범주형 변수를 소그룹으로 나누고 빈도수로 쌓은 막대 그래프를 그립니다.
+    이 함수는 범주형 변수를 소그룹으로 나누고 도수로 쌓은 막대 그래프를 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 범주형 변수명을 문자열로 지정합니다.
         group: x를 소그룹으로 나눌 범주형 변수명을 문자열로 지정합니다.
         kind: 막대 그래프의 종류를 'bar' 또는 'barh'로 지정합니다.(기본값: 'bar')
         pal: 팔레트를 리스트로 지정합니다.
@@ -306,15 +306,14 @@
         pal = sns.set_palette(sns.color_palette(pal))
     
     pv.plot(
         x = x, 
         kind = kind, 
         stacked = True, 
         rot = 0, 
-        title = f'{x}의 범주별 {group}의 빈도수 비교', 
         legend = 'reverse', 
         colormap = pal
     )
     
     if kind == 'bar':
         for col in cols:
             for i, (v1, v2) in enumerate(zip(cumsum[col], pv[col])):
@@ -338,14 +337,17 @@
                     ha = 'center', 
                     va = 'center', 
                     c = 'black', 
                     fontsize = 8, 
                     fontweight = 'bold'
                 )
 
+    plt.title(label = f'{x}의 범주별 {group}의 도수 비교', 
+              fontweight = 'bold')
+    
     plt.legend(loc = 'center left', 
                bbox_to_anchor = (1, 0.5), 
                fontsize = 8);
 
 
 # 범주형 변수를 소그룹으로 나누고 상대도수로 쌓은 막대 그래프를 그리는 함수
 def bar_stack_prop(data, x: str, group: str, kind: str = 'bar', pal: list = None) -> None:
@@ -397,15 +399,14 @@
         pal = sns.set_palette(sns.color_palette(pal))
         
     pv.plot(
         x = x, 
         kind = kind, 
         stacked = True, 
         rot = 0, 
-        title = f'{x}의 범주별 {group}의 상대도수 비교', 
         legend = 'reverse', 
         colormap = pal, 
         mark_right = True
     )
     
     if kind == 'bar':
         for col in cols:
@@ -431,14 +432,16 @@
                     s = v3, 
                     ha = 'center', 
                     va = 'center', 
                     c = 'black', 
                     fontsize = 8, 
                     fontweight = 'bold'
                 )
+    plt.title(label = f'{x}의 범주별 {group}의 상대도수 비교', 
+              fontweight = 'bold')
     
     plt.legend(loc = 'center left', 
                bbox_to_anchor = (1, 0.5), 
                fontsize = 8);
 
 
 ## End of Document
```

### Comparing `hds_stats-0.4.0/hds_stats/stat.py` & `hds_stats-0.4.1/hds_stats/stat.py`

 * *Files identical despite different names*

### Comparing `hds_stats-0.4.0/hds_stats.egg-info/PKG-INFO` & `hds_stats-0.4.1/hds_stats.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.4.0
+Version: 0.4.1
 Summary: Useful functions for EDA, Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds_stats-0.4.0/setup.py` & `hds_stats-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.4.0',
+    version = '0.4.1',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for EDA, Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

