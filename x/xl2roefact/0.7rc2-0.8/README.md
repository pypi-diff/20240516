# Comparing `tmp/xl2roefact-0.7rc2.tar.gz` & `tmp/xl2roefact-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xl2roefact-0.7rc2.tar", last modified: Mon May  6 03:29:53 2024, max compression
+gzip compressed data, was "xl2roefact-0.8.tar", last modified: Thu May 16 02:32:07 2024, max compression
```

## Comparing `xl2roefact-0.7rc2.tar` & `xl2roefact-0.8.tar`

### file list

```diff
@@ -1,15 +1,26 @@
--rw-r--r--   0        0        0    35149 2024-05-06 03:29:27.462748 xl2roefact-0.7rc2/LICENSE
--rw-r--r--   0        0        0    18839 2024-05-06 03:29:27.462748 xl2roefact-0.7rc2/README.md
--rw-r--r--   0        0        0     3336 2024-05-06 03:29:53.094666 xl2roefact-0.7rc2/pyproject.toml
--rw-r--r--   0        0        0      176 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/src/commands/__init__.py
--rw-r--r--   0        0        0     1808 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/src/data/README_app_config_rules.md
--rw-r--r--   0        0        0      174 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/src/data/__init__.py
--rw-r--r--   0        0        0     7134 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/src/data/app_settings.yml
--rw-r--r--   0        0        0        1 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/.gitkeep
--rw-r--r--   0        0        0    21711 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.json
--rw-r--r--   0        0        0   268862 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.xlsx
--rw-r--r--   0        0        0    15740 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.xml
--rw-r--r--   0        0        0      986 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/_test_results.txt
--rw-r--r--   0        0        0    24173 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/fact_RENF1004.json
--rw-r--r--   0        0        0    16332 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/fact_RENF1004.xlsx
--rw-r--r--   0        0        0    61437 1970-01-01 00:00:00.000000 xl2roefact-0.7rc2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-16 02:31:44.926588 xl2roefact-0.8/LICENSE
+-rw-r--r--   0        0        0    18403 2024-05-16 02:31:44.926588 xl2roefact-0.8/README.md
+-rw-r--r--   0        0        0     3362 2024-05-16 02:32:07.534645 xl2roefact-0.8/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-05-16 02:31:45.066588 xl2roefact-0.8/tests/.gitkeep
+-rw-r--r--   0        0        0    21711 2024-05-16 02:31:45.066588 xl2roefact-0.8/tests/Fact_Petrom_11017969.json
+-rw-r--r--   0        0        0   268862 2024-05-16 02:31:45.066588 xl2roefact-0.8/tests/Fact_Petrom_11017969.xlsx
+-rw-r--r--   0        0        0    15740 2024-05-16 02:31:45.066588 xl2roefact-0.8/tests/Fact_Petrom_11017969.xml
+-rw-r--r--   0        0        0      986 2024-05-16 02:31:45.066588 xl2roefact-0.8/tests/_test_results.txt
+-rw-r--r--   0        0        0    24173 2024-05-16 02:31:45.066588 xl2roefact-0.8/tests/fact_RENF1004.json
+-rw-r--r--   0        0        0    16332 2024-05-16 02:31:45.066588 xl2roefact-0.8/tests/fact_RENF1004.xlsx
+-rw-r--r--   0        0        0      518 2024-05-16 02:31:45.066588 xl2roefact-0.8/xl2roefact/__init__.py
+-rw-r--r--   0        0        0      601 2024-05-16 02:31:45.066588 xl2roefact-0.8/xl2roefact/__main__.py
+-rw-r--r--   0        0        0     1492 2024-05-16 02:31:45.066588 xl2roefact-0.8/xl2roefact/__version__.py
+-rw-r--r--   0        0        0     8402 2024-05-16 02:31:45.066588 xl2roefact-0.8/xl2roefact/app_cli.py
+-rw-r--r--   0        0        0      727 2024-05-16 02:31:45.066588 xl2roefact-0.8/xl2roefact/chkisld.py
+-rw-r--r--   0        0        0      584 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/chkxml.py
+-rw-r--r--   0        0        0     8898 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/config_settings.py
+-rw-r--r--   0        0        0     1808 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/data/README_app_config_rules.md
+-rw-r--r--   0        0        0      174 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/data/__init__.py
+-rw-r--r--   0        0        0     7134 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/data/app_settings.yml
+-rw-r--r--   0        0        0      600 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/ldxml.py
+-rw-r--r--   0        0        0    10206 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/libutils.py
+-rw-r--r--   0        0        0    71747 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/rdinv.py
+-rw-r--r--   0        0        0     1815 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/sys_settings.py
+-rw-r--r--   0        0        0      612 2024-05-16 02:31:45.070588 xl2roefact-0.8/xl2roefact/wrxml.py
+-rw-r--r--   0        0        0    60998 1970-01-01 00:00:00.000000 xl2roefact-0.8/PKG-INFO
```

### Comparing `xl2roefact-0.7rc2/LICENSE` & `xl2roefact-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc2/README.md` & `xl2roefact-0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
 **Comenzile detaliate:**
 
 <a id="comenzile-aplicatiei"></a>  <!-- #NOTE ATTN do not drop this anchor tag because is referred in `mkdocs.yml` navigation section -->
 
 <!--#NOTE: next section generate application commands in same style as obtained using `--help` CLI options -->
 ::: mkdocs-typer
