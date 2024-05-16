# Comparing `tmp/pxblat-1.1.9.tar.gz` & `tmp/pxblat-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxblat-1.1.9.tar", max compression
+gzip compressed data, was "pxblat-1.2.1.tar", max compression
```

## Comparing `pxblat-1.1.9.tar` & `pxblat-1.2.1.tar`

### file list

```diff
@@ -1,198 +1,198 @@
--rw-r--r--   0        0        0      269 2023-10-31 21:59:27.475692 pxblat-1.1.9/LICENSE
--rw-r--r--   0        0        0    11103 2023-10-31 21:59:27.475692 pxblat-1.1.9/README.md
--rw-r--r--   0        0        0     9281 2023-10-31 21:59:27.923700 pxblat-1.1.9/build.py
--rw-r--r--   0        0        0     6251 2023-10-31 21:59:27.983701 pxblat-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     1542 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/__init__.py
--rw-r--r--   0        0        0      116 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/cli/__init__.py
--rw-r--r--   0        0        0      961 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/cli/cli.py
--rw-r--r--   0        0        0     5997 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/cli/client.py
--rw-r--r--   0        0        0     2563 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/cli/fa2twobit.py
--rw-r--r--   0        0        0      227 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/cli/log.py
--rw-r--r--   0        0        0     7904 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/cli/server.py
--rw-r--r--   0        0        0     3559 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/cli/twobit2fa.py
--rw-r--r--   0        0        0      555 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/extc/__init__.py
--rw-r--r--   0        0        0    27386 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/extc/__init__.pyi
--rw-r--r--   0        0        0       40 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/.clang-format
--rw-r--r--   0        0        0     2083 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/_extc.cpp
--rw-r--r--   0        0        0       11 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/_extc.modules
--rw-r--r--   0        0        0       81 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/_extc.sources
--rw-r--r--   0        0        0     2163 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
--rw-r--r--   0        0        0    10825 2023-10-31 21:59:27.983701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/gfClient.cpp
--rw-r--r--   0        0        0    20049 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/gfServer.cpp
--rw-r--r--   0        0        0     2715 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/gfServer_1.cpp
--rw-r--r--   0        0        0     4632 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/pygfServer.cpp
--rw-r--r--   0        0        0     5912 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/binder/twoBitToFa.cpp
--rw-r--r--   0        0        0    33509 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/bs_thread_pool.hpp
--rw-r--r--   0        0        0    28417 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/dbg.h
--rw-r--r--   0        0        0     2116 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/faToTwoBit.cpp
--rw-r--r--   0        0        0     1243 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/faToTwoBit.hpp
--rw-r--r--   0        0        0    13652 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/gfClient.cpp
--rw-r--r--   0        0        0     4820 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/gfClient.hpp
--rw-r--r--   0        0        0    60623 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/gfServer.cpp
--rw-r--r--   0        0        0    11419 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/gfServer.hpp
--rw-r--r--   0        0        0    11325 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/pygfServer.cpp
--rw-r--r--   0        0        0      973 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/pygfServer.hpp
--rw-r--r--   0        0        0     8728 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/twoBitToFa.cpp
--rw-r--r--   0        0        0     3521 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/bindings/twoBitToFa.hpp
--rw-r--r--   0        0        0    24597 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/blat.c
--rw-r--r--   0        0        0     3485 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/faToTwoBit.c
--rw-r--r--   0        0        0     9944 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/gfClient.c
--rw-r--r--   0        0        0    53782 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/gfServer.c
--rw-r--r--   0        0        0       40 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/.clang-format
--rw-r--r--   0        0        0     2088 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/bandExt.h
--rw-r--r--   0        0        0     1073 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/base64.h
--rw-r--r--   0        0        0    27036 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/cheapcgi.h
--rw-r--r--   0        0        0     2097 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/filePath.h
--rw-r--r--   0        0        0      871 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/gfxPoly.h
--rw-r--r--   0        0        0     1034 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/hex.h
--rw-r--r--   0        0        0    10111 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/htmlPage.h
--rw-r--r--   0        0        0     9985 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/htmshell.h
--rw-r--r--   0        0        0      332 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/https.h
--rw-r--r--   0        0        0     4404 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/internet.h
--rw-r--r--   0        0        0     1990 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/kxTok.h
--rw-r--r--   0        0        0    16767 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/memgfx.h
--rw-r--r--   0        0        0     2997 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/mime.h
--rw-r--r--   0        0        0     1166 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/portimpl.h
--rw-r--r--   0        0        0     4401 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/rbTree.h
--rw-r--r--   0        0        0      164 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/aux/srcVersion.h
--rw-r--r--   0        0        0      916 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/aliType.h
--rw-r--r--   0        0        0     6547 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/asParse.h
--rw-r--r--   0        0        0    10193 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/axt.h
--rw-r--r--   0        0        0     6470 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/bPlusTree.h
--rw-r--r--   0        0        0    14293 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/basicBed.h
--rw-r--r--   0        0        0     4355 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/binRange.h
--rw-r--r--   0        0        0     3456 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/bits.h
--rw-r--r--   0        0        0     5877 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/chain.h
--rw-r--r--   0        0        0     1839 2023-10-31 21:59:27.987701 pxblat-1.1.9/src/pxblat/extc/include/core/chainBlock.h
--rw-r--r--   0        0        0    56916 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/common.h
--rw-r--r--   0        0        0     4198 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/dlist.h
--rw-r--r--   0        0        0     2681 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/dnaseq.h
--rw-r--r--   0        0        0    10058 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/dnautil.h
--rw-r--r--   0        0        0     3658 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/dystring.h
--rw-r--r--   0        0        0     2795 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/errAbort.h
--rw-r--r--   0        0        0     2128 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/errCatch.h
--rw-r--r--   0        0        0     5228 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/fa.h
--rw-r--r--   0        0        0    10590 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/fuzzyFind.h
--rw-r--r--   0        0        0    19945 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/genoFind.h
--rw-r--r--   0        0        0     1115 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/gfClientLib.h
--rw-r--r--   0        0        0     2884 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/gfInternal.h
--rw-r--r--   0        0        0    12187 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/hash.h
--rw-r--r--   0        0        0     1111 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/htmlColor.h
--rw-r--r--   0        0        0    14055 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/linefile.h
--rw-r--r--   0        0        0     3618 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/localmem.h
--rw-r--r--   0        0        0    10130 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/maf.h
--rw-r--r--   0        0        0     1786 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/memalloc.h
--rw-r--r--   0        0        0    12155 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/net.h
--rw-r--r--   0        0        0    12162 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/netlib.h
--rw-r--r--   0        0        0     4114 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/nib.h
--rw-r--r--   0        0        0     8773 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/obscure.h
--rw-r--r--   0        0        0      605 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/ooc.h
--rw-r--r--   0        0        0     3981 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/options.h
--rw-r--r--   0        0        0     1910 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/patSpace.h
--rw-r--r--   0        0        0     7300 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/pipeline.h
--rw-r--r--   0        0        0     6256 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/portable.h
--rw-r--r--   0        0        0    14633 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/psl.h
--rw-r--r--   0        0        0     4818 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/rangeTree.h
--rw-r--r--   0        0        0     2459 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/repMask.h
--rw-r--r--   0        0        0     3070 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/sig.h
--rw-r--r--   0        0        0     6814 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/sqlList.h
--rw-r--r--   0        0        0     3444 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/sqlNum.h
--rw-r--r--   0        0        0     2492 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/supStitch.h
--rw-r--r--   0        0        0     2499 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/tokenizer.h
--rw-r--r--   0        0        0     2086 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/trans3.h
--rw-r--r--   0        0        0     8657 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/twoBit.h
--rw-r--r--   0        0        0     9058 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/udc.h
--rw-r--r--   0        0        0     1821 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/core/verbose.h
--rw-r--r--   0        0        0        0 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/net/gfNet.h
--rw-r--r--   0        0        0     2278 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/include/net/log.h
--rw-r--r--   0        0        0       40 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/.clang-format
--rw-r--r--   0        0        0    31426 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/axt.c
--rw-r--r--   0        0        0    14386 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/bandExt.c
--rw-r--r--   0        0        0     2996 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/base64.c
--rw-r--r--   0        0        0    11289 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/binRange.c
--rw-r--r--   0        0        0    25709 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/blastOut.c
--rw-r--r--   0        0        0    80472 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/cheapcgi.c
--rw-r--r--   0        0        0    32618 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/ffSeedExtend.c
--rw-r--r--   0        0        0     6436 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/filePath.c
--rw-r--r--   0        0        0     2363 2023-10-31 21:59:27.991701 pxblat-1.1.9/src/pxblat/extc/src/aux/hex.c
--rw-r--r--   0        0        0    53011 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/htmlPage.c
--rw-r--r--   0        0        0    46630 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/htmshell.c
--rw-r--r--   0        0        0    27672 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/https.c
--rw-r--r--   0        0        0     2489 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/intExp.c
--rw-r--r--   0        0        0    16703 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/internet.c
--rw-r--r--   0        0        0    24031 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/maf.c
--rw-r--r--   0        0        0     2306 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/mafFromAxt.c
--rw-r--r--   0        0        0    16690 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/mime.c
--rw-r--r--   0        0        0    62706 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/net.c
--rw-r--r--   0        0        0    62778 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/netlib.c
--rw-r--r--   0        0        0     1742 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/ooc.c
--rw-r--r--   0        0        0    11962 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/patSpace.c
--rw-r--r--   0        0        0     3896 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/portimpl.c
--rw-r--r--   0        0        0    13003 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/rangeTree.c
--rw-r--r--   0        0        0    18572 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/rbTree.c
--rw-r--r--   0        0        0     5678 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/repMask.c
--rw-r--r--   0        0        0      848 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/servBrcMcw.c
--rw-r--r--   0        0        0     1033 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/servCrunx.c
--rw-r--r--   0        0        0      864 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/servcis.c
--rw-r--r--   0        0        0      906 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/servmsII.c
--rw-r--r--   0        0        0      921 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/servpws.c
--rw-r--r--   0        0        0    27041 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/sqlList.c
--rw-r--r--   0        0        0     7239 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/sqlNum.c
--rw-r--r--   0        0        0     3898 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/aux/wildcmp.c
--rw-r--r--   0        0        0      930 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/core/aliType.c
--rw-r--r--   0        0        0    21737 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/core/asParse.c
--rw-r--r--   0        0        0    19732 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/core/bPlusTree.c
--rw-r--r--   0        0        0    54752 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/core/basicBed.c
--rw-r--r--   0        0        0     9051 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/core/bits.c
--rw-r--r--   0        0        0    17259 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/core/chain.c
--rw-r--r--   0        0        0    17077 2023-10-31 21:59:27.995701 pxblat-1.1.9/src/pxblat/extc/src/core/chainBlock.c
--rw-r--r--   0        0        0    90522 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/common.c
--rw-r--r--   0        0        0     9450 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/dlist.c
--rw-r--r--   0        0        0     4604 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/dnaseq.c
--rw-r--r--   0        0        0    29952 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/dnautil.c
--rw-r--r--   0        0        0     7156 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/dystring.c
--rw-r--r--   0        0        0    12046 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/errAbort.c
--rw-r--r--   0        0        0     3932 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/errCatch.c
--rw-r--r--   0        0        0    15611 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/fa.c
--rw-r--r--   0        0        0     3714 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/ffAli.c
--rw-r--r--   0        0        0    10802 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/ffAliHelp.c
--rw-r--r--   0        0        0     4868 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/ffScore.c
--rw-r--r--   0        0        0    40189 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/fuzzyFind.c
--rw-r--r--   0        0        0    70461 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/genoFind.c
--rw-r--r--   0        0        0    52425 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/gfBlatLib.c
--rw-r--r--   0        0        0     6363 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/gfClientLib.c
--rw-r--r--   0        0        0     3845 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/gfInternal.c
--rw-r--r--   0        0        0    18190 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/gfOut.c
--rw-r--r--   0        0        0    22265 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/hash.c
--rw-r--r--   0        0        0     2919 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/htmlColor.c
--rw-r--r--   0        0        0     5273 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/kxTok.c
--rw-r--r--   0        0        0    40744 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/linefile.c
--rw-r--r--   0        0        0     7256 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/localmem.c
--rw-r--r--   0        0        0    15074 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/memalloc.c
--rw-r--r--   0        0        0    12778 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/nib.c
--rw-r--r--   0        0        0    24969 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/obscure.c
--rw-r--r--   0        0        0    13012 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/options.c
--rw-r--r--   0        0        0    20522 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/osunix.c
--rw-r--r--   0        0        0    23419 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/pipeline.c
--rw-r--r--   0        0        0    63467 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/psl.c
--rw-r--r--   0        0        0     1203 2023-10-31 21:59:27.999701 pxblat-1.1.9/src/pxblat/extc/src/core/servcl.c
--rw-r--r--   0        0        0    26961 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/src/core/supStitch.c
--rw-r--r--   0        0        0     5025 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/src/core/tokenizer.c
--rw-r--r--   0        0        0     3216 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/src/core/trans3.c
--rw-r--r--   0        0        0    33527 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/src/core/twoBit.c
--rw-r--r--   0        0        0    71967 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/src/core/udc.c
--rw-r--r--   0        0        0     4255 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/src/core/verbose.c
--rw-r--r--   0        0        0     2571 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/src/net/gfNet.c
--rw-r--r--   0        0        0     8795 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/src/net/log.c
--rw-r--r--   0        0        0     7666 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/extc/twoBitToFa.c
--rw-r--r--   0        0        0     6472 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/parser.py
--rw-r--r--   0        0        0        0 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/py.typed
--rw-r--r--   0        0        0      873 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/server/__init__.py
--rw-r--r--   0        0        0    16183 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/server/basic.py
--rw-r--r--   0        0        0    20278 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/server/client.py
--rw-r--r--   0        0        0    19995 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/server/server.py
--rw-r--r--   0        0        0     1812 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/server/status.py
--rw-r--r--   0        0        0      114 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/server/utils.py
--rw-r--r--   0        0        0     2930 2023-10-31 21:59:28.003701 pxblat-1.1.9/src/pxblat/toolkit/__init__.py
--rw-r--r--   0        0        0    12819 1970-01-01 00:00:00.000000 pxblat-1.1.9/setup.py
--rw-r--r--   0        0        0    12497 1970-01-01 00:00:00.000000 pxblat-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0      269 2024-05-16 05:48:50.273435 pxblat-1.2.1/LICENSE
+-rw-r--r--   0        0        0    11103 2024-05-16 05:48:50.273435 pxblat-1.2.1/README.md
+-rw-r--r--   0        0        0     9865 2024-05-16 05:48:50.745433 pxblat-1.2.1/build.py
+-rw-r--r--   0        0        0     6367 2024-05-16 05:48:50.801433 pxblat-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1248 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/__init__.py
+-rw-r--r--   0        0        0      117 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/cli/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/cli/cli.py
+-rw-r--r--   0        0        0     5997 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/cli/client.py
+-rw-r--r--   0        0        0     2563 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/cli/fa2twobit.py
+-rw-r--r--   0        0        0      227 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/cli/log.py
+-rw-r--r--   0        0        0     8161 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/cli/server.py
+-rw-r--r--   0        0        0     3559 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/cli/twobit2fa.py
+-rw-r--r--   0        0        0      555 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/__init__.py
+-rw-r--r--   0        0        0    27386 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/__init__.pyi
+-rw-r--r--   0        0        0       40 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/.clang-format
+-rw-r--r--   0        0        0     2083 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/_extc.cpp
+-rw-r--r--   0        0        0       11 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/_extc.modules
+-rw-r--r--   0        0        0       81 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/_extc.sources
+-rw-r--r--   0        0        0     2163 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
+-rw-r--r--   0        0        0    10825 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/gfClient.cpp
+-rw-r--r--   0        0        0    20049 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/gfServer.cpp
+-rw-r--r--   0        0        0     2715 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/gfServer_1.cpp
+-rw-r--r--   0        0        0     4632 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/pygfServer.cpp
+-rw-r--r--   0        0        0     5912 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/binder/twoBitToFa.cpp
+-rw-r--r--   0        0        0    33509 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/bs_thread_pool.hpp
+-rw-r--r--   0        0        0    28417 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/dbg.h
+-rw-r--r--   0        0        0     2116 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/faToTwoBit.cpp
+-rw-r--r--   0        0        0     1243 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/faToTwoBit.hpp
+-rw-r--r--   0        0        0    13652 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/gfClient.cpp
+-rw-r--r--   0        0        0     4820 2024-05-16 05:48:50.801433 pxblat-1.2.1/src/pxblat/extc/bindings/gfClient.hpp
+-rw-r--r--   0        0        0    60623 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/bindings/gfServer.cpp
+-rw-r--r--   0        0        0    11419 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/bindings/gfServer.hpp
+-rw-r--r--   0        0        0    11325 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/bindings/pygfServer.cpp
+-rw-r--r--   0        0        0      973 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/bindings/pygfServer.hpp
+-rw-r--r--   0        0        0     8728 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/bindings/twoBitToFa.cpp
+-rw-r--r--   0        0        0     3521 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/bindings/twoBitToFa.hpp
+-rw-r--r--   0        0        0    24597 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/blat.c
+-rw-r--r--   0        0        0     3485 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/faToTwoBit.c
+-rw-r--r--   0        0        0     9944 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/gfClient.c
+-rw-r--r--   0        0        0    53782 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/gfServer.c
+-rw-r--r--   0        0        0       40 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/.clang-format
+-rw-r--r--   0        0        0     2088 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/bandExt.h
+-rw-r--r--   0        0        0     1073 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/base64.h
+-rw-r--r--   0        0        0    27036 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/cheapcgi.h
+-rw-r--r--   0        0        0     2097 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/filePath.h
+-rw-r--r--   0        0        0      871 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/gfxPoly.h
+-rw-r--r--   0        0        0     1034 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/hex.h
+-rw-r--r--   0        0        0    10111 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/htmlPage.h
+-rw-r--r--   0        0        0     9985 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/htmshell.h
+-rw-r--r--   0        0        0      332 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/https.h
+-rw-r--r--   0        0        0     4404 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/internet.h
+-rw-r--r--   0        0        0     1990 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/kxTok.h
+-rw-r--r--   0        0        0    16767 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/memgfx.h
+-rw-r--r--   0        0        0     2997 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/mime.h
+-rw-r--r--   0        0        0     1166 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/portimpl.h
+-rw-r--r--   0        0        0     4401 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/rbTree.h
+-rw-r--r--   0        0        0      164 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/aux/srcVersion.h
+-rw-r--r--   0        0        0      916 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/aliType.h
+-rw-r--r--   0        0        0     6547 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/asParse.h
+-rw-r--r--   0        0        0    10193 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/axt.h
+-rw-r--r--   0        0        0     6470 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/bPlusTree.h
+-rw-r--r--   0        0        0    14293 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/basicBed.h
+-rw-r--r--   0        0        0     4355 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/binRange.h
+-rw-r--r--   0        0        0     3456 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/bits.h
+-rw-r--r--   0        0        0     5877 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/chain.h
+-rw-r--r--   0        0        0     1839 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/chainBlock.h
+-rw-r--r--   0        0        0    56916 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/common.h
+-rw-r--r--   0        0        0     4198 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/dlist.h
+-rw-r--r--   0        0        0     2681 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/dnaseq.h
+-rw-r--r--   0        0        0    10058 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/dnautil.h
+-rw-r--r--   0        0        0     3658 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/dystring.h
+-rw-r--r--   0        0        0     2795 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/errAbort.h
+-rw-r--r--   0        0        0     2128 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/errCatch.h
+-rw-r--r--   0        0        0     5228 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/fa.h
+-rw-r--r--   0        0        0    10590 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/fuzzyFind.h
+-rw-r--r--   0        0        0    19945 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/genoFind.h
+-rw-r--r--   0        0        0     1115 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/gfClientLib.h
+-rw-r--r--   0        0        0     2884 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/gfInternal.h
+-rw-r--r--   0        0        0    12187 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/hash.h
+-rw-r--r--   0        0        0     1111 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/htmlColor.h
+-rw-r--r--   0        0        0    14055 2024-05-16 05:48:50.805433 pxblat-1.2.1/src/pxblat/extc/include/core/linefile.h
+-rw-r--r--   0        0        0     3618 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/localmem.h
+-rw-r--r--   0        0        0    10130 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/maf.h
+-rw-r--r--   0        0        0     1786 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/memalloc.h
+-rw-r--r--   0        0        0    12155 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/net.h
+-rw-r--r--   0        0        0    12162 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/netlib.h
+-rw-r--r--   0        0        0     4114 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/nib.h
+-rw-r--r--   0        0        0     8773 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/obscure.h
+-rw-r--r--   0        0        0      605 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/ooc.h
+-rw-r--r--   0        0        0     3981 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/options.h
+-rw-r--r--   0        0        0     1910 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/patSpace.h
+-rw-r--r--   0        0        0     7300 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/pipeline.h
+-rw-r--r--   0        0        0     6256 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/portable.h
+-rw-r--r--   0        0        0    14633 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/psl.h
+-rw-r--r--   0        0        0     4818 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/rangeTree.h
+-rw-r--r--   0        0        0     2459 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/repMask.h
+-rw-r--r--   0        0        0     3070 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/sig.h
+-rw-r--r--   0        0        0     6814 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/sqlList.h
+-rw-r--r--   0        0        0     3444 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/sqlNum.h
+-rw-r--r--   0        0        0     2492 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/supStitch.h
+-rw-r--r--   0        0        0     2499 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/tokenizer.h
+-rw-r--r--   0        0        0     2086 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/trans3.h
+-rw-r--r--   0        0        0     8657 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/twoBit.h
+-rw-r--r--   0        0        0     9058 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/udc.h
+-rw-r--r--   0        0        0     1821 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/core/verbose.h
+-rw-r--r--   0        0        0        0 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/net/gfNet.h
+-rw-r--r--   0        0        0     2278 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/include/net/log.h
+-rw-r--r--   0        0        0       40 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/.clang-format
+-rw-r--r--   0        0        0    31426 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/axt.c
+-rw-r--r--   0        0        0    14386 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/bandExt.c
+-rw-r--r--   0        0        0     2996 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/base64.c
+-rw-r--r--   0        0        0    11289 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/binRange.c
+-rw-r--r--   0        0        0    25709 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/blastOut.c
+-rw-r--r--   0        0        0    80472 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/cheapcgi.c
+-rw-r--r--   0        0        0    32618 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/ffSeedExtend.c
+-rw-r--r--   0        0        0     6436 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/filePath.c
+-rw-r--r--   0        0        0     2363 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/hex.c
+-rw-r--r--   0        0        0    53011 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/htmlPage.c
+-rw-r--r--   0        0        0    46630 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/htmshell.c
+-rw-r--r--   0        0        0    27672 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/https.c
+-rw-r--r--   0        0        0     2489 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/intExp.c
+-rw-r--r--   0        0        0    16703 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/internet.c
+-rw-r--r--   0        0        0    24031 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/maf.c
+-rw-r--r--   0        0        0     2306 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/mafFromAxt.c
+-rw-r--r--   0        0        0    16690 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/mime.c
+-rw-r--r--   0        0        0    62706 2024-05-16 05:48:50.809433 pxblat-1.2.1/src/pxblat/extc/src/aux/net.c
+-rw-r--r--   0        0        0    62778 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/netlib.c
+-rw-r--r--   0        0        0     1742 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/ooc.c
+-rw-r--r--   0        0        0    11962 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/patSpace.c
+-rw-r--r--   0        0        0     3896 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/portimpl.c
+-rw-r--r--   0        0        0    13003 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/rangeTree.c
+-rw-r--r--   0        0        0    18572 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/rbTree.c
+-rw-r--r--   0        0        0     5678 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/repMask.c
+-rw-r--r--   0        0        0      848 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/servBrcMcw.c
+-rw-r--r--   0        0        0     1033 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/servCrunx.c
+-rw-r--r--   0        0        0      864 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/servcis.c
+-rw-r--r--   0        0        0      906 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/servmsII.c
+-rw-r--r--   0        0        0      921 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/servpws.c
+-rw-r--r--   0        0        0    27041 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/sqlList.c
+-rw-r--r--   0        0        0     7239 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/sqlNum.c
+-rw-r--r--   0        0        0     3898 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/aux/wildcmp.c
+-rw-r--r--   0        0        0      930 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/aliType.c
+-rw-r--r--   0        0        0    21737 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/asParse.c
+-rw-r--r--   0        0        0    19732 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/bPlusTree.c
+-rw-r--r--   0        0        0    54752 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/basicBed.c
+-rw-r--r--   0        0        0     9051 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/bits.c
+-rw-r--r--   0        0        0    17259 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/chain.c
+-rw-r--r--   0        0        0    17077 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/chainBlock.c
+-rw-r--r--   0        0        0    90522 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/common.c
+-rw-r--r--   0        0        0     9450 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/dlist.c
+-rw-r--r--   0        0        0     4604 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/dnaseq.c
+-rw-r--r--   0        0        0    29952 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/dnautil.c
+-rw-r--r--   0        0        0     7156 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/dystring.c
+-rw-r--r--   0        0        0    12046 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/errAbort.c
+-rw-r--r--   0        0        0     3932 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/errCatch.c
+-rw-r--r--   0        0        0    15611 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/fa.c
+-rw-r--r--   0        0        0     3714 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/ffAli.c
+-rw-r--r--   0        0        0    10802 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/ffAliHelp.c
+-rw-r--r--   0        0        0     4868 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/ffScore.c
+-rw-r--r--   0        0        0    40189 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/fuzzyFind.c
+-rw-r--r--   0        0        0    70461 2024-05-16 05:48:50.813433 pxblat-1.2.1/src/pxblat/extc/src/core/genoFind.c
+-rw-r--r--   0        0        0    52425 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/gfBlatLib.c
+-rw-r--r--   0        0        0     6363 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/gfClientLib.c
+-rw-r--r--   0        0        0     3845 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/gfInternal.c
+-rw-r--r--   0        0        0    18190 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/gfOut.c
+-rw-r--r--   0        0        0    22265 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/hash.c
+-rw-r--r--   0        0        0     2919 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/htmlColor.c
+-rw-r--r--   0        0        0     5273 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/kxTok.c
+-rw-r--r--   0        0        0    40744 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/linefile.c
+-rw-r--r--   0        0        0     7256 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/localmem.c
+-rw-r--r--   0        0        0    15074 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/memalloc.c
+-rw-r--r--   0        0        0    12778 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/nib.c
+-rw-r--r--   0        0        0    24969 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/obscure.c
+-rw-r--r--   0        0        0    13012 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/options.c
+-rw-r--r--   0        0        0    20522 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/osunix.c
+-rw-r--r--   0        0        0    23419 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/pipeline.c
+-rw-r--r--   0        0        0    63467 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/psl.c
+-rw-r--r--   0        0        0     1203 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/servcl.c
+-rw-r--r--   0        0        0    26961 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/supStitch.c
+-rw-r--r--   0        0        0     5025 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/tokenizer.c
+-rw-r--r--   0        0        0     3216 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/trans3.c
+-rw-r--r--   0        0        0    33527 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/twoBit.c
+-rw-r--r--   0        0        0    71967 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/udc.c
+-rw-r--r--   0        0        0     4255 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/core/verbose.c
+-rw-r--r--   0        0        0     2571 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/net/gfNet.c
+-rw-r--r--   0        0        0     8795 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/src/net/log.c
+-rw-r--r--   0        0        0     7666 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/extc/twoBitToFa.c
+-rw-r--r--   0        0        0     7345 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/parser.py
+-rw-r--r--   0        0        0        0 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/py.typed
+-rw-r--r--   0        0        0      910 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/server/__init__.py
+-rw-r--r--   0        0        0    16730 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/server/basic.py
+-rw-r--r--   0        0        0    20104 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/server/client.py
+-rw-r--r--   0        0        0    19968 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/server/server.py
+-rw-r--r--   0        0        0     1812 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/server/status.py
+-rw-r--r--   0        0        0      114 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/server/utils.py
+-rw-r--r--   0        0        0     2931 2024-05-16 05:48:50.817433 pxblat-1.2.1/src/pxblat/toolkit/__init__.py
+-rw-r--r--   0        0        0    12815 1970-01-01 00:00:00.000000 pxblat-1.2.1/setup.py
+-rw-r--r--   0        0        0    12493 1970-01-01 00:00:00.000000 pxblat-1.2.1/PKG-INFO
```

### Comparing `pxblat-1.1.9/README.md` & `pxblat-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/build.py` & `pxblat-1.2.1/build.py`

 * *Files 15% similar despite different names*

```diff
@@ -156,23 +156,41 @@
         return Path.cwd(), Path.cwd()
 
     header_path = Path(lib_path).parent.parent / "include"
 
     return Path(lib_path).parent, header_path
 
 
