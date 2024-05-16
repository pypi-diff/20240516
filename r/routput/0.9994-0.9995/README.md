# Comparing `tmp/routput-0.9994.tar.gz` & `tmp/routput-0.9995.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.9994.tar", last modified: Thu May 16 14:24:08 2024, max compression
+gzip compressed data, was "routput-0.9995.tar", last modified: Thu May 16 14:35:32 2024, max compression
```

## Comparing `routput-0.9994.tar` & `routput-0.9995.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 14:24:08.702675 routput-0.9994/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9994/LICENCE
--rw-rw-rw-   0        0        0     2597 2024-05-16 14:24:08.701657 routput-0.9994/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9994/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 14:24:08.696563 routput-0.9994/routput/
--rw-rw-rw-   0        0        0     2687 2024-05-16 14:24:08.000000 routput-0.9994/routput/_README.py
--rw-rw-rw-   0        0        0       22 2024-05-16 10:24:13.000000 routput-0.9994/routput/__init__.py
--rw-rw-rw-   0        0        0       31 2024-04-18 09:05:31.000000 routput-0.9994/routput/__main__.py
--rw-rw-rw-   0        0        0     3509 2024-05-16 14:24:08.000000 routput-0.9994/routput/_pickled.py
--rw-rw-rw-   0        0        0     8179 2024-04-18 09:10:57.000000 routput-0.9994/routput/routput.py
--rw-rw-rw-   0        0        0    21749 2024-05-16 14:24:08.000000 routput-0.9994/routput/templated_setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 14:24:08.700636 routput-0.9994/routput.egg-info/
--rw-rw-rw-   0        0        0     2597 2024-05-16 14:24:08.000000 routput-0.9994/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-05-16 14:24:08.000000 routput-0.9994/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 14:24:08.000000 routput-0.9994/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 14:24:08.000000 routput-0.9994/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 14:24:08.702675 routput-0.9994/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 14:23:13.000000 routput-0.9994/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:35:32.915474 routput-0.9995/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9995/LICENCE
+-rw-rw-rw-   0        0        0     2597 2024-05-16 14:35:32.890897 routput-0.9995/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9995/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 14:35:32.915474 routput-0.9995/routput/
+-rw-rw-rw-   0        0        0     2687 2024-05-16 14:35:32.000000 routput-0.9995/routput/_README.py
+-rw-rw-rw-   0        0        0       22 2024-05-16 10:24:13.000000 routput-0.9995/routput/__init__.py
+-rw-rw-rw-   0        0        0       31 2024-04-18 09:05:31.000000 routput-0.9995/routput/__main__.py
+-rw-rw-rw-   0        0        0     3509 2024-05-16 14:35:32.000000 routput-0.9995/routput/_pickled.py
+-rw-rw-rw-   0        0        0     8179 2024-04-18 09:10:57.000000 routput-0.9995/routput/routput.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:35:32.889879 routput-0.9995/routput.egg-info/
+-rw-rw-rw-   0        0        0     2597 2024-05-16 14:35:32.000000 routput-0.9995/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-05-16 14:35:32.000000 routput-0.9995/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:35:32.000000 routput-0.9995/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 14:35:32.000000 routput-0.9995/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:35:32.891973 routput-0.9995/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 14:32:26.000000 routput-0.9995/setup.py
+-rw-rw-rw-   0        0        0    22914 2024-05-16 14:35:32.000000 routput-0.9995/templated_setup.py
```

### Comparing `routput-0.9994/LICENCE` & `routput-0.9995/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.9994/PKG-INFO` & `routput-0.9995/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9994
+Version: 0.9995
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
 
-## V0.9994 released on 16th/5/2024
+## V0.9995 released on 16th/5/2024
 hopefully `templated_setup` works now...