-    :module: xl2roefact.src.app_cli
+    :module: xl2roefact.app_cli
     :command: app_cli
     :prog_name: xl2roefact
     :depth: 2
 
 
 
 
@@ -223,15 +223,15 @@
 >
 >* una este valoarea introdusa intr-o celula (de ex cu 3 zecimale) si
 >* alta este valoarea afisata (cu 2 zecimale) - aceasta din urma trebuie obtinuta prin formatarea celulei respective de a afisa 2 zecimale prin rotunjire insa valoarea efectiva trebuie sa fie cea originala cu 3 zecimale, lucru (diferenta) care se poate vedea la editarea continutului celulei.
 
 
 ### Reguli recomamdate in configurarea aplicatiei pe specificul Excel al facturilor dumneavoastra
 
-{% include './src/data/README_app_config_rules.md' %}
+{% include './xl2roefact/data/README_app_config_rules.md' %}
 
 
 
 
 ## Tutorial utilizare aplicatie
 
 
@@ -285,14 +285,15 @@
 * `factura_A.xlsx` ca fiind fisierul Excel original cu factura
 * `factura_A.json` acesta fiind fisierul format JSON rezultat in urma procesarii si ce poate fi folosit pentru interschimbarea electronica a informatiei intre sisteme
 
 
 
 
 
+
 ## Aspecte tehnice referitoare la formatul fisierului JSON aferent facturii
 
 Acest fisier este cel generat de catre aplicatie in urma executiei acesteia cu comanda `xl2json`. Formatul JSON are urmatoarra structura de baza:
 
 ```json
 {
     "Invoice": {...},
@@ -312,22 +313,14 @@
 * **`excel_original_data`** - informatiile originale din fisierul Excel, asa cum au fost ele identificate si gasite precum si locatia (adresele celulelor). Aceste informatii sunt utile in cazul in care exista neclaritati in urma procesuluicde conversie pentru "a intelege" de unde si cum arata informatiile originale din fisierul Excel
 
 Detalii suplimentare despre formatul JSON se gasesc in documentaţia *[Referinta dezvoltare software](./doc/README_xl2roefact_library.md)*.
 
 
 
 
-## Descarcare (download) aplicatie xl2roefact CLI
-
-* [Pachet instalare aplicatie Windows](../doc_src/downloads.md#format-executabil-windows-x64)
-* [Pachet instalare script Python](../doc_src/downloads.md#format-biblioteca-python)
-* [Model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact)
-* [Sablon fisier-date informatii furnizor](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor)
-
-
 
 
 ## Referinta dezvoltare software
 
 Documentatia **["Referinta dezvoltare software"](./doc/README_xl2roefact_library.md)** ofera detail necesare pentru utilizarea bibliotecii sursa in dezvoltari specifice, extindere si integrare cu alte sisteme.
```

### Comparing `xl2roefact-0.7rc2/pyproject.toml` & `xl2roefact-0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -51,40 +51,40 @@
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Operating System :: OS Independent",
     "Topic :: Office/Business :: Financial",
 ]
-version = "0.7rc2"
+version = "0.8"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://invoicetoroefact.renware.eu"
 PDF-Documentation = "https://invoicetoroefact.renware.eu/pdfs/print_page.html/print_page.pdf"
 PyPi-Package = "https://pypi.org/project/xl2roefact/"
 GitHub = "https://github.com/petre-renware/api_to_roefact"
 
 [project.scripts]
