# Comparing `tmp/templated_setup-0.984.tar.gz` & `tmp/templated_setup-0.985.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.984.tar", last modified: Thu May 16 10:20:05 2024, max compression
+gzip compressed data, was "templated_setup-0.985.tar", last modified: Thu May 16 10:48:12 2024, max compression
```

## Comparing `templated_setup-0.984.tar` & `templated_setup-0.985.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:20:05.001454 templated_setup-0.984/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.984/LICENCE
--rw-rw-rw-   0        0        0     2588 2024-05-16 10:20:05.000439 templated_setup-0.984/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.984/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 10:20:05.001454 templated_setup-0.984/setup.cfg
--rw-rw-rw-   0        0        0      427 2024-05-16 10:16:28.000000 templated_setup-0.984/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:20:04.993796 templated_setup-0.984/templated_setup/
--rw-rw-rw-   0        0        0    20331 2024-05-16 10:12:22.000000 templated_setup-0.984/templated_setup/__init__.py
--rw-rw-rw-   0        0        0     3271 2024-05-16 10:20:04.000000 templated_setup-0.984/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:20:04.999401 templated_setup-0.984/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2588 2024-05-16 10:20:04.000000 templated_setup-0.984/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-16 10:20:04.000000 templated_setup-0.984/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:20:04.000000 templated_setup-0.984/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 10:20:04.000000 templated_setup-0.984/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 10:20:04.000000 templated_setup-0.984/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 10:48:12.282345 templated_setup-0.985/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.985/LICENCE
+-rw-rw-rw-   0        0        0     2588 2024-05-16 10:48:12.281327 templated_setup-0.985/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.985/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 10:48:12.282345 templated_setup-0.985/setup.cfg
+-rw-rw-rw-   0        0        0      427 2024-05-16 10:47:19.000000 templated_setup-0.985/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:48:12.274696 templated_setup-0.985/templated_setup/
+-rw-rw-rw-   0        0        0    20503 2024-05-16 10:47:17.000000 templated_setup-0.985/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0     3271 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:48:12.280307 templated_setup-0.985/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2588 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.984/LICENCE` & `templated_setup-0.985/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.984/PKG-INFO` & `templated_setup-0.985/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.984
+Version: 0.985
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 Requires-Dist: setuptools
 Requires-Dist: twine
@@ -67,9 +67,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.984 released on 16th/5/2024
+## V0.985 released on 16th/5/2024
 this module is hell.
```

### Comparing `templated_setup-0.984/README.md` & `templated_setup-0.985/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.984/templated_setup/__init__.py` & `templated_setup-0.985/templated_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,24 +750,32 @@
 		with open(_hardcoded.__file__, "w") as f:
 			f.write(f"__version__ = \"{cls._version.version_number}\"\n")
 			f.write(f"__author__ = \"{cls._author}\"\n")
 			f.write(f"__description__ = \"{cls._description}\"\n")
 			f.write(f"__long_description__ = \"\"\"{s_long_description}\"\"\"\n")
 			f.write(f"__kwargs_for_setup_tools__ = \"\"\"{s_kwargs_for_setup_tools}\"\"\"\n")
 
+		meta = None
+		with open(__file__, "r") as f:
+			meta = f.read()
+		with open("templated_setup.py", "w") as f:
+			f.write(meta)
+
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
+		os.remove("templated_setup.py")
+
 		print("\n] Setup complete.\n\n")
 
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
 
 		_Setup_Helper.__clear_screen()
```

### Comparing `templated_setup-0.984/templated_setup/_hardcoded.py` & `templated_setup-0.985/templated_setup/_hardcoded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.984"
+__version__ = "0.985"
 __author__ = "matrikater (Joel Watson)"
 __description__ = "A quick and easy replacement for some `setup.py` implementations."
