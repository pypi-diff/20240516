# Comparing `tmp/routput-0.9977.tar.gz` & `tmp/routput-0.9978.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.9977.tar", last modified: Thu May 16 12:43:15 2024, max compression
+gzip compressed data, was "routput-0.9978.tar", last modified: Thu May 16 12:46:06 2024, max compression
```

## Comparing `routput-0.9977.tar` & `routput-0.9978.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:43:15.755808 routput-0.9977/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9977/LICENCE
--rw-rw-rw-   0        0        0     2595 2024-05-16 12:43:15.754791 routput-0.9977/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9977/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:43:15.000000 routput-0.9977/README.py
--rw-rw-rw-   0        0        0     3505 2024-05-16 12:43:15.000000 routput-0.9977/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:43:15.754791 routput-0.9977/routput.egg-info/
--rw-rw-rw-   0        0        0     2595 2024-05-16 12:43:15.000000 routput-0.9977/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 12:43:15.000000 routput-0.9977/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:43:15.000000 routput-0.9977/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 12:43:15.000000 routput-0.9977/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:43:15.755808 routput-0.9977/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:42:38.000000 routput-0.9977/setup.py
--rw-rw-rw-   0        0        0    20947 2024-05-16 12:43:15.000000 routput-0.9977/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:46:06.388990 routput-0.9978/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9978/LICENCE
+-rw-rw-rw-   0        0        0     2595 2024-05-16 12:46:06.387973 routput-0.9978/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9978/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:46:06.000000 routput-0.9978/README.py
+-rw-rw-rw-   0        0        0     3505 2024-05-16 12:46:06.000000 routput-0.9978/pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:46:06.386954 routput-0.9978/routput.egg-info/
+-rw-rw-rw-   0        0        0     2595 2024-05-16 12:46:06.000000 routput-0.9978/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 12:46:06.000000 routput-0.9978/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:46:06.000000 routput-0.9978/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-16 12:46:06.000000 routput-0.9978/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:46:06.388990 routput-0.9978/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:45:46.000000 routput-0.9978/setup.py
+-rw-rw-rw-   0        0        0    20947 2024-05-16 12:46:06.000000 routput-0.9978/templated_setup.py
```

### Comparing `routput-0.9977/LICENCE` & `routput-0.9978/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.9977/PKG-INFO` & `routput-0.9978/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9977
+Version: 0.9978
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
 
-## V0.9977 released on 16th/5/2024
+## V0.9978 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.9977/README.md` & `routput-0.9978/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.9977/README.py` & `routput-0.9978/README.py`

 * *Files identical despite different names*

