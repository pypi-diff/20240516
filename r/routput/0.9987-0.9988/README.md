# Comparing `tmp/routput-0.9987.tar.gz` & `tmp/routput-0.9988.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.9987.tar", last modified: Thu May 16 13:34:00 2024, max compression
+gzip compressed data, was "routput-0.9988.tar", last modified: Thu May 16 13:36:29 2024, max compression
```

## Comparing `routput-0.9987.tar` & `routput-0.9988.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:34:00.005713 routput-0.9987/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9987/LICENCE
--rw-rw-rw-   0        0        0     2597 2024-05-16 13:34:00.004181 routput-0.9987/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9987/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 13:33:59.000000 routput-0.9987/_README.py
--rw-rw-rw-   0        0        0     3509 2024-05-16 13:33:59.000000 routput-0.9987/_pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:34:00.002608 routput-0.9987/routput.egg-info/
--rw-rw-rw-   0        0        0     2597 2024-05-16 13:33:59.000000 routput-0.9987/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-16 13:33:59.000000 routput-0.9987/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:33:59.000000 routput-0.9987/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-16 13:33:59.000000 routput-0.9987/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 13:34:00.005713 routput-0.9987/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 13:33:16.000000 routput-0.9987/setup.py
--rw-rw-rw-   0        0        0    21307 2024-05-16 13:33:59.000000 routput-0.9987/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:36:29.716961 routput-0.9988/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9988/LICENCE
+-rw-rw-rw-   0        0        0     2597 2024-05-16 13:36:29.715941 routput-0.9988/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9988/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 13:36:29.000000 routput-0.9988/_README.py
+-rw-rw-rw-   0        0        0     3509 2024-05-16 13:36:29.000000 routput-0.9988/_pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:36:29.714923 routput-0.9988/routput.egg-info/
+-rw-rw-rw-   0        0        0     2597 2024-05-16 13:36:29.000000 routput-0.9988/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-16 13:36:29.000000 routput-0.9988/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:36:29.000000 routput-0.9988/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-16 13:36:29.000000 routput-0.9988/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:36:29.716961 routput-0.9988/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 13:35:56.000000 routput-0.9988/setup.py
+-rw-rw-rw-   0        0        0    21277 2024-05-16 13:36:29.000000 routput-0.9988/templated_setup.py
```

### Comparing `routput-0.9987/LICENCE` & `routput-0.9988/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.9987/PKG-INFO` & `routput-0.9988/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9987
+Version: 0.9988
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
 
-## V0.9987 released on 16th/5/2024
+## V0.9988 released on 16th/5/2024
 hopefully `templated_setup` works now...
