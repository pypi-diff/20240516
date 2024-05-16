# Comparing `tmp/routput-0.9981.tar.gz` & `tmp/routput-0.9982.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.9981.tar", last modified: Thu May 16 12:55:47 2024, max compression
+gzip compressed data, was "routput-0.9982.tar", last modified: Thu May 16 12:57:05 2024, max compression
```

## Comparing `routput-0.9981.tar` & `routput-0.9982.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:55:47.909134 routput-0.9981/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9981/LICENCE
--rw-rw-rw-   0        0        0     2595 2024-05-16 12:55:47.909134 routput-0.9981/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9981/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:55:47.000000 routput-0.9981/README.py
--rw-rw-rw-   0        0        0     3505 2024-05-16 12:55:47.000000 routput-0.9981/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:55:47.908109 routput-0.9981/routput.egg-info/
--rw-rw-rw-   0        0        0     2595 2024-05-16 12:55:47.000000 routput-0.9981/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 12:55:47.000000 routput-0.9981/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:55:47.000000 routput-0.9981/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 12:55:47.000000 routput-0.9981/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:55:47.910139 routput-0.9981/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:45:46.000000 routput-0.9981/setup.py
--rw-rw-rw-   0        0        0    21025 2024-05-16 12:55:47.000000 routput-0.9981/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:57:05.848330 routput-0.9982/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9982/LICENCE
+-rw-rw-rw-   0        0        0     2595 2024-05-16 12:57:05.848330 routput-0.9982/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9982/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:57:05.000000 routput-0.9982/README.py
+-rw-rw-rw-   0        0        0     3505 2024-05-16 12:57:05.000000 routput-0.9982/pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:57:05.847310 routput-0.9982/routput.egg-info/
+-rw-rw-rw-   0        0        0     2595 2024-05-16 12:57:05.000000 routput-0.9982/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 12:57:05.000000 routput-0.9982/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:57:05.000000 routput-0.9982/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-16 12:57:05.000000 routput-0.9982/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:57:05.849347 routput-0.9982/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:45:46.000000 routput-0.9982/setup.py
+-rw-rw-rw-   0        0        0    21056 2024-05-16 12:57:05.000000 routput-0.9982/templated_setup.py
```

### Comparing `routput-0.9981/LICENCE` & `routput-0.9982/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.9981/PKG-INFO` & `routput-0.9982/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9981
+Version: 0.9982
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
@@ -86,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.9981 released on 16th/5/2024
+## V0.9982 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.9981/README.md` & `routput-0.9982/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.9981/README.py` & `routput-0.9982/README.py`

 * *Files identical despite different names*

