# Comparing `tmp/pedil-0.1.0.tar.gz` & `tmp/pedil-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedil-0.1.0.tar", last modified: Tue May 14 19:13:40 2024, max compression
+gzip compressed data, was "pedil-0.1.1.tar", last modified: Wed May 15 22:15:52 2024, max compression
```

## Comparing `pedil-0.1.0.tar` & `pedil-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 19:13:40.675848 pedil-0.1.0/
--rw-rw-rw-   0        0        0     3499 2024-05-14 19:13:40.674844 pedil-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 19:13:40.647843 pedil-0.1.0/pedil/
--rw-rw-rw-   0        0        0        0 2024-05-14 19:13:12.000000 pedil-0.1.0/pedil/__init__.py
--rw-rw-rw-   0        0        0     3263 2024-05-14 19:04:05.000000 pedil-0.1.0/pedil/pedil.py
-drwxrwxrwx   0        0        0        0 2024-05-14 19:13:40.673844 pedil-0.1.0/pedil.egg-info/
--rw-rw-rw-   0        0        0     3499 2024-05-14 19:13:40.000000 pedil-0.1.0/pedil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-14 19:13:40.000000 pedil-0.1.0/pedil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 19:13:40.000000 pedil-0.1.0/pedil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 19:13:40.000000 pedil-0.1.0/pedil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 19:13:40.000000 pedil-0.1.0/pedil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 19:13:40.675848 pedil-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      796 2024-05-14 18:46:48.000000 pedil-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:15:52.376117 pedil-0.1.1/
+-rw-rw-rw-   0        0        0     3809 2024-05-15 22:15:52.374988 pedil-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 22:15:52.356237 pedil-0.1.1/pedil/
+-rw-rw-rw-   0        0        0        0 2024-05-14 19:13:12.000000 pedil-0.1.1/pedil/__init__.py
+-rw-rw-rw-   0        0        0     3683 2024-05-15 22:05:35.000000 pedil-0.1.1/pedil/pedil.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:15:52.363237 pedil-0.1.1/pedil.egg-info/
+-rw-rw-rw-   0        0        0     3809 2024-05-15 22:15:52.000000 pedil-0.1.1/pedil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-15 22:15:52.000000 pedil-0.1.1/pedil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:15:52.000000 pedil-0.1.1/pedil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 22:15:52.000000 pedil-0.1.1/pedil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 22:15:52.000000 pedil-0.1.1/pedil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:15:52.376117 pedil-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-15 22:10:38.000000 pedil-0.1.1/setup.py
```

### Comparing `pedil-0.1.0/PKG-INFO` & `pedil-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pedil
-Version: 0.1.0
-Summary: A Python package for generating unique IDs using the Prime Extended Decimal Index Listing (PEDIL) method.
-Home-page: https://github.com/IreGaddr/pedil
-Author: Your Name
-Author-email: your.email@example.com
+Version: 0.1.1
+Summary: A Python package for generating unique and secure IDs using Prime Extended Decimal Index Listing (PEDIL).
+Home-page: https://github.com/yourusername/pedil
+Author: Ire Gaddr
+Author-email: iregaddr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: sympy
 
@@ -37,23 +37,25 @@
 ```python
 
 from pedil import PEDIL
 
 # Create an instance of the PEDIL class
 pedil = PEDIL()
 
-# Generate unique IDs
+# Generate unique IDs securely
 id1 = pedil.get_or_create_prime_id("1")
 id2 = pedil.get_or_create_prime_id("1,1")
-id3 = pedil.get_or_create_prime_id("2,3,5")
+id3 = pedil.get_or_create_prime_id("2,3")
+id4 = pedil.get_or_create_prime_id("3,4")
 
-# Print the generated IDs
-print(f"ID for '1': {id1}")
-print(f"ID for '1,1': {id2}")
-print(f"ID for '2,3,5': {id3}")
+# Return the secure IDs
+print(f"{id1}")
+print(f"{id2}")
+print(f"{id3}")
+print(f"{id4}")
 ```
 
 ![example](1.png)
 
 Prime Extended Decimal Index Listing (PEDIL)
 Annotation System
 