```

### Comparing `routput-0.9987/README.md` & `routput-0.9988/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.9987/_README.py` & `routput-0.9988/_README.py`

 * *Files identical despite different names*

### Comparing `routput-0.9987/_pickled.py` & `routput-0.9988/_pickled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-__INST__ = """gASVLwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTk4N5SMBW5vdGVzlIwoaG9wZWZ1bGx5IGB0ZW1wbGF0ZWRfc2V0dXBgIHdvcmtzIG5vdy4uLpR1YowGYXV0aG9ylIwYbWF0cmlrYXRlciAoSm9lbCBXYXRzb24plIwLZGVzY3JpcHRpb26UjPByZWN1cnNpdmVseSBzZWFyY2hlcyBmb3IgZmlsZXMgYmFzZWQgb24gdGhlaXIgZXh0ZW5zaW9ucyBzdGFydGluZyBmcm9tIGEgc3BlY2lmaWVkIGRpcmVjdG9yeS4gSXQgY2FuIHByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLCBpbmNsdWRlIG9yIGV4Y2x1ZGUgc3BlY2lmaWMgZmlsZXMsIHVzZSBzeW50YXggaGlnaGxpZ2h0aW5nIGZvciBvdXRwdXQsIGFuZCBhbm9ueW1pemUgZmlsZSBwYXRocyBmb3IgcHJpdmFjeS6UjARuYW1llIwHcm91dHB1dJSMEGxvbmdfZGVzY3JpcHRpb26UWBwIAAAjIFJlY3Vyc2l2ZSBPdXRwdXQgVXRpbGl0eQoKIyMgT3ZlcnZpZXcKClRoaXMgUHl0aG9uIHNjcmlwdCByZWN1cnNpdmVseSBzZWFyY2hlcyBmb3IgZmlsZXMgYmFzZWQgb24gdGhlaXIgZXh0ZW5zaW9ucyBzdGFydGluZyBmcm9tIGEgc3BlY2lmaWVkIGRpcmVjdG9yeS4gSXQgY2FuIHByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLCBpbmNsdWRlIG9yIGV4Y2x1ZGUgc3BlY2lmaWMgZmlsZXMsIHVzZSBzeW50YXggaGlnaGxpZ2h0aW5nIGZvciBvdXRwdXQsIGFuZCBhbm9ueW1pemUgZmlsZSBwYXRocyBmb3IgcHJpdmFjeS4KCiMjIFJlcXVpcmVtZW50cwoKKiBQeXRob24gMy4xMCBvciBoaWdoZXIsCiogYGJhdGAgKG9wdGlvbmFsLCBmb3Igc3ludGF4IGhpZ2hsaWdodGluZyksCgojIyBJbnN0YWxsYXRpb24KCiMjIyBVc2luZyBwaXAKCmBgYGJhc2gKcHl0aG9uIC1tIHBpcCBpbnN0YWxsIHJvdXRwdXQKYGBgCgpPbiBzb21lIHN5c3RlbXMsIHlvdSBtYXkgbmVlZCB0byBwdXQgdGhlIHZlcnNpb24gbnVtYmVyIG9mIHB5dGhvbjoKCmBgYGJhc2gKcHl0aG9uMy4xMiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKPiBGb3IgdGhlIHNha2Ugb2Ygc2ltcGxpY2l0eSwgd2hlbmV2ZXIgSSBtZW50aW9uIGBweXRob25gIGluIHRoZSBmb2xsb3dpbmcgc2VjdGlvbnMsIHlvdSBjYW4gcmVwbGFjZSBpdCB3aXRoIGBweXRob24zLnhgIHZlcnNpb24gaWYgbmVjZXNzYXJ5LgoKIyMjIEZyb20gc291cmNlCgpDbG9uZSB0aGlzIHJlcG9zaXRvcnkuCgpgYGBiYXNoCmdpdCBjbG9uZSBodHRwczovL2dpdGh1Yi5jb20vbmFjaW9ib2kvcm91dHB1dC5naXQKYGBgCgpOYXZpZ2F0ZSB0byB0aGUgcmVwb3NpdG9yeSBkaXJlY3RvcnkuCgpgYGBiYXNoCmNkIHJvdXRwdXQKYGBgCgpBbmQgaW5zdGFsbCB0aGUgcGFja2FnZS4KCmBgYGJhc2gKcHl0aG9uIC1tIHBpcCBpbnN0YWxsIC4KYGBgCgojIyBVc2FnZQoKYGBgYmFzaApweXRob24gLW0gcm91dHB1dCBbb3B0aW9uc10KYGBgCgpPcHRpb25zCgoqIC1kLCAtLXN0YXJ0aW5nLWRpcmVjdG9yeTogRGlyZWN0b3J5IHRvIHN0YXJ0IHRoZSBzZWFyY2ggZnJvbSAoZGVmYXVsdDogY3VycmVudCBkaXJlY3RvcnkpLgoqIC1zLCAtLWRvLXByaW50LXN0cnVjdHVyZTogUHJpbnQgdGhlIGRpcmVjdG9yeSBzdHJ1Y3R1cmUuCiogLWUsIC0tZXh0ZW5zaW9uczogTGlzdCBvZiBmaWxlIGV4dGVuc2lvbnMgdG8gc2VhcmNoIGZvciwgZm9ybWF0IFtleHQxLGV4dDIsLi4uXSAoZGVmYXVsdDogW2MsaF0pLgoqIC1wLCAtLWRvLXByb3RlY3QtcHJpdmFjeTogQW5vbnltaXplIGZpbGUgcGF0aHMuCiogLWEsIC0tYWxzby1pbmNsdWRlOiBMaXN0IG9mIGFkZGl0aW9uYWwgZmlsZW5hbWVzIHRvIGluY2x1ZGUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsLi4uXS4KKiAtaSwgLS1pZ25vcmU6IExpc3Qgb2YgZmlsZW5hbWVzIHRvIGlnbm9yZSwgZm9ybWF0IFtmaWxlMSxmaWxlMixkaXIxLGRpcjIuLi5dLgoqIC1uLCAtLW5vLXByaW50OiBEb24ndCBwcmludCB0aGUgZmlsZXMsIGp1c3QgcmV0dXJuIHRoZW0uCiogLWIsIC0tZG8tdXNlLWJhdDogVXNlIGJhdCBmb3Igc3ludGF4IGhpZ2hsaWdodGluZy4KKiAtYywgLS1kby1jb2xvcnM6IFVzZSBkaWZmZXJlbnQgY29sb3JzIGZvciBlYWNoIGZpbGUgdHlwZS4KKiAtaCwgLS1oZWxwOiBTaG93IGhlbHAgbWVzc2FnZSBhbmQgZXhpdC4KCiMjIEV4YW1wbGVzCgpUbyBwcmludCB0aGUgc3RydWN0dXJlIG9mIGEgZGlyZWN0b3J5OgoKYGBgYmFzaApweXRob24gLW0gcm91dHB1dC5weSAtZCAvcGF0aC90by9kaXJlY3RvcnkgLXMKYGBgCgpUbyBmaW5kIGFuZCBwcmludCAucHkgZmlsZXMgaW4gdGhlIGN1cnJlbnQgZGlyZWN0b3J5LCB1c2luZyBiYXQgZm9yIGhpZ2hsaWdodGluZzoKCmBgYGJhc2gKcHl0aG9uIHJvdXRwdXQucHkgLWUgW3B5XSAtYgpgYGAKCiMjIExpY2Vuc2UKCk9wZW4tc291cmNlIHNvZnR3YXJlIGxpY2Vuc2VkIHVuZGVyIEdQTC0yIGxpY2Vuc2UuCgojIyBWMC45OTg3IHJlbGVhc2VkIG9uIDE2dGgvNS8yMDI0CmhvcGVmdWxseSBgdGVtcGxhdGVkX3NldHVwYCB3b3JrcyBub3cuLi6UjBZrd2FyZ3NfZm9yX3NldHVwX3Rvb2xzlH2UdS4="""
+__INST__ = """gASVLwoAAAAAAAB9lCiMB3ZlcnNpb26UjA90ZW1wbGF0ZWRfc2V0dXCUjAhfVmVyc2lvbpSTlCmBlH2UKIwEZGF0ZZSMCGRhdGV0aW1llIwEZGF0ZZSTlEMEB+gFEJSFlFKUjA52ZXJzaW9uX251bWJlcpSMBjAuOTk4OJSMBW5vdGVzlIwoaG9wZWZ1bGx5IGB0ZW1wbGF0ZWRfc2V0dXBgIHdvcmtzIG5vdy4uLpR1YowGYXV0aG9ylIwYbWF0cmlrYXRlciAoSm9lbCBXYXRzb24plIwLZGVzY3JpcHRpb26UjPByZWN1cnNpdmVseSBzZWFyY2hlcyBmb3IgZmlsZXMgYmFzZWQgb24gdGhlaXIgZXh0ZW5zaW9ucyBzdGFydGluZyBmcm9tIGEgc3BlY2lmaWVkIGRpcmVjdG9yeS4gSXQgY2FuIHByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLCBpbmNsdWRlIG9yIGV4Y2x1ZGUgc3BlY2lmaWMgZmlsZXMsIHVzZSBzeW50YXggaGlnaGxpZ2h0aW5nIGZvciBvdXRwdXQsIGFuZCBhbm9ueW1pemUgZmlsZSBwYXRocyBmb3IgcHJpdmFjeS6UjARuYW1llIwHcm91dHB1dJSMEGxvbmdfZGVzY3JpcHRpb26UWBwIAAAjIFJlY3Vyc2l2ZSBPdXRwdXQgVXRpbGl0eQoKIyMgT3ZlcnZpZXcKClRoaXMgUHl0aG9uIHNjcmlwdCByZWN1cnNpdmVseSBzZWFyY2hlcyBmb3IgZmlsZXMgYmFzZWQgb24gdGhlaXIgZXh0ZW5zaW9ucyBzdGFydGluZyBmcm9tIGEgc3BlY2lmaWVkIGRpcmVjdG9yeS4gSXQgY2FuIHByaW50IHRoZSBkaXJlY3Rvcnkgc3RydWN0dXJlLCBpbmNsdWRlIG9yIGV4Y2x1ZGUgc3BlY2lmaWMgZmlsZXMsIHVzZSBzeW50YXggaGlnaGxpZ2h0aW5nIGZvciBvdXRwdXQsIGFuZCBhbm9ueW1pemUgZmlsZSBwYXRocyBmb3IgcHJpdmFjeS4KCiMjIFJlcXVpcmVtZW50cwoKKiBQeXRob24gMy4xMCBvciBoaWdoZXIsCiogYGJhdGAgKG9wdGlvbmFsLCBmb3Igc3ludGF4IGhpZ2hsaWdodGluZyksCgojIyBJbnN0YWxsYXRpb24KCiMjIyBVc2luZyBwaXAKCmBgYGJhc2gKcHl0aG9uIC1tIHBpcCBpbnN0YWxsIHJvdXRwdXQKYGBgCgpPbiBzb21lIHN5c3RlbXMsIHlvdSBtYXkgbmVlZCB0byBwdXQgdGhlIHZlcnNpb24gbnVtYmVyIG9mIHB5dGhvbjoKCmBgYGJhc2gKcHl0aG9uMy4xMiAtbSBwaXAgaW5zdGFsbCByb3V0cHV0CmBgYAoKPiBGb3IgdGhlIHNha2Ugb2Ygc2ltcGxpY2l0eSwgd2hlbmV2ZXIgSSBtZW50aW9uIGBweXRob25gIGluIHRoZSBmb2xsb3dpbmcgc2VjdGlvbnMsIHlvdSBjYW4gcmVwbGFjZSBpdCB3aXRoIGBweXRob24zLnhgIHZlcnNpb24gaWYgbmVjZXNzYXJ5LgoKIyMjIEZyb20gc291cmNlCgpDbG9uZSB0aGlzIHJlcG9zaXRvcnkuCgpgYGBiYXNoCmdpdCBjbG9uZSBodHRwczovL2dpdGh1Yi5jb20vbmFjaW9ib2kvcm91dHB1dC5naXQKYGBgCgpOYXZpZ2F0ZSB0byB0aGUgcmVwb3NpdG9yeSBkaXJlY3RvcnkuCgpgYGBiYXNoCmNkIHJvdXRwdXQKYGBgCgpBbmQgaW5zdGFsbCB0aGUgcGFja2FnZS4KCmBgYGJhc2gKcHl0aG9uIC1tIHBpcCBpbnN0YWxsIC4KYGBgCgojIyBVc2FnZQoKYGBgYmFzaApweXRob24gLW0gcm91dHB1dCBbb3B0aW9uc10KYGBgCgpPcHRpb25zCgoqIC1kLCAtLXN0YXJ0aW5nLWRpcmVjdG9yeTogRGlyZWN0b3J5IHRvIHN0YXJ0IHRoZSBzZWFyY2ggZnJvbSAoZGVmYXVsdDogY3VycmVudCBkaXJlY3RvcnkpLgoqIC1zLCAtLWRvLXByaW50LXN0cnVjdHVyZTogUHJpbnQgdGhlIGRpcmVjdG9yeSBzdHJ1Y3R1cmUuCiogLWUsIC0tZXh0ZW5zaW9uczogTGlzdCBvZiBmaWxlIGV4dGVuc2lvbnMgdG8gc2VhcmNoIGZvciwgZm9ybWF0IFtleHQxLGV4dDIsLi4uXSAoZGVmYXVsdDogW2MsaF0pLgoqIC1wLCAtLWRvLXByb3RlY3QtcHJpdmFjeTogQW5vbnltaXplIGZpbGUgcGF0aHMuCiogLWEsIC0tYWxzby1pbmNsdWRlOiBMaXN0IG9mIGFkZGl0aW9uYWwgZmlsZW5hbWVzIHRvIGluY2x1ZGUsIGZvcm1hdCBbZmlsZTEsZmlsZTIsLi4uXS4KKiAtaSwgLS1pZ25vcmU6IExpc3Qgb2YgZmlsZW5hbWVzIHRvIGlnbm9yZSwgZm9ybWF0IFtmaWxlMSxmaWxlMixkaXIxLGRpcjIuLi5dLgoqIC1uLCAtLW5vLXByaW50OiBEb24ndCBwcmludCB0aGUgZmlsZXMsIGp1c3QgcmV0dXJuIHRoZW0uCiogLWIsIC0tZG8tdXNlLWJhdDogVXNlIGJhdCBmb3Igc3ludGF4IGhpZ2hsaWdodGluZy4KKiAtYywgLS1kby1jb2xvcnM6IFVzZSBkaWZmZXJlbnQgY29sb3JzIGZvciBlYWNoIGZpbGUgdHlwZS4KKiAtaCwgLS1oZWxwOiBTaG93IGhlbHAgbWVzc2FnZSBhbmQgZXhpdC4KCiMjIEV4YW1wbGVzCgpUbyBwcmludCB0aGUgc3RydWN0dXJlIG9mIGEgZGlyZWN0b3J5OgoKYGBgYmFzaApweXRob24gLW0gcm91dHB1dC5weSAtZCAvcGF0aC90by9kaXJlY3RvcnkgLXMKYGBgCgpUbyBmaW5kIGFuZCBwcmludCAucHkgZmlsZXMgaW4gdGhlIGN1cnJlbnQgZGlyZWN0b3J5LCB1c2luZyBiYXQgZm9yIGhpZ2hsaWdodGluZzoKCmBgYGJhc2gKcHl0aG9uIHJvdXRwdXQucHkgLWUgW3B5XSAtYgpgYGAKCiMjIExpY2Vuc2UKCk9wZW4tc291cmNlIHNvZnR3YXJlIGxpY2Vuc2VkIHVuZGVyIEdQTC0yIGxpY2Vuc2UuCgojIyBWMC45OTg4IHJlbGVhc2VkIG9uIDE2dGgvNS8yMDI0CmhvcGVmdWxseSBgdGVtcGxhdGVkX3NldHVwYCB3b3JrcyBub3cuLi6UjBZrd2FyZ3NfZm9yX3NldHVwX3Rvb2xzlH2UdS4="""
```

### Comparing `routput-0.9987/routput.egg-info/PKG-INFO` & `routput-0.9988/routput.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9987
+Version: 0.9988
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
 
-## V0.9987 released on 16th/5/2024
+## V0.9988 released on 16th/5/2024
 hopefully `templated_setup` works now...
```

### Comparing `routput-0.9987/templated_setup.py` & `routput-0.9988/templated_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,24 +685,24 @@
 			kwargs_for_setup_tools["py_modules"] = []
 		if not kwargs_for_setup_tools.get("packages"):
 			kwargs_for_setup_tools["packages"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 		kwargs_for_setup_tools["py_modules"].append("pickled")
 		kwargs_for_setup_tools["py_modules"].append("README")
 		kwargs_for_setup_tools["py_modules"].append(name)
-		kwargs_for_setup_tools["packages"].append(name)
 
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
 			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
+			provides=[name],
 			**kwargs_for_setup_tools
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
```

