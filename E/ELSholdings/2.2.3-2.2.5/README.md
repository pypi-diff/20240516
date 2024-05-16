# Comparing `tmp/elsholdings-2.2.3.tar.gz` & `tmp/elsholdings-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elsholdings-2.2.3.tar", last modified: Thu May 16 02:01:43 2024, max compression
+gzip compressed data, was "elsholdings-2.2.5.tar", last modified: Thu May 16 04:49:12 2024, max compression
```

## Comparing `elsholdings-2.2.3.tar` & `elsholdings-2.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 02:01:43.995366 elsholdings-2.2.3/
-drwxrwxrwx   0        0        0        0 2024-05-16 02:01:43.961809 elsholdings-2.2.3/ELSholdings/
-drwxrwxrwx   0        0        0        0 2024-05-16 02:01:43.990366 elsholdings-2.2.3/ELSholdings/kenwoo/
--rw-rw-rw-   0        0        0    46067 2024-05-15 22:45:21.000000 elsholdings-2.2.3/ELSholdings/kenwoo/xls2ppt.py
--rw-rw-rw-   0        0        0    46032 2024-05-16 02:01:15.000000 elsholdings-2.2.3/ELSholdings/kenwoo/xls2ppt_pc.py
-drwxrwxrwx   0        0        0        0 2024-05-16 02:01:43.992365 elsholdings-2.2.3/ELSholdings.egg-info/
--rw-rw-rw-   0        0        0      425 2024-05-16 02:01:43.000000 elsholdings-2.2.3/ELSholdings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-05-16 02:01:43.000000 elsholdings-2.2.3/ELSholdings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 02:01:43.000000 elsholdings-2.2.3/ELSholdings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 02:01:43.000000 elsholdings-2.2.3/ELSholdings.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      425 2024-05-16 02:01:43.994366 elsholdings-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.2.3/README.md
--rw-rw-rw-   0        0        0      366 2024-05-16 02:01:26.000000 elsholdings-2.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 02:01:43.995366 elsholdings-2.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 04:49:12.056450 elsholdings-2.2.5/
+drwxrwxrwx   0        0        0        0 2024-05-16 04:49:12.020374 elsholdings-2.2.5/ELSholdings/
+drwxrwxrwx   0        0        0        0 2024-05-16 04:49:12.051445 elsholdings-2.2.5/ELSholdings/kenwoo/
+-rw-rw-rw-   0        0        0    46067 2024-05-15 22:45:21.000000 elsholdings-2.2.5/ELSholdings/kenwoo/xls2ppt.py
+-rw-rw-rw-   0        0        0    45972 2024-05-16 04:43:57.000000 elsholdings-2.2.5/ELSholdings/kenwoo/xls2ppt_pc.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:49:12.053444 elsholdings-2.2.5/ELSholdings.egg-info/
+-rw-rw-rw-   0        0        0      425 2024-05-16 04:49:11.000000 elsholdings-2.2.5/ELSholdings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-05-16 04:49:12.000000 elsholdings-2.2.5/ELSholdings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 04:49:12.000000 elsholdings-2.2.5/ELSholdings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 04:49:12.000000 elsholdings-2.2.5/ELSholdings.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      425 2024-05-16 04:49:12.055446 elsholdings-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.2.5/README.md
+-rw-rw-rw-   0        0        0      366 2024-05-16 04:49:00.000000 elsholdings-2.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 04:49:12.057459 elsholdings-2.2.5/setup.cfg
```

### Comparing `elsholdings-2.2.3/ELSholdings/kenwoo/xls2ppt.py` & `elsholdings-2.2.5/ELSholdings/kenwoo/xls2ppt.py`

 * *Files identical despite different names*

### Comparing `elsholdings-2.2.3/ELSholdings/kenwoo/xls2ppt_pc.py` & `elsholdings-2.2.5/ELSholdings/kenwoo/xls2ppt_pc.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,14 @@
 
     ##########################################
     ########### PPT 자료 작성하기: Colab
     ###########################################
     from pandas_datareader import data as pdr
     import yfinance as yfin
 
-    file_out_ppt= '/content/drive/MyDrive/PPT_Output.xlsx'
 
     # Daily info 정리하기
     df_Daily_NAV_summary=df_Daily_NAV.iloc[:, [0] + list(range(-17, 0))] # 처음과 마지막 17개의 칼럼만 추출
     imsi=df_Daily_NAV_Market_Cap['날짜별발행잔액']/1e+9
     df_Daily_NAV_summary.loc[:, '시장가치잔액(10억)'] = imsi
```

