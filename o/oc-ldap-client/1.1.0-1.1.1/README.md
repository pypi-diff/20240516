# Comparing `tmp/oc_ldap_client-1.1.0-py3-none-any.whl.zip` & `tmp/oc_ldap_client-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 12441 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-20 09:45 oc_ldap_client/__init__.py
--rw-r--r--  2.0 unx    20363 b- defN 24-Feb-20 09:45 oc_ldap_client/oc_ldap.py
--rw-r--r--  2.0 unx     5798 b- defN 24-Feb-20 09:45 oc_ldap_client/oc_ldap_objects.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Feb-20 09:45 oc_ldap_client-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      258 b- defN 24-Feb-20 09:45 oc_ldap_client-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-20 09:45 oc_ldap_client-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Feb-20 09:45 oc_ldap_client-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      674 b- defN 24-Feb-20 09:45 oc_ldap_client-1.1.0.dist-info/RECORD
-8 files, 38557 bytes uncompressed, 11255 bytes compressed:  70.8%
+Zip file size: 12460 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 15:13 oc_ldap_client/__init__.py
+-rw-r--r--  2.0 unx    20363 b- defN 24-May-16 15:13 oc_ldap_client/oc_ldap.py
+-rw-r--r--  2.0 unx     5896 b- defN 24-May-16 15:13 oc_ldap_client/oc_ldap_objects.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-16 15:13 oc_ldap_client-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      258 b- defN 24-May-16 15:13 oc_ldap_client-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 15:13 oc_ldap_client-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-16 15:13 oc_ldap_client-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      674 b- defN 24-May-16 15:13 oc_ldap_client-1.1.1.dist-info/RECORD
+8 files, 38655 bytes uncompressed, 11274 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: oc_ldap_client/oc_ldap.py
 Comment: 
 
 Filename: oc_ldap_client/oc_ldap_objects.py
 Comment: 
 
-Filename: oc_ldap_client-1.1.0.dist-info/LICENSE
+Filename: oc_ldap_client-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: oc_ldap_client-1.1.0.dist-info/METADATA
+Filename: oc_ldap_client-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: oc_ldap_client-1.1.0.dist-info/WHEEL
+Filename: oc_ldap_client-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: oc_ldap_client-1.1.0.dist-info/top_level.txt
+Filename: oc_ldap_client-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_ldap_client-1.1.0.dist-info/RECORD
+Filename: oc_ldap_client-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oc_ldap_client/oc_ldap_objects.py

```diff
@@ -7,25 +7,27 @@
 
 
 class OcLdapUserCat(OcLdap):
     """
     User catalogue-specific methods
     """
 
-    def __init__(self, url=None, user_cert=None, user_key=None, ca_chain=None, baseDn=None):
+    def __init__(self, url=None, user_cert=None, user_key=None, ca_chain=None, baseDn=None,
+                 user=None, password=None):
         """
         Initialization
         :param str url: OpenLDAP host URI
         :param str user_cert: path to user SSL certificate
         :param str user_key: path to user private key
         :param str ca_chain: path to CA certificates chain
         :param str baseDn: base DN to work with
         """
         super().__init__(url=url, user_cert=user_cert,
-                         user_key=user_key, ca_chain=ca_chain, baseDn=baseDn)
+                         user_key=user_key, ca_chain=ca_chain, baseDn=baseDn,
+                         user=user, password=password)
         self._userObjectClass = 'inetOrgPerson'
         self._groupObjectClass = 'groupOfUniqueNames'
 
     def get_user_by_login(self, login):
         """
         Get catalogue user class instance.
         Gives a class derived from LDAP if exista.
```

## Comparing `oc_ldap_client-1.1.0.dist-info/LICENSE` & `oc_ldap_client-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

