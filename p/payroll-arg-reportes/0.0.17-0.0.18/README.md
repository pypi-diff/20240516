# Comparing `tmp/payroll_arg_reportes-0.0.17.tar.gz` & `tmp/payroll_arg_reportes-0.0.18.tar.gz`

## Comparing `payroll_arg_reportes-0.0.17.tar` & `payroll_arg_reportes-0.0.18.tar`

### file list

```diff
@@ -1,24 +1,36 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/.github/workflows/tests.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/base_reports/__init__.py
--rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/base_reports/recibo_base_1.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/reporters/__init__.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/reporters/descarga_excel.py
--rw-r--r--   0        0        0    34369 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/reporters/recibo_sueldo.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/tables/base_tables.py
--rw-r--r--   0        0        0   154914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/test_cases/liquidacion_completa.json
--rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/test_cases/liquidacion_corta.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/test_cases/test_recibo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/tools/__init__.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/py_arg_reports/tools/recibos_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/tests/__init__.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/tests/test_download_recibo.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/tests/temp/.gitignore
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/LICENSE
--rw-r--r--   0        0        0    12053 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/README.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/pyproject.toml
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/docs/libro-de-sueldos.md
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/docs/recibo-de-sueldos.md
+-rw-r--r--   0        0        0   285657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/docs/images/libro-sueldo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/config.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/logs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/base_reports/__init__.py
+-rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/base_reports/recibo_base_1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/reporters/__init__.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/reporters/descarga_excel.py
+-rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/reporters/recibo_sueldo.py
+-rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/reporters/libro_sueldo/__init__.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/reporters/libro_sueldo/data.py
+-rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/reporters/samples/samples-recibo-info.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/tables/base_tables.py
+-rw-r--r--   0        0        0   154914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/test_cases/liquidacion_completa.json
+-rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/test_cases/liquidacion_corta.json
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/test_cases/test_libro_sueldo.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/test_cases/test_recibo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/tools/__init__.py
+-rw-r--r--   0        0        0    14126 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/tools/base.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/py_arg_reports/tools/recibos_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/tests/__init__.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/tests/test_download_recibo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/tests/libro_sueldo/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/tests/libro_sueldo/test_base_pdf.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/tests/temp/.gitignore
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/README.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/pyproject.toml
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.18/PKG-INFO
```

### Comparing `payroll_arg_reportes-0.0.17/.github/workflows/python-publish.yml` & `payroll_arg_reportes-0.0.18/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.17/.github/workflows/tests.yml` & `payroll_arg_reportes-0.0.18/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -34,9 +34,9 @@
         --show-source \
         --max-complexity=14 \
         --max-line-length=130 \
         --statistics
 
     - name: Run Tests
       run: |
