# Comparing `tmp/routput-0.9575.tar.gz` & `tmp/routput-0.9576.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.9575.tar", last modified: Thu May 16 12:33:39 2024, max compression
+gzip compressed data, was "routput-0.9576.tar", last modified: Thu May 16 12:35:40 2024, max compression
```

## Comparing `routput-0.9575.tar` & `routput-0.9576.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:33:39.224485 routput-0.9575/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9575/LICENCE
--rw-rw-rw-   0        0        0     2595 2024-05-16 12:33:39.222956 routput-0.9575/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9575/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:33:39.000000 routput-0.9575/README.py
--rw-rw-rw-   0        0        0     3509 2024-05-16 12:33:39.000000 routput-0.9575/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:33:39.222956 routput-0.9575/routput.egg-info/
--rw-rw-rw-   0        0        0     2595 2024-05-16 12:33:39.000000 routput-0.9575/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 12:33:39.000000 routput-0.9575/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:33:39.000000 routput-0.9575/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 12:33:39.000000 routput-0.9575/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:33:39.225034 routput-0.9575/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:30:36.000000 routput-0.9575/setup.py
--rw-rw-rw-   0        0        0    20783 2024-05-16 12:33:39.000000 routput-0.9575/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:35:40.597461 routput-0.9576/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9576/LICENCE
+-rw-rw-rw-   0        0        0     2595 2024-05-16 12:35:40.597461 routput-0.9576/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9576/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:35:40.000000 routput-0.9576/README.py
+-rw-rw-rw-   0        0        0     3505 2024-05-16 12:35:40.000000 routput-0.9576/pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:35:40.596444 routput-0.9576/routput.egg-info/
+-rw-rw-rw-   0        0        0     2595 2024-05-16 12:35:40.000000 routput-0.9576/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 12:35:40.000000 routput-0.9576/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:35:40.000000 routput-0.9576/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-16 12:35:40.000000 routput-0.9576/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:35:40.597461 routput-0.9576/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:30:36.000000 routput-0.9576/setup.py
+-rw-rw-rw-   0        0        0    20775 2024-05-16 12:35:40.000000 routput-0.9576/templated_setup.py
```

### Comparing `routput-0.9575/LICENCE` & `routput-0.9576/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.9575/PKG-INFO` & `routput-0.9576/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9575
+Version: 0.9576
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
 
-## V0.9575 released on 16th/5/2024
+## V0.9576 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.9575/README.md` & `routput-0.9576/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.9575/README.py` & `routput-0.9576/README.py`

 * *Files identical despite different names*

### Comparing `routput-0.9575/pickled.py` & `routput-0.9576/pickled.py`

 * *Files 24% similar despite different names*

