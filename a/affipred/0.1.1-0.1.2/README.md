# Comparing `tmp/affipred-0.1.1.tar.gz` & `tmp/affipred-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affipred-0.1.1.tar", last modified: Tue Dec 19 19:06:07 2023, max compression
+gzip compressed data, was "affipred-0.1.2.tar", last modified: Thu May 16 07:57:27 2024, max compression
```

## Comparing `affipred-0.1.1.tar` & `affipred-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mustafa   (1000) mustafa   (1000)        0 2023-12-19 19:06:07.983768 affipred-0.1.1/
-drwxrwxr-x   0 mustafa   (1000) mustafa   (1000)        0 2023-12-19 19:06:07.983768 affipred-0.1.1/AFFIPred_cli/
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       36 2023-11-25 21:46:33.000000 affipred-0.1.1/AFFIPred_cli/__init__.py
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)     5496 2023-12-19 18:28:28.000000 affipred-0.1.1/AFFIPred_cli/affipred.py
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)      674 2023-12-19 18:29:19.000000 affipred-0.1.1/AFFIPred_cli/cli.py
--rw-r--r--   0 mustafa   (1000) mustafa   (1000)     1004 2023-12-19 19:06:07.983768 affipred-0.1.1/PKG-INFO
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)      306 2023-12-19 19:04:49.000000 affipred-0.1.1/README.md
-drwxrwxr-x   0 mustafa   (1000) mustafa   (1000)        0 2023-12-19 19:06:07.983768 affipred-0.1.1/affipred.egg-info/
--rw-r--r--   0 mustafa   (1000) mustafa   (1000)     1004 2023-12-19 19:06:07.000000 affipred-0.1.1/affipred.egg-info/PKG-INFO
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)      297 2023-12-19 19:06:07.000000 affipred-0.1.1/affipred.egg-info/SOURCES.txt
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)        1 2023-12-19 19:06:07.000000 affipred-0.1.1/affipred.egg-info/dependency_links.txt
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       56 2023-12-19 19:06:07.000000 affipred-0.1.1/affipred.egg-info/entry_points.txt
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       87 2023-12-19 19:06:07.000000 affipred-0.1.1/affipred.egg-info/requires.txt
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       13 2023-12-19 19:06:07.000000 affipred-0.1.1/affipred.egg-info/top_level.txt
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       84 2023-11-25 19:39:46.000000 affipred-0.1.1/pyproject.toml
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       38 2023-12-19 19:06:07.983768 affipred-0.1.1/setup.cfg
--rw-rw-r--   0 mustafa   (1000) mustafa   (1000)     1050 2023-12-19 19:05:34.000000 affipred-0.1.1/setup.py
+drwxrwxr-x   0 mustafa   (1000) mustafa   (1000)        0 2024-05-16 07:57:27.181598 affipred-0.1.2/
+drwxrwxr-x   0 mustafa   (1000) mustafa   (1000)        0 2024-05-16 07:57:27.181598 affipred-0.1.2/AFFIPred_cli/
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       31 2024-05-16 07:50:55.000000 affipred-0.1.2/AFFIPred_cli/__init__.py
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)     5505 2024-05-16 07:50:42.000000 affipred-0.1.2/AFFIPred_cli/affipred.py
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)      659 2024-05-16 07:50:40.000000 affipred-0.1.2/AFFIPred_cli/cli.py
+-rw-r--r--   0 mustafa   (1000) mustafa   (1000)     1211 2024-05-16 07:57:27.181598 affipred-0.1.2/PKG-INFO
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)      539 2024-05-16 07:51:25.000000 affipred-0.1.2/README.md
+drwxrwxr-x   0 mustafa   (1000) mustafa   (1000)        0 2024-05-16 07:57:27.181598 affipred-0.1.2/affipred.egg-info/
+-rw-r--r--   0 mustafa   (1000) mustafa   (1000)     1211 2024-05-16 07:57:27.000000 affipred-0.1.2/affipred.egg-info/PKG-INFO
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)      297 2024-05-16 07:57:27.000000 affipred-0.1.2/affipred.egg-info/SOURCES.txt
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)        1 2024-05-16 07:57:27.000000 affipred-0.1.2/affipred.egg-info/dependency_links.txt
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       51 2024-05-16 07:57:27.000000 affipred-0.1.2/affipred.egg-info/entry_points.txt
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       75 2024-05-16 07:57:27.000000 affipred-0.1.2/affipred.egg-info/requires.txt
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       13 2024-05-16 07:57:27.000000 affipred-0.1.2/affipred.egg-info/top_level.txt
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       84 2024-04-02 09:32:05.000000 affipred-0.1.2/pyproject.toml
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)       38 2024-05-16 07:57:27.181598 affipred-0.1.2/setup.cfg
+-rw-rw-r--   0 mustafa   (1000) mustafa   (1000)     1031 2024-05-16 07:55:53.000000 affipred-0.1.2/setup.py
```

### Comparing `affipred-0.1.1/AFFIPred_cli/affipred.py` & `affipred-0.1.2/AFFIPred_cli/affipred.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
         with VariantFile(input_file) as vcf_file:
             for _ in vcf_file:
                 total_records += 1
 
         return total_records
 
-def affipred_pred(input_file, output_file="output.csv"):
+def affipred(input_file, output_file="output.csv", type = "VCF"):
 
     f2 = VariantFile(input_file)
 
     total_variants = get_total_records(input_file)
 
     vcf_data = []
     progress_bar = tqdm(total=total_variants, desc='Reading the vcf file', position=0, leave=True)
```

### Comparing `affipred-0.1.1/AFFIPred_cli/cli.py` & `affipred-0.1.2/AFFIPred_cli/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 The command-line interface for AFFIPred
 """
 import argparse
-from .affipred import affipred_pred
+from .affipred import affipred
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="AlphaFold based Functional Impact Prediction tool for Missense Variations."
     )
     parser.add_argument(
         "input", type=str,
         help="The VCF file to calculate prediction."
     )
     parser.add_argument(
         "--output", "-o",
-        help=("File name of the output file. It will be placed under the current directory.")
+        help=("Name of the output file. It will be placed under the current directory.")
     )
     args = parser.parse_args()
-    affipred_pred(input_file=args.input, output_file=args.output)
+    affipred(input_file=args.input, output_file=args.output)
     print("Success!")
 
 if __name__ == "__main__":
     main()
```

### Comparing `affipred-0.1.1/setup.py` & `affipred-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="affipred",
-    version="0.1.1",
+    version="0.1.2",
     author="Mustafa S. Pir",
     author_email="mustafapir29@gmail.com",
     description=("AlphaFold based Functional Impact Prediction of Missense Variations"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mustafapir/affipred",
     project_urls={
         "Bug Tracker": "https://github.com/mustafapir/affipred/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["pysam>=0.22.0","requests>=2.31.0","pandas>=2.0.0","biopython>=1.81","numpy>=1.24.0","tqdm>=4.0.0"],
+    install_requires=["pysam>=0.22.0","requests>=2.31.0","pandas>=2.0.0","biopython>=1.81","numpy>=1.24.0"],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
     entry_points={
         "console_scripts": [
-            "affipred_pred = AFFIPred_cli.cli:main",
+            "affipred = AFFIPred_cli.cli:main",
         ]
     }
 )
```

