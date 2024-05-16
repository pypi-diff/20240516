# Comparing `tmp/ecuapassdocs-0.78.tar.gz` & `tmp/ecuapassdocs-0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecuapassdocs-0.78.tar", last modified: Wed May 15 05:02:34 2024, max compression
+gzip compressed data, was "ecuapassdocs-0.79.tar", last modified: Thu May 16 12:56:41 2024, max compression
```

## Comparing `ecuapassdocs-0.78.tar` & `ecuapassdocs-0.79.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.922690 ecuapassdocs-0.78/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-15 05:02:34.922690 ecuapassdocs-0.78/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)       40 2024-04-22 18:48:50.000000 ecuapassdocs-0.78/README.md
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.890690 ecuapassdocs-0.78/ecuapassdocs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.898690 ecuapassdocs-0.78/ecuapassdocs/info/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.78/ecuapassdocs/info/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3415 2024-05-10 22:36:24.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_data.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18226 2024-05-15 04:30:48.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_extractor.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4490 2024-04-29 15:28:31.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_feedback.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9457 2024-05-14 17:41:34.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    19585 2024-05-14 16:48:19.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1521 2024-05-12 16:16:09.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_declaracion.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    24020 2024-05-13 19:40:43.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2187 2024-05-10 22:50:32.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2065 2024-05-13 22:36:59.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    11223 2024-05-12 11:42:43.000000 ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.78/ecuapassdocs/info/resourceloader.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.898690 ecuapassdocs-0.78/ecuapassdocs/resources/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.906690 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      623 2024-05-14 16:35:53.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/documentos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/empresa.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/monedas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/out.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/sustancias.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.906690 ecuapassdocs-0.78/ecuapassdocs/resources/data_declaracion/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_declaracion/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.910690 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/sectores.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.918690 ecuapassdocs-0.78/ecuapassdocs/resources/docs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    15815 2024-05-11 02:21:09.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/declaracion_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/join.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-12 00:44:17.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.78/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.922690 ecuapassdocs-0.78/ecuapassdocs/resources/images/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/icon-colombia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/icon-ecuador.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/icon-white-bot.ico
--rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-cartaporte-vacia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-scroll-up.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.78/ecuapassdocs/resources/images/image-windows-WindowButtons.png
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-15 05:02:34.894690 ecuapassdocs-0.78/ecuapassdocs.egg-info/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-15 05:02:34.000000 ecuapassdocs-0.78/ecuapassdocs.egg-info/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)     5999 2024-05-15 05:02:34.000000 ecuapassdocs-0.78/ecuapassdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-15 05:02:34.000000 ecuapassdocs-0.78/ecuapassdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-15 05:02:34.000000 ecuapassdocs-0.78/ecuapassdocs.egg-info/requires.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-15 05:02:34.000000 ecuapassdocs-0.78/ecuapassdocs.egg-info/top_level.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-15 05:02:34.922690 ecuapassdocs-0.78/setup.cfg
--rw-rw-r--   0 lg        (1000) lg        (1000)     1593 2024-05-15 05:02:21.000000 ecuapassdocs-0.78/setup.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.647493 ecuapassdocs-0.79/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-16 12:56:41.647493 ecuapassdocs-0.79/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)       40 2024-04-22 18:48:50.000000 ecuapassdocs-0.79/README.md
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.543491 ecuapassdocs-0.79/ecuapassdocs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.547491 ecuapassdocs-0.79/ecuapassdocs/info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3416 2024-05-16 12:39:30.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_data.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18226 2024-05-15 04:30:48.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_extractor.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4490 2024-04-29 15:28:31.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_feedback.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9457 2024-05-14 17:41:34.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    19585 2024-05-14 16:48:19.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1521 2024-05-12 16:16:09.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_declaracion.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    24020 2024-05-13 19:40:43.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2187 2024-05-10 22:50:32.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2065 2024-05-13 22:36:59.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    11223 2024-05-12 11:42:43.000000 ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.79/ecuapassdocs/info/resourceloader.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.547491 ecuapassdocs-0.79/ecuapassdocs/resources/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.567492 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      623 2024-05-14 16:35:53.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/documentos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/empresa.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/monedas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/out.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/sustancias.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.567492 ecuapassdocs-0.79/ecuapassdocs/resources/data_declaracion/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_declaracion/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.595492 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/sectores.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.627493 ecuapassdocs-0.79/ecuapassdocs/resources/docs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    15815 2024-05-16 12:18:23.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte_input_parameters-CBIN_IDS.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)    15818 2024-05-16 12:20:48.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/join.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-16 12:23:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto_input_parameters-CBIN_IDS.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-12 00:44:17.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.79/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.647493 ecuapassdocs-0.79/ecuapassdocs/resources/images/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-colombia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-ecuador.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-white-bot.ico
+-rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-cartaporte-vacia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-scroll-up.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.79/ecuapassdocs/resources/images/image-windows-WindowButtons.png
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-16 12:56:41.543491 ecuapassdocs-0.79/ecuapassdocs.egg-info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6139 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/requires.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-16 12:56:41.000000 ecuapassdocs-0.79/ecuapassdocs.egg-info/top_level.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-16 12:56:41.647493 ecuapassdocs-0.79/setup.cfg
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1661 2024-05-16 12:56:39.000000 ecuapassdocs-0.79/setup.py
```

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_data.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 			"idTipo" : "NIT", 
 			"idNumero" : "890.901.321-5",
 			"modelCartaportes": "Model_Cartaportes_Botero",
 			"modelManifiestos": "Model_Manifiestos_Botero",
 			"modelDeclaraciones": None,
 			"MRN": None,
 			"MSN": None,
-			"permisos" : {"originario":"C.I.-E.C.-0060-04",
-				          "servicios1":"P.P.S.CO015905", "servicios2":"P.P.S.PE000210"}
 		},
 		"NTA" : { 
 			'id'     : "NTA",
 			"nombre" : "NUEVO TRANSPORTE DE AMERICA COMPAÑIA LIMITADA", 
 			"direccion": "ARGENTINA Y JUAN LEON MERA - TULCAN",
 			"idTipo" : "RUC", 
 			"idNumero" : "1791834461001",
 			"modelCartaportes": "Model_Cartaportes_NTA_BYZA",
 			"modelManifiestos": "Manifiestos_NTA_BYZA_Template",
 			"modelDeclaraciones": "Model_Declaraciones_NTA_Single",
 			"MRN": "CEC202340350941",
-			"MSN": "0001"
+			"MSN": "0001",
+			"permisos" : {"originario":"C.I.-E.C.-0060-04",
+				          "servicios1":"P.P.S.CO015905", "servicios2":"P.P.S.PE000210"}
 		},
 		"SILOGISTICA": {
 			'id'     : "SILOGISTICA",
 			"nombre": "PROVIZCAINO S.A.",
 			"direccion": "ANTIZ Y 9 DE AGOSTO, CALDERÓN - QUITO",
 			"idTipo": "RUC",
 			"idNumero": "1791882253001",
```

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_extractor.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_extractor.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_feedback.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_feedback.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_declaracion.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_declaracion.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/ecuapass_utils.py` & `ecuapassdocs-0.79/ecuapassdocs/info/ecuapass_utils.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/info/resourceloader.py` & `ecuapassdocs-0.79/ecuapassdocs/info/resourceloader.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/out.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/out.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/paises_todos.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/paises_todos.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/sustancias.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/sustancias.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/cartaporte_input_parameters.json` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/cartaporte_input_parameters-CBIN_IDS.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/declaracion_input_parameters.json` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/declaracion_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/join.pdf` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/join.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/manifiesto_input_parameters.json` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/manifiesto_input_parameters-CBIN_IDS.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.79/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/icon-colombia.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-colombia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/icon-ecuador.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-ecuador.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/icon-white-bot.ico` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/icon-white-bot.ico`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-cartaporte-vacia.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-cartaporte-vacia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-declaracion-ecuapass.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-declaracion-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png` & `ecuapassdocs-0.79/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.78/ecuapassdocs.egg-info/SOURCES.txt` & `ecuapassdocs-0.79/ecuapassdocs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -77,25 +77,27 @@
 ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
 ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
 ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
 ecuapassdocs/resources/docs/__init__.py
 ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
 ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
 ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