### Comparing `routput-0.9977/pickled.py` & `routput-0.9978/pickled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-__INST__ = """gASVKwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTk3N5SMBW5vdGVzlIwmYHRlbXBsYXRlZF9zZXR1cGAgaXMgZ2l2aW5nIG1lIGhlbGwuLi6UdWKMBmF1dGhvcpSMGG1hdHJpa2F0ZXIgKEpvZWwgV2F0c29uKZSMC2Rlc2NyaXB0aW9ulIzwcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kulIwEbmFtZZSMB3JvdXRwdXSUjBBsb25nX2Rlc2NyaXB0aW9ulFgaCAAAIyBSZWN1cnNpdmUgT3V0cHV0IFV0aWxpdHkKCiMjIE92ZXJ2aWV3CgpUaGlzIFB5dGhvbiBzY3JpcHQgcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kuCgojIyBSZXF1aXJlbWVudHMKCiogUHl0aG9uIDMuMTAgb3IgaGlnaGVyLAoqIGBiYXRgIChvcHRpb25hbCwgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcpLAoKIyMgSW5zdGFsbGF0aW9uCgojIyMgVXNpbmcgcGlwCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKT24gc29tZSBzeXN0ZW1zLCB5b3UgbWF5IG5lZWQgdG8gcHV0IHRoZSB2ZXJzaW9uIG51bWJlciBvZiBweXRob246CgpgYGBiYXNoCnB5dGhvbjMuMTIgLW0gcGlwIGluc3RhbGwgcm91dHB1dApgYGAKCj4gRm9yIHRoZSBzYWtlIG9mIHNpbXBsaWNpdHksIHdoZW5ldmVyIEkgbWVudGlvbiBgcHl0aG9uYCBpbiB0aGUgZm9sbG93aW5nIHNlY3Rpb25zLCB5b3UgY2FuIHJlcGxhY2UgaXQgd2l0aCBgcHl0aG9uMy54YCB2ZXJzaW9uIGlmIG5lY2Vzc2FyeS4KCiMjIyBGcm9tIHNvdXJjZQoKQ2xvbmUgdGhpcyByZXBvc2l0b3J5LgoKYGBgYmFzaApnaXQgY2xvbmUgaHR0cHM6Ly9naXRodWIuY29tL25hY2lvYm9pL3JvdXRwdXQuZ2l0CmBgYAoKTmF2aWdhdGUgdG8gdGhlIHJlcG9zaXRvcnkgZGlyZWN0b3J5LgoKYGBgYmFzaApjZCByb3V0cHV0CmBgYAoKQW5kIGluc3RhbGwgdGhlIHBhY2thZ2UuCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCAuCmBgYAoKIyMgVXNhZ2UKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQgW29wdGlvbnNdCmBgYAoKT3B0aW9ucwoKKiAtZCwgLS1zdGFydGluZy1kaXJlY3Rvcnk6IERpcmVjdG9yeSB0byBzdGFydCB0aGUgc2VhcmNoIGZyb20gKGRlZmF1bHQ6IGN1cnJlbnQgZGlyZWN0b3J5KS4KKiAtcywgLS1kby1wcmludC1zdHJ1Y3R1cmU6IFByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLgoqIC1lLCAtLWV4dGVuc2lvbnM6IExpc3Qgb2YgZmlsZSBleHRlbnNpb25zIHRvIHNlYXJjaCBmb3IsIGZvcm1hdCBbZXh0MSxleHQyLC4uLl0gKGRlZmF1bHQ6IFtjLGhdKS4KKiAtcCwgLS1kby1wcm90ZWN0LXByaXZhY3k6IEFub255bWl6ZSBmaWxlIHBhdGhzLgoqIC1hLCAtLWFsc28taW5jbHVkZTogTGlzdCBvZiBhZGRpdGlvbmFsIGZpbGVuYW1lcyB0byBpbmNsdWRlLCBmb3JtYXQgW2ZpbGUxLGZpbGUyLC4uLl0uCiogLWksIC0taWdub3JlOiBMaXN0IG9mIGZpbGVuYW1lcyB0byBpZ25vcmUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsZGlyMSxkaXIyLi4uXS4KKiAtbiwgLS1uby1wcmludDogRG9uJ3QgcHJpbnQgdGhlIGZpbGVzLCBqdXN0IHJldHVybiB0aGVtLgoqIC1iLCAtLWRvLXVzZS1iYXQ6IFVzZSBiYXQgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcuCiogLWMsIC0tZG8tY29sb3JzOiBVc2UgZGlmZmVyZW50IGNvbG9ycyBmb3IgZWFjaCBmaWxlIHR5cGUuCiogLWgsIC0taGVscDogU2hvdyBoZWxwIG1lc3NhZ2UgYW5kIGV4aXQuCgojIyBFeGFtcGxlcwoKVG8gcHJpbnQgdGhlIHN0cnVjdHVyZSBvZiBhIGRpcmVjdG9yeToKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQucHkgLWQgL3BhdGgvdG8vZGlyZWN0b3J5IC1zCmBgYAoKVG8gZmluZCBhbmQgcHJpbnQgLnB5IGZpbGVzIGluIHRoZSBjdXJyZW50IGRpcmVjdG9yeSwgdXNpbmcgYmF0IGZvciBoaWdobGlnaHRpbmc6CgpgYGBiYXNoCnB5dGhvbiByb3V0cHV0LnB5IC1lIFtweV0gLWIKYGBgCgojIyBMaWNlbnNlCgpPcGVuLXNvdXJjZSBzb2Z0d2FyZSBsaWNlbnNlZCB1bmRlciBHUEwtMiBsaWNlbnNlLgoKIyMgVjAuOTk3NyByZWxlYXNlZCBvbiAxNnRoLzUvMjAyNApgdGVtcGxhdGVkX3NldHVwYCBpcyBnaXZpbmcgbWUgaGVsbC4uLpSMFmt3YXJnc19mb3Jfc2V0dXBfdG9vbHOUfZR1Lg=="""
+__INST__ = """gASVKwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTk3OJSMBW5vdGVzlIwmYHRlbXBsYXRlZF9zZXR1cGAgaXMgZ2l2aW5nIG1lIGhlbGwuLi6UdWKMBmF1dGhvcpSMGG1hdHJpa2F0ZXIgKEpvZWwgV2F0c29uKZSMC2Rlc2NyaXB0aW9ulIzwcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kulIwEbmFtZZSMB3JvdXRwdXSUjBBsb25nX2Rlc2NyaXB0aW9ulFgaCAAAIyBSZWN1cnNpdmUgT3V0cHV0IFV0aWxpdHkKCiMjIE92ZXJ2aWV3CgpUaGlzIFB5dGhvbiBzY3JpcHQgcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kuCgojIyBSZXF1aXJlbWVudHMKCiogUHl0aG9uIDMuMTAgb3IgaGlnaGVyLAoqIGBiYXRgIChvcHRpb25hbCwgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcpLAoKIyMgSW5zdGFsbGF0aW9uCgojIyMgVXNpbmcgcGlwCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKT24gc29tZSBzeXN0ZW1zLCB5b3UgbWF5IG5lZWQgdG8gcHV0IHRoZSB2ZXJzaW9uIG51bWJlciBvZiBweXRob246CgpgYGBiYXNoCnB5dGhvbjMuMTIgLW0gcGlwIGluc3RhbGwgcm91dHB1dApgYGAKCj4gRm9yIHRoZSBzYWtlIG9mIHNpbXBsaWNpdHksIHdoZW5ldmVyIEkgbWVudGlvbiBgcHl0aG9uYCBpbiB0aGUgZm9sbG93aW5nIHNlY3Rpb25zLCB5b3UgY2FuIHJlcGxhY2UgaXQgd2l0aCBgcHl0aG9uMy54YCB2ZXJzaW9uIGlmIG5lY2Vzc2FyeS4KCiMjIyBGcm9tIHNvdXJjZQoKQ2xvbmUgdGhpcyByZXBvc2l0b3J5LgoKYGBgYmFzaApnaXQgY2xvbmUgaHR0cHM6Ly9naXRodWIuY29tL25hY2lvYm9pL3JvdXRwdXQuZ2l0CmBgYAoKTmF2aWdhdGUgdG8gdGhlIHJlcG9zaXRvcnkgZGlyZWN0b3J5LgoKYGBgYmFzaApjZCByb3V0cHV0CmBgYAoKQW5kIGluc3RhbGwgdGhlIHBhY2thZ2UuCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCAuCmBgYAoKIyMgVXNhZ2UKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQgW29wdGlvbnNdCmBgYAoKT3B0aW9ucwoKKiAtZCwgLS1zdGFydGluZy1kaXJlY3Rvcnk6IERpcmVjdG9yeSB0byBzdGFydCB0aGUgc2VhcmNoIGZyb20gKGRlZmF1bHQ6IGN1cnJlbnQgZGlyZWN0b3J5KS4KKiAtcywgLS1kby1wcmludC1zdHJ1Y3R1cmU6IFByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLgoqIC1lLCAtLWV4dGVuc2lvbnM6IExpc3Qgb2YgZmlsZSBleHRlbnNpb25zIHRvIHNlYXJjaCBmb3IsIGZvcm1hdCBbZXh0MSxleHQyLC4uLl0gKGRlZmF1bHQ6IFtjLGhdKS4KKiAtcCwgLS1kby1wcm90ZWN0LXByaXZhY3k6IEFub255bWl6ZSBmaWxlIHBhdGhzLgoqIC1hLCAtLWFsc28taW5jbHVkZTogTGlzdCBvZiBhZGRpdGlvbmFsIGZpbGVuYW1lcyB0byBpbmNsdWRlLCBmb3JtYXQgW2ZpbGUxLGZpbGUyLC4uLl0uCiogLWksIC0taWdub3JlOiBMaXN0IG9mIGZpbGVuYW1lcyB0byBpZ25vcmUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsZGlyMSxkaXIyLi4uXS4KKiAtbiwgLS1uby1wcmludDogRG9uJ3QgcHJpbnQgdGhlIGZpbGVzLCBqdXN0IHJldHVybiB0aGVtLgoqIC1iLCAtLWRvLXVzZS1iYXQ6IFVzZSBiYXQgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcuCiogLWMsIC0tZG8tY29sb3JzOiBVc2UgZGlmZmVyZW50IGNvbG9ycyBmb3IgZWFjaCBmaWxlIHR5cGUuCiogLWgsIC0taGVscDogU2hvdyBoZWxwIG1lc3NhZ2UgYW5kIGV4aXQuCgojIyBFeGFtcGxlcwoKVG8gcHJpbnQgdGhlIHN0cnVjdHVyZSBvZiBhIGRpcmVjdG9yeToKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQucHkgLWQgL3BhdGgvdG8vZGlyZWN0b3J5IC1zCmBgYAoKVG8gZmluZCBhbmQgcHJpbnQgLnB5IGZpbGVzIGluIHRoZSBjdXJyZW50IGRpcmVjdG9yeSwgdXNpbmcgYmF0IGZvciBoaWdobGlnaHRpbmc6CgpgYGBiYXNoCnB5dGhvbiByb3V0cHV0LnB5IC1lIFtweV0gLWIKYGBgCgojIyBMaWNlbnNlCgpPcGVuLXNvdXJjZSBzb2Z0d2FyZSBsaWNlbnNlZCB1bmRlciBHUEwtMiBsaWNlbnNlLgoKIyMgVjAuOTk3OCByZWxlYXNlZCBvbiAxNnRoLzUvMjAyNApgdGVtcGxhdGVkX3NldHVwYCBpcyBnaXZpbmcgbWUgaGVsbC4uLpSMFmt3YXJnc19mb3Jfc2V0dXBfdG9vbHOUfZR1Lg=="""
```

### Comparing `routput-0.9977/routput.egg-info/PKG-INFO` & `routput-0.9978/routput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9977
+Version: 0.9978
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
 
-## V0.9977 released on 16th/5/2024
+## V0.9978 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.9977/templated_setup.py` & `routput-0.9978/templated_setup.py`

 * *Files identical despite different names*