-        export PYTHONPATH=$PYTHONPATH:$(pwd)/py_arg_reports
-        python -m unittest
+        # export PYTHONPATH=$PYTHONPATH:$(pwd)/py_arg_reports
+        python -m unittest -v
```

### Comparing `payroll_arg_reportes-0.0.17/py_arg_reports/base_reports/recibo_base_1.py` & `payroll_arg_reportes-0.0.18/py_arg_reports/base_reports/recibo_base_1.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.17/py_arg_reports/reporters/descarga_excel.py` & `payroll_arg_reportes-0.0.18/py_arg_reports/reporters/descarga_excel.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.17/py_arg_reports/reporters/recibo_sueldo.py` & `payroll_arg_reportes-0.0.18/py_arg_reports/reporters/recibo_sueldo.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,206 +21,15 @@
 FONT_SIZE_MAIN = config_constants['FONT_SIZE_MAIN']
 FONT_SIZE_BODY = config_constants['FONT_SIZE_BODY']
 
 
 def get_recibo_info(json_data: dict) -> dict:
     """ Obtiene la información del recibo de sueldo en formato JSON
         Con datos de la empresa, empleado, liquidación, etc.
-        con este formato:
-
-[
-    {
-        "empresa": {
-            "pk": 1,
-            "name": "Empresa de Prueba",
-            "cuit": "20333333333",
-            "domicilio": {
-                "pk": 1,
-                "calle": "Calle de Prueba",
-                "numero": "123",
-                "piso": null,
-                "oficina": null,
-                "barrio": null,
-                "localidad": {
-                    "pk": 1252,
-                    "provincia": {
-                        "pk": 10,
-                        "name": "Formosa",
-                        "pais": {
-                            "pk": 11,
-                            "code": "AR",
-                            "name": "Argentina"
-                        }
-                    },
-                    "name": "10",
-                    "text": "10 (Formosa)"
-                },
-                "cod_postal": null
-            },
-            "ultimo_pago_seguridad_social": {
-                "id": 31,
-                "banco": "Banco De La Ciudad De Buenos Aires",
-                "mes": 12,
-                "anio": 2023,
-                "fecha_pago": "2024-01-09",
-                "empresa": 1
-            }
-        },
-        "liquidacion": {
-            "nro_liq": 0,
-            "tipo_liquidacion": "Mensual",
-            "periodo": {
-                "periodo": "2023-12"
-            },
-            "fecha_pago": "2024-01-04"
-        },
-        "empleado": {
-            "legajo": 6410,
-            "first_name": "Adriana Anahí",
-            "last_name": "Poblete",
-            "cuil": "20188712648",
-            "fecha_ingreso": "1990-10-01",
-            "fecha_ingreso_2": null,
-            "categoria": "Vendedor C",
-            "contrato": "A tiempo parcial: Indeterminado /permanente",
-            "obra_social": "O.S.DE LOS EMPLEADOS DE COMERCIO Y ACTIVIDADES CIVILES",
-            "area": "Area 1",
-            "posicion": "Posicion 1",
-            "basico": 112520.15,
-            "lugar_trabajo": "Mendiolaza",
-            "relacion_bancaria": {
-                "forma_pago": "EFVO",
-                "numero_cuenta": null,
-                "cbu": null
-            }
-        },
-        "conceptos_liquidados": [
-            {
-                "concepto": {
-                    "code": "SUELDO",
-                    "tipo_concepto": 1,
-                    "name": "Sueldo Básico"
-                },
-                "orden": 12,
-                "cantidad": 30.0,
-                "importe": 112520.15
-            },
-            {
-                "concepto": {
-                    "code": "ANTIGU",
-                    "tipo_concepto": 1,
-                    "name": "Antiguedad"
-                },
-                "orden": 49,
-                "cantidad": 33.0,
-                "importe": 37131.6495
-            }
-        ],
-        "totales_liquidacion": {
-            "total_remunerativo": 162122.78279166666,
-            "total_no_remunerativo": 36477.626128125004,
-            "total_retenciones": 32625.883297578122,
-            "neto_liquidacion": 165974.52562221355
-        }
-    },
-    {
-        "empresa": {
-            "pk": 1,
-            "name": "Empresa de Prueba",
-            "cuit": "20333333333",
-            "domicilio": {
-                "pk": 1,
-                "calle": "Calle de Prueba",
-                "numero": "123",
-                "piso": null,
-                "oficina": null,
-                "barrio": null,
-                "localidad": {
-                    "pk": 1252,
-                    "provincia": {
-                        "pk": 10,
-                        "name": "Formosa",
-                        "pais": {
-                            "pk": 11,
-                            "code": "AR",
-                            "name": "Argentina"
-                        }
-                    },
-                    "name": "10",
-                    "text": "10 (Formosa)"
-                },
-                "cod_postal": null
-            },
-            "ultimo_pago_seguridad_social": {
-                "id": 31,
-                "banco": "Banco De La Ciudad De Buenos Aires",
-                "mes": 12,
-                "anio": 2023,
-                "fecha_pago": "2024-01-09",
-                "empresa": 1
-            }
-        },
-        "liquidacion": {
-            "nro_liq": 0,
-            "tipo_liquidacion": "Mensual",
-            "periodo": {
-                "periodo": "2023-12"
-            },
-            "fecha_pago": "2024-01-04"
-        },
-        "empleado": {
-            "legajo": 7720,
-            "first_name": "Eduardo Viviana",
-            "last_name": "Monteverde",
-            "cuil": "20674648438",
-            "fecha_ingreso": "1990-10-01",
-            "fecha_ingreso_2": null,
-            "categoria": "Cajero C",
-            "contrato": "A tiempo parcial: Indeterminado /permanente",
-            "obra_social": "O.S.DE LOS EMPLEADOS DE COMERCIO Y ACTIVIDADES CIVILES",
-            "area": "Area 1",
-            "posicion": "Posicion 1",
-            "basico": 110645.24,
-            "lugar_trabajo": "25 de Mayo",
-            "relacion_bancaria": {
-                "forma_pago": "EFVO",
-                "numero_cuenta": null,
-                "cbu": null
-            }
-        },
-        "conceptos_liquidados": [
-            {
-                "concepto": {
-                    "code": "SUELDO",
-                    "tipo_concepto": 1,
-                    "name": "Sueldo Básico"
-                },
-                "orden": 12,
-                "cantidad": 30.0,
-                "importe": 110645.24
-            },
-            {
-                "concepto": {
-                    "code": "ANTIGU",
-                    "tipo_concepto": 1,
-                    "name": "Antiguedad"
-                },
-                "orden": 49,
-                "cantidad": 33.0,
-                "importe": 36512.929200000006
-            }
-        ],
-        "totales_liquidacion": {
-            "total_remunerativo": 159421.34996666666,
-            "total_no_remunerativo": 35869.8037425,
-            "total_retenciones": 32083.9083370625,
-            "neto_liquidacion": 163207.24537210417
-        }
-    }
-]
+        con el formato en el ejemplo reporters/samples/samples-recibo-info.json
     """
     # Si el json está vacío, no se puede descargar
     if not json_data:
         return {
             "error": "No se puede descargar el recibo, no hay datos"
         }
