# Comparing `tmp/elsholdings-2.0.1.tar.gz` & `tmp/elsholdings-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elsholdings-2.0.1.tar", last modified: Wed May 15 22:22:08 2024, max compression
+gzip compressed data, was "elsholdings-2.0.2.tar", last modified: Wed May 15 22:32:43 2024, max compression
```

## Comparing `elsholdings-2.0.1.tar` & `elsholdings-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:08.278759 elsholdings-2.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:08.242738 elsholdings-2.0.1/ELSholdings/
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:08.273707 elsholdings-2.0.1/ELSholdings/kenwoo/
--rw-rw-rw-   0        0        0    45836 2024-05-15 22:17:00.000000 elsholdings-2.0.1/ELSholdings/kenwoo/xls2ppt.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:08.275712 elsholdings-2.0.1/ELSholdings.egg-info/
--rw-rw-rw-   0        0        0      425 2024-05-15 22:22:08.000000 elsholdings-2.0.1/ELSholdings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-15 22:22:08.000000 elsholdings-2.0.1/ELSholdings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:22:08.000000 elsholdings-2.0.1/ELSholdings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-15 22:22:08.000000 elsholdings-2.0.1/ELSholdings.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      425 2024-05-15 22:22:08.276754 elsholdings-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.0.1/README.md
--rw-rw-rw-   0        0        0      366 2024-05-15 22:20:56.000000 elsholdings-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 22:22:08.278759 elsholdings-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 22:32:43.039997 elsholdings-2.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-15 22:32:43.009420 elsholdings-2.0.2/ELSholdings/
+drwxrwxrwx   0        0        0        0 2024-05-15 22:32:43.034990 elsholdings-2.0.2/ELSholdings/kenwoo/
+-rw-rw-rw-   0        0        0    45835 2024-05-15 22:32:07.000000 elsholdings-2.0.2/ELSholdings/kenwoo/xls2ppt.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:32:43.036996 elsholdings-2.0.2/ELSholdings.egg-info/
+-rw-rw-rw-   0        0        0      425 2024-05-15 22:32:42.000000 elsholdings-2.0.2/ELSholdings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-05-15 22:32:42.000000 elsholdings-2.0.2/ELSholdings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:32:42.000000 elsholdings-2.0.2/ELSholdings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-15 22:32:42.000000 elsholdings-2.0.2/ELSholdings.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      425 2024-05-15 22:32:43.038000 elsholdings-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.0.2/README.md
+-rw-rw-rw-   0        0        0      366 2024-05-15 22:32:32.000000 elsholdings-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:32:43.039997 elsholdings-2.0.2/setup.cfg
```

### Comparing `elsholdings-2.0.1/ELSholdings/kenwoo/xls2ppt.py` & `elsholdings-2.0.2/ELSholdings/kenwoo/xls2ppt.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,15 +541,15 @@
 
     # 마지막 워크시트를 세 번째 위치로 이동시킵니다.
     workbook.move_sheet(last_sheet, offset=-11)
 
     # 변경 사항을 저장합니다.
     workbook.save(file_out_ppt)
 
-    return df_Daily_NAV,df_Daily_NAV_Market_Cap
+    return None
 
 ############################################################################
 ############################################################################
 ############################################################################
 
 def remove_consecutive_zeros(df):
     # 첫 번째 행이 모두 0인 경우 삭제
@@ -593,14 +593,16 @@
     df_alives.at[code,'절대수익율']=Ret
     df_alives.at[code,'연환산수익율']=Ret_pa
 
   return df_alives
 
 
 def stats_for_redeemed(df_Daily_NAV,input_date):
+    import pandas as pd
+    
     # date가 인덱스에 있는지 확인
     if input_date not in df_Daily_NAV.index: # 인덱스에 없는 날짜라면
         input_date=df_Daily_NAV.index[df_Daily_NAV.index < input_date].max() # 가장 가까운 앞 날짜 추출
     else: # 인덱스에 있다면 그냥 날짜객체로 반환
         input_date=pd.Timestamp(input_date)
 
     # 특정일을 나타내는 행에서 그 값이 0인 것들중 칼럼 이름이 KR로 시작하는 것들을 Series로 추출함
```