-def find_openssl_libs():
-    openssl_dir = subprocess.getoutput('openssl version -d')
-    openssl_dir = openssl_dir.replace('OPENSSLDIR: "', '').replace('"', '').strip()
+def find_openssl_libs_header():
+    from shutil import which
+    import platform
 
-    lib_paths = [f"{openssl_dir}/lib"]
+    current_platform = platform.system().lower()
 
-    print(f"find openssl lib_paths: {lib_paths}")
+    lib_paths = []
+    head_paths = []
+
+    if current_platform == "darwin" and which("brew"):
+        openssl_dir = subprocess.getoutput('brew --prefix openssl')
+
+        lib_paths.append(f"{openssl_dir}/lib")
+        head_paths.append(f"{openssl_dir}/include")
+
+        if not Path(lib_paths[0]).exists():
+            print(f"Cannot find openssl lib in {lib_paths[0]}")
+        else:
+            print(f"Find openssl lib_paths: {lib_paths}")
+
+        if not Path(head_paths[0]).exists():
+            print(f"Cannot find openssl include in {head_paths[0]}")
+        else:
+            print(f"Find openssl include: {head_paths}")
+
+    return lib_paths, head_paths
 
-    return lib_paths
 
 def _extra_compile_args_for_libpxblat():
     return [
         "-D_FILE_OFFSET_BITS=64",
         "-D_LARGEFILE_SOURCE",
         "-D_GNU_SOURCE",
         "-DMACHTYPE_$(MACHTYPE)",
@@ -199,18 +217,21 @@
     if not DEBUG:
         flag.append("-DDBG_MACRO_DISABLE")
     return flag
 
 
 ParallelCompile(f"{get_thread_count()}").install()
 
+
+openssl_lib, openssl_include = find_openssl_libs_header()
+
 extra_compile_args = ["-pthread"]
 hidden_visibility_args = []
-include_dirs: list[str] = []
-library_dirs: list[str] = [] + find_openssl_libs()
+include_dirs: list[str] = [] + openssl_include
+library_dirs: list[str] = [] + openssl_lib
 python_module_link_args = []
 base_library_link_args: list[str] = []
 external_libraries = [
     "ssl",
     "crypto",
     "m",
 ]
```

### Comparing `pxblat-1.1.9/pyproject.toml` & `pxblat-1.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxblat"
-version = "1.1.9"
+version = "1.2.1"
 description = "A native python binding for blat suite"
 authors = ["Yangyang Li <yangyang.li@northwestern.edu>"]
 homepage = "https://github.com/ylab-hi/pxblat"
 documentation = "https://pxblat.readthedocs.io/en/latest/"
 repository = "https://github.com/ylab-hi/pxblat"
 readme = "README.md"
 license = "LICENSE"
@@ -22,72 +22,71 @@
 ]
 keywords = ["bioinformatics", "sequence aligner", "blat"]
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 loguru = "^0.7.0"
 pybind11 = "^2.10.4"