```

### Comparing `payroll_arg_reportes-0.0.17/py_arg_reports/test_cases/liquidacion_completa.json` & `payroll_arg_reportes-0.0.18/py_arg_reports/test_cases/liquidacion_completa.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.17/py_arg_reports/test_cases/liquidacion_corta.json` & `payroll_arg_reportes-0.0.18/py_arg_reports/test_cases/liquidacion_corta.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.17/py_arg_reports/tools/recibos_utils.py` & `payroll_arg_reportes-0.0.18/py_arg_reports/tools/recibos_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         I also add thousands separators and two decimal places
         decimal is separated by comma and thousands by dot
     """
     resp = "{:,.2f}".format(float_value)
     resp = resp.replace(",", "X").replace(".", ",").replace("X", ".")
     currency = "$ " if include_currency else ""
 
-    return f'{currency} {resp}'
+    return f'{currency}{resp}'
 
 
 def draw_text_with_max_width(canvas, text, max_width, x, y):
     formatted_text = textObject(canvas, text, max_width, x, y)
 
     canvas.drawText(formatted_text)
```

### Comparing `payroll_arg_reportes-0.0.17/tests/test_download_recibo.py` & `payroll_arg_reportes-0.0.18/tests/test_download_recibo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import tempfile
 import unittest
 
 from PyPDF2 import PdfReader
 
-from reporters.recibo_sueldo import descargar_recibo
+from py_arg_reports.reporters.recibo_sueldo import descargar_recibo
 
 
 class TestDownloadRecibo(unittest.TestCase):
     """ Testing para Descargar Recibos
     """
     @classmethod
     def setUpClass(cls):
```

### Comparing `payroll_arg_reportes-0.0.17/LICENSE` & `payroll_arg_reportes-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.17/pyproject.toml` & `payroll_arg_reportes-0.0.18/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "payroll_arg_reportes"
-version = "0.0.17"
+version = "0.0.18"
 dependencies = [
-  "numero-a-letras==0.0.4",
+  "numero-a-letras>=0.0.4",
   "reportlab==4.0.8",
   "XlsxWriter==3.2.0",
 ]
 requires-python = ">=3.10"
 authors = [
   { name="Eugenio", email="coding_with@eugeniovazquez.com.ar" },
 ]
```