-xl2roefact = "src.app_cli:main"
+xl2roefact = "xl2roefact.app_cli:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.version]
 source = "file"
-path = "src/__version__.py"
+path = "xl2roefact//__version__.py"
 
 [tool.pdm.build.wheel-data]
 data = [
     { path = "data/*", relative-to = "data/" },
 ]
 
 [tool.pdm.scripts.build_wheel]
@@ -104,18 +104,18 @@
     "--log-level=WARN",
     "--onefile",
     "--noconfirm",
     "xl2roefact_copy_for_sexe.py",
 ]
 
 [tool.pdm.scripts.post_build_sexe]
-call = "src.libutils:complete_sexe_file"
+call = "xl2roefact.libutils:complete_sexe_file"
 
 [tool.pdm.scripts.build_doc]
-shell = "pydoc-markdown -I src >doc/810.05a-xl2roefact_DLD_specs.md"
+shell = "pydoc-markdown -I xl2roefact >doc/810.05a-xl2roefact_DLD_specs.md"
 
 [tool.pdm.scripts.build_all]
 composite = [
     "build_wheel",
     "build_msi",
     "build_sexe",
     "build_doc",
```

### Comparing `xl2roefact-0.7rc2/src/data/README_app_config_rules.md` & `xl2roefact-0.8/xl2roefact/data/README_app_config_rules.md`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc2/src/data/app_settings.yml` & `xl2roefact-0.8/xl2roefact/data/app_settings.yml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.json` & `xl2roefact-0.8/tests/Fact_Petrom_11017969.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857142857142858%*

 * *Differences: {"'Invoice'": "{'cbc_Note': 'generated @2024-05-11T07:24:26.590737+00:00 with xl2roefact by "*

 * *              "RENware Software Systems'}",*

 * * "'meta_info'": "{'last_processing_time': '2024-05-11T07:24:26.590348+00:00'}"}*

```diff
@@ -171,15 +171,15 @@
             "cbc_TaxAmount": 8123.66
         },
         "cbc_DocumentCurrencyCode": "RON",
         "cbc_DueDate": "2023-11-16",
         "cbc_ID": "11017969",
         "cbc_InvoiceTypeCode": "380",
         "cbc_IssueDate": "2023-10-17",
-        "cbc_Note": "generated @2024-05-06T03:19:09.003169+00:00 with xl2roefact by RENware Software Systems",
+        "cbc_Note": "generated @2024-05-11T07:24:26.590737+00:00 with xl2roefact by RENware Software Systems",
         "cbc_TaxPointDate": "2023-11-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 49,
                 8
@@ -485,15 +485,15 @@
         "invoice_max_rows": 49,
         "invoice_worksheet": "Factura(Invoice)",
         "items_table_start_cell": [
             29,
             1
         ],
         "items_table_start_marker": "No. crt.",
-        "last_processing_time": "2024-05-06T03:19:09.002798+00:00",
+        "last_processing_time": "2024-05-11T07:24:26.590348+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
```

### Comparing `xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.xlsx` & `xl2roefact-0.8/tests/Fact_Petrom_11017969.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.xml` & `xl2roefact-0.8/tests/Fact_Petrom_11017969.xml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc2/tests/_test_results.txt` & `xl2roefact-0.8/tests/_test_results.txt`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc2/tests/fact_RENF1004.json` & `xl2roefact-0.8/tests/fact_RENF1004.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857142857142858%*

 * *Differences: {"'Invoice'": "{'cbc_Note': 'generated @2024-05-11T07:24:26.660927+00:00 with xl2roefact by "*

 * *              "RENware Software Systems'}",*

 * * "'meta_info'": "{'last_processing_time': '2024-05-11T07:24:26.660526+00:00'}"}*

```diff
@@ -198,15 +198,15 @@
             "cbc_TaxAmount": 7389.15
         },
         "cbc_DocumentCurrencyCode": "RON",
         "cbc_DueDate": "2023-09-27",
         "cbc_ID": "RENF-1004",
         "cbc_InvoiceTypeCode": "380",
         "cbc_IssueDate": "2023-08-28",
