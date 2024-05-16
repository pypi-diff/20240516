# Comparing `tmp/kmerator-0.9.3b0.tar.gz` & `tmp/kmerator-0.9.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerator-0.9.3b0.tar", last modified: Mon Dec 18 09:24:26 2023, max compression
+gzip compressed data, was "kmerator-0.9.6b0.tar", last modified: Wed May 15 16:04:05 2024, max compression
```

## Comparing `kmerator-0.9.3b0.tar` & `kmerator-0.9.6b0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-12-18 09:24:26.114877 kmerator-0.9.3b0/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      182 2023-08-31 15:02:10.000000 kmerator-0.9.3b0/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    12907 2023-12-18 09:24:26.110483 kmerator-0.9.3b0/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    10641 2023-08-31 15:02:10.000000 kmerator-0.9.3b0/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-12-18 09:24:26.007884 kmerator-0.9.3b0/kmerator/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-08-31 15:02:10.000000 kmerator-0.9.3b0/kmerator/__init__.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      249 2023-08-31 15:02:10.000000 kmerator-0.9.3b0/kmerator/color.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-08-31 15:02:10.000000 kmerator-0.9.3b0/kmerator/config.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    20758 2023-12-18 08:41:53.000000 kmerator-0.9.3b0/kmerator/dataset.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-08-31 15:02:10.000000 kmerator-0.9.3b0/kmerator/exit.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     6179 2023-09-07 09:04:12.000000 kmerator-0.9.3b0/kmerator/geneinfo.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     1872 2023-12-18 08:59:54.000000 kmerator-0.9.3b0/kmerator/info.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    12015 2023-09-05 10:51:45.000000 kmerator-0.9.3b0/kmerator/kmerator.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    18359 2023-09-06 08:19:27.000000 kmerator-0.9.3b0/kmerator/kmerize.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-09-06 08:34:34.000000 kmerator-0.9.3b0/kmerator/longest_transcript.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    12156 2023-09-04 15:10:47.000000 kmerator-0.9.3b0/kmerator/mk_geneinfo.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     9890 2023-09-05 10:17:44.000000 kmerator-0.9.3b0/kmerator/mk_transcriptome.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    14378 2023-09-06 08:25:25.000000 kmerator-0.9.3b0/kmerator/options.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-12-18 09:24:26.094459 kmerator-0.9.3b0/kmerator.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    12907 2023-12-18 09:24:25.000000 kmerator-0.9.3b0/kmerator.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      502 2023-12-18 09:24:25.000000 kmerator-0.9.3b0/kmerator.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-12-18 09:24:25.000000 kmerator-0.9.3b0/kmerator.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-12-18 09:24:25.000000 kmerator-0.9.3b0/kmerator.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-12-18 09:24:25.000000 kmerator-0.9.3b0/kmerator.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-12-18 09:24:25.000000 kmerator-0.9.3b0/kmerator.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-12-18 09:24:26.117401 kmerator-0.9.3b0/setup.cfg
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1109 2023-08-31 15:02:10.000000 kmerator-0.9.3b0/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-05-15 16:04:05.111045 kmerator-0.9.6b0/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      182 2023-08-31 15:02:10.000000 kmerator-0.9.6b0/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    12907 2024-05-15 16:04:05.106582 kmerator-0.9.6b0/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    10641 2023-08-31 15:02:10.000000 kmerator-0.9.6b0/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-05-15 16:04:04.985965 kmerator-0.9.6b0/kmerator/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-08-31 15:02:10.000000 kmerator-0.9.6b0/kmerator/__init__.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      249 2023-08-31 15:02:10.000000 kmerator-0.9.6b0/kmerator/color.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-08-31 15:02:10.000000 kmerator-0.9.6b0/kmerator/config.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    20730 2023-12-18 10:44:43.000000 kmerator-0.9.6b0/kmerator/dataset.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-08-31 15:02:10.000000 kmerator-0.9.6b0/kmerator/exit.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     6179 2023-09-07 09:04:12.000000 kmerator-0.9.6b0/kmerator/geneinfo.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     1872 2023-12-19 10:59:26.000000 kmerator-0.9.6b0/kmerator/info.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    12015 2023-12-19 10:40:44.000000 kmerator-0.9.6b0/kmerator/kmerator.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    18397 2023-12-19 10:56:23.000000 kmerator-0.9.6b0/kmerator/kmerize.py
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-09-06 08:34:34.000000 kmerator-0.9.6b0/kmerator/longest_transcript.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    12156 2023-09-04 15:10:47.000000 kmerator-0.9.6b0/kmerator/mk_geneinfo.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     9890 2023-09-05 10:17:44.000000 kmerator-0.9.6b0/kmerator/mk_transcriptome.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    14378 2023-09-06 08:25:25.000000 kmerator-0.9.6b0/kmerator/options.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-05-15 16:04:05.090556 kmerator-0.9.6b0/kmerator.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    12907 2024-05-15 16:04:04.000000 kmerator-0.9.6b0/kmerator.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      502 2024-05-15 16:04:04.000000 kmerator-0.9.6b0/kmerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2024-05-15 16:04:04.000000 kmerator-0.9.6b0/kmerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2024-05-15 16:04:04.000000 kmerator-0.9.6b0/kmerator.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2024-05-15 16:04:04.000000 kmerator-0.9.6b0/kmerator.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2024-05-15 16:04:04.000000 kmerator-0.9.6b0/kmerator.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2024-05-15 16:04:05.113633 kmerator-0.9.6b0/setup.cfg
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1109 2023-08-31 15:02:10.000000 kmerator-0.9.6b0/setup.py
```

### Comparing `kmerator-0.9.3b0/PKG-INFO` & `kmerator-0.9.6b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.9.3b0
+Version: 0.9.6b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.9.3b0/README.md` & `kmerator-0.9.6b0/README.md`

 * *Files identical despite different names*

### Comparing `kmerator-0.9.3b0/kmerator/config.py` & `kmerator-0.9.6b0/kmerator/config.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.9.3b0/kmerator/dataset.py` & `kmerator-0.9.6b0/kmerator/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,16 +413,15 @@
                 sys.exit("Aborted by user.")
         else:
             print(f"The last release for {self.args.specie} is {self.args.release}, nothing to do.")
         exit.gracefully(self.args)
 
 
     def last_available(self):