@@ -87,11 +89,19 @@
 
 Applications and Use Cases
 Practical Use
 
 For most real-world applications, using 1 or 2 levels of PEDIL notation should be sufficient to provide a vast number of unique IDs efficiently without excessive computational overhead.
 Big Data and Machine Learning
 
-For applications like big data and machine learning, where handling trillions of tokens and long processing times are common, PEDIL can scale to higher levels and larger base arrays, offering unique IDs in the trillions.
+For applications like big data and machine learning, where handling trillions of tokens and long processing times are common, PEDIL can scale to higher levels and larger base arrays, offering unique IDs in far beyond the trillions.
+
+Security Considerations
+
+Salting and Hashing
+
+    Each ID is salted and hashed using HMAC with SHA-256 to ensure uniqueness and prevent prediction or spoofing.
+    The salt is randomly generated during initialization, making each ID unique even with the same input.
+
 License
 
 This project is licensed under the MIT License.
```

### Comparing `pedil-0.1.0/pedil/pedil.py` & `pedil-0.1.1/pedil/pedil.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import sympy
+import hashlib
+import os
+import hmac
 
 class PEDIL:
-    def __init__(self, base_prime_limit=10**6):  # Base array size up to 1 million
+    def __init__(self, base_prime_limit=10**6, salt_length=16):
         self.base_primes = list(sympy.primerange(0, base_prime_limit))
-        #print(f"Initialized with {len(self.base_primes)} base primes.")
+        self.salt = os.urandom(salt_length)
         self.prime_cache = {}
+        #print(f"Initialized with {len(self.base_primes)} base primes.")
 
     def generate_prime_id(self, pedil_notation):
         """
         Generate a unique prime ID based on the PEDIL notation.
         :param pedil_notation: A string representing the PEDIL notation, e.g., '1,1'
         :return: A unique prime number as the ID
         """
@@ -17,51 +21,60 @@
         prime_index = 0
         base_length = len(self.base_primes)
         for i, level in enumerate(levels):
             prime_index += int(level) * (base_length ** (len(levels) - i - 1))
         #print(f"Calculated prime_index: {prime_index}")
         if prime_index >= len(self.base_primes):
             self.extend_prime_array(prime_index)
-        #print(f"Generated prime ID: {self.base_primes[prime_index]}")
-        return self.base_primes[prime_index]
+        prime_value = self.base_primes[prime_index]
+        return self.obscure_prime_id(prime_value, pedil_notation)
 
     def extend_prime_array(self, required_index):
         """
         Extend the base prime array to accommodate higher indices.
         :param required_index: The required index to extend the array to
         """
         current_max = len(self.base_primes)
         additional_primes_needed = required_index - current_max + 1
         #print(f"Extending prime array to accommodate index: {required_index} (adding {additional_primes_needed} primes)")
 
         next_prime_start = self.base_primes[-1] + 1
-        new_primes = []
         chunk_size = 100000  # Manageable chunk size for generating primes
-        while len(new_primes) < additional_primes_needed:
+        while len(self.base_primes) <= required_index:
             next_prime_end = next_prime_start + chunk_size
             #print(f"Generating primes in range: {next_prime_start} to {next_prime_end}")
             primes_generated = list(sympy.primerange(next_prime_start, next_prime_end))
-            new_primes.extend(primes_generated)
+            self.base_primes.extend(primes_generated)
             next_prime_start = next_prime_end
             #print(f"Primes generated in this iteration: {len(primes_generated)}")
-            #print(f"Total primes generated so far: {len(new_primes)}")
+            #print(f"Total primes generated so far: {len(self.base_primes)}")
 
             if not primes_generated:
                 raise RuntimeError("Failed to generate new primes.")
 
-        self.base_primes.extend(new_primes[:additional_primes_needed])
         #print(f"Extended prime array to {len(self.base_primes)} primes.")
