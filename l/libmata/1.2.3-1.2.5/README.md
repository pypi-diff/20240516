# Comparing `tmp/libmata-1.2.3.tar.gz` & `tmp/libmata-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmata-1.2.3.tar", last modified: Thu Mar 21 11:40:43 2024, max compression
+gzip compressed data, was "libmata-1.2.5.tar", last modified: Thu May 16 19:11:29 2024, max compression
```

## Comparing `libmata-1.2.3.tar` & `libmata-1.2.5.tar`

### file list

```diff
@@ -1,327 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.256002 libmata-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-03-21 11:40:43.256002 libmata-1.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.236002 libmata-1.2.3/libmata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   558446 2024-03-21 11:38:40.103370 libmata-1.2.3/libmata/alphabets.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/alphabets.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/alphabets.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.236002 libmata-1.2.3/libmata/nfa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/nfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1797221 2024-03-21 11:38:40.891373 libmata-1.2.3/libmata/nfa/nfa.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/nfa/nfa.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    45100 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/nfa/nfa.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   460699 2024-03-21 11:38:41.439376 libmata-1.2.3/libmata/nfa/strings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/nfa/strings.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/nfa/strings.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   302758 2024-03-21 11:38:41.863378 libmata-1.2.3/libmata/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/parser.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/parser.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   734276 2024-03-21 11:38:42.355381 libmata-1.2.3/libmata/plotting.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/plotting.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   487576 2024-03-21 11:38:42.659382 libmata-1.2.3/libmata/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-03-21 11:38:04.503167 libmata-1.2.3/libmata/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.240002 libmata-1.2.3/mata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.236002 libmata-1.2.3/mata/3rdparty/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.240002 libmata-1.2.3/mata/3rdparty/cudd/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   104287 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/README
--rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/RELEASE.NOTES
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.240002 libmata-1.2.3/mata/3rdparty/cudd/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (127)   118858 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cplusplus/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cplusplus/test_obj.test.in
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cplusplus/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23907 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cplusplus/testobj.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.244002 libmata-1.2.3/mata/3rdparty/cudd/cudd/
--rw-r--r--   0 runner    (1001) docker     (127)   105019 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (127)    15462 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (127)    15444 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-03-21 11:38:04.479167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (127)    19718 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (127)    65063 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (127)    33952 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (127)    23919 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (127)    24032 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (127)    44880 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (127)    59815 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (127)    40003 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (127)    24861 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (127)    46041 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (127)    57084 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (127)    26667 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (127)    57030 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (127)    15705 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (127)    47195 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (127)    34453 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (127)    35196 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (127)    54937 2024-03-21 11:38:04.483167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (127)    16895 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (127)    17072 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (127)    54629 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (127)    45218 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (127)    40719 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (127)    53495 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (127)    46846 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (127)    92286 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (127)   102122 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (127)    24532 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (127)    36242 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (127)    35725 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (127)    25595 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (127)    40115 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (127)    43419 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (127)    30406 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/r7x8.1.mat
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/test_cudd.test.in
--rw-r--r--   0 runner    (1001) docker     (127)    31625 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd/testextra.c
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/cudd_config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.244002 libmata-1.2.3/mata/3rdparty/cudd/dddmp/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/README.dddmp
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/README.testdddmp
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-03-21 11:38:04.487167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (127)    45057 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (127)    30128 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (127)    25140 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (127)    28404 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (127)    33164 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (127)    47973 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (127)    45283 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpUtil.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.244002 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/credit.html
--rw-r--r--   0 runner    (1001) docker     (127)    64661 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
--rw-r--r--   0 runner    (1001) docker     (127)    64648 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
--rw-r--r--   0 runner    (1001) docker     (127)    23413 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
--rw-r--r--   0 runner    (1001) docker     (127)   127869 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
--rw-r--r--   0 runner    (1001) docker     (127)    32197 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
--rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
--rw-r--r--   0 runner    (1001) docker     (127)    27862 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/packages.html
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.248002 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/0.add
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/0.bdd
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/1.add
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/1.bdd
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/2.bdd
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/3.bdd
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.cnf
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.max1
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-03-21 11:38:04.491167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.max2
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/5.bdd
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/composeids.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/one.bdd
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/varnames.ord
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/zero.bdd
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
--rw-r--r--   0 runner    (1001) docker     (127)    66662 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/dddmp/testdddmp.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.248002 libmata-1.2.3/mata/3rdparty/cudd/doc/
--rw-r--r--   0 runner    (1001) docker     (127)    97463 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/doc/cudd.tex.in
--rw-r--r--   0 runner    (1001) docker     (127)    17981 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/doc/phase.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.248002 libmata-1.2.3/mata/3rdparty/cudd/epd/
--rw-r--r--   0 runner    (1001) docker     (127)    23011 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/epd/epd.c
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/epd/epd.h
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/epd/epdInt.h
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/groups.dox
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.232002 libmata-1.2.3/mata/3rdparty/cudd/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.232002 libmata-1.2.3/mata/3rdparty/cudd/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.248002 libmata-1.2.3/mata/3rdparty/cudd/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (127)    47917 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (127)    29098 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.248002 libmata-1.2.3/mata/3rdparty/cudd/mtr/
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/mtr/mtr.h
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/mtr/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/mtr/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/mtr/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/mtr/test.groups
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/mtr/test_mtr.test.in
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/mtr/testmtr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.248002 libmata-1.2.3/mata/3rdparty/cudd/st/
--rw-r--r--   0 runner    (1001) docker     (127)    30078 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/st/st.c
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/st/st.h
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/st/test_st.test.in
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/st/testst.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.248002 libmata-1.2.3/mata/3rdparty/cudd/util/
--rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/prtime.c
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/strsav.c
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/texpand.c
--rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/cudd/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/3rdparty/re2/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/re2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/re2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/re2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/re2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/3rdparty/re2/re2/
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/re2/re2/bitmap256.h
--rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-03-21 11:38:04.495167 libmata-1.2.3/mata/3rdparty/re2/re2/compile.cc
--rw-r--r--   0 runner    (1001) docker     (127)    76112 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/parse.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/perl_groups.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/pod_array.h
--rw-r--r--   0 runner    (1001) docker     (127)    31582 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/prog.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/prog.h
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/re2.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/re2.h
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/regexp.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21633 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/regexp.h
--rw-r--r--   0 runner    (1001) docker     (127)    19503 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/simplify.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/sparse_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/sparse_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/tostring.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/unicode_casefold.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/unicode_casefold.h
--rw-r--r--   0 runner    (1001) docker     (127)   124977 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/unicode_groups.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/unicode_groups.h
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/re2/walker-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/3rdparty/re2/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/util/rune.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/util/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/util/strutil.h
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/util/utf.h
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/re2/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/3rdparty/simlib/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.236002 libmata-1.2.3/mata/3rdparty/simlib/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.236002 libmata-1.2.3/mata/3rdparty/simlib/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
--rw-r--r--   0 runner    (1001) docker     (127)    19405 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/3rdparty/simlib/src/
--rw-r--r--   0 runner    (1001) docker     (127)    18405 2024-03-21 11:38:04.499167 libmata-1.2.3/mata/3rdparty/simlib/src/explicit_lts_sim.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-03-21 11:40:43.156002 libmata-1.2.3/mata/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101164 2024-03-21 11:40:43.156002 libmata-1.2.3/mata/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-21 11:40:43.152001 libmata-1.2.3/mata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-03-21 11:40:43.152001 libmata-1.2.3/mata/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-03-21 11:40:43.152001 libmata-1.2.3/mata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-21 11:40:43.152001 libmata-1.2.3/mata/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-03-21 11:38:04.503167 libmata-1.2.3/mata/cmake/GetGitRevisionDescription.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-21 11:38:04.503167 libmata-1.2.3/mata/cmake/GetGitRevisionDescription.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-21 11:40:43.156002 libmata-1.2.3/mata/cmake_uninstall.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.236002 libmata-1.2.3/mata/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/include/mata/
--rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/alphabet.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/include/mata/nfa/
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/nfa/algorithms.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/nfa/builder.hh
--rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/nfa/delta.hh
--rw-r--r--   0 runner    (1001) docker     (127)    27547 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/nfa/nfa.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/nfa/plumbing.hh
--rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/nfa/strings.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/nfa/types.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.252002 libmata-1.2.3/mata/include/mata/parser/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/parser/inter-aut.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/parser/mintermization.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/parser/parser.hh
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/parser/re2parser.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.256002 libmata-1.2.3/mata/include/mata/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/utils/closed-set.hh
--rw-r--r--   0 runner    (1001) docker     (127)    16745 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/utils/ord-vector.hh
--rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/utils/sparse-set.hh
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/utils/synchronized-iterator.hh
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/include/mata/utils/utils.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.256002 libmata-1.2.3/mata/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/config.cc.in
--rw-r--r--   0 runner    (1001) docker     (127)    26710 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/inter-aut.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13984 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.256002 libmata-1.2.3/mata/src/nfa/
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/builder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/complement.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (127)    27623 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/delta.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/inclusion.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/intersection.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19615 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31014 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/operations.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/nfa/universal.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31065 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/re2parser.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:40:43.256002 libmata-1.2.3/mata/src/strings/
--rw-r--r--   0 runner    (1001) docker     (127)    16737 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-03-21 11:38:04.507167 libmata-1.2.3/mata/src/strings/nfa-strings.cc
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-21 11:38:04.503167 libmata-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-03-21 11:38:04.503167 libmata-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.936964 libmata-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-16 19:11:29.936964 libmata-1.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.916964 libmata-1.2.5/libmata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   559290 2024-05-16 19:09:26.297257 libmata-1.2.5/libmata/alphabets.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/alphabets.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/alphabets.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.920964 libmata-1.2.5/libmata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/nfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1798080 2024-05-16 19:09:27.065256 libmata-1.2.5/libmata/nfa/nfa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/nfa/nfa.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    45100 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/nfa/nfa.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   461546 2024-05-16 19:09:27.609255 libmata-1.2.5/libmata/nfa/strings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/nfa/strings.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/nfa/strings.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   303605 2024-05-16 19:09:28.045255 libmata-1.2.5/libmata/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/parser.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   735141 2024-05-16 19:09:28.533254 libmata-1.2.5/libmata/plotting.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/plotting.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   488395 2024-05-16 19:09:28.845253 libmata-1.2.5/libmata/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-16 19:08:51.061304 libmata-1.2.5/libmata/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.920964 libmata-1.2.5/mata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.916964 libmata-1.2.5/mata/3rdparty/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.920964 libmata-1.2.5/mata/3rdparty/cudd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   104287 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/README
+-rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/RELEASE.NOTES
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.920964 libmata-1.2.5/mata/3rdparty/cudd/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (127)   118858 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/cplusplus/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/cplusplus/test_obj.test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/cplusplus/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23907 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/cplusplus/testobj.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.924964 libmata-1.2.5/mata/3rdparty/cudd/cudd/
+-rw-r--r--   0 runner    (1001) docker     (127)   105019 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15462 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-05-16 19:08:51.037304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15444 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19718 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (127)    65063 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33952 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (127)    23919 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24032 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (127)    44880 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (127)    59815 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    40003 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24861 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (127)    46041 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (127)    57084 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26667 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (127)    57030 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15705 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    47195 2024-05-16 19:08:51.041304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (127)    34453 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (127)    35196 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (127)    54937 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16895 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17072 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (127)    54629 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45218 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    40719 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (127)    53495 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (127)    46846 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (127)    92286 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (127)   102122 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24532 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36242 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (127)    35725 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25595 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-16 19:08:51.045304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (127)    40115 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43419 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30406 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/r7x8.1.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/test_cudd.test.in
+-rw-r--r--   0 runner    (1001) docker     (127)    31625 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/cudd_config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.924964 libmata-1.2.5/mata/3rdparty/cudd/dddmp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/README.dddmp
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/README.testdddmp
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45057 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30128 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25140 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (127)    28404 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33164 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (127)    47973 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45283 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpUtil.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.928964 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/credit.html
+-rw-r--r--   0 runner    (1001) docker     (127)    64661 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
+-rw-r--r--   0 runner    (1001) docker     (127)    64648 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
+-rw-r--r--   0 runner    (1001) docker     (127)    23413 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-16 19:08:51.049304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
+-rw-r--r--   0 runner    (1001) docker     (127)   127869 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32197 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)    27862 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/packages.html
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.928964 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/0.add
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/0.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/1.add
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/1.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/2.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/3.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.cnf
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.max1
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.max2
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/5.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/composeids.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/one.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/varnames.ord
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/zero.bdd
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
+-rw-r--r--   0 runner    (1001) docker     (127)    66662 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/dddmp/testdddmp.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.928964 libmata-1.2.5/mata/3rdparty/cudd/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    97463 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/doc/cudd.tex.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17981 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/doc/phase.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.928964 libmata-1.2.5/mata/3rdparty/cudd/epd/
+-rw-r--r--   0 runner    (1001) docker     (127)    23011 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/epd/epd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/epd/epd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/epd/epdInt.h
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/groups.dox
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.916964 libmata-1.2.5/mata/3rdparty/cudd/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.916964 libmata-1.2.5/mata/3rdparty/cudd/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.928964 libmata-1.2.5/mata/3rdparty/cudd/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (127)    47917 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29098 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.928964 libmata-1.2.5/mata/3rdparty/cudd/mtr/
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/mtr/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/mtr/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/mtr/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/mtr/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/mtr/test.groups
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/mtr/test_mtr.test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-16 19:08:51.053304 libmata-1.2.5/mata/3rdparty/cudd/mtr/testmtr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.928964 libmata-1.2.5/mata/3rdparty/cudd/st/
+-rw-r--r--   0 runner    (1001) docker     (127)    30078 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/st/st.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/st/st.h
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/st/test_st.test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/st/testst.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/3rdparty/cudd/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/cudd/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/3rdparty/re2/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/3rdparty/re2/re2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/bitmap256.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/compile.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    76112 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/parse.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/perl_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/pod_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31582 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/prog.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/prog.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/re2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/re2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/regexp.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21633 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/regexp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19503 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/simplify.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/sparse_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/sparse_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/tostring.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/unicode_casefold.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/unicode_casefold.h
+-rw-r--r--   0 runner    (1001) docker     (127)   124977 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/unicode_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/unicode_groups.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/re2/walker-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/3rdparty/re2/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/util/rune.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-16 19:08:51.057304 libmata-1.2.5/mata/3rdparty/re2/util/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/re2/util/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/re2/util/utf.h
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/re2/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/3rdparty/simlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.916964 libmata-1.2.5/mata/3rdparty/simlib/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.916964 libmata-1.2.5/mata/3rdparty/simlib/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    19405 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/3rdparty/simlib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    18405 2024-05-16 19:08:51.061304 libmata-1.2.5/mata/3rdparty/simlib/src/explicit_lts_sim.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-16 19:11:29.820964 libmata-1.2.5/mata/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101164 2024-05-16 19:11:29.820964 libmata-1.2.5/mata/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-16 19:11:29.820964 libmata-1.2.5/mata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-16 19:11:29.820964 libmata-1.2.5/mata/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-16 19:11:29.820964 libmata-1.2.5/mata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 19:11:29.820964 libmata-1.2.5/mata/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/cmake/GetGitRevisionDescription.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/cmake/GetGitRevisionDescription.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-16 19:11:29.820964 libmata-1.2.5/mata/cmake_uninstall.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.916964 libmata-1.2.5/mata/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.932964 libmata-1.2.5/mata/include/mata/
+-rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/alphabet.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.936964 libmata-1.2.5/mata/include/mata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/nfa/algorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/nfa/builder.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/nfa/delta.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    27579 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/nfa/nfa.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/nfa/plumbing.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/nfa/strings.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/nfa/types.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.936964 libmata-1.2.5/mata/include/mata/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/parser/inter-aut.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/parser/mintermization.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/parser/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/parser/re2parser.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.936964 libmata-1.2.5/mata/include/mata/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/utils/closed-set.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    16745 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/utils/ord-vector.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/utils/sparse-set.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/utils/synchronized-iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/include/mata/utils/utils.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.936964 libmata-1.2.5/mata/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/src/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/src/config.cc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26710 2024-05-16 19:08:51.065304 libmata-1.2.5/mata/src/inter-aut.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13984 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.936964 libmata-1.2.5/mata/src/nfa/
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/complement.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    27623 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/delta.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/inclusion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19615 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31038 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/operations.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/nfa/universal.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31065 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/re2parser.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:11:29.936964 libmata-1.2.5/mata/src/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)    16737 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-16 19:08:51.069304 libmata-1.2.5/mata/src/strings/nfa-strings.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-16 19:08:51.061304 libmata-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 19:08:51.061304 libmata-1.2.5/setup.py
```

### Comparing `libmata-1.2.3/PKG-INFO` & `libmata-1.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmata
-Version: 1.2.3
+Version: 1.2.5
 Summary: The automata library
 Home-page: https://github.com/verifit/mata
 Author: Lukáš Holík <holik@fit.vutbr.cz>, Ondřej Lengál <lengal@fit.vutbr.cz>, Martin Hruška <ihruskam@fit.vutbr.cz>, Tomáš Fiedor <ifiedortom@fit.vutbr.cz>, David Chocholatý <chocholaty.david@protonmail.com>, Juraj Síč <sicjuraj@fit.vutbr.cz>, Tomáš Vojnar <vojnar@fit.vutbr.cz>
 Author-email: lengal@fit.vutbr.cz
 License: UNKNOWN
 Keywords: automata,finite automata,alternating automata
 Platform: UNKNOWN
