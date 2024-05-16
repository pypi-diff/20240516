# Comparing `tmp/DevoteamLib-0.1.8.tar.gz` & `tmp/DevoteamLib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DevoteamLib-0.1.8.tar", last modified: Fri Feb  9 09:48:32 2024, max compression
+gzip compressed data, was "DevoteamLib-0.1.9.tar", last modified: Mon Feb 12 06:58:34 2024, max compression
```

## Comparing `DevoteamLib-0.1.8.tar` & `DevoteamLib-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-09 09:48:32.990492 DevoteamLib-0.1.8/
--rw-r--r--   0 pijarcandra   (501) staff       (20)        0 2023-12-27 07:02:24.000000 DevoteamLib-0.1.8/LICENSE
--rw-r--r--   0 pijarcandra   (501) staff       (20)      372 2024-02-09 09:48:32.990306 DevoteamLib-0.1.8/PKG-INFO
--rw-r--r--   0 pijarcandra   (501) staff       (20)        0 2023-12-27 07:26:58.000000 DevoteamLib-0.1.8/README.md
--rw-r--r--   0 pijarcandra   (501) staff       (20)      888 2024-02-09 09:48:10.000000 DevoteamLib-0.1.8/pyproject.toml
--rw-r--r--   0 pijarcandra   (501) staff       (20)       38 2024-02-09 09:48:32.990528 DevoteamLib-0.1.8/setup.cfg
-drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-09 09:48:32.984156 DevoteamLib-0.1.8/src/
-drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-09 09:48:32.985595 DevoteamLib-0.1.8/src/DevoteamLib/
-drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-09 09:48:32.986645 DevoteamLib-0.1.8/src/DevoteamLib/AuthentificationFile/
--rw-r--r--   0 pijarcandra   (501) staff       (20)        0 2024-01-15 19:21:23.000000 DevoteamLib-0.1.8/src/DevoteamLib/AuthentificationFile/__init__.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)      171 2024-01-29 05:03:14.000000 DevoteamLib-0.1.8/src/DevoteamLib/AuthentificationFile/devoteam.yml
--rw-r--r--   0 pijarcandra   (501) staff       (20)      155 2024-01-15 10:53:57.000000 DevoteamLib-0.1.8/src/DevoteamLib/AuthentificationFile/pupuk_indonesia.yml
--rw-r--r--   0 pijarcandra   (501) staff       (20)    11549 2024-01-30 07:35:53.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementEkstraction.py
-drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-09 09:48:32.989936 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/
--rw-r--r--   0 pijarcandra   (501) staff       (20)     2066 2024-01-29 04:41:00.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Allo.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     1702 2024-01-29 04:40:50.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Artha_Graha.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     4023 2024-01-29 04:40:33.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/BCA.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     3153 2024-01-29 04:40:05.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/BNI.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     1728 2024-02-05 05:03:45.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/BRI.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     2052 2024-01-29 04:39:40.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/BTPN.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     3603 2024-01-30 21:48:53.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/CIMB.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     1591 2024-01-29 04:38:49.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Danamon.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     1914 2024-01-29 04:38:36.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/HANA.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     1846 2024-01-29 04:38:03.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/MEGA.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     3735 2024-02-05 05:14:17.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Mandiri.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     3511 2024-01-29 04:36:45.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/OCBC.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     2510 2024-01-29 04:37:48.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Permata.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)        0 2024-01-29 05:23:01.000000 DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/__init__.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     6102 2024-02-09 08:40:23.000000 DevoteamLib-0.1.8/src/DevoteamLib/GenAI.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)    10650 2024-02-09 09:48:02.000000 DevoteamLib-0.1.8/src/DevoteamLib/OCRLayouting.py
--rw-r--r--   0 pijarcandra   (501) staff       (20)     1737 2024-01-29 05:04:51.000000 DevoteamLib-0.1.8/src/DevoteamLib/__init__.py
-drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-09 09:48:32.990071 DevoteamLib-0.1.8/src/DevoteamLib.egg-info/
--rw-r--r--   0 pijarcandra   (501) staff       (20)      372 2024-02-09 09:48:32.000000 DevoteamLib-0.1.8/src/DevoteamLib.egg-info/PKG-INFO
--rw-r--r--   0 pijarcandra   (501) staff       (20)     1106 2024-02-09 09:48:32.000000 DevoteamLib-0.1.8/src/DevoteamLib.egg-info/SOURCES.txt
--rw-r--r--   0 pijarcandra   (501) staff       (20)        1 2024-02-09 09:48:32.000000 DevoteamLib-0.1.8/src/DevoteamLib.egg-info/dependency_links.txt
--rw-r--r--   0 pijarcandra   (501) staff       (20)       12 2024-02-09 09:48:32.000000 DevoteamLib-0.1.8/src/DevoteamLib.egg-info/top_level.txt
+drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-12 06:58:34.974460 DevoteamLib-0.1.9/
+-rw-r--r--   0 pijarcandra   (501) staff       (20)        0 2023-12-27 07:02:24.000000 DevoteamLib-0.1.9/LICENSE
+-rw-r--r--   0 pijarcandra   (501) staff       (20)      372 2024-02-12 06:58:34.974268 DevoteamLib-0.1.9/PKG-INFO
+-rw-r--r--   0 pijarcandra   (501) staff       (20)        0 2023-12-27 07:26:58.000000 DevoteamLib-0.1.9/README.md
+-rw-r--r--   0 pijarcandra   (501) staff       (20)      888 2024-02-12 06:58:10.000000 DevoteamLib-0.1.9/pyproject.toml
+-rw-r--r--   0 pijarcandra   (501) staff       (20)       38 2024-02-12 06:58:34.974514 DevoteamLib-0.1.9/setup.cfg
+drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-12 06:58:34.967458 DevoteamLib-0.1.9/src/
+drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-12 06:58:34.969193 DevoteamLib-0.1.9/src/DevoteamLib/
+drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-12 06:58:34.970585 DevoteamLib-0.1.9/src/DevoteamLib/AuthentificationFile/
+-rw-r--r--   0 pijarcandra   (501) staff       (20)        0 2024-01-15 19:21:23.000000 DevoteamLib-0.1.9/src/DevoteamLib/AuthentificationFile/__init__.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)      171 2024-01-29 05:03:14.000000 DevoteamLib-0.1.9/src/DevoteamLib/AuthentificationFile/devoteam.yml
+-rw-r--r--   0 pijarcandra   (501) staff       (20)      155 2024-01-15 10:53:57.000000 DevoteamLib-0.1.9/src/DevoteamLib/AuthentificationFile/pupuk_indonesia.yml
+-rw-r--r--   0 pijarcandra   (501) staff       (20)    18284 2024-02-12 06:40:25.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementEkstraction.py
+drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-12 06:58:34.973928 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     2066 2024-01-29 04:41:00.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Allo.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     1702 2024-01-29 04:40:50.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Artha_Graha.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     4023 2024-01-29 04:40:33.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/BCA.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     3153 2024-01-29 04:40:05.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/BNI.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     1728 2024-02-05 05:03:45.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/BRI.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     2052 2024-01-29 04:39:40.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/BTPN.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     3603 2024-01-30 21:48:53.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/CIMB.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     1591 2024-01-29 04:38:49.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Danamon.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     1914 2024-01-29 04:38:36.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/HANA.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     1846 2024-01-29 04:38:03.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/MEGA.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     3687 2024-02-12 01:03:59.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Mandiri.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     3511 2024-01-29 04:36:45.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/OCBC.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     2510 2024-01-29 04:37:48.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Permata.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)        0 2024-01-29 05:23:01.000000 DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/__init__.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     6102 2024-02-09 08:40:23.000000 DevoteamLib-0.1.9/src/DevoteamLib/GenAI.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)    11386 2024-02-12 03:07:40.000000 DevoteamLib-0.1.9/src/DevoteamLib/OCRLayouting.py
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     1737 2024-01-29 05:04:51.000000 DevoteamLib-0.1.9/src/DevoteamLib/__init__.py
+drwxr-xr-x   0 pijarcandra   (501) staff       (20)        0 2024-02-12 06:58:34.974055 DevoteamLib-0.1.9/src/DevoteamLib.egg-info/
+-rw-r--r--   0 pijarcandra   (501) staff       (20)      372 2024-02-12 06:58:34.000000 DevoteamLib-0.1.9/src/DevoteamLib.egg-info/PKG-INFO
+-rw-r--r--   0 pijarcandra   (501) staff       (20)     1106 2024-02-12 06:58:34.000000 DevoteamLib-0.1.9/src/DevoteamLib.egg-info/SOURCES.txt
+-rw-r--r--   0 pijarcandra   (501) staff       (20)        1 2024-02-12 06:58:34.000000 DevoteamLib-0.1.9/src/DevoteamLib.egg-info/dependency_links.txt
+-rw-r--r--   0 pijarcandra   (501) staff       (20)       12 2024-02-12 06:58:34.000000 DevoteamLib-0.1.9/src/DevoteamLib.egg-info/top_level.txt
```

### Comparing `DevoteamLib-0.1.8/pyproject.toml` & `DevoteamLib-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "importlib",
     "pdf2image==1.16.3"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DevoteamLib"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Pijar Candra", email="pijarcandra22@gmail.com"},
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Allo.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Allo.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Artha_Graha.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Artha_Graha.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/BCA.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/BCA.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/BNI.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/BNI.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/BRI.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/BRI.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/BTPN.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/BTPN.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/CIMB.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/CIMB.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Danamon.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Danamon.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/HANA.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/HANA.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/MEGA.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/MEGA.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Mandiri.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Mandiri.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,10 +104,9 @@
             })
 
       #   except Exception as ex:
       #     print(ex)
       #     print(er)
 
     df = pd.DataFrame(dictList)