+ecuapassdocs/resources/docs/cartaporte_input_parameters-CBIN_IDS.json
 ecuapassdocs/resources/docs/cartaporte_input_parameters.json
 ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
 ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
 ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
 ecuapassdocs/resources/docs/declaracion_input_parameters.json
 ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
 ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
 ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
 ecuapassdocs/resources/docs/join.pdf
 ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
 ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
+ecuapassdocs/resources/docs/manifiesto_input_parameters-CBIN_IDS.json
 ecuapassdocs/resources/docs/manifiesto_input_parameters.json
 ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
 ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
 ecuapassdocs/resources/images/__init__.py
 ecuapassdocs/resources/images/icon-colombia.png
 ecuapassdocs/resources/images/icon-ecuador.png
 ecuapassdocs/resources/images/icon-white-bot.ico
```

### Comparing `ecuapassdocs-0.78/setup.py` & `ecuapassdocs-0.79/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ecuapassdocs',  # Package name
-    version='0.78',  # Package version
+    version='0.79',  # Package version
     url="https://github.com/lgarreta/ecuapassdocs",
     author='Luis Garreta',
     author_email='lgarreta@gmail.com',
     description='Utils for creating PDFs, loading resources and extracting info from fields in ECUAPASS docs: cartaportes, manifiestos, declaraciones',
     packages=find_packages(),  # Automatically finds packages within the directory
 	include_package_data=True, 
 	package_data={"ecuapassdocs": ["resources/images/*", 
@@ -17,14 +17,15 @@
 	# List any dependencies here
     install_requires = [
 		"PyPDF2==3.0.1",
 		"reportlab==4.0.8",
 		"Pillow==10.1.0"
 	], 
 	logs = {
+		"0.79"   : "Search codebin form by NAME. Added settings for NTA",
 		"0.78"   : "Improved infos:depositos, dates, vehiculo",
 		"0.77"   : "Improved update (posprocessing) ECUAPASS file",
 		"0.76"   : "Improved Utils, getCodebinValues",
 		"0.75"   : "Simplified info classes (e.g. removed Gastos table)",
 		"0.74"   : "Changed tipoProc (Byza === NTA)",
 		"0.73"   : "Improved Byza's clean watermarks",
 		"0.72"   : "Improved infos: embalaje",
```