### Comparing `routput-0.9981/pickled.py` & `routput-0.9982/pickled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-__INST__ = """gASVKwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTk4MZSMBW5vdGVzlIwmYHRlbXBsYXRlZF9zZXR1cGAgaXMgZ2l2aW5nIG1lIGhlbGwuLi6UdWKMBmF1dGhvcpSMGG1hdHJpa2F0ZXIgKEpvZWwgV2F0c29uKZSMC2Rlc2NyaXB0aW9ulIzwcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kulIwEbmFtZZSMB3JvdXRwdXSUjBBsb25nX2Rlc2NyaXB0aW9ulFgaCAAAIyBSZWN1cnNpdmUgT3V0cHV0IFV0aWxpdHkKCiMjIE92ZXJ2aWV3CgpUaGlzIFB5dGhvbiBzY3JpcHQgcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kuCgojIyBSZXF1aXJlbWVudHMKCiogUHl0aG9uIDMuMTAgb3IgaGlnaGVyLAoqIGBiYXRgIChvcHRpb25hbCwgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcpLAoKIyMgSW5zdGFsbGF0aW9uCgojIyMgVXNpbmcgcGlwCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKT24gc29tZSBzeXN0ZW1zLCB5b3UgbWF5IG5lZWQgdG8gcHV0IHRoZSB2ZXJzaW9uIG51bWJlciBvZiBweXRob246CgpgYGBiYXNoCnB5dGhvbjMuMTIgLW0gcGlwIGluc3RhbGwgcm91dHB1dApgYGAKCj4gRm9yIHRoZSBzYWtlIG9mIHNpbXBsaWNpdHksIHdoZW5ldmVyIEkgbWVudGlvbiBgcHl0aG9uYCBpbiB0aGUgZm9sbG93aW5nIHNlY3Rpb25zLCB5b3UgY2FuIHJlcGxhY2UgaXQgd2l0aCBgcHl0aG9uMy54YCB2ZXJzaW9uIGlmIG5lY2Vzc2FyeS4KCiMjIyBGcm9tIHNvdXJjZQoKQ2xvbmUgdGhpcyByZXBvc2l0b3J5LgoKYGBgYmFzaApnaXQgY2xvbmUgaHR0cHM6Ly9naXRodWIuY29tL25hY2lvYm9pL3JvdXRwdXQuZ2l0CmBgYAoKTmF2aWdhdGUgdG8gdGhlIHJlcG9zaXRvcnkgZGlyZWN0b3J5LgoKYGBgYmFzaApjZCByb3V0cHV0CmBgYAoKQW5kIGluc3RhbGwgdGhlIHBhY2thZ2UuCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCAuCmBgYAoKIyMgVXNhZ2UKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQgW29wdGlvbnNdCmBgYAoKT3B0aW9ucwoKKiAtZCwgLS1zdGFydGluZy1kaXJlY3Rvcnk6IERpcmVjdG9yeSB0byBzdGFydCB0aGUgc2VhcmNoIGZyb20gKGRlZmF1bHQ6IGN1cnJlbnQgZGlyZWN0b3J5KS4KKiAtcywgLS1kby1wcmludC1zdHJ1Y3R1cmU6IFByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLgoqIC1lLCAtLWV4dGVuc2lvbnM6IExpc3Qgb2YgZmlsZSBleHRlbnNpb25zIHRvIHNlYXJjaCBmb3IsIGZvcm1hdCBbZXh0MSxleHQyLC4uLl0gKGRlZmF1bHQ6IFtjLGhdKS4KKiAtcCwgLS1kby1wcm90ZWN0LXByaXZhY3k6IEFub255bWl6ZSBmaWxlIHBhdGhzLgoqIC1hLCAtLWFsc28taW5jbHVkZTogTGlzdCBvZiBhZGRpdGlvbmFsIGZpbGVuYW1lcyB0byBpbmNsdWRlLCBmb3JtYXQgW2ZpbGUxLGZpbGUyLC4uLl0uCiogLWksIC0taWdub3JlOiBMaXN0IG9mIGZpbGVuYW1lcyB0byBpZ25vcmUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsZGlyMSxkaXIyLi4uXS4KKiAtbiwgLS1uby1wcmludDogRG9uJ3QgcHJpbnQgdGhlIGZpbGVzLCBqdXN0IHJldHVybiB0aGVtLgoqIC1iLCAtLWRvLXVzZS1iYXQ6IFVzZSBiYXQgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcuCiogLWMsIC0tZG8tY29sb3JzOiBVc2UgZGlmZmVyZW50IGNvbG9ycyBmb3IgZWFjaCBmaWxlIHR5cGUuCiogLWgsIC0taGVscDogU2hvdyBoZWxwIG1lc3NhZ2UgYW5kIGV4aXQuCgojIyBFeGFtcGxlcwoKVG8gcHJpbnQgdGhlIHN0cnVjdHVyZSBvZiBhIGRpcmVjdG9yeToKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQucHkgLWQgL3BhdGgvdG8vZGlyZWN0b3J5IC1zCmBgYAoKVG8gZmluZCBhbmQgcHJpbnQgLnB5IGZpbGVzIGluIHRoZSBjdXJyZW50IGRpcmVjdG9yeSwgdXNpbmcgYmF0IGZvciBoaWdobGlnaHRpbmc6CgpgYGBiYXNoCnB5dGhvbiByb3V0cHV0LnB5IC1lIFtweV0gLWIKYGBgCgojIyBMaWNlbnNlCgpPcGVuLXNvdXJjZSBzb2Z0d2FyZSBsaWNlbnNlZCB1bmRlciBHUEwtMiBsaWNlbnNlLgoKIyMgVjAuOTk4MSByZWxlYXNlZCBvbiAxNnRoLzUvMjAyNApgdGVtcGxhdGVkX3NldHVwYCBpcyBnaXZpbmcgbWUgaGVsbC4uLpSMFmt3YXJnc19mb3Jfc2V0dXBfdG9vbHOUfZR1Lg=="""
+__INST__ = """gASVKwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTk4MpSMBW5vdGVzlIwmYHRlbXBsYXRlZF9zZXR1cGAgaXMgZ2l2aW5nIG1lIGhlbGwuLi6UdWKMBmF1dGhvcpSMGG1hdHJpa2F0ZXIgKEpvZWwgV2F0c29uKZSMC2Rlc2NyaXB0aW9ulIzwcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kulIwEbmFtZZSMB3JvdXRwdXSUjBBsb25nX2Rlc2NyaXB0aW9ulFgaCAAAIyBSZWN1cnNpdmUgT3V0cHV0IFV0aWxpdHkKCiMjIE92ZXJ2aWV3CgpUaGlzIFB5dGhvbiBzY3JpcHQgcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kuCgojIyBSZXF1aXJlbWVudHMKCiogUHl0aG9uIDMuMTAgb3IgaGlnaGVyLAoqIGBiYXRgIChvcHRpb25hbCwgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcpLAoKIyMgSW5zdGFsbGF0aW9uCgojIyMgVXNpbmcgcGlwCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKT24gc29tZSBzeXN0ZW1zLCB5b3UgbWF5IG5lZWQgdG8gcHV0IHRoZSB2ZXJzaW9uIG51bWJlciBvZiBweXRob246CgpgYGBiYXNoCnB5dGhvbjMuMTIgLW0gcGlwIGluc3RhbGwgcm91dHB1dApgYGAKCj4gRm9yIHRoZSBzYWtlIG9mIHNpbXBsaWNpdHksIHdoZW5ldmVyIEkgbWVudGlvbiBgcHl0aG9uYCBpbiB0aGUgZm9sbG93aW5nIHNlY3Rpb25zLCB5b3UgY2FuIHJlcGxhY2UgaXQgd2l0aCBgcHl0aG9uMy54YCB2ZXJzaW9uIGlmIG5lY2Vzc2FyeS4KCiMjIyBGcm9tIHNvdXJjZQoKQ2xvbmUgdGhpcyByZXBvc2l0b3J5LgoKYGBgYmFzaApnaXQgY2xvbmUgaHR0cHM6Ly9naXRodWIuY29tL25hY2lvYm9pL3JvdXRwdXQuZ2l0CmBgYAoKTmF2aWdhdGUgdG8gdGhlIHJlcG9zaXRvcnkgZGlyZWN0b3J5LgoKYGBgYmFzaApjZCByb3V0cHV0CmBgYAoKQW5kIGluc3RhbGwgdGhlIHBhY2thZ2UuCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCAuCmBgYAoKIyMgVXNhZ2UKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQgW29wdGlvbnNdCmBgYAoKT3B0aW9ucwoKKiAtZCwgLS1zdGFydGluZy1kaXJlY3Rvcnk6IERpcmVjdG9yeSB0byBzdGFydCB0aGUgc2VhcmNoIGZyb20gKGRlZmF1bHQ6IGN1cnJlbnQgZGlyZWN0b3J5KS4KKiAtcywgLS1kby1wcmludC1zdHJ1Y3R1cmU6IFByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLgoqIC1lLCAtLWV4dGVuc2lvbnM6IExpc3Qgb2YgZmlsZSBleHRlbnNpb25zIHRvIHNlYXJjaCBmb3IsIGZvcm1hdCBbZXh0MSxleHQyLC4uLl0gKGRlZmF1bHQ6IFtjLGhdKS4KKiAtcCwgLS1kby1wcm90ZWN0LXByaXZhY3k6IEFub255bWl6ZSBmaWxlIHBhdGhzLgoqIC1hLCAtLWFsc28taW5jbHVkZTogTGlzdCBvZiBhZGRpdGlvbmFsIGZpbGVuYW1lcyB0byBpbmNsdWRlLCBmb3JtYXQgW2ZpbGUxLGZpbGUyLC4uLl0uCiogLWksIC0taWdub3JlOiBMaXN0IG9mIGZpbGVuYW1lcyB0byBpZ25vcmUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsZGlyMSxkaXIyLi4uXS4KKiAtbiwgLS1uby1wcmludDogRG9uJ3QgcHJpbnQgdGhlIGZpbGVzLCBqdXN0IHJldHVybiB0aGVtLgoqIC1iLCAtLWRvLXVzZS1iYXQ6IFVzZSBiYXQgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcuCiogLWMsIC0tZG8tY29sb3JzOiBVc2UgZGlmZmVyZW50IGNvbG9ycyBmb3IgZWFjaCBmaWxlIHR5cGUuCiogLWgsIC0taGVscDogU2hvdyBoZWxwIG1lc3NhZ2UgYW5kIGV4aXQuCgojIyBFeGFtcGxlcwoKVG8gcHJpbnQgdGhlIHN0cnVjdHVyZSBvZiBhIGRpcmVjdG9yeToKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQucHkgLWQgL3BhdGgvdG8vZGlyZWN0b3J5IC1zCmBgYAoKVG8gZmluZCBhbmQgcHJpbnQgLnB5IGZpbGVzIGluIHRoZSBjdXJyZW50IGRpcmVjdG9yeSwgdXNpbmcgYmF0IGZvciBoaWdobGlnaHRpbmc6CgpgYGBiYXNoCnB5dGhvbiByb3V0cHV0LnB5IC1lIFtweV0gLWIKYGBgCgojIyBMaWNlbnNlCgpPcGVuLXNvdXJjZSBzb2Z0d2FyZSBsaWNlbnNlZCB1bmRlciBHUEwtMiBsaWNlbnNlLgoKIyMgVjAuOTk4MiByZWxlYXNlZCBvbiAxNnRoLzUvMjAyNApgdGVtcGxhdGVkX3NldHVwYCBpcyBnaXZpbmcgbWUgaGVsbC4uLpSMFmt3YXJnc19mb3Jfc2V0dXBfdG9vbHOUfZR1Lg=="""
```

### Comparing `routput-0.9981/routput.egg-info/PKG-INFO` & `routput-0.9982/routput.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9981
+Version: 0.9982
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
@@ -86,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.9981 released on 16th/5/2024
+## V0.9982 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.9981/templated_setup.py` & `routput-0.9982/templated_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,16 +681,16 @@
 		description = c["description"]
 		long_description = c["long_description"]
 		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
 		if not kwargs_for_setup_tools.get("py_modules"):
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 		kwargs_for_setup_tools["py_modules"].append("pickled")
+		kwargs_for_setup_tools["py_modules"].append("README")
 
-		os.remove("README.py")
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
 			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
```