@@ -229,34 +229,15 @@
 
 # Publications
 - Chocholatý, D., Fiedor, T., Havlena, V., Holík, L., Hruška, M., Lengál, O., & Síč, J. (2023). [Mata, a Fast and Simple Finite Automata Library](https://doi.org/10.48550/arXiv.2310.10136). arXiv preprint arXiv:2310.10136.
     - Chocholatý, D., Fiedor, T., Havlena, V., Holík, L., Hruška, M., Lengál, O., Síč, J.: [A replication package for reproducing the results of paper “Mata: A fast and simple finite automata library”](https://doi.org/10.5281/zenodo.10044515) (Oct 2023).
 
 # Contributing
 
-If you'd like to contribute to the libmata, 
-please [fork the repository](https://github.com/VeriFIT/mata/fork), create a new 
-feature branch, and finally [create a new pull request](https://github.com/VeriFIT/mata/compare).
-
-In case you run into some unexpected behaviour, error or anything suspicious
-either contact us directly through mail or 
-[create a new issue](https://github.com/VeriFIT/mata/issues/new/choose).
-When creating a new issue, please, try to include everything necessary for us to know
-(such as the version, operation system, etc.) so we can sucessfully replicate the issue.
-
-## Note to main contributors
-
-By default, each merge automatically increases the `minor` version of the library
-(i.e., `0.0.0 -> 0.1.0` ). This can be overruled using either tag `#patch` (increasing
-patch version, i.e., `0.0.0 -> 0.0.1`) or `#major` (increasing major version, i.e.,
-`0.0.0 -> 1.0.0`). This tag is specified in the merge message.
-
-Generally, it is recommended to use `#major` for changes that introduces backward-incompatible
-changes for people that used previous versions, and `#patch` for minor changes, such as bug-fixes,
-performance fixes or refactoring.
+Please refer to our [contributing guidelines](CONTRIBUTING.md).
 
 # Links
 
   - Project (origin) repository: <https://github.com/verifit/mata>
   - Issue tracker: <https://github.com/verifit/mata/issues>
     - In case of some sensitive bugs (like security vulnerabilities),
       please contact us directly, instead of using issue tracker.
```

### Comparing `libmata-1.2.3/libmata/alphabets.cpp` & `libmata-1.2.5/libmata/alphabets.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
@@ -63,18 +63,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -158,14 +158,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -219,14 +221,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -280,60 +284,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -416,14 +443,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2135,30 +2165,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -7767,20 +7797,20 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 104, __pyx_L1_error)
+  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 104, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(3, 215, __pyx_L1_error)
-  __pyx_ptype_7libmata_3nfa_3nfa_Transition = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.nfa.nfa", "Transition", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Transition), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_3nfa_3nfa_Transition),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_3nfa_3nfa_Transition) __PYX_ERR(3, 223, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(3, 215, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Transition = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.nfa.nfa", "Transition", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Transition), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_3nfa_3nfa_Transition),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_3nfa_3nfa_Transition) __PYX_ERR(3, 223, __pyx_L1_error)
   __pyx_vtabptr_7libmata_3nfa_3nfa_Transition = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Transition*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Transition); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Transition)) __PYX_ERR(3, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -10443,18 +10473,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -10500,23 +10530,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `libmata-1.2.3/libmata/alphabets.pxd` & `libmata-1.2.5/libmata/alphabets.pxd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/alphabets.pyx` & `libmata-1.2.5/libmata/alphabets.pyx`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/nfa/nfa.cpp` & `libmata-1.2.5/libmata/nfa/nfa.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
@@ -63,18 +63,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -158,14 +158,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -219,14 +221,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -280,60 +284,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -416,14 +443,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2351,30 +2381,30 @@
 
 /* MergeVTables.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_MergeVtables(PyTypeObject *type);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -30494,25 +30524,27 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_7libmata_3nfa_3nfa___pyx_scope_struct__iterate *__pyx_freelist_7libmata_3nfa_3nfa___pyx_scope_struct__iterate[8];
 static int __pyx_freecount_7libmata_3nfa_3nfa___pyx_scope_struct__iterate = 0;
+#endif
 
 static PyObject *__pyx_tp_new_7libmata_3nfa_3nfa___pyx_scope_struct__iterate(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7libmata_3nfa_3nfa___pyx_scope_struct__iterate *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_7libmata_3nfa_3nfa___pyx_scope_struct__iterate > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_7libmata_3nfa_3nfa___pyx_scope_struct__iterate)))) {
     o = (PyObject*)__pyx_freelist_7libmata_3nfa_3nfa___pyx_scope_struct__iterate[--__pyx_freecount_7libmata_3nfa_3nfa___pyx_scope_struct__iterate];
     memset(o, 0, sizeof(struct __pyx_obj_7libmata_3nfa_3nfa___pyx_scope_struct__iterate));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -30539,15 +30571,15 @@
   #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->__pyx_v_iterator);
   __Pyx_call_destructor(p->__pyx_v_lhs);
   __Pyx_call_destructor(p->__pyx_v_transitions);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_trans);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_7libmata_3nfa_3nfa___pyx_scope_struct__iterate < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_7libmata_3nfa_3nfa___pyx_scope_struct__iterate)))) {
     __pyx_freelist_7libmata_3nfa_3nfa___pyx_scope_struct__iterate[__pyx_freecount_7libmata_3nfa_3nfa___pyx_scope_struct__iterate++] = ((struct __pyx_obj_7libmata_3nfa_3nfa___pyx_scope_struct__iterate *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -32280,19 +32312,19 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 104, __pyx_L1_error)
+  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 104, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
+  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
   __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -37007,18 +37039,18 @@
     __Pyx_DECREF_TypeName(base_name);
     free(base_vtables);
     return -1;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -37064,23 +37096,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `libmata-1.2.3/libmata/nfa/nfa.pxd` & `libmata-1.2.5/libmata/nfa/nfa.pxd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/nfa/nfa.pyx` & `libmata-1.2.5/libmata/nfa/nfa.pyx`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/nfa/strings.cpp` & `libmata-1.2.5/libmata/nfa/strings.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
@@ -64,18 +64,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -159,14 +159,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -220,14 +222,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -281,60 +285,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -417,14 +444,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2070,30 +2100,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyTypeObject *type);
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
@@ -6052,25 +6082,25 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 104, __pyx_L1_error)
+  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 104, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
+  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
   __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(4, 215, __pyx_L1_error)
-  __pyx_ptype_7libmata_3nfa_3nfa_Transition = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.nfa.nfa", "Transition", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Transition), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_3nfa_3nfa_Transition),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_3nfa_3nfa_Transition) __PYX_ERR(4, 223, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(4, 215, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Transition = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.nfa.nfa", "Transition", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Transition), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_3nfa_3nfa_Transition),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_3nfa_3nfa_Transition) __PYX_ERR(4, 223, __pyx_L1_error)
   __pyx_vtabptr_7libmata_3nfa_3nfa_Transition = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Transition*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Transition); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Transition)) __PYX_ERR(4, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -8456,18 +8486,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -8513,23 +8543,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `libmata-1.2.3/libmata/nfa/strings.pxd` & `libmata-1.2.5/libmata/nfa/strings.pxd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/nfa/strings.pyx` & `libmata-1.2.5/libmata/nfa/strings.pyx`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/parser.cpp` & `libmata-1.2.5/libmata/parser.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
@@ -68,18 +68,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -163,14 +163,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -224,14 +226,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -285,60 +289,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -421,14 +448,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1895,30 +1925,30 @@
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyTypeObject *type);
 
 /* IncludeStructmemberH.proto */
 #include <structmember.h>
@@ -3758,25 +3788,25 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 104, __pyx_L1_error)
+  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 104, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
+  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
   __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(4, 215, __pyx_L1_error)