-setuptools = "^68.2.2"
+setuptools = ">=68.2.2,<70.0.0"
 rich = "^13.3.5"
-pysimdjson = "^5.0.2"
+pysimdjson = ">=5.0.2,<7.0.0"
 biopython = "^1.81"
 deprecated = "^1.2.13"
 mashumaro = "^3.7"
-urllib3 = "2.0.7"
-typer = "^0.9.0"
+urllib3 = "2.2.1"
+typer = ">=0.9,<0.13"
 
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
-pytest-sugar = "^0.9.7"
-black = "^23.3.0"
-pybind11-stubgen = ">=0.13,<2.4"
+pytest = ">=7.3.1,<9.0.0"
+pytest-sugar = ">=0.9.7,<1.1.0"
+pybind11-stubgen = ">=0.13,<2.6"
 invoke = "^2.1.2"
 ipdb = "^0.13.13"
-pysam = ">=0.21,<0.23"
 pytest-ordering = "^0.6"
 pytest-xdist = "^3.3.1"
 scienceplots = "^2.0.1"
 tikzplotlib = "^0.10.1"
-nox = "^2023.4.22"
+nox = ">=2023.4.22,<2025.0.0"
 nox-poetry = "^1.0.2"
 codecov = "^2.1.13"
-myst-parser = ">=1,<3"
+myst-parser = ">=1,<4"
 sphinx-immaterial = { extras = [
     "clang-format",
     "cpp",
     "json",
     "keys",
-], version = "^0.11.6" }
+], version = "^0.11.11" }
 linkify-it-py = "^2.0.2"
 sphinx-copybutton = "^0.5.2"
 sphinx-togglebutton = "^0.3.2"
 sphinxcontrib-bibtex = "^2.5.0"
 sphinx-autoapi = ">=2.1,<4.0"