-        "cbc_Note": "generated @2024-05-06T03:19:09.081098+00:00 with xl2roefact by RENware Software Systems",
+        "cbc_Note": "generated @2024-05-11T07:24:26.660927+00:00 with xl2roefact by RENware Software Systems",
         "cbc_TaxPointDate": "2023-09-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 31,
                 9
@@ -560,15 +560,15 @@
         "invoice_max_rows": 31,
         "invoice_worksheet": "FACTURA FINALA",
         "items_table_start_cell": [
             20,
             1
         ],
         "items_table_start_marker": "#",
-        "last_processing_time": "2024-05-06T03:19:09.080691+00:00",
+        "last_processing_time": "2024-05-11T07:24:26.660526+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
```

### Comparing `xl2roefact-0.7rc2/tests/fact_RENF1004.xlsx` & `xl2roefact-0.8/tests/fact_RENF1004.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc2/PKG-INFO` & `xl2roefact-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl2roefact
-Version: 0.7rc2
+Version: 0.8
 Summary: Excel invoices data retrieve, export & upload to RO E-Fact system
 Author-Email: Petre Iordanescu <petre.iordanescu@gmail.com>, RENware Software Systems <renware.systems@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -928,15 +928,15 @@
 
 **Comenzile detaliate:**
 
 <a id="comenzile-aplicatiei"></a>  <!-- #NOTE ATTN do not drop this anchor tag because is referred in `mkdocs.yml` navigation section -->
 
 <!--#NOTE: next section generate application commands in same style as obtained using `--help` CLI options -->
 ::: mkdocs-typer
-    :module: xl2roefact.src.app_cli
+    :module: xl2roefact.app_cli
     :command: app_cli
     :prog_name: xl2roefact
     :depth: 2
 
 
 
 
@@ -952,15 +952,15 @@
 >
 >* una este valoarea introdusa intr-o celula (de ex cu 3 zecimale) si
 >* alta este valoarea afisata (cu 2 zecimale) - aceasta din urma trebuie obtinuta prin formatarea celulei respective de a afisa 2 zecimale prin rotunjire insa valoarea efectiva trebuie sa fie cea originala cu 3 zecimale, lucru (diferenta) care se poate vedea la editarea continutului celulei.
 
 
 ### Reguli recomamdate in configurarea aplicatiei pe specificul Excel al facturilor dumneavoastra
 
-{% include './src/data/README_app_config_rules.md' %}
+{% include './xl2roefact/data/README_app_config_rules.md' %}
 
 
 
 
 ## Tutorial utilizare aplicatie
 
 
@@ -1014,14 +1014,15 @@
 * `factura_A.xlsx` ca fiind fisierul Excel original cu factura
 * `factura_A.json` acesta fiind fisierul format JSON rezultat in urma procesarii si ce poate fi folosit pentru interschimbarea electronica a informatiei intre sisteme
 
 
 
 
 
+
 ## Aspecte tehnice referitoare la formatul fisierului JSON aferent facturii
 
 Acest fisier este cel generat de catre aplicatie in urma executiei acesteia cu comanda `xl2json`. Formatul JSON are urmatoarra structura de baza:
 
 ```json
 {
     "Invoice": {...},
@@ -1041,22 +1042,14 @@
 * **`excel_original_data`** - informatiile originale din fisierul Excel, asa cum au fost ele identificate si gasite precum si locatia (adresele celulelor). Aceste informatii sunt utile in cazul in care exista neclaritati in urma procesuluicde conversie pentru "a intelege" de unde si cum arata informatiile originale din fisierul Excel
 
 Detalii suplimentare despre formatul JSON se gasesc in documentaţia *[Referinta dezvoltare software](./doc/README_xl2roefact_library.md)*.
 
 
 
 
-## Descarcare (download) aplicatie xl2roefact CLI
-
-* [Pachet instalare aplicatie Windows](../doc_src/downloads.md#format-executabil-windows-x64)
-* [Pachet instalare script Python](../doc_src/downloads.md#format-biblioteca-python)
-* [Model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact)
-* [Sablon fisier-date informatii furnizor](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor)
-
-
 
 
 ## Referinta dezvoltare software
 
 Documentatia **["Referinta dezvoltare software"](./doc/README_xl2roefact_library.md)** ofera detail necesare pentru utilizarea bibliotecii sursa in dezvoltari specifice, extindere si integrare cu alte sisteme.
```