-        # ~ self.get_ebl_releases()
-        print(max(self.ebl_releases))
+        print(self.get_ebl_current_release())
         exit.gracefully(self.args)
 
 
 def usage():
     parser = argparse.ArgumentParser()
     exclusive = parser.add_mutually_exclusive_group(required=True)
     ### OPTION
```

### Comparing `kmerator-0.9.3b0/kmerator/geneinfo.py` & `kmerator-0.9.6b0/kmerator/geneinfo.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.9.3b0/kmerator/info.py` & `kmerator-0.9.6b0/kmerator/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # info.py
 
 """
 Genral informations on to the program.
 """
 
 APPNAME = "kmerator"
-VERSION = "0.9.3-beta"
+VERSION = "0.9.6-beta"
 VERSION_DATASET = 1
 SHORTDESC = "Find specific gene or transcript kmers. And more."
 LICENCE = "GPL3"
 AUTHOR = 'Sébastien RIQUIER, IRMB, Montpellier'
 AUTHOR_EMAIL = "sebastien.riquier@ucd.ie"
 CONTIBUTORS = [
     'Chloe BESSIERE chloe.bessiere@inserm.fr>'
```

### Comparing `kmerator-0.9.3b0/kmerator/kmerator.py` & `kmerator-0.9.6b0/kmerator/kmerator.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.9.3b0/kmerator/kmerize.py` & `kmerator-0.9.6b0/kmerator/kmerize.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,28 +101,28 @@
     def dump_seq(self, f_id, seq):
         '''
         Write sequences in temporary file (needed by jellyfish)
         '''
         seq_dir = os.path.join(self.args['tmpdir'], 'sequences')
         os.makedirs(seq_dir, exist_ok=True)
         ### write sequence as fasta
-        seq_file = os.path.join(seq_dir, f"{f_id}.fa")
+        seq_file = os.path.join(seq_dir, f"{f_id.replace('/', '--')}.fa")
         with open(seq_file, 'w') as fh:
             fh.write(f">{f_id}\n{seq}\n")
         return seq_file
 
 
     def jellyfish(self, seq_file, jf_file):
         """
         From sequence, compute jellyfish againt the genome/transcriptome and convert results
         as dict ()
         """
         if self.args['debug']: print(f"{YELLOW}start jellyfish on {os.path.basename(seq_file)} "
                                      f"against {os.path.basename(jf_file)}{ENDCOL}")
-        cmd = f"jellyfish query -s '{seq_file}' {jf_file}"
+        cmd = f'jellyfish query -s "{seq_file}" {jf_file}'
         try:
             result = subprocess.check_output(cmd, shell=True, text=True, stderr=subprocess.STDOUT) \
                                              .rstrip('\n').split('\n')
         except subprocess.CalledProcessError as err:
             sys.exit(f"{ERROR}Error: executing jellyfish:\n"
                      f"  {ERROR}command: {ENDCOL}{cmd}\n"
                      f"  {ERROR}returned: {ENDCOL}{err.output}")
@@ -358,15 +358,15 @@
         return 'done', mesg
 
 
     def write(self, args, outfile, specific_seq, type):
         """ Write results as fasta file"""
         outdir = os.path.join(args['tmpdir'], type)
         os.makedirs(outdir, exist_ok=True)
-        with open(os.path.join(outdir, outfile), 'w') as fh:
+        with open(os.path.join(outdir, outfile.replace('/', '--')), 'w') as fh:
             fh.write("\n".join(specific_seq) + '\n')
 
 
     def __canonical(self, mer):
         revcomp = mer[::-1].translate(str.maketrans('ATCG','TAGC'))
         return sorted((mer, revcomp))[0]
```

### Comparing `kmerator-0.9.3b0/kmerator/longest_transcript.py` & `kmerator-0.9.6b0/kmerator/longest_transcript.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.9.3b0/kmerator/mk_geneinfo.py` & `kmerator-0.9.6b0/kmerator/mk_geneinfo.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.9.3b0/kmerator/mk_transcriptome.py` & `kmerator-0.9.6b0/kmerator/mk_transcriptome.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.9.3b0/kmerator/options.py` & `kmerator-0.9.6b0/kmerator/options.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.9.3b0/kmerator.egg-info/PKG-INFO` & `kmerator-0.9.6b0/kmerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.9.3b0
+Version: 0.9.6b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.9.3b0/setup.py` & `kmerator-0.9.6b0/setup.py`

 * *Files identical despite different names*