```diff
@@ -1 +1 @@
-__INST__ = """gASVLwoAAAAAAAB9lCiMCF92ZXJzaW9ulIwPdGVtcGxhdGVkX3NldHVwlIwIX1ZlcnNpb26Uk5QpgZR9lCiMBGRhdGWUjAhkYXRldGltZZSMBGRhdGWUk5RDBAfoBRCUhZRSlIwOdmVyc2lvbl9udW1iZXKUjAYwLjk1NzWUjAVub3Rlc5SMJmB0ZW1wbGF0ZWRfc2V0dXBgIGlzIGdpdmluZyBtZSBoZWxsLi4ulHVijAdfYXV0aG9ylIwYbWF0cmlrYXRlciAoSm9lbCBXYXRzb24plIwMX2Rlc2NyaXB0aW9ulIzwcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kulIwFX25hbWWUjAdyb3V0cHV0lIwQbG9uZ19kZXNjcmlwdGlvbpRYGggAACMgUmVjdXJzaXZlIE91dHB1dCBVdGlsaXR5CgojIyBPdmVydmlldwoKVGhpcyBQeXRob24gc2NyaXB0IHJlY3Vyc2l2ZWx5IHNlYXJjaGVzIGZvciBmaWxlcyBiYXNlZCBvbiB0aGVpciBleHRlbnNpb25zIHN0YXJ0aW5nIGZyb20gYSBzcGVjaWZpZWQgZGlyZWN0b3J5LiBJdCBjYW4gcHJpbnQgdGhlIGRpcmVjdG9yeSBzdHJ1Y3R1cmUsIGluY2x1ZGUgb3IgZXhjbHVkZSBzcGVjaWZpYyBmaWxlcywgdXNlIHN5bnRheCBoaWdobGlnaHRpbmcgZm9yIG91dHB1dCwgYW5kIGFub255bWl6ZSBmaWxlIHBhdGhzIGZvciBwcml2YWN5LgoKIyMgUmVxdWlyZW1lbnRzCgoqIFB5dGhvbiAzLjEwIG9yIGhpZ2hlciwKKiBgYmF0YCAob3B0aW9uYWwsIGZvciBzeW50YXggaGlnaGxpZ2h0aW5nKSwKCiMjIEluc3RhbGxhdGlvbgoKIyMjIFVzaW5nIHBpcAoKYGBgYmFzaApweXRob24gLW0gcGlwIGluc3RhbGwgcm91dHB1dApgYGAKCk9uIHNvbWUgc3lzdGVtcywgeW91IG1heSBuZWVkIHRvIHB1dCB0aGUgdmVyc2lvbiBudW1iZXIgb2YgcHl0aG9uOgoKYGBgYmFzaApweXRob24zLjEyIC1tIHBpcCBpbnN0YWxsIHJvdXRwdXQKYGBgCgo+IEZvciB0aGUgc2FrZSBvZiBzaW1wbGljaXR5LCB3aGVuZXZlciBJIG1lbnRpb24gYHB5dGhvbmAgaW4gdGhlIGZvbGxvd2luZyBzZWN0aW9ucywgeW91IGNhbiByZXBsYWNlIGl0IHdpdGggYHB5dGhvbjMueGAgdmVyc2lvbiBpZiBuZWNlc3NhcnkuCgojIyMgRnJvbSBzb3VyY2UKCkNsb25lIHRoaXMgcmVwb3NpdG9yeS4KCmBgYGJhc2gKZ2l0IGNsb25lIGh0dHBzOi8vZ2l0aHViLmNvbS9uYWNpb2JvaS9yb3V0cHV0LmdpdApgYGAKCk5hdmlnYXRlIHRvIHRoZSByZXBvc2l0b3J5IGRpcmVjdG9yeS4KCmBgYGJhc2gKY2Qgcm91dHB1dApgYGAKCkFuZCBpbnN0YWxsIHRoZSBwYWNrYWdlLgoKYGBgYmFzaApweXRob24gLW0gcGlwIGluc3RhbGwgLgpgYGAKCiMjIFVzYWdlCgpgYGBiYXNoCnB5dGhvbiAtbSByb3V0cHV0IFtvcHRpb25zXQpgYGAKCk9wdGlvbnMKCiogLWQsIC0tc3RhcnRpbmctZGlyZWN0b3J5OiBEaXJlY3RvcnkgdG8gc3RhcnQgdGhlIHNlYXJjaCBmcm9tIChkZWZhdWx0OiBjdXJyZW50IGRpcmVjdG9yeSkuCiogLXMsIC0tZG8tcHJpbnQtc3RydWN0dXJlOiBQcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZS4KKiAtZSwgLS1leHRlbnNpb25zOiBMaXN0IG9mIGZpbGUgZXh0ZW5zaW9ucyB0byBzZWFyY2ggZm9yLCBmb3JtYXQgW2V4dDEsZXh0MiwuLi5dIChkZWZhdWx0OiBbYyxoXSkuCiogLXAsIC0tZG8tcHJvdGVjdC1wcml2YWN5OiBBbm9ueW1pemUgZmlsZSBwYXRocy4KKiAtYSwgLS1hbHNvLWluY2x1ZGU6IExpc3Qgb2YgYWRkaXRpb25hbCBmaWxlbmFtZXMgdG8gaW5jbHVkZSwgZm9ybWF0IFtmaWxlMSxmaWxlMiwuLi5dLgoqIC1pLCAtLWlnbm9yZTogTGlzdCBvZiBmaWxlbmFtZXMgdG8gaWdub3JlLCBmb3JtYXQgW2ZpbGUxLGZpbGUyLGRpcjEsZGlyMi4uLl0uCiogLW4sIC0tbm8tcHJpbnQ6IERvbid0IHByaW50IHRoZSBmaWxlcywganVzdCByZXR1cm4gdGhlbS4KKiAtYiwgLS1kby11c2UtYmF0OiBVc2UgYmF0IGZvciBzeW50YXggaGlnaGxpZ2h0aW5nLgoqIC1jLCAtLWRvLWNvbG9yczogVXNlIGRpZmZlcmVudCBjb2xvcnMgZm9yIGVhY2ggZmlsZSB0eXBlLgoqIC1oLCAtLWhlbHA6IFNob3cgaGVscCBtZXNzYWdlIGFuZCBleGl0LgoKIyMgRXhhbXBsZXMKClRvIHByaW50IHRoZSBzdHJ1Y3R1cmUgb2YgYSBkaXJlY3Rvcnk6CgpgYGBiYXNoCnB5dGhvbiAtbSByb3V0cHV0LnB5IC1kIC9wYXRoL3RvL2RpcmVjdG9yeSAtcwpgYGAKClRvIGZpbmQgYW5kIHByaW50IC5weSBmaWxlcyBpbiB0aGUgY3VycmVudCBkaXJlY3RvcnksIHVzaW5nIGJhdCBmb3IgaGlnaGxpZ2h0aW5nOgoKYGBgYmFzaApweXRob24gcm91dHB1dC5weSAtZSBbcHldIC1iCmBgYAoKIyMgTGljZW5zZQoKT3Blbi1zb3VyY2Ugc29mdHdhcmUgbGljZW5zZWQgdW5kZXIgR1BMLTIgbGljZW5zZS4KCiMjIFYwLjk1NzUgcmVsZWFzZWQgb24gMTZ0aC81LzIwMjQKYHRlbXBsYXRlZF9zZXR1cGAgaXMgZ2l2aW5nIG1lIGhlbGwuLi6UjBZrd2FyZ3NfZm9yX3NldHVwX3Rvb2xzlH2UdS4="""
+__INST__ = """gASVKwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTU3NpSMBW5vdGVzlIwmYHRlbXBsYXRlZF9zZXR1cGAgaXMgZ2l2aW5nIG1lIGhlbGwuLi6UdWKMBmF1dGhvcpSMGG1hdHJpa2F0ZXIgKEpvZWwgV2F0c29uKZSMC2Rlc2NyaXB0aW9ulIzwcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kulIwEbmFtZZSMB3JvdXRwdXSUjBBsb25nX2Rlc2NyaXB0aW9ulFgaCAAAIyBSZWN1cnNpdmUgT3V0cHV0IFV0aWxpdHkKCiMjIE92ZXJ2aWV3CgpUaGlzIFB5dGhvbiBzY3JpcHQgcmVjdXJzaXZlbHkgc2VhcmNoZXMgZm9yIGZpbGVzIGJhc2VkIG9uIHRoZWlyIGV4dGVuc2lvbnMgc3RhcnRpbmcgZnJvbSBhIHNwZWNpZmllZCBkaXJlY3RvcnkuIEl0IGNhbiBwcmludCB0aGUgZGlyZWN0b3J5IHN0cnVjdHVyZSwgaW5jbHVkZSBvciBleGNsdWRlIHNwZWNpZmljIGZpbGVzLCB1c2Ugc3ludGF4IGhpZ2hsaWdodGluZyBmb3Igb3V0cHV0LCBhbmQgYW5vbnltaXplIGZpbGUgcGF0aHMgZm9yIHByaXZhY3kuCgojIyBSZXF1aXJlbWVudHMKCiogUHl0aG9uIDMuMTAgb3IgaGlnaGVyLAoqIGBiYXRgIChvcHRpb25hbCwgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcpLAoKIyMgSW5zdGFsbGF0aW9uCgojIyMgVXNpbmcgcGlwCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKT24gc29tZSBzeXN0ZW1zLCB5b3UgbWF5IG5lZWQgdG8gcHV0IHRoZSB2ZXJzaW9uIG51bWJlciBvZiBweXRob246CgpgYGBiYXNoCnB5dGhvbjMuMTIgLW0gcGlwIGluc3RhbGwgcm91dHB1dApgYGAKCj4gRm9yIHRoZSBzYWtlIG9mIHNpbXBsaWNpdHksIHdoZW5ldmVyIEkgbWVudGlvbiBgcHl0aG9uYCBpbiB0aGUgZm9sbG93aW5nIHNlY3Rpb25zLCB5b3UgY2FuIHJlcGxhY2UgaXQgd2l0aCBgcHl0aG9uMy54YCB2ZXJzaW9uIGlmIG5lY2Vzc2FyeS4KCiMjIyBGcm9tIHNvdXJjZQoKQ2xvbmUgdGhpcyByZXBvc2l0b3J5LgoKYGBgYmFzaApnaXQgY2xvbmUgaHR0cHM6Ly9naXRodWIuY29tL25hY2lvYm9pL3JvdXRwdXQuZ2l0CmBgYAoKTmF2aWdhdGUgdG8gdGhlIHJlcG9zaXRvcnkgZGlyZWN0b3J5LgoKYGBgYmFzaApjZCByb3V0cHV0CmBgYAoKQW5kIGluc3RhbGwgdGhlIHBhY2thZ2UuCgpgYGBiYXNoCnB5dGhvbiAtbSBwaXAgaW5zdGFsbCAuCmBgYAoKIyMgVXNhZ2UKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQgW29wdGlvbnNdCmBgYAoKT3B0aW9ucwoKKiAtZCwgLS1zdGFydGluZy1kaXJlY3Rvcnk6IERpcmVjdG9yeSB0byBzdGFydCB0aGUgc2VhcmNoIGZyb20gKGRlZmF1bHQ6IGN1cnJlbnQgZGlyZWN0b3J5KS4KKiAtcywgLS1kby1wcmludC1zdHJ1Y3R1cmU6IFByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLgoqIC1lLCAtLWV4dGVuc2lvbnM6IExpc3Qgb2YgZmlsZSBleHRlbnNpb25zIHRvIHNlYXJjaCBmb3IsIGZvcm1hdCBbZXh0MSxleHQyLC4uLl0gKGRlZmF1bHQ6IFtjLGhdKS4KKiAtcCwgLS1kby1wcm90ZWN0LXByaXZhY3k6IEFub255bWl6ZSBmaWxlIHBhdGhzLgoqIC1hLCAtLWFsc28taW5jbHVkZTogTGlzdCBvZiBhZGRpdGlvbmFsIGZpbGVuYW1lcyB0byBpbmNsdWRlLCBmb3JtYXQgW2ZpbGUxLGZpbGUyLC4uLl0uCiogLWksIC0taWdub3JlOiBMaXN0IG9mIGZpbGVuYW1lcyB0byBpZ25vcmUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsZGlyMSxkaXIyLi4uXS4KKiAtbiwgLS1uby1wcmludDogRG9uJ3QgcHJpbnQgdGhlIGZpbGVzLCBqdXN0IHJldHVybiB0aGVtLgoqIC1iLCAtLWRvLXVzZS1iYXQ6IFVzZSBiYXQgZm9yIHN5bnRheCBoaWdobGlnaHRpbmcuCiogLWMsIC0tZG8tY29sb3JzOiBVc2UgZGlmZmVyZW50IGNvbG9ycyBmb3IgZWFjaCBmaWxlIHR5cGUuCiogLWgsIC0taGVscDogU2hvdyBoZWxwIG1lc3NhZ2UgYW5kIGV4aXQuCgojIyBFeGFtcGxlcwoKVG8gcHJpbnQgdGhlIHN0cnVjdHVyZSBvZiBhIGRpcmVjdG9yeToKCmBgYGJhc2gKcHl0aG9uIC1tIHJvdXRwdXQucHkgLWQgL3BhdGgvdG8vZGlyZWN0b3J5IC1zCmBgYAoKVG8gZmluZCBhbmQgcHJpbnQgLnB5IGZpbGVzIGluIHRoZSBjdXJyZW50IGRpcmVjdG9yeSwgdXNpbmcgYmF0IGZvciBoaWdobGlnaHRpbmc6CgpgYGBiYXNoCnB5dGhvbiByb3V0cHV0LnB5IC1lIFtweV0gLWIKYGBgCgojIyBMaWNlbnNlCgpPcGVuLXNvdXJjZSBzb2Z0d2FyZSBsaWNlbnNlZCB1bmRlciBHUEwtMiBsaWNlbnNlLgoKIyMgVjAuOTU3NiByZWxlYXNlZCBvbiAxNnRoLzUvMjAyNApgdGVtcGxhdGVkX3NldHVwYCBpcyBnaXZpbmcgbWUgaGVsbC4uLpSMFmt3YXJnc19mb3Jfc2V0dXBfdG9vbHOUfZR1Lg=="""
```

