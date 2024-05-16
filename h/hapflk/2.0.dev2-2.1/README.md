# Comparing `tmp/hapflk-2.0.dev2.tar.gz` & `tmp/hapflk-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hapflk-2.0.dev2.tar", last modified: Wed Jul  8 06:59:18 2020, max compression
+gzip compressed data, was "/scratch/code/hapflk/dist/.tmp-f1hc3kx6/hapflk-2.1.tar", last modified: Thu May 16 12:58:35 2024, max compression
```

## Comparing `hapflk-2.0.dev2.tar` & `hapflk-2.1.tar`

### file list

```diff
@@ -1,42 +1,29 @@
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-07-08 06:59:18.024526 hapflk-2.0.dev2/
--rw-rw-rw-   0 bservin   (1000) biomath   (1001)      794 2013-10-08 08:58:19.000000 hapflk-2.0.dev2/COPYING.txt
--rw-rw-r--   0 bservin   (1000) biomath   (1001)    35147 2013-10-08 08:58:00.000000 hapflk-2.0.dev2/LICENSE.txt
--rw-rw-rw-   0 bservin   (1000) biomath   (1001)      190 2019-01-25 13:24:05.000000 hapflk-2.0.dev2/MANIFEST.in
--rw-r-----   0 bservin   (1000) biomath   (1001)     1506 2020-07-08 06:59:18.020527 hapflk-2.0.dev2/PKG-INFO
--rw-r-----   0 bservin   (1000) biomath   (1001)      704 2017-09-01 08:05:48.000000 hapflk-2.0.dev2/README
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-07-08 06:59:17.888527 hapflk-2.0.dev2/bin/
--rwxr-x--x   0 bservin   (1000) biomath   (1001)     4164 2019-03-26 09:04:51.000000 hapflk-2.0.dev2/bin/flkfreq
--rwxr-x--x   0 bservin   (1000) biomath   (1001)     2348 2018-11-16 07:25:30.000000 hapflk-2.0.dev2/bin/flkpoptree
--rwxr-x--x   0 bservin   (1000) biomath   (1001)      692 2018-11-15 08:03:14.000000 hapflk-2.0.dev2/bin/hapflk
--rw-r-----   0 bservin   (1000) biomath   (1001)     5191 2020-07-08 06:53:51.000000 hapflk-2.0.dev2/bin/hapflkadapt
--rwxr-x--x   0 bservin   (1000) biomath   (1001)    15916 2019-03-13 14:58:09.000000 hapflk-2.0.dev2/bin/poolflkadapt
--rw-r-----   0 bservin   (1000) biomath   (1001)    12236 2019-01-28 15:15:39.000000 hapflk-2.0.dev2/bin/poolflkannot
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-07-08 06:59:17.920527 hapflk-2.0.dev2/fastphase/
--rw-r-----   0 bservin   (1000) biomath   (1001)  1655716 2020-07-07 14:53:56.000000 hapflk-2.0.dev2/fastphase/fastphase.c
--rw-------   0 bservin   (1000) biomath   (1001)    38892 2020-07-07 14:48:57.000000 hapflk-2.0.dev2/fastphase/fastphase.pyx
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-07-08 06:59:17.940527 hapflk-2.0.dev2/hapflk/
--rw-r-----   0 bservin   (1000) biomath   (1001)    15386 2020-07-08 06:53:51.000000 hapflk-2.0.dev2/hapflk/InputOutput.py
--rw-rw-r--   0 bservin   (1000) biomath   (1001)      265 2018-06-15 07:44:49.000000 hapflk-2.0.dev2/hapflk/__init__.py
--rw-rw-r--   0 bservin   (1000) biomath   (1001)    28362 2019-03-26 08:36:16.000000 hapflk-2.0.dev2/hapflk/data.py
--rw-r-----   0 bservin   (1000) biomath   (1001)    18957 2019-03-01 16:20:00.000000 hapflk-2.0.dev2/hapflk/hapflk.py
--rw-r-----   0 bservin   (1000) biomath   (1001)    33439 2019-04-10 16:10:31.000000 hapflk-2.0.dev2/hapflk/hapflkadapt.py
--rw-r-----   0 bservin   (1000) biomath   (1001)    12450 2019-03-26 09:19:43.000000 hapflk-2.0.dev2/hapflk/nj.py
--rw-rw-r--   0 bservin   (1000) biomath   (1001)    12150 2018-12-17 10:59:13.000000 hapflk-2.0.dev2/hapflk/popgen.py
--rw-r-----   0 bservin   (1000) biomath   (1001)      916 2018-08-27 09:56:04.000000 hapflk-2.0.dev2/hapflk/utils.py
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-07-08 06:59:17.952527 hapflk-2.0.dev2/hapflk.egg-info/
--rw-r-----   0 bservin   (1000) biomath   (1001)     1506 2020-07-08 06:59:17.000000 hapflk-2.0.dev2/hapflk.egg-info/PKG-INFO
--rw-r-----   0 bservin   (1000) biomath   (1001)      687 2020-07-08 06:59:17.000000 hapflk-2.0.dev2/hapflk.egg-info/SOURCES.txt
--rw-r-----   0 bservin   (1000) biomath   (1001)        1 2020-07-08 06:59:17.000000 hapflk-2.0.dev2/hapflk.egg-info/dependency_links.txt
--rw-r-----   0 bservin   (1000) biomath   (1001)       19 2020-07-08 06:59:17.000000 hapflk-2.0.dev2/hapflk.egg-info/requires.txt
--rw-r-----   0 bservin   (1000) biomath   (1001)        7 2020-07-08 06:59:17.000000 hapflk-2.0.dev2/hapflk.egg-info/top_level.txt
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-07-08 06:59:18.020527 hapflk-2.0.dev2/pgenlib/
--rw-r-----   0 bservin   (1000) biomath   (1001)  1627883 2020-07-08 06:53:04.000000 hapflk-2.0.dev2/pgenlib/_pgenlib.cpp
--rw-------   0 bservin   (1000) biomath   (1001)    90126 2017-10-18 07:00:39.000000 hapflk-2.0.dev2/pgenlib/_pgenlib.pyx
--rw-------   0 bservin   (1000) biomath   (1001)   391687 2017-10-16 13:46:51.000000 hapflk-2.0.dev2/pgenlib/pgenlib_internal.cpp
--rw-------   0 bservin   (1000) biomath   (1001)    55172 2017-10-16 13:46:51.000000 hapflk-2.0.dev2/pgenlib/pgenlib_internal.h
--rw-------   0 bservin   (1000) biomath   (1001)    17624 2017-10-16 13:46:51.000000 hapflk-2.0.dev2/pgenlib/pgenlib_python_support.cpp
--rw-------   0 bservin   (1000) biomath   (1001)     3970 2017-10-16 13:46:51.000000 hapflk-2.0.dev2/pgenlib/pgenlib_python_support.h
--rw-------   0 bservin   (1000) biomath   (1001)    34704 2017-10-16 13:46:51.000000 hapflk-2.0.dev2/pgenlib/plink2_base.cpp
--rw-------   0 bservin   (1000) biomath   (1001)    45250 2017-10-16 13:46:51.000000 hapflk-2.0.dev2/pgenlib/plink2_base.h
--rw-r-----   0 bservin   (1000) biomath   (1001)       38 2020-07-08 06:59:18.024526 hapflk-2.0.dev2/setup.cfg
--rw-rw-rw-   0 bservin   (1000) biomath   (1001)     2140 2020-07-08 06:59:09.000000 hapflk-2.0.dev2/setup.py
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-16 12:58:35.877911 hapflk-2.1/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      794 2023-07-18 12:03:54.000000 hapflk-2.1/COPYING.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    35147 2023-07-18 12:03:54.000000 hapflk-2.1/LICENSE.txt
+-rw-r--r--   0 bservin   (1001) bservin   (1001)      796 2024-05-16 12:58:35.877911 hapflk-2.1/PKG-INFO
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      704 2023-07-18 12:03:54.000000 hapflk-2.1/README
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-16 12:58:35.877911 hapflk-2.1/bin/
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)      692 2023-07-18 12:03:54.000000 hapflk-2.1/bin/hapflk
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)     5072 2024-05-16 12:53:06.000000 hapflk-2.1/bin/hapflkadapt
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-16 12:58:35.877911 hapflk-2.1/hapflk/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    15357 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/InputOutput.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      313 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/__init__.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    29639 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/data.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     4553 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/flkfreq.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)     2265 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/flkpoptree.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)    22595 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/hapflk.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    36839 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/hapflkadapt.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    12970 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/nj.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    18920 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/poolflkadapt.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    12659 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/popgen.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     1012 2024-05-16 12:53:06.000000 hapflk-2.1/hapflk/utils.py
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-16 12:58:35.877911 hapflk-2.1/hapflk.egg-info/
+-rw-r--r--   0 bservin   (1001) bservin   (1001)      796 2024-05-16 12:58:35.000000 hapflk-2.1/hapflk.egg-info/PKG-INFO
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      457 2024-05-16 12:58:35.000000 hapflk-2.1/hapflk.egg-info/SOURCES.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        1 2024-05-16 12:58:35.000000 hapflk-2.1/hapflk.egg-info/dependency_links.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      207 2024-05-16 12:58:35.000000 hapflk-2.1/hapflk.egg-info/entry_points.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)       45 2024-05-16 12:58:35.000000 hapflk-2.1/hapflk.egg-info/requires.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        7 2024-05-16 12:58:35.000000 hapflk-2.1/hapflk.egg-info/top_level.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     1182 2024-05-16 12:53:06.000000 hapflk-2.1/pyproject.toml
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)       38 2024-05-16 12:58:35.877911 hapflk-2.1/setup.cfg
```

### Comparing `hapflk-2.0.dev2/COPYING.txt` & `hapflk-2.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `hapflk-2.0.dev2/LICENSE.txt` & `hapflk-2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hapflk-2.0.dev2/README` & `hapflk-2.1/README`

 * *Files identical despite different names*

### Comparing `hapflk-2.0.dev2/bin/flkpoptree` & `hapflk-2.1/hapflk/flkpoptree.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,70 @@
-#!/usr/bin/env python3
 import sys
 import datetime as dt
 import numpy as np
 from hapflk import hapflk, utils, popgen
 
- 
+
 def main():
     counter = utils.Stepper()
     myopts = hapflk.HapFLK.get_opts(sys.argv)
     mymod = hapflk.HapFLK()
 
     counter.new("Reading In Data")
-    data = mymod.read_input( myopts)
-    
+    data = mymod.read_input(myopts)
+
     counter.new("Computing Allele Frequencies")
     res = data.compute_pop_frq()
-    frq = res['freqs']
-    pops = res['pops']
-    
+    frq = res["freqs"]
+    pops = res["pops"]
+
     counter.new("Setting up SNP subset")
-    minfrq = np.min( frq, axis= 0)
-    maxfrq = np.max( frq, axis= 0)
+    minfrq = np.min(frq, axis=0)
+    maxfrq = np.max(frq, axis=0)
     ## Keep SNPs where at least one pop has freq in ]a, 1-a[ with
     ## a small (0.1)
     a = 0.1
-    subset = (maxfrq > a) & (minfrq < (1-a))
-    nsnp = np.sum( subset)
-    print( "SNP subset : %d/%d"%(nsnp,len(maxfrq)))
-    subfreqs = frq[:,subset]
-    pbinom = np.min( (1,float(myopts.reysnps)/nsnp))
-    rand_subset = np.array( np.random.binomial( 1,pbinom,nsnp),dtype=bool)
-    reynolds = popgen.reynolds( subfreqs[:,rand_subset])
-    hzy = popgen.heterozygosity( subfreqs[:,rand_subset])
-    
-    kinship  = popgen.popKinship_new( reynolds, pops, myopts.outgroup,
-                                      fprefix = myopts.prefix,
-                                      keep_outgroup = myopts.keepOG,
-                                      hzy = hzy,
-                                        dump_tree = myopts.tree)
+    subset = (maxfrq > a) & (minfrq < (1 - a))
+    nsnp = np.sum(subset)
+    print("SNP subset : %d/%d" % (nsnp, len(maxfrq)))
+    subfreqs = frq[:, subset]
+    pbinom = np.min((1, float(myopts.reysnps) / nsnp))
+    rand_subset = np.array(np.random.binomial(1, pbinom, nsnp), dtype=bool)
+    reynolds = popgen.reynolds(subfreqs[:, rand_subset])
+    hzy = popgen.heterozygosity(subfreqs[:, rand_subset])
+
+    kinship = popgen.popKinship_new(
+        reynolds,
+        pops,
+        myopts.outgroup,
+        fprefix=myopts.prefix,
+        keep_outgroup=myopts.keepOG,
+        hzy=hzy,
+        dump_tree=myopts.tree,
+    )
     if myopts.covkin:
-        counter.new('Computing Covariance Matrix')
-        ff=popgen.FLK_test(kinship)
+        counter.new("Computing Covariance Matrix")
+        ff = popgen.FLK_test(kinship)
         ## calculate hat(p0)
-        pzero=np.array([ff.eigen_contrib(subfreqs[:,s])[0] for s in range(nsnp)])
-        sub=(pzero>0.05)&(pzero<0.95)
+        pzero = np.array([ff.eigen_contrib(subfreqs[:, s])[0] for s in range(nsnp)])
+        sub = (pzero > 0.05) & (pzero < 0.95)
         ## calculate empirical covariance matrix
-        myf=subfreqs[:,sub]
-        m=pzero[sub]
-        s=np.sqrt(m*(1-m))
-        myfstd=(myf-m)/s
-        covkin=np.cov(myfstd,rowvar=True)
+        myf = subfreqs[:, sub]
+        m = pzero[sub]
+        s = np.sqrt(m * (1 - m))
+        myfstd = (myf - m) / s
+        covkin = np.cov(myfstd, rowvar=True)
         ## Add a small term on the diagonal to ensure stable inverse
-        val=np.trace(covkin)/kinship.shape[0]
-        assert (val >0)
-        covkin=covkin+np.diag(np.ones(kinship.shape[0])*0.01*val)
-        with open(myopts.prefix+'_cov.txt','w') as fcov:
-            for i,pi in enumerate(pops):
-                tw=[pi]
-                for j,pj in enumerate(pops):
-                    tw.append(str(covkin[i,j]))
-                print(' '.join(tw),file=fcov)
+        val = np.trace(covkin) / kinship.shape[0]
+        assert val > 0
+        covkin = covkin + np.diag(np.ones(kinship.shape[0]) * 0.01 * val)
+        with open(myopts.prefix + "_cov.txt", "w") as fcov:
+            for i, pi in enumerate(pops):
+                tw = [pi]
+                for j, pj in enumerate(pops):
+                    tw.append(str(covkin[i, j]))
+                print(" ".join(tw), file=fcov)
     counter.end()
-    
-if __name__=='__main__':
+
+
+if __name__ == "__main__":
     main()
```

### Comparing `hapflk-2.0.dev2/bin/hapflk` & `hapflk-2.1/bin/hapflk`

 * *Files identical despite different names*

### Comparing `hapflk-2.0.dev2/bin/hapflkadapt` & `hapflk-2.1/bin/hapflkadapt`

 * *Files 3% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from hapflk import utils, hapflk, hapflkadapt
 from hapflk import InputOutput as IO
 
 
 
 def main():
     counter = utils.Stepper()
-    
-    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+
+    parser = argparse.ArgumentParser()
     parser.add_argument( '--flkdb', dest='dbfile', help='DB file created by hapflk', default=None)
     parser.add_argument( '-o', '--prefix', dest='prefix', help='prefix for output files', default='hapflkadapt_out')
     parser.add_argument( '-x', '--ncpu', dest = 'ncpu', help='Number of threads ( default = number of CPU)', default = cpu_count(), type = int)
     parser.add_argument( '--std', dest='std', help='Standardize cofactors', default =False, action = "store_true")
     IO.populate_covariate_args( parser)
 
     if len(sys.argv) < 2:
         parser.print_help()
         sys.exit(0)
     myopts = parser.parse_args( sys.argv[ 1:])
 
     counter.new('Loading FLK DB file')
     flkmodel = hapflk.HapFLK.from_db_file( myopts.dbfile)
-    
+
     counter.new('Getting covariates information')
     covdata = IO.get_covariates_matrix( myopts.covar_file, myopts.cov, myopts.qcov, flkmodel.pops)
     ##print( covdata)
 
     for f in covdata['cofactors']:
         counter.new( " Analysing cofactor %s"% f)
         myprefix = myopts.prefix+'_'+f
@@ -88,10 +88,7 @@
                 print('rs', 'chr', 'pos', 'Zh', 'pvalueh', file=fout)
                 for i, d in enumerate(flka):
                     rs = flkmodel.sorted_snps[i].name
                     chrom,_,pos = flkmodel.carte.position(rs)
                     print( rs, chrom, int(pos), hflka[i]['Z'], hflka[i]['pvalue'], file=fout)
     counter.new('Done')
     counter.end()
-                    
-if __name__=='__main__':
-    main()
```

### Comparing `hapflk-2.0.dev2/hapflk/InputOutput.py` & `hapflk-2.1/hapflk/InputOutput.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,98 @@
 import sys
 import re
 import argparse
 import numpy as np
 from bisect import insort
 from hapflk import missing
 from hapflk import data
-import hapflk._pgenlib as _pgenlib
+import pgenlib
+
 
 def plink_bfile(string):
     try:
-        open(string+'.bed')
+        open(string + ".bed")
     except IOError:
-        msg="can't open BED file %s"%string+'.bed'
+        msg = "can't open BED file %s" % string + ".bed"
         raise argparse.ArgumentTypeError(msg)
     try:
-        open(string+'.fam')
+        open(string + ".fam")
     except IOError:
-        msg="can't open FAM file %s"%string+'.fam'
+        msg = "can't open FAM file %s" % string + ".fam"
         raise argparse.ArgumentTypeError(msg)
     try:
-        open(string+'.bim')
+        open(string + ".bim")
     except IOError:
-        msg="can't open BIM file %s"%string+'.bim'
+        msg = "can't open BIM file %s" % string + ".bim"
         raise argparse.ArgumentTypeError(msg)
     return string
 
+
 def shapeit_file(string):
     try:
-        open(string+'.haps')
+        open(string + ".haps")
     except IOError:
-        msg="can't open HAPS file%s"%string+'.haps'
+        msg = "can't open HAPS file%s" % string + ".haps"
         raise argparse.ArgumentTypeError(msg)
     try:
-        open(string+'.sample')
+        open(string + ".sample")
     except IOError:
-        msg="can't open SAMPLE file%s"%string+'.sample'
+        msg = "can't open SAMPLE file%s" % string + ".sample"
         raise argparse.ArgumentTypeError(msg)
     return string
 