-sphinx-autodoc2 = "^0.4.2"
+sphinx-autodoc2 = ">=0.4.2,<0.6.0"
 psutil = "^5.9.5"
 seaborn = ">=0.12.2,<0.14.0"
 mypy = "^1.4.1"
 sphinx-click = ">=4.4,<6.0"
 py-spy = "^0.3.14"
-sphinx-autobuild = "^2021.3.14"
+sphinx-autobuild = ">=2021.3.14,<2025.0.0"
 cibuildwheel = "^2.16.2"
-ruff = "^0.1.2"
+ruff = ">=0.1.2,<0.5.0"
+delocate = ">=0.10.4,<0.12.0"
 
 
 [tool.poetry.scripts]
 pxblat = "pxblat.cli.cli:app"
 
 
 [tool.ruff]
 target-version = "py38"
 line-length = 120
 fix = true
-fixable = ["ALL"]
-select = [
+lint.fixable = ["ALL"]
+lint.select = [
     "ANN",
     "D",
     "A",
     "F",
     "E",
     "W",
     "C90",
@@ -131,15 +130,15 @@
     "PIE",
     "ISC",
     "FA",
     "EXE",
     # "CPY",
     "COM",
 ]
-ignore = [
+lint.ignore = [
     "E501",
     "D203",
     "D100",
     "D401",
     "ANN101",
     "ANN102",
     "ANN001",
@@ -195,35 +194,36 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
+    "figures",
 
 ]
 
 
 [tool.ruff.format]
 # Like Black, use double quotes for strings.
 quote-style = "double"
 # Like Black, indent with spaces, rather than tabs.
 indent-style = "space"
 # Like Black, respect magic trailing commas.
 # magic-trailing-comma = "respect"
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 
-[tool.ruff.flake8-bugbear]
+[tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = ["chr", "typer.Argument", "typer.Option"]
 
-[tool.ruff.flake8-annotations]
+[tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "src/pxblat/cli/twobit2fa.py" = ["B008", "PLR0913", "FBT001", "FBT003"]
 "src/pxblat/extc/__init__.py" = ["F405", "F403", "D104", "D103", "TID252"]
 "src/pxblat/server/basic.py" = ["PLR0913"]
 "src/pxblat/server/server.py" = ["PLR0913", "D102"]
 "src/pxblat/server/client.py" = ["PLR0913"]
 "src/pxblat/cli/server.py" = ["PLR0913", "N816", "FBT001", "FBT003"]
 "src/pxblat/cli/client.py" = ["B008", "PLR0913", "FBT001", "FBT003"]
@@ -233,15 +233,15 @@
 "src/pxblat/parser.py" = ["A001", "A002", "ARG001"]
 "docs/tutorial_data/query_context.py" = ["T201", "D103"]
 "docs/tutorial_data/2bit.py" = ["T201", "D103"]
 "docs/tutorial_data/query_general.py" = ["T201", "D103"]
 "docs/tutorial_data/query_result.py" = ["T201", "D103"]
 "docs/tutorial_data/blat.py" = ["T201", "D103"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = 'google'
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
```

### Comparing `pxblat-1.1.9/src/pxblat/cli/cli.py` & `pxblat-1.2.1/src/pxblat/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command line interface for pxblat."""
+
 import sys
 from datetime import datetime
 
 import typer
 
 from pxblat import __version__
```

### Comparing `pxblat-1.1.9/src/pxblat/cli/client.py` & `pxblat-1.2.1/src/pxblat/cli/client.py`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/cli/fa2twobit.py` & `pxblat-1.2.1/src/pxblat/cli/fa2twobit.py`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/cli/server.py` & `pxblat-1.2.1/src/pxblat/cli/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,15 +254,24 @@
         try_new_port=False,
     )
 
 
 @server_app.command()
 def stop(host: str, port: int):
     """To remove a server."""
-    stop_server(host, port)
+    from rich.console import Console
+
+    console = Console()
+
+    try:
+        stop_server(host, port)
+    except ConnectionRefusedError:
+        console.print(f"[yellow]Server {host}:{port} may be not running")
+    else:
+        console.print(f"[green]Server {host}:{port} stopped")
 
 
 @server_app.command()
 def status(
     host: str,
     port: int,
     trans: bool = trans,
```

### Comparing `pxblat-1.1.9/src/pxblat/cli/twobit2fa.py` & `pxblat-1.2.1/src/pxblat/cli/twobit2fa.py`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/__init__.py` & `pxblat-1.2.1/src/pxblat/extc/__init__.py`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/__init__.pyi` & `pxblat-1.2.1/src/pxblat/extc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/binder/_extc.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/binder/_extc.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/binder/faToTwoBit.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/binder/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/binder/gfClient.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/binder/gfClient.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/binder/gfServer.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/binder/gfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/binder/gfServer_1.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/binder/gfServer_1.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/binder/pygfServer.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/binder/pygfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/binder/twoBitToFa.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/binder/twoBitToFa.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/bs_thread_pool.hpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/bs_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/dbg.h` & `pxblat-1.2.1/src/pxblat/extc/bindings/dbg.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/faToTwoBit.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/faToTwoBit.hpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/faToTwoBit.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/gfClient.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/gfClient.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/gfClient.hpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/gfClient.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/gfServer.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/gfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/gfServer.hpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/gfServer.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/pygfServer.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/pygfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/pygfServer.hpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/pygfServer.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/twoBitToFa.cpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/twoBitToFa.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/bindings/twoBitToFa.hpp` & `pxblat-1.2.1/src/pxblat/extc/bindings/twoBitToFa.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/blat.c` & `pxblat-1.2.1/src/pxblat/extc/blat.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/faToTwoBit.c` & `pxblat-1.2.1/src/pxblat/extc/faToTwoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/gfClient.c` & `pxblat-1.2.1/src/pxblat/extc/gfClient.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/gfServer.c` & `pxblat-1.2.1/src/pxblat/extc/gfServer.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/bandExt.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/bandExt.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/base64.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/base64.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/cheapcgi.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/cheapcgi.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/filePath.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/filePath.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/gfxPoly.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/gfxPoly.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/hex.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/hex.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/htmlPage.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/htmlPage.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/htmshell.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/htmshell.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/internet.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/internet.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/kxTok.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/kxTok.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/memgfx.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/memgfx.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/mime.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/mime.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/portimpl.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/portimpl.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/aux/rbTree.h` & `pxblat-1.2.1/src/pxblat/extc/include/aux/rbTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/aliType.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/aliType.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/asParse.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/asParse.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/axt.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/axt.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/bPlusTree.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/bPlusTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/basicBed.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/basicBed.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/binRange.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/binRange.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/bits.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/bits.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/chain.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/chain.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/chainBlock.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/chainBlock.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/common.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/common.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/dlist.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/dlist.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/dnaseq.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/dnaseq.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/dnautil.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/dnautil.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/dystring.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/dystring.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/errAbort.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/errAbort.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/errCatch.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/errCatch.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/fa.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/fa.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/fuzzyFind.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/fuzzyFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/genoFind.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/genoFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/gfClientLib.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/gfClientLib.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/gfInternal.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/gfInternal.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/hash.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/hash.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/htmlColor.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/htmlColor.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/linefile.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/linefile.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/localmem.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/localmem.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/maf.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/maf.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/memalloc.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/memalloc.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/net.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/net.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/netlib.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/netlib.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/nib.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/nib.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/obscure.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/obscure.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/ooc.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/ooc.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/options.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/options.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/patSpace.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/patSpace.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/pipeline.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/portable.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/portable.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/psl.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/psl.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/rangeTree.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/rangeTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/repMask.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/repMask.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/sig.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/sig.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/sqlList.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/sqlList.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/sqlNum.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/sqlNum.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/supStitch.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/supStitch.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/tokenizer.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/tokenizer.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/trans3.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/trans3.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/twoBit.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/twoBit.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/udc.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/udc.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/core/verbose.h` & `pxblat-1.2.1/src/pxblat/extc/include/core/verbose.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/include/net/log.h` & `pxblat-1.2.1/src/pxblat/extc/include/net/log.h`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/axt.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/axt.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/bandExt.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/bandExt.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/base64.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/base64.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/binRange.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/binRange.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/blastOut.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/blastOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/cheapcgi.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/cheapcgi.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/ffSeedExtend.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/ffSeedExtend.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/filePath.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/filePath.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/hex.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/hex.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/htmlPage.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/htmlPage.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/htmshell.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/htmshell.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/https.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/https.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/intExp.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/intExp.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/internet.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/internet.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/maf.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/maf.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/mafFromAxt.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/mafFromAxt.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/mime.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/mime.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/net.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/net.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/netlib.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/netlib.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/ooc.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/ooc.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/patSpace.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/patSpace.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/portimpl.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/portimpl.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/rangeTree.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/rangeTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/rbTree.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/rbTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/repMask.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/repMask.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/servBrcMcw.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/servBrcMcw.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/servCrunx.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/servCrunx.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/servcis.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/servcis.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/servmsII.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/servmsII.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/servpws.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/servpws.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/sqlList.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/sqlList.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/sqlNum.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/sqlNum.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/aux/wildcmp.c` & `pxblat-1.2.1/src/pxblat/extc/src/aux/wildcmp.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/aliType.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/aliType.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/asParse.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/asParse.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/bPlusTree.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/bPlusTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/basicBed.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/basicBed.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/bits.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/bits.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/chain.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/chain.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/chainBlock.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/chainBlock.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/common.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/common.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/dlist.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/dlist.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/dnaseq.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/dnaseq.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/dnautil.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/dnautil.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/dystring.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/dystring.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/errAbort.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/errAbort.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/errCatch.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/errCatch.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/fa.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/fa.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/ffAli.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/ffAli.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/ffAliHelp.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/ffAliHelp.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/ffScore.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/ffScore.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/fuzzyFind.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/fuzzyFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/genoFind.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/genoFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/gfBlatLib.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/gfBlatLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/gfClientLib.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/gfClientLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/gfInternal.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/gfInternal.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/gfOut.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/gfOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/hash.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/hash.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/htmlColor.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/htmlColor.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/kxTok.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/kxTok.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/linefile.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/linefile.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/localmem.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/localmem.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/memalloc.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/memalloc.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/nib.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/nib.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/obscure.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/obscure.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/options.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/options.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/osunix.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/osunix.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/pipeline.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/pipeline.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/psl.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/psl.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/servcl.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/servcl.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/supStitch.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/supStitch.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/tokenizer.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/tokenizer.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/trans3.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/trans3.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/twoBit.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/twoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/udc.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/udc.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/core/verbose.c` & `pxblat-1.2.1/src/pxblat/extc/src/core/verbose.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/net/gfNet.c` & `pxblat-1.2.1/src/pxblat/extc/src/net/gfNet.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/src/net/log.c` & `pxblat-1.2.1/src/pxblat/extc/src/net/log.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/extc/twoBitToFa.c` & `pxblat-1.2.1/src/pxblat/extc/twoBitToFa.c`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/parser.py` & `pxblat-1.2.1/src/pxblat/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,16 @@
         # handle the errors with helpful messages
         if format is None:
             raise ValueError("Format required (lower case string)") from None
 
         if not isinstance(format, str):
             raise TypeError("Need a string for the file format (lower case)") from None
         if format != format.lower():
-            raise ValueError("Format string %r should be lower case" % format) from None
+            msg = f"Format string {format!r} should be lower case"
+            raise ValueError(msg) from None
 
         msg = f"Unknown format {format!r}. Supported formats are {', '.join(mapping)}"
         raise ValueError(msg) from None
 
     else:
         return handle
 
@@ -93,15 +94,16 @@
         if format is None:
             msg = "Format required (lower case string)"
             raise ValueError(msg) from None
         if not isinstance(format, str):
             msg = "Need a string for the file format (lower case)"
             raise TypeError(msg) from None
         if format != format.lower():
-            raise ValueError("Format string %r should be lower case" % format) from None
+            msg = f"Format string {format!r} should be lower case"
+            raise ValueError(msg) from None
 
         msg = f"Unknown format {format!r}. Supported formats are {', '.join(mapping)}"
         raise ValueError(msg) from None
 
     else:
         return obj_info
 
@@ -129,23 +131,29 @@
         format = "psl"
 
     iterator = get_processor(format, _ITERATOR_MAP)
     handle = get_handle(format, _HANDLE_MAP)
     yield from iterator(handle(content), **kwargs)
 
 
-def read(content: str, format=None, **kwargs):
+def _assign_info_to_query_result(query_result):
+    query_result.version = "v.37x1"
+    return query_result
+
+
+def read(content: str, format=None, seqid=None, **kwargs):
     """Reads and returns the first query result from the given content.
 
     This function takes a string content and a format string, parses the content using the `parse` function,
     and returns the first query result. If no results are found, or if more than one result is found, it raises an error.
 
     Args:
         content (str): The string content to parse and read.
         format (str, optional): The format string indicating how to parse the content. If not provided, 'psl' format will be used. Defaults to None.
+        seqid (str, optional): The sequence identifier to verify the query results. If not provided, no filtering will be done. Defaults to None.
         **kwargs: Arbitrary keyword arguments to be passed to the `parse` function.
 
     Returns:
         query_result: The first query result found in the content.
 
     Raises:
         ValueError: If no query results are found in the content, or if more than one query result is found.
@@ -154,18 +162,30 @@
     query_results = parse(content, format, **kwargs)
     try:
         query_result = next(query_results)
     except StopIteration:
         msg = "No query results found in handle"
         raise ValueError(msg) from None
 
+    # WARN: the code is related to issue #244,
+    # the real result may be empty but server will return some "trash"
+    # lets ignore that as a temporary solution.
+    # Currently, we do not verify the query result from path
+    # <Yangyang Li yangyang.li@northwestern.edu>
+    if seqid is not None and query_result.id != seqid:
+        return None
+
+    _assign_info_to_query_result(query_result)
+
     try:
         next(query_results)
         msg = "More than one query result found in handle"
-        raise ValueError(msg)
+        # WARN: issue #244: It seems like the server will return some "trash",
+        # lets ignore that as a temporary solution  <02-06-24, Yangyang Li>
+        # not raise ValueError(msg)
     except StopIteration:
         pass
 
     return query_result
 
 
 def _psl2sam(psl: str, samfile: Path):
```

### Comparing `pxblat-1.1.9/src/pxblat/server/__init__.py` & `pxblat-1.2.1/src/pxblat/server/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Server module."""
+
 from .basic import (
+    build_index,
     check_port_in_use,
     check_port_open,
     files,
     find_free_port,
     server_query,
     start_server,
     start_server_mt,
@@ -38,8 +40,9 @@
     "start_server_mt_nb",
     "wait_server_ready",
     "find_free_port",
     "check_port_in_use",
     "copy_client_option",
     "Status",
     "Client",
+    "build_index",
 ]
```

### Comparing `pxblat-1.1.9/src/pxblat/server/basic.py` & `pxblat-1.2.1/src/pxblat/server/basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,15 @@
 import time
 import warnings
 from collections import Counter
 from multiprocessing import Process
 
 from deprecated import deprecated  # type: ignore
 
-from pxblat.extc import (
-    ServerOption,
-    UsageStats,
-    pygetFileList,
-    pyqueryServer,
-    pystartServer,
-    startServer,
-)
+from pxblat.extc import ServerOption, UsageStats, buildIndex, pygetFileList, pyqueryServer, pystartServer, startServer
 
 from .status import Status
 
 MAX_PORT = 65535
 
 
 def check_port_in_use(host: str, port: int, tries: int = 3) -> bool:
@@ -491,7 +484,25 @@
         try:
             if not check_port_in_use(host, port):
                 return port
         except OSError as e:
             raise e
     msg = f"Cannot find available port in range [{start}, {end}]"
     raise RuntimeError(msg)
+
+
+def build_index(
+    gfx_file: str,
+    seq_files: list[str],
+    options: ServerOption,
+):
+    """To generate a precomputed index.
+
+         gfServer index gfidx file(s)
+
+    where the files are .2bit or .nib format files.  Separate indexes are
+    be created for untranslated and translated queries.  These can be used
+    with a persistent server as with 'start -indexFile or a dynamic server.
+    They must follow the naming convention for for dynamic servers.
+    """
+    file_count = len(seq_files)
+    buildIndex(gfx_file, file_count, seq_files, options)
```

### Comparing `pxblat-1.1.9/src/pxblat/server/client.py` & `pxblat-1.2.1/src/pxblat/server/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,19 +126,14 @@
                 return None
         else:
             return ret
 
     return ret_decode
 
 
-def _assign_info_to_query_result(query_result):
-    query_result.version = "v.37x1"
-    return query_result
-
-
 def query_server(
     option: ClientOption,
     host: str | None = None,
     port: int | None = None,
     seqname: str | None = None,
     *,
     parse: bool = True,
@@ -159,43 +154,46 @@
     _resolve_host_port(option, host, port)
 
     fafile = None
     if not option.inName and not option.inSeq:
         msg = "inName and inSeq are both empty"
         raise ValueError(msg)
 
+    seqid = None
+
     if option.inSeq:
         with tempfile.NamedTemporaryFile(mode="w", delete=False) as fafile:
             seqname = fafile.name if seqname is None else seqname
-            fafile.write(f">{seqname}\n")
+            seqid = f"{option.inSeq[:5]}_{len(option.inSeq)}"
+            fafile.write(f">{seqid}\n")
             fafile.write(option.inSeq)
         option.inName = fafile.name
 
     ret = pygfClient(option)
 
     try:
         ret_decode = ret.decode().rsplit(",\n", 1)[0]  # type: ignore
     except UnicodeDecodeError:
         ret_decode = ret.decode("latin-1").rsplit(",\n", 1)[0]  # type: ignore
 
     if fafile is not None:
         Path(fafile.name).unlink()
 
-    if parse and ret_decode:
-        try:
-            res = read(ret_decode, "psl")
-        except ValueError as e:
-            if "No query results" in str(e):
-                return None
-        else:
-            if isinstance(res, str):
-                return _assign_info_to_query_result(read(res, "psl"))
-            return _assign_info_to_query_result(res)
+    if not parse:
+        return ret_decode
 
-    return ret_decode
+    try:
+        res = read(ret_decode, "psl", seqid=seqid)
+    except ValueError as e:
+        if "No query results" in str(e):
+            return None
+
+        raise e
+    else:
+        return res
 
 
 class ClientThread(Thread):
     """A class for managing client connections to a server in a separate thread.
 
     This class can be used to query a gfServer in a separate thread, and can optionally wait until the server is ready before
     sending a query. It can also parse the result of the query.
```

### Comparing `pxblat-1.1.9/src/pxblat/server/server.py` & `pxblat-1.2.1/src/pxblat/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,33 +393,33 @@
         """Returns True if the server is open, False otherwise.
 
         Returns:
             bool: True if the server is open, False otherwise.
         """
         return self._is_open
 
-    def wait_ready(self, timeout: int = 60, *, restart: bool = False):
+    def wait_ready(self, *, restart: bool = False):
         """Wait server ready in block mode.
 
         Args:
             timeout: Timeout for wait server ready.
             restart: If timeout, restart server and wait again.
 
         Raises:
             RuntimeError: If server is not opened by gfServer or the server takes longer time to be ready, the `wait_server_ready` may be timeout.
             If `restart` is True, the server will be restarted and wait again.
         """
         if not self._is_ready:
             try:
-                wait_server_ready(self.host, self.port, timeout, self.option)
+                wait_server_ready(self.host, self.port, self.timeout, self.option)
             except RuntimeError as e:
                 if restart and self.use_others:
                     self.use_others = False
                     self.start()
-                    self.wait_ready(timeout * 2, restart=restart)
+                    self.wait_ready(restart=restart)
                 else:
                     msg = f"Timeout for Waiting for {self.host} {self.port} server ready due to server is not opened by gfServer or need longer time to wait"
                     raise RuntimeError(
                         msg,
                     ) from e
             else:
                 self._is_ready = True
```

### Comparing `pxblat-1.1.9/src/pxblat/server/status.py` & `pxblat-1.2.1/src/pxblat/server/status.py`

 * *Files identical despite different names*

### Comparing `pxblat-1.1.9/src/pxblat/toolkit/__init__.py` & `pxblat-1.2.1/src/pxblat/toolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Toolkit functions for working with BLAT."""
+
 from __future__ import annotations
 
 from pathlib import Path
 
 from pxblat.extc import TwoBitToFaOption, faToTwoBit, twoBitToFa
 
 #     "Args",
```

### Comparing `pxblat-1.1.9/setup.py` & `pxblat-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 
 install_requires = \
 ['biopython>=1.81,<2.0',
  'deprecated>=1.2.13,<2.0.0',
  'loguru>=0.7.0,<0.8.0',
  'mashumaro>=3.7,<4.0',
  'pybind11>=2.10.4,<3.0.0',
- 'pysimdjson>=5.0.2,<6.0.0',
+ 'pysimdjson>=5.0.2,<7.0.0',
  'rich>=13.3.5,<14.0.0',
- 'setuptools>=68.2.2,<69.0.0',
- 'typer>=0.9.0,<0.10.0',
- 'urllib3==2.0.7']
+ 'setuptools>=68.2.2,<70.0.0',
+ 'typer>=0.9,<0.13',
+ 'urllib3==2.2.1']
 
 entry_points = \
 {'console_scripts': ['pxblat = pxblat.cli.cli:app']}
 
 setup_kwargs = {
     'name': 'pxblat',
-    'version': '1.1.9',
+    'version': '1.2.1',
     'description': 'A native python binding for blat suite',
     'long_description': '# <img src="https://raw.githubusercontent.com/cauliyang/pxblat/main/docs/_static/logo.png" alt="logo" height=100> **PxBLAT** [![social](https://img.shields.io/github/stars/cauliyang/pxblat?style=social)](https://github.com/cauliyang/pxblat/stargazers)\n\n_An Efficient and Ergonomic Python Binding Library for BLAT_\n\n[![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)](https://www.python.org/)\n[![c++](https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white)](https://en.cppreference.com/w/)\n[![c](https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black)](https://www.gnu.org/software/gnu-c-manual/)\n[![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)][pypi]\n[![conda](https://img.shields.io/conda/vn/bioconda/pxblat?style=for-the-badge)][conda]\n![Linux](https://img.shields.io/badge/-Linux-grey?logo=linux&style=for-the-badge)\n![macOS](https://img.shields.io/badge/-OSX-black?logo=apple&style=for-the-badge)\n[![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)][pypi]\n[![tests](https://img.shields.io/github/actions/workflow/status/cauliyang/pxblat/tests.yml?style=for-the-badge&logo=github&label=Tests)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)\n[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge)](https://app.codecov.io/gh/cauliyang/pxblat)\n[![docs](https://img.shields.io/readthedocs/pxblat?style=for-the-badge)](https://pxblat.readthedocs.io/en/latest/)\n[![download](https://img.shields.io/pypi/dm/pxblat?logo=pypi&label=pypi%20download&style=for-the-badge)][pypi]\n[![condadownload](https://img.shields.io/conda/dn/bioconda/pxblat?style=for-the-badge&logo=anaconda&label=Conda%20Download)][conda]\n[![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![ruff](https://img.shields.io/badge/code%20style-ruff-000000.svg?style=for-the-badge)](https://github.com/charliermarsh/ruff)\n[![release](https://img.shields.io/github/release-date/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/releases)\n[![open-issue](https://img.shields.io/github/issues-raw/cauliyang/pxblat?style=for-the-badge)][open-issue]\n[![close-issue](https://img.shields.io/github/issues-closed-raw/cauliyang/pxblat?style=for-the-badge)][close-issue]\n[![activity](https://img.shields.io/github/commit-activity/m/cauliyang/pxblat?style=for-the-badge)][repo]\n[![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)][repo]\n[![opull](https://img.shields.io/github/issues-pr-raw/cauliyang/pxblat?style=for-the-badge)][opull]\n[![all contributors](https://img.shields.io/github/all-contributors/cauliyang/pxblat?style=for-the-badge)](#contributors)\n\n<!-- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)][colab] -->\n\n[repo]: https://github.com/ylab-hi/pxblat\n[open-issue]: https://github.com/cauliyang/pxblat/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc\n[close-issue]: https://github.com/cauliyang/pxblat/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aclosed\n[opull]: https://github.com/cauliyang/pxblat/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc\n[conda]: https://bioconda.github.io/recipes/pxblat/README.html\n[pypi]: https://pypi.org/project/pxblat/\n[colab]: https://colab.research.google.com/drive/1TXb9GBmYa2EYezwBKbD-y9Xg6MC2gL36\n\n## Why PxBLAT?\n\nWhen conducting extensive queries, using the `blat` of `BLAT` suite can prove to be quite inefficient, especially if these operations aren\'t grouped. The tasks are allocated sporadically, often interspersed among other tasks.\nIn general, the choice narrows down to either utilizing `blat` or combining `gfServer` with `gfClient`.\nIndeed, `blat` is a program that launches `gfServer`, conducts the sequence query via `gfClient`, and then proceeds to terminate the server.\n\nThis approach is far from ideal when performing numerous queries that aren\'t grouped since `blat` repeatedly initializes and shuts down `gfServer` for each query, resulting in substantial overhead.\nThis overhead consists of the time required for the server to index the reference, contingent on the reference\'s size.\nTo index the human genome (hg38), for example, would take approximately five minutes.\n\nA more efficient solution would involve initializing `gfServer` once and invoking `gfClient` multiple times for the queries.\nHowever, `gfServer` and `gfClient` are only accessible via the command line.\nThis necessitates managing system calls (for instance, `subprocess` or `os.system`), intermediate temporary files, and format conversion, further diminishing performance.\n\nThat is why `PxBLAT` holds its position.\nIt resolves the issues mentioned above while introducing handy features like `port retry`, `use current running server`, etc.\n\n## 📚 **Table of Contents**\n\n- [ **PxBLAT** ](#-pxblat-)\n  - [📚 **Table of Contents**](#-table-of-contents)\n  - [🔮 **Features**](#-features)\n  - [📎 **Citation**](#-citation)\n  - [🚀 **Getting Started**](#-getting-started)\n  - [🤝 **Contributing**](#-contributing)\n  - [\U0001faaa **License**](#-license)\n  - [🤗 **Contributors**](#contributors)\n  - [🙏 **Acknowledgments**](#-acknowledgments)\n\n## 🔮 **Features**\n\n- **Zero System Calls**: Avoids system calls, leading to a smoother, quicker operation.<br>\n- **Ergonomics**: With an ergonomic design, `PxBLAT` aims for a seamless user experience.<br>\n- **No External Dependencies**: `PxBLAT` operates independently without any external dependencies.<br>\n- **Self-Monitoring**: No need to trawl through log files; `PxBLAT` monitors its status internally.<br>\n- **Robust Validation**: Extensively tested to ensure reliable performance and superior stability as BLAT.<br>\n- **Format-Agnostic:** `PxBLAT` doesn\'t require you to worry about file formats.<br>\n- **In-Memory Processing**: `PxBLAT` discards the need for intermediate files by doing all its operations in memory, ensuring speed and efficiency.<br>\n\n## 📎 **Citation**\n\nPxBLAT is scientific software, with a published paper in the BioRxiv.\nCheck the [published](https://www.biorxiv.org/content/10.1101/2023.08.02.551686v2) to read the paper.\n\n```bibtex\n@article {Li2023pxblat,\n\tauthor = {Yangyang Li and Rendong Yang},\n\ttitle = {PxBLAT: An Ergonomic and Efficient Python Binding Library for BLAT},\n\telocation-id = {2023.08.02.551686},\n\tyear = {2023},\n\tdoi = {10.1101/2023.08.02.551686},\n\tpublisher = {Cold Spring Harbor Laboratory},\n\turl = {https://www.biorxiv.org/content/10.1101/2023.08.02.551686v2},\n\tjournal = {bioRxiv}\n}\n```\n\n## 🚀 **Getting Started**\n\nWelcome to PxBLAT! To kickstart your journey and get the most out of this tool, we have prepared a comprehensive [documentation](https://pxblat.readthedocs.io/en/latest/installation.html).\nInside, you’ll find detailed guides, examples, and all the necessary information to help you navigate and utilize PxBLAT effectively.\n\n### Need Help or Found an Issue?\n\nIf you encounter any issues or if something is not clear in the documentation, do not hesitate to [open an issue](https://github.com/ylab-hi/pxblat/issues/new/choose).\nWe are here to help and appreciate your feedback for improving PxBLAT.\n\n### Show Your Support\n\nIf PxBLAT has been beneficial to your projects or you appreciate the work put into it, consider leaving a ⭐️ [Star](https://github.com/ylab-hi/pxblat/stargazers) on our GitHub repository.\nYour support means the world to us and motivates us to continue enhancing PxBLAT.\n\nLet’s embark on this journey together and make the most out of PxBLAT! 🎉\nPlease see the [document](https://pxblat.readthedocs.io/en/latest/installation.html) for details and more examples.\n\n## 🤝 **Contributing**\n\nContributions are always welcome! Please follow these steps:\n\n1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.\n2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.\n3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).\n\n```bash\ngit checkout -b new-feature-branch\n```\n\n4. Take changes to the project\'s codebase.\n5. Install the latest package\n\n```bash\npoetry install\n```\n\n6. Test your changes\n\n```bash\npytest -vlsx tests\n```\n\n7. Commit your changes to your local branch with a clear commit message that explains the changes you\'ve made.\n\n```bash\ngit commit -m \'Implemented new feature.\'\n```\n\n8. Push your changes to your forked repository on GitHub using the following command\n\n```bash\ngit push origin new-feature-branch\n```\n\nCreate a pull request to the original repository.\nOpen a new pull request to the original project repository. In the pull request, describe the changes you\'ve made and why they\'re necessary.\nThe project maintainers will review your changes and provide feedback or merge them into the main branch.\n\n## \U0001faaa **License**\n\n**PxBLAT is modified from blat, the license is the same as blat. The source code and\nexecutables are freely available for academic, nonprofit, and personal use.\nCommercial licensing information is available on the Kent Informatics website\n(https://kentinformatics.com/).**\n\n## **Contributors**\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://yangyangli.top"><img src="https://avatars.githubusercontent.com/u/38903141?v=4?s=100" width="100px;" alt="yangliz5"/><br /><sub><b>yangliz5</b></sub></a><br /><a href="#maintenance-cauliyang" title="Maintenance">🚧</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mencian"><img src="https://avatars.githubusercontent.com/u/71105179?v=4?s=100" width="100px;" alt="Joshua Zhuang"/><br /><sub><b>Joshua Zhuang</b></sub></a><br /><a href="#infra-mencian" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\n## 🙏 **Acknowledgments**\n\n- [BLAT](http://genome.ucsc.edu/goldenPath/help/blatSpec.html)\n- [UCSC](https://github.com/ucscGenomeBrowser/kent)\n- [pybind11](https://github.com/pybind/pybind11/tree/stable)\n\n<!-- github-only -->\n\n<br>\n<picture>\n  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=cauliyang/pxblat&type=Date&theme=light" />\n  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=cauliyang/pxblat&type=Date" />\n  <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=cauliyang/pxblat&type=Date" />\n</picture>\n',
     'author': 'Yangyang Li',
     'author_email': 'yangyang.li@northwestern.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ylab-hi/pxblat',
```

### Comparing `pxblat-1.1.9/PKG-INFO` & `pxblat-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxblat
-Version: 1.1.9
+Version: 1.2.1
 Summary: A native python binding for blat suite
 Home-page: https://github.com/ylab-hi/pxblat
 License: LICENSE
 Keywords: bioinformatics,sequence aligner,blat
 Author: Yangyang Li
 Author-email: yangyang.li@northwestern.edu
 Requires-Python: >=3.9,<3.12
@@ -20,19 +20,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: biopython (>=1.81,<2.0)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mashumaro (>=3.7,<4.0)
 Requires-Dist: pybind11 (>=2.10.4,<3.0.0)
-Requires-Dist: pysimdjson (>=5.0.2,<6.0.0)
+Requires-Dist: pysimdjson (>=5.0.2,<7.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
-Requires-Dist: setuptools (>=68.2.2,<69.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: urllib3 (==2.0.7)
+Requires-Dist: setuptools (>=68.2.2,<70.0.0)
+Requires-Dist: typer (>=0.9,<0.13)
+Requires-Dist: urllib3 (==2.2.1)
 Project-URL: Documentation, https://pxblat.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ylab-hi/pxblat
 Description-Content-Type: text/markdown
 
 # <img src="https://raw.githubusercontent.com/cauliyang/pxblat/main/docs/_static/logo.png" alt="logo" height=100> **PxBLAT** [![social](https://img.shields.io/github/stars/cauliyang/pxblat?style=social)](https://github.com/cauliyang/pxblat/stargazers)
 
 _An Efficient and Ergonomic Python Binding Library for BLAT_
```