### Comparing `routput-0.9575/routput.egg-info/PKG-INFO` & `routput-0.9576/routput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9575
+Version: 0.9576
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
 
-## V0.9575 released on 16th/5/2024
+## V0.9576 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.9575/templated_setup.py` & `routput-0.9576/templated_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -672,19 +672,19 @@
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
 		import pickled
 		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
-		version = c["_version"]
-		author = c["_author"]
-		description = c["_description"]
+		version = c["version"]
+		author = c["author"]
+		description = c["description"]
 		long_description = c["long_description"]
-		kwargs_for_setup_tools = c["_kwargs_for_setup_tools"]
+		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
 			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
@@ -767,18 +767,18 @@
 		assert cls._author is not None
 		assert cls._description is not None
 		assert cls._name is not None
 		assert cls._long_description is not None
 		with open("pickled.py", "w") as f:
 			f.write("__INST__ = \"\"\"")
 			f.write(base64_x_b64encode(pickle_x_dumps({
-				"_version": cls._version,
-				"_author": cls._author,
-				"_description": cls._description,
-				"_name": cls._name,
+				"version": cls._version,
+				"author": cls._author,
+				"description": cls._description,
+				"name": cls._name,
 				"long_description": cls._long_description,
 				"kwargs_for_setup_tools": kwargs_for_setup_tools,
 			})).decode())
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
```