-  __pyx_ptype_7libmata_3nfa_3nfa_Transition = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.nfa.nfa", "Transition", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Transition), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_3nfa_3nfa_Transition),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_3nfa_3nfa_Transition) __PYX_ERR(4, 223, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(4, 215, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Transition = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.nfa.nfa", "Transition", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Transition), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_3nfa_3nfa_Transition),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_3nfa_3nfa_Transition) __PYX_ERR(4, 223, __pyx_L1_error)
   __pyx_vtabptr_7libmata_3nfa_3nfa_Transition = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Transition*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Transition); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Transition)) __PYX_ERR(4, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -4903,18 +4933,18 @@
         ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
     __Pyx_DECREF_TypeName(type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -4960,23 +4990,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `libmata-1.2.3/libmata/parser.pxd` & `libmata-1.2.5/libmata/parser.pxd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/parser.pyx` & `libmata-1.2.5/libmata/parser.pyx`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/plotting.cpp` & `libmata-1.2.5/libmata/plotting.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
@@ -63,18 +63,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -158,14 +158,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -219,14 +221,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -280,60 +284,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -416,14 +443,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2287,30 +2317,30 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyTypeObject *type);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -9633,24 +9663,26 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_7libmata_8plotting___pyx_scope_struct__genexpr *__pyx_freelist_7libmata_8plotting___pyx_scope_struct__genexpr[8];
 static int __pyx_freecount_7libmata_8plotting___pyx_scope_struct__genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_7libmata_8plotting___pyx_scope_struct__genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_7libmata_8plotting___pyx_scope_struct__genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_7libmata_8plotting___pyx_scope_struct__genexpr)))) {
     o = (PyObject*)__pyx_freelist_7libmata_8plotting___pyx_scope_struct__genexpr[--__pyx_freecount_7libmata_8plotting___pyx_scope_struct__genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_7libmata_8plotting___pyx_scope_struct__genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -9670,15 +9702,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_t);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_7libmata_8plotting___pyx_scope_struct__genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_7libmata_8plotting___pyx_scope_struct__genexpr)))) {
     __pyx_freelist_7libmata_8plotting___pyx_scope_struct__genexpr[__pyx_freecount_7libmata_8plotting___pyx_scope_struct__genexpr++] = ((struct __pyx_obj_7libmata_8plotting___pyx_scope_struct__genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -10321,25 +10353,25 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(1, 104, __pyx_L1_error)
+  __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(1, 104, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(2, 35, __pyx_L1_error)
+  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(2, 35, __pyx_L1_error)
   __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(2, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(3, 215, __pyx_L1_error)
-  __pyx_ptype_7libmata_3nfa_3nfa_Transition = __Pyx_ImportType_3_0_9(__pyx_t_1, "libmata.nfa.nfa", "Transition", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Transition), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7libmata_3nfa_3nfa_Transition),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7libmata_3nfa_3nfa_Transition) __PYX_ERR(3, 223, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(3, 215, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Transition = __Pyx_ImportType_3_0_10(__pyx_t_1, "libmata.nfa.nfa", "Transition", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Transition), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7libmata_3nfa_3nfa_Transition),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7libmata_3nfa_3nfa_Transition) __PYX_ERR(3, 223, __pyx_L1_error)
   __pyx_vtabptr_7libmata_3nfa_3nfa_Transition = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Transition*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Transition); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Transition)) __PYX_ERR(3, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -13665,18 +13697,18 @@
         }
     }
     return descr;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -13722,23 +13754,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `libmata-1.2.3/libmata/plotting.pyx` & `libmata-1.2.5/libmata/plotting.pyx`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/utils.cpp` & `libmata-1.2.5/libmata/utils.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/utils/ord-vector.hh",