```

### Comparing `routput-0.9994/README.md` & `routput-0.9995/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.9994/routput/_README.py` & `routput-0.9995/routput/_README.py`

 * *Files identical despite different names*

### Comparing `routput-0.9994/routput/_pickled.py` & `routput-0.9995/routput/_pickled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-__INST__ = """gASVLwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTk5NJSMBW5vdGVzlIwoaG9wZWZ1bGx5IGB0ZW1wbGF0ZWRfc2V0dXBgIHdvcmtzIG5vdy4uLpR1YowGYXV0aG9ylIwYbWF0cmlrYXRlciAoSm9lbCBXYXRzb24plIwLZGVzY3JpcHRpb26UjPByZWN1cnNpdmVseSBzZWFyY2hlcyBmb3IgZmlsZXMgYmFzZWQgb24gdGhlaXIgZXh0ZW5zaW9ucyBzdGFydGluZyBmcm9tIGEgc3BlY2lmaWVkIGRpcmVjdG9yeS4gSXQgY2FuIHByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLCBpbmNsdWRlIG9yIGV4Y2x1ZGUgc3BlY2lmaWMgZmlsZXMsIHVzZSBzeW50YXggaGlnaGxpZ2h0aW5nIGZvciBvdXRwdXQsIGFuZCBhbm9ueW1pemUgZmlsZSBwYXRocyBmb3IgcHJpdmFjeS6UjARuYW1llIwHcm91dHB1dJSMEGxvbmdfZGVzY3JpcHRpb26UWBwIAAAjIFJlY3Vyc2l2ZSBPdXRwdXQgVXRpbGl0eQoKIyMgT3ZlcnZpZXcKClRoaXMgUHl0aG9uIHNjcmlwdCByZWN1cnNpdmVseSBzZWFyY2hlcyBmb3IgZmlsZXMgYmFzZWQgb24gdGhlaXIgZXh0ZW5zaW9ucyBzdGFydGluZyBmcm9tIGEgc3BlY2lmaWVkIGRpcmVjdG9yeS4gSXQgY2FuIHByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLCBpbmNsdWRlIG9yIGV4Y2x1ZGUgc3BlY2lmaWMgZmlsZXMsIHVzZSBzeW50YXggaGlnaGxpZ2h0aW5nIGZvciBvdXRwdXQsIGFuZCBhbm9ueW1pemUgZmlsZSBwYXRocyBmb3IgcHJpdmFjeS4KCiMjIFJlcXVpcmVtZW50cwoKKiBQeXRob24gMy4xMCBvciBoaWdoZXIsCiogYGJhdGAgKG9wdGlvbmFsLCBmb3Igc3ludGF4IGhpZ2hsaWdodGluZyksCgojIyBJbnN0YWxsYXRpb24KCiMjIyBVc2luZyBwaXAKCmBgYGJhc2gKcHl0aG9uIC1tIHBpcCBpbnN0YWxsIHJvdXRwdXQKYGBgCgpPbiBzb21lIHN5c3RlbXMsIHlvdSBtYXkgbmVlZCB0byBwdXQgdGhlIHZlcnNpb24gbnVtYmVyIG9mIHB5dGhvbjoKCmBgYGJhc2gKcHl0aG9uMy4xMiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKPiBGb3IgdGhlIHNha2Ugb2Ygc2ltcGxpY2l0eSwgd2hlbmV2ZXIgSSBtZW50aW9uIGBweXRob25gIGluIHRoZSBmb2xsb3dpbmcgc2VjdGlvbnMsIHlvdSBjYW4gcmVwbGFjZSBpdCB3aXRoIGBweXRob24zLnhgIHZlcnNpb24gaWYgbmVjZXNzYXJ5LgoKIyMjIEZyb20gc291cmNlCgpDbG9uZSB0aGlzIHJlcG9zaXRvcnkuCgpgYGBiYXNoCmdpdCBjbG9uZSBodHRwczovL2dpdGh1Yi5jb20vbmFjaW9ib2kvcm91dHB1dC5naXQKYGBgCgpOYXZpZ2F0ZSB0byB0aGUgcmVwb3NpdG9yeSBkaXJlY3RvcnkuCgpgYGBiYXNoCmNkIHJvdXRwdXQKYGBgCgpBbmQgaW5zdGFsbCB0aGUgcGFja2FnZS4KCmBgYGJhc2gKcHl0aG9uIC1tIHBpcCBpbnN0YWxsIC4KYGBgCgojIyBVc2FnZQoKYGBgYmFzaApweXRob24gLW0gcm91dHB1dCBbb3B0aW9uc10KYGBgCgpPcHRpb25zCgoqIC1kLCAtLXN0YXJ0aW5nLWRpcmVjdG9yeTogRGlyZWN0b3J5IHRvIHN0YXJ0IHRoZSBzZWFyY2ggZnJvbSAoZGVmYXVsdDogY3VycmVudCBkaXJlY3RvcnkpLgoqIC1zLCAtLWRvLXByaW50LXN0cnVjdHVyZTogUHJpbnQgdGhlIGRpcmVjdG9yeSBzdHJ1Y3R1cmUuCiogLWUsIC0tZXh0ZW5zaW9uczogTGlzdCBvZiBmaWxlIGV4dGVuc2lvbnMgdG8gc2VhcmNoIGZvciwgZm9ybWF0IFtleHQxLGV4dDIsLi4uXSAoZGVmYXVsdDogW2MsaF0pLgoqIC1wLCAtLWRvLXByb3RlY3QtcHJpdmFjeTogQW5vbnltaXplIGZpbGUgcGF0aHMuCiogLWEsIC0tYWxzby1pbmNsdWRlOiBMaXN0IG9mIGFkZGl0aW9uYWwgZmlsZW5hbWVzIHRvIGluY2x1ZGUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsLi4uXS4KKiAtaSwgLS1pZ25vcmU6IExpc3Qgb2YgZmlsZW5hbWVzIHRvIGlnbm9yZSwgZm9ybWF0IFtmaWxlMSxmaWxlMixkaXIxLGRpcjIuLi5dLgoqIC1uLCAtLW5vLXByaW50OiBEb24ndCBwcmludCB0aGUgZmlsZXMsIGp1c3QgcmV0dXJuIHRoZW0uCiogLWIsIC0tZG8tdXNlLWJhdDogVXNlIGJhdCBmb3Igc3ludGF4IGhpZ2hsaWdodGluZy4KKiAtYywgLS1kby1jb2xvcnM6IFVzZSBkaWZmZXJlbnQgY29sb3JzIGZvciBlYWNoIGZpbGUgdHlwZS4KKiAtaCwgLS1oZWxwOiBTaG93IGhlbHAgbWVzc2FnZSBhbmQgZXhpdC4KCiMjIEV4YW1wbGVzCgpUbyBwcmludCB0aGUgc3RydWN0dXJlIG9mIGEgZGlyZWN0b3J5OgoKYGBgYmFzaApweXRob24gLW0gcm91dHB1dC5weSAtZCAvcGF0aC90by9kaXJlY3RvcnkgLXMKYGBgCgpUbyBmaW5kIGFuZCBwcmludCAucHkgZmlsZXMgaW4gdGhlIGN1cnJlbnQgZGlyZWN0b3J5LCB1c2luZyBiYXQgZm9yIGhpZ2hsaWdodGluZzoKCmBgYGJhc2gKcHl0aG9uIHJvdXRwdXQucHkgLWUgW3B5XSAtYgpgYGAKCiMjIExpY2Vuc2UKCk9wZW4tc291cmNlIHNvZnR3YXJlIGxpY2Vuc2VkIHVuZGVyIEdQTC0yIGxpY2Vuc2UuCgojIyBWMC45OTk0IHJlbGVhc2VkIG9uIDE2dGgvNS8yMDI0CmhvcGVmdWxseSBgdGVtcGxhdGVkX3NldHVwYCB3b3JrcyBub3cuLi6UjBZrd2FyZ3NfZm9yX3NldHVwX3Rvb2xzlH2UdS4="""
+__INST__ = """gASVLwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTk5NZSMBW5vdGVzlIwoaG9wZWZ1bGx5IGB0ZW1wbGF0ZWRfc2V0dXBgIHdvcmtzIG5vdy4uLpR1YowGYXV0aG9ylIwYbWF0cmlrYXRlciAoSm9lbCBXYXRzb24plIwLZGVzY3JpcHRpb26UjPByZWN1cnNpdmVseSBzZWFyY2hlcyBmb3IgZmlsZXMgYmFzZWQgb24gdGhlaXIgZXh0ZW5zaW9ucyBzdGFydGluZyBmcm9tIGEgc3BlY2lmaWVkIGRpcmVjdG9yeS4gSXQgY2FuIHByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLCBpbmNsdWRlIG9yIGV4Y2x1ZGUgc3BlY2lmaWMgZmlsZXMsIHVzZSBzeW50YXggaGlnaGxpZ2h0aW5nIGZvciBvdXRwdXQsIGFuZCBhbm9ueW1pemUgZmlsZSBwYXRocyBmb3IgcHJpdmFjeS6UjARuYW1llIwHcm91dHB1dJSMEGxvbmdfZGVzY3JpcHRpb26UWBwIAAAjIFJlY3Vyc2l2ZSBPdXRwdXQgVXRpbGl0eQoKIyMgT3ZlcnZpZXcKClRoaXMgUHl0aG9uIHNjcmlwdCByZWN1cnNpdmVseSBzZWFyY2hlcyBmb3IgZmlsZXMgYmFzZWQgb24gdGhlaXIgZXh0ZW5zaW9ucyBzdGFydGluZyBmcm9tIGEgc3BlY2lmaWVkIGRpcmVjdG9yeS4gSXQgY2FuIHByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLCBpbmNsdWRlIG9yIGV4Y2x1ZGUgc3BlY2lmaWMgZmlsZXMsIHVzZSBzeW50YXggaGlnaGxpZ2h0aW5nIGZvciBvdXRwdXQsIGFuZCBhbm9ueW1pemUgZmlsZSBwYXRocyBmb3IgcHJpdmFjeS4KCiMjIFJlcXVpcmVtZW50cwoKKiBQeXRob24gMy4xMCBvciBoaWdoZXIsCiogYGJhdGAgKG9wdGlvbmFsLCBmb3Igc3ludGF4IGhpZ2hsaWdodGluZyksCgojIyBJbnN0YWxsYXRpb24KCiMjIyBVc2luZyBwaXAKCmBgYGJhc2gKcHl0aG9uIC1tIHBpcCBpbnN0YWxsIHJvdXRwdXQKYGBgCgpPbiBzb21lIHN5c3RlbXMsIHlvdSBtYXkgbmVlZCB0byBwdXQgdGhlIHZlcnNpb24gbnVtYmVyIG9mIHB5dGhvbjoKCmBgYGJhc2gKcHl0aG9uMy4xMiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKPiBGb3IgdGhlIHNha2Ugb2Ygc2ltcGxpY2l0eSwgd2hlbmV2ZXIgSSBtZW50aW9uIGBweXRob25gIGluIHRoZSBmb2xsb3dpbmcgc2VjdGlvbnMsIHlvdSBjYW4gcmVwbGFjZSBpdCB3aXRoIGBweXRob24zLnhgIHZlcnNpb24gaWYgbmVjZXNzYXJ5LgoKIyMjIEZyb20gc291cmNlCgpDbG9uZSB0aGlzIHJlcG9zaXRvcnkuCgpgYGBiYXNoCmdpdCBjbG9uZSBodHRwczovL2dpdGh1Yi5jb20vbmFjaW9ib2kvcm91dHB1dC5naXQKYGBgCgpOYXZpZ2F0ZSB0byB0aGUgcmVwb3NpdG9yeSBkaXJlY3RvcnkuCgpgYGBiYXNoCmNkIHJvdXRwdXQKYGBgCgpBbmQgaW5zdGFsbCB0aGUgcGFja2FnZS4KCmBgYGJhc2gKcHl0aG9uIC1tIHBpcCBpbnN0YWxsIC4KYGBgCgojIyBVc2FnZQoKYGBgYmFzaApweXRob24gLW0gcm91dHB1dCBbb3B0aW9uc10KYGBgCgpPcHRpb25zCgoqIC1kLCAtLXN0YXJ0aW5nLWRpcmVjdG9yeTogRGlyZWN0b3J5IHRvIHN0YXJ0IHRoZSBzZWFyY2ggZnJvbSAoZGVmYXVsdDogY3VycmVudCBkaXJlY3RvcnkpLgoqIC1zLCAtLWRvLXByaW50LXN0cnVjdHVyZTogUHJpbnQgdGhlIGRpcmVjdG9yeSBzdHJ1Y3R1cmUuCiogLWUsIC0tZXh0ZW5zaW9uczogTGlzdCBvZiBmaWxlIGV4dGVuc2lvbnMgdG8gc2VhcmNoIGZvciwgZm9ybWF0IFtleHQxLGV4dDIsLi4uXSAoZGVmYXVsdDogW2MsaF0pLgoqIC1wLCAtLWRvLXByb3RlY3QtcHJpdmFjeTogQW5vbnltaXplIGZpbGUgcGF0aHMuCiogLWEsIC0tYWxzby1pbmNsdWRlOiBMaXN0IG9mIGFkZGl0aW9uYWwgZmlsZW5hbWVzIHRvIGluY2x1ZGUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsLi4uXS4KKiAtaSwgLS1pZ25vcmU6IExpc3Qgb2YgZmlsZW5hbWVzIHRvIGlnbm9yZSwgZm9ybWF0IFtmaWxlMSxmaWxlMixkaXIxLGRpcjIuLi5dLgoqIC1uLCAtLW5vLXByaW50OiBEb24ndCBwcmludCB0aGUgZmlsZXMsIGp1c3QgcmV0dXJuIHRoZW0uCiogLWIsIC0tZG8tdXNlLWJhdDogVXNlIGJhdCBmb3Igc3ludGF4IGhpZ2hsaWdodGluZy4KKiAtYywgLS1kby1jb2xvcnM6IFVzZSBkaWZmZXJlbnQgY29sb3JzIGZvciBlYWNoIGZpbGUgdHlwZS4KKiAtaCwgLS1oZWxwOiBTaG93IGhlbHAgbWVzc2FnZSBhbmQgZXhpdC4KCiMjIEV4YW1wbGVzCgpUbyBwcmludCB0aGUgc3RydWN0dXJlIG9mIGEgZGlyZWN0b3J5OgoKYGBgYmFzaApweXRob24gLW0gcm91dHB1dC5weSAtZCAvcGF0aC90by9kaXJlY3RvcnkgLXMKYGBgCgpUbyBmaW5kIGFuZCBwcmludCAucHkgZmlsZXMgaW4gdGhlIGN1cnJlbnQgZGlyZWN0b3J5LCB1c2luZyBiYXQgZm9yIGhpZ2hsaWdodGluZzoKCmBgYGJhc2gKcHl0aG9uIHJvdXRwdXQucHkgLWUgW3B5XSAtYgpgYGAKCiMjIExpY2Vuc2UKCk9wZW4tc291cmNlIHNvZnR3YXJlIGxpY2Vuc2VkIHVuZGVyIEdQTC0yIGxpY2Vuc2UuCgojIyBWMC45OTk1IHJlbGVhc2VkIG9uIDE2dGgvNS8yMDI0CmhvcGVmdWxseSBgdGVtcGxhdGVkX3NldHVwYCB3b3JrcyBub3cuLi6UjBZrd2FyZ3NfZm9yX3NldHVwX3Rvb2xzlH2UdS4="""
```

### Comparing `routput-0.9994/routput/routput.py` & `routput-0.9995/routput/routput.py`

 * *Files identical despite different names*

### Comparing `routput-0.9994/routput/templated_setup.py` & `routput-0.9995/templated_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -830,14 +830,57 @@
 
 		os.remove(f"{cls._name}{os.path.sep}_pickled.py")
 		os.remove(f"{cls._name}{os.path.sep}templated_setup.py")
 		os.remove(f"{cls._name}{os.path.sep}_README.py")
 
 		print("\n] Setup complete.\n\n")
 