-    df['AMMOUNT'] = df['AMMOUNT'].astype(float)
 
     return df
```

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/OCBC.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/OCBC.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/BankStatementParser/Permata.py` & `DevoteamLib-0.1.9/src/DevoteamLib/BankStatementParser/Permata.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/GenAI.py` & `DevoteamLib-0.1.9/src/DevoteamLib/GenAI.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/OCRLayouting.py` & `DevoteamLib-0.1.9/src/DevoteamLib/OCRLayouting.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,38 @@
       newdata[1] = pd.concat(newdata[:2])
     except:
       newdata.append(df.iloc[:end_i])
       newdata[1] = pd.concat(newdata[:2])
     return newdata[1:]
   else:
     return "You not allowed to used this function"
+  
+def funcPositionBS(df,pos):
+  start_i = 0
+  end_i   = 1
+
+  datacur = 0
+  newdata = []
+
+  for i in range(1,len(df)):
+      data_before  = [x for x in range(min(df.iloc[[i-1]][pos].values[0]),max(df.iloc[[i-1]][pos].values[0])+1)]
+      data_current = [x for x in range(min(df.iloc[[i]][pos].values[0]),max(df.iloc[[i]][pos].values[0])+1)]
+
+      if jaccard_similarity(data_before,data_current)<0.35:
+          newdata.append(df.iloc[start_i:end_i])
+          start_i = end_i
+          end_i   = i
+      if end_i != start_i:
+          try:
+              newdata[-1] = df.iloc[start_i:end_i]
+          except:
+              newdata.append(df.iloc[start_i:end_i])
+
+  newdata.append(df.iloc[end_i:])
+  newdata[1] = pd.concat(newdata[:2])
 
 ## Creating Black Box for Spliting Text in Image
 def blockingImage(im_bw,size):
   if DevoteamLib.OCRLayoutingStatus('blockingImage'):
     length,width = im_bw.shape
 
     for w in range(0,width-size,size):
```

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib/__init__.py` & `DevoteamLib-0.1.9/src/DevoteamLib/__init__.py`

 * *Files identical despite different names*

### Comparing `DevoteamLib-0.1.8/src/DevoteamLib.egg-info/SOURCES.txt` & `DevoteamLib-0.1.9/src/DevoteamLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