@@ -59,18 +59,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -154,14 +154,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -215,14 +217,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -276,60 +280,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -412,14 +439,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
```

### Comparing `libmata-1.2.3/libmata/utils.pxd` & `libmata-1.2.5/libmata/utils.pxd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/libmata/utils.pyx` & `libmata-1.2.5/libmata/utils.pyx`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/CMakeLists.txt` & `libmata-1.2.5/mata/3rdparty/cudd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/Doxyfile.in` & `libmata-1.2.5/mata/3rdparty/cudd/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/LICENSE` & `libmata-1.2.5/mata/3rdparty/cudd/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/README` & `libmata-1.2.5/mata/3rdparty/cudd/README`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/RELEASE.NOTES` & `libmata-1.2.5/mata/3rdparty/cudd/RELEASE.NOTES`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cplusplus/cuddObj.cc` & `libmata-1.2.5/mata/3rdparty/cudd/cplusplus/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cplusplus/test_obj.test.in` & `libmata-1.2.5/mata/3rdparty/cudd/cplusplus/test_obj.test.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cplusplus/testmulti.cc` & `libmata-1.2.5/mata/3rdparty/cudd/cplusplus/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cplusplus/testobj.cc` & `libmata-1.2.5/mata/3rdparty/cudd/cplusplus/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAPI.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddAbs.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddApply.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddFind.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddInv.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddIte.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddNeg.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAddWalsh.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAndAbs.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddAnneal.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddApa.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddApprox.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddBddAbs.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddBddCorr.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddBddIte.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddBridge.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddCache.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddCheck.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddClip.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddCof.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddCompose.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddDecomp.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddEssent.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddExact.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddExport.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddGenCof.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddGenetic.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddGroup.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddHarwell.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddInit.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddInt.h` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddInteract.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddLCache.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddLevelQ.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddLinear.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddLiteral.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddMatMult.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddPriority.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddRead.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddRef.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddReorder.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSat.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSign.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSolve.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSplit.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSubsetHB.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSubsetSP.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddSymmetry.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddTable.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddUtil.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddWindow.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddCount.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddFuncs.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddGroup.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddIsop.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddLin.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddMisc.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddPort.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddReord.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddSetop.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddSymm.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/cuddZddUtil.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/test_cudd.test.in` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/test_cudd.test.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/testcudd.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd/testextra.c` & `libmata-1.2.5/mata/3rdparty/cudd/cudd/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/cudd_config.h.in` & `libmata-1.2.5/mata/3rdparty/cudd/cudd_config.h.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/README.dddmp` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/README.dddmp`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/README.testdddmp` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/README.testdddmp`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/RELEASE_NOTES` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/RELEASE_NOTES`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmp.h` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpBinary.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpConvert.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpDbg.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpInt.h` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpLoad.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/dddmpUtil.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/0or1.bdd` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/0or1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/1.add` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/1.add`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/1.bdd` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/2.bdd` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/2.bdd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/2and3.bdd` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/2and3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/3.bdd` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.cnf` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.cnf`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.max1` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.max1`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4.max2` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4.max2`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4bis.bdd` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4bis.bdd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/dddmp/testdddmp.c` & `libmata-1.2.5/mata/3rdparty/cudd/dddmp/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/doc/cudd.tex.in` & `libmata-1.2.5/mata/3rdparty/cudd/doc/cudd.tex.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/doc/phase.pdf` & `libmata-1.2.5/mata/3rdparty/cudd/doc/phase.pdf`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/epd/epd.c` & `libmata-1.2.5/mata/3rdparty/cudd/epd/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/epd/epd.h` & `libmata-1.2.5/mata/3rdparty/cudd/epd/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/epd/epdInt.h` & `libmata-1.2.5/mata/3rdparty/cudd/epd/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/groups.dox` & `libmata-1.2.5/mata/3rdparty/cudd/groups.dox`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/include/mata/cudd/cudd.h` & `libmata-1.2.5/mata/3rdparty/cudd/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh` & `libmata-1.2.5/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/mtr/mtr.h` & `libmata-1.2.5/mata/3rdparty/cudd/mtr/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/mtr/mtrBasic.c` & `libmata-1.2.5/mata/3rdparty/cudd/mtr/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/mtr/mtrGroup.c` & `libmata-1.2.5/mata/3rdparty/cudd/mtr/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/mtr/mtrInt.h` & `libmata-1.2.5/mata/3rdparty/cudd/mtr/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/mtr/test_mtr.test.in` & `libmata-1.2.5/mata/3rdparty/cudd/mtr/test_mtr.test.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/mtr/testmtr.c` & `libmata-1.2.5/mata/3rdparty/cudd/mtr/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/st/st.c` & `libmata-1.2.5/mata/3rdparty/cudd/st/st.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/st/st.h` & `libmata-1.2.5/mata/3rdparty/cudd/st/st.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/st/testst.c` & `libmata-1.2.5/mata/3rdparty/cudd/st/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/cpu_stats.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/cpu_time.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/cstringstream.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/cstringstream.h` & `libmata-1.2.5/mata/3rdparty/cudd/util/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/datalimit.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/pathsearch.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/pipefork.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/prtime.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/safe_mem.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/strsav.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/texpand.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/ucbqsort.c` & `libmata-1.2.5/mata/3rdparty/cudd/util/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/cudd/util/util.h` & `libmata-1.2.5/mata/3rdparty/cudd/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/CMakeLists.txt` & `libmata-1.2.5/mata/3rdparty/re2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/CONTRIBUTORS` & `libmata-1.2.5/mata/3rdparty/re2/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/LICENSE` & `libmata-1.2.5/mata/3rdparty/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/bitmap256.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/compile.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/parse.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/perl_groups.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/pod_array.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/prog.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/prog.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/re2.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/re2.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/re2.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/regexp.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/regexp.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/regexp.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/simplify.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/sparse_array.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/sparse_set.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/sparse_set.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/stringpiece.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/stringpiece.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/tostring.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/unicode_casefold.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/unicode_casefold.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/unicode_groups.cc` & `libmata-1.2.5/mata/3rdparty/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/unicode_groups.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/re2/walker-inl.h` & `libmata-1.2.5/mata/3rdparty/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/util/logging.h` & `libmata-1.2.5/mata/3rdparty/re2/util/logging.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/util/mutex.h` & `libmata-1.2.5/mata/3rdparty/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/util/rune.cc` & `libmata-1.2.5/mata/3rdparty/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/util/strutil.cc` & `libmata-1.2.5/mata/3rdparty/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/util/utf.h` & `libmata-1.2.5/mata/3rdparty/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/re2/util/util.h` & `libmata-1.2.5/mata/3rdparty/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh` & `libmata-1.2.5/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/3rdparty/simlib/src/explicit_lts_sim.cc` & `libmata-1.2.5/mata/3rdparty/simlib/src/explicit_lts_sim.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/CMakeLists.txt` & `libmata-1.2.5/mata/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/Doxyfile.in` & `libmata-1.2.5/mata/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/LICENSE` & `libmata-1.2.5/mata/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/Makefile` & `libmata-1.2.5/mata/Makefile`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/README.md` & `libmata-1.2.5/mata/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -217,34 +217,15 @@
 
 # Publications
 - Chocholatý, D., Fiedor, T., Havlena, V., Holík, L., Hruška, M., Lengál, O., & Síč, J. (2023). [Mata, a Fast and Simple Finite Automata Library](https://doi.org/10.48550/arXiv.2310.10136). arXiv preprint arXiv:2310.10136.
     - Chocholatý, D., Fiedor, T., Havlena, V., Holík, L., Hruška, M., Lengál, O., Síč, J.: [A replication package for reproducing the results of paper “Mata: A fast and simple finite automata library”](https://doi.org/10.5281/zenodo.10044515) (Oct 2023).
 
 # Contributing
 
-If you'd like to contribute to the libmata, 
-please [fork the repository](https://github.com/VeriFIT/mata/fork), create a new 
-feature branch, and finally [create a new pull request](https://github.com/VeriFIT/mata/compare).
-
-In case you run into some unexpected behaviour, error or anything suspicious
-either contact us directly through mail or 
-[create a new issue](https://github.com/VeriFIT/mata/issues/new/choose).
-When creating a new issue, please, try to include everything necessary for us to know
-(such as the version, operation system, etc.) so we can sucessfully replicate the issue.
-
-## Note to main contributors
-
-By default, each merge automatically increases the `minor` version of the library
-(i.e., `0.0.0 -> 0.1.0` ). This can be overruled using either tag `#patch` (increasing
-patch version, i.e., `0.0.0 -> 0.0.1`) or `#major` (increasing major version, i.e.,
-`0.0.0 -> 1.0.0`). This tag is specified in the merge message.
-
-Generally, it is recommended to use `#major` for changes that introduces backward-incompatible
-changes for people that used previous versions, and `#patch` for minor changes, such as bug-fixes,
-performance fixes or refactoring.
+Please refer to our [contributing guidelines](CONTRIBUTING.md).
 
 # Links
 
   - Project (origin) repository: <https://github.com/verifit/mata>
   - Issue tracker: <https://github.com/verifit/mata/issues>
     - In case of some sensitive bugs (like security vulnerabilities),
       please contact us directly, instead of using issue tracker.
```

### Comparing `libmata-1.2.3/mata/cmake/GetGitRevisionDescription.cmake` & `libmata-1.2.5/mata/cmake/GetGitRevisionDescription.cmake`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/cmake/GetGitRevisionDescription.cmake.in` & `libmata-1.2.5/mata/cmake/GetGitRevisionDescription.cmake.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/cmake_uninstall.cmake.in` & `libmata-1.2.5/mata/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/alphabet.hh` & `libmata-1.2.5/mata/include/mata/alphabet.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/nfa/algorithms.hh` & `libmata-1.2.5/mata/include/mata/nfa/algorithms.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/nfa/builder.hh` & `libmata-1.2.5/mata/include/mata/nfa/builder.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/nfa/delta.hh` & `libmata-1.2.5/mata/include/mata/nfa/delta.hh`

 * *Files 0% similar despite different names*

```diff
@@ -266,17 +266,19 @@
  */
 class Delta {
 public:
     inline static const StatePost empty_state_post; // When posts[q] is not allocated, then delta[q] returns this.
 
     Delta(): state_posts_{} {}
     Delta(const Delta& other) = default;
+    Delta(Delta&& other) = default;
     explicit Delta(size_t n): state_posts_{ n } {}
 
     Delta& operator=(const Delta& other) = default;
+    Delta& operator=(Delta&& other) = default;
 
     bool operator==(const Delta& other) const;
 
     void reserve(size_t n) {
         state_posts_.reserve(n);
     };
```

### Comparing `libmata-1.2.3/mata/include/mata/nfa/nfa.hh` & `libmata-1.2.5/mata/include/mata/nfa/nfa.hh`

 * *Files 1% similar despite different names*

```diff
@@ -309,19 +309,19 @@
      * @brief Is the automaton graph acyclic? Used for checking language finiteness.
      * 
      * @return true <-> Automaton graph is acyclic.
      */
     bool is_acyclic() const;
 
     /**
-     * Fill @p alphabet with symbols from @p nfa.
-     * @param[in] nfa NFA with symbols to fill @p alphabet with.
-     * @param[out] alphabet Alphabet to be filled with symbols from @p nfa.
+     * Fill @p alphabet_to_fill with symbols from @p nfa.
+     * @param[in] nfa NFA with symbols to fill @p alphabet_to_fill with.
+     * @param[out] alphabet_to_fill Alphabet to be filled with symbols from @p nfa.
      */
-    void fill_alphabet(mata::OnTheFlyAlphabet& alphabet) const;
+    void fill_alphabet(mata::OnTheFlyAlphabet& alphabet_to_fill) const;
 
     /// Is the language of the automaton universal?
     bool is_universal(const Alphabet& alphabet, Run* cex = nullptr,
                       const ParameterMap& params = {{ "algorithm", "antichains" }}) const;
     /// Is the language of the automaton universal?
     bool is_universal(const Alphabet& alphabet, const ParameterMap& params) const;
```

### Comparing `libmata-1.2.3/mata/include/mata/nfa/plumbing.hh` & `libmata-1.2.5/mata/include/mata/nfa/plumbing.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/nfa/strings.hh` & `libmata-1.2.5/mata/include/mata/nfa/strings.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/nfa/types.hh` & `libmata-1.2.5/mata/include/mata/nfa/types.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/parser/inter-aut.hh` & `libmata-1.2.5/mata/include/mata/parser/inter-aut.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/parser/mintermization.hh` & `libmata-1.2.5/mata/include/mata/parser/mintermization.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/parser/parser.hh` & `libmata-1.2.5/mata/include/mata/parser/parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/parser/re2parser.hh` & `libmata-1.2.5/mata/include/mata/parser/re2parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/utils/closed-set.hh` & `libmata-1.2.5/mata/include/mata/utils/closed-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/utils/ord-vector.hh` & `libmata-1.2.5/mata/include/mata/utils/ord-vector.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/utils/sparse-set.hh` & `libmata-1.2.5/mata/include/mata/utils/sparse-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/utils/synchronized-iterator.hh` & `libmata-1.2.5/mata/include/mata/utils/synchronized-iterator.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/include/mata/utils/utils.hh` & `libmata-1.2.5/mata/include/mata/utils/utils.hh`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/CMakeLists.txt` & `libmata-1.2.5/mata/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/alphabet.cc` & `libmata-1.2.5/mata/src/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/inter-aut.cc` & `libmata-1.2.5/mata/src/inter-aut.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/mintermization.cc` & `libmata-1.2.5/mata/src/mintermization.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/nfa/builder.cc` & `libmata-1.2.5/mata/src/nfa/builder.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/nfa/complement.cc` & `libmata-1.2.5/mata/src/nfa/complement.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/nfa/concatenation.cc` & `libmata-1.2.5/mata/src/nfa/concatenation.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/nfa/delta.cc` & `libmata-1.2.5/mata/src/nfa/delta.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/nfa/inclusion.cc` & `libmata-1.2.5/mata/src/nfa/inclusion.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/nfa/intersection.cc` & `libmata-1.2.5/mata/src/nfa/intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/nfa/nfa.cc` & `libmata-1.2.5/mata/src/nfa/nfa.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/nfa/operations.cc` & `libmata-1.2.5/mata/src/nfa/operations.cc`

 * *Files 1% similar despite different names*

```diff
@@ -739,19 +739,19 @@
 }
 
 std::ostream& std::operator<<(std::ostream& os, const Nfa& nfa) {
     nfa.print_to_mata(os);
     return os;
 }
 
-void mata::nfa::Nfa::fill_alphabet(OnTheFlyAlphabet& alphabet) const {
+void mata::nfa::Nfa::fill_alphabet(OnTheFlyAlphabet& alphabet_to_fill) const {
     for (const StatePost& state_post: this->delta) {
         for (const SymbolPost& symbol_post: state_post) {
-            alphabet.update_next_symbol_value(symbol_post.symbol);
-            alphabet.try_add_new_symbol(std::to_string(symbol_post.symbol), symbol_post.symbol);
+            alphabet_to_fill.update_next_symbol_value(symbol_post.symbol);
+            alphabet_to_fill.try_add_new_symbol(std::to_string(symbol_post.symbol), symbol_post.symbol);
         }
     }
 }
 
 mata::OnTheFlyAlphabet mata::nfa::create_alphabet(const std::vector<std::reference_wrapper<const Nfa>>& nfas) {
     mata::OnTheFlyAlphabet alphabet{};
     for (const auto& nfa: nfas) {
```

### Comparing `libmata-1.2.3/mata/src/nfa/universal.cc` & `libmata-1.2.5/mata/src/nfa/universal.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/parser.cc` & `libmata-1.2.5/mata/src/parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/re2parser.cc` & `libmata-1.2.5/mata/src/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/strings/nfa-noodlification.cc` & `libmata-1.2.5/mata/src/strings/nfa-noodlification.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/strings/nfa-segmentation.cc` & `libmata-1.2.5/mata/src/strings/nfa-segmentation.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/mata/src/strings/nfa-strings.cc` & `libmata-1.2.5/mata/src/strings/nfa-strings.cc`

 * *Files identical despite different names*

### Comparing `libmata-1.2.3/setup.py` & `libmata-1.2.5/setup.py`

 * *Files identical despite different names*