+		# We must unzip the tar.gz file and conduct post-processing.
+		import tarfile
+		dist_dir = os.path.join(os.getcwd(), "dist")
+		tar_file = None
+		for p, d, f in os.walk(dist_dir):
+			for ff in f:
+				if ff.endswith(f"{cls._version.version_number}.tar.gz"):
+					tar_file = os.path.join(p, ff)
+					break
+			if tar_file:
+				break
+		if not tar_file:
+			raise FileNotFoundError("Could not find the tar.gz file.")
+		with tarfile.open(tar_file, "r:gz") as tar:
+			tar.extractall(dist_dir)
+		os.remove(tar_file)
+		shutil.move(
+			os.path.join(
+				dist_dir,
+				f"{cls._name}-{cls._version.version_number}",
+				f"{cls._name}",
+				f"templated_setup.py"
+			),
+			os.path.join(
+				dist_dir,
+				f"{cls._name}-{cls._version.version_number}",
+				"templated_setup.py"
+			)
+		)
+		# Zip the tar file back up.
+		with tarfile.open(tar_file, "w:gz") as tar:
+			tar.add(
+				os.path.join(
+					dist_dir,
+					f"{cls._name}-{cls._version.version_number}"
+				),
+				f"{cls._name}-{cls._version.version_number}"
+			)
+		# Remove the temp dir.
+		shutil.rmtree(
+			os.path.join(dist_dir, f"{cls._name}-{cls._version.version_number}")
+		)
+
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
 
 		_Setup_Helper.__clear_screen()
 
 		print(f"] Description is readable below...\n{long_description}")
```

### Comparing `routput-0.9994/routput.egg-info/PKG-INFO` & `routput-0.9995/routput.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9994
+Version: 0.9995
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
 
-## V0.9994 released on 16th/5/2024
+## V0.9995 released on 16th/5/2024
 hopefully `templated_setup` works now...
```