-io_parser=argparse.ArgumentParser(add_help=False,formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-input_group=io_parser.add_argument_group('Input Files')
+
+io_parser = argparse.ArgumentParser(
+    add_help=False, formatter_class=argparse.ArgumentDefaultsHelpFormatter
+)
+input_group = io_parser.add_argument_group("Input Files")
 input_type_group = input_group.add_mutually_exclusive_group(required=True)
-input_type_group.add_argument('--bfile',metavar='PREFIX',help='PLINK bfile prefix (bim,fam,bed)',type=plink_bfile)
-input_type_group.add_argument('--sfile',metavar='PREFIX',help='ShapeIT file prefix (haps,sample)',type=shapeit_file)
+input_type_group.add_argument(
+    "--bfile", metavar="PREFIX", help="PLINK bfile prefix (bim,fam,bed)", type=plink_bfile
+)
+input_type_group.add_argument(
+    "--sfile", metavar="PREFIX", help="ShapeIT file prefix (haps,sample)", type=shapeit_file
+)
 
 
-defaultParams= {
-    "MissGeno":'0',
-    "MissPheno":'-9',
-    "MissParent":'0',
-    "MissSex":'0'
-    }
+defaultParams = {"MissGeno": "0", "MissPheno": "-9", "MissParent": "0", "MissSex": "0"}
+
 
+key = "kshuwewekiuvf"
 
-key="kshuwewekiuvf"
 
-def _get_snpIdx(myMap,chrom,left,right,othermap=False):
-    '''
+def _get_snpIdx(myMap, chrom, left, right, othermap=False):
+    """
     Return index of SNPs in map
 
     Parameters
     --------------
     myMap : the map
     chrom : chromosome
     left : leftmost position
     right : rightmost position
     othermap : use other (genetic / RH) map scale
-    '''
+    """
     if othermap:
-        getMap=myMap.genetMap
+        getMap = myMap.genetMap
     else:
-        getMap=myMap.physMap
-    mySnps=[ x for x in getMap(chrom,xleft=left,xright=right)]
-    mySnpIdx=[]
-    for i,s in enumerate(myMap.input_order):
+        getMap = myMap.physMap
+    mySnps = [x for x in getMap(chrom, xleft=left, xright=right)]
+    mySnpIdx = []
+    for i, s in enumerate(myMap.input_order):
         if s in mySnps:
             mySnpIdx.append(i)
     return mySnpIdx
 
+
 ##### generic input function ####
-def parseInput(options,params=defaultParams):
-    '''
-    Read input files 
-    
+def parseInput(options, params=defaultParams):
+    """
+    Read input files
+
     Parameters
     --------------
     options : options from io_parser
     params : parameters for coding used in input files, overidden using options
 
     Returns
     ----------
@@ -94,363 +100,401 @@
          -- dataset : an instance from the gwas Dataset class
          -- map : an instance from the gwas Map class
 
     See also
     ----------
     data.Dataset
     data.Map
-    '''
+    """
 
     ## read input
     if options.bfile:
-        return parsePlinkBfile(options.bfile,params=params,options=options)
+        return parsePlinkBfile(options.bfile, params=params, options=options)
     elif options.sfile:
         return parseShapeIT(options.sfile, params=params)
-        
-               
+
+
 ################ SHAPEIT2 files ####################################
 def parseShapeIT(prefix, params=defaultParams):
     ## parse sample file
-    idata=[]
-    with open(prefix+'.sample') as f:
-        for il,ligne in enumerate(f):
-            if il<2:
+    idata = []
+    with open(prefix + ".sample") as f:
+        for il, ligne in enumerate(f):
+            if il < 2:
                 continue
-            buf=ligne.split()
-            phe=((buf[6]!=params['MissPheno']) and float(buf[6])) or None
-            idata.append([buf[0], \
-                          buf[1],  \
-                              ((buf[3]!=params['MissParent']) and buf[3]) or None, \
-                              ((buf[4]!=params['MissParent']) and buf[4]) or None, \
-                              (buf[5]!=params['MissSex'] and buf[5]) or None, \
-                              phe])
-                              
+            buf = ligne.split()
+            phe = ((buf[6] != params["MissPheno"]) and float(buf[6])) or None
+            idata.append(
+                [
+                    buf[0],
+                    buf[1],
+                    ((buf[3] != params["MissParent"]) and buf[3]) or None,
+                    ((buf[4] != params["MissParent"]) and buf[4]) or None,
+                    (buf[5] != params["MissSex"] and buf[5]) or None,
+                    phe,
+                ]
+            )
+
     ## parse haps file
-    SNPs=[]
-    myMap=data.Map()
+    SNPs = []
+    myMap = data.Map()
     hdata = []
-    with open(prefix+'.haps') as f:
+    with open(prefix + ".haps") as f:
         for ligne in f:
-            buf=ligne.split()
-            hdata.append( [ int(i) for i in buf[5:] ] )
+            buf = ligne.split()
+            hdata.append([int(i) for i in buf[5:]])
             ## create SNP
-            myS=data.SNP(buf[1])
-            myS.alleles[0]=buf[3]
-            myS.alleles[1]=buf[4]
+            myS = data.SNP(buf[1])
+            myS.alleles[0] = buf[3]
+            myS.alleles[1] = buf[4]
             ## add marker to map
             try:
-                mychr=int(buf[0])
+                mychr = int(buf[0])
             except:
-                mychr=buf[0]
-            mychr=buf[0]
-            myMap.addMarker(M=buf[1],C=mychr,posG=float(buf[2])*1e-6,posP=float(buf[2]))
+                mychr = buf[0]
+            mychr = buf[0]
+            myMap.addMarker(M=buf[1], C=mychr, posG=float(buf[2]) * 1e-6, posP=float(buf[2]))
             SNPs.append(myS)
-    sdata = {'snps':SNPs, 'map':myMap}
-    ni = 2*len(idata)
-    ns = len(sdata['snps'])
+    sdata = {"snps": SNPs, "map": myMap}
+    ni = 2 * len(idata)
+    ns = len(sdata["snps"])
     mySnpIdx = range(ns)
-    dataset = data.Dataset(prefix,nsnp = ns, nindiv = ni)
+    dataset = data.Dataset(prefix, nsnp=ns, nindiv=ni)
     ## fill in SNP data
-    for s in [sdata['snps'][i] for i in mySnpIdx]:
+    for s in [sdata["snps"][i] for i in mySnpIdx]:
         dataset.addSnp(s.name)
-        dataset.snp[s.name].initAlleles(s.alleles[0],s.alleles[1])
-    for iind,ind in enumerate(idata):
-        dataset.addIndividual(pop=ind[0],
-                              ID=ind[1]+'.1',
-                              fatherID=ind[2],
-                              motherID=ind[3],
-                              sex=ind[4],
-                              phenotype=ind[5])
-        dataset.addIndividual(pop=ind[0],
-                              ID=ind[1]+'.2',
-                              fatherID=ind[2],
-                              motherID=ind[3],
-                              sex=ind[4],
-                              phenotype=ind[5])
-        dataset.Data[2*iind  ,:]=np.array( [ 2*hdata[s][2*iind] for s in mySnpIdx], dtype=np.int)
-        dataset.Data[2*iind+1,:]=np.array( [ 2*hdata[s][2*iind+1] for s in mySnpIdx], dtype=np.int)
-    return {'dataset':dataset, 'map': sdata['map']}
+        dataset.snp[s.name].initAlleles(s.alleles[0], s.alleles[1])
+    for iind, ind in enumerate(idata):
+        dataset.addIndividual(
+            pop=ind[0],
+            ID=ind[1] + ".1",
+            fatherID=ind[2],
+            motherID=ind[3],
+            sex=ind[4],
+            phenotype=ind[5],
+        )
+        dataset.addIndividual(
+            pop=ind[0],
+            ID=ind[1] + ".2",
+            fatherID=ind[2],
+            motherID=ind[3],
+            sex=ind[4],
+            phenotype=ind[5],
+        )
+        dataset.Data[2 * iind, :] = np.array(
+            [2 * hdata[s][2 * iind] for s in mySnpIdx], dtype=int
+        )
+        dataset.Data[2 * iind + 1, :] = np.array(
+            [2 * hdata[s][2 * iind + 1] for s in mySnpIdx], dtype=int
+        )
+    return {"dataset": dataset, "map": sdata["map"]}
+
 
 ################ BED / BIM / FAM files #############################
 
-def parsePlinkBfile(prefix,noPheno=False,params=defaultParams,options=None):
-    fam=prefix+'.fam'
-    bim=prefix+'.bim'
-    bed=prefix+'.bed'
+
+def parsePlinkBfile(prefix, noPheno=False, params=defaultParams, options=None):
+    fam = prefix + ".fam"
+    bim = prefix + ".bim"
+    bed = prefix + ".bed"
     ## individual data
-    idata=parseFamFile(fam) ## options not implemented
-    ni=len(idata)
+    idata = parseFamFile(fam)  ## options not implemented
+    ni = len(idata)
     ### SNP data
-    sdata=parseBimFile(bim)
-    ns=len(sdata['snps'])
-    mySnpIdx=range(ns)
-    dataset=data.Dataset(prefix,nsnp=ns,nindiv=ni)
+    sdata = parseBimFile(bim)
+    ns = len(sdata["snps"])
+    mySnpIdx = range(ns)
+    dataset = data.Dataset(prefix, nsnp=ns, nindiv=ni)
     ## fill in SNP data
-    for s in [sdata['snps'][i] for i in mySnpIdx]:
+    for s in [sdata["snps"][i] for i in mySnpIdx]:
         dataset.addSnp(s.name)
-        dataset.snp[s.name].initAlleles(s.alleles[0],s.alleles[1])
+        dataset.snp[s.name].initAlleles(s.alleles[0], s.alleles[1])
     ## fill in indiv data
     for ind in idata:
-        dataset.addIndividual(pop=ind[0],
-                              ID=ind[1],
-                              fatherID=ind[2],
-                              motherID=ind[3],
-                              sex=ind[4],
-                              phenotype=ind[5])
-    fillBedData_fast(bed.encode(),dataset.Data)
-    return {'dataset':dataset,'map':sdata['map']}
+        dataset.addIndividual(
+            pop=ind[0], ID=ind[1], fatherID=ind[2], motherID=ind[3], sex=ind[4], phenotype=ind[5]
+        )
+    fillBedData_fast(bed.encode(), dataset.Data)
+    return {"dataset": dataset, "map": sdata["map"]}
+
 
-def parseFamFile(fileName,noPheno=False,params=defaultParams):
-    indiv_data=[]
+def parseFamFile(fileName, noPheno=False, params=defaultParams):
+    indiv_data = []
     with open(fileName) as f:
         for ligne in f:
-            buf=ligne.split()
+            buf = ligne.split()
             if noPheno:
-                phe=None
+                phe = None
             else:
-                phe=((buf[5]!=params['MissPheno']) and float(buf[5])) or None
-  
-            indiv_data.append([buf[0], \
-                               buf[1],  \
-                               ((buf[2]!=params['MissParent']) and buf[2]) or None, \
-                               ((buf[3]!=params['MissParent']) and buf[3]) or None, \
-                               (buf[4]!=params['MissSex'] and buf[4]) or None, \
-                                phe])
+                phe = ((buf[5] != params["MissPheno"]) and float(buf[5])) or None
+
+            indiv_data.append(
+                [
+                    buf[0],
+                    buf[1],
+                    ((buf[2] != params["MissParent"]) and buf[2]) or None,
+                    ((buf[3] != params["MissParent"]) and buf[3]) or None,
+                    (buf[4] != params["MissSex"] and buf[4]) or None,
+                    phe,
+                ]
+            )
     return indiv_data
 
+
 def parseBimFile(fileName):
-    SNPs=[]
-    myMap=data.Map()
+    SNPs = []
+    myMap = data.Map()
     with open(fileName) as f:
         for ligne in f:
-            buf=ligne.split()
+            buf = ligne.split()
             ## create SNP
-            myS=data.SNP(buf[1])
-            myS.alleles[0]=buf[4]
-            myS.alleles[1]=buf[5]
+            myS = data.SNP(buf[1])
+            myS.alleles[0] = buf[4]
+            myS.alleles[1] = buf[5]
             ## add marker to map
             try:
-                mychr=int(buf[0])
+                mychr = int(buf[0])
             except:
-                mychr=buf[0]
-            mychr=buf[0]
-            myMap.addMarker(M=buf[1],C=mychr,posG=float(buf[2]),posP=float(buf[3]))
+                mychr = buf[0]
+            mychr = buf[0]
+            myMap.addMarker(M=buf[1], C=mychr, posG=float(buf[2]), posP=float(buf[3]))
             SNPs.append(myS)
-    return {'snps':SNPs,'map':myMap}
+    return {"snps": SNPs, "map": myMap}
+
 
-def fillBedData_fast(fileName,DataMatrix):
-    n_indiv,n_snp=DataMatrix.shape
-    reader=_pgenlib.PgenReader(fileName,raw_sample_ct=n_indiv)
-    buf=np.empty(n_indiv,np.int8)
+def fillBedData_fast(fileName, DataMatrix):
+    n_indiv, n_snp = DataMatrix.shape
+    reader = pgenlib.PgenReader(fileName, raw_sample_ct=n_indiv)
+    buf = np.empty(n_indiv, dtype="int8")
     for isnp in range(n_snp):
-        reader.read(isnp,buf,0)
-        buf[buf==-9]=missing
-        DataMatrix[:,isnp]=buf
+        reader.read(isnp, buf, 0)
+        buf[buf == -9] = missing
+        DataMatrix[:, isnp] = buf
+
 
-def fillBedData_slow(fileName,DataMatrix,snpidx=None):
-    n_indiv,n_snp=DataMatrix.shape
+def fillBedData_slow(fileName, DataMatrix, snpidx=None):
+    n_indiv, n_snp = DataMatrix.shape
     ## use dict type for faster look up
     ## key index in total, val : index in DataMatrix
     if snpidx is None:
-        snpidx=dict([ (i,i) for i in range(n_snp)])
+        snpidx = dict([(i, i) for i in range(n_snp)])
     else:
-        snpidx=dict([ (s,i) for i,s in enumerate(snpidx)])
-    cur_snp=0
+        snpidx = dict([(s, i) for i, s in enumerate(snpidx)])
+    cur_snp = 0
     ## bit enumerator
     def bits(f):
         bytes = (ord(b) for b in f.read())
         for b in bytes:
             for i in range(8):
                 yield (b >> i) & 1
+
     ## bit pair to geno converter
     def bpair_2_geno(pair):
-        '''
+        """
         from plink doc
-        '''
-        if pair=='00':
+        """
+        if pair == "00":
             return 0
-        if pair=='11':
+        if pair == "11":
             return 2
-        if pair=='01':
+        if pair == "01":
             return 1
-        if pair=='10':
+        if pair == "10":
             return missing
+
     ## constants
-    target_magic='0011011011011000'
-    snp_major='10000000'    
-    indiv_major='00000000'
+    target_magic = "0011011011011000"
+    snp_major = "10000000"
+    indiv_major = "00000000"
     ### let's go
-    bed_stream=open(fileName, 'r')
-    magic=[]
-    f_mode=[]
-    i_major=0
-    i_minor=0
-    proceed_2_next_bit=False
-    bit_geno=[]
-    nbit=-1
+    bed_stream = open(fileName, "r")
+    magic = []
+    f_mode = []
+    i_major = 0
+    i_minor = 0
+    proceed_2_next_bit = False
+    bit_geno = []
+    nbit = -1
     for b in bits(bed_stream):
-        nbit+=1
+        nbit += 1
         ## Test for magic number
-        if nbit<16:
+        if nbit < 16:
             magic.append(str(b))
             continue
-        if nbit==16:
-            magic=''.join(magic)
-            if magic!=target_magic:
-                print('Not a bed file')
+        if nbit == 16:
+            magic = "".join(magic)
+            if magic != target_magic:
+                print("Not a bed file")
                 raise ValueError
         ## Find out packing mode
-        if nbit<24:
+        if nbit < 24:
             f_mode.append(str(b))
             continue
-        if nbit==24:
-            f_mode=''.join(f_mode)
-            if f_mode==snp_major:
-                pack_len=n_indiv 
-            elif f_mode==indiv_major:
-                pack_len=n_snp
+        if nbit == 24:
+            f_mode = "".join(f_mode)
+            if f_mode == snp_major:
+                pack_len = n_indiv
+            elif f_mode == indiv_major:
+                pack_len = n_snp
             else:
-                print('Cannot determine packing mode, abort')
+                print("Cannot determine packing mode, abort")
                 raise ValueError
         ## Now i>24, we are reading genotypes
         ## case where we just wait for next bit to start reading again
         if proceed_2_next_bit:
-            if nbit%8!=0:
+            if nbit % 8 != 0:
                 continue
             else:
-                proceed_2_next_bit=False
-        ## reading genotypes        
+                proceed_2_next_bit = False
+        ## reading genotypes
         bit_geno.append(str(b))
-        if nbit%2!=0:
+        if nbit % 2 != 0:
             ##assert len(bit_geno)==2
             ## print nbit,i_major,i_minor,bit_geno
-            geno=bpair_2_geno(''.join(bit_geno))
-            if f_mode==snp_major:
+            geno = bpair_2_geno("".join(bit_geno))
+            if f_mode == snp_major:
                 try:
-                    data_idx=snpidx[i_major]
-                    DataMatrix[i_minor,data_idx]=geno
+                    data_idx = snpidx[i_major]
+                    DataMatrix[i_minor, data_idx] = geno
                 except KeyError:
                     pass
             else:
                 try:
-                    data_idx=snpidx[i_minor]
-                    DataMatrix[i_major,data_idx]=geno
+                    data_idx = snpidx[i_minor]
+                    DataMatrix[i_major, data_idx] = geno
                 except KeyError:
                     pass
-            i_minor += 1 
-            bit_geno=[]
-        if i_minor==pack_len:
-            proceed_2_next_bit=True
-            i_minor=0
-            i_major+=1
-        
+            i_minor += 1
+            bit_geno = []
+        if i_minor == pack_len:
+            proceed_2_next_bit = True
+            i_minor = 0
+            i_major += 1
+
 
 ############################ Covariate Information Files ##################
 
 ## File Format
 
 ## Header :ID cov1_name cov2_name ...
 ## Indiv1/pop1 val1 val2 ...
 
 ## add parser options to read in covariate files
 def populate_covariate_args(parser):
-    ''' Add options to read covariates in option parser'''
-    covariate_args=parser.add_argument_group('Covariates','')
-    covariate_args.add_argument('--covar',dest='covar_file',metavar='FILE',default=None,
-                                help='File with available covariates. Use --cov or --qcov to include them in the analysis')
-    covariate_args.add_argument('--cov',metavar='LIST',dest='cov',default=[],
-                                help='List of *qualitative* covariates to include, separated by commas')
-    covariate_args.add_argument('--qcov',metavar='LIST',dest='qcov',default=[],
-                                help='List of *quantitative*  covariates to include, separated by commas')
-    covariate_args.add_argument('--delim',metavar='DELIMITER',dest='delim',default=',',
-                                help='Delimiter used in covariates file')
+    """Add options to read covariates in option parser"""
+    covariate_args = parser.add_argument_group("Covariates", "")
+    covariate_args.add_argument(
+        "--covar",
+        dest="covar_file",
+        metavar="FILE",
+        default=None,
+        help="File with available covariates. Use --cov or --qcov to include them in the analysis",
+    )
+    covariate_args.add_argument(
+        "--cov",
+        metavar="LIST",
+        dest="cov",
+        default="",
+        help="List of *qualitative* covariates to include, separated by commas",
+    )
+    covariate_args.add_argument(
+        "--qcov",
+        metavar="LIST",
+        dest="qcov",
+        default="",
+        help="List of *quantitative*  covariates to include, separated by commas",
+    )
 
-def get_covariates_raw(fichier,missing_value='NA',delim=","):
-    ''' Get raw data from covariate file /fichier/
+
+def get_covariates_raw(fichier, missing_value="NA"):
+    """Get raw data from covariate file /fichier/
 
     File Format:
     Header     : ID cov1_name cov2_name ...
     Other lines: ID1 val1_1 val1_2 ...
 
     Returns a dictionary with covariate names as keys (read from header)
     For each covariate, the value is a dictionary with IDs as keys and string as value
     No conversion is done. Missing value key can be specified (default = NA)
-    '''
-    f=open(fichier)
-    covar_dat=f.readlines()
-    covar_name=covar_dat[0].strip().split(delim)[1:]
-    covariates={}
+    """
+    f = open(fichier)
+    covar_dat = f.readlines()
+    covar_name = covar_dat[0].split()[1:]
+    covariates = {}
     for nom in covar_name:
-        covariates[nom]={}
+        covariates[nom] = {}
     for ligne in covar_dat[1:]:
-        buf=ligne.strip().split(delim)
-        indiv=buf[0]
-        for i,covar in enumerate(covar_name):
-            if buf[i+1]==missing_value:
+        buf = ligne.split()
+        indiv = buf[0]
+        for i, covar in enumerate(covar_name):
+            if buf[i + 1] == missing_value:
                 continue
-            covariates[covar][indiv]=buf[i+1]## no conversion done here
+            covariates[covar][indiv] = buf[i + 1]  ## no conversion done here
     return covariates
 
-def get_covariates_matrix(filename,fact_names,qcov_names,names,stdize=True):
-    ''' 
-    Returns a design matrix of all covariates listed in fact_names and qcov_names. 
+
+def get_covariates_matrix(filename, fact_names, qcov_names, names, stdize=True):
+    """
+    Returns a design matrix of all covariates listed in fact_names and qcov_names.
     fact_names, qcov_names: string of qualitative (resp. quantitative) covariates, separated by commas.
     names : list of ID names providing the required ordering of rows.
     stdize : if True, standardize quantitative covariates (X-m)/s.
 
     Returns a dictionary with keys:
     -- DesignMatrices: dict with covar names as keys and DM as value
     -- levels: dict with cofact names as keys and ordered levels as value
-    '''
-    covariates=get_covariates_raw(filename)
-    cofact=[] ## qualitative cofactors
-    covar=[] ## quantitative covariables
-    nids=len(names)
+    """
+    covariates = get_covariates_raw(filename)
+    cofact = []  ## qualitative cofactors
+    covar = []  ## quantitative covariables
+    nids = len(names)
     try:
-        for c in fact_names.split(','):
-            if c!='':
+        for c in fact_names.split(","):
+            if c != "":
                 if c in covariates:
                     cofact.append(c)
                 else:
-                    print( 'Covariate %s not found in covariate file, ignoring.'%c)
+                    print("Covariate %s not found in covariate file, ignoring." % c)
     except:
         pass
     try:
-        for c in qcov_names.split(','):
-            if c!='':
+        for c in qcov_names.split(","):
+            if c != "":
                 if c in covariates:
                     covar.append(c)
                 else:
-                    print( 'Covariate %s not found in covariate file, ignoring.'%c)
+                    print("Covariate %s not found in covariate file, ignoring." % c)
     except:
         pass
-    Matrices={}
-    levels={}
+    Matrices = {}
+    levels = {}
     for q in cofact:
-        q_vec=[]
+        q_vec = []
         for nom in names:
             q_vec.append(covariates[q][nom])
-        u,aa=np.unique(q_vec,return_inverse=True)
-        print( 'Cofactor "%s" with %d levels'%(q,len(u)))
-        print( 'Levels:',*u)
-        levels[q]=u
-        M=np.zeros((nids,len(u)),dtype=np.int)
-        M[range(nids),aa]=1
-        Matrices[q]=M[:,1:]
+        u, aa = np.unique(q_vec, return_inverse=True)
+        print('Cofactor "%s" with %d levels' % (q, len(u)))
+        print("Levels:" * u)
+        levels[q] = u
+        M = np.zeros((nids, len(u)), dtype=int)
+        M[range(nids), aa] = 1
+        Matrices[q] = M[:, 1:]
     for q in covar:
-        M=np.zeros((nids,1),dtype=np.float)
-        for i,nom in enumerate(names):
+        M = np.zeros((nids, 1), dtype=float)
+        for i, nom in enumerate(names):
             try:
-                val=float(covariates[q][nom])
-                M[i,0]=val
+                val = float(covariates[q][nom])
+                M[i, 0] = val
             except ValueError:
-                raise ValueError('Covariate %s is not quantitative !'%q)
-        mu=np.mean(M)
-        ss=np.std(M)
+                raise ValueError("Covariate %s is not quantitative !" % q)
+        mu = np.mean(M)
+        ss = np.std(M)
         if stdize:
-            M=(M-mu)/ss
-        print( 'Covariate "%s" with mean %f and sd %f'%(q,mu,ss))
-        Matrices[q]=M
-    return { 'cofactors' : cofact,
-                 'covariables' : covar,
-                 "DesignMatrices":Matrices,
-                 "factor_levels":levels}
+            M = (M - mu) / ss
+        print('Covariate "%s" with mean %f and sd %f' % (q, mu, ss))
+        Matrices[q] = M
+    return {
+        "cofactors": cofact,
+        "covariables": covar,
+        "DesignMatrices": Matrices,
+        "factor_levels": levels,
+    }
```

### Comparing `hapflk-2.0.dev2/hapflk/data.py` & `hapflk-2.1/hapflk/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,784 +1,884 @@
 ##from __future__ import division
 from operator import itemgetter
 from bisect import *
 import sys
 import numpy as np
+
 ##import numpy.ma as ma
 from hapflk import missing, complete_cases, is_na
 
-zero=np.int16(0)
-un=np.int16(1)
-deux=np.int16(2)
-
-class Dataset():
-    def __init__(self,fileName,nsnp,nindiv):
-        self.name=fileName
+zero = np.int16(0)
+un = np.int16(1)
+deux = np.int16(2)
+
+
+class Dataset:
+    def __init__(self, fileName, nsnp, nindiv):
+        self.name = fileName
         ## Individuals
-        self.nindiv=nindiv
-        self.iindiv=0
-        self.indiv={}
+        self.nindiv = nindiv
+        self.iindiv = 0
+        self.indiv = {}
         ## Individual index in Data Matrix
-        self.indivIdx={}
+        self.indivIdx = {}
         ## SNPs
-        self.nsnp=nsnp
-        self.isnp=0
-        self.snp={}
+        self.nsnp = nsnp
+        self.isnp = 0
+        self.snp = {}
         ## SNP indices in Data Matrix
-        self.snpIdx={}
+        self.snpIdx = {}
         self._initDataMatrix()
         ## populations
         ## populations are accessed by a name (key of the dict)
         ## the value is a vector of booleans taking a True value for individuals
         ## belonging to the pop otherwise
         ## These vectors can be used for fast access to population genotypes e.g.:
         ## vpop=self.populations['mypop']
         ## mypop_genotypes=self.Data[vpop,]
-        self.populations={}
-    def addSnp(self,Name):
-        ''' Add a snp to the dataset '''
+        self.populations = {}
+
+    def addSnp(self, Name):
+        """Add a snp to the dataset"""
         if Name in self.snp:
             return
-        self.snp[Name]=SNP(Name)
-        self.snpIdx[Name]=self.isnp
-        self.isnp+=1
-    def rmSnp(self,Name):
-        ''' 
-        Remove a snp from the dataset 
+        self.snp[Name] = SNP(Name)
+        self.snpIdx[Name] = self.isnp
+        self.isnp += 1
+
+    def rmSnp(self, Name):
+        """
+        Remove a snp from the dataset
         The SNP is made unaccessible but the data stay in the Data Matrix
-        '''
+        """
         if not Name in self.snp:
             return
         else:
             del self.snp[Name]
             del self.snpIdx[Name]
             del self._allSnps
-    def addIndividual(self,ID,pop=None,sex=None,fatherID=None,motherID=None,phenotype=None):
-        ''' Add an individual to the dataset'''
+
+    def addIndividual(self, ID, pop=None, sex=None, fatherID=None, motherID=None, phenotype=None):
+        """Add an individual to the dataset"""
         if ID in self.indiv:
-            print( "Warning: Individual ",ID," has been seen before !")
+            print("Warning: Individual ", ID, " has been seen before !")
             return
-        self.indiv[ID]=Individual(ID,pop,sex,fatherID,motherID,phenotype)
-        self.indivIdx[ID]=self.iindiv
+        self.indiv[ID] = Individual(ID, pop, sex, fatherID, motherID, phenotype)
+        self.indivIdx[ID] = self.iindiv
         if pop is not None:
             try:
-                vpop=self.populations[pop]
+                vpop = self.populations[pop]
             except KeyError:
-                vpop=np.array([0]*self.nindiv,dtype=bool)
-                self.populations[pop]=vpop
-            vpop[self.iindiv]=True
-        self.iindiv+=1
+                vpop = np.array([0] * self.nindiv, dtype=bool)
+                self.populations[pop] = vpop
+            vpop[self.iindiv] = True
+        self.iindiv += 1
+
     def _initDataMatrix(self):
-        ''' Initialize Data Matrix to an int16 array filled with -1'''
-        self.Data=-np.ones(shape=(self.nindiv,self.nsnp),dtype='int16')
-    def IndivGenotype(self,indiv,snps=None):
-        '''
+        """Initialize Data Matrix to an int16 array filled with -1"""
+        self.Data = -np.ones(shape=(self.nindiv, self.nsnp), dtype="int16")
+
+    def IndivGenotype(self, indiv, snps=None):
+        """
         Return (0,1,2) genotype of individual INDIV at all SNPs in the dataset
-        '''
+        """
         try:
-            i=self.indivIdx[indiv]
+            i = self.indivIdx[indiv]
         except KeyError:
-            print( 'Individual',indiv,'not in Data')
+            print("Individual", indiv, "not in Data")
             raise
         if snps is None:
-            return [ (x<0 and missing) or x for x in  self.Data[i,]]
+            return [
+                (x < 0 and missing) or x
+                for x in self.Data[
+                    i,
+                ]
+            ]
         else:
-            return [ (x<0 and missing) or x for x in self.Data[i,[self.snpIdx[s] for s in snps]]]
-    def IndivGenotype_char(self,indiv,snps=None):
-        igeno=self.IndivGenotype(indiv,snps)
-        cgeno=[]
+            return [(x < 0 and missing) or x for x in self.Data[i, [self.snpIdx[s] for s in snps]]]
+
+    def IndivGenotype_char(self, indiv, snps=None):
+        igeno = self.IndivGenotype(indiv, snps)
+        cgeno = []
         if snps is None:
-            snps=self.AllSnps()
-        for i,s in enumerate(snps):
-            cgeno.append(self.Alleles(igeno[i],s))
+            snps = self.AllSnps()
+        for i, s in enumerate(snps):
+            cgeno.append(self.Alleles(igeno[i], s))
         return cgeno
+
     def AllSnps(self):
         try:
             return self._allSnps
         except AttributeError:
-            self._allSnps=sorted(self.snp,key=lambda x: self.snpIdx[x])
+            self._allSnps = sorted(self.snp, key=lambda x: self.snpIdx[x])
         return self._allSnps
-    def SnpGenotype(self,snp):
-        '''
+
+    def SnpGenotype(self, snp):
+        """
         Return genotype of snp SNP for all individuals in the dataset
-        '''
+        """
         try:
-            j=self.snpIdx[snp]
+            j = self.snpIdx[snp]
         except KeyError:
-            return [missing]*self.nindiv
-        return [ (x<0 and missing) or x for x in self.Data[:,j]]
-    def Alleles(self,geno,snp):
-        '''
+            return [missing] * self.nindiv
+        return [(x < 0 and missing) or x for x in self.Data[:, j]]
+
+    def Alleles(self, geno, snp):
+        """
         Return the alleles corresponding to genotype GENO at snp SNP
-        '''
+        """
         if geno is missing:
-            return ('?','?')
-        snpAll=self.snp[snp].alleles
-        if geno==0:
-            return (snpAll[0],snpAll[0])
-        elif geno==1:
-            return (snpAll[0],snpAll[1])
+            return ("?", "?")
+        snpAll = self.snp[snp].alleles
+        if geno == 0:
+            return (snpAll[0], snpAll[0])
+        elif geno == 1:
+            return (snpAll[0], snpAll[1])
         else:
-            assert geno==2
-            return (snpAll[1],snpAll[1])
-    def Genotype(self,indiv,snp):
-        '''
-        Return the genotype of individual INDIV  at snp SNP 
+            assert geno == 2
+            return (snpAll[1], snpAll[1])
+
+    def Genotype(self, indiv, snp):
+        """
+        Return the genotype of individual INDIV  at snp SNP
         If SNP is not found in the dataset, returns 'missing'
-        '''
+        """
         try:
-            i=self.indivIdx[indiv]
+            i = self.indivIdx[indiv]
         except KeyError:
-            print( 'Individual',indiv,'not in Data')
+            print("Individual", indiv, "not in Data")
             raise
         try:
-            j=self.snpIdx[snp]
+            j = self.snpIdx[snp]
         except KeyError:
             return missing
-        return self.Data[i,j]<0 and missing or self.Data[i,j]
-    def SetGenotypeSlow(self,indiv,snp,value):
-        '''
+        return self.Data[i, j] < 0 and missing or self.Data[i, j]
+
+    def SetGenotypeSlow(self, indiv, snp, value):
+        """
         Set the genotype of individual INDIV at snp SNP to value VALUE
         Correct Genotype is a value of length 2, with alleles matching the SNP
-        '''
+        """
         try:
-            i=self.indivIdx[indiv]
+            i = self.indivIdx[indiv]
         except KeyError:
-            print( 'Individual',indiv,'not in Data')
+            print("Individual", indiv, "not in Data")
             raise
         try:
-            j=self.snpIdx[snp]
+            j = self.snpIdx[snp]
         except KeyError:
-            print( 'SNP',snp,'not in Data')
+            print("SNP", snp, "not in Data")
             raise
-        if self.Data[i,j] > -1:
-            self.snp[snp].delGenotype(self.Data[i,j])
-        geno=self.snp[snp].addObservation(value)
+        if self.Data[i, j] > -1:
+            self.snp[snp].delGenotype(self.Data[i, j])
+        geno = self.snp[snp].addObservation(value)
         if geno is not missing:
-            self.indiv[indiv].callrate+=1
-        self.Data[i,j]=geno
-    def SetGenotype(self,indiv,snp,value):
-        '''
-        Fast Version of SetGenotype with no checking for errors 
+            self.indiv[indiv].callrate += 1
+        self.Data[i, j] = geno
+
+    def SetGenotype(self, indiv, snp, value):
+        """
+        Fast Version of SetGenotype with no checking for errors
         Use with caution
         --
         Set the genotype of individual INDIV at snp SNP to value VALUE
         Correct Genotype is a value of length 2, with alleles matching the SNP
-        '''
+        """
         try:
-            i=self.indivIdx[indiv]
-            j=self.snpIdx[snp]
-            self.Data[i,j]=self.snp[snp].addObservation(value)     
+            i = self.indivIdx[indiv]
+            j = self.snpIdx[snp]
+            self.Data[i, j] = self.snp[snp].addObservation(value)
         except:
-            print( 'Error')
+            print("Error")
             raise
-    def printSNP(self,stream=sys.stdout):
-        '''
+
+    def printSNP(self, stream=sys.stdout):
+        """
         Print SNP information
-        '''
-        print( 'name\tA1\tA2\tcallRate', file = stream)
-        for sName in sorted(self.snp,key=lambda x:self.snpIdx[x]):
-            geno=self.SnpGenotype(sName)
-            s=self.snp[sName]
-            print(s.name,s.alleles[0],s.alleles[1],np.mean([g is not missing for g in geno]), file = stream)
+        """
+        print("name\tA1\tA2\tcallRate", file=stream)
+        for sName in sorted(self.snp, key=lambda x: self.snpIdx[x]):
+            geno = self.SnpGenotype(sName)
+            s = self.snp[sName]
+            print(
+                s.name,
+                s.alleles[0],
+                s.alleles[1],
+                np.mean([g is not missing for g in geno]),
+                file=stream,
+            )
+
     ##### PEDIGREE AND FAMILIES
     def BuildPedigree(self):
-        '''
+        """
         Construct the pedigree relationships between individuals in the dataset
         Identify founders and parent-offspring links
-        '''
-        self.pedigree=Pedigree(self.indiv.values())
-        self.founders=np.array([0]*self.nindiv,dtype=bool)
+        """
+        self.pedigree = Pedigree(self.indiv.values())
+        self.founders = np.array([0] * self.nindiv, dtype=bool)
         for guy in self.indiv.values():
-            founder=True
-            if self.pedigree.setFather(guy,guy.fatherID):
-                founder=False
-            if self.pedigree.setMother(guy,guy.motherID):
-                founder=False
+            founder = True
+            if self.pedigree.setFather(guy, guy.fatherID):
+                founder = False
+            if self.pedigree.setMother(guy, guy.motherID):
+                founder = False
             if founder:
                 self.pedigree.founders.append(guy)
-                self.founders[self.indivIdx[guy.id]]=True
+                self.founders[self.indivIdx[guy.id]] = True
+
     def BuildFamilies(self):
-        '''
+        """
         Cluster related individuals in families
         Sets the self.families attribute to a list of the families
-        '''
+        """
         try:
-            ped=self.pedigree
+            ped = self.pedigree
         except AttributeError:
             self.BuildPedigree()
-            ped=self.pedigree
+            ped = self.pedigree
         ped.BuildFamilies()
-        self.families=ped.families
+        self.families = ped.families
+
     def UnrelatedIndividuals(self):
         try:
-            ped=self.pedigree
+            ped = self.pedigree
         except AttributeError:
             self.BuildPedigree()
-            ped=self.pedigree
+            ped = self.pedigree
         return ped.UnrelatedIndividuals()
+
     def NuclearFamilies(self):
-        '''
+        """
         Generator that yields all nuclear families in the dataset (with both parents present)
-        '''
+        """
         try:
-            allFams=self.families
+            allFams = self.families
         except AttributeError:
             self.BuildFamilies()
-            allFams=self.families
+            allFams = self.families
         for fam in allFams:
             for nucFam in fam.NuclearFamilies():
                 yield nucFam
-    
+
     def HalfSibFamilies(self):
-        '''
+        """
         Generator that yields all half-sib families in the dataset.
-        '''
+        """
         try:
-            allFams=self.families
+            allFams = self.families
         except AttributeError:
             self.BuildFamilies()
-            allFams=self.families
+            allFams = self.families
         for fam in allFams:
             for hsFam in fam.HalfSibFamilies():
                 yield hsFam
-    
-    def checkSegregation(self,autosome=True,sex_type='XY'):
+
+    def checkSegregation(self, autosome=True, sex_type="XY"):
         # if not autosome:
         #     if sex_type=='XY':
         #         return self.checkSegregationXY()
         #     elif sex_type=='ZW':
         #         return self.checkSegregationZW()
         try:
-            allFams=self.families
+            allFams = self.families
         except AttributeError:
             self.BuildFamilies()
-            allFams=self.families
-        self.MendelErrors={}
+            allFams = self.families
+        self.MendelErrors = {}
         for fam in allFams:
             for node in fam.nonFounders:
-                o=node.indiv
+                o = node.indiv
                 ## father <-> offspring
-                if (autosome or sex_type=='ZW') and node.father is not None:
-                    father=node.father.indiv
+                if (autosome or sex_type == "ZW") and node.father is not None:
+                    father = node.father.indiv
                     for snp in self.AllSnps():
-                        go=self.Genotype(o.id,snp)
-                        gf=self.Genotype(father.id,snp)
+                        go = self.Genotype(o.id, snp)
+                        gf = self.Genotype(father.id, snp)
                         if go is missing or gf is missing:
                             continue
-                        if (go==0 and gf==2) or (go==2 and gf==0):
+                        if (go == 0 and gf == 2) or (go == 2 and gf == 0):
                             try:
-                                self.SetGenotype(o.id,snp,missing)
-                                self.SetGenotype(father.id,snp,missing)
+                                self.SetGenotype(o.id, snp, missing)
+                                self.SetGenotype(father.id, snp, missing)
                             except:
-                                print( o.id,father.id,go,gf)
-                                
-                            try :
-                                self.MendelErrors[snp]+=1
+                                print(o.id, father.id, go, gf)
+
+                            try:
+                                self.MendelErrors[snp] += 1
                             except KeyError:
-                                self.MendelErrors[snp]=1
-                            try :
-                                self.MendelErrors[o.id]+=1
+                                self.MendelErrors[snp] = 1
+                            try:
+                                self.MendelErrors[o.id] += 1
                             except KeyError:
-                                self.MendelErrors[o.id]=1
-                            try :
-                                self.MendelErrors[father.id]+=1
+                                self.MendelErrors[o.id] = 1
+                            try:
+                                self.MendelErrors[father.id] += 1
                             except KeyError:
-                                self.MendelErrors[father.id]=1
+                                self.MendelErrors[father.id] = 1
                 ## mother <-> offspring
-                if (autosome or sex_type=='XY') and node.mother is not None:
-                    mother=node.mother.indiv
+                if (autosome or sex_type == "XY") and node.mother is not None:
+                    mother = node.mother.indiv
                     for snp in self.AllSnps():
-                        go=self.Genotype(o.id,snp)
-                        gm=self.Genotype(mother.id,snp)
+                        go = self.Genotype(o.id, snp)
+                        gm = self.Genotype(mother.id, snp)
                         if go is missing or gm is missing:
                             continue
-                        if (go==0 and gm==2) or (go==2 and gm==0):
-                            self.SetGenotype(o.id,snp,missing)
-                            self.SetGenotype(mother.id,snp,missing)
-                            try :
-                                self.MendelErrors[snp]+=1
+                        if (go == 0 and gm == 2) or (go == 2 and gm == 0):
+                            self.SetGenotype(o.id, snp, missing)
+                            self.SetGenotype(mother.id, snp, missing)
+                            try:
+                                self.MendelErrors[snp] += 1
                             except KeyError:
-                                self.MendelErrors[snp]=1
-                            try :
-                                self.MendelErrors[o.id]+=1
+                                self.MendelErrors[snp] = 1
+                            try:
+                                self.MendelErrors[o.id] += 1
                             except KeyError:
-                                self.MendelErrors[o.id]=1
-                            try :
-                                self.MendelErrors[mother.id]+=1
+                                self.MendelErrors[o.id] = 1
+                            try:
+                                self.MendelErrors[mother.id] += 1
                             except KeyError:
-                                self.MendelErrors[mother.id]=1
+                                self.MendelErrors[mother.id] = 1
         return self.MendelErrors
+
     ### POPULATION GENETICS methods
-    def compute_pop_frq(self,verbose=True):
-        '''
+    def compute_pop_frq(self, verbose=True):
+        """
         Compute allele frequencies for each population in the dataset, considering only
          founders.
-        '''
+        """
         try:
-            fvec=self.founders
+            fvec = self.founders
         except AttributeError:
             self.BuildPedigree()
-            fvec=self.founders
-        pop_names=[]
-        frqs=[]
+            fvec = self.founders
+        pop_names = []
+        frqs = []
         ## identify missing markers
-        wtot = np.ones( self.Data.shape[1], dtype=np.bool)
-        for pname,pvec in self.populations.items():
-            pop_founders = pvec&fvec
+        wtot = np.ones(self.Data.shape[1], dtype=bool)
+        for pname, pvec in self.populations.items():
+            pop_founders = pvec & fvec
             ##w = complete_cases(self.Data[pop_founders,])
-            w = self.Data[pop_founders,] != missing
-            wbar = np.sum( w, axis = 0)
-            nmiss = np.sum(wbar==0)
+            w = (
+                self.Data[
+                    pop_founders,
+                ]
+                != missing
+            )
+            wbar = np.sum(w, axis=0)
+            nmiss = np.sum(wbar == 0)
             ##if np.min( wbar) == 0:
-            if nmiss >0 :
-                print( '\t%16s: %d individuals, %d SNPs with no info'%(pname, sum(pvec),nmiss))
+            if nmiss > 0:
+                print("\t%16s: %d individuals, %d SNPs with no info" % (pname, sum(pvec), nmiss))
             wtot &= wbar > 0
-        print( '\tFound %d SNPs with info on all pops'%(np.sum(wtot!=0)))
+        print("\tFound %d SNPs with info on all pops" % (np.sum(wtot != 0)))
         ## Compute allele frequencies
-        for pname,pvec in self.populations.items():
-            print('\t %16s'%pname)
-            pop_founders = pvec&fvec
-            w = complete_cases(self.Data[pop_founders,])
-            ff = np.zeros( self.Data.shape[1], dtype=np.float)
-            subw = w[:,wtot]
-            subdata = self.Data[pop_founders,][:,wtot]
+        for pname, pvec in self.populations.items():
+            print("\t %16s" % pname)
+            pop_founders = pvec & fvec
+            w = complete_cases(
+                self.Data[
+                    pop_founders,
+                ]
+            )
+            ff = np.zeros(self.Data.shape[1], dtype=float)
+            subw = w[:, wtot]
+            subdata = self.Data[
+                pop_founders,
+            ][:, wtot]
             ##
-            ff[ wtot ] = 0.5*np.average( subdata, axis=0, weights=subw)
+            ff[wtot] = 0.5 * np.average(subdata, axis=0, weights=subw)
             ## using mean
-            ff[ wtot ] = 0.5*np.mean(subdata*subw,axis=0)/np.mean(subw,axis=0)
+            ff[wtot] = 0.5 * np.mean(subdata * subw, axis=0) / np.mean(subw, axis=0)
             subset = wtot == 0
-            ff[ subset ] = np.ma.masked
+            ff[subset] = np.ma.masked
             frqs.append(ff)
             pop_names.append(pname)
         print()
-        return {"pops":tuple(pop_names),'freqs':np.vstack(frqs)}
-   
-class Family():
-    def __init__(self,founders=[],nonFounders=[]):
-        self.founders=founders
-        self.nonFounders=nonFounders
+        return {"pops": tuple(pop_names), "freqs": np.vstack(frqs)}
+
+
+class Family:
+    def __init__(self, founders=[], nonFounders=[]):
+        self.founders = founders
+        self.nonFounders = nonFounders
+
     def __str__(self):
-        tw='Founders: '+'x'.join([x.indiv.id for x in self.founders])+' with '+str(len(self.nonFounders))+' offspring'
+        tw = (
+            "Founders: "
+            + "x".join([x.indiv.id for x in self.founders])
+            + " with "
+            + str(len(self.nonFounders))
+            + " offspring"
+        )
         return tw
-    def addFounder(self,founder):
-        ''' Add a node to the founders '''
+
+    def addFounder(self, founder):
+        """Add a node to the founders"""
         if founder not in self.founders:
             self.founders.append(founder)
-    def addNonFounders(self,offspring):
-        ''' Add a list of nodes to the offspring '''
+
+    def addNonFounders(self, offspring):
+        """Add a list of nodes to the offspring"""
         if offspring not in self.nonFounders:
             self.nonFounders.append(offspring)
+
     def NuclearFamilies(self):
-        '''
-            Build Nuclear Families within an extended pedigree (family)
-            Family founders are ordered so that fam.founders[0] is dad
-        '''
-        FSfam=[]
-        children=list(self.nonFounders)
-        while len(children)>0:
-            firstFS=children[0]
-            papa=firstFS.father
-            maman=firstFS.mother
+        """
+        Build Nuclear Families within an extended pedigree (family)
+        Family founders are ordered so that fam.founders[0] is dad
+        """
+        FSfam = []
+        children = list(self.nonFounders)
+        while len(children) > 0:
+            firstFS = children[0]
+            papa = firstFS.father
+            maman = firstFS.mother
             if papa is not None and maman is not None:
-                enfants=[off for off in children if off.father==papa and off.mother==maman]
-                FSfam.append(Family(founders=[papa,maman],nonFounders=enfants))
+                enfants = [off for off in children if off.father == papa and off.mother == maman]
+                FSfam.append(Family(founders=[papa, maman], nonFounders=enfants))
                 for off in enfants:
                     children.remove(off)
             else:
                 children.remove(firstFS)
         return FSfam
-    def _rmHiddenFullSibs(self,enfants,fatherConnected=True):
-        '''
+
+    def _rmHiddenFullSibs(self, enfants, fatherConnected=True):
+        """
         remove "hidden" full sibs from a set of individuals (i.e.
-        have same motherID (fatherConnected=True) 
+        have same motherID (fatherConnected=True)
         or fatherID (fatherConnected=False))
-        '''
-        keepThem=[]
-        trashThem=[]
-        otherParents={}
+        """
+        keepThem = []
+        trashThem = []
+        otherParents = {}
         ## make sure we consider enfants always in the same order
-        enfants=sorted(enfants,key=lambda x:x.indiv.id)
-        for node in sorted(enfants,key=lambda x:x.indiv.callrate,reverse=True):
-            guy=node.indiv
+        enfants = sorted(enfants, key=lambda x: x.indiv.id)
+        for node in sorted(enfants, key=lambda x: x.indiv.callrate, reverse=True):
+            guy = node.indiv
             if fatherConnected:
-                otherID=guy.motherID
+                otherID = guy.motherID
             else:
-                otherID=guy.fatherID
+                otherID = guy.fatherID
             try:
                 # we have encountered a full sib before
                 # we don't keep that guy
-                otherParents[otherID]+=1
+                otherParents[otherID] += 1
                 trashThem.append(node)
             except KeyError:
-                otherParents[otherID]=1
+                otherParents[otherID] = 1
                 keepThem.append(node)
-        return keepThem,trashThem
-                    
+        return keepThem, trashThem
+
     def HalfSibFamilies(self):
-        '''
+        """
         Return HalfSib Families contained in the family
-        '''
-        HSfam=[]
-        children=list(self.nonFounders)
-        while len(children)>0:
-            firstHS=children[0]
-            papa=firstHS.father
-            maman=firstHS.mother
+        """
+        HSfam = []
+        children = list(self.nonFounders)
+        while len(children) > 0:
+            firstHS = children[0]
+            papa = firstHS.father
+            maman = firstHS.mother
             if papa is not None:
                 if maman is None:
                     ## be sure all of them have none mothers
-                    enfants=[off for off in children if off.father==papa and off.mother is None]
+                    enfants = [off for off in children if off.father == papa and off.mother is None]
                     for off in enfants:
                         children.remove(off)
                     ## remove hidden FS
                     ##enfants,rmvd=self._rmHiddenFullSibs(enfants)
-                    HSfam.append(Family(founders=[papa],nonFounders=enfants))
+                    HSfam.append(Family(founders=[papa], nonFounders=enfants))
                 else:
                     ## nuclear family: remove everyone
-                    enfants=[off for off in children if off.father==papa and off.mother==maman]
+                    enfants = [
+                        off for off in children if off.father == papa and off.mother == maman
+                    ]
                     for off in enfants:
                         children.remove(off)
             elif maman is not None:
                 ## father is None
-                enfants=[off for off in children if off.mother==maman and off.father is None]
+                enfants = [off for off in children if off.mother == maman and off.father is None]
                 for off in enfants:
                     children.remove(off)
                 ## remove hidden FS
                 ##enfants,rmvd=self._rmHiddenFullSibs(enfants,fatherConnected=False)
-                HSfam.append(Family(founders=[maman],nonFounders=enfants))
+                HSfam.append(Family(founders=[maman], nonFounders=enfants))
             else:
                 children.remove(firstHS)
         return HSfam
-    
-    
-class Pedigree():
-    ''' Pedigree relationships between individuals'''
-    def __init__(self,guys=[]):
-        self.nodes={}
-        self.founders=[]
-        self.families=[]
+
+
+class Pedigree:
+    """Pedigree relationships between individuals"""
+
+    def __init__(self, guys=[]):
+        self.nodes = {}
+        self.founders = []
+        self.families = []
         for guy in guys:
             self.addNode(guy)
-    def addNode(self,guy):
-        ''' Add a new guy to the pedigree'''
-        self.nodes[guy.id]=PedNode(guy)
-    def setFather(self,son,dadID):
-        ''' 
-        Set that dadId is dad of sonId 
+
+    def addNode(self, guy):
+        """Add a new guy to the pedigree"""
+        self.nodes[guy.id] = PedNode(guy)
+
+    def setFather(self, son, dadID):
+        """
+        Set that dadId is dad of sonId
         return True if dad found
         return False if not found
         raise if sonID not found
-        '''
+        """
         if not son.id in self.nodes:
-            print( "Don't know that guy",son.id)
-            raise KeyError 
+            print("Don't know that guy", son.id)
+            raise KeyError
         try:
-            self.nodes[son.id].father=self.nodes[dadID]
+            self.nodes[son.id].father = self.nodes[dadID]
             self.nodes[dadID].children.append(self.nodes[son.id])
             return True
         except KeyError:
             return False
-    def setMother(self,son,momID):
-        ''' 
-        Set that momId is mom of sonId 
+
+    def setMother(self, son, momID):
+        """
+        Set that momId is mom of sonId
         return True if mom found
         return False if not found
         raise if sonID not found
-        '''
+        """
         if not son.id in self.nodes:
-            print( "Don't know that guy",sonId)
-            raise KeyError 
+            print("Don't know that guy", sonId)
+            raise KeyError
         try:
-            self.nodes[son.id].mother=self.nodes[momID]
+            self.nodes[son.id].mother = self.nodes[momID]
             self.nodes[momID].children.append(self.nodes[son.id])
             return True
         except KeyError:
-            return False    
-    def _getRelatives(self,node,connected):
+            return False
+
+    def _getRelatives(self, node, connected):
         if node in connected:
             return
         connected.append(node)
         for off in [x for x in node.children]:
-            self._getRelatives(off,connected)
-        if node.father!=None:
-            self._getRelatives(node.father,connected)
-        if node.mother!=None and node.mother not in connected:
-            self._getRelatives(node.mother,connected)
+            self._getRelatives(off, connected)
+        if node.father != None:
+            self._getRelatives(node.father, connected)
+        if node.mother != None and node.mother not in connected:
+            self._getRelatives(node.mother, connected)
+
     def UnrelatedIndividuals(self):
-        return [x.id for x in self.founders if len(self.nodes[x.id].children)==0]
+        return [x.id for x in self.founders if len(self.nodes[x.id].children) == 0]
+
     def BuildFamilies(self):
-        '''
+        """
         Cluster individuals by families
-        '''
-        founders2go=[self.nodes[x.id] for x in self.founders[:]]
-        offspring2go=list(set(self.nodes.values())-(set(founders2go)&set(self.nodes.values())))
-        while len(founders2go)>0:
-            relatives=[]
-            self._getRelatives(founders2go[0],relatives)
-            famFounders=[]
-            famNonFounders=[]
+        """
+        founders2go = [self.nodes[x.id] for x in self.founders[:]]
+        offspring2go = list(
+            set(self.nodes.values()) - (set(founders2go) & set(self.nodes.values()))
+        )
+        while len(founders2go) > 0:
+            relatives = []
+            self._getRelatives(founders2go[0], relatives)
+            famFounders = []
+            famNonFounders = []
             for x in relatives:
                 if x in founders2go:
                     famFounders.append(x)
                 else:
                     famNonFounders.append(x)
-            if len(famNonFounders)>0:
-                self.families.append(Family(founders=famFounders,nonFounders=famNonFounders))
+            if len(famNonFounders) > 0:
+                self.families.append(Family(founders=famFounders, nonFounders=famNonFounders))
             for x in famFounders:
                 founders2go.remove(x)
             for x in famNonFounders:
                 try:
                     offspring2go.remove(x)
                 except ValueError:
-                    print( 'pula',x.indiv.id)
+                    print("pula", x.indiv.id)
+
 
-class PedNode():
-    def __init__(self,indiv,father=None,mother=None):
-        self.indiv=indiv
-        self.father=father
-        self.mother=mother
-        self.children=[]
-    def addChild(self,child):
+class PedNode:
+    def __init__(self, indiv, father=None, mother=None):
+        self.indiv = indiv
+        self.father = father
+        self.mother = mother
+        self.children = []
+
+    def addChild(self, child):
         if child not in self.children:
             self.children.append(child)
-        
-class Individual():
-    def __init__(self,id,pop=None,sex=None,fatherID=None,motherID=None,phenotype=None):
-        self.id=id
-        self.pop=pop
-        self.sex=sex
-        self.fatherID=fatherID
-        self.motherID=motherID
-        self.phenotype=[phenotype]
-        self.callrate=0
-
-
-class SNP():
-    def __init__(self,Name):
-        self.name=Name
-        self.alleles=[None,None] ## maps 0,1 to alleles
-        self.mapping={} ## maps allele to 0,1
-        self.counts=np.zeros(3,dtype='int16') ## number(a1),number(a2),number(missing)
-        self.Gcounts=[0,0,0]
-        self.addObservation=self.addObservationNotFull
+
+
+class Individual:
+    def __init__(self, id, pop=None, sex=None, fatherID=None, motherID=None, phenotype=None):
+        self.id = id
+        self.pop = pop
+        self.sex = sex
+        self.fatherID = fatherID
+        self.motherID = motherID
+        self.phenotype = [phenotype]
+        self.callrate = 0
+
+
+class SNP:
+    def __init__(self, Name):
+        self.name = Name
+        self.alleles = [None, None]  ## maps 0,1 to alleles
+        self.mapping = {}  ## maps allele to 0,1
+        self.counts = np.zeros(3, dtype="int16")  ## number(a1),number(a2),number(missing)
+        self.Gcounts = [0, 0, 0]
+        self.addObservation = self.addObservationNotFull
+
     def callrate(self):
-        return 0.5*(self.counts[0]+self.counts[1])/(0.5*(self.counts[0]+self.counts[1])+self.counts[2])
-    def initAlleles(self,a1,a2):
-        self.alleles[0]=a1
-        self.alleles[1]=a2
-        self.mapping[a1]=0
-        self.mapping[a2]=1
+        return (
+            0.5
+            * (self.counts[0] + self.counts[1])
+            / (0.5 * (self.counts[0] + self.counts[1]) + self.counts[2])
+        )
+
+    def initAlleles(self, a1, a2):
+        self.alleles[0] = a1
+        self.alleles[1] = a2
+        self.mapping[a1] = 0
+        self.mapping[a2] = 1
         self._create_mapping()
-        self.addObservation=self.addObservationFull
-    def delGenotype(self,geno):
-        '''
+        self.addObservation = self.addObservationFull
+
+    def delGenotype(self, geno):
+        """
         Remove a genotype from observed alleles
-        '''
+        """
         if geno == missing:
             self.counts[2] -= 1
         else:
-            self.counts[0] -= 2-geno
+            self.counts[0] -= 2 - geno
             self.counts[1] -= geno
-    def addGenotype(self,geno):
-        '''
+
+    def addGenotype(self, geno):
+        """
         Add a genotype to observed alleles
-        '''
-        if geno==missing:
-            self.counts[2]-=1
+        """
+        if geno == missing:
+            self.counts[2] -= 1
         else:
-            self.counts[0] += 2-geno
+            self.counts[0] += 2 - geno
             self.counts[1] += geno
+
     def _create_mapping(self):
-        self.g2int={}
-        self.g2int[self.alleles[0]+self.alleles[0]]=zero
-        self.g2int[self.alleles[0]+self.alleles[1]]=un
-        self.g2int[self.alleles[1]+self.alleles[0]]=un
-        self.g2int[self.alleles[1]+self.alleles[1]]=deux
-    def addObservationFull(self,value):
+        self.g2int = {}
+        self.g2int[self.alleles[0] + self.alleles[0]] = zero
+        self.g2int[self.alleles[0] + self.alleles[1]] = un
+        self.g2int[self.alleles[1] + self.alleles[0]] = un
+        self.g2int[self.alleles[1] + self.alleles[1]] = deux
+
+    def addObservationFull(self, value):
         try:
             return self.g2int[value]
         except KeyError:
             return missing
-    def addObservationNotFull(self,value):
-        ''' 
-        Add an observed genotype ('AA','01'...) to the SNP 
+
+    def addObservationNotFull(self, value):
+        """
+        Add an observed genotype ('AA','01'...) to the SNP
         Return the 'integer genotype',0,1,2
         if two alleles have already been observed, switch to fast
         version
-        '''
-        geno=missing
+        """
+        geno = missing
         try:
-            i1,i2=value[0],value[1]
-        except :
+            i1, i2 = value[0], value[1]
+        except:
             return geno
         try:
-            g1=self.mapping[i1]
+            g1 = self.mapping[i1]
         except KeyError:
             if self.alleles[0] is None:
-                self.alleles[0]=i1
-                self.mapping[i1]=zero
-                g1=zero
+                self.alleles[0] = i1
+                self.mapping[i1] = zero
+                g1 = zero
             elif self.alleles[1] is None:
-                self.alleles[1]=i1
-                self.mapping[i1]=un
-                g1=un
+                self.alleles[1] = i1
+                self.mapping[i1] = un
+                g1 = un
                 self._create_mapping()
-                self.addObservation=self.addObservationFull
+                self.addObservation = self.addObservationFull
             else:
                 return geno
         try:
-            g2=self.mapping[i2]
+            g2 = self.mapping[i2]
         except KeyError:
-            assert self.alleles[0]!=None
+            assert self.alleles[0] != None
             if self.alleles[1] is None:
-                self.alleles[1]=i2
-                self.mapping[i2]=un
-                g2=un
+                self.alleles[1] = i2
+                self.mapping[i2] = un
+                g2 = un
                 self._create_mapping()
-                self.addObservation=self.addObservationFull
+                self.addObservation = self.addObservationFull
             else:
                 return geno
-        geno=g1+g2
+        geno = g1 + g2
         return geno
 
-class Locus():
-    def __init__(self,nom,position):
-        self.name=nom
-        self.pos=position
-    def __eq__(self,other):
+
+class Locus:
+    def __init__(self, nom, position):
+        self.name = nom
+        self.pos = position
+
+    def __eq__(self, other):
         return self.pos == other.pos
-    def __ne__(self,other):
+
+    def __ne__(self, other):
         return self.pos != other.pos
-    def __lt__(self,other):
+
+    def __lt__(self, other):
         return self.pos < other.pos
-    def __le__(self,other):
+
+    def __le__(self, other):
         return self.pos <= other.pos
-    def __gt__(self,other):
+
+    def __gt__(self, other):
         return self.pos > other.pos
+
     def __ge__(self, other):
         return self.pos >= other.pos
 
-class Map():
+
+class Map:
     def __init__(self):
-        '''
+        """
         Map class contains maps (duh)
         The chromosome names are stored in the chromosomes attribute (in sorted order)
         Each chromosome has two maps (genetic/RH and physical)
-        '''
-        self.chromosomes=[] 
-        self.cartes={}
-        self.markers={}
-        self.input_order=[]
-    def write(self,stream=sys.stdout):
+        """
+        self.chromosomes = []
+        self.cartes = {}
+        self.markers = {}
+        self.input_order = []
+
+    def write(self, stream=sys.stdout):
         for chrom in self.chromosomes:
             for mk in self.physMap(chrom):
-                pos=self.position(mk)
-                print( '\t'.join([str(x) for x in [pos[0],mk,int(pos[1]),int(pos[2])]]), file=stream)
+                pos = self.position(mk)
+                print(
+                    "\t".join([str(x) for x in [pos[0], mk, int(pos[1]), int(pos[2])]]), file=stream
+                )
         return
-    def addMarker(self,M,C,posG=0,posP=0):
-        '''
+
+    def addMarker(self, M, C, posG=0, posP=0):
+        """
         Add a marker on chromosome C, with genetic position posG and
         physical position posP
-        '''
+        """
         self.input_order.append(M)
         if not C in self.cartes:
-            insort(self.chromosomes,C)
-            self.cartes[C]={'Genet':[],'Phys':[]}
-        locG=Locus(M,posG)
-        locM=Locus(M,posP)
-        self.markers[M]=(C,locG,locM)
-        insort(self.cartes[C]['Genet'],locG)
-        insort(self.cartes[C]['Phys'],locM)
-    def delMarker(self,M):
+            insort(self.chromosomes, C)
+            self.cartes[C] = {"Genet": [], "Phys": []}
+        locG = Locus(M, posG)
+        locM = Locus(M, posP)
+        self.markers[M] = (C, locG, locM)
+        insort(self.cartes[C]["Genet"], locG)
+        insort(self.cartes[C]["Phys"], locM)
+
+    def delMarker(self, M):
         try:
             locus = self.markers[M]
         except KeyError:
-            print( "No such marker")
+            print("No such marker")
         del self.markers[M]
-        self.cartes[locus[0]]['Genet'].remove(locus[1])
-        self.cartes[locus[0]]['Phys'].remove(locus[2])
-    def genetMap(self,C,xleft=-1,xright=np.inf):
-        '''
-        Returns and iterator on the genetic map between position xleft and xright 
+        self.cartes[locus[0]]["Genet"].remove(locus[1])
+        self.cartes[locus[0]]["Phys"].remove(locus[2])
+
+    def genetMap(self, C, xleft=-1, xright=np.inf):
+        """
+        Returns and iterator on the genetic map between position xleft and xright
         on chromosome C
-        '''
+        """
         try:
-            carte=self.cartes[C]['Genet']
+            carte = self.cartes[C]["Genet"]
         except KeyError:
             return []
-        mk=carte[bisect_left(carte,Locus(0,xleft)):bisect_right(carte,Locus(0,xright))]
+        mk = carte[bisect_left(carte, Locus(0, xleft)) : bisect_right(carte, Locus(0, xright))]
         return (m.name for m in mk)
-    def physMap(self,C,xleft=0,xright=np.inf):
-        '''
-        Returns and iterator on the genetic map between position xleft and xright 
+
+    def physMap(self, C, xleft=0, xright=np.inf):
+        """
+        Returns and iterator on the genetic map between position xleft and xright
         on chromosome C
-        '''
+        """
         try:
-            carte=self.cartes[C]['Phys']
+            carte = self.cartes[C]["Phys"]
         except KeyError:
             return []
-        mk=carte[bisect_left(carte,Locus(0,xleft)):bisect_right(carte,Locus(0,xright))]
+        mk = carte[bisect_left(carte, Locus(0, xleft)) : bisect_right(carte, Locus(0, xright))]
         return (m.name for m in mk)
-    def length(self,C):
-        '''
+
+    def length(self, C):
+        """
         Return the length of maps of chromosome C [physical,genetic]
-        '''
-        carte=self.cartes[C]['Phys']
-        lenP=carte[-1].pos-carte[0].pos
-        carte=self.cartes[C]['Genet']
-        lenG=carte[-1].pos-carte[0].pos
-        return [lenP,lenG]
-    def position(self,M):
-        '''
+        """
+        carte = self.cartes[C]["Phys"]
+        lenP = carte[-1].pos - carte[0].pos
+        carte = self.cartes[C]["Genet"]
+        lenG = carte[-1].pos - carte[0].pos
+        return [lenP, lenG]
+
+    def position(self, M):
+        """
         Returns chromosome,genetic,physical position of marker M
-        '''
+        """
         try:
-            locus=self.markers[M]
-            return locus[0],locus[1].pos,locus[2].pos
+            locus = self.markers[M]
+            return locus[0], locus[1].pos, locus[2].pos
         except KeyError:
-            print( M,'not found')
+            print(M, "not found")
             return None
-    def sort_loci(self,loci,physical=True):
-        '''
+
+    def sort_loci(self, loci, physical=True):
+        """
         Sort loci according to their position on the map
 
         Parameters:
         ---------------
 
         loci : a list of loci names
         physical : if True sort according to physical position, o.w. use genetic  / RH position
 
         Return Value:
         -----------------
 
         list of the same loci, sorted
-        '''
-        new_list=[]
+        """
+        new_list = []
         for locus in loci:
             try:
-                tmp=self.markers[locus]
+                tmp = self.markers[locus]
                 if physical:
-                    myloc=tmp[2]
+                    myloc = tmp[2]
                 else:
-                    myloc=tmp[1]
+                    myloc = tmp[1]
                 try:
-                    mychr=int(tmp[0])
+                    mychr = int(tmp[0])
                 except:
-                    mychr=tmp[0]
+                    mychr = tmp[0]
             except KeyError:
                 continue
-            new_list.append((locus,mychr,myloc.pos))
-        new_list=sorted(new_list,key=itemgetter(1,2))
+            new_list.append((locus, mychr, myloc.pos))
+        new_list = sorted(new_list, key=itemgetter(1, 2))
         return [x[0] for x in new_list]
-    
-    def iterate_pos_windows(self,wlen,padlen=0):
+
+    def iterate_pos_windows(self, wlen, padlen=0):
         for c in self.chromosomes:
-            pos_left=0
-            pos_right=-1
-            clen=self.length(c)[0]
-            print( c,clen)
+            pos_left = 0
+            pos_right = -1
+            clen = self.length(c)[0]
+            print(c, clen)
             while pos_right < clen:
-                pos_right=pos_left+wlen
-                yield (c,(pos_left-padlen)>0 and pos_left-padlen or 0,(pos_right+padlen)>clen and clen+1 or pos_right+padlen )
-                pos_left=pos_right
-                
+                pos_right = pos_left + wlen
+                yield (
+                    c,
+                    (pos_left - padlen) > 0 and pos_left - padlen or 0,
+                    (pos_right + padlen) > clen and clen + 1 or pos_right + padlen,
+                )
+                pos_left = pos_right
```

### Comparing `hapflk-2.0.dev2/hapflk/hapflk.py` & `hapflk-2.1/hapflk/hapflk.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 #!/usr/bin/env python3
 import pickle
 import sys
 import argparse
 import bz2
 from hapflk import InputOutput as IO
-from hapflk import popgen
-import hapflk.fastphase as myfph
+from hapflk import popgen, utils
+from fastphase import fastphase as myfph
 import numpy as np
 from multiprocessing import cpu_count
 
 
 class SNP(object):
-    """ Pickable simplified SNP class"""
+    """Pickable simplified SNP class"""
+
     def __init__(self, name, a1, a2):
         """
         SNP class to store name and alleles
         :type name: basestring
         :type a1: basestring
         :type a2: basestring
         """
         self.name = name
         self.alleles = [a1, a2]
 
+
 class HapFLK(object):
-    ''' A class to run an hapFLK analysis.
-    '''
+    """A class to run an hapFLK analysis."""
+
     def __init__(self):
-        ''' Attributes of the class (not all need be specified)
+        """Attributes of the class (not all need be specified)
 
         Note: Data arrays indices relate to the pops and sortes_snps lists.
 
             Input Data
             ----------
             - carte: data.Map instance of SNP info (may contain > nsnp)
             - sorted_snps: list of SNP objects ordered by position in carte
@@ -41,392 +43,586 @@
             -----------
             - outgroup: name of the outgroup used to build kinship. Usually not in pops
             - reynolds: matrix of reynolds distances between pop
             - hzy: heterozygosity of pops
             - kinship: Kinship matrix between pops
             - frq: SNP allele freq in pops
             - K : number of clusters
-            - nfit : number of EM fits 
+            - nfit : number of EM fits
             - kfrq: haplotype cluster frequencies
 
             Test Data
             ---------
             - flk: FLK values
             - pzero: estimated ancestral allele frequencies
             - pval_FLK: theoretical p-value of FLK
             - hapflk: hapFLK values
             - eigvec: Eigen Vectors of kinship matrix
             - eigval: Eigen Values of kinship matrix
             - eigen_FLK: Spectral decomposition of FLK test
             - eigen_hapFLK: Spectral decomposition of hapFLK test
-        '''
+        """
         ## SNP info
-        self.carte=None
-        self.sorted_snps=None
-        self.alleles=None
+        self.carte = None
+        self.sorted_snps = None
+        self.alleles = None
         ## Model data
-        self.pops=None
-        self.outgroup=None
-        self.reynolds=None
-        self.hzy=None
-        self.kinship=None
-        self.frq=None
-        self.K=-1
-        self.nfit=0
-        self.kfrq=None
+        self.pops = None
+        self.outgroup = None
+        self.reynolds = None
+        self.hzy = None
+        self.kinship = None
+        self.frq = None
+        self.K = -1
+        self.nfit = 0
+        self.kfrq = None
         ## Test data
-        self.flk=None
-        self.pzero=None
-        self.hapflk=None
-        self.eigvec=None
-        self.eigval=None
-        self.flk_eigen=None
-        self.hapflk_eigen=None
+        self.flk = None
+        self.pzero = None
+        self.hapflk = None
+        self.eigvec = None
+        self.eigval = None
+        self.flk_eigen = None
+        self.hapflk_eigen = None
 
     @property
     def nsnp(self):
         return len(self.sorted_snps)
 
     @property
     def npop(self):
         return len(self.pops)
-    
+
     @classmethod
-    def from_db_file(cls,filename):
-        '''Create Instance from dbfile'''
-        with bz2.BZ2File(filename,'rb') as f:
-            obj=pickle.load(f)
-        obj.__class__=cls ## allows to load parent obj from subclasses
+    def from_db_file(cls, filename):
+        """Create Instance from dbfile"""
+        with bz2.BZ2File(filename, "rb") as f:
+            obj = pickle.load(f)
+        obj.__class__ = cls  ## allows to load parent obj from subclasses
         return obj
 
     @classmethod
-    def from_cmd_line(cls,opts):
-        '''Create instance from command line arguments'''
-        obj=cls()
+    def from_cmd_line(cls, opts):
+        """Create instance from command line arguments"""
+        obj = cls()
 
-        data=obj.read_input(opts)
-        obj.model_setup(data,opts)
+        data = obj.read_input(opts)
+        obj.model_setup(data, opts)
         obj.write_frq(opts.prefix)
-        
-        if opts.K>0:
+
+        if opts.K > 0:
             print("Fitting LD model (this might take a while)")
-            fphpars=obj.run_fastphase(data,opts)
+            fphpars = obj.run_fastphase(data, opts)
             print("Computing haplotype cluster frequencies")
-            obj.calc_kfrq(data,opts,fphpars)
+            obj.calc_kfrq(data, opts, fphpars)
             if opts.kfrq:
                 obj.write_kfrq(opts.prefix)
-            obj.nfit,obj.K,np,ns=obj.kfrq.shape
+            obj.nfit, obj.K, np, ns = obj.kfrq.shape
         else:
-            obj.kfrq=None
-            obj.nfit=0
-            obj.K=0
+            obj.kfrq = None
+            obj.nfit = 0
+            obj.K = 0
         return obj
-        
 
     @staticmethod
     def populate_parser(parser):
-        parser.add_argument('-p','--prefix',dest='prefix',help='prefix for output files',default='hapflk')
-        parser.add_argument('--ncpu',metavar='N',help='Use N processors when possible',default=cpu_count(),type=int)
-        parser.add_argument('--eigen',help='Perform eigen decomposition of tests',default=False,action='store_true')
-        parser.add_argument('--reynolds',help='Force writing down Reynolds distances',default=False,action='store_true')
-        parser.add_argument('--future',help=argparse.SUPPRESS,default=False,action="store_true") ## for testing future release
-        parser.add_argument('--debug',help=argparse.SUPPRESS,default=False,action="store_true") ## for debug purpose
-        parser.add_argument('--savedb',help=argparse.SUPPRESS,default=False,action="store_true") ## save hapflk DB
-        parser.add_argument('--loaddb',dest='dbfile',help=argparse.SUPPRESS,default=None) ## load hapflk DB
-        flk_opts=parser.add_argument_group('Population kinship ','Set parameters for getting the population kinship matrix')
-        flk_opts.add_argument('--kinship',help='Read population kinship from file (if None, kinship is estimated)',metavar='FILE',default=None)
-        flk_opts.add_argument('--reynolds-snps',dest='reysnps',type=int,help='Number of SNPs to use to estimate Reynolds distances',default=100000,metavar='L')
-        flk_opts.add_argument('--outgroup',default=None,help='Use population POP as outgroup for tree rooting (if None, optimize root location)',metavar="POP")
-        flk_opts.add_argument('--keep-outgroup',dest='keepOG',default=False,help='Keep outgroup in population set',action="store_true")
-        flk_opts.add_argument('--covkin',default=False,help='Use covariance matrix as kinship', action='store_true')
-        LD_opts=parser.add_argument_group('hapFLK and LD model','Switch on hapFLK calculations and set parameters of the LD model ')
-        LD_opts.add_argument('-K',help='Set the number of clusters to K. hapFLK calculations switched off if K<0',default=-1,type=int)
-        LD_opts.add_argument('--nfit',help='Set the number of model fit to use',type=int,default=10)
-        LD_opts.add_argument('--phased','--inbred',help='Haplotype data provided',dest='inbred',action="store_true",default=False)
-        LD_opts.add_argument('--fastLD',help=argparse.SUPPRESS,default=False,action='store_true') ## Fit LD model on "haploidized" individuals
-        LD_opts.add_argument('--kfrq',dest='kfrq',help='Write Cluster frequencies (Big files)',action="store_true",default=False)
-        LD_opts.add_argument('--write-params',dest='wparams',help=argparse.SUPPRESS,default=False,action='store_true')
-        LD_opts.add_argument('--legacy', dest='legacy',help='Use Legacy fastPHASE', default=False, action='store_true')
-        parser.add_argument('--annot',help='Shortcut for --eigen --reynolds --kfrq',default=False,action='store_true')
-        parser.add_argument('--tree',help=argparse.SUPPRESS,default=False,action='store_true')
+        parser.add_argument(
+            "-p",
+            "--prefix",
+            dest="prefix",
+            help="prefix for output files",
+            default="hapflk",
+        )
+        parser.add_argument(
+            "--ncpu",
+            metavar="N",
+            help="Use N processors when possible",
+            default=cpu_count(),
+            type=int,
+        )
+        parser.add_argument(
+            "--eigen",
+            help="Perform eigen decomposition of tests",
+            default=False,
+            action="store_true",
+        )
+        parser.add_argument(
+            "--reynolds",
+            help="Force writing down Reynolds distances",
+            default=False,
+            action="store_true",
+        )
+        parser.add_argument(
+            "--future", help=argparse.SUPPRESS, default=False, action="store_true"
+        )  ## for testing future release
+        parser.add_argument(
+            "--debug", help=argparse.SUPPRESS, default=False, action="store_true"
+        )  ## for debug purpose
+        parser.add_argument(
+            "--savedb", help=argparse.SUPPRESS, default=False, action="store_true"
+        )  ## save hapflk DB
+        parser.add_argument(
+            "--loaddb", dest="dbfile", help=argparse.SUPPRESS, default=None
+        )  ## load hapflk DB
+        flk_opts = parser.add_argument_group(
+            "Population kinship ",
+            "Set parameters for getting the population kinship matrix",
+        )
+        flk_opts.add_argument(
+            "--kinship",
+            help="Read population kinship from file (if None, kinship is estimated)",
+            metavar="FILE",
+            default=None,
+        )
+        flk_opts.add_argument(
+            "--reynolds-snps",
+            dest="reysnps",
+            type=int,
+            help="Number of SNPs to use to estimate Reynolds distances",
+            default=100000,
+            metavar="L",
+        )
+        flk_opts.add_argument(
+            "--outgroup",
+            default=None,
+            help="Use population POP as outgroup for tree rooting (if None, optimize root location)",
+            metavar="POP",
+        )
+        flk_opts.add_argument(
+            "--keep-outgroup",
+            dest="keepOG",
+            default=False,
+            help="Keep outgroup in population set",
+            action="store_true",
+        )
+        flk_opts.add_argument(
+            "--covkin",
+            default=False,
+            help="Use covariance matrix as kinship",
+            action="store_true",
+        )
+        LD_opts = parser.add_argument_group(
+            "hapFLK and LD model",
+            "Switch on hapFLK calculations and set parameters of the LD model ",
+        )
+        LD_opts.add_argument(
+            "-K",
+            help="Set the number of clusters to K. hapFLK calculations switched off if K<0",
+            default=-1,
+            type=int,
+        )
+        LD_opts.add_argument(
+            "--nfit", help="Set the number of model fit to use", type=int, default=10
+        )
+        LD_opts.add_argument(
+            "--phased",
+            "--inbred",
+            help="Haplotype data provided",
+            dest="inbred",
+            action="store_true",
+            default=False,
+        )
+        LD_opts.add_argument(
+            "--fastLD", help=argparse.SUPPRESS, default=False, action="store_true"
+        )  ## Fit LD model on "haploidized" individuals
+        LD_opts.add_argument(
+            "--kfrq",
+            dest="kfrq",
+            help="Write Cluster frequencies (Big files)",
+            action="store_true",
+            default=False,
+        )
+        LD_opts.add_argument(
+            "--write-params",
+            dest="wparams",
+            help=argparse.SUPPRESS,
+            default=False,
+            action="store_true",
+        )
+        LD_opts.add_argument(
+            "--legacy",
+            dest="legacy",
+            help="Use Legacy fastPHASE",
+            default=False,
+            action="store_true",
+        )
+        parser.add_argument(
+            "--annot",
+            help="Shortcut for --eigen --reynolds --kfrq",
+            default=False,
+            action="store_true",
+        )
+        parser.add_argument("--tree", help=argparse.SUPPRESS, default=False, action="store_true")
 
     @classmethod
-    def get_opts(cls,args):
-        ''' Parse arguments from a command line and returns hapFLK options'''
+    def get_opts(cls, args):
+        """Parse arguments from a command line and returns hapFLK options"""
         ## Arguments and option parser
-        parser=argparse.ArgumentParser(parents=[IO.io_parser],formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+        parser = argparse.ArgumentParser(
+            parents=[IO.io_parser],
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        )
         cls.populate_parser(parser)
-        if len(args)<2:
+        if len(args) < 2:
             parser.print_help()
             sys.exit(0)
-        opts=parser.parse_args(args[1:])
+        opts = parser.parse_args(args[1:])
         if opts.annot:
-            opts.reynolds=True
-            opts.kfrq=True
-            opts.eigen=True
+            opts.reynolds = True
+            opts.kfrq = True
+            opts.eigen = True
         if opts.sfile:
-            opts.inbred=True
+            opts.inbred = True
         return opts
-    
-    def read_input(self,opts):
-        '''Read input files
+
+    def read_input(self, opts):
+        """Read input files
         Creates the following attributes:
         -- carte
         -- sorted_snps
         -- nsnps
-        '''
-        myi=IO.parseInput(opts)
+        """
+        myi = IO.parseInput(opts)
         if myi is None:
             self.parser.print_help()
             sys.exit(0)
-        data=myi['dataset']
-        self.carte=myi['map']
-        self.sorted_snps=[]
+        data = myi["dataset"]
+        self.carte = myi["map"]
+        self.sorted_snps = []
         for sname in self.carte.sort_loci(data.snp.keys()):
-            self.sorted_snps.append(SNP(sname,data.snp[sname].alleles[0],data.snp[sname].alleles[1]))
-            
+            self.sorted_snps.append(
+                SNP(sname, data.snp[sname].alleles[0], data.snp[sname].alleles[1])
+            )
+
         return data
-    
-    def model_setup(self,data,opts):
-        ''' Sets up FLK model. Creates the following attributes:
-        -- reynolds 
+
+    def model_setup(self, data, opts):
+        """Sets up FLK model. Creates the following attributes:
+        -- reynolds
         -- hzy
         -- outgroup
         -- kinship
         -- frq
         -- pops
 
-        '''
+        """
         ## Compute allele frequencies
-        print('Computing Allele Frequencies')
-        res=data.compute_pop_frq()
-        freqs=res['freqs']
-        pops=res['pops']
-        
+        print("Computing Allele Frequencies")
+        res = data.compute_pop_frq()
+        freqs = res["freqs"]
+        pops = res["pops"]
+
         ## compute Reynolds distances
-        print('Computing Reynolds distances')
-        if opts.reysnps>self.nsnp:
-            opts.reysnps=self.nsnp
-        pbinom=float(opts.reysnps)/self.nsnp
-        snp_subset=np.array(np.random.binomial(1,pbinom,self.nsnp),dtype=bool)
-        self.reynolds=popgen.reynolds(freqs[:,snp_subset])
-        self.hzy=popgen.heterozygosity(freqs[:,snp_subset])
-        self.outgroup=opts.outgroup
+        print("Computing Reynolds distances")
+        if opts.reysnps > self.nsnp:
+            opts.reysnps = self.nsnp
+        pbinom = float(opts.reysnps) / self.nsnp
+        snp_subset = np.array(np.random.binomial(1, pbinom, self.nsnp), dtype=bool)
+        self.reynolds = popgen.reynolds(freqs[:, snp_subset])
+        self.hzy = popgen.heterozygosity(freqs[:, snp_subset])
+        self.outgroup = opts.outgroup
         ## Get kinship
         if opts.kinship:
-            print('Reading Kinship Matrix')
+            print("Reading Kinship Matrix")
             if not opts.keepOG:
-                self.kinship=popgen.popKinship_fromFile(opts.kinship,[pop for pop in pops if pop != self.outgroup])
+                self.kinship = popgen.popKinship_fromFile(
+                    opts.kinship, [pop for pop in pops if pop != self.outgroup]
+                )
             else:
-                self.kinship=popgen.popKinship_fromFile(opts.kinship,[pop for pop in pops])
+                self.kinship = popgen.popKinship_fromFile(opts.kinship, [pop for pop in pops])
         else:
-        ## estimate kinship
+            ## estimate kinship
             print("Computing Kinship Matrix")
-            self.kinship=popgen.popKinship_new(self.reynolds,pops,self.outgroup,
-                                              fprefix=opts.prefix,
-                                              keep_outgroup=opts.keepOG,
-                                              hzy=self.hzy,
-                                              dump_tree=opts.tree)
+            self.kinship = popgen.popKinship_new(
+                self.reynolds,
+                pops,
+                self.outgroup,
+                fprefix=opts.prefix,
+                keep_outgroup=opts.keepOG,
+                hzy=self.hzy,
+                dump_tree=opts.tree,
+            )
         ## store eigen decomp of kinship matrix
-        self.eigval,self.eigvec=np.linalg.eigh(self.kinship)
+        self.eigval, self.eigvec = np.linalg.eigh(self.kinship)
         ## forget about the outgroup if we keep it
         if opts.keepOG:
             ## override results / initial value
-            self.outgroup='Iwantmyoutgroupback'
+            self.outgroup = "Iwantmyoutgroupback"
         ## boolean array indicating kept populations
-        keep_pop=np.array([x!=self.outgroup for x in pops],dtype=bool)
-        self.frq=freqs[keep_pop,]
-        self.pops=tuple([x for x in pops if x!=self.outgroup])
+        keep_pop = np.array([x != self.outgroup for x in pops], dtype=bool)
+        self.frq = freqs[
+            keep_pop,
+        ]
+        self.pops = tuple([x for x in pops if x != self.outgroup])
         if opts.covkin:
-            print('Computing Covariance Matrix')
-            ff=popgen.FLK_test(self.kinship)
+            print("Computing Covariance Matrix")
+            ff = popgen.FLK_test(self.kinship)
             ## calculate hat(p0)
-            pzero=np.array([ff.eigen_contrib(self.frq[:,s])[0] for s in range(self.nsnp)])
-            sub=(pzero>0.05)&(pzero<0.95)
+            pzero = np.array([ff.eigen_contrib(self.frq[:, s])[0] for s in range(self.nsnp)])
+            sub = (pzero > 0.05) & (pzero < 0.95)
             ## calculate empirical covariance matrix
-            myf=self.frq[:,sub]
-            m=pzero[sub]
-            s=np.sqrt(m*(1-m))
-            myfstd=(myf-m)/s
-            covkin=np.cov(myfstd,rowvar=True)
+            myf = self.frq[:, sub]
+            m = pzero[sub]
+            s = np.sqrt(m * (1 - m))
+            myfstd = (myf - m) / s
+            covkin = np.cov(myfstd, rowvar=True)
             ## Add a small term on the diagonal to ensure stable inverse
-            val=np.trace(covkin)/self.npop
-            assert (val >0)
-            covkin=covkin+np.diag(np.ones(self.npop)*0.01*val)
-            with open(opts.prefix+'_cov.txt','w') as fcov:
-                for i,pi in enumerate(self.pops):
-                    tw=[pi]
-                    for j,pj in enumerate(self.pops):
-                        tw.append(str(covkin[i,j]))
-                    print(' '.join(tw),file=fcov)
-            self.kinship=covkin
-        
-    def run_fastphase(self,data,opts):
-        '''Estimates Scheet and Stephens LD model on data'''
-        fphpars=[]
-        with myfph.fastphase(self.nsnp, opts.ncpu, prfx = opts.prefix+'.fphlog') as fastphase_model:
-            tohap=np.vectorize(lambda x: (x==1) and -1 or (x//2))
-            sorted_snps_idx=np.array([data.snpIdx[s.name] for s in self.sorted_snps])
-            for name,i in data.indivIdx.items():
-                if data.indiv[name].pop==self.outgroup:
+            val = np.trace(covkin) / self.npop
+            assert val > 0
+            covkin = covkin + np.diag(np.ones(self.npop) * 0.01 * val)
+            with open(opts.prefix + "_cov.txt", "w") as fcov:
+                for i, pi in enumerate(self.pops):
+                    tw = [pi]
+                    for j, pj in enumerate(self.pops):
+                        tw.append(str(covkin[i, j]))
+                    print(" ".join(tw), file=fcov)
+            self.kinship = covkin
+
+    def run_fastphase(self, data, opts):
+        """Estimates Scheet and Stephens LD model on data"""
+        fphpars = []
+        with myfph.fastphase(self.nsnp, opts.ncpu, prfx=opts.prefix + ".fphlog") as fastphase_model:
+            tohap = np.vectorize(lambda x: (x == 1) and -1 or (x // 2))
+            sorted_snps_idx = np.array([data.snpIdx[s.name] for s in self.sorted_snps])
+            for name, i in data.indivIdx.items():
+                if data.indiv[name].pop == self.outgroup:
                     continue
                 if opts.inbred:
-                    haplo=np.array(tohap(np.array(data.Data[i,sorted_snps_idx],dtype=int)),dtype=np.int)
-                    fastphase_model.addHaplotype(name,haplo)
+                    haplo = np.array(
+                        tohap(np.array(data.Data[i, sorted_snps_idx], dtype=int)),
+                        dtype=int,
+                    )
+                    fastphase_model.addHaplotype(name, haplo)
                 else:
-                    fastphase_model.addGenotype(name,np.array(data.Data[i,sorted_snps_idx],dtype=int))
+                    fastphase_model.addGenotype(
+                        name, np.array(data.Data[i, sorted_snps_idx], dtype=int)
+                    )
             if opts.legacy:
                 for e in range(opts.nfit):
-                    sys.stderr.write('\tEM %d / %d \r'%(e+1,opts.nfit))
+                    sys.stderr.write("\tEM %d / %d \r" % (e + 1, opts.nfit))
                     sys.stderr.flush()
                     if opts.debug:
                         print()
-                    par=fastphase_model.fit(nClus=opts.K,verbose=opts.debug, fast=opts.fastLD)
+                    par = fastphase_model.fit(nClus=opts.K, verbose=opts.debug, fast=opts.fastLD)
                     fphpars.append(par)
                     if opts.wparams:
-                        fout=open(opts.prefix+'fph_par_'+str(e),'w')
+                        fout = open(opts.prefix + "fph_par_" + str(e), "w")
                         par.write(fout)
                         fout.close()
             else:
-                par = fastphase_model.optimfit(nClus=opts.K,verbose=opts.debug,nEM=opts.nfit, fast=opts.fastLD)
+                par = fastphase_model.optimfit(
+                    nClus=opts.K, verbose=opts.debug, nEM=opts.nfit, fast=opts.fastLD
+                )
                 # with open(opts.prefix+'debug_alpha_const.txt','w') as fpar:
                 #     par.write(stream=fpar)
                 ## update alpha
                 # print('Finalizing: Updating Cluster Weights')
                 # par.alpha_up = True
                 # par = fastphase_model.fit(params=par,nClus=opts.K,verbose=opts.debug,nstep=50)
                 # with open(opts.prefix+'debug_alpha_free.txt','w') as fpar:
                 #     par.write(stream=fpar)
                 opts.nfit = 1
                 fphpars.append(par)
                 if opts.wparams:
-                        fout=open(opts.prefix+'fph_par','w')
-                        par.write(fout)
-                        fout.close()
+                    fout = open(opts.prefix + "fph_par", "w")
+                    par.write(fout)
+                    fout.close()
             print()
         return fphpars
-        
-    def calc_kfrq(self,data,opts,fphpars):
-        ''' Compute haplotype cluster population frequencies '''
+
+    def calc_kfrq(self, data, opts, fphpars):
+        """Compute haplotype cluster population frequencies"""
         ## [E][K][npop x nsnp] array
-        pop_cluster_freq=np.zeros((opts.nfit,opts.K,self.npop,self.nsnp),dtype=float)
-        with myfph.fastphase( self.nsnp, opts.ncpu) as fastphase_model:
-            tohap=np.vectorize(lambda x: (x==1) and -1 or (x/2))
-            sorted_snps_idx=np.array([data.snpIdx[s.name] for s in self.sorted_snps])
-            for ipop,popname in enumerate(self.pops):
-                sys.stdout.write("\t %16s\r"%popname)
+        pop_cluster_freq = np.zeros((opts.nfit, opts.K, self.npop, self.nsnp), dtype=float)
+        with myfph.fastphase(self.nsnp, opts.ncpu) as fastphase_model:
+            tohap = np.vectorize(lambda x: (x == 1) and -1 or (x / 2))
+            sorted_snps_idx = np.array([data.snpIdx[s.name] for s in self.sorted_snps])
+            for ipop, popname in enumerate(self.pops):
+                sys.stdout.write("\t %16s\r" % popname)
                 sys.stdout.flush()
-                pvec=data.populations[popname]
-                n_pop_indiv=sum(pvec)
-                for name,iind in data.indivIdx.items():
+                pvec = data.populations[popname]
+                n_pop_indiv = sum(pvec)
+                for name, iind in data.indivIdx.items():
                     if pvec[iind]:
                         if opts.inbred:
-                            haplo=np.array(tohap(np.array(data.Data[iind,sorted_snps_idx],dtype=int)),dtype=np.int)
-                            fastphase_model.addHaplotype(name,haplo)
+                            haplo = np.array(
+                                tohap(np.array(data.Data[iind, sorted_snps_idx], dtype=int)),
+                                dtype=int,
+                            )
+                            fastphase_model.addHaplotype(name, haplo)
                         else:
-                            fastphase_model.addGenotype(name,np.array(data.Data[iind,sorted_snps_idx],dtype=int))
+                            fastphase_model.addGenotype(
+                                name,
+                                np.array(data.Data[iind, sorted_snps_idx], dtype=int),
+                            )
                 for ifit in range(opts.nfit):
-                    imputations=fastphase_model.impute([fphpars[ifit]])
-                    for nom,dat in imputations.items():
-                        probZ=dat[1]
+                    imputations = fastphase_model.impute([fphpars[ifit]])
+                    for nom, dat in imputations.items():
+                        probZ = dat[1]
                         if opts.inbred:
-                            pop_cluster_freq[ifit,:,ipop,:]+=np.transpose(probZ[0]/n_pop_indiv)
+                            pop_cluster_freq[ifit, :, ipop, :] += np.transpose(
+                                probZ[0] / n_pop_indiv
+                            )
                         else:
-                            pop_cluster_freq[ifit,:,ipop,:]+=np.transpose((0.5/n_pop_indiv)*(np.sum(probZ[0],axis=1)+np.sum(probZ[0],axis=2)))
+                            pop_cluster_freq[ifit, :, ipop, :] += np.transpose(
+                                (0.5 / n_pop_indiv)
+                                * (np.sum(probZ[0], axis=1) + np.sum(probZ[0], axis=2))
+                            )
                 fastphase_model.flush()
-        self.kfrq=pop_cluster_freq
+        self.kfrq = pop_cluster_freq
 
-    def run_tests(self,opts):
+    def run_tests(self, opts):
         if self.flk is None:
-            print('Computing FLK tests')
+            print("Computing FLK tests")
             self.calc_flk()
             self.write_flk(opts.prefix)
-            
-        if self.K>0:
+
+        if self.K > 0:
             if self.hapflk is None:
                 print("Computing hapFLK tests")
                 self.calc_hapflk()
                 self.write_hapflk(opts.prefix)
         return
+
     def calc_flk(self):
-        '''Computes FLK tests'''
+        """Computes FLK tests"""
         ## Compute single SNP FLK tests
-        myFLK=popgen.FLK_test(self.kinship)
-        myFLK_res=np.apply_along_axis(myFLK.eval_flk,0,self.frq)
-        self.pzero=myFLK_res[0,]
-        self.flk=myFLK_res[1,]
-        self.pval_FLK=myFLK_res[2,]
-        self.eigen_FLK=np.power(myFLK_res[3:,],2)
+        myFLK = popgen.FLK_test(self.kinship)
+        myFLK_res = np.apply_along_axis(myFLK.eval_flk, 0, self.frq)
+        self.pzero = myFLK_res[
+            0,
+        ]
+        self.flk = myFLK_res[
+            1,
+        ]
+        self.pval_FLK = myFLK_res[
+            2,
+        ]
+        self.eigen_FLK = np.power(
+            myFLK_res[
+                3:,
+            ],
+            2,
+        )
         return
-    
+
     def calc_hapflk(self):
-        ''' Compute hapFLK tests '''
-        myFLK=popgen.FLK_test(self.kinship,diallelic=False)
-        self.hapflk=np.zeros(self.nsnp,dtype=float)
-        self.eigen_hapFLK=np.zeros((self.npop,self.nsnp),dtype=float)
+        """Compute hapFLK tests"""
+        myFLK = popgen.FLK_test(self.kinship, diallelic=False)
+        self.hapflk = np.zeros(self.nsnp, dtype=float)
+        self.eigen_hapFLK = np.zeros((self.npop, self.nsnp), dtype=float)
         for e in range(self.nfit):
             for k in range(self.K):
-                myFLK_res=np.apply_along_axis(myFLK.eval_flk,0,self.kfrq[e,k,])
-                self.hapflk+=myFLK_res[1,]
-                self.eigen_hapFLK+=np.power(myFLK_res[3:,],2)
-        self.hapflk/=self.nfit
-        self.eigen_hapFLK/=self.nfit
+                myFLK_res = np.apply_along_axis(
+                    myFLK.eval_flk,
+                    0,
+                    self.kfrq[
+                        e,
+                        k,
+                    ],
+                )
+                self.hapflk += myFLK_res[
+                    1,
+                ]
+                self.eigen_hapFLK += np.power(
+                    myFLK_res[
+                        3:,
+                    ],
+                    2,
+                )
+        self.hapflk /= self.nfit
+        self.eigen_hapFLK /= self.nfit
         return
 
     def calc_hapflk_ng(self):
         pass
-    
-    def savedb(self,prefix):
-        ''' Save (pickle) instance of the class in a 'prefix'.db file
-            NB: The instance can be loaded (unpickled) using the class method from_db_file.
-        '''
-        dbfile=bz2.BZ2File(prefix+'.db','wb')
-        pickle.dump(self,dbfile,protocol=2)
+
+    def savedb(self, prefix):
+        """Save (pickle) instance of the class in a 'prefix'.db file
+        NB: The instance can be loaded (unpickled) using the class method from_db_file.
+        """
+        dbfile = bz2.BZ2File(prefix + ".db", "wb")
+        pickle.dump(self, dbfile, protocol=2)
         dbfile.close()
 
-    def write_frq(self,prefix):
-        ''' Write allele frequencies to 'prefix'.frq'''
-        assert(self.frq is not None)
-        with open(prefix+'.frq','w') as fout:
-            print('rs','chr','pos','all_ref','all_alt',' '.join(self.pops),file=fout)
-            for sidx,s in enumerate(self.sorted_snps):
-                spos=self.carte.position(s.name)
-                tw=[s.name,spos[0],int(spos[2]),s.alleles[1],s.alleles[0]]
-                for ip,nom in enumerate(self.pops):
-                    tw.append(self.frq[ip,sidx])
-                print(*tw,file=fout)
+    def write_frq(self, prefix):
+        """Write allele frequencies to 'prefix'.frq"""
+        assert self.frq is not None
+        with open(prefix + ".frq", "w") as fout:
+            print("rs", "chr", "pos", "all_ref", "all_alt", " ".join(self.pops), file=fout)
+            for sidx, s in enumerate(self.sorted_snps):
+                spos = self.carte.position(s.name)
+                tw = [s.name, spos[0], int(spos[2]), s.alleles[1], s.alleles[0]]
+                for ip, nom in enumerate(self.pops):
+                    tw.append(self.frq[ip, sidx])
+                print(*tw, file=fout)
 
-    def write_kfrq(self,prefix):
+    def write_kfrq(self, prefix):
         if self.kfrq is None:
             pass
-        nfit,nclus,npop,nsnp = self.kfrq.shape
+        nfit, nclus, npop, nsnp = self.kfrq.shape
         for ifit in range(nfit):
-            with bz2.open(prefix+'.fit_'+str(ifit)+'.bz2','wt') as fout:
-                print('pop','locus','position','cluster','prob',file=fout)
+            with bz2.open(prefix + ".fit_" + str(ifit) + ".bz2", "wt") as fout:
+                print("pop", "locus", "position", "cluster", "prob", file=fout)
                 for ipop in range(npop):
-                    for i,s in enumerate(self.sorted_snps):
-                        spos=self.carte.position(s.name)
+                    for i, s in enumerate(self.sorted_snps):
+                        spos = self.carte.position(s.name)
                         for ik in range(nclus):
-                            print(self.pops[ipop],s.name,int(spos[2]),ik,self.kfrq[ifit,ik,ipop,i], file=fout)
-            
-    def write_flk(self,prefix):
-        ''' Write FLK results to 'prefix'.flk'''
-        assert(self.flk is not None)
-        with open(prefix+'.flk','w') as fout:
-            print('rs','chr','pos','pzero','flk','pvalue',file=fout)
-            for sidx,s in enumerate(self.sorted_snps):
-                spos=self.carte.position(s.name)
-                tw=[s.name,spos[0],int(spos[2]),self.pzero[sidx],self.flk[sidx],self.pval_FLK[sidx]]
-                print(*tw,file=fout)
-
-    def write_hapflk(self,prefix):
-        ''' Write hapFLK results to 'prefix'.hapflk'''
-        assert(self.flk is not None)
-        with open(prefix+'.hapflk','w') as fout:
-            print('rs','chr','pos','hapflk','K',file=fout)
-            for sidx,s in enumerate(self.sorted_snps):
-                spos=self.carte.position(s.name)
-                tw=[s.name,spos[0],int(spos[2]),self.hapflk[sidx],self.kfrq.shape[1]]
-                print(*tw,file=fout)
-
-    
- 
+                            print(
+                                self.pops[ipop],
+                                s.name,
+                                int(spos[2]),
+                                ik,
+                                self.kfrq[ifit, ik, ipop, i],
+                                file=fout,
+                            )
+
+    def write_flk(self, prefix):
+        """Write FLK results to 'prefix'.flk"""
+        assert self.flk is not None
+        with open(prefix + ".flk", "w") as fout:
+            print("rs", "chr", "pos", "pzero", "flk", "pvalue", file=fout)
+            for sidx, s in enumerate(self.sorted_snps):
+                spos = self.carte.position(s.name)
+                tw = [
+                    s.name,
+                    spos[0],
+                    int(spos[2]),
+                    self.pzero[sidx],
+                    self.flk[sidx],
+                    self.pval_FLK[sidx],
+                ]
+                print(*tw, file=fout)
+
+    def write_hapflk(self, prefix):
+        """Write hapFLK results to 'prefix'.hapflk"""
+        assert self.flk is not None
+        with open(prefix + ".hapflk", "w") as fout:
+            print("rs", "chr", "pos", "hapflk", "K", file=fout)
+            for sidx, s in enumerate(self.sorted_snps):
+                spos = self.carte.position(s.name)
+                tw = [
+                    s.name,
+                    spos[0],
+                    int(spos[2]),
+                    self.hapflk[sidx],
+                    self.kfrq.shape[1],
+                ]
+                print(*tw, file=fout)
+
+
+def run_hapflk():
+    counter = utils.Stepper()
+    myopts = HapFLK.get_opts(sys.argv)
+    ## Load hapFLK data
+    if myopts.dbfile is None:
+        counter.new("Setting up from command line")
+        myh = HapFLK.from_cmd_line(myopts)
+    else:
+        counter.new("Setting up from saved run in %s" % myopts.dbfile)
+        myh = HapFLK.from_db_file(myopts.dbfile)
+    ## Run tests
+    counter.new("Running Tests")
+    myh.run_tests(myopts)
+    counter.new("Saving run in %s" % myopts.prefix + ".db")
+    myh.savedb(myopts.prefix)
+    counter.end()
```

### Comparing `hapflk-2.0.dev2/hapflk/hapflkadapt.py` & `hapflk-2.1/hapflk/hapflkadapt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,140 @@
-from __future__ import print_function, division
+import argparse
 import sys
 import numpy as np
 import scipy.stats as ss
-from scipy.stats import chi2,norm, multivariate_normal
+from scipy.stats import chi2, norm, multivariate_normal
 from scipy.stats import percentileofscore
 from scipy.optimize import minimize as optim
 from scipy import interpolate
 from numpy.linalg import multi_dot
-from multiprocessing import Pool
+from multiprocessing import Pool, cpu_count
+from hapflk import utils, hapflk
+from hapflk import InputOutput as IO
 
 #### Base functions for parallel computations (to put into own file)
 def pscore(args):
     a, val = args
-    return percentileofscore(a,val,kind='weak')
+    return percentileofscore(a, val, kind="weak")
 
-def loglik_h0_qfunc(pzero,p,Vinv):
-    ll = - p.shape[0] * np.log( pzero * (1-pzero))
+
+def loglik_h0_qfunc(pzero, p, Vinv):
+    ll = -p.shape[0] * np.log(pzero * (1 - pzero))
     res = p - pzero
-    ll -= multi_dot( (res.T, Vinv, res) ) / (pzero * (1-pzero))
+    ll -= multi_dot((res.T, Vinv, res)) / (pzero * (1 - pzero))
     return -ll
 
+
 def root_pzero_h0(args):
     p, pini, Vinv = args
-    res = optim(loglik_h0_qfunc, pini, args=( p, Vinv), method='SLSQP', bounds = [ (0,1) ],options = {'maxiter':20})
+    res = optim(
+        loglik_h0_qfunc,
+        pini,
+        args=(p, Vinv),
+        method="SLSQP",
+        bounds=[(0, 1)],
+        options={"maxiter": 20},
+    )
     if not res.success:
         ## we do it by hand
-        xx = np.linspace(np.min(p),np.max(p),100) ## pzero should be between min(p) and max(p)
-        ll = [ loglik_h0_qfunc( pz, p, Vinv) for pz in xx]
+        xx = np.linspace(np.min(p), np.max(p), 100)  ## pzero should be between min(p) and max(p)
+        ll = [loglik_h0_qfunc(pz, p, Vinv) for pz in xx]
         ill = np.argmin(ll)
         if ill == 0:
-            xx = np.linspace(0,np.min(p),100)
-            ll =  [ loglik_h0_qfunc( pz, p, Vinv) for pz in xx]
+            xx = np.linspace(0, np.min(p), 100)
+            ll = [loglik_h0_qfunc(pz, p, Vinv) for pz in xx]
             ill = np.argmin(ll)
         elif ill == 99:
-            xx = np.linspace(np.max(p),1,100)
-            ll =  [ loglik_h0_qfunc( pz, p, Vinv) for pz in xx]
+            xx = np.linspace(np.max(p), 1, 100)
+            ll = [loglik_h0_qfunc(pz, p, Vinv) for pz in xx]
             ill = np.argmin(ll)
-        res = xx[ ill ]
+        res = xx[ill]
         return (res, 0)
     else:
         return (res.x[0], 1)
-                    
-def loglik_h1_qfunc(pzero,p,xVinv,jacobian,x,Vinv):
-    '''Optimization function to minimize -logLikelihood (i.e. maximize logLikelihood) '''
-    #num = np.dot( xVinv, p-pzero)
-    beta = multi_dot( (jacobian, xVinv, p-pzero))
-    ll = - p.shape[0] * np.log( pzero * (1-pzero))
-    res = ( p - pzero - np.dot(x, beta) )
-    ll -= multi_dot( (res.T, Vinv, res) ) / (pzero * (1-pzero))
+
+
+def loglik_h1_qfunc(pzero, p, xVinv, jacobian, x, Vinv):
+    """Optimization function to minimize -logLikelihood (i.e. maximize logLikelihood)"""
+    # num = np.dot( xVinv, p-pzero)
+    beta = multi_dot((jacobian, xVinv, p - pzero))
+    ll = -p.shape[0] * np.log(pzero * (1 - pzero))
+    res = p - pzero - np.dot(x, beta)
+    ll -= multi_dot((res.T, Vinv, res)) / (pzero * (1 - pzero))
     return -ll
 
+
 def root_pzero(args):
     p, pini, xVinv, denum, x, Vinv = args
-    res = optim(loglik_h1_qfunc,pini, args=(p,xVinv,denum,x,Vinv),method='SLSQP', bounds = [ (0,1) ],options = {'maxiter':20})
+    res = optim(
+        loglik_h1_qfunc,
+        pini,
+        args=(p, xVinv, denum, x, Vinv),
+        method="SLSQP",
+        bounds=[(0, 1)],
+        options={"maxiter": 20},
+    )
     if not res.success:
         ## we do it by hand
-        xx = np.linspace(np.min(p),np.max(p),100) ## pzero should be between min(p) and max(p)
-        ll = [ loglik_h1_qfunc(pz, p, xVinv,denum,x,Vinv) for pz in xx]
+        xx = np.linspace(np.min(p), np.max(p), 100)  ## pzero should be between min(p) and max(p)
+        ll = [loglik_h1_qfunc(pz, p, xVinv, denum, x, Vinv) for pz in xx]
         ill = np.argmin(ll)
         if ill == 0:
-            xx = np.linspace(1e-4,np.min(p),100)
-            ll =  [ loglik_h1_qfunc( pz, p,xVinv,denum,x, Vinv) for pz in xx]
+            xx = np.linspace(1e-4, np.min(p), 100)
+            ll = [loglik_h1_qfunc(pz, p, xVinv, denum, x, Vinv) for pz in xx]
             ill = np.argmin(ll)
         elif ill == 99:
-            xx = np.linspace(np.max(p),0.9999,100)
-            ll =  [ loglik_h1_qfunc( pz, p,xVinv,denum,x, Vinv) for pz in xx]
+            xx = np.linspace(np.max(p), 0.9999, 100)
+            ll = [loglik_h1_qfunc(pz, p, xVinv, denum, x, Vinv) for pz in xx]
             ill = np.argmin(ll)
-        res = xx[ ill ]
+        res = xx[ill]
         return (res, 0)
     else:
         return (res.x[0], 1)
-    
-def beta_h1(pzero,p,xVinv, denum):
-    num = np.dot( xVinv, (p-pzero) )
-    beta = np.dot( denum, num)
+
+
+def beta_h1(pzero, p, xVinv, denum):
+    num = np.dot(xVinv, (p - pzero))
+    beta = np.dot(denum, num)
     return beta
 
+
 def calc_beta_h1(args):
     pzero, p, xVinv, denum = args
-    return beta_h1(pzero,p,xVinv, denum)
+    return beta_h1(pzero, p, xVinv, denum)
+
 
-def loglik_h1( pzero, beta, frq, x, Vinv):
+def loglik_h1(pzero, beta, frq, x, Vinv):
     npop = x.shape[0]
-    ll   = - npop * np.log( pzero * (1-pzero))
-    res  = ( frq - pzero - np.dot(x, beta) )
-    ll  -= multi_dot( ( res.T, Vinv, res)) / (pzero * (1-pzero))
+    ll = -npop * np.log(pzero * (1 - pzero))
+    res = frq - pzero - np.dot(x, beta)
+    ll -= multi_dot((res.T, Vinv, res)) / (pzero * (1 - pzero))
     return ll
 
+
 def calc_loglik_h1(args):
     pzero, beta, p, x, Vinv = args
-    return loglik_h1(pzero,beta,p,x,Vinv)
+    return loglik_h1(pzero, beta, p, x, Vinv)
+
 
 def loglik_h0(p, w, Vinv):
-    npop=p.shape[0]
-    pzero_hat = np.dot( w.T, p)
+    npop = p.shape[0]
+    pzero_hat = np.dot(w.T, p)
     ##pzero_hat = self.xx[ np.argmin( np.abs( pzero_hat - self.xx) ) ]
-    ll = - npop * np.log( pzero_hat * (1 - pzero_hat))
-    res = (p - pzero_hat)
-    ll -= np.dot( res.T, np.dot( Vinv, res ) ) / (pzero_hat * (1 - pzero_hat) )
+    ll = -npop * np.log(pzero_hat * (1 - pzero_hat))
+    res = p - pzero_hat
+    ll -= np.dot(res.T, np.dot(Vinv, res)) / (pzero_hat * (1 - pzero_hat))
     return ll
 
+
 def calc_loglik_h0(args):
     p, w, Vinv = args
     return loglik_h0(p, w, Vinv)
 
+
 def calc_lrt(args):
     p, xVinv, denum, x, Vinv, w = args
     #### H1 Calculations
     # pini = np.mean(p)
     # res = optim(loglik_h1_qfunc, pini, args=(p, xVinv, denum, x, Vinv), method='SLSQP', bounds = [ (0,1) ],options = {'maxiter':20})
     # if not res.success:
     #     ## we do it by hand
@@ -119,697 +146,903 @@
     ## beta
     pbar = np.mean(p)
     if (pbar < 1e-3) or (pbar > 0.999):
         pzero = pbar
         succ1 = 1
         beta = np.zeros(x.shape[1])
         ll1 = 0
-        pzero_null=pbar
+        pzero_null = pbar
         ll0 = 0
         succ0 = 1
     else:
-        pzero, succ1 = root_pzero( [ p, pbar, xVinv, denum, x, Vinv ])
-        beta = multi_dot( (denum, xVinv, p-pzero))
-        ll1 = -loglik_h1_qfunc( pzero, p, xVinv, denum, x, Vinv)
+        pzero, succ1 = root_pzero([p, pbar, xVinv, denum, x, Vinv])
+        beta = multi_dot((denum, xVinv, p - pzero))
+        ll1 = -loglik_h1_qfunc(pzero, p, xVinv, denum, x, Vinv)
         #### H0 Calculations
-        pzero_null, succ0 = root_pzero_h0( (p, pbar, Vinv))
-        ll0 = -loglik_h0_qfunc( pzero_null, p, Vinv)
-    succ = ( ( succ0 == 1 ) and (succ1 ==1) and 1) or 0
+        pzero_null, succ0 = root_pzero_h0((p, pbar, Vinv))
+        ll0 = -loglik_h0_qfunc(pzero_null, p, Vinv)
+    succ = ((succ0 == 1) and (succ1 == 1) and 1) or 0
     lrt = ll1 - ll0
-    if lrt <0 :
+    if lrt < 0:
         lrt = 0
-    res_h0 = { 'llik': ll0, 'pzero': pzero_null, 'pzsucc': succ0}
-    res_h1 = { 'llik': ll1, 'pzero': pzero, 'beta': beta, 'pzsucc': succ1}
-    return { 'H0': res_h0, 'H1': res_h1, 'lrt':lrt, 'pvalue': chi2.sf( lrt, x.shape[1]),'pzsucc':succ }
+    res_h0 = {"llik": ll0, "pzero": pzero_null, "pzsucc": succ0}
+    res_h1 = {"llik": ll1, "pzero": pzero, "beta": beta, "pzsucc": succ1}
+    return {
+        "H0": res_h0,
+        "H1": res_h1,
+        "lrt": lrt,
+        "pvalue": chi2.sf(lrt, x.shape[1]),
+        "pzsucc": succ,
+    }
+
 
 def loglik_h0_ML(p, w, Vinv):
-    npop=p.shape[0]
-    pzero_hat,_ = root_pzero_h0( (p, np.mean(p), Vinv ))
-    ll = - npop * np.log( pzero_hat * (1 - pzero_hat))
-    res = (p - pzero_hat)
-    ll -= multi_dot( ( res.T, Vinv, res)) / (pzero_hat * (1 - pzero_hat) )
+    npop = p.shape[0]
+    pzero_hat, _ = root_pzero_h0((p, np.mean(p), Vinv))
+    ll = -npop * np.log(pzero_hat * (1 - pzero_hat))
+    res = p - pzero_hat
+    ll -= multi_dot((res.T, Vinv, res)) / (pzero_hat * (1 - pzero_hat))
     return ll
 
+
 def calc_lrt_ML_old(args):
     p, xVinv, denum, x, Vinv, w = args
     ## root_pzero
     pini = np.mean(p)
-    res = optim(loglik_h1_qfunc, pini, args=(p, xVinv, denum, x, Vinv), method='SLSQP', bounds = [ (0,1) ],options = {'maxiter':20})
+    res = optim(
+        loglik_h1_qfunc,
+        pini,
+        args=(p, xVinv, denum, x, Vinv),
+        method="SLSQP",
+        bounds=[(0, 1)],
+        options={"maxiter": 20},
+    )
     if not res.success:
         ## we do it by hand
-        xx = np.linspace(np.min(p),np.max(p),100) ## pzero has to be between min(p) and max(p)
-        ll = [ loglik_h1_qfunc(pz, p, xVinv,denum,x,Vinv) for pz in xx]
-        pzero = xx[ np.argmin(ll) ]
+        xx = np.linspace(np.min(p), np.max(p), 100)  ## pzero has to be between min(p) and max(p)
+        ll = [loglik_h1_qfunc(pz, p, xVinv, denum, x, Vinv) for pz in xx]
+        pzero = xx[np.argmin(ll)]
     else:
         pzero = res.x[0]
     ## beta
-    beta = multi_dot( (denum, xVinv, p-pzero))
-    ## LRT 
-    ll1 = loglik_h1( pzero, beta, p, x, Vinv)
-    ll0 = loglik_h0_ML( p, w, Vinv)
-    return { 'pzero': np.dot(w.T, p), 'lrt':ll1 - ll0}
+    beta = multi_dot((denum, xVinv, p - pzero))
+    ## LRT
+    ll1 = loglik_h1(pzero, beta, p, x, Vinv)
+    ll0 = loglik_h0_ML(p, w, Vinv)
+    return {"pzero": np.dot(w.T, p), "lrt": ll1 - ll0}
 
 
 def bayes_factor_vect(p, xx, logdet_omega, logdet_nu, logdet_V, beta_mean_fact, omega_inv, Vinv):
     npop = p.shape[0]
     if len(p.shape) == 1:
-        frq = p.reshape( npop, 1)
-    else: 
+        frq = p.reshape(npop, 1)
+    else:
         frq = p
     ns = frq.shape[1]
-    pzero = np.broadcast_to( xx, ( ns, len(xx)) )
+    pzero = np.broadcast_to(xx, (ns, len(xx)))
 
     ## scaling factor
-    lp = - npop * np.log( pzero * (1-pzero))
+    lp = -npop * np.log(pzero * (1 - pzero))
     lp_1 = lp + logdet_omega - logdet_nu - logdet_V
     lp_0 = lp - logdet_V
     ## SNP Sum of Squares
     res = (frq - pzero).T
-    res=res.reshape( len(xx), npop, ns)
-    postmean = np.einsum( 'ij,kjl->kil', beta_mean_fact, res)
-    betass = np.einsum( 'ij,kjl->kil', omega_inv, postmean)
-    BT = np.einsum('ijk->ikj',postmean)
-    betass = np.einsum( 'ijk,ikj->i',BT,betass)
-    datass=np.einsum('ij,kjl->kil',Vinv,res)
-    RT=np.einsum('ijk->ikj',res)
-    datass=np.einsum('ijk,ikj->i',RT,datass)
+    res = res.reshape(len(xx), npop, ns)
+    postmean = np.einsum("ij,kjl->kil", beta_mean_fact, res)
+    betass = np.einsum("ij,kjl->kil", omega_inv, postmean)
+    BT = np.einsum("ijk->ikj", postmean)
+    betass = np.einsum("ijk,ikj->i", BT, betass)
+    datass = np.einsum("ij,kjl->kil", Vinv, res)
+    RT = np.einsum("ijk->ikj", res)
+    datass = np.einsum("ijk,ikj->i", RT, datass)
     ## compute Bayes Factor
-    lp_0 -= datass / (pzero * (1-pzero))
-    lp_1 -= ( datass - betass) / ( pzero * ( 1 - pzero))
+    lp_0 -= datass / (pzero * (1 - pzero))
+    lp_1 -= (datass - betass) / (pzero * (1 - pzero))
     vmax0 = np.max(lp_0)
-    P0 = np.log( np.sum( np.exp( lp_0 - vmax0) ) ) + vmax0
+    P0 = np.log(np.sum(np.exp(lp_0 - vmax0))) + vmax0
     vmax1 = np.max(lp_1)
-    P1 = np.log( np.sum( np.exp( lp_1 - vmax1) ) ) + vmax1
-    return (P1-P0)/np.log(10)
-    
+    P1 = np.log(np.sum(np.exp(lp_1 - vmax1))) + vmax1
+    return (P1 - P0) / np.log(10)
+
+
 def calc_bf(args):
     p, xx, logdet_omega, logdet_nu, logdet_V, beta_mean_fact, omega_inv, Vinv = args
     pbar = np.mean(p)
     if (pbar < 1e-2) or (pbar > 0.99):
         return 0
-    return bayes_factor_vect(p, xx, logdet_omega, logdet_nu, logdet_V, beta_mean_fact, omega_inv, Vinv)
+    return bayes_factor_vect(
+        p, xx, logdet_omega, logdet_nu, logdet_V, beta_mean_fact, omega_inv, Vinv
+    )
+
 
 def average_log10bf(logbf):
-    '''Computes the average of a list of log10(bf)'''
+    """Computes the average of a list of log10(bf)"""
     vmax = np.max(logbf)
-    bfm = np.log10( np.mean( np.power(10, logbf - vmax))) + vmax 
+    bfm = np.log10(np.mean(np.power(10, logbf - vmax))) + vmax
     return bfm
 
+
 def stdize_covar(x):
     try:
         ncovar = x.shape[1]
     except IndexError:
-        x = x.reshape( x.shape[0], 1)
+        x = x.reshape(x.shape[0], 1)
         ncovar = 1
     assert len(x.shape) == 2
     sx = np.zeros(x.shape)
     for ic in range(ncovar):
-        m = np.mean( x[ :, ic])
-        s = np.std( x[ :, ic], ddof=1)
-        assert s>0
-        sx[:, ic] = (x[ :, ic] - m)/s
+        m = np.mean(x[:, ic])
+        s = np.std(x[:, ic], ddof=1)
+        assert s > 0
+        sx[:, ic] = (x[:, ic] - m) / s
     return sx
-        
+
+
 ###### MAIN Class
 class FLKadapt(object):
-    def __init__( self, kinship, x, prefix = 'hapflkadapt', pz_step=0.01, ncpu=4, stdize=True):
-        self.prefix=prefix
-        self.standardized=False
+    def __init__(self, kinship, x, prefix="hapflkadapt", pz_step=0.01, ncpu=4, stdize=True):
+        self.prefix = prefix
+        self.standardized = False
         if stdize:
             self.standardized = True
-            self.x = ss.zscore(x, axis=0, ddof=1) #stdize_covar(x)
+            self.x = ss.zscore(x, axis=0, ddof=1)  # stdize_covar(x)
         else:
             self.x = x - np.mean(x, axis=0)
             ##print("Covariables not standardized, proceed with care ... ")
         self.F = kinship
-        self.diagFbar = np.mean( np.diag( self.F)) ## average distance to root
-        _,self.logdet_V = np.linalg.slogdet( self.F)
-        self.U,self.S,_ = np.linalg.svd(self.F)
+        self.diagFbar = np.mean(np.diag(self.F))  ## average distance to root
+        _, self.logdet_V = np.linalg.slogdet(self.F)
+        self.U, self.S, _ = np.linalg.svd(self.F)
         self.df = self.x.shape[1]
-        self.Vinv = np.linalg.inv(self.F) 
-        self.xVinv = np.dot(self.x.T,self.Vinv) # x'Vinv
-        self.xVinvx = multi_dot( ( self.x.T, self.Vinv, self.x) )
-        self.denum = np.linalg.inv( self.xVinvx ) # ( x' Vinv x )^{-1}
-        self.npop=self.F.shape[0]
+        self.Vinv = np.linalg.inv(self.F)
+        self.xVinv = np.dot(self.x.T, self.Vinv)  # x'Vinv
+        self.xVinvx = multi_dot((self.x.T, self.Vinv, self.x))
+        self.denum = np.linalg.inv(self.xVinvx)  # ( x' Vinv x )^{-1}
+        self.npop = self.F.shape[0]
         self.un = np.ones(self.npop)
-        self.w = np.dot(self.Vinv,self.un.T)/multi_dot( ( self.un, self.Vinv, self.un.T))
-        self.pz_step=pz_step
-        self.xx = np.arange(pz_step,1,step=pz_step)
-        self.nproc=ncpu
-        self.logfile=sys.stdout
-        self.pool=None
+        self.w = np.dot(self.Vinv, self.un.T) / multi_dot((self.un, self.Vinv, self.un.T))
+        self.pz_step = pz_step
+        self.xx = np.arange(pz_step, 1, step=pz_step)
+        self.nproc = ncpu
+        self.logfile = sys.stdout
+        self.pool = None
         ## NULL calibrations
         self.bf_null = None
         self.correct_lrt = None
-        
+
     def __enter__(self):
         self.pool = Pool(self.nproc)
-        self.logfile = open(self.prefix+'.log','w')
+        self.logfile = open(self.prefix + ".log", "w")
         return self
 
-    def __exit__(self,*args):
+    def __exit__(self, *args):
         self.pool.terminate()
         self.logfile.close()
-        
+
     ## LRT Single SNP
-    def calibrate_null( self, nsim = 10000, pmin=0.02):
-        ''' 
+    def calibrate_null(self, nsim=10000, pmin=0.02):
+        """
         Create predictor of LRT correcting for inflation on low pzero values.
 
-        1. Simulate frequency data (p) from MVN (pzero, self.F * (p0 * (1-p0))) for 
+        1. Simulate frequency data (p) from MVN (pzero, self.F * (p0 * (1-p0))) for
            p0 in [pmin, 1-pmin], on a log10 scale
         2. Compute LRT(p,x|p0)
-        3. Adjust a spline on (x, LRT(p,x|p0)) and create a predictor f(LRT(p,x)) 
+        3. Adjust a spline on (x, LRT(p,x|p0)) and create a predictor f(LRT(p,x))
            that estimates #df of Chisq | p0
-        '''
+        """
         assert self.pool is not None
-        xp = 10**(np.linspace(np.log10(pmin),np.log10(0.5),20,endpoint=False))
+        xp = 10 ** (np.linspace(np.log10(pmin), np.log10(0.5), 20, endpoint=False))
         lrt_res = []
         bf_res = []
-        args=[]
+        args = []
         for pzero in xp:
-            pm = pzero * np.ones( self.npop)
-            mvnorm = multivariate_normal( mean=pm, cov=self.F*pzero*(1-pzero))
+            pm = pzero * np.ones(self.npop)
+            mvnorm = multivariate_normal(mean=pm, cov=self.F * pzero * (1 - pzero))
             frq = mvnorm.rvs(nsim)
-            frq[ frq < 0] = 0
-            frq[ frq > 1] = 1
+            frq[frq < 0] = 0
+            frq[frq > 1] = 1
             for isim in range(nsim):
-                args.append((frq[isim,], self.xVinv, self.denum, self.x, self.Vinv, self.w))
+                args.append(
+                    (
+                        frq[
+                            isim,
+                        ],
+                        self.xVinv,
+                        self.denum,
+                        self.x,
+                        self.Vinv,
+                        self.w,
+                    )
+                )
             # lrt_res += list( np.apply_along_axis( self.fit_loglik_optim, 1, frq, skip_small = False, correct = False))
-            bf_res += list(  np.apply_along_axis( self.bayes_factor, 1, frq))
+            bf_res += list(np.apply_along_axis(self.bayes_factor, 1, frq))
         lrt_res += self.pool.map(calc_lrt, args)
         x = []
         y = []
         for v in lrt_res:
-            if not np.isnan(v['lrt']):
-              x.append( v['H1']['pzero'])
-              x.append( 1-v['H1']['pzero'])
-              y.append( v['lrt'])
-              y.append( v['lrt'])
+            if not np.isnan(v["lrt"]):
+                x.append(v["H1"]["pzero"])
+                x.append(1 - v["H1"]["pzero"])
+                y.append(v["lrt"])
+                y.append(v["lrt"])
         x = np.array(x)
         y = np.array(y)
         idx = np.argsort(x)
-        knots = sorted( np.concatenate( [ xp, 1-xp]))[1:-1]
-        self.correct_lrt = interpolate.LSQUnivariateSpline(x[idx], y[idx],knots)
+        knots = sorted(np.concatenate([xp, 1 - xp]))[1:-1]
+        self.correct_lrt = interpolate.LSQUnivariateSpline(x[idx], y[idx], knots)
         self.bf_null = sorted(bf_res)
-        with open(self.prefix+'.calib','w') as f:
-            print('# LRT DF',file=f)
+        with open(self.prefix + ".calib", "w") as f:
+            print("# LRT DF", file=f)
             for xx in knots:
-                print(xx,self.correct_lrt(xx),file=f)
-            print('# BF percentiles',file=f)
-            ntot=len(xp)*nsim
-            probs=np.array([1.0/ntot, 1.0/nsim, 0.005, 0.01, 0.025, 0.05, 0.1, 0.5, 0.9, 0.95, 0.975, 0.99, 0.995, 1-1.0/nsim, 1-1.0/ntot])
-            pc = np.percentile(bf_res, q=100*probs)
-            for i,q in enumerate(probs):
-                print(q,pc[i],file=f)
-        
-    def beta_h1(self,pzero,p):
-        num = np.dot( self.xVinv, (p-pzero) )
+                print(xx, self.correct_lrt(xx), file=f)
+            print("# BF percentiles", file=f)
+            ntot = len(xp) * nsim
+            probs = np.array(
+                [
+                    1.0 / ntot,
+                    1.0 / nsim,
+                    0.005,
+                    0.01,
+                    0.025,
+                    0.05,
+                    0.1,
+                    0.5,
+                    0.9,
+                    0.95,
+                    0.975,
+                    0.99,
+                    0.995,
+                    1 - 1.0 / nsim,
+                    1 - 1.0 / ntot,
+                ]
+            )
+            pc = np.percentile(bf_res, q=100 * probs)
+            for i, q in enumerate(probs):
+                print(q, pc[i], file=f)
+
+    def beta_h1(self, pzero, p):
+        num = np.dot(self.xVinv, (p - pzero))
         beta = np.dot(self.denum, num)
         return beta
-    
-    def loglik_h1(self,pzero,p):
-        beta = self.beta_h1(pzero,p)
-        ll = - self.npop * np.log( pzero * (1-pzero))
-        res = ( p - pzero - np.dot(self.x, beta) )
-        ll -= np.dot( res.T, np.dot( self.Vinv, res) ) / (pzero * (1-pzero))
-        return {'llik': ll, 'beta': beta}
-    
-    def loglik_h0(self,p):
-        pzero_hat = np.dot( self.w.T, p)
+
+    def loglik_h1(self, pzero, p):
+        beta = self.beta_h1(pzero, p)
+        ll = -self.npop * np.log(pzero * (1 - pzero))
+        res = p - pzero - np.dot(self.x, beta)
+        ll -= np.dot(res.T, np.dot(self.Vinv, res)) / (pzero * (1 - pzero))
+        return {"llik": ll, "beta": beta}
+
+    def loglik_h0(self, p):
+        pzero_hat = np.dot(self.w.T, p)
         ##pzero_hat = self.xx[ np.argmin( np.abs( pzero_hat - self.xx) ) ]
-        ll = - self.npop * np.log( pzero_hat * (1 - pzero_hat))
-        res = (p - pzero_hat)
-        ll -= np.dot( res.T, np.dot( self.Vinv, res ) ) / (pzero_hat * (1 - pzero_hat) )
-        return {'llik': ll, 'pzero': pzero_hat}
+        ll = -self.npop * np.log(pzero_hat * (1 - pzero_hat))
+        res = p - pzero_hat
+        ll -= np.dot(res.T, np.dot(self.Vinv, res)) / (pzero_hat * (1 - pzero_hat))
+        return {"llik": ll, "pzero": pzero_hat}
 
-    def fit_loglik(self,p):
+    def fit_loglik(self, p):
         res_h0 = self.loglik_h0(p)
-        profile_h1 = [ self.loglik_h1(pz,p) for pz in self.xx ]
-        best_pz = np.argmax( [ x['llik'] for x in profile_h1 ] )
-        res_h1 = profile_h1[ best_pz ]
+        profile_h1 = [self.loglik_h1(pz, p) for pz in self.xx]
+        best_pz = np.argmax([x["llik"] for x in profile_h1])
+        res_h1 = profile_h1[best_pz]
         pzero_hat = self.xx[best_pz]
-        ## var_beta = self.denum*pzero_hat*(1-pzero_hat) # does'nt seem to work here 
-        res_h1.update( { 'pzero' : self.xx[best_pz] } )
-        lbd= (res_h1['llik']-res_h0['llik'])
-        if lbd<0:
-            lbd=np.nan
-        return {'H0': res_h0, 'H1': res_h1 ,'Lbd': lbd, 'pval': chi2.sf(lbd,self.df)}
+        ## var_beta = self.denum*pzero_hat*(1-pzero_hat) # does'nt seem to work here
+        res_h1.update({"pzero": self.xx[best_pz]})
+        lbd = res_h1["llik"] - res_h0["llik"]
+        if lbd < 0:
+            lbd = np.nan
+        return {"H0": res_h0, "H1": res_h1, "Lbd": lbd, "pval": chi2.sf(lbd, self.df)}
 
     def fit_loglik_optim_ML(self, p, skip_small=True):
         res_h0 = self.loglik_h0(p)
-        pz=res_h0['pzero']
-        if skip_small and (np.min([pz,1-pz]) < 0.05):
-            res_h1={ 'pzero': np.nan, 'llik': np.nan, 'beta': np.full((self.df),np.nan)}
-            lbd=np.nan
+        pz = res_h0["pzero"]
+        if skip_small and (np.min([pz, 1 - pz]) < 0.05):
+            res_h1 = {
+                "pzero": np.nan,
+                "llik": np.nan,
+                "beta": np.full((self.df), np.nan),
+            }
+            lbd = np.nan
         else:
-            val_h0,_ = root_pzero_h0( (p, res_h0['pzero'], self.Vinv))
-            res_h0['pzero'] = val_h0
-            res_h0['llik'] = -loglik_h0_qfunc( val_h0, p, self.Vinv)
-            val_h1,_ = root_pzero( ( p, val_h0, self.xVinv,self.denum,self.x,self.Vinv))
-            res_h1 = self.loglik_h1(val_h1,p)
-            res_h1.update({ 'pzero' : val_h1} )
-            lbd= (res_h1['llik']-res_h0['llik'])
+            val_h0, _ = root_pzero_h0((p, res_h0["pzero"], self.Vinv))
+            res_h0["pzero"] = val_h0
+            res_h0["llik"] = -loglik_h0_qfunc(val_h0, p, self.Vinv)
+            val_h1, _ = root_pzero((p, val_h0, self.xVinv, self.denum, self.x, self.Vinv))
+            res_h1 = self.loglik_h1(val_h1, p)
+            res_h1.update({"pzero": val_h1})
+            lbd = res_h1["llik"] - res_h0["llik"]
             ##print(pz, res_h0['pzero'], res_h1['pzero'], res_h0['llik'], res_h1['llik'], file=self.logfile)
             # if correct:
             #     df = self.correct_lrt( res_h0['pzero'])
             #     lbd = chi2.ppf( chi2.cdf( lbd, df = df), df = self.df)
             ##print(res_h0['pzero'],val_h1.x[0],val_h1.success,val_h1.nfev,val_h1.nit,lbd)
-        return {'H0': res_h0, 'H1': res_h1 ,'lrt': lbd, 'pvalue': chi2.sf(lbd,self.df)}
+        return {"H0": res_h0, "H1": res_h1, "lrt": lbd, "pvalue": chi2.sf(lbd, self.df)}
 
-    def FLKadapt(self, frq, skip_small = True):
+    def FLKadapt(self, frq, skip_small=True):
         try:
             npop, nsnp = frq.shape
         except:
             return self.fit_loglik_optim_ML(p, frq, skip_small)
-        args=[]
+        args = []
         for isnp in range(nsnp):
-                args.append((frq[:,isnp], self.xVinv, self.denum, self.x, self.Vinv, self.w))
+            args.append((frq[:, isnp], self.xVinv, self.denum, self.x, self.Vinv, self.w))
         lrt_res = self.pool.map(calc_lrt, args)
         return lrt_res
-  
-    def fit_loglik_optim(self,p,skip_small=True, correct = True):
-        ''' Numerical optimization of loglikelihood'''
+
+    def fit_loglik_optim(self, p, skip_small=True, correct=True):
+        """Numerical optimization of loglikelihood"""
         res_h0 = self.loglik_h0(p)
-        pz=res_h0['pzero']
-        if skip_small and (np.min([pz,1-pz]) < 0.05):
-            res_h1={ 'pzero': np.nan, 'llik': np.nan, 'beta': np.full((self.df),np.nan)}
-            lbd=np.nan
+        pz = res_h0["pzero"]
+        if skip_small and (np.min([pz, 1 - pz]) < 0.05):
+            res_h1 = {
+                "pzero": np.nan,
+                "llik": np.nan,
+                "beta": np.full((self.df), np.nan),
+            }
+            lbd = np.nan
         else:
-            val_h1 = optim(loglik_h1_qfunc,res_h0['pzero'], args=(p,self.xVinv,self.denum,self.x,self.Vinv),method='SLSQP', bounds = [ (0,1) ],options = {'maxiter':20})
-            res_h1 = self.loglik_h1(val_h1.x[0],p)
-            res_h1.update({ 'pzero' : val_h1.x[0]} )
-            lbd= (res_h1['llik']-res_h0['llik'])
+            val_h1 = optim(
+                loglik_h1_qfunc,
+                res_h0["pzero"],
+                args=(p, self.xVinv, self.denum, self.x, self.Vinv),
+                method="SLSQP",
+                bounds=[(0, 1)],
+                options={"maxiter": 20},
+            )
+            res_h1 = self.loglik_h1(val_h1.x[0], p)
+            res_h1.update({"pzero": val_h1.x[0]})
+            lbd = res_h1["llik"] - res_h0["llik"]
             if correct:
-                df = self.correct_lrt( res_h0['pzero'])
-                lbd = chi2.ppf( chi2.cdf( lbd, df = df), df = self.df)
+                df = self.correct_lrt(res_h0["pzero"])
+                lbd = chi2.ppf(chi2.cdf(lbd, df=df), df=self.df)
             ##print(res_h0['pzero'],val_h1.x[0],val_h1.success,val_h1.nfev,val_h1.nit,lbd)
-        return {'H0': res_h0, 'H1': res_h1 ,'Lbd': lbd, 'pvalue': chi2.sf(lbd,self.df)}
+        return {"H0": res_h0, "H1": res_h1, "Lbd": lbd, "pvalue": chi2.sf(lbd, self.df)}
 
     #### hapFLKadapt
-    def PCA_clust(self,kfrq):
-        E,K,R = kfrq.shape
-        Pbar = np.einsum('j,klj->kl',self.w,kfrq)
-        Pbar=np.kron(Pbar,np.ones(R)).reshape(E,K,R)
-        Pmat = np.concatenate(kfrq-Pbar).T
-        assert Pmat.shape == (R,E*K)
-        u,s,v = np.linalg.svd(Pmat)
-        print('Global Lbd',*self.S)
-        print('Local Lbd', *s)
-        with open('test_Qglob.txt','w') as f:
+    def PCA_clust(self, kfrq):
+        E, K, R = kfrq.shape
+        Pbar = np.einsum("j,klj->kl", self.w, kfrq)
+        Pbar = np.kron(Pbar, np.ones(R)).reshape(E, K, R)
+        Pmat = np.concatenate(kfrq - Pbar).T
+        assert Pmat.shape == (R, E * K)
+        u, s, v = np.linalg.svd(Pmat)
+        print("Global Lbd", *self.S)
+        print("Local Lbd", *s)
+        with open("test_Qglob.txt", "w") as f:
             for r in range(R):
-                print(*self.U[r,],file=f)
-        with open('test_Qloc.txt','w') as f:
+                print(
+                    *self.U[
+                        r,
+                    ],
+                    file=f
+                )
+        with open("test_Qloc.txt", "w") as f:
             for r in range(R):
-                print(*u[r,],file=f)
+                print(
+                    *u[
+                        r,
+                    ],
+                    file=f
+                )
         for pc in range(R):
             for r in range(R):
-                print(pc,u[r,pc],self.U[r,pc],self.x[r,0],file=self.logfile)
-    
-    def BF_clust(self,kfrq, pmin = 0.05, beta_priors = None):
+                print(pc, u[r, pc], self.U[r, pc], self.x[r, 0], file=self.logfile)
+
+    def BF_clust(self, kfrq, pmin=0.05, beta_priors=None):
         if beta_priors is None:
-            beta_priors = np.power( 10, np.linspace( -1, 0, 10))
-        
+            beta_priors = np.power(10, np.linspace(-1, 0, 10))
+
         assert self.pool is not None
         E, K, R = kfrq.shape
-        P = len( beta_priors)
+        P = len(beta_priors)
         args = []
-        Pbar = np.mean( kfrq, axis = 2)
-        subset = np.array( ( Pbar > pmin) & ( Pbar < (1-pmin)))
-        Keff = np.sum( subset, axis = 1)
-        ## compute logBF_k for each EM 
+        Pbar = np.mean(kfrq, axis=2)
+        subset = np.array((Pbar > pmin) & (Pbar < (1 - pmin)))
+        Keff = np.sum(subset, axis=1)
+        ## compute logBF_k for each EM
         for e in range(E):
             for k in range(K):
                 ## ajout boucle prior
-                for ip, nu in enumerate( beta_priors):
-                    self.set_beta_prior( var_prior = nu * self.diagFbar)
-                    args.append( ( kfrq[e,k,], self.xx, self.logdet_omega, self.logdet_nu, self.logdet_V, self.beta_mean_fact, self.omega_inv, self.Vinv))
-        logBFk =  np.array( self.pool.map( calc_bf, args))
-        logBFk = logBFk.reshape( E, K, P)
+                for ip, nu in enumerate(beta_priors):
+                    self.set_beta_prior(var_prior=nu * self.diagFbar)
+                    args.append(
+                        (
+                            kfrq[
+                                e,
+                                k,
+                            ],
+                            self.xx,
+                            self.logdet_omega,
+                            self.logdet_nu,
+                            self.logdet_V,
+                            self.beta_mean_fact,
+                            self.omega_inv,
+                            self.Vinv,
+                        )
+                    )
+        logBFk = np.array(self.pool.map(calc_bf, args))
+        logBFk = logBFk.reshape(E, K, P)
         # print("New locus")
         # with open('bf.profile','w') as fbf:
         #     print('e','k','pz','nu','Keff','logbf',file=fbf)
         #     for e in range(E):
         #         for k in range(K):
         #             if pmin < Pbar[e,k] < (1 - pmin) :
         #                 for ip, nu in enumerate( beta_priors):
         #                     print( e, k, Pbar[ e, k], nu, Keff[e], logBFk[ e, k, ip],file=fbf)
-                    
+
         ## only consider clusters which pmin < mean(pk) < pmin
         logBFe = np.zeros(E)
         for e in range(E):
             subK = range(K)
             for k in subK:
-                if pmin < Pbar[ e, k] < (1-pmin):
-                    logbfk_i =  average_log10bf( logBFk[ e, k, ])
-                    logBFe[e] += logbfk_i #average_log10bf( logBFk[ e, k, ] )
+                if pmin < Pbar[e, k] < (1 - pmin):
+                    logbfk_i = average_log10bf(
+                        logBFk[
+                            e,
+                            k,
+                        ]
+                    )
+                    logBFe[e] += logbfk_i  # average_log10bf( logBFk[ e, k, ] )
             ##print( e, logBFe[ e])
             # if Keff > 0:
             #     ## uniform prior on number of associated clusters
             #     logBFe[e] += Keff * np.log10( (Keff + 1)/( 2*Keff))
-        return average_log10bf( logBFe)
+        return average_log10bf(logBFe)
 
-    
     def hapflkadapt(self, kfrq):
         assert self.pool is not None
         assert self.correct_lrt is not None
-     
-        if len(kfrq.shape)==4:
+
+        if len(kfrq.shape) == 4:
             E, K, R, L = kfrq.shape
         elif len(kfrq.shape) == 3:
             return self.fit_loglik_clust_pz(kfrq)
         else:
             raise ValueError("Bad Shape for kfrq")
-        
-        LRT  = np.zeros( ( E, K, L))
-        Succ = np.zeros( ( E, K, L))
+
+        LRT = np.zeros((E, K, L))
+        Succ = np.zeros((E, K, L))
         args = []
         for e in range(E):
             for k in range(K):
                 for l in range(L):
-                    args.append( ( kfrq[e,k,:,l], self.xVinv, self.denum, self.x, self.Vinv, self.w))
-        res =  self.pool.map( calc_lrt, args)
-        
-        LRT = np.array( [ x['lrt'] for x in res])
-        Succ = np.array([ x['pzsucc'] for x in res])
-        
-        LRT = LRT.reshape(E,K,L)
-        Succ = Succ.reshape(E,K,L)
-        LRT = LRT*Succ
+                    args.append(
+                        (
+                            kfrq[e, k, :, l],
+                            self.xVinv,
+                            self.denum,
+                            self.x,
+                            self.Vinv,
+                            self.w,
+                        )
+                    )
+        res = self.pool.map(calc_lrt, args)
+
+        LRT = np.array([x["lrt"] for x in res])
+        Succ = np.array([x["pzsucc"] for x in res])
+
+        LRT = LRT.reshape(E, K, L)
+        Succ = Succ.reshape(E, K, L)
+        LRT = LRT * Succ
 
         hflka_res = []
         for l in range(L):
-            myLRT = LRT[:,:,l]
-            mykfrq = kfrq[:,:,:,l]
-            Pbar = np.einsum('j,klj->kl',self.w,mykfrq)
-            subset = np.array( ( Pbar > 0.05) & ( Pbar < 0.95))
+            myLRT = LRT[:, :, l]
+            mykfrq = kfrq[:, :, :, l]
+            Pbar = np.einsum("j,klj->kl", self.w, mykfrq)
+            subset = np.array((Pbar > 0.05) & (Pbar < 0.95))
             df_pbar = self.correct_lrt(Pbar)
-            df = np.sum( df_pbar*subset , axis=1)
-            lrt = np.sum( myLRT*subset, axis=1)
+            df = np.sum(df_pbar * subset, axis=1)
+            lrt = np.sum(myLRT * subset, axis=1)
             qchisq = chi2.sf(lrt, df)
-            zscores = -norm.ppf( qchisq)
+            zscores = -norm.ppf(qchisq)
             Ztot = np.mean(zscores)
-            hflka_res.append({ 'Z':Ztot, 'pvalue': norm.sf(Ztot), 'Z_mat': zscores})
+            hflka_res.append({"Z": Ztot, "pvalue": norm.sf(Ztot), "Z_mat": zscores})
         return hflka_res
 
-    def fit_loglik_clust_pz(self,kfrq):
-        '''
+    def fit_loglik_clust_pz(self, kfrq):
+        """
         Computes Likelihood Ratio Test of model:
 
-        kfrq = p0_k + X beta_k + e 
+        kfrq = p0_k + X beta_k + e
         e ~ N( 0, F. p0_k_1*(1-p0_k_1))
 
         against:
 
-        kfrq = p0_k + e 
+        kfrq = p0_k + e
         e ~ N( 0, F. p0_k_0*(1-p0_k_0))
         input:
-            -- kfrq: cluster frequencies ( E x K x R ) 
+            -- kfrq: cluster frequencies ( E x K x R )
             with E (Number of EM fits), K (number of clusters), R (number of pops)
-        '''
+        """
         assert self.pool is not None
         assert self.correct_lrt is not None
         E, K, R = kfrq.shape
         args = []
         for e in range(E):
             for k in range(K):
-                args.append( ( kfrq[e,k,], self.xVinv, self.denum, self.x, self.Vinv, self.w))
-        res =  self.pool.map( calc_lrt, args)
-        LRT = np.array( [ x['lrt'] for x in res])
-        Succ = np.array([ x['pzsucc'] for x in res])
-
-        LRT = LRT.reshape(E,K)
-        Succ = Succ.reshape(E,K)
-            
-        LRT = LRT*Succ
-        
-        Pbar = np.einsum('j,klj->kl',self.w,kfrq)
-        subset = np.array( ( Pbar > 0.05) & ( Pbar < 0.95))
+                args.append(
+                    (
+                        kfrq[
+                            e,
+                            k,
+                        ],
+                        self.xVinv,
+                        self.denum,
+                        self.x,
+                        self.Vinv,
+                        self.w,
+                    )
+                )
+        res = self.pool.map(calc_lrt, args)
+        LRT = np.array([x["lrt"] for x in res])
+        Succ = np.array([x["pzsucc"] for x in res])
+
+        LRT = LRT.reshape(E, K)
+        Succ = Succ.reshape(E, K)
+
+        LRT = LRT * Succ
+
+        Pbar = np.einsum("j,klj->kl", self.w, kfrq)
+        subset = np.array((Pbar > 0.05) & (Pbar < 0.95))
         df_pbar = self.correct_lrt(Pbar)
-        df = np.sum( df_pbar*subset , axis=1)
+        df = np.sum(df_pbar * subset, axis=1)
         # df = np.sum( subset , axis=1)
-        lrt = np.sum( LRT*subset, axis=1)
+        lrt = np.sum(LRT * subset, axis=1)
         qchisq = chi2.sf(lrt, df)
-        zscores = -norm.ppf( qchisq)
+        zscores = -norm.ppf(qchisq)
         Ztot = np.mean(zscores)
-        return({ 'Z':Ztot, 'pvalue': norm.sf(Ztot), 'Z_mat': zscores})
-  
-    def fit_loglik_clust(self,kfrq):
-        '''
+        return {"Z": Ztot, "pvalue": norm.sf(Ztot), "Z_mat": zscores}
+
+    def fit_loglik_clust(self, kfrq):
+        """
         Computes Likelihood Ratio Test of model :
 
-        kfrq = p0_k + X beta_k + e 
+        kfrq = p0_k + X beta_k + e
         e ~ N( 0, F . var_k_1)
-        
+
         against:
-        
+
         kfrq = p0_k + e
         e ~ N(0, F . var_k_0)
 
         input:
-        -- kfrq: cluster frequencies ( E x K x R ) 
+        -- kfrq: cluster frequencies ( E x K x R )
         with E (Number of EM fits), K (number of clusters), R (number of pops)
-        '''
-        E,K,R = kfrq.shape
+        """
+        E, K, R = kfrq.shape
         P = self.df
-        pk = kfrq.reshape( ( E, K, R, 1))
+        pk = kfrq.reshape((E, K, R, 1))
         ## MLE  under H1
-        unx = np.hstack( (self.un.reshape(R,1), self.x))
-        ### ( X' . Vinv . X)inv . (X' . Vinv) p 
-        Emat =  np.linalg.inv( multi_dot( [unx.T, self.Vinv, unx]) )
-        Emat = multi_dot( [ Emat, unx.T, self.Vinv] )
-        mles = np.einsum('ij,kljm->klim',Emat,pk)
+        unx = np.hstack((self.un.reshape(R, 1), self.x))
+        ### ( X' . Vinv . X)inv . (X' . Vinv) p
+        Emat = np.linalg.inv(multi_dot([unx.T, self.Vinv, unx]))
+        Emat = multi_dot([Emat, unx.T, self.Vinv])
+        mles = np.einsum("ij,kljm->klim", Emat, pk)
         ### yhat = X . B
-        fitted = np.einsum('ij,kljm->klim',unx,mles)
+        fitted = np.einsum("ij,kljm->klim", unx, mles)
         resid = pk - fitted
         ### (y - yhat)' Vinv (y - yhat)
-        RSS = np.einsum('ij,kljm->klim',self.Vinv,resid)
-        RSS = np.einsum('ijkl,ijkm->ijlm',resid,RSS)
-        mle_sigma=RSS/R
-        ll_h1 = -R*np.log(mle_sigma) - RSS/mle_sigma
+        RSS = np.einsum("ij,kljm->klim", self.Vinv, resid)
+        RSS = np.einsum("ijkl,ijkm->ijlm", resid, RSS)
+        mle_sigma = RSS / R
+        ll_h1 = -R * np.log(mle_sigma) - RSS / mle_sigma
         ## MLE under H0
-        _un = self.un.reshape(R,1)
-        Emat = np.linalg.inv( multi_dot( [_un.T, self.Vinv, _un]) )
-        Emat = multi_dot( [ Emat, _un.T, self.Vinv] )
-        mles_H0 = np.einsum('ij,kljm->klim',Emat,pk)
-        fitted_H0 = np.einsum('ij,kljm->klim',_un,mles_H0)
+        _un = self.un.reshape(R, 1)
+        Emat = np.linalg.inv(multi_dot([_un.T, self.Vinv, _un]))
+        Emat = multi_dot([Emat, _un.T, self.Vinv])
+        mles_H0 = np.einsum("ij,kljm->klim", Emat, pk)
+        fitted_H0 = np.einsum("ij,kljm->klim", _un, mles_H0)
         resid_H0 = pk - fitted_H0
-        RSS_H0 = np.einsum('ij,kljm->klim',self.Vinv,resid_H0)
-        RSS_H0 = np.einsum('ijkl,ijkm->ijlm',resid_H0,RSS_H0)
-        mle_sigma_H0 = RSS_H0/R
-        ll_h0 = -R*np.log(mle_sigma_H0) - RSS_H0/mle_sigma_H0
-
-        LRT = (ll_h1 - ll_h0).reshape(E,K)
-        LRT_av = np.mean(np.sum(LRT,axis=1))
-        return({ 'Lbd':LRT_av, 'pvalue': chi2.sf(LRT_av,df=K), 'LRT_mat': LRT})
-        
+        RSS_H0 = np.einsum("ij,kljm->klim", self.Vinv, resid_H0)
+        RSS_H0 = np.einsum("ijkl,ijkm->ijlm", resid_H0, RSS_H0)
+        mle_sigma_H0 = RSS_H0 / R
+        ll_h0 = -R * np.log(mle_sigma_H0) - RSS_H0 / mle_sigma_H0
+
+        LRT = (ll_h1 - ll_h0).reshape(E, K)
+        LRT_av = np.mean(np.sum(LRT, axis=1))
+        return {"Lbd": LRT_av, "pvalue": chi2.sf(LRT_av, df=K), "LRT_mat": LRT}
+
     ## Bayes Factors
-    def set_beta_prior(self,var_prior=0.1):
+    def set_beta_prior(self, var_prior=0.1):
         self.prior = True
         self.nu = var_prior
         ## 1 par
-        self.nuinv = np.diag([1/self.nu]*self.df)
-        self.logdet_nu = self.df * np.log(self.nu) 
+        self.nuinv = np.diag([1 / self.nu] * self.df)
+        self.logdet_nu = self.df * np.log(self.nu)
         self.omega_inv = self.nuinv + self.xVinvx
         self.omega = np.linalg.inv(self.omega_inv)
-        self.beta_mean_fact = np.dot( self.omega, self.xVinv)
-        _,self.logdet_omega = np.linalg.slogdet( self.omega)
-   
-    def bayes_factor_vect(self,p):
+        self.beta_mean_fact = np.dot(self.omega, self.xVinv)
+        _, self.logdet_omega = np.linalg.slogdet(self.omega)
+
+    def bayes_factor_vect(self, p):
         if len(p.shape) == 1:
-            frq = p.reshape( self.npop, 1)
-        else: 
+            frq = p.reshape(self.npop, 1)
+        else:
             frq = p
         ns = frq.shape[1]
-        pzero = np.broadcast_to( self.xx, ( ns, len(self.xx)) )
-        
+        pzero = np.broadcast_to(self.xx, (ns, len(self.xx)))
+
         ## scaling factor
-        lp = - self.npop * np.log( pzero * (1-pzero))
+        lp = -self.npop * np.log(pzero * (1 - pzero))
         lp_1 = lp + self.logdet_omega - self.logdet_nu - self.logdet_V
         lp_0 = lp - self.logdet_V
         ## SNP Sum of Squares
         res = (frq - pzero).T
-        res=res.reshape( len(self.xx), self.npop, ns)
-        postmean = np.einsum( 'ij,kjl->kil', self.beta_mean_fact, res)
-        betass = np.einsum( 'ij,kjl->kil', self.omega_inv, postmean)
-        BT = np.einsum('ijk->ikj',postmean)
-        betass = np.einsum( 'ijk,ikj->i',BT,betass)
-        datass=np.einsum('ij,kjl->kil',self.Vinv,res)
-        RT=np.einsum('ijk->ikj',res)
-        datass=np.einsum('ijk,ikj->i',RT,datass)
+        res = res.reshape(len(self.xx), self.npop, ns)
+        postmean = np.einsum("ij,kjl->kil", self.beta_mean_fact, res)
+        betass = np.einsum("ij,kjl->kil", self.omega_inv, postmean)
+        BT = np.einsum("ijk->ikj", postmean)
+        betass = np.einsum("ijk,ikj->i", BT, betass)
+        datass = np.einsum("ij,kjl->kil", self.Vinv, res)
+        RT = np.einsum("ijk->ikj", res)
+        datass = np.einsum("ijk,ikj->i", RT, datass)
         ## compute Bayes Factor
-        lp_0 -= datass / (pzero * (1-pzero))
-        lp_1 -= ( datass - betass) / ( pzero * ( 1 - pzero))
+        lp_0 -= datass / (pzero * (1 - pzero))
+        lp_1 -= (datass - betass) / (pzero * (1 - pzero))
         vmax0 = np.max(lp_0)
-        P0 = np.log( np.sum( np.exp( lp_0 - vmax0) ) ) + vmax0
+        P0 = np.log(np.sum(np.exp(lp_0 - vmax0))) + vmax0
         vmax1 = np.max(lp_1)
-        P1 = np.log( np.sum( np.exp( lp_1 - vmax1) ) ) + vmax1
-        return (P1-P0)/np.log(10)
+        P1 = np.log(np.sum(np.exp(lp_1 - vmax1))) + vmax1
+        return (P1 - P0) / np.log(10)
 
-    def bayes_factor(self,p, beta_priors = None ):
+    def bayes_factor(self, p, beta_priors=None):
         ## priors: variance of divergence in scale of drift units
         ## assumes covariables are standardized.
         if beta_priors is None:
-            beta_priors = np.power(10,np.linspace(-1,1,10))
+            beta_priors = np.power(10, np.linspace(-1, 1, 10))
         bf = np.zeros(len(beta_priors))
-        for i,nu in enumerate(beta_priors):
-            self.set_beta_prior( var_prior = nu * self.diagFbar )
-            bf[i] =  self.bayes_factor_vect(p)
+        for i, nu in enumerate(beta_priors):
+            self.set_beta_prior(var_prior=nu * self.diagFbar)
+            bf[i] = self.bayes_factor_vect(p)
         vmax = np.max(bf)
-        bf = np.log10( np.sum( np.power(10, bf - vmax))) + vmax
-        return bf - np.log10( len(beta_priors))
+        bf = np.log10(np.sum(np.power(10, bf - vmax))) + vmax
+        return bf - np.log10(len(beta_priors))
 
-    def bayesFLKadapt( self, frq, beta_priors = np.power( 10, np.linspace(-1,1,10) )):
-        npop,nsnp = frq.shape
+    def bayesFLKadapt(self, frq, beta_priors=np.power(10, np.linspace(-1, 1, 10))):
+        npop, nsnp = frq.shape
         P = len(beta_priors)
         args = []
-        for ip, nu in enumerate( beta_priors):
-            self.set_beta_prior( var_prior = nu*self.diagFbar)
+        for ip, nu in enumerate(beta_priors):
+            self.set_beta_prior(var_prior=nu * self.diagFbar)
             for s in range(nsnp):
-                args.append( (frq[:, s], self.xx, self.logdet_omega, self.logdet_nu, self.logdet_V, self.beta_mean_fact, self.omega_inv, self.Vinv))
-        logBF_t = np.array( self.pool.map( calc_bf, args))
-        logBF_t = logBF_t.reshape( P, nsnp)
-        logBF = self.pool.map( average_log10bf, logBF_t.T)
+                args.append(
+                    (
+                        frq[:, s],
+                        self.xx,
+                        self.logdet_omega,
+                        self.logdet_nu,
+                        self.logdet_V,
+                        self.beta_mean_fact,
+                        self.omega_inv,
+                        self.Vinv,
+                    )
+                )
+        logBF_t = np.array(self.pool.map(calc_bf, args))
+        logBF_t = logBF_t.reshape(P, nsnp)
+        logBF = self.pool.map(average_log10bf, logBF_t.T)
         return logBF
-            
-        
-    def bf_rank(self,val):
+
+    def bf_rank(self, val):
         assert self.pool is not None
         val = np.asarray(val)
-        args=[]
+        args = []
         for x in val:
-            args.append((self.bf_null,x))
+            args.append((self.bf_null, x))
         scores = self.pool.map(pscore, args)
-        scores = np.array( scores )
-        p = 1 - scores/100
-        p[ p==0] = 0.5/len(self.bf_null)
-        p[ p==1] =  1-0.5/len(self.bf_null)
+        scores = np.array(scores)
+        p = 1 - scores / 100
+        p[p == 0] = 0.5 / len(self.bf_null)
+        p[p == 1] = 1 - 0.5 / len(self.bf_null)
         return p
-        
-    def logprob(self,pzero,p):
-        ''' Computes log(p|pzero,x,Beta) under Beta=0 and Beta>0 
+
+    def logprob(self, pzero, p):
+        """Computes log(p|pzero,x,Beta) under Beta=0 and Beta>0
         Returns:
-            lp = [logp0,logp1] 
-        '''
+            lp = [logp0,logp1]
+        """
         ## scaling factor
-        lp = - self.npop * np.log( pzero * (1-pzero))
+        lp = -self.npop * np.log(pzero * (1 - pzero))
         lp_1 = lp + self.logdet_omega - self.logdet_nu - self.logdet_V
         lp_0 = lp - self.logdet_V
 
         ## SNP Sum of Squares
-        res = (p - pzero)
-        postmean = np.dot( self.beta_mean_fact, res )
-        betass = multi_dot( ( postmean.T, self.omega_inv, postmean) )
-        datass = multi_dot( ( res.T, self.Vinv, res ) )
-
-        lp_0 -= datass / ( pzero * ( 1 - pzero))
-        lp_1 -= ( datass - betass) / ( pzero * ( 1 - pzero))
-        return np.array([lp_0,lp_1])
-
- 
-        
-# if __name__ == '__main__':    
-#     #myh=HapFLK.from_db_file('../hapflkadapt/covkin.db')
-#     ##myh=HapFLK.from_db_file('./hapflk.db')
-#     #myh=HapFLK.from_db_file('../hapflkadapt/bta29.db')
-#     ##myh.kinship=myh.kinship+0.01*(np.trace(myh.kinship)/myh.npop)
-
-    
-#     # input_file='../hapflkadapt/bta29.db'
-#     try:
-#         input_file=sys.argv[1]
-#         output_file_prefix=input_file[:-3]+'_test'
-#     except IndexError:
-#         ##input_file='../hapflkadapt/BTA2.db'
-#         input_file='../hapflkadapt/bta29.db'
-#         output_file_prefix='test'
-#         print(input_file,output_file_prefix)
-#         myh=HapFLK.from_db_file(input_file)
-#         nullcov = norm.rvs(size=myh.npop)
-#         myh.counter.new('NULL Analysis')
-#         Covs=np.vstack([nullcov]).T
-#         with FLKadapt(myh.kinship, Covs, prefix='test',ncpu=16) as ffnull:
-#             ##ffnull.calibrate_null(nsim=1000)
-#             test_snps = range(0,myh.nsnp,1)
-#             myh.counter.new('hapFLKadapt')
-#             if myh.kfrq is not None:
-#                 #pass
-#                 # resnull_h = [ffnull.PCA_clust(myh.kfrq[:,:,:,i]) for i in range(200,myh.nsnp,20000)]
-#                 resnull_h = [ffnull.fit_loglik_clust_pz(myh.kfrq[:,:,:,i]) for i in test_snps]
-#                 # resnull_h = [ffnull.BF_clust(myh.kfrq[:,:,:,i]) for i in range(0,myh.nsnp,200)]
-#             # myh.counter.new('FLKadapt: BF Stat 2 pars')
-#             # bfnull2 = np.apply_along_axis(ffnull.bayes_factor_2pars,0,myh.frq)
-#             # myh.counter.new('LRT raw')
-#             # lrtraw = np.apply_along_axis(ffnull.fit_loglik_optim,0,myh.frq, correct = False)
-#             # myh.counter.new('LRT cor')
-#             # lrtcor = np.apply_along_axis(ffnull.fit_loglik_optim,0,myh.frq)
-#             myh.counter.new('LRT ML')
-#             lrtml = np.apply_along_axis(ffnull.fit_loglik_optim_ML,0,myh.frq)
-#             myh.counter.new('BF')
-#             bfnull  = np.apply_along_axis(ffnull.bayes_factor,0,myh.frq)
-#             # print(bfnull2.shape,lrtnull.shape,bfnull.shape)
-#             with open( 'test.out', 'w') as fout:
-#                 print( 'LRTr', 'pvalr', 'LRTc', 'pvalc', 'LRTML','pvalML', 'bf',  'Zh', 'pvalh', file=fout)
-#                 for ix,i in enumerate(test_snps):
-#                     print( lrtraw[i]['Lbd'], lrtraw[i]['pvalue'], lrtcor[i]['Lbd'], lrtcor[i]['pvalue'], lrtml[i]['Lbd'], lrtml[i]['pvalue'], bfnull[i], resnull_h[ix]['Z'], resnull_h[ix]['pvalue'], file=fout)
-#         myh.counter.end()
-#         sys.exit(0)
-            
-#     print(input_file,output_file_prefix)
-#     myh=HapFLK.from_db_file(input_file)
-    
-#     covdata=pd.read_table('../data/breed_phenotypes.txt',sep=' ')
-#     covpops=list(covdata.index)
-#     smscov=np.array( [ covdata.values[ covpops.index(p), 1] for p in myh.pops])
-#     smscov=(smscov-np.mean(smscov))/ np.std(smscov)
-#     prodcov=np.array( [ covdata.values[ covpops.index(p), 0] == 'Dairy' for p in myh.pops], dtype=np.int)
-    
-#     ## Stature
-#     myh.counter.new('Stature Analysis')
-#     Covs=np.vstack([smscov]).T
-#     with FLKadapt(myh.kinship, Covs, prefix = output_file_prefix, ncpu=16) as ffsms:
-#         myh.counter.new('Null Simulations')
-#         ffsms.calibrate_null()
-#         myh.counter.new('FLKadapt: LRT Stat')
-#         ressms = np.apply_along_axis(ffsms.fit_loglik_optim_ML,0,myh.frq)
-#         myh.counter.new('FLKadapt: BF Stat')
-#         bfsms = np.apply_along_axis(ffsms.bayes_factor,0,myh.frq)
-#         rankbfsms = ffsms.bf_rank(bfsms)
-#         if myh.kfrq is not None:
-#             myh.counter.new('hapFLKadapt')
-#             ressms_h = [ffsms.fit_loglik_clust_pz(myh.kfrq[:,:,:,i]) for i in range(myh.nsnp)]
-         
-#     ## Write out
-#     myh.counter.new('Writing results')
-#     with open(output_file_prefix+'_sms_opt.out','w') as fout:
-#         print('rs','chr','pos','pzero.null','bf', 'bfrank', 'LRT', 'pvalue', 'Zh', 'pvalueh', 'pzero','beta', file=fout)
-#         for i,d in enumerate(ressms):
-#             rs=myh.sorted_snps[i].name
-#             chrom,_,pos=myh.carte.position(rs)
-#             print( rs, chrom, int(pos), d['H0']['pzero'], bfsms[i], rankbfsms[i],  d['Lbd'],  d['pvalue'], ressms_h[i]['Z'], ressms_h[i]['pvalue'], d['H1']['pzero'], *d['H1']['beta'],  file=fout)
-
-#     ## Production
-#     myh.counter.new('Type Analysis')
-#     Covs=np.vstack([prodcov]).T
-#     with FLKadapt(myh.kinship, Covs, prefix = output_file_prefix, ncpu=16) as ffprod:
-#         myh.counter.new('Null Simulations')
-#         ffprod.calibrate_null()
-#         myh.counter.new('FLKadapt: LRT Stat')
-#         resprod = np.apply_along_axis( ffprod.fit_loglik_optim_ML, 0, myh.frq)
-#         myh.counter.new('FLKadapt: BF Stat')
-#         bfprod = np.apply_along_axis( ffprod.bayes_factor, 0, myh.frq)
-#         rankbfprod = ffprod.bf_rank(bfprod)
-#         if myh.kfrq is not None:
-#             myh.counter.new('hapFLKadapt')
-#             resprod_h = [ffprod.fit_loglik_clust_pz(myh.kfrq[:,:,:,i]) for i in range(myh.nsnp)]
-
-  
-#     myh.counter.new('Writing results')
-#     with open(output_file_prefix+'_prod_opt.out','w') as fout:
-#         print('rs','chr','pos','pzero.null','bf', 'bfrank', 'LRT', 'pvalue', 'Zh', 'pvalueh', 'pzero','beta', file=fout)
-#         for i,d in enumerate(resprod):
-#             rs=myh.sorted_snps[i].name
-#             chrom,_,pos=myh.carte.position(rs)
-#             print( rs, chrom, int(pos), d['H0']['pzero'], bfprod[i], rankbfprod[i], d['Lbd'],  d['pvalue'], resprod_h[i]['Z'], resprod_h[i]['pvalue'], d['H1']['pzero'], *d['H1']['beta'],  file=fout)
-#     print()
- 
-#     myh.counter.end()
+        res = p - pzero
+        postmean = np.dot(self.beta_mean_fact, res)
+        betass = multi_dot((postmean.T, self.omega_inv, postmean))
+        datass = multi_dot((res.T, self.Vinv, res))
+
+        lp_0 -= datass / (pzero * (1 - pzero))
+        lp_1 -= (datass - betass) / (pzero * (1 - pzero))
+        return np.array([lp_0, lp_1])
+
+
+def run_hapflkadapt():
+    counter = utils.Stepper()
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--flkdb", dest="dbfile", help="DB file created by hapflk", default=None)
+    parser.add_argument(
+        "-o",
+        "--prefix",
+        dest="prefix",
+        help="prefix for output files",
+        default="hapflkadapt_out",
+    )
+    parser.add_argument(
+        "-x",
+        "--ncpu",
+        dest="ncpu",
+        help="Number of threads ( default = number of CPU)",
+        default=cpu_count(),
+        type=int,
+    )
+    parser.add_argument(
+        "--std",
+        dest="std",
+        help="Standardize cofactors",
+        default=False,
+        action="store_true",
+    )
+    IO.populate_covariate_args(parser)
+
+    if len(sys.argv) < 2:
+        parser.print_help()
+        sys.exit(0)
+    myopts = parser.parse_args(sys.argv[1:])
+
+    counter.new("Loading FLK DB file")
+    flkmodel = hapflk.HapFLK.from_db_file(myopts.dbfile)
+
+    counter.new("Getting covariates information")
+    covdata = IO.get_covariates_matrix(myopts.covar_file, myopts.cov, myopts.qcov, flkmodel.pops)
+    ##print( covdata)
+
+    for f in covdata["cofactors"]:
+        counter.new(" Analysing cofactor %s" % f)
+        myprefix = myopts.prefix + "_" + f
+        niv = covdata["factor_levels"][f]
+        beta_names = ["beta_" + x for x in niv[1:]]
+        with hapflkadapt.FLKadapt(
+            flkmodel.kinship,
+            covdata["DesignMatrices"][f],
+            prefix=myprefix,
+            ncpu=myopts.ncpu,
+            stdize=myopts.std,
+        ) as flkadapt:
+            flkadapt.correct_lrt = lambda x: flkadapt.df
+            counter.new("Single SNP tests")
+            counter.new("BayesFLKadapt")
+            ##bflka = np.apply_along_axis( flkadapt.bayes_factor,0,flkmodel.frq)
+            bflka = flkadapt.bayesFLKadapt(flkmodel.frq)
+            counter.new("FLK adapt")
+            flka = flkadapt.FLKadapt(flkmodel.frq)
+            ##flka  = np.apply_along_axis( flkadapt.fit_loglik_optim_ML,0,flkmodel.frq)
+            if flkmodel.kfrq is not None:
+                counter.new("hapFLKadapt")
+                hflka = [
+                    flkadapt.fit_loglik_clust_pz(flkmodel.kfrq[:, :, :, i])
+                    for i in range(flkmodel.nsnp)
+                ]
+        with open(myprefix + ".flkadapt", "w") as fout:
+            print(
+                "rs",
+                "chr",
+                "pos",
+                "pzero.null",
+                "bf",
+                "L0",
+                "L1",
+                "LRT",
+                "pvalue",
+                "pzero",
+                *beta_names,
+                "converge",
+                file=fout
+            )
+            for i, d in enumerate(flka):
+                rs = flkmodel.sorted_snps[i].name
+                chrom, _, pos = flkmodel.carte.position(rs)
+                print(
+                    rs,
+                    chrom,
+                    int(pos),
+                    d["H0"]["pzero"],
+                    bflka[i],
+                    d["H0"]["llik"],
+                    d["H1"]["llik"],
+                    d["lrt"],
+                    d["pvalue"],
+                    d["H1"]["pzero"],
+                    *d["H1"]["beta"],
+                    d["pzsucc"],
+                    file=fout
+                )
+        if flkmodel.kfrq is not None:
+            with open(myprefix + ".hapflkadapt", "w") as fout:
+                print("rs", "chr", "pos", "Zh", "pvalueh", file=fout)
+                for i, d in enumerate(flka):
+                    rs = flkmodel.sorted_snps[i].name
+                    chrom, _, pos = flkmodel.carte.position(rs)
+                    print(
+                        rs,
+                        chrom,
+                        int(pos),
+                        hflka[i]["Z"],
+                        hflka[i]["pvalue"],
+                        file=fout,
+                    )
+
+    for f in covdata["covariables"]:
+        counter.new(" Analysing covariate %s" % f)
+        myprefix = myopts.prefix + "_" + f
+        with hapflkadapt.FLKadapt(
+            flkmodel.kinship,
+            covdata["DesignMatrices"][f],
+            prefix=myprefix,
+            ncpu=myopts.ncpu,
+        ) as flkadapt:
+            flkadapt.correct_lrt = lambda x: flkadapt.df
+            counter.new("Single SNP tests")
+            counter.new("BayesFLKadapt")
+            ##bflka = np.apply_along_axis( flkadapt.bayes_factor,0,flkmodel.frq)
+            bflka = flkadapt.bayesFLKadapt(flkmodel.frq)
+            counter.new("FLK adapt")
+            flka = flkadapt.FLKadapt(flkmodel.frq)
+            ##flka  = np.apply_along_axis( flkadapt.fit_loglik_optim_ML,0,flkmodel.frq)
+            if flkmodel.kfrq is not None:
+                counter.new("hapFLKadapt")
+                hflka = [
+                    flkadapt.fit_loglik_clust_pz(flkmodel.kfrq[:, :, :, i])
+                    for i in range(flkmodel.nsnp)
+                ]
+        with open(myprefix + ".flkadapt", "w") as fout:
+            print(
+                "rs",
+                "chr",
+                "pos",
+                "pzero.null",
+                "bf",
+                "L0",
+                "L1",
+                "LRT",
+                "pvalue",
+                "pzero",
+                "beta",
+                "converge",
+                file=fout,
+            )
+            for i, d in enumerate(flka):
+                rs = flkmodel.sorted_snps[i].name
+                chrom, _, pos = flkmodel.carte.position(rs)
+                print(
+                    rs,
+                    chrom,
+                    int(pos),
+                    d["H0"]["pzero"],
+                    bflka[i],
+                    d["H0"]["llik"],
+                    d["H1"]["llik"],
+                    d["lrt"],
+                    d["pvalue"],
+                    d["H1"]["pzero"],
+                    *d["H1"]["beta"],
+                    d["pzsucc"],
+                    file=fout
+                )
+        if flkmodel.kfrq is not None:
+            with open(myprefix + ".hapflkadapt", "w") as fout:
+                print("rs", "chr", "pos", "Zh", "pvalueh", file=fout)
+                for i, d in enumerate(flka):
+                    rs = flkmodel.sorted_snps[i].name
+                    chrom, _, pos = flkmodel.carte.position(rs)
+                    print(
+                        rs,
+                        chrom,
+                        int(pos),
+                        hflka[i]["Z"],
+                        hflka[i]["pvalue"],
+                        file=fout,
+                    )
+    counter.new("Done")
+    counter.end()
```

### Comparing `hapflk-2.0.dev2/hapflk/nj.py` & `hapflk-2.1/hapflk/nj.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,346 +1,379 @@
-''' Implementation of the Neighbour Joining Algorithm '''
+""" Implementation of the Neighbour Joining Algorithm """
 from __future__ import print_function
 import numpy as np
 from scipy.optimize import minimize as optim
 
-class Edge():
-    def __init__(self,node1,node2,length):
-        self.n1=node1
-        self.n2=node2
-        if (length>0):
-            self.l=length
+
+class Edge:
+    def __init__(self, node1, node2, length):
+        self.n1 = node1
+        self.n2 = node2
+        if length > 0:
+            self.l = length
         else:
-            self.l=1e-5
+            self.l = 1e-5
+
     def __str__(self):
-        return "%s -- [ %f ] -- %s"%(self.n1.label,self.l,self.n2.label)
-    
-class Node():
-    def __init__(self,label=''):
-        self.label=label
-        self.child=[] ## list of children nodes
-        self.f=[]     ## distance to children
-        self.parent=None ## parent node
-    def newickize(self,parent_distance):
-        ''' Create a newick representation of the node and its children'''
-        if len( self.child) == 0:
+        return "%s -- [ %f ] -- %s" % (self.n1.label, self.l, self.n2.label)
+
+
+class Node:
+    def __init__(self, label=""):
+        self.label = label
+        self.child = []  ## list of children nodes
+        self.f = []  ## distance to children
+        self.parent = None  ## parent node
+
+    def newickize(self, parent_distance):
+        """Create a newick representation of the node and its children"""
+        if len(self.child) == 0:
             name = self.label
         else:
-            name = ''
+            name = ""
         if self.parent is None:
-            tw=name
+            tw = name
         else:
-            tw=name+':'+str(parent_distance)
-        if len(self.child)==0:
-            return (tw)
+            tw = name + ":" + str(parent_distance)
+        if len(self.child) == 0:
+            return tw
         else:
-            subtrees= (sub.newickize(self.f[i]) for i,sub in enumerate(self.child))
-            return '(%s)%s' % (','.join(subtrees),tw)       
-    def grow_from_edges(self,cur_edges):
-        ''' Construct recursively a subtree from edges information '''
+            subtrees = (sub.newickize(self.f[i]) for i, sub in enumerate(self.child))
+            return "(%s)%s" % (",".join(subtrees), tw)
+
+    def grow_from_edges(self, cur_edges):
+        """Construct recursively a subtree from edges information"""
         ## we build a new tree: reset values
-        self.child=[]
-        self.f=[]
-        mye=[e for e in cur_edges if e.n1 is self or e.n2 is self]
-        if len(mye)==0:
+        self.child = []
+        self.f = []
+        mye = [e for e in cur_edges if e.n1 is self or e.n2 is self]
+        if len(mye) == 0:
             return
         for e in mye:
             try:
-                assert e.l>0
+                assert e.l > 0
             except AssertionError:
                 print("Warning: Negative branch length encountered in NJ")
                 raise
             if e.n1 is self:
                 self.child.append(e.n2)
                 self.f.append(e.l)
-                e.n2.parent=self
+                e.n2.parent = self
             elif e.n2 is self:
                 self.child.append(e.n1)
                 self.f.append(e.l)
-                e.n1.parent=self
+                e.n1.parent = self
             cur_edges.remove(e)
         for c in self.child:
             c.grow_from_edges(cur_edges)
         return
-    def get_fi(self,curval,res):
-        ''' Computes fi : distance from a tip to the root'''
-        if len(self.child)==0:
+
+    def get_fi(self, curval, res):
+        """Computes fi : distance from a tip to the root"""
+        if len(self.child) == 0:
             ## tip
-            res[self.label]=curval
+            res[self.label] = curval
         else:
-            for i,c in enumerate(self.child):
-                c.get_fi(curval+self.f[i],res)
+            for i, c in enumerate(self.child):
+                c.get_fi(curval + self.f[i], res)
         return
-    def distance_to_root(self,curval=0):
-        res=curval
+
+    def distance_to_root(self, curval=0):
+        res = curval
         if self.parent is not None:
-            res+=self.parent.f[self.parent.child.index(self)]
-            res+=self.parent.distance_to_root(curval)
+            res += self.parent.f[self.parent.child.index(self)]
+            res += self.parent.distance_to_root(curval)
             return res
         else:
             return 0
+
     def get_leaves(self):
-        ''' Returns a list of leaves (node instances) under self '''
-        if len(self.child)==0:
-            res=[self]
+        """Returns a list of leaves (node instances) under self"""
+        if len(self.child) == 0:
+            res = [self]
         else:
-            res=[]
+            res = []
             for c in self.child:
-                res+=c.get_leaves()
+                res += c.get_leaves()
         return res
-    def mrca(self,other):
-        ''' Identifies most recent common ancestor with other node'''
+
+    def mrca(self, other):
+        """Identifies most recent common ancestor with other node"""
         try:
-            assert len(self.child)==0 and len(other.child)==0
+            assert len(self.child) == 0 and len(other.child) == 0
         except AssertionError:
-            raise AssertionError('MRCA only applies to leaves')
-        anc=self.parent
+            raise AssertionError("MRCA only applies to leaves")
+        anc = self.parent
         while other not in anc.get_leaves():
-            anc=anc.parent
+            anc = anc.parent
             assert anc is not None
         return anc
-        
-###Optimization function to root the tree 
-def qfunc(h0,fi,hi):
-    return sum( (((1-fi)*h0-hi)/hi)**2)
-
-def qfunc_2pars(pars,tree,hzy):
-    h0=pars[0]
-    posroot=pars[1]
-    fi_tips=tree.calc_fi(posroot)
-    fi_opt=np.zeros(len(fi_tips),dtype=float)
-    hi_opt=np.zeros(len(fi_tips),dtype=float)
-    for i,pop in enumerate(fi_tips.keys()):
-        fi_opt[i]=fi_tips[pop]
-        hi_opt[i]=hzy[pop]
-    return(qfunc(h0,fi_opt,hi_opt))
 
-class Rooted_Tree():
+
+###Optimization function to root the tree
+def qfunc(h0, fi, hi):
+    return sum((((1 - fi) * h0 - hi) / hi) ** 2)
+
+
+def qfunc_2pars(pars, tree, hzy):
+    h0 = pars[0]
+    posroot = pars[1]
+    fi_tips = tree.calc_fi(posroot)
+    fi_opt = np.zeros(len(fi_tips), dtype=float)
+    hi_opt = np.zeros(len(fi_tips), dtype=float)
+    for i, pop in enumerate(fi_tips.keys()):
+        fi_opt[i] = fi_tips[pop]
+        hi_opt[i] = hzy[pop]
+    return qfunc(h0, fi_opt, hi_opt)
+
+
+class Rooted_Tree:
     def __init__(self):
-        self.root=None
-    def build_from_edges(self,edges,root_edge,outgroup=None):
-        ''' Builds a tree from a list of edges
-            If outgroup is specified, it allows to identify the root and is dropped from the tree.
-            Else, the root is  positioned in the center of root_edge.
-        '''
-        current_edges=[e for e in edges if e is not root_edge]
+        self.root = None
+
+    def build_from_edges(self, edges, root_edge, outgroup=None):
+        """Builds a tree from a list of edges
+        If outgroup is specified, it allows to identify the root and is dropped from the tree.
+        Else, the root is  positioned in the center of root_edge.
+        """
+        current_edges = [e for e in edges if e is not root_edge]
         if outgroup:
-            if root_edge.n1.label==outgroup:
-                self.root=root_edge.n2
-            elif root_edge.n2.label==outgroup:
-                self.root=root_edge.n1
+            if root_edge.n1.label == outgroup:
+                self.root = root_edge.n2
+            elif root_edge.n2.label == outgroup:
+                self.root = root_edge.n1
             else:
-                raise ValueError('Outgroup %s not found'%outgroup)
-            left_edges=[]
+                raise ValueError("Outgroup %s not found" % outgroup)
+            left_edges = []
             for e in current_edges:
                 ## find children and set their distances
-                if e.n1.label==self.root.label:
+                if e.n1.label == self.root.label:
                     self.root.child.append(e.n2)
                     self.root.f.append(e.l)
                     ##current_edges.remove(e)
-                elif e.n2.label==self.root.label:
+                elif e.n2.label == self.root.label:
                     self.root.child.append(e.n1)
                     self.root.f.append(e.l)
                     ##current_edges.remove(e)
                 else:
                     left_edges.append(e)
-            current_edges=left_edges
+            current_edges = left_edges
         else:
-            self.root=Node(label=root_edge.n1.label+'-'+root_edge.n2.label)
-            self.root.child=[root_edge.n1,root_edge.n2]
-            self.root.f=[0.5*root_edge.l,0.5*root_edge.l]
+            self.root = Node(label=root_edge.n1.label + "-" + root_edge.n2.label)
+            self.root.child = [root_edge.n1, root_edge.n2]
+            self.root.f = [0.5 * root_edge.l, 0.5 * root_edge.l]
         for c in self.root.child:
-            c.parent=self.root
+            c.parent = self.root
             c.grow_from_edges(current_edges)
+
     def newick(self):
         if self.root:
-            return self.root.newickize('')+';'
-    def shift_root(self,posroot):
-        root_edge_len=np.sum(self.root.f)
-        self.root.f[0]=posroot*root_edge_len
-        self.root.f[1]=(1-posroot)*root_edge_len
-    def calc_fi(self,posroot=None):
-        '''
+            return self.root.newickize("") + ";"
+
+    def shift_root(self, posroot):
+        root_edge_len = np.sum(self.root.f)
+        self.root.f[0] = posroot * root_edge_len
+        self.root.f[1] = (1 - posroot) * root_edge_len
+
+    def calc_fi(self, posroot=None):
+        """
         Get a dictionary of distances from tips to root.
-        optional parameter posroot (0<pos<1) adjusts the position 
+        optional parameter posroot (0<pos<1) adjusts the position
         of the root between its two children
-        '''
+        """
         if posroot:
             self.shift_root(posroot)
-        res={}
-        self.root.get_fi(0,res)
+        res = {}
+        self.root.get_fi(0, res)
         return res
-    def optim_h0(self,hzy):
-        fi_tips=self.calc_fi()
-        fi_opt=np.zeros(len(fi_tips),dtype=float)
-        hi_opt=np.zeros(len(fi_tips),dtype=float)
-        for i,pop in enumerate(fi_tips.keys()):
-            fi_opt[i]=fi_tips[pop]
-            hi_opt[i]=hzy[pop]
-        val=optim(qfunc,np.mean(hi_opt),args=(fi_opt,hi_opt))
+
+    def optim_h0(self, hzy):
+        fi_tips = self.calc_fi()
+        fi_opt = np.zeros(len(fi_tips), dtype=float)
+        hi_opt = np.zeros(len(fi_tips), dtype=float)
+        for i, pop in enumerate(fi_tips.keys()):
+            fi_opt[i] = fi_tips[pop]
+            hi_opt[i] = hzy[pop]
+        val = optim(qfunc, np.mean(hi_opt), args=(fi_opt, hi_opt))
         return val
-    def optim_root(self,hzy):
-        ''' Optimize root placement
+
+    def optim_root(self, hzy):
+        """Optimize root placement
         optim parameters: hzy_ancestral (0,0.5) , posroot(0,1)
-        '''
-        val=optim(qfunc_2pars,[0.25,0.5],args=(self,hzy),bounds=[ (0,0.5),(0,1) ] )
+        """
+        val = optim(qfunc_2pars, [0.25, 0.5], args=(self, hzy), bounds=[(0, 0.5), (0, 1)])
         return val
+
     def kinship(self):
-        ''' Returns the Kinship matrix of the leaves '''
-        leaves=self.root.get_leaves()
-        n=len(leaves)
-        kinship=np.zeros((n,n),dtype=float)
-        for i,l1 in enumerate(leaves):
-            kinship[i,i]=l1.distance_to_root()
-            for j in range(i+1,n):
-                anc=l1.mrca(leaves[j])
-                val=anc.distance_to_root()
-                if val<0:
-                    print('Warning: zeroing negative values in kinship')
-                    val=0
-                kinship[i,j]=val
-                kinship[j,i]=kinship[i,j]
-        return kinship,[l.label for l in leaves]
-    
-class NJ():
-    ''' Class Implementing the Neighbour Joining Algorithm
-    '''
-    def __init__(self,Distance,labels):
-        ''' 
-        Create an instance from a Distance Matrix n x n and a 
-        list of corresponding population albels '''
-        assert len(labels)==Distance.shape[0] and Distance.shape[0]==Distance.shape[1]
-        self.D=Distance
-        self.tips=[Node(x) for x in labels]
-        self.Dnodes=[x for x in self.tips]
-        self.edges=[]
-        
-    def _QfromD(self,D):
-        ''' Calculates Q-matrix from D.
-        Returns Q and (imax,jmax) the indices of smallest Q'''
-        n=D.shape[0]
-        rowsum=np.sum(D,axis=0)
-        Q=(n-2)*D
+        """Returns the Kinship matrix of the leaves"""
+        leaves = self.root.get_leaves()
+        n = len(leaves)
+        kinship = np.zeros((n, n), dtype=float)
+        for i, l1 in enumerate(leaves):
+            kinship[i, i] = l1.distance_to_root()
+            for j in range(i + 1, n):
+                anc = l1.mrca(leaves[j])
+                val = anc.distance_to_root()
+                if val < 0:
+                    print("Warning: zeroing negative values in kinship")
+                    val = 0
+                kinship[i, j] = val
+                kinship[j, i] = kinship[i, j]
+        return kinship, [l.label for l in leaves]
+
+
+class NJ:
+    """Class Implementing the Neighbour Joining Algorithm"""
+
+    def __init__(self, Distance, labels):
+        """
+        Create an instance from a Distance Matrix n x n and a
+        list of corresponding population albels"""
+        assert len(labels) == Distance.shape[0] and Distance.shape[0] == Distance.shape[1]
+        self.D = Distance
+        self.tips = [Node(x) for x in labels]
+        self.Dnodes = [x for x in self.tips]
+        self.edges = []
+
+    def _QfromD(self, D):
+        """Calculates Q-matrix from D.
+        Returns Q and (imax,jmax) the indices of smallest Q"""
+        n = D.shape[0]
+        rowsum = np.sum(D, axis=0)
+        Q = (n - 2) * D
         for i in range(n):
-            Q[:,i]-=rowsum[i]
-            Q[i,:]-=rowsum[i]
-            Q[i,i]=0
+            Q[:, i] -= rowsum[i]
+            Q[i, :] -= rowsum[i]
+            Q[i, i] = 0
         ## make sure the diagonal does not contain smallest value
-        Q+=np.diag(n*[np.max(Q)+1])
-        return Q,np.unravel_index(np.argmin(Q),Q.shape)
+        Q += np.diag(n * [np.max(Q) + 1])
+        return Q, np.unravel_index(np.argmin(Q), Q.shape)
 
-    def _get_new_D(self,D,pair):
-        '''Calculates a new distance matrix after joining the pair (i,j) into new node u 
-           and creating the 2 new corresponding edges.
-           return newD
-        '''
-        n=D.shape[0]
-        delta=np.zeros(2)
-        imin,jmin=pair
-        node1=self.Dnodes[imin]
-        node2=self.Dnodes[jmin]
-        node_intern=Node(label=node1.label+'-'+node2.label)
-        delta[0]=0.5*D[imin,jmin]+(0.5/(n-2))*(np.sum(D[imin,])-np.sum(D[jmin,]))
-        delta[1]=D[imin,jmin]-delta[0]
+    def _get_new_D(self, D, pair):
+        """Calculates a new distance matrix after joining the pair (i,j) into new node u
+        and creating the 2 new corresponding edges.
+        return newD
+        """
+        n = D.shape[0]
+        delta = np.zeros(2)
+        imin, jmin = pair
+        node1 = self.Dnodes[imin]
+        node2 = self.Dnodes[jmin]
+        node_intern = Node(label=node1.label + "-" + node2.label)
+        delta[0] = 0.5 * D[imin, jmin] + (0.5 / (n - 2)) * (
+            np.sum(
+                D[
+                    imin,
+                ]
+            )
+            - np.sum(
+                D[
+                    jmin,
+                ]
+            )
+        )
+        delta[1] = D[imin, jmin] - delta[0]
         ## create new edges
-        new_edge=Edge(node1,node_intern,delta[0] >0 and delta[0] or 1e-5)
+        new_edge = Edge(node1, node_intern, delta[0] > 0 and delta[0] or 1e-5)
         self.edges.append(new_edge)
-        new_edge=Edge(node2,node_intern,delta[1]>0 and delta[1] or 1e-5)
+        new_edge = Edge(node2, node_intern, delta[1] > 0 and delta[1] or 1e-5)
         self.edges.append(new_edge)
 
-        newD=np.zeros((n-1,n-1))
-        ind_left=[ i for i in range(n)]
+        newD = np.zeros((n - 1, n - 1))
+        ind_left = [i for i in range(n)]
         ind_left.remove(imin)
         ind_left.remove(jmin)
         self.Dnodes.remove(node1)
         self.Dnodes.remove(node2)
-        self.Dnodes=[node_intern]+self.Dnodes
-        newD[1:,1:]=D[ind_left,:][:,ind_left]
-        for newi,i in enumerate(ind_left):
-            newD[0,newi+1]=0.5*(D[imin,i]+D[jmin,i]-D[imin,jmin])
-            newD[newi+1,0]=newD[0,newi+1]
+        self.Dnodes = [node_intern] + self.Dnodes
+        newD[1:, 1:] = D[ind_left, :][:, ind_left]
+        for newi, i in enumerate(ind_left):
+            newD[0, newi + 1] = 0.5 * (D[imin, i] + D[jmin, i] - D[imin, jmin])
+            newD[newi + 1, 0] = newD[0, newi + 1]
         return newD
-    
+
     def fit(self):
-        '''
+        """
         Calculates the neighbor joining tree
         Sets up internal nodes and edges between nodes.
-        '''
-        curD=np.copy(self.D)
-        while curD.shape[0]>2:
-            # print('+++')        
-            Q,pair=self._QfromD(curD)
+        """
+        curD = np.copy(self.D)
+        while curD.shape[0] > 2:
+            # print('+++')
+            Q, pair = self._QfromD(curD)
             # print(Q,pair,sep='\n')
-            newD=self._get_new_D(curD,pair)
+            newD = self._get_new_D(curD, pair)
             # print(self.edges[-1])
             # print(self.edges[-2])
             # print(newD,sep='\n')
-            curD=newD
+            curD = newD
         ## terminate
-        new_edge=Edge(self.Dnodes[0],self.Dnodes[1],curD[0,1])
+        new_edge = Edge(self.Dnodes[0], self.Dnodes[1], curD[0, 1])
         self.edges.append(new_edge)
         # print(self.edges[-1])
 
-       
-    
+
 def test():
     ## Test distance matrix from wikipedia :)
     print("#### Wikipedia example ####\nsee https://en.wikipedia.org/wiki/Neighbor_joining")
-    Dtest=np.array([[0,5,9,9,8],
-                    [5,0,10,10,9],
-                    [9,10,0,8,7],
-                    [9,10,8,0,3],
-                    [8,9,7,3,0]])
-    labels=['a','b','c','d','e']
-    my_nj=NJ(Dtest,labels)
+    Dtest = np.array(
+        [[0, 5, 9, 9, 8], [5, 0, 10, 10, 9], [9, 10, 0, 8, 7], [9, 10, 8, 0, 3], [8, 9, 7, 3, 0]]
+    )
+    labels = ["a", "b", "c", "d", "e"]
+    my_nj = NJ(Dtest, labels)
     my_nj.fit()
     print("Edges from NJ:")
-    print(*my_nj.edges,sep='\n')
+    print(*my_nj.edges, sep="\n")
     print("#### Ovis  example ####")
-    Dsheep=2*np.array([[0.0, 0.052524410884, 0.479593743725, 0.15280193534],
-                     [0.052524410884 , 0.0 , 0.489188722484 ,0.162238830969],
-                     [0.479593743725 , 0.489188722484 , 0.0 , 0.423091249114],
-                     [0.15280193534 , 0.162238830969 , 0.423091249114 ,0.0]])
-    labels=['MOOA','IROA','Capra','IROO']
-    my_nj=NJ(Dsheep,labels)
+    Dsheep = 2 * np.array(
+        [
+            [0.0, 0.052524410884, 0.479593743725, 0.15280193534],
+            [0.052524410884, 0.0, 0.489188722484, 0.162238830969],
+            [0.479593743725, 0.489188722484, 0.0, 0.423091249114],
+            [0.15280193534, 0.162238830969, 0.423091249114, 0.0],
+        ]
+    )
+    labels = ["MOOA", "IROA", "Capra", "IROO"]
+    my_nj = NJ(Dsheep, labels)
     my_nj.fit()
     print("Edges from NJ:")
-    print(*my_nj.edges,sep='\n')
+    print(*my_nj.edges, sep="\n")
     ## remove outgroup
-    outgroup='Capra'
+    outgroup = "Capra"
     ## find edge from root
-    root_edge=[e for e in my_nj.edges if e.n1.label==outgroup or e.n2.label==outgroup][0]
-    tree=Rooted_Tree()
-    tree.build_from_edges(my_nj.edges,root_edge,outgroup=outgroup)
-    print("Outgroup Tree:",tree.newick())
-    Dsheep_nocapra=Dsheep[(0,1,3),:][:,(0,1,3)]
-    labels.remove('Capra')
-    my_nj=NJ(Dsheep_nocapra,labels)
+    root_edge = [e for e in my_nj.edges if e.n1.label == outgroup or e.n2.label == outgroup][0]
+    tree = Rooted_Tree()
+    tree.build_from_edges(my_nj.edges, root_edge, outgroup=outgroup)
+    print("Outgroup Tree:", tree.newick())
+    Dsheep_nocapra = Dsheep[(0, 1, 3), :][:, (0, 1, 3)]
+    labels.remove("Capra")
+    my_nj = NJ(Dsheep_nocapra, labels)
     my_nj.fit()
     print("\n")
-    print(*my_nj.edges,sep='\n')
-    hzy={'MOOA':0.2531,'IROA':0.2479,'IROO':0.2874}
-    resid=np.inf
-    root_edge_best=None
-    with open('sheep.tree','w') as ftree:
+    print(*my_nj.edges, sep="\n")
+    hzy = {"MOOA": 0.2531, "IROA": 0.2479, "IROO": 0.2874}
+    resid = np.inf
+    root_edge_best = None
+    with open("sheep.tree", "w") as ftree:
         for root_e in my_nj.edges:
-            the_edges=[e for e in my_nj.edges]
-            tree=Rooted_Tree()
-            tree.build_from_edges(the_edges,root_e)
+            the_edges = [e for e in my_nj.edges]
+            tree = Rooted_Tree()
+            tree.build_from_edges(the_edges, root_e)
             print(resid)
             # tree_fit=tree.optim_h0(hzy)
-            tree_fit=tree.optim_root(hzy)
-            print(tree_fit.x,tree_fit.fun)
-            if tree_fit.x[1]>0 and tree_fit.fun<resid:
-                resid=tree_fit.fun
-                root_edge_best=root_e
-                root_pos_best=tree_fit.x[1]
-    print("Found best tree with %f accuracy"%resid)
-    tree=Rooted_Tree()
-    tree.build_from_edges(my_nj.edges,root_edge_best)
+            tree_fit = tree.optim_root(hzy)
+            print(tree_fit.x, tree_fit.fun)
+            if tree_fit.x[1] > 0 and tree_fit.fun < resid:
+                resid = tree_fit.fun
+                root_edge_best = root_e
+                root_pos_best = tree_fit.x[1]
+    print("Found best tree with %f accuracy" % resid)
+    tree = Rooted_Tree()
+    tree.build_from_edges(my_nj.edges, root_edge_best)
     tree.shift_root(root_pos_best)
-    print("Optimized tree:",tree.newick())
-    kin,popnames=tree.kinship()
-    print(kin,*popnames)
-    
-if __name__=='__main__':
+    print("Optimized tree:", tree.newick())
+    kin, popnames = tree.kinship()
+    print(kin, *popnames)
+
+
+if __name__ == "__main__":
     test()
```

### Comparing `hapflk-2.0.dev2/hapflk/popgen.py` & `hapflk-2.1/hapflk/popgen.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,108 @@
 import sys
 import os
 import pickle
 import tempfile
 import numpy as np
-from scipy.stats import chi2,norm
+from scipy.stats import chi2, norm
 from hapflk import nj
 import warnings
 
-debug=False
+debug = False
 if not debug:
-    np.seterr(all='ignore')
-    warnings.filterwarnings('ignore',category=FutureWarning)
+    np.seterr(all="ignore")
+    warnings.filterwarnings("ignore", category=FutureWarning)
 
-def reynolds_multi_allelic(Mf,nloc,decompose=False):
-    '''
+
+def reynolds_multi_allelic(Mf, nloc, decompose=False):
+    """
     Compute Reynolds distances from multiallelic loci
 
     Parameters:
     -----------
-    
+
     Mf : numpy array of allele frequencies in populations
          rows are populations
          columns are allele frequencies, by loci
     nloc : number of loci
 
     Returns:
     --------
 
     dist : numpy array (n x n) of reynolds genetic distances
     numerator    : numerator of the Reynolds Distance
     denominator  : denominator of the Reynolds Distance
-    '''
-    npop=Mf.shape[0]
-    A=np.dot(Mf,Mf.T)
-    dist=np.zeros((npop,npop))
+    """
+    npop = Mf.shape[0]
+    A = np.dot(Mf, Mf.T)
+    dist = np.zeros((npop, npop))
     if decompose:
-        numerator=np.zeros((npop,npop))
-        denominator=np.zeros((npop,npop))
+        numerator = np.zeros((npop, npop))
+        denominator = np.zeros((npop, npop))
     else:
-        numerator=None
-        denominator=None
-    for i in range(npop-1):
-        for j in range(i+1,npop):
-            dist[i,j]=0.5*(A[i,i]+A[j,j]-2*A[i,j])/(nloc-A[i,j])
+        numerator = None
+        denominator = None
+    for i in range(npop - 1):
+        for j in range(i + 1, npop):
+            dist[i, j] = 0.5 * (A[i, i] + A[j, j] - 2 * A[i, j]) / (nloc - A[i, j])
             if decompose:
-                numerator[i,j]=A[i,i]+A[j,j]-2*A[i,j]
-                denominator[i,j]=2*(nloc-A[i,j])
-    dist=dist+dist.T
-    numerator=numerator+numerator.T
-    denominator=denominator+denominator.T
-    return dist,numerator,denominator
-   
+                numerator[i, j] = A[i, i] + A[j, j] - 2 * A[i, j]
+                denominator[i, j] = 2 * (nloc - A[i, j])
+    dist = dist + dist.T
+    numerator = numerator + numerator.T
+    denominator = denominator + denominator.T
+    return dist, numerator, denominator
+
+
 def reynolds(Mf):
-    '''
+    """
     Compute Reynolds distances from SNP allele frequencies
 
     Parameters:
     ----------------
 
     Mf : numpy array of allele frequencies in populations
           rows are populations (n), columns are markers (p).
 
     Returns:
     -----------
 
     dist : numpy array (n x n) of reynolds genetic distances
-    '''
-    npop,nloc=Mf.shape
-    dist=np.zeros((npop,npop))
-    A=np.dot(Mf,Mf.T)+np.dot((1-Mf),(1-Mf).T)
-    for i in range(npop-1):
-        for j in range(i+1,npop):
-            dist[i,j]=0.5*(A[i,i]+A[j,j]-2*A[i,j])/(nloc-A[i,j])
-    dist=dist+dist.T
+    """
+    npop, nloc = Mf.shape
+    dist = np.zeros((npop, npop))
+    A = np.dot(Mf, Mf.T) + np.dot((1 - Mf), (1 - Mf).T)
+    for i in range(npop - 1):
+        for j in range(i + 1, npop):
+            dist[i, j] = 0.5 * (A[i, i] + A[j, j] - 2 * A[i, j]) / (nloc - A[i, j])
+    dist = dist + dist.T
     return dist
 
+
 def heterozygosity(Mf):
-    '''
+    """
     Compute heterozygosity from SNP allele frequencies
     Parameters:
     ----------------
 
     Mf : numpy array of allele frequencies in populations
           rows are populations (n), columns are markers (p).
 
     Returns:
     -----------
 
     hzy : numpy array (n x 1) of mean heterozygosities
-    '''
-    npop,nloc=Mf.shape
-    hzy_func = lambda x: 2*x*(1-x)
-    return np.average(hzy_func(Mf),axis=1)
+    """
+    npop, nloc = Mf.shape
+    hzy_func = lambda x: 2 * x * (1 - x)
+    return np.average(hzy_func(Mf), axis=1)
 
-def popKinship_fromFile(file_name,popnames):
-    '''
+
+def popKinship_fromFile(file_name, popnames):
+    """
     Read population kinship matrix from file
 
     File format is :
 
     Pop1 a11 a12 ...
     Pop2 a21 a22 ....
 
@@ -109,42 +113,45 @@
     -----------
     file_name : name of the file to read kinship from
     popnames : name of the pop to find in the file (order is preserved)
 
     See Also:
     ---------
     popKinship for estimating the kinship matrix
-    '''
+    """
 
-    data=[x.split() for x in open(file_name).readlines()]
+    data = [x.split() for x in open(file_name).readlines()]
     ##popnames2=popnames[:]
     # if outgroup is not None:
     #     popnames2.remove(outgroup)
-    ordre=[popnames.index(x[0]) for x in data]
+    ordre = [popnames.index(x[0]) for x in data]
     if len(ordre) != len(data):
-        print( 'Not Enough populations in kinship file !')
+        print("Not Enough populations in kinship file !")
         raise ValueError
-    FF=np.zeros((len(popnames),len(popnames)),dtype=float)
+    FF = np.zeros((len(popnames), len(popnames)), dtype=float)
     for i in range(len(popnames)):
-        ix=ordre[i]
+        ix = ordre[i]
         for j in range(len(popnames)):
-            jx=ordre[j]
-            FF[ix,jx]=float(data[i][j+1])
+            jx = ordre[j]
+            FF[ix, jx] = float(data[i][j + 1])
     return FF
 
-def popKinship_new(D,popnames,outgroup=None,fprefix=None,keep_outgroup=False,hzy=None,dump_tree=True):
-    '''
+
+def popKinship_new(
+    D, popnames, outgroup=None, fprefix=None, keep_outgroup=False, hzy=None, dump_tree=True
+):
+    """
     Compute kinship matrix between populations
 
     Parameters:
     ---------------
 
     D : Reynolds distances between populations
     popnames : names of populations
-    outgroup : population to use as outgroup for rooting (if None, use hzy (should give good results) 
+    outgroup : population to use as outgroup for rooting (if None, use hzy (should give good results)
                or do midpoint rooting (not implemented))
     fprefix : if set, save the temporary files with names built from fprefix
     keep_outgroup : do not drop the population used for rooting the tree
     hzy : Optimize root finding on observed heterozygosities vector hzy
 
     Returns:
     -----------
@@ -153,146 +160,160 @@
     fprefix_{ }.txt : if fprefix was set
 
     See Also:
     ------------
 
     popgen.reynolds to compute reynolds distances between populations
     popgen.heterozygosity to compute heterozygosities of populations
-    '''
+    """
     if outgroup is not None:
         try:
             assert outgroup in popnames
         except AssertionError:
-            print( "Outgroup not found in file",outgroup)
-            print( *popnames)
+            print("Outgroup not found in file", outgroup)
+            print(*popnames)
             sys.exit(1)
     if not fprefix:
-        buf,rey_file_name=tempfile.mkstemp(prefix='reynolds')
-        buf,fij_file_name=tempfile.mkstemp(prefix='fij',suffix='.txt')
-        buf,tree_file_name=tempfile.mkstemp(prefix='tree',suffix='.txt')
-        buf,treedump_file_name=tempfile.mkstemp(prefix='treedump',suffix='.tree')
+        buf, rey_file_name = tempfile.mkstemp(prefix="reynolds")
+        buf, fij_file_name = tempfile.mkstemp(prefix="fij", suffix=".txt")
+        buf, tree_file_name = tempfile.mkstemp(prefix="tree", suffix=".txt")
+        buf, treedump_file_name = tempfile.mkstemp(prefix="treedump", suffix=".tree")
     else:
-        rey_file_name=fprefix+'_reynolds.txt'
-        fij_file_name=fprefix+'_fij.txt'
-        tree_file_name=fprefix+'_tree.txt'
-        treedump_file_name=fprefix+'.tree'
+        rey_file_name = fprefix + "_reynolds.txt"
+        fij_file_name = fprefix + "_fij.txt"
+        tree_file_name = fprefix + "_tree.txt"
+        treedump_file_name = fprefix + ".tree"
     ## write reynolds to file
-    reynolds_out=open(rey_file_name,'w')
+    reynolds_out = open(rey_file_name, "w")
     for i in range(D.shape[0]):
-        tw=[popnames[i]]
+        tw = [popnames[i]]
         for j in range(D.shape[1]):
-            tw.append(str(D[i,j]))
-        print(' '.join(tw), file = reynolds_out)
+            tw.append(str(D[i, j]))
+        print(" ".join(tw), file=reynolds_out)
     reynolds_out.close()
     ## Build the tree
-    dist_mat=2*D
-    my_nj=nj.NJ(dist_mat,popnames)
+    dist_mat = 2 * D
+    my_nj = nj.NJ(dist_mat, popnames)
     my_nj.fit()
     if outgroup:
-        root_edge=[e for e in my_nj.edges if e.n1.label==outgroup or e.n2.label==outgroup][0]
-        tree=nj.Rooted_Tree()
+        root_edge = [e for e in my_nj.edges if e.n1.label == outgroup or e.n2.label == outgroup][0]
+        tree = nj.Rooted_Tree()
         if keep_outgroup:
-            tree.build_from_edges(my_nj.edges,root_edge)
+            tree.build_from_edges(my_nj.edges, root_edge)
             if hzy is not None:
                 ## we can optimize root placement
-                hzy_dict={}
-                for i,nom in enumerate(popnames):
-                    hzy_dict[nom]=hzy[i]
+                hzy_dict = {}
+                for i, nom in enumerate(popnames):
+                    hzy_dict[nom] = hzy[i]
                 tree.optim_root(hzy_dict)
         else:
-            print( "Rooting with %s and dropping it."%outgroup)
-            tree.build_from_edges(my_nj.edges,root_edge,outgroup=outgroup)
+            print("Rooting with %s and dropping it." % outgroup)
+            tree.build_from_edges(my_nj.edges, root_edge, outgroup=outgroup)
     else:
         ## No outgroup information
         if hzy is not None:
-            hzy_dict={}
-            for i,nom in enumerate(popnames):
-                hzy_dict[nom]=hzy[i]
+            hzy_dict = {}
+            for i, nom in enumerate(popnames):
+                hzy_dict[nom] = hzy[i]
             ## we can optimize using heterozygosities
-            resid=np.inf ## optim criterion
-            root_edge_best=None ## where we will place the root
+            resid = np.inf  ## optim criterion
+            root_edge_best = None  ## where we will place the root
             for candidate in my_nj.edges:
-                edges=[e for e in my_nj.edges]
-                tree=nj.Rooted_Tree()
-                tree.build_from_edges(edges,candidate)
-                tree_fit=tree.optim_root(hzy_dict)
+                edges = [e for e in my_nj.edges]
+                tree = nj.Rooted_Tree()
+                tree.build_from_edges(edges, candidate)
+                tree_fit = tree.optim_root(hzy_dict)
                 ##print 'Edge',candidate,' : ',tree_fit.fun
-                if tree_fit.x[1]>0 and tree_fit.fun<resid:
-                    resid=tree_fit.fun
-                    root_edge_best=candidate
-                    root_pos_best=tree_fit.x[1]
-            tree=nj.Rooted_Tree()
-            tree.build_from_edges(my_nj.edges,root_edge_best)
+                if tree_fit.x[1] > 0 and tree_fit.fun < resid:
+                    resid = tree_fit.fun
+                    root_edge_best = candidate
+                    root_pos_best = tree_fit.x[1]
+            tree = nj.Rooted_Tree()
+            tree.build_from_edges(my_nj.edges, root_edge_best)
             tree.shift_root(root_pos_best)
         else:
             ## no hzy information, should revert to midpoint but this is
             ## usually not a good idea ...
             raise NotImplementedError
     ## Now we have a tree, get Kinship
-    with open(tree_file_name,'w') as f:
-        print( tree.newick(), file = f)
+    with open(tree_file_name, "w") as f:
+        print(tree.newick(), file=f)
     if dump_tree:
-        with open(treedump_file_name,'w') as f:
-            pickle.dump(tree,f)
-    kin,poplabels=tree.kinship()
-    with open(fij_file_name,'w') as f:
-        for i,nom in enumerate(poplabels):
-            print( nom,' '.join([str(x) for x in kin[i,]]), file = f)
+        with open(treedump_file_name, "w") as f:
+            pickle.dump(tree, f)
+    kin, poplabels = tree.kinship()
+    with open(fij_file_name, "w") as f:
+        for i, nom in enumerate(poplabels):
+            print(
+                nom,
+                " ".join(
+                    [
+                        str(x)
+                        for x in kin[
+                            i,
+                        ]
+                    ]
+                ),
+                file=f,
+            )
     ### we have to be careful because the pop order can change within Fij
     if outgroup and not keep_outgroup:
-        pname_temp=[x for x in popnames if x!=outgroup]
+        pname_temp = [x for x in popnames if x != outgroup]
     else:
-        pname_temp=popnames[:]
-    ordre=[poplabels.index(x) for x in pname_temp]
-    FF=kin[ordre,:][:,ordre]
+        pname_temp = popnames[:]
+    ordre = [poplabels.index(x) for x in pname_temp]
+    FF = kin[ordre, :][:, ordre]
     ## clean up temp files if needed
     if not fprefix:
         os.remove(rey_file_name)
         os.remove(fij_file_name)
         os.remove(tree_file_name)
         if dump_tree:
             os.remove(treedump_file_name)
     return FF
 
-class FLK_result():
+
+class FLK_result:
     def __init__(self):
-        self.p0=np.nan
-        self.val=0
-        self.pval=1
-        
-class FLK_test():
-    '''
+        self.p0 = np.nan
+        self.val = 0
+        self.pval = 1
+
+
+class FLK_test:
+    """
     FLK test implementation
-    '''
-    def __init__(self,kinship,diallelic=True):
-        '''
+    """
+
+    def __init__(self, kinship, diallelic=True):
+        """
         Creates an FLK test
 
         Parameters:
         ---------------
 
         kinship : population kinship matrix
         diallelic : if True, the locus is diallelic (e.g. a SNP) o.w. multiallelic
-        
-        '''
-        self.F=kinship
-        assert self.F.shape[0]==self.F.shape[1]
-        self.dimension=self.F.shape[0]
-        self.diallelic=diallelic
-        self.invF=np.linalg.inv(self.F)
+
+        """
+        self.F = kinship
+        assert self.F.shape[0] == self.F.shape[1]
+        self.dimension = self.F.shape[0]
+        self.diallelic = diallelic
+        self.invF = np.linalg.inv(self.F)
         self.un = np.ones(self.dimension)
-        self.w = np.dot(self.invF,self.un.T)/np.dot(self.un,np.dot(self.invF,self.un.T))
-        self.D,self.Q = np.linalg.eigh(self.F)
+        self.w = np.dot(self.invF, self.un.T) / np.dot(self.un, np.dot(self.invF, self.un.T))
+        self.D, self.Q = np.linalg.eigh(self.F)
         if diallelic:
-            self.eigen_contrib=self.eigen_contrib_diallelic
+            self.eigen_contrib = self.eigen_contrib_diallelic
         else:
-            self.eigen_contrib=self.eigen_contrib_multi
-        
-    def eigen_contrib_diallelic(self,p,diallelic=True):
-        '''
+            self.eigen_contrib = self.eigen_contrib_multi
+
+    def eigen_contrib_diallelic(self, p, diallelic=True):
+        """
         Computes orthogonalized contributions of each component to the FLK
         statistic, using the spectral decomposition of the variance
         covariance matrix V(p) V=cste*F=cste*Q*D*Q.T where Q is the matrix
         of eigen vectors and D the corresponding diagonal matrix with
         eigen values on the diagonal.
 
         Parameters:
@@ -303,76 +324,75 @@
         Return Value:
         -----------------
         a tuple of :
             - p0hat : estimated allele frequency in the ancestral population
             - Z : contributions of each PC to the FLK statistic
             - cste : multiplying constant to the test
         the value of FLK is = C*sum(L^2)
-        '''
-        p0hat = np.dot(self.w.T,p)
-        cste = ((1 - (1/(np.dot(self.un,np.dot(self.invF,self.un.T)))))/(p0hat*(1-p0hat)))
-        Z=np.dot((p-(p0hat*self.un)),self.Q)
-        Z=np.dot(Z,np.diag(np.sqrt(1/self.D)))
+        """
+        p0hat = np.dot(self.w.T, p)
+        cste = (1 - (1 / (np.dot(self.un, np.dot(self.invF, self.un.T))))) / (p0hat * (1 - p0hat))
+        Z = np.dot((p - (p0hat * self.un)), self.Q)
+        Z = np.dot(Z, np.diag(np.sqrt(1 / self.D)))
         Z *= np.sqrt(cste)
         # tmp=np.dot(p-(p0hat*self.un),self.invF*cste)
         # tmp=np.dot(tmp,(p-(p0hat*self.un).T))
         # print tmp,np.sum([z**2 for z in Z])
         # R = np.dot(self.Q.T,(p-(p0hat*self.un).T))
         # R = np.dot(np.diag(np.sqrt(1/self.D)),R)
         # R *= np.sqrt(cste)
         # print R.shape
         # Z=[R[i] for i in range(R.shape[0])]
-        return p0hat,Z,cste
+        return p0hat, Z, cste
 
-    def eigen_contrib_multi(self,p):
-        '''
+    def eigen_contrib_multi(self, p):
+        """
         Multiallelic version of eigen_contrib_diallelic
-        
+
         Parameters:
         ---------------
-        
+
         p : vector of population allele frequencies at a locus
-        
+
         Return Value:
         -----------------
         a tuple of :
         - p0hat : estimated allele frequency in the ancestral population
         - Z : contributions of each PC to the FLK statistic
         - cste : multiplying constant to the test
         the value of FLK is = C*sum(L^2)
-        
+
         See Also:
         ------------
-        
-        eigen_contrib_diallelic 
-        '''
-        p0hat = np.dot(self.w.T,p)
-        Z=np.dot((p-(p0hat*self.un)),self.Q)
-        Z=np.dot(Z,np.diag(np.sqrt(1/self.D)))
-        return p0hat,Z,1.0
-    
-    def eval_flk(self,p):
-        '''
+
+        eigen_contrib_diallelic
+        """
+        p0hat = np.dot(self.w.T, p)
+        Z = np.dot((p - (p0hat * self.un)), self.Q)
+        Z = np.dot(Z, np.diag(np.sqrt(1 / self.D)))
+        return p0hat, Z, 1.0
+
+    def eval_flk(self, p):
+        """
         Computes the FLK statistic
 
         Parameters:
         ---------------
 
         p : vector of population allele frequencies
 
         Return Value:
         -----------------
         a list of :
            -- p0
            -- FLK value
            -- corresponding p-value
            -- each contribution of the PC in turn
-        '''
-        assert p.shape[0]==self.dimension
-        p0,Z,C=self.eigen_contrib(p)
-        val=sum([x**2 for x in Z])
-        if self.diallelic and p0>0.05 and p0<0.95:
-            pval=chi2.sf(val,self.dimension-1)
+        """
+        assert p.shape[0] == self.dimension
+        p0, Z, C = self.eigen_contrib(p)
+        val = sum([x ** 2 for x in Z])
+        if self.diallelic and p0 > 0.05 and p0 < 0.95:
+            pval = chi2.sf(val, self.dimension - 1)
         else:
-            pval=np.nan
-        return [p0,val,pval]+Z.tolist()
-      
+            pval = np.nan
+        return [p0, val, pval] + Z.tolist()
```

### Comparing `hapflk-2.0.dev2/hapflk/utils.py` & `hapflk-2.1/hapflk/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import datetime as dt
 
+
 class Stepper(object):
-    def __init__(self, prefix=''):
+    def __init__(self, prefix=""):
         """
 
         :type prefix: basestring
         """
         self.start = dt.datetime.now()
         self.ncalls = 0
         self.prefix = prefix
-        self.write(msg="Start @ "+dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
+        self.write(msg="Start @ " + dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
 
     @staticmethod
     def formatTD(td):
         hours = td.seconds // 3600
         minutes = (td.seconds % 3600) // 60
         seconds = td.seconds % 60
-        return '%02d:%02d:%02d' % (hours, minutes, seconds)
+        return "%02d:%02d:%02d" % (hours, minutes, seconds)
 
-    def new(self, msg='Step'):
+    def new(self, msg="Step"):
         self.ncalls += 1
-        print(self.prefix, self.ncalls, ". [", self.formatTD(dt.datetime.now()-self.start), "] ", msg)
-        return dt.datetime.now()-self.start
+        print(
+            self.prefix,
+            self.ncalls,
+            ". [",
+            self.formatTD(dt.datetime.now() - self.start),
+            "] ",
+            msg,
+        )
+        return dt.datetime.now() - self.start
 
     def write(self, msg):
-        print ((10+len(self.prefix))*' '+msg)
+        print((10 + len(self.prefix)) * " " + msg)
 
     def end(self):
-        return self.new(msg="The End @ "+dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
-
+        return self.new(msg="The End @ " + dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
```