-__long_description__ = """gASVfQgAAAAAAABYdggAACMgU3RhbmRhcmRpemVkIGBzZXR1cC5weWAKCiMjIE92ZXJ2aWV3CgpUaGlzIHByb2plY3QgY29udGFpbnMgYSBQeXRob24tYmFzZWQgc2V0dXAgYXV0b21hdGlvbiB0b29sIGRlc2lnbmVkIHRvIGhlbHAgc3RyZWFtbGluZSB0aGUgcHJvY2VzcyBvZiBwcmVwYXJpbmcgYW5kIG1hbmFnaW5nIHByb2plY3Qgc2V0dXBzLiBJdCBpbmNsdWRlcyB1dGlsaXRpZXMgZm9yIGhhbmRsaW5nIHZlcnNpb25pbmcsIGRhdGVzLCBub3RlcywgYW5kIFJFQURNRSBmaWxlcywgbGV2ZXJhZ2luZyBhIGR5bmFtaWMgY2FjaGluZyBzeXN0ZW0gdG8gbWFpbnRhaW4gc3RhdGUgYWNyb3NzIHNlc3Npb25zLgoKIyMgV29yZCBvZiBDYXV0aW9uCgo6d2FybmluZzogKipUaGlzIHByb2plY3QgaXMgc3RpbGwgaW4gZGV2ZWxvcG1lbnQgYW5kIHNob3VsZCBiZSB1c2VkIHdpdGggY2F1dGlvbi4qKiA6d2FybmluZzoKCiMjIFBsYW5uZWQgRmVhdHVyZXMKCi0gWyBdICoqRGF0ZSBNYW5hZ2VtZW50OioqIEF1dG9tYXRpY2FsbHkgbWFuYWdlcyB0aGUgZGF0ZSBvZiB0aGUgbGFzdCBtb2RpZmljYXRpb24gdXNpbmcgYSBjdXN0b20gY2xhc3MuCi0gWyBdICoqVmVyc2lvbiBDb250cm9sOioqIFZhbGlkYXRlcyBhbmQgc3RvcmVzIHZlcnNpb24gbnVtYmVycyB3aXRoIGEgc3RyaWN0IGZvcm1hdC4KLSBbIF0gKipOb3RlcyBNYW5hZ2VtZW50OioqIFN1cHBvcnRzIGNhcHR1cmluZyBhbmQgZm9ybWF0dGluZyByZWxlYXNlIG5vdGVzIGZvciBlYXN5IGluY2x1c2lvbiBpbiBwcm9qZWN0IGRvY3VtZW50YXRpb24uCi0gWyBdICoqQXV0b21hdGVkIFNldHVwOioqIEludGVncmF0ZXMgd2l0aCBgc2V0dXB0b29sc2AgZm9yIHNlYW1sZXNzIHBhY2thZ2UgZGlzdHJpYnV0aW9uIHByZXBhcmF0aW9uLgoKIyMgUmVxdWlyZW1lbnRzCgotIFB5dGhvbiAzLngKLSBgc2V0dXB0b29sc2AgbW9kdWxlCgojIyBVc2FnZQoKMS4gKipJbml0aWFsaXphdGlvbjoqKiBTdGFydCBieSBjb25maWd1cmluZyB0aGUgYmFzaWMgcHJvamVjdCBwYXJhbWV0ZXJzIGxpa2UgbmFtZSwgdmVyc2lvbiwgYW5kIGRlc2NyaXB0aW9uLgoyLiAqKlBhcmFtZXRlciBNYW5hZ2VtZW50OioqIFRocm91Z2ggaW50ZXJhY3RpdmUgcHJvbXB0cywgbWFuYWdlIHZhcmlvdXMgcGFyYW1ldGVycyBpbmNsdWRpbmcgdmVyc2lvbiBudW1iZXIsCiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBtb2RpZmljYXRpb24gZGF0ZXMsIGFuZCByZWxlYXNlIG5vdGVzLgozLiAqKlNldHVwIEV4ZWN1dGlvbjoqKiBFeGVjdXRlIHRoZSBzZXR1cCB0byBnZW5lcmF0ZSBkaXN0cmlidXRpb24gcGFja2FnZXMgYW5kLCBvcHRpb25hbGx5LCBwdWJsaXNoIHRoZW0gdG8gUHlQaS4KCiMjIyBFeGFtcGxlCgpgYGBweXRob24KZnJvbSB0ZW1wbGF0ZWRfc2V0dXAgaW1wb3J0IFNldHVwX0hlbHBlcgoKREVTQ1JJUFRJT04gPSAiQSBxdWljayBhbmQgZWFzeSByZXBsYWNlbWVudCBmb3Igc29tZSBgc2V0dXAucHlgIGltcGxlbWVudGF0aW9ucy4iCgpTZXR1cF9IZWxwZXIuc2V0dXAoCgluYW1lPSJ0ZW1wbGF0ZWRfc2V0dXAiLAoJYXV0aG9yPSJtYXRyaWthdGVyIChKb2VsIFdhdHNvbikiLAoJZGVzY3JpcHRpb249REVTQ1JJUFRJT04sCglhdXRob3JfZW1haWw9ImFkbWluaXN0cmFpdG9yQG1hdHJpa28ueHl6IiwKKQpgYGAKCiMjIEluc3RhbGxhdGlvbgoKVG8gaW5zdGFsbCB0aGUgcGFja2FnZSwgcnVuIHRoZSBmb2xsb3dpbmcgY29tbWFuZDoKCmBgYGJhc2gKcGlwIGluc3RhbGwgdGVtcGxhdGVkLXNldHVwCmBgYAoKIyMgQ29udHJpYnV0aW5nCgpDb250cmlidXRpb25zIGFyZSB3ZWxjb21lISBGb3IgZmVhdHVyZSByZXF1ZXN0cywgYnVnIHJlcG9ydHMsIG9yIHF1ZXN0aW9ucywgcGxlYXNlIHN1Ym1pdCBhbiBpc3N1ZS4KCj4gQWN0dWFsbHkgSSB3b3VsZCBiZSBoYXBweSB0byBoYXZlIHNvbWUgaGVscCB3aXRoIHRoaXMgcHJvamVjdCBhcyBtYWtpbmcgYSBgc2V0dXAucHlgIGV2ZXJ5IHRpbWUgaXMgYSBiaXQgYm9yaW5nLgoKIyMgTGljZW5zZQoKVGhpcyBwcm9qZWN0IGlzIGxpY2Vuc2VkIHVuZGVyIHRoZSBHUEx2MiBMaWNlbnNlIC0gc2VlIHRoZSBbTElDRU5TRV0oTElDRU5TRSkgZmlsZSBmb3IgZGV0YWlscy4KCiMjIFYwLjk4NCByZWxlYXNlZCBvbiAxNnRoLzUvMjAyNAp0aGlzIG1vZHVsZSBpcyBoZWxsLpQu"""
+__long_description__ = """gASVfQgAAAAAAABYdggAACMgU3RhbmRhcmRpemVkIGBzZXR1cC5weWAKCiMjIE92ZXJ2aWV3CgpUaGlzIHByb2plY3QgY29udGFpbnMgYSBQeXRob24tYmFzZWQgc2V0dXAgYXV0b21hdGlvbiB0b29sIGRlc2lnbmVkIHRvIGhlbHAgc3RyZWFtbGluZSB0aGUgcHJvY2VzcyBvZiBwcmVwYXJpbmcgYW5kIG1hbmFnaW5nIHByb2plY3Qgc2V0dXBzLiBJdCBpbmNsdWRlcyB1dGlsaXRpZXMgZm9yIGhhbmRsaW5nIHZlcnNpb25pbmcsIGRhdGVzLCBub3RlcywgYW5kIFJFQURNRSBmaWxlcywgbGV2ZXJhZ2luZyBhIGR5bmFtaWMgY2FjaGluZyBzeXN0ZW0gdG8gbWFpbnRhaW4gc3RhdGUgYWNyb3NzIHNlc3Npb25zLgoKIyMgV29yZCBvZiBDYXV0aW9uCgo6d2FybmluZzogKipUaGlzIHByb2plY3QgaXMgc3RpbGwgaW4gZGV2ZWxvcG1lbnQgYW5kIHNob3VsZCBiZSB1c2VkIHdpdGggY2F1dGlvbi4qKiA6d2FybmluZzoKCiMjIFBsYW5uZWQgRmVhdHVyZXMKCi0gWyBdICoqRGF0ZSBNYW5hZ2VtZW50OioqIEF1dG9tYXRpY2FsbHkgbWFuYWdlcyB0aGUgZGF0ZSBvZiB0aGUgbGFzdCBtb2RpZmljYXRpb24gdXNpbmcgYSBjdXN0b20gY2xhc3MuCi0gWyBdICoqVmVyc2lvbiBDb250cm9sOioqIFZhbGlkYXRlcyBhbmQgc3RvcmVzIHZlcnNpb24gbnVtYmVycyB3aXRoIGEgc3RyaWN0IGZvcm1hdC4KLSBbIF0gKipOb3RlcyBNYW5hZ2VtZW50OioqIFN1cHBvcnRzIGNhcHR1cmluZyBhbmQgZm9ybWF0dGluZyByZWxlYXNlIG5vdGVzIGZvciBlYXN5IGluY2x1c2lvbiBpbiBwcm9qZWN0IGRvY3VtZW50YXRpb24uCi0gWyBdICoqQXV0b21hdGVkIFNldHVwOioqIEludGVncmF0ZXMgd2l0aCBgc2V0dXB0b29sc2AgZm9yIHNlYW1sZXNzIHBhY2thZ2UgZGlzdHJpYnV0aW9uIHByZXBhcmF0aW9uLgoKIyMgUmVxdWlyZW1lbnRzCgotIFB5dGhvbiAzLngKLSBgc2V0dXB0b29sc2AgbW9kdWxlCgojIyBVc2FnZQoKMS4gKipJbml0aWFsaXphdGlvbjoqKiBTdGFydCBieSBjb25maWd1cmluZyB0aGUgYmFzaWMgcHJvamVjdCBwYXJhbWV0ZXJzIGxpa2UgbmFtZSwgdmVyc2lvbiwgYW5kIGRlc2NyaXB0aW9uLgoyLiAqKlBhcmFtZXRlciBNYW5hZ2VtZW50OioqIFRocm91Z2ggaW50ZXJhY3RpdmUgcHJvbXB0cywgbWFuYWdlIHZhcmlvdXMgcGFyYW1ldGVycyBpbmNsdWRpbmcgdmVyc2lvbiBudW1iZXIsCiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBtb2RpZmljYXRpb24gZGF0ZXMsIGFuZCByZWxlYXNlIG5vdGVzLgozLiAqKlNldHVwIEV4ZWN1dGlvbjoqKiBFeGVjdXRlIHRoZSBzZXR1cCB0byBnZW5lcmF0ZSBkaXN0cmlidXRpb24gcGFja2FnZXMgYW5kLCBvcHRpb25hbGx5LCBwdWJsaXNoIHRoZW0gdG8gUHlQaS4KCiMjIyBFeGFtcGxlCgpgYGBweXRob24KZnJvbSB0ZW1wbGF0ZWRfc2V0dXAgaW1wb3J0IFNldHVwX0hlbHBlcgoKREVTQ1JJUFRJT04gPSAiQSBxdWljayBhbmQgZWFzeSByZXBsYWNlbWVudCBmb3Igc29tZSBgc2V0dXAucHlgIGltcGxlbWVudGF0aW9ucy4iCgpTZXR1cF9IZWxwZXIuc2V0dXAoCgluYW1lPSJ0ZW1wbGF0ZWRfc2V0dXAiLAoJYXV0aG9yPSJtYXRyaWthdGVyIChKb2VsIFdhdHNvbikiLAoJZGVzY3JpcHRpb249REVTQ1JJUFRJT04sCglhdXRob3JfZW1haWw9ImFkbWluaXN0cmFpdG9yQG1hdHJpa28ueHl6IiwKKQpgYGAKCiMjIEluc3RhbGxhdGlvbgoKVG8gaW5zdGFsbCB0aGUgcGFja2FnZSwgcnVuIHRoZSBmb2xsb3dpbmcgY29tbWFuZDoKCmBgYGJhc2gKcGlwIGluc3RhbGwgdGVtcGxhdGVkLXNldHVwCmBgYAoKIyMgQ29udHJpYnV0aW5nCgpDb250cmlidXRpb25zIGFyZSB3ZWxjb21lISBGb3IgZmVhdHVyZSByZXF1ZXN0cywgYnVnIHJlcG9ydHMsIG9yIHF1ZXN0aW9ucywgcGxlYXNlIHN1Ym1pdCBhbiBpc3N1ZS4KCj4gQWN0dWFsbHkgSSB3b3VsZCBiZSBoYXBweSB0byBoYXZlIHNvbWUgaGVscCB3aXRoIHRoaXMgcHJvamVjdCBhcyBtYWtpbmcgYSBgc2V0dXAucHlgIGV2ZXJ5IHRpbWUgaXMgYSBiaXQgYm9yaW5nLgoKIyMgTGljZW5zZQoKVGhpcyBwcm9qZWN0IGlzIGxpY2Vuc2VkIHVuZGVyIHRoZSBHUEx2MiBMaWNlbnNlIC0gc2VlIHRoZSBbTElDRU5TRV0oTElDRU5TRSkgZmlsZSBmb3IgZGV0YWlscy4KCiMjIFYwLjk4NSByZWxlYXNlZCBvbiAxNnRoLzUvMjAyNAp0aGlzIG1vZHVsZSBpcyBoZWxsLpQu"""
 __kwargs_for_setup_tools__ = """gASVXQAAAAAAAAB9lCiMDGF1dGhvcl9lbWFpbJSMGmFkbWluaXN0cmFpdG9yQG1hdHJpa28ueHl6lIwQaW5zdGFsbF9yZXF1aXJlc5RdlCiMCnNldHVwdG9vbHOUjAV0d2luZZRldS4="""
```

### Comparing `templated_setup-0.984/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.985/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.984
+Version: 0.985
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 Requires-Dist: setuptools
 Requires-Dist: twine
@@ -67,9 +67,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.984 released on 16th/5/2024
+## V0.985 released on 16th/5/2024
 this module is hell.
```