-        #print(f"New primes added: {new_primes[:additional_primes_needed]}")
+
+    def obscure_prime_id(self, prime_value, pedil_notation):
+        """
+        Obscure the prime ID by hashing it with a salt and the PEDIL notation.
+        :param prime_value: The prime number generated by the PEDIL notation
+        :param pedil_notation: The original PEDIL notation
+        :return: A hashed and salted prime ID
+        """
+        data = f"{prime_value}:{pedil_notation}".encode('utf-8')
+        hashed = hmac.new(self.salt, data, hashlib.sha256).hexdigest()
+        return hashed
 
     def get_or_create_prime_id(self, alias):
         """
         Retrieve or generate a unique prime ID for a given alias.
         :param alias: A string alias for the ID
         :return: A unique prime number as the ID
         """
         if alias in self.prime_cache:
             #print(f"Found cached prime ID for alias '{alias}': {self.prime_cache[alias]}")
             return self.prime_cache[alias]
         prime_id = self.generate_prime_id(alias)
         self.prime_cache[alias] = prime_id
         #print(f"Cached prime ID for alias '{alias}': {prime_id}")
         return prime_id
+
```

### Comparing `pedil-0.1.0/pedil.egg-info/PKG-INFO` & `pedil-0.1.1/pedil.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pedil
-Version: 0.1.0
-Summary: A Python package for generating unique IDs using the Prime Extended Decimal Index Listing (PEDIL) method.
-Home-page: https://github.com/IreGaddr/pedil
-Author: Your Name
-Author-email: your.email@example.com
+Version: 0.1.1
+Summary: A Python package for generating unique and secure IDs using Prime Extended Decimal Index Listing (PEDIL).
+Home-page: https://github.com/yourusername/pedil
+Author: Ire Gaddr
+Author-email: iregaddr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: sympy
 
@@ -37,23 +37,25 @@
 ```python
 
 from pedil import PEDIL
 
 # Create an instance of the PEDIL class
 pedil = PEDIL()
 
-# Generate unique IDs
+# Generate unique IDs securely
 id1 = pedil.get_or_create_prime_id("1")
 id2 = pedil.get_or_create_prime_id("1,1")
-id3 = pedil.get_or_create_prime_id("2,3,5")
+id3 = pedil.get_or_create_prime_id("2,3")
+id4 = pedil.get_or_create_prime_id("3,4")
 
-# Print the generated IDs
-print(f"ID for '1': {id1}")
-print(f"ID for '1,1': {id2}")
-print(f"ID for '2,3,5': {id3}")
+# Return the secure IDs
+print(f"{id1}")
+print(f"{id2}")
+print(f"{id3}")
+print(f"{id4}")
 ```
 
 ![example](1.png)
 
 Prime Extended Decimal Index Listing (PEDIL)
 Annotation System
 
@@ -87,11 +89,19 @@
 
 Applications and Use Cases
 Practical Use
 
 For most real-world applications, using 1 or 2 levels of PEDIL notation should be sufficient to provide a vast number of unique IDs efficiently without excessive computational overhead.
 Big Data and Machine Learning
 
-For applications like big data and machine learning, where handling trillions of tokens and long processing times are common, PEDIL can scale to higher levels and larger base arrays, offering unique IDs in the trillions.
+For applications like big data and machine learning, where handling trillions of tokens and long processing times are common, PEDIL can scale to higher levels and larger base arrays, offering unique IDs in far beyond the trillions.
+
+Security Considerations
+
+Salting and Hashing
+
+    Each ID is salted and hashed using HMAC with SHA-256 to ensure uniqueness and prevent prediction or spoofing.
+    The salt is randomly generated during initialization, making each ID unique even with the same input.
+
 License
 
 This project is licensed under the MIT License.
```

### Comparing `pedil-0.1.0/setup.py` & `pedil-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup, find_packages
 
+# Read the contents of the README file
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
-    name='pedil',
-    version='0.1.0',
+    name="pedil",
+    version="0.1.1",  # Increment the version number
+    author="Ire Gaddr",
+    author_email="iregaddr@gmail.com",
+    description="A Python package for generating unique and secure IDs using Prime Extended Decimal Index Listing (PEDIL).",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/yourusername/pedil",
     packages=find_packages(),
-    install_requires=[
-        'sympy',  # Specify dependencies here
-    ],
-    author='Your Name',
-    author_email='your.email@example.com',
-    description='A Python package for generating unique IDs using the Prime Extended Decimal Index Listing (PEDIL) method.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/IreGaddr/pedil',  # Replace with your GitHub repository URL
     classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires=">=3.6",
+    install_requires=[
+        "sympy",
     ],
-    python_requires='>=3.6',
 )
```

