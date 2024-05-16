# Comparing `tmp/brian_lib-0.2.3.tar.gz` & `tmp/brian_lib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brian_lib-0.2.3.tar", last modified: Mon Mar  4 02:52:01 2024, max compression
+gzip compressed data, was "brian_lib-0.2.4.tar", last modified: Mon Mar  4 02:56:53 2024, max compression
```

## Comparing `brian_lib-0.2.3.tar` & `brian_lib-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:52:01.883848 brian_lib-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-03-04 02:52:01.883848 brian_lib-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      584 2024-03-04 02:51:49.000000 brian_lib-0.2.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:52:01.875848 brian_lib-0.2.3/brian_lib/
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:52:01.875848 brian_lib-0.2.3/brian_lib/connectors/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/connectors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/connectors/ftp.py
--rw-rw-rw-   0 root         (0) root         (0)     9314 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/connectors/sharepoint.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:52:01.879848 brian_lib-0.2.3/brian_lib/context_managers/
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/context_managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/context_managers/switch.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:52:01.879848 brian_lib-0.2.3/brian_lib/decorators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/decorators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3102 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/decorators/general.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/decorators/logging_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/decorators/retry_decorator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:52:01.883848 brian_lib-0.2.3/brian_lib/utilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/data_transform.py
--rw-rw-rw-   0 root         (0) root         (0)    12828 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/date_time.py
--rw-rw-rw-   0 root         (0) root         (0)     4715 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/demography.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/downloader.py
--rw-rw-rw-   0 root         (0) root         (0)    10395 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/file_management.py
--rw-rw-rw-   0 root         (0) root         (0)     3625 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/rut.py
--rw-rw-rw-   0 root         (0) root         (0)     2062 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2024-03-04 02:51:49.000000 brian_lib-0.2.3/brian_lib/utilities/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:52:01.875848 brian_lib-0.2.3/brian_lib.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-03-04 02:52:01.000000 brian_lib-0.2.3/brian_lib.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      831 2024-03-04 02:52:01.000000 brian_lib-0.2.3/brian_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-04 02:52:01.000000 brian_lib-0.2.3/brian_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-04 02:52:01.000000 brian_lib-0.2.3/brian_lib.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       10 2024-03-04 02:52:01.000000 brian_lib-0.2.3/brian_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-04 02:52:01.883848 brian_lib-0.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-04 02:51:49.000000 brian_lib-0.2.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:56:53.917090 brian_lib-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-03-04 02:56:53.917090 brian_lib-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-03-04 02:56:40.000000 brian_lib-0.2.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:56:53.913089 brian_lib-0.2.4/brian_lib/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:56:53.913089 brian_lib-0.2.4/brian_lib/connectors/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/connectors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/connectors/ftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9314 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/connectors/sharepoint.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:56:53.913089 brian_lib-0.2.4/brian_lib/context_managers/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/context_managers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/context_managers/switch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:56:53.913089 brian_lib-0.2.4/brian_lib/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/decorators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3102 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/decorators/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/decorators/logging_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/decorators/retry_decorator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:56:53.917090 brian_lib-0.2.4/brian_lib/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/data_transform.py
+-rw-rw-rw-   0 root         (0) root         (0)    12896 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/date_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     4626 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/demography.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)    10395 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/file_management.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/rut.py
+-rw-rw-rw-   0 root         (0) root         (0)     2062 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2024-03-04 02:56:40.000000 brian_lib-0.2.4/brian_lib/utilities/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-04 02:56:53.913089 brian_lib-0.2.4/brian_lib.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-03-04 02:56:53.000000 brian_lib-0.2.4/brian_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      831 2024-03-04 02:56:53.000000 brian_lib-0.2.4/brian_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-04 02:56:53.000000 brian_lib-0.2.4/brian_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-04 02:56:53.000000 brian_lib-0.2.4/brian_lib.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       10 2024-03-04 02:56:53.000000 brian_lib-0.2.4/brian_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-04 02:56:53.917090 brian_lib-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-04 02:56:40.000000 brian_lib-0.2.4/setup.py
```

### Comparing `brian_lib-0.2.3/README.md` & `brian_lib-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/connectors/ftp.py` & `brian_lib-0.2.4/brian_lib/connectors/ftp.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/connectors/sharepoint.py` & `brian_lib-0.2.4/brian_lib/connectors/sharepoint.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/context_managers/switch.py` & `brian_lib-0.2.4/brian_lib/context_managers/switch.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/decorators/general.py` & `brian_lib-0.2.4/brian_lib/decorators/general.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/decorators/logging_decorator.py` & `brian_lib-0.2.4/brian_lib/decorators/logging_decorator.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/decorators/retry_decorator.py` & `brian_lib-0.2.4/brian_lib/decorators/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/utilities/data_transform.py` & `brian_lib-0.2.4/brian_lib/utilities/data_transform.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/utilities/date_time.py` & `brian_lib-0.2.4/brian_lib/utilities/date_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,14 +385,16 @@
 def is_business_day(date: datetime = None, country_code: str = None, city: str = None) -> bool:
     """Determina si una fecha es un día hábil.
     Args:
         date (datetime): Fecha a verificar.
     Returns:
         bool: True si es un día hábil, False si no.
     """
+    if country_code is None:
+        country_code = current_country
     if date is None:
         date = datetime.now()
     if date.weekday() > 4:
         print('Es fin de semana')
         return False
     if is_holiday(date=date, country_code=country_code, city=city):
         print('Es festivo')
```

### Comparing `brian_lib-0.2.3/brian_lib/utilities/demography.py` & `brian_lib-0.2.4/brian_lib/utilities/demography.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,14 @@
                     print(f"Se aplica solo a las siguientes regiones: {', '.join(holiday['counties'])}")
                     if city is not None:
                         print(f"La ciudad actual es {city}.")
                         print('--------------------------------------------------------------')
                         return city in holiday['counties']
                     else:
                         return True
-                print(f"{date} is a holiday in {country_code} ({holiday['localName']})")
                 return True
     
     return False
 
 def get_next_holiday(country_code: str = current_country) -> dict:
     """Obtiene la próxima fecha festiva en un país específico.
     Args:
```

### Comparing `brian_lib-0.2.3/brian_lib/utilities/downloader.py` & `brian_lib-0.2.4/brian_lib/utilities/downloader.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/utilities/file_management.py` & `brian_lib-0.2.4/brian_lib/utilities/file_management.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/utilities/rut.py` & `brian_lib-0.2.4/brian_lib/utilities/rut.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/utilities/serialization.py` & `brian_lib-0.2.4/brian_lib/utilities/serialization.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib/utilities/validation.py` & `brian_lib-0.2.4/brian_lib/utilities/validation.py`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/brian_lib.egg-info/SOURCES.txt` & `brian_lib-0.2.4/brian_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brian_lib-0.2.3/setup.py` & `brian_lib-0.2.4/setup.py`

 * *Files identical despite different names*

